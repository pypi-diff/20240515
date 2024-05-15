# Comparing `tmp/criteo_api_retailmedia_sdk-2024.1.0.240515.tar.gz` & `tmp/criteo_api_retailmedia_sdk-2024.4.0.240515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo_api_retailmedia_sdk-2024.1.0.240515.tar", last modified: Wed May 15 14:51:59 2024, max compression
+gzip compressed data, was "criteo_api_retailmedia_sdk-2024.4.0.240515.tar", last modified: Wed May 15 14:52:03 2024, max compression
```

## Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515.tar` & `criteo_api_retailmedia_sdk-2024.4.0.240515.tar`

### file list

```diff
@@ -1,251 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.130691 criteo_api_retailmedia_sdk-2024.1.0.240515/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-15 14:51:59.130691 criteo_api_retailmedia_sdk-2024.1.0.240515/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.130691 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-15 14:51:59.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-05-15 14:51:59.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:51:59.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:51:59.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:51:59.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.082691 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.086691 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26445 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   421608 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39276 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.086691 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/flow_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.130691 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_funds_to_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keyword_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_to_basket_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/approval_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/asset_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/asset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19634 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_campaigns_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_line_items_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_line_items_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_line_items_report_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_report_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    23198 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_revenue_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_revenue_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_revenue_report_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_create_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_update_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/audience_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/audience_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/audience_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_response_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_daily_budget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_monthly_budget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    18708 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/category202204.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/category202204_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/change_dates_of_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/choice_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/choice_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/choice_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/color_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/create_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12806 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202110_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202210.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202210_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202210_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative_create_model202207.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative_update_model202207.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/daily_line_item_budget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/editable_campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_add_funds_to_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_change_dates_of_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_create_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_line_item_capping202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_line_item_page202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_line_item_page_category202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    16309 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    15046 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_retailer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_retailer_pages202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_update_balance_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/files_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/files_variables_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/hyperlink_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/input_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/input_resource_of_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/input_resource_of_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_retailer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_request_of_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keyword_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keyword_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keyword_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keywords_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/match_type_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/monthly_line_item_budeget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/negotiation_state_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/page_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/page_type_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/post_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item_create_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/promoted_product202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/promoted_product202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/proposal_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/proposal_status_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/proposal_status_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/put_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/report_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_add_funds_to_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_balance_campaign202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_category202204.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_change_dates_of_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_create_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_creative202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_creative202210.py
--rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_update_balance_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/review_state_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_create_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_customer_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13142 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_create_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14553 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rmca_common_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/section.py
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bids_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bids_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bids_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/status_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/store_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/store_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/store_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/text_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/text_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/update_balance_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_of_campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_of_line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12114 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    82565 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.130691 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/models/
--rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 14:51:59.130691 criteo_api_retailmedia_sdk-2024.1.0.240515/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:51:59.130691 criteo_api_retailmedia_sdk-2024.1.0.240515/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.1.0.240515/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.934690 criteo_api_retailmedia_sdk-2024.4.0.240515/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-15 14:52:03.934690 criteo_api_retailmedia_sdk-2024.4.0.240515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19295 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.934690 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-15 14:52:03.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-05-15 14:52:03.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:52:03.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:52:03.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 14:52:03.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.882691 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.886690 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18826 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26445 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   428555 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39191 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.886690 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.930690 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_funds_to_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keyword_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_to_basket_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_to_basket_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_to_basket_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/approval_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/asset_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19634 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_campaigns_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_campaigns_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_campaigns_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_line_items_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_line_items_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_line_items_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23198 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_revenue_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_revenue_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_revenue_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_create_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_update_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/audience_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/audience_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/audience_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/balance_campaign202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/balance_campaign202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/balance_response_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_daily_budget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_monthly_budget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18708 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/category202204.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/category202204_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/change_dates_of_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/change_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/choice_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/choice_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/choice_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/color_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/create_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12806 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202110_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202210_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202210_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative_create_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative_update_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/daily_line_item_budget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/editable_campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_add_funds_to_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_change_dates_of_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_create_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_line_item_capping202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_line_item_page202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_line_item_page_category202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16309 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15046 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_retailer_pages202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_update_balance_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/files_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/files_variables_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/hyperlink_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/input_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/input_resource_of_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/input_resource_of_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/insertion_order_history_change_data_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_request_of_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keyword_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keyword_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keyword_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keywords_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/match_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/monthly_line_item_budeget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/negotiation_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/page_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/page_of_insertion_order_history_change_data_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/page_type_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/post_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item_create_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/promoted_product202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/promoted_product202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/proposal_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/proposal_status_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/proposal_status_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/put_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/report_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_add_funds_to_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_balance_campaign202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_category202204.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_change_dates_of_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_create_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_retail_media_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_update_balance_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_outcome_of_retail_media_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13802 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/retail_media_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/retail_media_brand_account_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/retail_media_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/review_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_input_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_input_entity_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_user_behavior_create_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_user_behavior_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_customer_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13142 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_create_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14553 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rmca_common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bids_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bids_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11768 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bids_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/status_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/store_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/store_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/store_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/text_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/text_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/update_balance_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_input_of_campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_input_of_line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_input_of_retail_media_brand_account_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_input_of_retail_media_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_of_campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_of_line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11780 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_of_retail_media_brand_account_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_of_retail_media_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_outcome_of_campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_outcome_of_line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12114 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82565 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.934690 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    25924 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 14:52:03.934690 criteo_api_retailmedia_sdk-2024.4.0.240515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:52:03.934690 criteo_api_retailmedia_sdk-2024.4.0.240515/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-15 14:51:12.000000 criteo_api_retailmedia_sdk-2024.4.0.240515/test/test_gateway_api.py
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/PKG-INFO` & `criteo_api_retailmedia_sdk-2024.4.0.240515/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240515
+pip install criteo-api-retailmedia-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2024_01
+import criteo_api_retailmedia_v2024_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/README.md` & `criteo_api_retailmedia_sdk-2024.4.0.240515/README.md`

 * *Files 3% similar despite different names*

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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240515
+pip install criteo-api-retailmedia-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2024_01
+import criteo_api_retailmedia_v2024_04
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
 
 Download the code or clone the repository locally, then execute the following command:
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2024_01
+import criteo_api_retailmedia_v2024_04
 ```
 
 ## Example
 There are multiple examples for the different OAuth flows that the SDK supports.
 - See [test/example_application_with_client_credentials.py](test/example_application_with_client_credentials.py) for an example with Client Credentials.
 - See [test/example_application_with_auth_code.py](test/example_application_with_auth_code.py) for an example with Authorization Code.
 Once you follow the authorization code flow, you will have a refresh token that has to be used to regenerate access token for future usage. 
@@ -100,14 +100,15 @@
  - [CampaignBudgetOverrides](docs/CampaignBudgetOverrides.md)
  - [CampaignDailyBudgetOverride](docs/CampaignDailyBudgetOverride.md)
  - [CampaignMonthlyBudgetOverride](docs/CampaignMonthlyBudgetOverride.md)
  - [CampaignV202301](docs/CampaignV202301.md)
  - [Category202204](docs/Category202204.md)
  - [Category202204ListResponse](docs/Category202204ListResponse.md)
  - [ChangeDatesOfBalanceRequest](docs/ChangeDatesOfBalanceRequest.md)
+ - [ChangeDetails](docs/ChangeDetails.md)
  - [ChoiceOption](docs/ChoiceOption.md)
  - [ChoiceVariableSpecification](docs/ChoiceVariableSpecification.md)
  - [ChoiceVariableValue](docs/ChoiceVariableValue.md)
  - [ColorVariableValue](docs/ColorVariableValue.md)
  - [CommonError](docs/CommonError.md)
  - [CommonLineItemPagedListResponse](docs/CommonLineItemPagedListResponse.md)
  - [CommonLineItemResponse](docs/CommonLineItemResponse.md)
@@ -154,14 +155,15 @@
  - [ExternalUpdateBalanceModel](docs/ExternalUpdateBalanceModel.md)
  - [FilesVariableValue](docs/FilesVariableValue.md)
  - [FilesVariablesSpecification](docs/FilesVariablesSpecification.md)
  - [HyperlinkVariableValue](docs/HyperlinkVariableValue.md)
  - [InputKeywordsModel](docs/InputKeywordsModel.md)
  - [InputResourceOfAuctionLineItemCreateModel](docs/InputResourceOfAuctionLineItemCreateModel.md)
  - [InputResourceOfPreferredLineItemCreateModel202110](docs/InputResourceOfPreferredLineItemCreateModel202110.md)
+ - [InsertionOrderHistoryChangeDataCapture](docs/InsertionOrderHistoryChangeDataCapture.md)
  - [JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301](docs/JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301.md)
  - [JsonApiBodyWithIdOfInt64AndAccountAndAccount](docs/JsonApiBodyWithIdOfInt64AndAccountAndAccount.md)
  - [JsonApiBodyWithIdOfInt64AndBrandAndBrand](docs/JsonApiBodyWithIdOfInt64AndBrandAndBrand.md)
  - [JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301](docs/JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301.md)
  - [JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus](docs/JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus.md)
  - [JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers](docs/JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers.md)
  - [JsonApiBodyWithIdOfInt64AndRetailerAndRetailer](docs/JsonApiBodyWithIdOfInt64AndRetailerAndRetailer.md)
@@ -182,17 +184,19 @@
  - [KeywordsModelResource](docs/KeywordsModelResource.md)
  - [KeywordsModelResponse](docs/KeywordsModelResponse.md)
  - [LineItemBidMultipliers](docs/LineItemBidMultipliers.md)
  - [LineItemBidMultipliersRequest](docs/LineItemBidMultipliersRequest.md)
  - [LineItemBidMultipliersResponse](docs/LineItemBidMultipliersResponse.md)
  - [LineItemBudgetOverrides](docs/LineItemBudgetOverrides.md)
  - [MatchTypeModel](docs/MatchTypeModel.md)
+ - [Metadata](docs/Metadata.md)
  - [MonthlyLineItemBudegetOverride](docs/MonthlyLineItemBudegetOverride.md)
  - [NegotiationStateModel](docs/NegotiationStateModel.md)
  - [PageMetadata](docs/PageMetadata.md)
+ - [PageOfInsertionOrderHistoryChangeDataCapture](docs/PageOfInsertionOrderHistoryChangeDataCapture.md)
  - [PageTypeEnvironment](docs/PageTypeEnvironment.md)
  - [PostCampaignV202301](docs/PostCampaignV202301.md)
  - [PreferredLineItem202110PagedListResponse](docs/PreferredLineItem202110PagedListResponse.md)
  - [PreferredLineItem202110Response](docs/PreferredLineItem202110Response.md)
  - [PreferredLineItemCreateModel202110Request](docs/PreferredLineItemCreateModel202110Request.md)
  - [PreferredLineItemUpdateModel202110Request](docs/PreferredLineItemUpdateModel202110Request.md)
  - [ProblemDetails](docs/ProblemDetails.md)
@@ -214,17 +218,22 @@
  - [ResourceOfCreateBalance](docs/ResourceOfCreateBalance.md)
  - [ResourceOfCreative202110](docs/ResourceOfCreative202110.md)
  - [ResourceOfCreative202210](docs/ResourceOfCreative202210.md)
  - [ResourceOfLineItemBidMultipliers](docs/ResourceOfLineItemBidMultipliers.md)
  - [ResourceOfPreferredLineItem202110](docs/ResourceOfPreferredLineItem202110.md)
  - [ResourceOfPreferredLineItemUpdateModel202110](docs/ResourceOfPreferredLineItemUpdateModel202110.md)
  - [ResourceOfPromotedProduct202110](docs/ResourceOfPromotedProduct202110.md)
+ - [ResourceOfRetailMediaAccount](docs/ResourceOfRetailMediaAccount.md)
  - [ResourceOfTemplate](docs/ResourceOfTemplate.md)
  - [ResourceOfUpdateBalanceModel](docs/ResourceOfUpdateBalanceModel.md)
  - [ResourceOutcome](docs/ResourceOutcome.md)
+ - [ResourceOutcomeOfRetailMediaAccount](docs/ResourceOutcomeOfRetailMediaAccount.md)
+ - [RetailMediaAccount](docs/RetailMediaAccount.md)
+ - [RetailMediaBrandAccountCreation](docs/RetailMediaBrandAccountCreation.md)
+ - [RetailMediaBrands](docs/RetailMediaBrands.md)
  - [ReviewStateModel](docs/ReviewStateModel.md)
  - [RmLegacyAudienceCreateEntityV1](docs/RmLegacyAudienceCreateEntityV1.md)
  - [RmLegacyAudienceCreateEntityV1Resource](docs/RmLegacyAudienceCreateEntityV1Resource.md)
  - [RmLegacyAudienceCreateEntityV1Response](docs/RmLegacyAudienceCreateEntityV1Response.md)
  - [RmLegacyAudienceCreateEntityV2](docs/RmLegacyAudienceCreateEntityV2.md)
  - [RmLegacyAudienceCreateEntityV2Resource](docs/RmLegacyAudienceCreateEntityV2Resource.md)
  - [RmLegacyAudienceCreateEntityV2Response](docs/RmLegacyAudienceCreateEntityV2Response.md)
@@ -259,16 +268,20 @@
  - [TemplateVariable](docs/TemplateVariable.md)
  - [TemplateVariableValue](docs/TemplateVariableValue.md)
  - [TextVariableSpecification](docs/TextVariableSpecification.md)
  - [TextVariableValue](docs/TextVariableValue.md)
  - [UpdateBalanceModelRequest](docs/UpdateBalanceModelRequest.md)
  - [ValueResourceInputOfCampaignBudgetOverrides](docs/ValueResourceInputOfCampaignBudgetOverrides.md)
  - [ValueResourceInputOfLineItemBudgetOverrides](docs/ValueResourceInputOfLineItemBudgetOverrides.md)
+ - [ValueResourceInputOfRetailMediaBrandAccountCreation](docs/ValueResourceInputOfRetailMediaBrandAccountCreation.md)
+ - [ValueResourceInputOfRetailMediaBrands](docs/ValueResourceInputOfRetailMediaBrands.md)
  - [ValueResourceOfCampaignBudgetOverrides](docs/ValueResourceOfCampaignBudgetOverrides.md)
  - [ValueResourceOfLineItemBudgetOverrides](docs/ValueResourceOfLineItemBudgetOverrides.md)
+ - [ValueResourceOfRetailMediaBrandAccountCreation](docs/ValueResourceOfRetailMediaBrandAccountCreation.md)
+ - [ValueResourceOfRetailMediaBrands](docs/ValueResourceOfRetailMediaBrands.md)
  - [ValueResourceOutcomeOfCampaignBudgetOverrides](docs/ValueResourceOutcomeOfCampaignBudgetOverrides.md)
  - [ValueResourceOutcomeOfLineItemBudgetOverrides](docs/ValueResourceOutcomeOfLineItemBudgetOverrides.md)
  - [ValueTypeResourceOfAddToBasketIdsUpdateModel202110](docs/ValueTypeResourceOfAddToBasketIdsUpdateModel202110.md)
  - [ValueTypeResourceOfAddToBasketTarget202110](docs/ValueTypeResourceOfAddToBasketTarget202110.md)
  - [ValueTypeResourceOfAudienceIdsUpdateModel202110](docs/ValueTypeResourceOfAudienceIdsUpdateModel202110.md)
  - [ValueTypeResourceOfAudienceTarget202110](docs/ValueTypeResourceOfAudienceTarget202110.md)
  - [ValueTypeResourceOfKeywordTarget202110](docs/ValueTypeResourceOfKeywordTarget202110.md)
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/PKG-INFO` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240515
+pip install criteo-api-retailmedia-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2024_01
+import criteo_api_retailmedia_v2024_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,241 +2,255 @@
 setup.cfg
 setup.py
 criteo_api_retailmedia_sdk.egg-info/PKG-INFO
 criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
 criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
 criteo_api_retailmedia_sdk.egg-info/requires.txt
 criteo_api_retailmedia_sdk.egg-info/top_level.txt
-criteo_api_retailmedia_v2024_01/__init__.py
-criteo_api_retailmedia_v2024_01/api_client.py
-criteo_api_retailmedia_v2024_01/api_client_builder.py
-criteo_api_retailmedia_v2024_01/configuration.py
-criteo_api_retailmedia_v2024_01/criteo_api_client.py
-criteo_api_retailmedia_v2024_01/criteo_auth.py
-criteo_api_retailmedia_v2024_01/criteo_rest.py
-criteo_api_retailmedia_v2024_01/exceptions.py
-criteo_api_retailmedia_v2024_01/flow_constants.py
-criteo_api_retailmedia_v2024_01/model_utils.py
-criteo_api_retailmedia_v2024_01/rest.py
-criteo_api_retailmedia_v2024_01/api/__init__.py
-criteo_api_retailmedia_v2024_01/api/analytics_api.py
-criteo_api_retailmedia_v2024_01/api/audience_api.py
-criteo_api_retailmedia_v2024_01/api/campaign_api.py
-criteo_api_retailmedia_v2024_01/api/gateway_api.py
-criteo_api_retailmedia_v2024_01/apis/__init__.py
-criteo_api_retailmedia_v2024_01/model/__init__.py
-criteo_api_retailmedia_v2024_01/model/add_funds_to_balance_request.py
-criteo_api_retailmedia_v2024_01/model/add_remove_keyword_model.py
-criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model.py
-criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model_request.py
-criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model_resource.py
-criteo_api_retailmedia_v2024_01/model/add_to_basket_ids_update_model202110_request.py
-criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_request.py
-criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_response.py
-criteo_api_retailmedia_v2024_01/model/application_summary_model.py
-criteo_api_retailmedia_v2024_01/model/application_summary_model_resource.py
-criteo_api_retailmedia_v2024_01/model/application_summary_model_response.py
-criteo_api_retailmedia_v2024_01/model/approval_status_model.py
-criteo_api_retailmedia_v2024_01/model/asset.py
-criteo_api_retailmedia_v2024_01/model/asset_resource.py
-criteo_api_retailmedia_v2024_01/model/asset_response.py
-criteo_api_retailmedia_v2024_01/model/async_campaigns_report.py
-criteo_api_retailmedia_v2024_01/model/async_campaigns_report_request.py
-criteo_api_retailmedia_v2024_01/model/async_campaigns_report_resource.py
-criteo_api_retailmedia_v2024_01/model/async_line_items_report.py
-criteo_api_retailmedia_v2024_01/model/async_line_items_report_request.py
-criteo_api_retailmedia_v2024_01/model/async_line_items_report_resource.py
-criteo_api_retailmedia_v2024_01/model/async_report_response.py
-criteo_api_retailmedia_v2024_01/model/async_revenue_report.py
-criteo_api_retailmedia_v2024_01/model/async_revenue_report_request.py
-criteo_api_retailmedia_v2024_01/model/async_revenue_report_resource.py
-criteo_api_retailmedia_v2024_01/model/auction_line_item_create_model_request.py
-criteo_api_retailmedia_v2024_01/model/auction_line_item_paged_list_response.py
-criteo_api_retailmedia_v2024_01/model/auction_line_item_response.py
-criteo_api_retailmedia_v2024_01/model/auction_line_item_update_model_request.py
-criteo_api_retailmedia_v2024_01/model/audience_ids_update_model202110_request.py
-criteo_api_retailmedia_v2024_01/model/audience_target202110_request.py
-criteo_api_retailmedia_v2024_01/model/audience_target202110_response.py
-criteo_api_retailmedia_v2024_01/model/balance_campaign202110_list_request.py
-criteo_api_retailmedia_v2024_01/model/balance_campaign202110_paged_list_response.py
-criteo_api_retailmedia_v2024_01/model/balance_response.py
-criteo_api_retailmedia_v2024_01/model/balance_response_paged_list_response.py
-criteo_api_retailmedia_v2024_01/model/campaign_attributes_v202301.py
-criteo_api_retailmedia_v2024_01/model/campaign_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/campaign_daily_budget_override.py
-criteo_api_retailmedia_v2024_01/model/campaign_monthly_budget_override.py
-criteo_api_retailmedia_v2024_01/model/campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/category202204.py
-criteo_api_retailmedia_v2024_01/model/category202204_list_response.py
-criteo_api_retailmedia_v2024_01/model/change_dates_of_balance_request.py
-criteo_api_retailmedia_v2024_01/model/choice_option.py
-criteo_api_retailmedia_v2024_01/model/choice_variable_specification.py
-criteo_api_retailmedia_v2024_01/model/choice_variable_value.py
-criteo_api_retailmedia_v2024_01/model/color_variable_value.py
-criteo_api_retailmedia_v2024_01/model/common_error.py
-criteo_api_retailmedia_v2024_01/model/common_line_item_paged_list_response.py
-criteo_api_retailmedia_v2024_01/model/common_line_item_response.py
-criteo_api_retailmedia_v2024_01/model/common_problem.py
-criteo_api_retailmedia_v2024_01/model/common_warning.py
-criteo_api_retailmedia_v2024_01/model/create_balance_request.py
-criteo_api_retailmedia_v2024_01/model/creative202110.py
-criteo_api_retailmedia_v2024_01/model/creative202110_list_response.py
-criteo_api_retailmedia_v2024_01/model/creative202210.py
-criteo_api_retailmedia_v2024_01/model/creative202210_list_response.py
-criteo_api_retailmedia_v2024_01/model/creative202210_response.py
-criteo_api_retailmedia_v2024_01/model/creative_create_model202207.py
-criteo_api_retailmedia_v2024_01/model/creative_update_model202207.py
-criteo_api_retailmedia_v2024_01/model/daily_line_item_budget_override.py
-criteo_api_retailmedia_v2024_01/model/editable_campaign_attributes_v202301.py
-criteo_api_retailmedia_v2024_01/model/external_account.py
-criteo_api_retailmedia_v2024_01/model/external_add_funds_to_balance.py
-criteo_api_retailmedia_v2024_01/model/external_add_to_basket_ids_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/external_add_to_basket_target202110.py
-criteo_api_retailmedia_v2024_01/model/external_auction_line_item.py
-criteo_api_retailmedia_v2024_01/model/external_auction_line_item_create_model.py
-criteo_api_retailmedia_v2024_01/model/external_auction_line_item_update_model.py
-criteo_api_retailmedia_v2024_01/model/external_audience_ids_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/external_audience_target202110.py
-criteo_api_retailmedia_v2024_01/model/external_balance_response.py
-criteo_api_retailmedia_v2024_01/model/external_brand.py
-criteo_api_retailmedia_v2024_01/model/external_catalog_request.py
-criteo_api_retailmedia_v2024_01/model/external_catalog_status.py
-criteo_api_retailmedia_v2024_01/model/external_change_dates_of_balance.py
-criteo_api_retailmedia_v2024_01/model/external_common_line_item.py
-criteo_api_retailmedia_v2024_01/model/external_create_balance.py
-criteo_api_retailmedia_v2024_01/model/external_keyword_target202110.py
-criteo_api_retailmedia_v2024_01/model/external_line_item_capping202110.py
-criteo_api_retailmedia_v2024_01/model/external_line_item_page202110.py
-criteo_api_retailmedia_v2024_01/model/external_line_item_page_category202110.py
-criteo_api_retailmedia_v2024_01/model/external_preferred_line_item202110.py
-criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_create_model202110.py
-criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/external_promoted_product202110.py
-criteo_api_retailmedia_v2024_01/model/external_retailer.py
-criteo_api_retailmedia_v2024_01/model/external_retailer_pages202110.py
-criteo_api_retailmedia_v2024_01/model/external_store_ids_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/external_store_target202110.py
-criteo_api_retailmedia_v2024_01/model/external_update_balance_model.py
-criteo_api_retailmedia_v2024_01/model/files_variable_value.py
-criteo_api_retailmedia_v2024_01/model/files_variables_specification.py
-criteo_api_retailmedia_v2024_01/model/hyperlink_variable_value.py
-criteo_api_retailmedia_v2024_01/model/input_keywords_model.py
-criteo_api_retailmedia_v2024_01/model/input_resource_of_auction_line_item_create_model.py
-criteo_api_retailmedia_v2024_01/model/input_resource_of_preferred_line_item_create_model202110.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
-criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_account.py
-criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_brand.py
-criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_retailer.py
-criteo_api_retailmedia_v2024_01/model/json_api_request_of_catalog_request.py
-criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_catalog_status.py
-criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2024_01/model/keyword_data_model.py
-criteo_api_retailmedia_v2024_01/model/keyword_target202110_request.py
-criteo_api_retailmedia_v2024_01/model/keyword_target202110_response.py
-criteo_api_retailmedia_v2024_01/model/keywords_model.py
-criteo_api_retailmedia_v2024_01/model/keywords_model_resource.py
-criteo_api_retailmedia_v2024_01/model/keywords_model_response.py
-criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers.py
-criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_request.py
-criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_response.py
-criteo_api_retailmedia_v2024_01/model/line_item_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/match_type_model.py
-criteo_api_retailmedia_v2024_01/model/monthly_line_item_budeget_override.py
-criteo_api_retailmedia_v2024_01/model/negotiation_state_model.py
-criteo_api_retailmedia_v2024_01/model/page_metadata.py
-criteo_api_retailmedia_v2024_01/model/page_type_environment.py
-criteo_api_retailmedia_v2024_01/model/post_campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_paged_list_response.py
-criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_response.py
-criteo_api_retailmedia_v2024_01/model/preferred_line_item_create_model202110_request.py
-criteo_api_retailmedia_v2024_01/model/preferred_line_item_update_model202110_request.py
-criteo_api_retailmedia_v2024_01/model/problem_details.py
-criteo_api_retailmedia_v2024_01/model/promoted_product202110_list_request.py
-criteo_api_retailmedia_v2024_01/model/promoted_product202110_paged_list_response.py
-criteo_api_retailmedia_v2024_01/model/proposal_status_model.py
-criteo_api_retailmedia_v2024_01/model/proposal_status_model_resource.py
-criteo_api_retailmedia_v2024_01/model/proposal_status_model_response.py
-criteo_api_retailmedia_v2024_01/model/put_campaign_v202301.py
-criteo_api_retailmedia_v2024_01/model/report_outcome.py
-criteo_api_retailmedia_v2024_01/model/resource_of_add_funds_to_balance.py
-criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item.py
-criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item_update_model.py
-criteo_api_retailmedia_v2024_01/model/resource_of_balance_campaign202110.py
-criteo_api_retailmedia_v2024_01/model/resource_of_balance_response.py
-criteo_api_retailmedia_v2024_01/model/resource_of_category202204.py
-criteo_api_retailmedia_v2024_01/model/resource_of_change_dates_of_balance.py
-criteo_api_retailmedia_v2024_01/model/resource_of_common_line_item.py
-criteo_api_retailmedia_v2024_01/model/resource_of_create_balance.py
-criteo_api_retailmedia_v2024_01/model/resource_of_creative202110.py
-criteo_api_retailmedia_v2024_01/model/resource_of_creative202210.py
-criteo_api_retailmedia_v2024_01/model/resource_of_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item202110.py
-criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/resource_of_promoted_product202110.py
-criteo_api_retailmedia_v2024_01/model/resource_of_template.py
-criteo_api_retailmedia_v2024_01/model/resource_of_update_balance_model.py
-criteo_api_retailmedia_v2024_01/model/resource_outcome.py
-criteo_api_retailmedia_v2024_01/model/review_state_model.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_resource.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_response.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_resource.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_response.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v1.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v2.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_list_response.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_resource.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_list_response.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_resource.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_create_v2.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_details_v2.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_customer_list.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_create_v2.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v1.py
-criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v2.py
-criteo_api_retailmedia_v2024_01/model/rmca_common_problem.py
-criteo_api_retailmedia_v2024_01/model/section.py
-criteo_api_retailmedia_v2024_01/model/set_bid_model.py
-criteo_api_retailmedia_v2024_01/model/set_bids_model.py
-criteo_api_retailmedia_v2024_01/model/set_bids_model_request.py
-criteo_api_retailmedia_v2024_01/model/set_bids_model_resource.py
-criteo_api_retailmedia_v2024_01/model/status_response.py
-criteo_api_retailmedia_v2024_01/model/status_response_resource.py
-criteo_api_retailmedia_v2024_01/model/store_ids_update_model202110_request.py
-criteo_api_retailmedia_v2024_01/model/store_target202110_request.py
-criteo_api_retailmedia_v2024_01/model/store_target202110_response.py
-criteo_api_retailmedia_v2024_01/model/template.py
-criteo_api_retailmedia_v2024_01/model/template_list_response.py
-criteo_api_retailmedia_v2024_01/model/template_response.py
-criteo_api_retailmedia_v2024_01/model/template_variable.py
-criteo_api_retailmedia_v2024_01/model/template_variable_value.py
-criteo_api_retailmedia_v2024_01/model/text_variable_specification.py
-criteo_api_retailmedia_v2024_01/model/text_variable_value.py
-criteo_api_retailmedia_v2024_01/model/update_balance_model_request.py
-criteo_api_retailmedia_v2024_01/model/value_resource_input_of_campaign_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/value_resource_input_of_line_item_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/value_resource_of_campaign_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/value_resource_of_line_item_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_campaign_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_line_item_budget_overrides.py
-criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_target202110.py
-criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_ids_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_target202110.py
-criteo_api_retailmedia_v2024_01/model/value_type_resource_of_keyword_target202110.py
-criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_ids_update_model202110.py
-criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_target202110.py
-criteo_api_retailmedia_v2024_01/models/__init__.py
+criteo_api_retailmedia_v2024_04/__init__.py
+criteo_api_retailmedia_v2024_04/api_client.py
+criteo_api_retailmedia_v2024_04/api_client_builder.py
+criteo_api_retailmedia_v2024_04/configuration.py
+criteo_api_retailmedia_v2024_04/criteo_api_client.py
+criteo_api_retailmedia_v2024_04/criteo_auth.py
+criteo_api_retailmedia_v2024_04/criteo_rest.py
+criteo_api_retailmedia_v2024_04/exceptions.py
+criteo_api_retailmedia_v2024_04/flow_constants.py
+criteo_api_retailmedia_v2024_04/model_utils.py
+criteo_api_retailmedia_v2024_04/rest.py
+criteo_api_retailmedia_v2024_04/api/__init__.py
+criteo_api_retailmedia_v2024_04/api/accounts_api.py
+criteo_api_retailmedia_v2024_04/api/analytics_api.py
+criteo_api_retailmedia_v2024_04/api/audience_api.py
+criteo_api_retailmedia_v2024_04/api/campaign_api.py
+criteo_api_retailmedia_v2024_04/api/gateway_api.py
+criteo_api_retailmedia_v2024_04/apis/__init__.py
+criteo_api_retailmedia_v2024_04/model/__init__.py
+criteo_api_retailmedia_v2024_04/model/add_funds_to_balance_request.py
+criteo_api_retailmedia_v2024_04/model/add_remove_keyword_model.py
+criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model.py
+criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model_request.py
+criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model_resource.py
+criteo_api_retailmedia_v2024_04/model/add_to_basket_ids_update_model202110_request.py
+criteo_api_retailmedia_v2024_04/model/add_to_basket_target202110_request.py
+criteo_api_retailmedia_v2024_04/model/add_to_basket_target202110_response.py
+criteo_api_retailmedia_v2024_04/model/application_summary_model.py
+criteo_api_retailmedia_v2024_04/model/application_summary_model_resource.py
+criteo_api_retailmedia_v2024_04/model/application_summary_model_response.py
+criteo_api_retailmedia_v2024_04/model/approval_status_model.py
+criteo_api_retailmedia_v2024_04/model/asset.py
+criteo_api_retailmedia_v2024_04/model/asset_resource.py
+criteo_api_retailmedia_v2024_04/model/asset_response.py
+criteo_api_retailmedia_v2024_04/model/async_campaigns_report.py
+criteo_api_retailmedia_v2024_04/model/async_campaigns_report_request.py
+criteo_api_retailmedia_v2024_04/model/async_campaigns_report_resource.py
+criteo_api_retailmedia_v2024_04/model/async_line_items_report.py
+criteo_api_retailmedia_v2024_04/model/async_line_items_report_request.py
+criteo_api_retailmedia_v2024_04/model/async_line_items_report_resource.py
+criteo_api_retailmedia_v2024_04/model/async_report_response.py
+criteo_api_retailmedia_v2024_04/model/async_revenue_report.py
+criteo_api_retailmedia_v2024_04/model/async_revenue_report_request.py
+criteo_api_retailmedia_v2024_04/model/async_revenue_report_resource.py
+criteo_api_retailmedia_v2024_04/model/auction_line_item_create_model_request.py
+criteo_api_retailmedia_v2024_04/model/auction_line_item_paged_list_response.py
+criteo_api_retailmedia_v2024_04/model/auction_line_item_response.py
+criteo_api_retailmedia_v2024_04/model/auction_line_item_update_model_request.py
+criteo_api_retailmedia_v2024_04/model/audience_ids_update_model202110_request.py
+criteo_api_retailmedia_v2024_04/model/audience_target202110_request.py
+criteo_api_retailmedia_v2024_04/model/audience_target202110_response.py
+criteo_api_retailmedia_v2024_04/model/balance_campaign202110_list_request.py
+criteo_api_retailmedia_v2024_04/model/balance_campaign202110_paged_list_response.py
+criteo_api_retailmedia_v2024_04/model/balance_response.py
+criteo_api_retailmedia_v2024_04/model/balance_response_paged_list_response.py
+criteo_api_retailmedia_v2024_04/model/campaign_attributes_v202301.py
+criteo_api_retailmedia_v2024_04/model/campaign_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/campaign_daily_budget_override.py
+criteo_api_retailmedia_v2024_04/model/campaign_monthly_budget_override.py
+criteo_api_retailmedia_v2024_04/model/campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/category202204.py
+criteo_api_retailmedia_v2024_04/model/category202204_list_response.py
+criteo_api_retailmedia_v2024_04/model/change_dates_of_balance_request.py
+criteo_api_retailmedia_v2024_04/model/change_details.py
+criteo_api_retailmedia_v2024_04/model/choice_option.py
+criteo_api_retailmedia_v2024_04/model/choice_variable_specification.py
+criteo_api_retailmedia_v2024_04/model/choice_variable_value.py
+criteo_api_retailmedia_v2024_04/model/color_variable_value.py
+criteo_api_retailmedia_v2024_04/model/common_error.py
+criteo_api_retailmedia_v2024_04/model/common_line_item_paged_list_response.py
+criteo_api_retailmedia_v2024_04/model/common_line_item_response.py
+criteo_api_retailmedia_v2024_04/model/common_problem.py
+criteo_api_retailmedia_v2024_04/model/common_warning.py
+criteo_api_retailmedia_v2024_04/model/create_balance_request.py
+criteo_api_retailmedia_v2024_04/model/creative202110.py
+criteo_api_retailmedia_v2024_04/model/creative202110_list_response.py
+criteo_api_retailmedia_v2024_04/model/creative202210.py
+criteo_api_retailmedia_v2024_04/model/creative202210_list_response.py
+criteo_api_retailmedia_v2024_04/model/creative202210_response.py
+criteo_api_retailmedia_v2024_04/model/creative_create_model202207.py
+criteo_api_retailmedia_v2024_04/model/creative_update_model202207.py
+criteo_api_retailmedia_v2024_04/model/daily_line_item_budget_override.py
+criteo_api_retailmedia_v2024_04/model/editable_campaign_attributes_v202301.py
+criteo_api_retailmedia_v2024_04/model/external_account.py
+criteo_api_retailmedia_v2024_04/model/external_add_funds_to_balance.py
+criteo_api_retailmedia_v2024_04/model/external_add_to_basket_ids_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/external_add_to_basket_target202110.py
+criteo_api_retailmedia_v2024_04/model/external_auction_line_item.py
+criteo_api_retailmedia_v2024_04/model/external_auction_line_item_create_model.py
+criteo_api_retailmedia_v2024_04/model/external_auction_line_item_update_model.py
+criteo_api_retailmedia_v2024_04/model/external_audience_ids_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/external_audience_target202110.py
+criteo_api_retailmedia_v2024_04/model/external_balance_response.py
+criteo_api_retailmedia_v2024_04/model/external_brand.py
+criteo_api_retailmedia_v2024_04/model/external_catalog_request.py
+criteo_api_retailmedia_v2024_04/model/external_catalog_status.py
+criteo_api_retailmedia_v2024_04/model/external_change_dates_of_balance.py
+criteo_api_retailmedia_v2024_04/model/external_common_line_item.py
+criteo_api_retailmedia_v2024_04/model/external_create_balance.py
+criteo_api_retailmedia_v2024_04/model/external_keyword_target202110.py
+criteo_api_retailmedia_v2024_04/model/external_line_item_capping202110.py
+criteo_api_retailmedia_v2024_04/model/external_line_item_page202110.py
+criteo_api_retailmedia_v2024_04/model/external_line_item_page_category202110.py
+criteo_api_retailmedia_v2024_04/model/external_preferred_line_item202110.py
+criteo_api_retailmedia_v2024_04/model/external_preferred_line_item_create_model202110.py
+criteo_api_retailmedia_v2024_04/model/external_preferred_line_item_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/external_promoted_product202110.py
+criteo_api_retailmedia_v2024_04/model/external_retailer.py
+criteo_api_retailmedia_v2024_04/model/external_retailer_pages202110.py
+criteo_api_retailmedia_v2024_04/model/external_store_ids_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/external_store_target202110.py
+criteo_api_retailmedia_v2024_04/model/external_update_balance_model.py
+criteo_api_retailmedia_v2024_04/model/files_variable_value.py
+criteo_api_retailmedia_v2024_04/model/files_variables_specification.py
+criteo_api_retailmedia_v2024_04/model/hyperlink_variable_value.py
+criteo_api_retailmedia_v2024_04/model/input_keywords_model.py
+criteo_api_retailmedia_v2024_04/model/input_resource_of_auction_line_item_create_model.py
+criteo_api_retailmedia_v2024_04/model/input_resource_of_preferred_line_item_create_model202110.py
+criteo_api_retailmedia_v2024_04/model/insertion_order_history_change_data_capture.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_account.py
+criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_brand.py
+criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_retailer.py
+criteo_api_retailmedia_v2024_04/model/json_api_request_of_catalog_request.py
+criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_catalog_status.py
+criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2024_04/model/keyword_data_model.py
+criteo_api_retailmedia_v2024_04/model/keyword_target202110_request.py
+criteo_api_retailmedia_v2024_04/model/keyword_target202110_response.py
+criteo_api_retailmedia_v2024_04/model/keywords_model.py
+criteo_api_retailmedia_v2024_04/model/keywords_model_resource.py
+criteo_api_retailmedia_v2024_04/model/keywords_model_response.py
+criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers.py
+criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers_request.py
+criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers_response.py
+criteo_api_retailmedia_v2024_04/model/line_item_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/match_type_model.py
+criteo_api_retailmedia_v2024_04/model/metadata.py
+criteo_api_retailmedia_v2024_04/model/monthly_line_item_budeget_override.py
+criteo_api_retailmedia_v2024_04/model/negotiation_state_model.py
+criteo_api_retailmedia_v2024_04/model/page_metadata.py
+criteo_api_retailmedia_v2024_04/model/page_of_insertion_order_history_change_data_capture.py
+criteo_api_retailmedia_v2024_04/model/page_type_environment.py
+criteo_api_retailmedia_v2024_04/model/post_campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/preferred_line_item202110_paged_list_response.py
+criteo_api_retailmedia_v2024_04/model/preferred_line_item202110_response.py
+criteo_api_retailmedia_v2024_04/model/preferred_line_item_create_model202110_request.py
+criteo_api_retailmedia_v2024_04/model/preferred_line_item_update_model202110_request.py
+criteo_api_retailmedia_v2024_04/model/problem_details.py
+criteo_api_retailmedia_v2024_04/model/promoted_product202110_list_request.py
+criteo_api_retailmedia_v2024_04/model/promoted_product202110_paged_list_response.py
+criteo_api_retailmedia_v2024_04/model/proposal_status_model.py
+criteo_api_retailmedia_v2024_04/model/proposal_status_model_resource.py
+criteo_api_retailmedia_v2024_04/model/proposal_status_model_response.py
+criteo_api_retailmedia_v2024_04/model/put_campaign_v202301.py
+criteo_api_retailmedia_v2024_04/model/report_outcome.py
+criteo_api_retailmedia_v2024_04/model/resource_of_add_funds_to_balance.py
+criteo_api_retailmedia_v2024_04/model/resource_of_auction_line_item.py
+criteo_api_retailmedia_v2024_04/model/resource_of_auction_line_item_update_model.py
+criteo_api_retailmedia_v2024_04/model/resource_of_balance_campaign202110.py
+criteo_api_retailmedia_v2024_04/model/resource_of_balance_response.py
+criteo_api_retailmedia_v2024_04/model/resource_of_category202204.py
+criteo_api_retailmedia_v2024_04/model/resource_of_change_dates_of_balance.py
+criteo_api_retailmedia_v2024_04/model/resource_of_common_line_item.py
+criteo_api_retailmedia_v2024_04/model/resource_of_create_balance.py
+criteo_api_retailmedia_v2024_04/model/resource_of_creative202110.py
+criteo_api_retailmedia_v2024_04/model/resource_of_creative202210.py
+criteo_api_retailmedia_v2024_04/model/resource_of_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2024_04/model/resource_of_preferred_line_item202110.py
+criteo_api_retailmedia_v2024_04/model/resource_of_preferred_line_item_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/resource_of_promoted_product202110.py
+criteo_api_retailmedia_v2024_04/model/resource_of_retail_media_account.py
+criteo_api_retailmedia_v2024_04/model/resource_of_template.py
+criteo_api_retailmedia_v2024_04/model/resource_of_update_balance_model.py
+criteo_api_retailmedia_v2024_04/model/resource_outcome.py
+criteo_api_retailmedia_v2024_04/model/resource_outcome_of_retail_media_account.py
+criteo_api_retailmedia_v2024_04/model/retail_media_account.py
+criteo_api_retailmedia_v2024_04/model/retail_media_brand_account_creation.py
+criteo_api_retailmedia_v2024_04/model/retail_media_brands.py
+criteo_api_retailmedia_v2024_04/model/review_state_model.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1_resource.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1_response.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2_resource.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2_response.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_input_entity_v1.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_input_entity_v2.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1_list_response.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1_resource.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2_list_response.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2_resource.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_user_behavior_create_v2.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_user_behavior_details_v2.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_customer_list.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_create_v2.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_v1.py
+criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_v2.py
+criteo_api_retailmedia_v2024_04/model/rmca_common_problem.py
+criteo_api_retailmedia_v2024_04/model/section.py
+criteo_api_retailmedia_v2024_04/model/set_bid_model.py
+criteo_api_retailmedia_v2024_04/model/set_bids_model.py
+criteo_api_retailmedia_v2024_04/model/set_bids_model_request.py
+criteo_api_retailmedia_v2024_04/model/set_bids_model_resource.py
+criteo_api_retailmedia_v2024_04/model/status_response.py
+criteo_api_retailmedia_v2024_04/model/status_response_resource.py
+criteo_api_retailmedia_v2024_04/model/store_ids_update_model202110_request.py
+criteo_api_retailmedia_v2024_04/model/store_target202110_request.py
+criteo_api_retailmedia_v2024_04/model/store_target202110_response.py
+criteo_api_retailmedia_v2024_04/model/template.py
+criteo_api_retailmedia_v2024_04/model/template_list_response.py
+criteo_api_retailmedia_v2024_04/model/template_response.py
+criteo_api_retailmedia_v2024_04/model/template_variable.py
+criteo_api_retailmedia_v2024_04/model/template_variable_value.py
+criteo_api_retailmedia_v2024_04/model/text_variable_specification.py
+criteo_api_retailmedia_v2024_04/model/text_variable_value.py
+criteo_api_retailmedia_v2024_04/model/update_balance_model_request.py
+criteo_api_retailmedia_v2024_04/model/value_resource_input_of_campaign_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/value_resource_input_of_line_item_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/value_resource_input_of_retail_media_brand_account_creation.py
+criteo_api_retailmedia_v2024_04/model/value_resource_input_of_retail_media_brands.py
+criteo_api_retailmedia_v2024_04/model/value_resource_of_campaign_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/value_resource_of_line_item_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/value_resource_of_retail_media_brand_account_creation.py
+criteo_api_retailmedia_v2024_04/model/value_resource_of_retail_media_brands.py
+criteo_api_retailmedia_v2024_04/model/value_resource_outcome_of_campaign_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/value_resource_outcome_of_line_item_budget_overrides.py
+criteo_api_retailmedia_v2024_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/value_type_resource_of_add_to_basket_target202110.py
+criteo_api_retailmedia_v2024_04/model/value_type_resource_of_audience_ids_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/value_type_resource_of_audience_target202110.py
+criteo_api_retailmedia_v2024_04/model/value_type_resource_of_keyword_target202110.py
+criteo_api_retailmedia_v2024_04/model/value_type_resource_of_store_ids_update_model202110.py
+criteo_api_retailmedia_v2024_04/model/value_type_resource_of_store_target202110.py
+criteo_api_retailmedia_v2024_04/models/__init__.py
 test/test_gateway_api.py
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/__init__.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2024.01.0.240515"
+__version__ = "2024.04.0.240515"
 
 # import ApiClient
-from criteo_api_retailmedia_v2024_01.api_client import ApiClient
-from criteo_api_retailmedia_v2024_01.criteo_api_client import CriteoApiClient
-from criteo_api_retailmedia_v2024_01.api_client_builder import ApiClientBuilder
-from criteo_api_retailmedia_v2024_01 import flow_constants
+from criteo_api_retailmedia_v2024_04.api_client import ApiClient
+from criteo_api_retailmedia_v2024_04.criteo_api_client import CriteoApiClient
+from criteo_api_retailmedia_v2024_04.api_client_builder import ApiClientBuilder
+from criteo_api_retailmedia_v2024_04 import flow_constants
 
 # import Configuration
-from criteo_api_retailmedia_v2024_01.configuration import Configuration
+from criteo_api_retailmedia_v2024_04.configuration import Configuration
 
 # import exceptions
-from criteo_api_retailmedia_v2024_01.exceptions import OpenApiException
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
-from criteo_api_retailmedia_v2024_01.exceptions import ApiTypeError
-from criteo_api_retailmedia_v2024_01.exceptions import ApiValueError
-from criteo_api_retailmedia_v2024_01.exceptions import ApiKeyError
-from criteo_api_retailmedia_v2024_01.exceptions import ApiException
+from criteo_api_retailmedia_v2024_04.exceptions import OpenApiException
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiTypeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiValueError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiKeyError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiException
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/analytics_api.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/analytics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2024_01.model.async_campaigns_report_request import AsyncCampaignsReportRequest
-from criteo_api_retailmedia_v2024_01.model.async_line_items_report_request import AsyncLineItemsReportRequest
-from criteo_api_retailmedia_v2024_01.model.async_report_response import AsyncReportResponse
-from criteo_api_retailmedia_v2024_01.model.async_revenue_report_request import AsyncRevenueReportRequest
-from criteo_api_retailmedia_v2024_01.model.report_outcome import ReportOutcome
+from criteo_api_retailmedia_v2024_04.model.async_campaigns_report_request import AsyncCampaignsReportRequest
+from criteo_api_retailmedia_v2024_04.model.async_line_items_report_request import AsyncLineItemsReportRequest
+from criteo_api_retailmedia_v2024_04.model.async_report_response import AsyncReportResponse
+from criteo_api_retailmedia_v2024_04.model.async_revenue_report_request import AsyncRevenueReportRequest
+from criteo_api_retailmedia_v2024_04.model.report_outcome import ReportOutcome
 
 
 class AnalyticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -42,15 +42,15 @@
         self.generate_async_campaigns_report_endpoint = _Endpoint(
             settings={
                 'response_type': (AsyncReportResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/reports/campaigns',
+                'endpoint_path': '/2024-04/retail-media/reports/campaigns',
                 'operation_id': 'generate_async_campaigns_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'async_campaigns_report_request',
@@ -100,15 +100,15 @@
         self.generate_async_line_items_report_endpoint = _Endpoint(
             settings={
                 'response_type': (AsyncReportResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/reports/line-items',
+                'endpoint_path': '/2024-04/retail-media/reports/line-items',
                 'operation_id': 'generate_async_line_items_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'async_line_items_report_request',
@@ -158,15 +158,15 @@
         self.generate_async_revenue_report_endpoint = _Endpoint(
             settings={
                 'response_type': (AsyncReportResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/reports/revenue',
+                'endpoint_path': '/2024-04/retail-media/reports/revenue',
                 'operation_id': 'generate_async_revenue_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'async_revenue_report_request',
@@ -216,15 +216,15 @@
         self.get_async_export_output_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/reports/{reportId}/output',
+                'endpoint_path': '/2024-04/retail-media/reports/{reportId}/output',
                 'operation_id': 'get_async_export_output',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'report_id',
@@ -270,15 +270,15 @@
         self.get_async_export_status_endpoint = _Endpoint(
             settings={
                 'response_type': (AsyncReportResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/reports/{reportId}/status',
+                'endpoint_path': '/2024-04/retail-media/reports/{reportId}/status',
                 'operation_id': 'get_async_export_status',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'report_id',
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/audience_api.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/audience_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v1_response import RmLegacyAudienceCreateEntityV1Response
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v2_response import RmLegacyAudienceCreateEntityV2Response
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_input_entity_v1 import RmLegacyAudienceCreateInputEntityV1
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_input_entity_v2 import RmLegacyAudienceCreateInputEntityV2
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v1_list_response import RmLegacyAudienceGetEntityV1ListResponse
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v2_list_response import RmLegacyAudienceGetEntityV2ListResponse
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v1_response import RmLegacyAudienceCreateEntityV1Response
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v2_response import RmLegacyAudienceCreateEntityV2Response
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_input_entity_v1 import RmLegacyAudienceCreateInputEntityV1
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_input_entity_v2 import RmLegacyAudienceCreateInputEntityV2
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v1_list_response import RmLegacyAudienceGetEntityV1ListResponse
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v2_list_response import RmLegacyAudienceGetEntityV2ListResponse
 
 
 class AudienceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -43,15 +43,15 @@
         self.legacy_create_audience_v1_endpoint = _Endpoint(
             settings={
                 'response_type': (RmLegacyAudienceCreateEntityV1Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{accountId}/audiences',
+                'endpoint_path': '/2024-04/retail-media/accounts/{accountId}/audiences',
                 'operation_id': 'legacy_create_audience_v1',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -107,15 +107,15 @@
         self.legacy_get_audience_v1_endpoint = _Endpoint(
             settings={
                 'response_type': (RmLegacyAudienceGetEntityV1ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{accountId}/audiences',
+                'endpoint_path': '/2024-04/retail-media/accounts/{accountId}/audiences',
                 'operation_id': 'legacy_get_audience_v1',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -177,15 +177,15 @@
         self.legacy_get_audience_v2_endpoint = _Endpoint(
             settings={
                 'response_type': (RmLegacyAudienceGetEntityV2ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/v2/accounts/{accountId}/audiences',
+                'endpoint_path': '/2024-04/retail-media/v2/accounts/{accountId}/audiences',
                 'operation_id': 'legacy_get_audience_v2',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -247,15 +247,15 @@
         self.legacy_update_audience_v2_endpoint = _Endpoint(
             settings={
                 'response_type': (RmLegacyAudienceCreateEntityV2Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/v2/accounts/{accountId}/audiences',
+                'endpoint_path': '/2024-04/retail-media/v2/accounts/{accountId}/audiences',
                 'operation_id': 'legacy_update_audience_v2',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/campaign_api.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/campaign_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2024_01.model.add_funds_to_balance_request import AddFundsToBalanceRequest
-from criteo_api_retailmedia_v2024_01.model.add_remove_keywords_model_request import AddRemoveKeywordsModelRequest
-from criteo_api_retailmedia_v2024_01.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.asset_response import AssetResponse
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_response import AuctionLineItemResponse
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
-from criteo_api_retailmedia_v2024_01.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.audience_target202110_request import AudienceTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.audience_target202110_response import AudienceTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
-from criteo_api_retailmedia_v2024_01.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
-from criteo_api_retailmedia_v2024_01.model.balance_response import BalanceResponse
-from criteo_api_retailmedia_v2024_01.model.balance_response_paged_list_response import BalanceResponsePagedListResponse
-from criteo_api_retailmedia_v2024_01.model.category202204 import Category202204
-from criteo_api_retailmedia_v2024_01.model.category202204_list_response import Category202204ListResponse
-from criteo_api_retailmedia_v2024_01.model.change_dates_of_balance_request import ChangeDatesOfBalanceRequest
-from criteo_api_retailmedia_v2024_01.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
-from criteo_api_retailmedia_v2024_01.model.common_line_item_response import CommonLineItemResponse
-from criteo_api_retailmedia_v2024_01.model.create_balance_request import CreateBalanceRequest
-from criteo_api_retailmedia_v2024_01.model.creative202110_list_response import Creative202110ListResponse
-from criteo_api_retailmedia_v2024_01.model.creative202210_list_response import Creative202210ListResponse
-from criteo_api_retailmedia_v2024_01.model.creative202210_response import Creative202210Response
-from criteo_api_retailmedia_v2024_01.model.creative_create_model202207 import CreativeCreateModel202207
-from criteo_api_retailmedia_v2024_01.model.creative_update_model202207 import CreativeUpdateModel202207
-from criteo_api_retailmedia_v2024_01.model.external_retailer_pages202110 import ExternalRetailerPages202110
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
-from criteo_api_retailmedia_v2024_01.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
-from criteo_api_retailmedia_v2024_01.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
-from criteo_api_retailmedia_v2024_01.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2024_01.model.keyword_target202110_request import KeywordTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.keyword_target202110_response import KeywordTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.keywords_model_response import KeywordsModelResponse
-from criteo_api_retailmedia_v2024_01.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
-from criteo_api_retailmedia_v2024_01.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
-from criteo_api_retailmedia_v2024_01.model.post_campaign_v202301 import PostCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item202110_response import PreferredLineItem202110Response
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
-from criteo_api_retailmedia_v2024_01.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
-from criteo_api_retailmedia_v2024_01.model.proposal_status_model_response import ProposalStatusModelResponse
-from criteo_api_retailmedia_v2024_01.model.put_campaign_v202301 import PutCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.resource_outcome import ResourceOutcome
-from criteo_api_retailmedia_v2024_01.model.set_bids_model_request import SetBidsModelRequest
-from criteo_api_retailmedia_v2024_01.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.store_target202110_request import StoreTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.store_target202110_response import StoreTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.template_list_response import TemplateListResponse
-from criteo_api_retailmedia_v2024_01.model.template_response import TemplateResponse
-from criteo_api_retailmedia_v2024_01.model.update_balance_model_request import UpdateBalanceModelRequest
-from criteo_api_retailmedia_v2024_01.model.value_resource_input_of_campaign_budget_overrides import ValueResourceInputOfCampaignBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_input_of_line_item_budget_overrides import ValueResourceInputOfLineItemBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_outcome_of_campaign_budget_overrides import ValueResourceOutcomeOfCampaignBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_outcome_of_line_item_budget_overrides import ValueResourceOutcomeOfLineItemBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.add_funds_to_balance_request import AddFundsToBalanceRequest
+from criteo_api_retailmedia_v2024_04.model.add_remove_keywords_model_request import AddRemoveKeywordsModelRequest
+from criteo_api_retailmedia_v2024_04.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.asset_response import AssetResponse
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_response import AuctionLineItemResponse
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
+from criteo_api_retailmedia_v2024_04.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.audience_target202110_request import AudienceTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.audience_target202110_response import AudienceTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
+from criteo_api_retailmedia_v2024_04.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
+from criteo_api_retailmedia_v2024_04.model.balance_response import BalanceResponse
+from criteo_api_retailmedia_v2024_04.model.balance_response_paged_list_response import BalanceResponsePagedListResponse
+from criteo_api_retailmedia_v2024_04.model.category202204 import Category202204
+from criteo_api_retailmedia_v2024_04.model.category202204_list_response import Category202204ListResponse
+from criteo_api_retailmedia_v2024_04.model.change_dates_of_balance_request import ChangeDatesOfBalanceRequest
+from criteo_api_retailmedia_v2024_04.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
+from criteo_api_retailmedia_v2024_04.model.common_line_item_response import CommonLineItemResponse
+from criteo_api_retailmedia_v2024_04.model.create_balance_request import CreateBalanceRequest
+from criteo_api_retailmedia_v2024_04.model.creative202110_list_response import Creative202110ListResponse
+from criteo_api_retailmedia_v2024_04.model.creative202210_list_response import Creative202210ListResponse
+from criteo_api_retailmedia_v2024_04.model.creative202210_response import Creative202210Response
+from criteo_api_retailmedia_v2024_04.model.creative_create_model202207 import CreativeCreateModel202207
+from criteo_api_retailmedia_v2024_04.model.creative_update_model202207 import CreativeUpdateModel202207
+from criteo_api_retailmedia_v2024_04.model.external_retailer_pages202110 import ExternalRetailerPages202110
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
+from criteo_api_retailmedia_v2024_04.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
+from criteo_api_retailmedia_v2024_04.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
+from criteo_api_retailmedia_v2024_04.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2024_04.model.keyword_target202110_request import KeywordTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.keyword_target202110_response import KeywordTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.keywords_model_response import KeywordsModelResponse
+from criteo_api_retailmedia_v2024_04.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
+from criteo_api_retailmedia_v2024_04.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
+from criteo_api_retailmedia_v2024_04.model.page_of_insertion_order_history_change_data_capture import PageOfInsertionOrderHistoryChangeDataCapture
+from criteo_api_retailmedia_v2024_04.model.post_campaign_v202301 import PostCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item202110_response import PreferredLineItem202110Response
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
+from criteo_api_retailmedia_v2024_04.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
+from criteo_api_retailmedia_v2024_04.model.proposal_status_model_response import ProposalStatusModelResponse
+from criteo_api_retailmedia_v2024_04.model.put_campaign_v202301 import PutCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.resource_outcome import ResourceOutcome
+from criteo_api_retailmedia_v2024_04.model.set_bids_model_request import SetBidsModelRequest
+from criteo_api_retailmedia_v2024_04.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.store_target202110_request import StoreTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.store_target202110_response import StoreTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.template_list_response import TemplateListResponse
+from criteo_api_retailmedia_v2024_04.model.template_response import TemplateResponse
+from criteo_api_retailmedia_v2024_04.model.update_balance_model_request import UpdateBalanceModelRequest
+from criteo_api_retailmedia_v2024_04.model.value_resource_input_of_campaign_budget_overrides import ValueResourceInputOfCampaignBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_input_of_line_item_budget_overrides import ValueResourceInputOfLineItemBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_outcome_of_campaign_budget_overrides import ValueResourceOutcomeOfCampaignBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_outcome_of_line_item_budget_overrides import ValueResourceOutcomeOfLineItemBudgetOverrides
 
 
 class CampaignApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -100,15 +101,15 @@
         self.add_remove_keywords_endpoint = _Endpoint(
             settings={
                 'response_type': (ResourceOutcome,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{id}/keywords/add-remove',
+                'endpoint_path': '/2024-04/retail-media/line-items/{id}/keywords/add-remove',
                 'operation_id': 'add_remove_keywords',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -158,15 +159,15 @@
         self.create_asset_endpoint = _Endpoint(
             settings={
                 'response_type': (AssetResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/assets',
+                'endpoint_path': '/2024-04/retail-media/assets',
                 'operation_id': 'create_asset',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'asset_file',
@@ -214,15 +215,15 @@
         self.fetch_keywords_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordsModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{id}/keywords',
+                'endpoint_path': '/2024-04/retail-media/line-items/{id}/keywords',
                 'operation_id': 'fetch_keywords',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -266,15 +267,15 @@
         self.fetch_proposal_endpoint = _Endpoint(
             settings={
                 'response_type': (ProposalStatusModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-deal-line-items/{id}/proposal',
+                'endpoint_path': '/2024-04/retail-media/preferred-deal-line-items/{id}/proposal',
                 'operation_id': 'fetch_proposal',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -318,15 +319,15 @@
         self.get_api202110_external_account_creatives_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202110ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/creatives',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/creatives',
                 'operation_id': 'get_api202110_external_account_creatives_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -370,15 +371,15 @@
         self.get_api202110_external_auction_line_item_targeting_keywords_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/auction-line-items/{line-item-id}/targeting/keywords',
+                'endpoint_path': '/2024-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords',
                 'operation_id': 'get_api202110_external_auction_line_item_targeting_keywords_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -422,15 +423,15 @@
         self.get_api202110_external_balance_campaigns_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/balances/{balance-id}/campaigns',
+                'endpoint_path': '/2024-04/retail-media/balances/{balance-id}/campaigns',
                 'operation_id': 'get_api202110_external_balance_campaigns_by_balance_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -490,15 +491,15 @@
         self.get_api202110_external_campaign_preferred_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaign-id}/preferred-line-items',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaign-id}/preferred-line-items',
                 'operation_id': 'get_api202110_external_campaign_preferred_line_items_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -558,15 +559,15 @@
         self.get_api202110_external_line_item_products_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}/products',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}/products',
                 'operation_id': 'get_api202110_external_line_item_products_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -626,15 +627,15 @@
         self.get_api202110_external_preferred_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}',
                 'operation_id': 'get_api202110_external_preferred_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -678,15 +679,15 @@
         self.get_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -730,15 +731,15 @@
         self.get_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -782,15 +783,15 @@
         self.get_api202110_external_preferred_line_item_targeting_stores_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_stores_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -834,15 +835,15 @@
         self.get_api202110_external_retailer_pages_by_retailer_id_endpoint = _Endpoint(
             settings={
                 'response_type': (ExternalRetailerPages202110,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/retailers/{retailerId}/pages',
+                'endpoint_path': '/2024-04/retail-media/retailers/{retailerId}/pages',
                 'operation_id': 'get_api202110_external_retailer_pages_by_retailer_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -886,15 +887,15 @@
         self.get_api202204_external_categorie_by_category_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Category202204,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/categories/{categoryId}',
+                'endpoint_path': '/2024-04/retail-media/categories/{categoryId}',
                 'operation_id': 'get_api202204_external_categorie_by_category_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'category_id',
@@ -938,15 +939,15 @@
         self.get_api202204_external_categories_endpoint = _Endpoint(
             settings={
                 'response_type': (Category202204ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/categories',
+                'endpoint_path': '/2024-04/retail-media/categories',
                 'operation_id': 'get_api202204_external_categories',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -1015,15 +1016,15 @@
         self.get_api202207_external_retailer_by_retailer_id_templatestemplate_id_endpoint = _Endpoint(
             settings={
                 'response_type': (TemplateResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/retailers/{retailer-id}/templates/{template-id}',
+                'endpoint_path': '/2024-04/retail-media/retailers/{retailer-id}/templates/{template-id}',
                 'operation_id': 'get_api202207_external_retailer_by_retailer_id_templatestemplate_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -1073,15 +1074,15 @@
         self.get_api202207_external_retailer_templates_by_retailer_id_endpoint = _Endpoint(
             settings={
                 'response_type': (TemplateListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/retailers/{retailer-id}/templates',
+                'endpoint_path': '/2024-04/retail-media/retailers/{retailer-id}/templates',
                 'operation_id': 'get_api202207_external_retailer_templates_by_retailer_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -1125,15 +1126,15 @@
         self.get_api202210_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/creatives/{creative-id}',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/creatives/{creative-id}',
                 'operation_id': 'get_api202210_external_account_by_account_id_creativescreative_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1183,15 +1184,15 @@
         self.get_api202301_external_account_campaigns_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/campaigns',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/campaigns',
                 'operation_id': 'get_api202301_external_account_campaigns_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1251,15 +1252,15 @@
         self.get_api202301_external_campaign_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaignId}',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaignId}',
                 'operation_id': 'get_api202301_external_campaign_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -1303,15 +1304,15 @@
         self.get_api202301_external_line_item_bid_multipliers_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfLineItemBidMultipliers,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}/bid-multipliers',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}/bid-multipliers',
                 'operation_id': 'get_api202301_external_line_item_bid_multipliers_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1357,15 +1358,15 @@
         self.get_api_v1_external_account_balances_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceResponsePagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/balances',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/balances',
                 'operation_id': 'get_api_v1_external_account_balances_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1425,15 +1426,15 @@
         self.get_api_v1_external_account_brands_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfBrand,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{accountId}/brands',
+                'endpoint_path': '/2024-04/retail-media/accounts/{accountId}/brands',
                 'operation_id': 'get_api_v1_external_account_brands_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1493,15 +1494,15 @@
         self.get_api_v1_external_account_by_account_id_and_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/balances/{balanceId}',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/balances/{balanceId}',
                 'operation_id': 'get_api_v1_external_account_by_account_id_and_balance_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1551,15 +1552,15 @@
         self.get_api_v1_external_account_retailers_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfRetailer,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{accountId}/retailers',
+                'endpoint_path': '/2024-04/retail-media/accounts/{accountId}/retailers',
                 'operation_id': 'get_api_v1_external_account_retailers_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1619,15 +1620,15 @@
         self.get_api_v1_external_accounts_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfAccount,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts',
+                'endpoint_path': '/2024-04/retail-media/accounts',
                 'operation_id': 'get_api_v1_external_accounts',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'limit_to_id',
@@ -1680,15 +1681,15 @@
         self.get_api_v1_external_catalog_output_by_catalog_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/catalogs/{catalogId}/output',
+                'endpoint_path': '/2024-04/retail-media/catalogs/{catalogId}/output',
                 'operation_id': 'get_api_v1_external_catalog_output_by_catalog_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'catalog_id',
@@ -1733,15 +1734,15 @@
         self.get_api_v1_external_catalog_status_by_catalog_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCatalogStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/catalogs/{catalogId}/status',
+                'endpoint_path': '/2024-04/retail-media/catalogs/{catalogId}/status',
                 'operation_id': 'get_api_v1_external_catalog_status_by_catalog_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'catalog_id',
@@ -1785,15 +1786,15 @@
         self.get_api_v2_external_account_line_items_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (CommonLineItemPagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/line-items',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/line-items',
                 'operation_id': 'get_api_v2_external_account_line_items_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1871,15 +1872,15 @@
         self.get_api_v2_external_auction_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/auction-line-items/{line-item-id}',
+                'endpoint_path': '/2024-04/retail-media/auction-line-items/{line-item-id}',
                 'operation_id': 'get_api_v2_external_auction_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1923,15 +1924,15 @@
         self.get_api_v2_external_campaign_auction_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemPagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaign-id}/auction-line-items',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaign-id}/auction-line-items',
                 'operation_id': 'get_api_v2_external_campaign_auction_line_items_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -1991,15 +1992,15 @@
         self.get_api_v2_external_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (CommonLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}',
                 'operation_id': 'get_api_v2_external_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2043,15 +2044,15 @@
         self.get_campaign_budget_overrides_endpoint = _Endpoint(
             settings={
                 'response_type': (ValueResourceOutcomeOfCampaignBudgetOverrides,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaignId}/campaign-budget-overrides',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaignId}/campaign-budget-overrides',
                 'operation_id': 'get_campaign_budget_overrides',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -2088,22 +2089,101 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_insertion_order_history_change_data_capture_endpoint = _Endpoint(
+            settings={
+                'response_type': (PageOfInsertionOrderHistoryChangeDataCapture,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2024-04/retail-media/insertion-order-history/{insertionOrderId}/change-data-capture',
+                'operation_id': 'get_insertion_order_history_change_data_capture',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'insertion_order_id',
+                    'offset',
+                    'limit',
+                    'limit_to_change_types',
+                ],
+                'required': [
+                    'insertion_order_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'offset',
+                    'limit',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('offset',): {
+
+                        'inclusive_maximum': 2147483647,
+                        'inclusive_minimum': 0,
+                    },
+                    ('limit',): {
+
+                        'inclusive_maximum': 100,
+                        'inclusive_minimum': 1,
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'insertion_order_id':
+                        (str,),
+                    'offset':
+                        (int,),
+                    'limit':
+                        (int,),
+                    'limit_to_change_types':
+                        (str,),
+                },
+                'attribute_map': {
+                    'insertion_order_id': 'insertionOrderId',
+                    'offset': 'offset',
+                    'limit': 'limit',
+                    'limit_to_change_types': 'limitToChangeTypes',
+                },
+                'location_map': {
+                    'insertion_order_id': 'path',
+                    'offset': 'query',
+                    'limit': 'query',
+                    'limit_to_change_types': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_line_item_budget_overrides_endpoint = _Endpoint(
             settings={
                 'response_type': (ValueResourceOutcomeOfLineItemBudgetOverrides,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{lineItemId}/line-item-budget-overrides',
+                'endpoint_path': '/2024-04/retail-media/line-items/{lineItemId}/line-item-budget-overrides',
                 'operation_id': 'get_line_item_budget_overrides',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2147,15 +2227,15 @@
         self.patch_api_v1_external_account_by_account_id_and_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/balances/{balanceId}',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/balances/{balanceId}',
                 'operation_id': 'patch_api_v1_external_account_by_account_id_and_balance_id',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -2211,15 +2291,15 @@
         self.post_api202110_external_auction_line_item_targeting_keywords_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/auction-line-items/{line-item-id}/targeting/keywords/append',
+                'endpoint_path': '/2024-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords/append',
                 'operation_id': 'post_api202110_external_auction_line_item_targeting_keywords_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2269,15 +2349,15 @@
         self.post_api202110_external_auction_line_item_targeting_keywords_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/auction-line-items/{line-item-id}/targeting/keywords/delete',
+                'endpoint_path': '/2024-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords/delete',
                 'operation_id': 'post_api202110_external_auction_line_item_targeting_keywords_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2327,15 +2407,15 @@
         self.post_api202110_external_balance_campaigns_append_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/balances/{balance-id}/campaigns/append',
+                'endpoint_path': '/2024-04/retail-media/balances/{balance-id}/campaigns/append',
                 'operation_id': 'post_api202110_external_balance_campaigns_append_by_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -2385,15 +2465,15 @@
         self.post_api202110_external_balance_campaigns_delete_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/balances/{balance-id}/campaigns/delete',
+                'endpoint_path': '/2024-04/retail-media/balances/{balance-id}/campaigns/delete',
                 'operation_id': 'post_api202110_external_balance_campaigns_delete_by_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -2443,15 +2523,15 @@
         self.post_api202110_external_campaign_preferred_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaign-id}/preferred-line-items',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaign-id}/preferred-line-items',
                 'operation_id': 'post_api202110_external_campaign_preferred_line_items_by_campaign_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -2501,15 +2581,15 @@
         self.post_api202110_external_line_item_products_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}/products/append',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}/products/append',
                 'operation_id': 'post_api202110_external_line_item_products_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2559,15 +2639,15 @@
         self.post_api202110_external_line_item_products_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}/products/delete',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}/products/delete',
                 'operation_id': 'post_api202110_external_line_item_products_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2617,15 +2697,15 @@
         self.post_api202110_external_line_item_products_pause_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}/products/pause',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}/products/pause',
                 'operation_id': 'post_api202110_external_line_item_products_pause_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2673,15 +2753,15 @@
         self.post_api202110_external_line_item_products_unpause_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}/products/unpause',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}/products/unpause',
                 'operation_id': 'post_api202110_external_line_item_products_unpause_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2729,15 +2809,15 @@
         self.post_api202110_external_preferred_line_item_targeting_add_to_basket_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/append',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_add_to_basket_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2787,15 +2867,15 @@
         self.post_api202110_external_preferred_line_item_targeting_add_to_basket_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/delete',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_add_to_basket_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2845,15 +2925,15 @@
         self.post_api202110_external_preferred_line_item_targeting_audiences_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/append',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_audiences_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2903,15 +2983,15 @@
         self.post_api202110_external_preferred_line_item_targeting_audiences_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/delete',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_audiences_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2961,15 +3041,15 @@
         self.post_api202110_external_preferred_line_item_targeting_stores_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores/append',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_stores_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3019,15 +3099,15 @@
         self.post_api202110_external_preferred_line_item_targeting_stores_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores/delete',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_stores_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3077,15 +3157,15 @@
         self.post_api202210_external_account_creatives_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/creatives',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/creatives',
                 'operation_id': 'post_api202210_external_account_creatives_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3135,15 +3215,15 @@
         self.post_api202210_external_account_creatives_search_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/creatives/search',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/creatives/search',
                 'operation_id': 'post_api202210_external_account_creatives_search_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3193,15 +3273,15 @@
         self.post_api202301_external_account_campaigns_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/campaigns',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/campaigns',
                 'operation_id': 'post_api202301_external_account_campaigns_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3251,15 +3331,15 @@
         self.post_api_v1_external_account_add_funds_by_account_id_and_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/balances/{balanceId}/add-funds',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/balances/{balanceId}/add-funds',
                 'operation_id': 'post_api_v1_external_account_add_funds_by_account_id_and_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3315,15 +3395,15 @@
         self.post_api_v1_external_account_balances_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/balances',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/balances',
                 'operation_id': 'post_api_v1_external_account_balances_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3373,15 +3453,15 @@
         self.post_api_v1_external_account_catalogs_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCatalogStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{accountId}/catalogs',
+                'endpoint_path': '/2024-04/retail-media/accounts/{accountId}/catalogs',
                 'operation_id': 'post_api_v1_external_account_catalogs_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3431,15 +3511,15 @@
         self.post_api_v1_external_account_change_dates_by_account_id_and_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/balances/{balanceId}/change-dates',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/balances/{balanceId}/change-dates',
                 'operation_id': 'post_api_v1_external_account_change_dates_by_account_id_and_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3495,15 +3575,15 @@
         self.post_api_v2_external_campaign_auction_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaign-id}/auction-line-items',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaign-id}/auction-line-items',
                 'operation_id': 'post_api_v2_external_campaign_auction_line_items_by_campaign_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -3553,15 +3633,15 @@
         self.put_api202110_external_preferred_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}',
                 'operation_id': 'put_api202110_external_preferred_line_item_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3611,15 +3691,15 @@
         self.put_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3669,15 +3749,15 @@
         self.put_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3727,15 +3807,15 @@
         self.put_api202110_external_preferred_line_item_targeting_stores_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
+                'endpoint_path': '/2024-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_stores_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3785,15 +3865,15 @@
         self.put_api202210_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/accounts/{account-id}/creatives/{creative-id}',
+                'endpoint_path': '/2024-04/retail-media/accounts/{account-id}/creatives/{creative-id}',
                 'operation_id': 'put_api202210_external_account_by_account_id_creativescreative_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3849,15 +3929,15 @@
         self.put_api202301_external_campaign_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaignId}',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaignId}',
                 'operation_id': 'put_api202301_external_campaign_by_campaign_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -3907,15 +3987,15 @@
         self.put_api202301_external_line_item_bid_multipliers_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (LineItemBidMultipliersResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{line-item-id}/bid-multipliers',
+                'endpoint_path': '/2024-04/retail-media/line-items/{line-item-id}/bid-multipliers',
                 'operation_id': 'put_api202301_external_line_item_bid_multipliers_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3967,15 +4047,15 @@
         self.put_api_v2_external_auction_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/auction-line-items/{line-item-id}',
+                'endpoint_path': '/2024-04/retail-media/auction-line-items/{line-item-id}',
                 'operation_id': 'put_api_v2_external_auction_line_item_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -4025,15 +4105,15 @@
         self.set_keyword_bids_endpoint = _Endpoint(
             settings={
                 'response_type': (ResourceOutcome,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{id}/keywords/set-bid',
+                'endpoint_path': '/2024-04/retail-media/line-items/{id}/keywords/set-bid',
                 'operation_id': 'set_keyword_bids',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -4083,15 +4163,15 @@
         self.submit_proposal_endpoint = _Endpoint(
             settings={
                 'response_type': (ProposalStatusModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/preferred-deal-line-items/{id}/proposal/submit',
+                'endpoint_path': '/2024-04/retail-media/preferred-deal-line-items/{id}/proposal/submit',
                 'operation_id': 'submit_proposal',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -4135,15 +4215,15 @@
         self.update_campaign_budget_overrides_endpoint = _Endpoint(
             settings={
                 'response_type': (ValueResourceOutcomeOfCampaignBudgetOverrides,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/campaigns/{campaignId}/campaign-budget-overrides',
+                'endpoint_path': '/2024-04/retail-media/campaigns/{campaignId}/campaign-budget-overrides',
                 'operation_id': 'update_campaign_budget_overrides',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -4196,15 +4276,15 @@
         self.update_line_item_budget_overrides_endpoint = _Endpoint(
             settings={
                 'response_type': (ValueResourceOutcomeOfLineItemBudgetOverrides,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2024-01/retail-media/line-items/{lineItemId}/line-item-budget-overrides',
+                'endpoint_path': '/2024-04/retail-media/line-items/{lineItemId}/line-item-budget-overrides',
                 'operation_id': 'update_line_item_budget_overrides',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -7112,14 +7192,100 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         kwargs['campaign_id'] = \
             campaign_id
         return self.get_campaign_budget_overrides_endpoint.call_with_http_info(**kwargs)
 
+    def get_insertion_order_history_change_data_capture(
+        self,
+        insertion_order_id,
+        **kwargs
+    ):
+        """get_insertion_order_history_change_data_capture  # noqa: E501
+
+        Gets the balance's historical data change capture.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_insertion_order_history_change_data_capture(insertion_order_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            insertion_order_id (str): External insertion order id.
+
+        Keyword Args:
+            offset (int): The (zero-based) starting offset in the collection.. [optional] if omitted the server will use the default value of 0
+            limit (int): The number of elements to be returned.. [optional] if omitted the server will use the default value of 25
+            limit_to_change_types (str): Comma separated change types string that will be queried.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            PageOfInsertionOrderHistoryChangeDataCapture
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['insertion_order_id'] = \
+            insertion_order_id
+        return self.get_insertion_order_history_change_data_capture_endpoint.call_with_http_info(**kwargs)
+
     def get_line_item_budget_overrides(
         self,
         line_item_id,
         **kwargs
     ):
         """get_line_item_budget_overrides  # noqa: E501
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api/gateway_api.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api/gateway_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2024_01.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_retailmedia_v2024_04.model.application_summary_model_response import ApplicationSummaryModelResponse
 
 
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
-                'endpoint_path': '/2024-01/retail-media/me',
+                'endpoint_path': '/2024-04/retail-media/me',
                 'operation_id': 'get_current_application',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api_client.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
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
 
 
-from criteo_api_retailmedia_v2024_01 import rest
-from criteo_api_retailmedia_v2024_01.configuration import Configuration
-from criteo_api_retailmedia_v2024_01.exceptions import ApiTypeError, ApiValueError, ApiException
-from criteo_api_retailmedia_v2024_01.model_utils import (
+from criteo_api_retailmedia_v2024_04 import rest
+from criteo_api_retailmedia_v2024_04.configuration import Configuration
+from criteo_api_retailmedia_v2024_04.exceptions import ApiTypeError, ApiValueError, ApiException
+from criteo_api_retailmedia_v2024_04.model_utils import (
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
 
@@ -799,19 +799,19 @@
 
         return params
 
     def __call__(self, *args, **kwargs):
         """ This method is invoked when endpoints are called
         Example:
 
-        api_instance = AnalyticsApi()
-        api_instance.generate_async_campaigns_report  # this is an instance of the class Endpoint
-        api_instance.generate_async_campaigns_report()  # this invokes api_instance.generate_async_campaigns_report.__call__()
+        api_instance = AccountsApi()
+        api_instance.add_brands  # this is an instance of the class Endpoint
+        api_instance.add_brands()  # this invokes api_instance.add_brands.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.generate_async_campaigns_report.callable or self.callable in this class
+        api_instance.add_brands.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
 
         try:
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/api_client_builder.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/api_client_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_retailmedia_v2024_01.configuration import Configuration
-from criteo_api_retailmedia_v2024_01.criteo_api_client import CriteoApiClient
-from criteo_api_retailmedia_v2024_01 import flow_constants
+from criteo_api_retailmedia_v2024_04.configuration import Configuration
+from criteo_api_retailmedia_v2024_04.criteo_api_client import CriteoApiClient
+from criteo_api_retailmedia_v2024_04 import flow_constants
 
 class ApiClientBuilder :
 
     @staticmethod
     def WithClientCredentials(clientId, clientSecret, host=None):
         configuration = Configuration(username=clientId, password=clientSecret, host=host)
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/apis/__init__.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/apis/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from criteo_api_retailmedia_v2024_01.api.analytics_api import AnalyticsApi
+#   from criteo_api_retailmedia_v2024_04.api.accounts_api import AccountsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from criteo_api_retailmedia_v2024_01.api.analytics_api import AnalyticsApi
-from criteo_api_retailmedia_v2024_01.api.audience_api import AudienceApi
-from criteo_api_retailmedia_v2024_01.api.campaign_api import CampaignApi
-from criteo_api_retailmedia_v2024_01.api.gateway_api import GatewayApi
+from criteo_api_retailmedia_v2024_04.api.accounts_api import AccountsApi
+from criteo_api_retailmedia_v2024_04.api.analytics_api import AnalyticsApi
+from criteo_api_retailmedia_v2024_04.api.audience_api import AudienceApi
+from criteo_api_retailmedia_v2024_04.api.campaign_api import CampaignApi
+from criteo_api_retailmedia_v2024_04.api.gateway_api import GatewayApi
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/configuration.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiValueError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiValueError
 
 
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
-        self.logger["package_logger"] = logging.getLogger("criteo_api_retailmedia_v2024_01")
+        self.logger["package_logger"] = logging.getLogger("criteo_api_retailmedia_v2024_04")
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

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/criteo_api_client.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/criteo_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from criteo_api_retailmedia_v2024_01.api_client import ApiClient
-from criteo_api_retailmedia_v2024_01.criteo_rest import CriteoRESTClientObject
+from criteo_api_retailmedia_v2024_04.api_client import ApiClient
+from criteo_api_retailmedia_v2024_04.criteo_rest import CriteoRESTClientObject
 
 class CriteoApiClient(ApiClient):
     def __init__(self, configuration=None, header_name=None, header_value=None,
              cookie=None, pool_threads=1, additional_parameters= {}):
         super().__init__(configuration=configuration,header_name=header_name, header_value=header_value, cookie=cookie, pool_threads=pool_threads)
         self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/criteo_auth.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/criteo_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from datetime import datetime, timedelta
-from criteo_api_retailmedia_v2024_01.exceptions import ApiException
-from criteo_api_retailmedia_v2024_01.api_client import ApiClient
-from criteo_api_retailmedia_v2024_01 import flow_constants
+from criteo_api_retailmedia_v2024_04.exceptions import ApiException
+from criteo_api_retailmedia_v2024_04.api_client import ApiClient
+from criteo_api_retailmedia_v2024_04 import flow_constants
 
 class Token(object):
 
     def __init__(self, token_string , expiration_date = None):
         self.expiration_date = expiration_date 
         self.token_string = token_string
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/criteo_rest.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/criteo_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_retailmedia_v2024_01.rest import RESTClientObject
-from criteo_api_retailmedia_v2024_01.criteo_auth import *
-from criteo_api_retailmedia_v2024_01 import flow_constants
+from criteo_api_retailmedia_v2024_04.rest import RESTClientObject
+from criteo_api_retailmedia_v2024_04.criteo_auth import *
+from criteo_api_retailmedia_v2024_04 import flow_constants
 
 
 class CriteoRESTClientObject(RESTClientObject):
 
     def __init__(self, configuration, additional_parameters = {}, pools_size=4, maxsize=None):
         super().__init__(configuration, pools_size, maxsize)
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/exceptions.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_funds_to_balance_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_funds_to_balance_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_add_funds_to_balance import ResourceOfAddFundsToBalance
+    from criteo_api_retailmedia_v2024_04.model.resource_of_add_funds_to_balance import ResourceOfAddFundsToBalance
     globals()['ResourceOfAddFundsToBalance'] = ResourceOfAddFundsToBalance
 
 
 class AddFundsToBalanceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keyword_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keyword_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.match_type_model import MatchTypeModel
+    from criteo_api_retailmedia_v2024_04.model.match_type_model import MatchTypeModel
     globals()['MatchTypeModel'] = MatchTypeModel
 
 
 class AddRemoveKeywordModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.add_remove_keyword_model import AddRemoveKeywordModel
+    from criteo_api_retailmedia_v2024_04.model.add_remove_keyword_model import AddRemoveKeywordModel
     globals()['AddRemoveKeywordModel'] = AddRemoveKeywordModel
 
 
 class AddRemoveKeywordsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.add_remove_keywords_model_resource import AddRemoveKeywordsModelResource
+    from criteo_api_retailmedia_v2024_04.model.add_remove_keywords_model_resource import AddRemoveKeywordsModelResource
     globals()['AddRemoveKeywordsModelResource'] = AddRemoveKeywordsModelResource
 
 
 class AddRemoveKeywordsModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_remove_keywords_model_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_remove_keywords_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.add_remove_keywords_model import AddRemoveKeywordsModel
+    from criteo_api_retailmedia_v2024_04.model.add_remove_keywords_model import AddRemoveKeywordsModel
     globals()['AddRemoveKeywordsModel'] = AddRemoveKeywordsModel
 
 
 class AddRemoveKeywordsModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_to_basket_ids_update_model202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_to_basket_ids_update_model202110_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
     globals()['ValueTypeResourceOfAddToBasketIdsUpdateModel202110'] = ValueTypeResourceOfAddToBasketIdsUpdateModel202110
 
 
 class AddToBasketIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_to_basket_target202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
     globals()['ValueTypeResourceOfAddToBasketTarget202110'] = ValueTypeResourceOfAddToBasketTarget202110
 
 
 class AddToBasketTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/add_to_basket_target202110_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfAddToBasketTarget202110'] = ValueTypeResourceOfAddToBasketTarget202110
 
 
 class AddToBasketTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/application_summary_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/application_summary_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ApplicationSummaryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/application_summary_model_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/application_summary_model_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.application_summary_model import ApplicationSummaryModel
+    from criteo_api_retailmedia_v2024_04.model.application_summary_model import ApplicationSummaryModel
     globals()['ApplicationSummaryModel'] = ApplicationSummaryModel
 
 
 class ApplicationSummaryModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/application_summary_model_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/application_summary_model_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
     globals()['ApplicationSummaryModelResource'] = ApplicationSummaryModelResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class ApplicationSummaryModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/approval_status_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/approval_status_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ApprovalStatusModel(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/asset.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class Asset(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/asset_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/asset_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.asset import Asset
+    from criteo_api_retailmedia_v2024_04.model.asset import Asset
     globals()['Asset'] = Asset
 
 
 class AssetResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/asset_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/asset_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.asset_resource import AssetResource
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.asset_resource import AssetResource
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
     globals()['AssetResource'] = AssetResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AssetResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_campaigns_report.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_campaigns_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AsyncCampaignsReport(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_campaigns_report_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.async_campaigns_report_resource import AsyncCampaignsReportResource
+    from criteo_api_retailmedia_v2024_04.model.async_campaigns_report_resource import AsyncCampaignsReportResource
     globals()['AsyncCampaignsReportResource'] = AsyncCampaignsReportResource
 
 
 class AsyncCampaignsReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_campaigns_report_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.async_campaigns_report import AsyncCampaignsReport
+    from criteo_api_retailmedia_v2024_04.model.async_campaigns_report import AsyncCampaignsReport
     globals()['AsyncCampaignsReport'] = AsyncCampaignsReport
 
 
 class AsyncCampaignsReportResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_line_items_report.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_line_items_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AsyncLineItemsReport(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_line_items_report_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_line_items_report_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.async_line_items_report_resource import AsyncLineItemsReportResource
+    from criteo_api_retailmedia_v2024_04.model.async_line_items_report_resource import AsyncLineItemsReportResource
     globals()['AsyncLineItemsReportResource'] = AsyncLineItemsReportResource
 
 
 class AsyncLineItemsReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_line_items_report_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_line_items_report_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.async_line_items_report import AsyncLineItemsReport
+    from criteo_api_retailmedia_v2024_04.model.async_line_items_report import AsyncLineItemsReport
     globals()['AsyncLineItemsReport'] = AsyncLineItemsReport
 
 
 class AsyncLineItemsReportResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_report_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_report_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.status_response_resource import StatusResponseResource
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.status_response_resource import StatusResponseResource
     globals()['CommonProblem'] = CommonProblem
     globals()['StatusResponseResource'] = StatusResponseResource
 
 
 class AsyncReportResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_revenue_report.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_revenue_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class AsyncRevenueReport(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_revenue_report_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_revenue_report_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.async_revenue_report_resource import AsyncRevenueReportResource
+    from criteo_api_retailmedia_v2024_04.model.async_revenue_report_resource import AsyncRevenueReportResource
     globals()['AsyncRevenueReportResource'] = AsyncRevenueReportResource
 
 
 class AsyncRevenueReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/async_revenue_report_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/async_revenue_report_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.async_revenue_report import AsyncRevenueReport
+    from criteo_api_retailmedia_v2024_04.model.async_revenue_report import AsyncRevenueReport
     globals()['AsyncRevenueReport'] = AsyncRevenueReport
 
 
 class AsyncRevenueReportResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_create_model_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_create_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
+    from criteo_api_retailmedia_v2024_04.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
     globals()['InputResourceOfAuctionLineItemCreateModel'] = InputResourceOfAuctionLineItemCreateModel
 
 
 class AuctionLineItemCreateModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_paged_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_paged_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfAuctionLineItem'] = ResourceOfAuctionLineItem
 
 
 class AuctionLineItemPagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfAuctionLineItem'] = ResourceOfAuctionLineItem
 
 
 class AuctionLineItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/auction_line_item_update_model_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/auction_line_item_update_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
+    from criteo_api_retailmedia_v2024_04.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
     globals()['ResourceOfAuctionLineItemUpdateModel'] = ResourceOfAuctionLineItemUpdateModel
 
 
 class AuctionLineItemUpdateModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/audience_ids_update_model202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/audience_ids_update_model202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
     globals()['ValueTypeResourceOfAudienceIdsUpdateModel202110'] = ValueTypeResourceOfAudienceIdsUpdateModel202110
 
 
 class AudienceIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/audience_target202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/audience_target202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
     globals()['ValueTypeResourceOfAudienceTarget202110'] = ValueTypeResourceOfAudienceTarget202110
 
 
 class AudienceTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/audience_target202110_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/audience_target202110_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfAudienceTarget202110'] = ValueTypeResourceOfAudienceTarget202110
 
 
 class AudienceTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_list_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/balance_campaign202110_list_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+    from criteo_api_retailmedia_v2024_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
     globals()['ResourceOfBalanceCampaign202110'] = ResourceOfBalanceCampaign202110
 
 
 class BalanceCampaign202110ListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_paged_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/balance_campaign202110_paged_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfBalanceCampaign202110'] = ResourceOfBalanceCampaign202110
 
 
 class BalanceCampaign202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_balance_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.resource_of_balance_response import ResourceOfBalanceResponse
-    globals()['CommonProblem'] = CommonProblem
-    globals()['ResourceOfBalanceResponse'] = ResourceOfBalanceResponse
+    from criteo_api_retailmedia_v2024_04.model.external_balance_response import ExternalBalanceResponse
+    globals()['ExternalBalanceResponse'] = ExternalBalanceResponse
 
 
-class BalanceResponse(ModelNormal):
+class ResourceOfBalanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,41 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (ResourceOfBalanceResponse,),  # noqa: E501
-            'warnings': ([CommonProblem],),  # noqa: E501
-            'errors': ([CommonProblem],),  # noqa: E501
+            'attributes': (ExternalBalanceResponse,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
+            'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
-        'warnings': 'warnings',  # noqa: E501
-        'errors': 'errors',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
-        'warnings',  # noqa: E501
-        'errors',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BalanceResponse - a model defined in OpenAPI
+        """ResourceOfBalanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfBalanceResponse): [optional]  # noqa: E501
-            warnings ([CommonProblem]): [optional]  # noqa: E501
-            errors ([CommonProblem]): [optional]  # noqa: E501
+            attributes (ExternalBalanceResponse): [optional]  # noqa: E501
+            id (str, none_type): Id of the entity. [optional]  # noqa: E501
+            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -199,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BalanceResponse - a model defined in OpenAPI
+        """ResourceOfBalanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,17 +228,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (ResourceOfBalanceResponse): [optional]  # noqa: E501
-            warnings ([CommonProblem]): [optional]  # noqa: E501
-            errors ([CommonProblem]): [optional]  # noqa: E501
+            attributes (ExternalBalanceResponse): [optional]  # noqa: E501
+            id (str, none_type): Id of the entity. [optional]  # noqa: E501
+            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/balance_response_paged_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/balance_response_paged_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2024_01.model.resource_of_balance_response import ResourceOfBalanceResponse
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.resource_of_balance_response import ResourceOfBalanceResponse
     globals()['CommonProblem'] = CommonProblem
     globals()['PageMetadata'] = PageMetadata
     globals()['ResourceOfBalanceResponse'] = ResourceOfBalanceResponse
 
 
 class BalanceResponsePagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_attributes_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_attributes_v202301.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CampaignAttributesV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_budget_overrides.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.campaign_daily_budget_override import CampaignDailyBudgetOverride
-    from criteo_api_retailmedia_v2024_01.model.campaign_monthly_budget_override import CampaignMonthlyBudgetOverride
+    from criteo_api_retailmedia_v2024_04.model.campaign_daily_budget_override import CampaignDailyBudgetOverride
+    from criteo_api_retailmedia_v2024_04.model.campaign_monthly_budget_override import CampaignMonthlyBudgetOverride
     globals()['CampaignDailyBudgetOverride'] = CampaignDailyBudgetOverride
     globals()['CampaignMonthlyBudgetOverride'] = CampaignMonthlyBudgetOverride
 
 
 class CampaignBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_daily_budget_override.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_daily_budget_override.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CampaignDailyBudgetOverride(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_monthly_budget_override.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_monthly_budget_override.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CampaignMonthlyBudgetOverride(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/campaign_v202301.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/category202204.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/category202204.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class Category202204(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/category202204_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/category202204_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_category202204 import ResourceOfCategory202204
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_category202204 import ResourceOfCategory202204
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCategory202204'] = ResourceOfCategory202204
 
 
 class Category202204ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/change_dates_of_balance_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/change_dates_of_balance_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_change_dates_of_balance import ResourceOfChangeDatesOfBalance
+    from criteo_api_retailmedia_v2024_04.model.resource_of_change_dates_of_balance import ResourceOfChangeDatesOfBalance
     globals()['ResourceOfChangeDatesOfBalance'] = ResourceOfChangeDatesOfBalance
 
 
 class ChangeDatesOfBalanceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/choice_option.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/choice_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.template_variable import TemplateVariable
+    from criteo_api_retailmedia_v2024_04.model.template_variable import TemplateVariable
     globals()['TemplateVariable'] = TemplateVariable
 
 
 class ChoiceOption(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/choice_variable_specification.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/choice_variable_specification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.choice_option import ChoiceOption
+    from criteo_api_retailmedia_v2024_04.model.choice_option import ChoiceOption
     globals()['ChoiceOption'] = ChoiceOption
 
 
 class ChoiceVariableSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/choice_variable_value.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/choice_variable_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ChoiceVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/color_variable_value.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/color_variable_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ColorVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_error.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CommonError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_line_item_paged_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_line_item_paged_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_common_line_item import ResourceOfCommonLineItem
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCommonLineItem'] = ResourceOfCommonLineItem
 
 
 class CommonLineItemPagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_line_item_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_line_item_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_common_line_item import ResourceOfCommonLineItem
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCommonLineItem'] = ResourceOfCommonLineItem
 
 
 class CommonLineItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_problem.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CommonProblem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/common_warning.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/common_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class CommonWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/create_balance_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/create_balance_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_create_balance import ResourceOfCreateBalance
+    from criteo_api_retailmedia_v2024_04.model.resource_of_create_balance import ResourceOfCreateBalance
     globals()['ResourceOfCreateBalance'] = ResourceOfCreateBalance
 
 
 class CreateBalanceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class Creative202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202110_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202110_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_creative202110 import ResourceOfCreative202110
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_creative202110 import ResourceOfCreative202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCreative202110'] = ResourceOfCreative202110
 
 
 class Creative202110ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202210.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202210.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.page_type_environment import PageTypeEnvironment
-    from criteo_api_retailmedia_v2024_01.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2024_04.model.page_type_environment import PageTypeEnvironment
+    from criteo_api_retailmedia_v2024_04.model.template_variable_value import TemplateVariableValue
     globals()['PageTypeEnvironment'] = PageTypeEnvironment
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class Creative202210(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202210_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202210_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_creative202210 import ResourceOfCreative202210
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_creative202210 import ResourceOfCreative202210
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCreative202210'] = ResourceOfCreative202210
 
 
 class Creative202210ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative202210_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative202210_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_creative202210 import ResourceOfCreative202210
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_creative202210 import ResourceOfCreative202210
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCreative202210'] = ResourceOfCreative202210
 
 
 class Creative202210Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative_create_model202207.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative_create_model202207.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2024_04.model.template_variable_value import TemplateVariableValue
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class CreativeCreateModel202207(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/creative_update_model202207.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/creative_update_model202207.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2024_04.model.template_variable_value import TemplateVariableValue
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class CreativeUpdateModel202207(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/daily_line_item_budget_override.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/daily_line_item_budget_override.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class DailyLineItemBudgetOverride(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/editable_campaign_attributes_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/editable_campaign_attributes_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class EditableCampaignAttributesV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_account.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_add_funds_to_balance.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_add_funds_to_balance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAddFundsToBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_ids_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_add_to_basket_ids_update_model202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAddToBasketIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_add_to_basket_target202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAddToBasketTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_auction_line_item.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_auction_line_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_create_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_auction_line_item_create_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItemCreateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_update_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_auction_line_item_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItemUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_audience_ids_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_audience_ids_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAudienceIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_audience_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_audience_target202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalAudienceTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_balance_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_balance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalBalanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_brand.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_brand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalBrand(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_catalog_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_catalog_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_catalog_status.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_catalog_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_change_dates_of_balance.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_change_dates_of_balance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalChangeDatesOfBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_common_line_item.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_common_line_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalCommonLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_create_balance.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_create_balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalCreateBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_keyword_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_keyword_target202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalKeywordTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_line_item_capping202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_line_item_capping202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalLineItemCapping202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_line_item_page202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_line_item_page202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
+    from criteo_api_retailmedia_v2024_04.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
     globals()['ExternalLineItemPageCategory202110'] = ExternalLineItemPageCategory202110
 
 
 class ExternalLineItemPage202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_line_item_page_category202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_line_item_page_category202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalLineItemPageCategory202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_preferred_line_item202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2024_01.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2024_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2024_04.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
 class ExternalPreferredLineItem202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_create_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_preferred_line_item_create_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2024_01.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2024_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2024_04.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
 class ExternalPreferredLineItemCreateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_preferred_line_item_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2024_01.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2024_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2024_04.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
 class ExternalPreferredLineItemUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_promoted_product202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_promoted_product202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalPromotedProduct202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_retailer.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_retailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalRetailer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_retailer_pages202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_retailer_pages202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalRetailerPages202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_store_ids_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_store_ids_update_model202110.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalStoreIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_store_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_store_target202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalStoreTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/external_update_balance_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/external_update_balance_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ExternalUpdateBalanceModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/files_variable_value.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/files_variable_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class FilesVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/files_variables_specification.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/files_variables_specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class FilesVariablesSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/hyperlink_variable_value.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/hyperlink_variable_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class HyperlinkVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/input_keywords_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/input_keywords_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class InputKeywordsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/input_resource_of_auction_line_item_create_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/input_resource_of_auction_line_item_create_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
+    from criteo_api_retailmedia_v2024_04.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
     globals()['ExternalAuctionLineItemCreateModel'] = ExternalAuctionLineItemCreateModel
 
 
 class InputResourceOfAuctionLineItemCreateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/input_resource_of_preferred_line_item_create_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/input_resource_of_preferred_line_item_create_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
+    from criteo_api_retailmedia_v2024_04.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
     globals()['ExternalPreferredLineItemCreateModel202110'] = ExternalPreferredLineItemCreateModel202110
 
 
 class InputResourceOfPreferredLineItemCreateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
+    from criteo_api_retailmedia_v2024_04.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
     globals()['EditableCampaignAttributesV202301'] = EditableCampaignAttributesV202301
 
 
 class JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_account_and_account.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_account_and_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_account import ExternalAccount
+    from criteo_api_retailmedia_v2024_04.model.external_account import ExternalAccount
     globals()['ExternalAccount'] = ExternalAccount
 
 
 class JsonApiBodyWithIdOfInt64AndAccountAndAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_brand import ExternalBrand
+    from criteo_api_retailmedia_v2024_04.model.external_brand import ExternalBrand
     globals()['ExternalBrand'] = ExternalBrand
 
 
 class JsonApiBodyWithIdOfInt64AndBrandAndBrand(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.campaign_v202301 import CampaignV202301
+    from criteo_api_retailmedia_v2024_04.model.campaign_v202301 import CampaignV202301
     globals()['CampaignV202301'] = CampaignV202301
 
 
 class JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_catalog_status import ExternalCatalogStatus
+    from criteo_api_retailmedia_v2024_04.model.external_catalog_status import ExternalCatalogStatus
     globals()['ExternalCatalogStatus'] = ExternalCatalogStatus
 
 
 class JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.line_item_bid_multipliers import LineItemBidMultipliers
+    from criteo_api_retailmedia_v2024_04.model.line_item_bid_multipliers import LineItemBidMultipliers
     globals()['LineItemBidMultipliers'] = LineItemBidMultipliers
 
 
 class JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_retailer import ExternalRetailer
+    from criteo_api_retailmedia_v2024_04.model.external_retailer import ExternalRetailer
     globals()['ExternalRetailer'] = ExternalRetailer
 
 
 class JsonApiBodyWithIdOfInt64AndRetailerAndRetailer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.campaign_attributes_v202301 import CampaignAttributesV202301
+    from criteo_api_retailmedia_v2024_04.model.campaign_attributes_v202301 import CampaignAttributesV202301
     globals()['CampaignAttributesV202301'] = CampaignAttributesV202301
 
 
 class JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_catalog_request import ExternalCatalogRequest
+    from criteo_api_retailmedia_v2024_04.model.external_catalog_request import ExternalCatalogRequest
     globals()['ExternalCatalogRequest'] = ExternalCatalogRequest
 
 
 class JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_account.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndAccountAndAccount'] = JsonApiBodyWithIdOfInt64AndAccountAndAccount
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfAccount(ModelNormal):
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_brand.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_brand.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndBrandAndBrand'] = JsonApiBodyWithIdOfInt64AndBrandAndBrand
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfBrand(ModelNormal):
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_campaign_v202301.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301'] = JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfCampaignV202301(ModelNormal):
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_retailer.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_page_response_of_retailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndRetailerAndRetailer'] = JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfRetailer(ModelNormal):
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_request_of_catalog_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_request_of_catalog_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
     globals()['JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest'] = JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
 
 
 class JsonApiRequestOfCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_campaign_v202301.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301'] = JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
 
 
 class JsonApiSingleResponseOfCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_catalog_status.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_catalog_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
+    from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus'] = JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
 
 
 class JsonApiSingleResponseOfCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_line_item_bid_multipliers.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/json_api_single_response_of_line_item_bid_multipliers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-    from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
+    from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+    from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers'] = JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
 
 
 class JsonApiSingleResponseOfLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keyword_data_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keyword_data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.input_keywords_model import InputKeywordsModel
-    from criteo_api_retailmedia_v2024_01.model.match_type_model import MatchTypeModel
-    from criteo_api_retailmedia_v2024_01.model.review_state_model import ReviewStateModel
+    from criteo_api_retailmedia_v2024_04.model.input_keywords_model import InputKeywordsModel
+    from criteo_api_retailmedia_v2024_04.model.match_type_model import MatchTypeModel
+    from criteo_api_retailmedia_v2024_04.model.review_state_model import ReviewStateModel
     globals()['InputKeywordsModel'] = InputKeywordsModel
     globals()['MatchTypeModel'] = MatchTypeModel
     globals()['ReviewStateModel'] = ReviewStateModel
 
 
 class KeywordDataModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keyword_target202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keyword_target202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
     globals()['ValueTypeResourceOfKeywordTarget202110'] = ValueTypeResourceOfKeywordTarget202110
 
 
 class KeywordTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keyword_target202110_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keyword_target202110_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfKeywordTarget202110'] = ValueTypeResourceOfKeywordTarget202110
 
 
 class KeywordTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keywords_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keywords_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.keyword_data_model import KeywordDataModel
+    from criteo_api_retailmedia_v2024_04.model.keyword_data_model import KeywordDataModel
     globals()['KeywordDataModel'] = KeywordDataModel
 
 
 class KeywordsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keywords_model_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keywords_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.keywords_model import KeywordsModel
+    from criteo_api_retailmedia_v2024_04.model.keywords_model import KeywordsModel
     globals()['KeywordsModel'] = KeywordsModel
 
 
 class KeywordsModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/keywords_model_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/keywords_model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.keywords_model_resource import KeywordsModelResource
-    from criteo_api_retailmedia_v2024_01.model.rmca_common_problem import RmcaCommonProblem
+    from criteo_api_retailmedia_v2024_04.model.keywords_model_resource import KeywordsModelResource
+    from criteo_api_retailmedia_v2024_04.model.rmca_common_problem import RmcaCommonProblem
     globals()['KeywordsModelResource'] = KeywordsModelResource
     globals()['RmcaCommonProblem'] = RmcaCommonProblem
 
 
 class KeywordsModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class LineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+    from criteo_api_retailmedia_v2024_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
     globals()['ResourceOfLineItemBidMultipliers'] = ResourceOfLineItemBidMultipliers
 
 
 class LineItemBidMultipliersRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_bid_multipliers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfLineItemBidMultipliers'] = ResourceOfLineItemBidMultipliers
 
 
 class LineItemBidMultipliersResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/line_item_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/line_item_budget_overrides.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.daily_line_item_budget_override import DailyLineItemBudgetOverride
-    from criteo_api_retailmedia_v2024_01.model.monthly_line_item_budeget_override import MonthlyLineItemBudegetOverride
+    from criteo_api_retailmedia_v2024_04.model.daily_line_item_budget_override import DailyLineItemBudgetOverride
+    from criteo_api_retailmedia_v2024_04.model.monthly_line_item_budeget_override import MonthlyLineItemBudegetOverride
     globals()['DailyLineItemBudgetOverride'] = DailyLineItemBudgetOverride
     globals()['MonthlyLineItemBudegetOverride'] = MonthlyLineItemBudegetOverride
 
 
 class LineItemBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/match_type_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/match_type_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class MatchTypeModel(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/monthly_line_item_budeget_override.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/monthly_line_item_budeget_override.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class MonthlyLineItemBudegetOverride(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/negotiation_state_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/negotiation_state_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class NegotiationStateModel(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/page_metadata.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/page_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PageMetadata(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/page_type_environment.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/page_type_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class PageTypeEnvironment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/post_campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/post_campaign_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
     globals()['JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301'] = JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
 
 
 class PostCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_paged_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item202110_paged_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPreferredLineItem202110'] = ResourceOfPreferredLineItem202110
 
 
 class PreferredLineItem202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item202110_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPreferredLineItem202110'] = ResourceOfPreferredLineItem202110
 
 
 class PreferredLineItem202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item_create_model202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item_create_model202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
+    from criteo_api_retailmedia_v2024_04.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
     globals()['InputResourceOfPreferredLineItemCreateModel202110'] = InputResourceOfPreferredLineItemCreateModel202110
 
 
 class PreferredLineItemCreateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/preferred_line_item_update_model202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/preferred_line_item_update_model202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
     globals()['ResourceOfPreferredLineItemUpdateModel202110'] = ResourceOfPreferredLineItemUpdateModel202110
 
 
 class PreferredLineItemUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/problem_details.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ProblemDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/promoted_product202110_list_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/promoted_product202110_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+    from criteo_api_retailmedia_v2024_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
     globals()['ResourceOfPromotedProduct202110'] = ResourceOfPromotedProduct202110
 
 
 class PromotedProduct202110ListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/promoted_product202110_paged_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/promoted_product202110_paged_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+    from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPromotedProduct202110'] = ResourceOfPromotedProduct202110
 
 
 class PromotedProduct202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/proposal_status_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/proposal_status_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.approval_status_model import ApprovalStatusModel
-    from criteo_api_retailmedia_v2024_01.model.negotiation_state_model import NegotiationStateModel
+    from criteo_api_retailmedia_v2024_04.model.approval_status_model import ApprovalStatusModel
+    from criteo_api_retailmedia_v2024_04.model.negotiation_state_model import NegotiationStateModel
     globals()['ApprovalStatusModel'] = ApprovalStatusModel
     globals()['NegotiationStateModel'] = NegotiationStateModel
 
 
 class ProposalStatusModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/proposal_status_model_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/proposal_status_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.proposal_status_model import ProposalStatusModel
+    from criteo_api_retailmedia_v2024_04.model.proposal_status_model import ProposalStatusModel
     globals()['ProposalStatusModel'] = ProposalStatusModel
 
 
 class ProposalStatusModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/proposal_status_model_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/proposal_status_model_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.proposal_status_model_resource import ProposalStatusModelResource
-    from criteo_api_retailmedia_v2024_01.model.rmca_common_problem import RmcaCommonProblem
+    from criteo_api_retailmedia_v2024_04.model.proposal_status_model_resource import ProposalStatusModelResource
+    from criteo_api_retailmedia_v2024_04.model.rmca_common_problem import RmcaCommonProblem
     globals()['ProposalStatusModelResource'] = ProposalStatusModelResource
     globals()['RmcaCommonProblem'] = RmcaCommonProblem
 
 
 class ProposalStatusModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/put_campaign_v202301.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/put_campaign_v202301.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2024_04.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
     globals()['JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301'] = JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
 
 
 class PutCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/report_outcome.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/report_outcome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
     globals()['CommonProblem'] = CommonProblem
 
 
 class ReportOutcome(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_add_funds_to_balance.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_add_funds_to_balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_add_funds_to_balance import ExternalAddFundsToBalance
+    from criteo_api_retailmedia_v2024_04.model.external_add_funds_to_balance import ExternalAddFundsToBalance
     globals()['ExternalAddFundsToBalance'] = ExternalAddFundsToBalance
 
 
 class ResourceOfAddFundsToBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_auction_line_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_auction_line_item import ExternalAuctionLineItem
+    from criteo_api_retailmedia_v2024_04.model.external_auction_line_item import ExternalAuctionLineItem
     globals()['ExternalAuctionLineItem'] = ExternalAuctionLineItem
 
 
 class ResourceOfAuctionLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item_update_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_auction_line_item_update_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
+    from criteo_api_retailmedia_v2024_04.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
     globals()['ExternalAuctionLineItemUpdateModel'] = ExternalAuctionLineItemUpdateModel
 
 
 class ResourceOfAuctionLineItemUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_balance_campaign202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_balance_campaign202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ResourceOfBalanceCampaign202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_balance_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_common_line_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_balance_response import ExternalBalanceResponse
-    globals()['ExternalBalanceResponse'] = ExternalBalanceResponse
+    from criteo_api_retailmedia_v2024_04.model.external_common_line_item import ExternalCommonLineItem
+    globals()['ExternalCommonLineItem'] = ExternalCommonLineItem
 
 
-class ResourceOfBalanceResponse(ModelNormal):
+class ResourceOfCommonLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (ExternalBalanceResponse,),  # noqa: E501
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
+            'attributes': (ExternalCommonLineItem,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfBalanceResponse - a model defined in OpenAPI
+        """ResourceOfCommonLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (ExternalBalanceResponse): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfBalanceResponse - a model defined in OpenAPI
+        """ResourceOfCommonLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +228,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (ExternalBalanceResponse): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_category202204.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_category202204.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.category202204 import Category202204
+    from criteo_api_retailmedia_v2024_04.model.category202204 import Category202204
     globals()['Category202204'] = Category202204
 
 
 class ResourceOfCategory202204(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_change_dates_of_balance.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_change_dates_of_balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_change_dates_of_balance import ExternalChangeDatesOfBalance
+    from criteo_api_retailmedia_v2024_04.model.external_change_dates_of_balance import ExternalChangeDatesOfBalance
     globals()['ExternalChangeDatesOfBalance'] = ExternalChangeDatesOfBalance
 
 
 class ResourceOfChangeDatesOfBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_common_line_item.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_preferred_line_item202110.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_common_line_item import ExternalCommonLineItem
-    globals()['ExternalCommonLineItem'] = ExternalCommonLineItem
+    from criteo_api_retailmedia_v2024_04.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
+    globals()['ExternalPreferredLineItem202110'] = ExternalPreferredLineItem202110
 
 
-class ResourceOfCommonLineItem(ModelNormal):
+class ResourceOfPreferredLineItem202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
-            'attributes': (ExternalCommonLineItem,),  # noqa: E501
+            'attributes': (ExternalPreferredLineItem202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfCommonLineItem - a model defined in OpenAPI
+        """ResourceOfPreferredLineItem202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
+            attributes (ExternalPreferredLineItem202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfCommonLineItem - a model defined in OpenAPI
+        """ResourceOfPreferredLineItem202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,15 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalCommonLineItem): [optional]  # noqa: E501
+            attributes (ExternalPreferredLineItem202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_create_balance.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_create_balance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_create_balance import ExternalCreateBalance
+    from criteo_api_retailmedia_v2024_04.model.external_create_balance import ExternalCreateBalance
     globals()['ExternalCreateBalance'] = ExternalCreateBalance
 
 
 class ResourceOfCreateBalance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_creative202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_creative202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.creative202110 import Creative202110
+    from criteo_api_retailmedia_v2024_04.model.creative202110 import Creative202110
     globals()['Creative202110'] = Creative202110
 
 
 class ResourceOfCreative202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_creative202210.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_creative202210.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.creative202210 import Creative202210
+    from criteo_api_retailmedia_v2024_04.model.creative202210 import Creative202210
     globals()['Creative202210'] = Creative202210
 
 
 class ResourceOfCreative202210(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_line_item_bid_multipliers.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_line_item_bid_multipliers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.line_item_bid_multipliers import LineItemBidMultipliers
+    from criteo_api_retailmedia_v2024_04.model.line_item_bid_multipliers import LineItemBidMultipliers
     globals()['LineItemBidMultipliers'] = LineItemBidMultipliers
 
 
 class ResourceOfLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_preferred_line_item_update_model202110.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
-    globals()['ExternalPreferredLineItem202110'] = ExternalPreferredLineItem202110
+    from criteo_api_retailmedia_v2024_04.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
+    globals()['ExternalPreferredLineItemUpdateModel202110'] = ExternalPreferredLineItemUpdateModel202110
 
 
-class ResourceOfPreferredLineItem202110(ModelNormal):
+class ResourceOfPreferredLineItemUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
-            'attributes': (ExternalPreferredLineItem202110,),  # noqa: E501
+            'attributes': (ExternalPreferredLineItemUpdateModel202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfPreferredLineItem202110 - a model defined in OpenAPI
+        """ResourceOfPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalPreferredLineItem202110): [optional]  # noqa: E501
+            attributes (ExternalPreferredLineItemUpdateModel202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfPreferredLineItem202110 - a model defined in OpenAPI
+        """ResourceOfPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,15 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalPreferredLineItem202110): [optional]  # noqa: E501
+            attributes (ExternalPreferredLineItemUpdateModel202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
-    globals()['ExternalPreferredLineItemUpdateModel202110'] = ExternalPreferredLineItemUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.template import Template
+    globals()['Template'] = Template
 
 
-class ResourceOfPreferredLineItemUpdateModel202110(ModelNormal):
+class ResourceOfTemplate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'attributes': (Template,),  # noqa: E501
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
-            'attributes': (ExternalPreferredLineItemUpdateModel202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'attributes': 'attributes',  # noqa: E501
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
+        """ResourceOfTemplate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            attributes (Template): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalPreferredLineItemUpdateModel202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfPreferredLineItemUpdateModel202110 - a model defined in OpenAPI
+        """ResourceOfTemplate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +228,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            attributes (Template): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalPreferredLineItemUpdateModel202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_promoted_product202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_promoted_product202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_promoted_product202110 import ExternalPromotedProduct202110
+    from criteo_api_retailmedia_v2024_04.model.external_promoted_product202110 import ExternalPromotedProduct202110
     globals()['ExternalPromotedProduct202110'] = ExternalPromotedProduct202110
 
 
 class ResourceOfPromotedProduct202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_template.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bids_model_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.template import Template
-    globals()['Template'] = Template
+    from criteo_api_retailmedia_v2024_04.model.set_bids_model import SetBidsModel
+    globals()['SetBidsModel'] = SetBidsModel
 
 
-class ResourceOfTemplate(ModelNormal):
+class SetBidsModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -83,39 +76,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (Template,),  # noqa: E501
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
+            'attributes': (SetBidsModel,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfTemplate - a model defined in OpenAPI
+        """SetBidsModelResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +133,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (Template): [optional]  # noqa: E501
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            id (str, none_type): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
+            attributes (SetBidsModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfTemplate - a model defined in OpenAPI
+        """SetBidsModelResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +221,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (Template): [optional]  # noqa: E501
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
-            type (str, none_type): Canonical type name of the entity. [optional]  # noqa: E501
+            id (str, none_type): [optional]  # noqa: E501
+            type (str, none_type): [optional]  # noqa: E501
+            attributes (SetBidsModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_of_update_balance_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_of_update_balance_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_update_balance_model import ExternalUpdateBalanceModel
+    from criteo_api_retailmedia_v2024_04.model.external_update_balance_model import ExternalUpdateBalanceModel
     globals()['ExternalUpdateBalanceModel'] = ExternalUpdateBalanceModel
 
 
 class ResourceOfUpdateBalanceModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/resource_outcome.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/resource_outcome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rmca_common_problem import RmcaCommonProblem
+    from criteo_api_retailmedia_v2024_04.model.rmca_common_problem import RmcaCommonProblem
     globals()['RmcaCommonProblem'] = RmcaCommonProblem
 
 
 class ResourceOutcome(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/review_state_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/review_state_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class ReviewStateModel(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RmLegacyAudienceCreateEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v1 import RmLegacyAudienceCreateEntityV1
-    globals()['RmLegacyAudienceCreateEntityV1'] = RmLegacyAudienceCreateEntityV1
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v2 import RmLegacyAudienceCreateEntityV2
+    globals()['RmLegacyAudienceCreateEntityV2'] = RmLegacyAudienceCreateEntityV2
 
 
-class RmLegacyAudienceCreateEntityV1Resource(ModelNormal):
+class RmLegacyAudienceCreateEntityV2Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (RmLegacyAudienceCreateEntityV1,),  # noqa: E501
+            'attributes': (RmLegacyAudienceCreateEntityV2,),  # noqa: E501
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RmLegacyAudienceCreateEntityV1Resource - a model defined in OpenAPI
+        """RmLegacyAudienceCreateEntityV2Resource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +140,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (RmLegacyAudienceCreateEntityV1): [optional]  # noqa: E501
+            attributes (RmLegacyAudienceCreateEntityV2): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RmLegacyAudienceCreateEntityV1Resource - a model defined in OpenAPI
+        """RmLegacyAudienceCreateEntityV2Resource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,15 +228,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (RmLegacyAudienceCreateEntityV1): [optional]  # noqa: E501
+            attributes (RmLegacyAudienceCreateEntityV2): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v1_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v1_resource import RmLegacyAudienceCreateEntityV1Resource
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v1_resource import RmLegacyAudienceCreateEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
     globals()['RmLegacyAudienceCreateEntityV1Resource'] = RmLegacyAudienceCreateEntityV1Resource
 
 
 class RmLegacyAudienceCreateEntityV1Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_user_behavior_create_v2 import RmLegacyAudienceUserBehaviorCreateV2
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_user_behavior_create_v2 import RmLegacyAudienceUserBehaviorCreateV2
     globals()['RmLegacyAudienceUserBehaviorCreateV2'] = RmLegacyAudienceUserBehaviorCreateV2
 
 
 class RmLegacyAudienceCreateEntityV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v2 import RmLegacyAudienceCreateEntityV2
-    globals()['RmLegacyAudienceCreateEntityV2'] = RmLegacyAudienceCreateEntityV2
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v2 import RmLegacyAudienceGetEntityV2
+    globals()['RmLegacyAudienceGetEntityV2'] = RmLegacyAudienceGetEntityV2
 
 
-class RmLegacyAudienceCreateEntityV2Resource(ModelNormal):
+class RmLegacyAudienceGetEntityV2Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,15 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (RmLegacyAudienceCreateEntityV2,),  # noqa: E501
+            'attributes': (RmLegacyAudienceGetEntityV2,),  # noqa: E501
             'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RmLegacyAudienceCreateEntityV2Resource - a model defined in OpenAPI
+        """RmLegacyAudienceGetEntityV2Resource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,15 +140,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (RmLegacyAudienceCreateEntityV2): [optional]  # noqa: E501
+            attributes (RmLegacyAudienceGetEntityV2): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RmLegacyAudienceCreateEntityV2Resource - a model defined in OpenAPI
+        """RmLegacyAudienceGetEntityV2Resource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,15 +228,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (RmLegacyAudienceCreateEntityV2): [optional]  # noqa: E501
+            attributes (RmLegacyAudienceGetEntityV2): [optional]  # noqa: E501
             id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_entity_v2_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v2_resource import RmLegacyAudienceCreateEntityV2Resource
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v2_resource import RmLegacyAudienceCreateEntityV2Resource
     globals()['CommonProblem'] = CommonProblem
     globals()['RmLegacyAudienceCreateEntityV2Resource'] = RmLegacyAudienceCreateEntityV2Resource
 
 
 class RmLegacyAudienceCreateEntityV2Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v1.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_input_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v1_resource import RmLegacyAudienceCreateEntityV1Resource
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v1_resource import RmLegacyAudienceCreateEntityV1Resource
     globals()['RmLegacyAudienceCreateEntityV1Resource'] = RmLegacyAudienceCreateEntityV1Resource
 
 
 class RmLegacyAudienceCreateInputEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v2.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_create_input_entity_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v2_resource import RmLegacyAudienceCreateEntityV2Resource
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v2_resource import RmLegacyAudienceCreateEntityV2Resource
     globals()['RmLegacyAudienceCreateEntityV2Resource'] = RmLegacyAudienceCreateEntityV2Resource
 
 
 class RmLegacyAudienceCreateInputEntityV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_customer_list import RmLegacySegmentCustomerList
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_user_behavior_v1 import RmLegacySegmentUserBehaviorV1
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_customer_list import RmLegacySegmentCustomerList
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_user_behavior_v1 import RmLegacySegmentUserBehaviorV1
     globals()['RmLegacySegmentCustomerList'] = RmLegacySegmentCustomerList
     globals()['RmLegacySegmentUserBehaviorV1'] = RmLegacySegmentUserBehaviorV1
 
 
 class RmLegacyAudienceGetEntityV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v1_resource import RmLegacyAudienceGetEntityV1Resource
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v1_resource import RmLegacyAudienceGetEntityV1Resource
     globals()['CommonProblem'] = CommonProblem
     globals()['RmLegacyAudienceGetEntityV1Resource'] = RmLegacyAudienceGetEntityV1Resource
 
 
 class RmLegacyAudienceGetEntityV1ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v1_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v1 import RmLegacyAudienceGetEntityV1
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v1 import RmLegacyAudienceGetEntityV1
     globals()['RmLegacyAudienceGetEntityV1'] = RmLegacyAudienceGetEntityV1
 
 
 class RmLegacyAudienceGetEntityV1Resource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_user_behavior_details_v2 import RmLegacyAudienceUserBehaviorDetailsV2
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_customer_list import RmLegacySegmentCustomerList
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_user_behavior_details_v2 import RmLegacyAudienceUserBehaviorDetailsV2
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_customer_list import RmLegacySegmentCustomerList
     globals()['RmLegacyAudienceUserBehaviorDetailsV2'] = RmLegacyAudienceUserBehaviorDetailsV2
     globals()['RmLegacySegmentCustomerList'] = RmLegacySegmentCustomerList
 
 
 class RmLegacyAudienceGetEntityV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_get_entity_v2_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v2_resource import RmLegacyAudienceGetEntityV2Resource
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v2_resource import RmLegacyAudienceGetEntityV2Resource
     globals()['CommonProblem'] = CommonProblem
     globals()['RmLegacyAudienceGetEntityV2Resource'] = RmLegacyAudienceGetEntityV2Resource
 
 
 class RmLegacyAudienceGetEntityV2ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_of_campaign_budget_overrides.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v2 import RmLegacyAudienceGetEntityV2
-    globals()['RmLegacyAudienceGetEntityV2'] = RmLegacyAudienceGetEntityV2
+    from criteo_api_retailmedia_v2024_04.model.campaign_budget_overrides import CampaignBudgetOverrides
+    globals()['CampaignBudgetOverrides'] = CampaignBudgetOverrides
 
 
-class RmLegacyAudienceGetEntityV2Resource(ModelNormal):
+class ValueResourceOfCampaignBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -83,39 +76,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (RmLegacyAudienceGetEntityV2,),  # noqa: E501
-            'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
+            'attributes': (CampaignBudgetOverrides,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RmLegacyAudienceGetEntityV2Resource - a model defined in OpenAPI
+        """ValueResourceOfCampaignBudgetOverrides - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (RmLegacyAudienceGetEntityV2): [optional]  # noqa: E501
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
+            attributes (CampaignBudgetOverrides): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RmLegacyAudienceGetEntityV2Resource - a model defined in OpenAPI
+        """ValueResourceOfCampaignBudgetOverrides - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +218,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attributes (RmLegacyAudienceGetEntityV2): [optional]  # noqa: E501
-            id (str, none_type): Id of the entity. [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
+            attributes (CampaignBudgetOverrides): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_create_v2.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_user_behavior_create_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_user_behavior_create_v2 import RmLegacySegmentUserBehaviorCreateV2
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_user_behavior_create_v2 import RmLegacySegmentUserBehaviorCreateV2
     globals()['RmLegacySegmentUserBehaviorCreateV2'] = RmLegacySegmentUserBehaviorCreateV2
 
 
 class RmLegacyAudienceUserBehaviorCreateV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_details_v2.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_audience_user_behavior_details_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_user_behavior_v2 import RmLegacySegmentUserBehaviorV2
+    from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_user_behavior_v2 import RmLegacySegmentUserBehaviorV2
     globals()['RmLegacySegmentUserBehaviorV2'] = RmLegacySegmentUserBehaviorV2
 
 
 class RmLegacyAudienceUserBehaviorDetailsV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_customer_list.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_customer_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RmLegacySegmentCustomerList(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_create_v2.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_create_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RmLegacySegmentUserBehaviorCreateV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v1.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RmLegacySegmentUserBehaviorV1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v2.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rm_legacy_segment_user_behavior_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RmLegacySegmentUserBehaviorV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/rmca_common_problem.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/rmca_common_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class RmcaCommonProblem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/section.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/section.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.template_variable import TemplateVariable
+    from criteo_api_retailmedia_v2024_04.model.template_variable import TemplateVariable
     globals()['TemplateVariable'] = TemplateVariable
 
 
 class Section(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bid_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bid_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class SetBidModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bids_model.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bids_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.set_bid_model import SetBidModel
+    from criteo_api_retailmedia_v2024_04.model.set_bid_model import SetBidModel
     globals()['SetBidModel'] = SetBidModel
 
 
 class SetBidsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bids_model_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/set_bids_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.set_bids_model_resource import SetBidsModelResource
+    from criteo_api_retailmedia_v2024_04.model.set_bids_model_resource import SetBidsModelResource
     globals()['SetBidsModelResource'] = SetBidsModelResource
 
 
 class SetBidsModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/set_bids_model_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_of_retail_media_brands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.set_bids_model import SetBidsModel
-    globals()['SetBidsModel'] = SetBidsModel
+    from criteo_api_retailmedia_v2024_04.model.retail_media_brands import RetailMediaBrands
+    globals()['RetailMediaBrands'] = RetailMediaBrands
 
 
-class SetBidsModelResource(ModelNormal):
+class ValueResourceOfRetailMediaBrands(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,39 +76,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, none_type,),  # noqa: E501
             'type': (str, none_type,),  # noqa: E501
-            'attributes': (SetBidsModel,),  # noqa: E501
+            'attributes': (RetailMediaBrands,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SetBidsModelResource - a model defined in OpenAPI
+        """ValueResourceOfRetailMediaBrands - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,17 +131,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str, none_type): [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
-            attributes (SetBidsModel): [optional]  # noqa: E501
+            attributes (RetailMediaBrands): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SetBidsModelResource - a model defined in OpenAPI
+        """ValueResourceOfRetailMediaBrands - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,17 +218,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str, none_type): [optional]  # noqa: E501
             type (str, none_type): [optional]  # noqa: E501
-            attributes (SetBidsModel): [optional]  # noqa: E501
+            attributes (RetailMediaBrands): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/status_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/status_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class StatusResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/status_response_resource.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/status_response_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.status_response import StatusResponse
+    from criteo_api_retailmedia_v2024_04.model.status_response import StatusResponse
     globals()['StatusResponse'] = StatusResponse
 
 
 class StatusResponseResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/store_ids_update_model202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/store_ids_update_model202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
     globals()['ValueTypeResourceOfStoreIdsUpdateModel202110'] = ValueTypeResourceOfStoreIdsUpdateModel202110
 
 
 class StoreIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/store_target202110_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/store_target202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
     globals()['ValueTypeResourceOfStoreTarget202110'] = ValueTypeResourceOfStoreTarget202110
 
 
 class StoreTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/store_target202110_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/store_target202110_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfStoreTarget202110'] = ValueTypeResourceOfStoreTarget202110
 
 
 class StoreTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.section import Section
+    from criteo_api_retailmedia_v2024_04.model.section import Section
     globals()['Section'] = Section
 
 
 class Template(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_list_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_template import ResourceOfTemplate
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_template import ResourceOfTemplate
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfTemplate'] = ResourceOfTemplate
 
 
 class TemplateListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_response.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2024_01.model.resource_of_template import ResourceOfTemplate
+    from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2024_04.model.resource_of_template import ResourceOfTemplate
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfTemplate'] = ResourceOfTemplate
 
 
 class TemplateResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_variable.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.choice_variable_specification import ChoiceVariableSpecification
-    from criteo_api_retailmedia_v2024_01.model.files_variables_specification import FilesVariablesSpecification
-    from criteo_api_retailmedia_v2024_01.model.text_variable_specification import TextVariableSpecification
+    from criteo_api_retailmedia_v2024_04.model.choice_variable_specification import ChoiceVariableSpecification
+    from criteo_api_retailmedia_v2024_04.model.files_variables_specification import FilesVariablesSpecification
+    from criteo_api_retailmedia_v2024_04.model.text_variable_specification import TextVariableSpecification
     globals()['ChoiceVariableSpecification'] = ChoiceVariableSpecification
     globals()['FilesVariablesSpecification'] = FilesVariablesSpecification
     globals()['TextVariableSpecification'] = TextVariableSpecification
 
 
 class TemplateVariable(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/template_variable_value.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/template_variable_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.choice_variable_value import ChoiceVariableValue
-    from criteo_api_retailmedia_v2024_01.model.color_variable_value import ColorVariableValue
-    from criteo_api_retailmedia_v2024_01.model.files_variable_value import FilesVariableValue
-    from criteo_api_retailmedia_v2024_01.model.hyperlink_variable_value import HyperlinkVariableValue
-    from criteo_api_retailmedia_v2024_01.model.text_variable_value import TextVariableValue
+    from criteo_api_retailmedia_v2024_04.model.choice_variable_value import ChoiceVariableValue
+    from criteo_api_retailmedia_v2024_04.model.color_variable_value import ColorVariableValue
+    from criteo_api_retailmedia_v2024_04.model.files_variable_value import FilesVariableValue
+    from criteo_api_retailmedia_v2024_04.model.hyperlink_variable_value import HyperlinkVariableValue
+    from criteo_api_retailmedia_v2024_04.model.text_variable_value import TextVariableValue
     globals()['ChoiceVariableValue'] = ChoiceVariableValue
     globals()['ColorVariableValue'] = ColorVariableValue
     globals()['FilesVariableValue'] = FilesVariableValue
     globals()['HyperlinkVariableValue'] = HyperlinkVariableValue
     globals()['TextVariableValue'] = TextVariableValue
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/text_variable_specification.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/text_variable_specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class TextVariableSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/text_variable_value.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/text_variable_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 
 class TextVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/update_balance_model_request.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/update_balance_model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.resource_of_update_balance_model import ResourceOfUpdateBalanceModel
+    from criteo_api_retailmedia_v2024_04.model.resource_of_update_balance_model import ResourceOfUpdateBalanceModel
     globals()['ResourceOfUpdateBalanceModel'] = ResourceOfUpdateBalanceModel
 
 
 class UpdateBalanceModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_campaign_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_input_of_campaign_budget_overrides.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_resource_of_campaign_budget_overrides import ValueResourceOfCampaignBudgetOverrides
+    from criteo_api_retailmedia_v2024_04.model.value_resource_of_campaign_budget_overrides import ValueResourceOfCampaignBudgetOverrides
     globals()['ValueResourceOfCampaignBudgetOverrides'] = ValueResourceOfCampaignBudgetOverrides
 
 
 class ValueResourceInputOfCampaignBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_line_item_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_input_of_line_item_budget_overrides.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.value_resource_of_line_item_budget_overrides import ValueResourceOfLineItemBudgetOverrides
+    from criteo_api_retailmedia_v2024_04.model.value_resource_of_line_item_budget_overrides import ValueResourceOfLineItemBudgetOverrides
     globals()['ValueResourceOfLineItemBudgetOverrides'] = ValueResourceOfLineItemBudgetOverrides
 
 
 class ValueResourceInputOfLineItemBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_of_campaign_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_add_to_basket_target202110.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.campaign_budget_overrides import CampaignBudgetOverrides
-    globals()['CampaignBudgetOverrides'] = CampaignBudgetOverrides
+    from criteo_api_retailmedia_v2024_04.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
+    globals()['ExternalAddToBasketTarget202110'] = ExternalAddToBasketTarget202110
 
 
-class ValueResourceOfCampaignBudgetOverrides(ModelNormal):
+class ValueTypeResourceOfAddToBasketTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,15 +60,22 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -76,16 +83,16 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (str, none_type,),  # noqa: E501
-            'attributes': (CampaignBudgetOverrides,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': (ExternalAddToBasketTarget202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -98,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValueResourceOfCampaignBudgetOverrides - a model defined in OpenAPI
+        """ValueTypeResourceOfAddToBasketTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str, none_type): [optional]  # noqa: E501
-            attributes (CampaignBudgetOverrides): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalAddToBasketTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValueResourceOfCampaignBudgetOverrides - a model defined in OpenAPI
+        """ValueTypeResourceOfAddToBasketTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,16 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str, none_type): [optional]  # noqa: E501
-            attributes (CampaignBudgetOverrides): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalAddToBasketTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_of_line_item_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_of_line_item_budget_overrides.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.line_item_budget_overrides import LineItemBudgetOverrides
+    from criteo_api_retailmedia_v2024_04.model.line_item_budget_overrides import LineItemBudgetOverrides
     globals()['LineItemBudgetOverrides'] = LineItemBudgetOverrides
 
 
 class ValueResourceOfLineItemBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_campaign_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_outcome_of_campaign_budget_overrides.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.value_resource_of_campaign_budget_overrides import ValueResourceOfCampaignBudgetOverrides
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.value_resource_of_campaign_budget_overrides import ValueResourceOfCampaignBudgetOverrides
     globals()['CommonProblem'] = CommonProblem
     globals()['ValueResourceOfCampaignBudgetOverrides'] = ValueResourceOfCampaignBudgetOverrides
 
 
 class ValueResourceOutcomeOfCampaignBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_line_item_budget_overrides.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_outcome_of_line_item_budget_overrides.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2024_01.model.value_resource_of_line_item_budget_overrides import ValueResourceOfLineItemBudgetOverrides
+    from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2024_04.model.value_resource_of_line_item_budget_overrides import ValueResourceOfLineItemBudgetOverrides
     globals()['CommonProblem'] = CommonProblem
     globals()['ValueResourceOfLineItemBudgetOverrides'] = ValueResourceOfLineItemBudgetOverrides
 
 
 class ValueResourceOutcomeOfLineItemBudgetOverrides(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
     globals()['ExternalAddToBasketIdsUpdateModel202110'] = ExternalAddToBasketIdsUpdateModel202110
 
 
 class ValueTypeResourceOfAddToBasketIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_audience_target202110.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
-    globals()['ExternalAddToBasketTarget202110'] = ExternalAddToBasketTarget202110
+    from criteo_api_retailmedia_v2024_04.model.external_audience_target202110 import ExternalAudienceTarget202110
+    globals()['ExternalAudienceTarget202110'] = ExternalAudienceTarget202110
 
 
-class ValueTypeResourceOfAddToBasketTarget202110(ModelNormal):
+class ValueTypeResourceOfAudienceTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalAddToBasketTarget202110,),  # noqa: E501
+            'attributes': (ExternalAudienceTarget202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfAddToBasketTarget202110 - a model defined in OpenAPI
+        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +139,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             type (str): [optional]  # noqa: E501
-            attributes (ExternalAddToBasketTarget202110): [optional]  # noqa: E501
+            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfAddToBasketTarget202110 - a model defined in OpenAPI
+        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +226,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             type (str): [optional]  # noqa: E501
-            attributes (ExternalAddToBasketTarget202110): [optional]  # noqa: E501
+            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_ids_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_audience_ids_update_model202110.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
     globals()['ExternalAudienceIdsUpdateModel202110'] = ExternalAudienceIdsUpdateModel202110
 
 
 class ValueTypeResourceOfAudienceIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_store_target202110.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_audience_target202110 import ExternalAudienceTarget202110
-    globals()['ExternalAudienceTarget202110'] = ExternalAudienceTarget202110
+    from criteo_api_retailmedia_v2024_04.model.external_store_target202110 import ExternalStoreTarget202110
+    globals()['ExternalStoreTarget202110'] = ExternalStoreTarget202110
 
 
-class ValueTypeResourceOfAudienceTarget202110(ModelNormal):
+class ValueTypeResourceOfStoreTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalAudienceTarget202110,),  # noqa: E501
+            'attributes': (ExternalStoreTarget202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +139,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             type (str): [optional]  # noqa: E501
-            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
+            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +226,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             type (str): [optional]  # noqa: E501
-            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
+            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_keyword_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_keyword_target202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_keyword_target202110 import ExternalKeywordTarget202110
+    from criteo_api_retailmedia_v2024_04.model.external_keyword_target202110 import ExternalKeywordTarget202110
     globals()['ExternalKeywordTarget202110'] = ExternalKeywordTarget202110
 
 
 class ValueTypeResourceOfKeywordTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_ids_update_model202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_type_resource_of_store_ids_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
+    from criteo_api_retailmedia_v2024_04.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
     globals()['ExternalStoreIdsUpdateModel202110'] = ExternalStoreIdsUpdateModel202110
 
 
 class ValueTypeResourceOfStoreIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_target202110.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model/value_resource_input_of_retail_media_brands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2024-01
+    The version of the OpenAPI document: 2024-04
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2024_01.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2024_04.model_utils import (  # noqa: F401
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
-from criteo_api_retailmedia_v2024_01.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2024_01.model.external_store_target202110 import ExternalStoreTarget202110
-    globals()['ExternalStoreTarget202110'] = ExternalStoreTarget202110
+    from criteo_api_retailmedia_v2024_04.model.value_resource_of_retail_media_brands import ValueResourceOfRetailMediaBrands
+    globals()['ValueResourceOfRetailMediaBrands'] = ValueResourceOfRetailMediaBrands
 
 
-class ValueTypeResourceOfStoreTarget202110(ModelNormal):
+class ValueResourceInputOfRetailMediaBrands(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -83,37 +76,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'attributes': (ExternalStoreTarget202110,),  # noqa: E501
+            'data': (ValueResourceOfRetailMediaBrands,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
+        """ValueResourceInputOfRetailMediaBrands - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +129,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
+            data (ValueResourceOfRetailMediaBrands): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
+        """ValueResourceInputOfRetailMediaBrands - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,16 +215,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
+            data (ValueResourceOfRetailMediaBrands): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/model_utils.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
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
 
-from criteo_api_retailmedia_v2024_01.exceptions import (
+from criteo_api_retailmedia_v2024_04.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/models/__init__.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,225 +1,238 @@
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from criteo_api_retailmedia_v2024_01.model.pet import Pet
+# from criteo_api_retailmedia_v2024_04.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from criteo_api_retailmedia_v2024_01.model.add_funds_to_balance_request import AddFundsToBalanceRequest
-from criteo_api_retailmedia_v2024_01.model.add_remove_keyword_model import AddRemoveKeywordModel
-from criteo_api_retailmedia_v2024_01.model.add_remove_keywords_model import AddRemoveKeywordsModel
-from criteo_api_retailmedia_v2024_01.model.add_remove_keywords_model_request import AddRemoveKeywordsModelRequest
-from criteo_api_retailmedia_v2024_01.model.add_remove_keywords_model_resource import AddRemoveKeywordsModelResource
-from criteo_api_retailmedia_v2024_01.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.application_summary_model import ApplicationSummaryModel
-from criteo_api_retailmedia_v2024_01.model.application_summary_model_resource import ApplicationSummaryModelResource
-from criteo_api_retailmedia_v2024_01.model.application_summary_model_response import ApplicationSummaryModelResponse
-from criteo_api_retailmedia_v2024_01.model.approval_status_model import ApprovalStatusModel
-from criteo_api_retailmedia_v2024_01.model.asset import Asset
-from criteo_api_retailmedia_v2024_01.model.asset_resource import AssetResource
-from criteo_api_retailmedia_v2024_01.model.asset_response import AssetResponse
-from criteo_api_retailmedia_v2024_01.model.async_campaigns_report import AsyncCampaignsReport
-from criteo_api_retailmedia_v2024_01.model.async_campaigns_report_request import AsyncCampaignsReportRequest
-from criteo_api_retailmedia_v2024_01.model.async_campaigns_report_resource import AsyncCampaignsReportResource
-from criteo_api_retailmedia_v2024_01.model.async_line_items_report import AsyncLineItemsReport
-from criteo_api_retailmedia_v2024_01.model.async_line_items_report_request import AsyncLineItemsReportRequest
-from criteo_api_retailmedia_v2024_01.model.async_line_items_report_resource import AsyncLineItemsReportResource
-from criteo_api_retailmedia_v2024_01.model.async_report_response import AsyncReportResponse
-from criteo_api_retailmedia_v2024_01.model.async_revenue_report import AsyncRevenueReport
-from criteo_api_retailmedia_v2024_01.model.async_revenue_report_request import AsyncRevenueReportRequest
-from criteo_api_retailmedia_v2024_01.model.async_revenue_report_resource import AsyncRevenueReportResource
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_response import AuctionLineItemResponse
-from criteo_api_retailmedia_v2024_01.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
-from criteo_api_retailmedia_v2024_01.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.audience_target202110_request import AudienceTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.audience_target202110_response import AudienceTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
-from criteo_api_retailmedia_v2024_01.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
-from criteo_api_retailmedia_v2024_01.model.balance_response import BalanceResponse
-from criteo_api_retailmedia_v2024_01.model.balance_response_paged_list_response import BalanceResponsePagedListResponse
-from criteo_api_retailmedia_v2024_01.model.campaign_attributes_v202301 import CampaignAttributesV202301
-from criteo_api_retailmedia_v2024_01.model.campaign_budget_overrides import CampaignBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.campaign_daily_budget_override import CampaignDailyBudgetOverride
-from criteo_api_retailmedia_v2024_01.model.campaign_monthly_budget_override import CampaignMonthlyBudgetOverride
-from criteo_api_retailmedia_v2024_01.model.campaign_v202301 import CampaignV202301
-from criteo_api_retailmedia_v2024_01.model.category202204 import Category202204
-from criteo_api_retailmedia_v2024_01.model.category202204_list_response import Category202204ListResponse
-from criteo_api_retailmedia_v2024_01.model.change_dates_of_balance_request import ChangeDatesOfBalanceRequest
-from criteo_api_retailmedia_v2024_01.model.choice_option import ChoiceOption
-from criteo_api_retailmedia_v2024_01.model.choice_variable_specification import ChoiceVariableSpecification
-from criteo_api_retailmedia_v2024_01.model.choice_variable_value import ChoiceVariableValue
-from criteo_api_retailmedia_v2024_01.model.color_variable_value import ColorVariableValue
-from criteo_api_retailmedia_v2024_01.model.common_error import CommonError
-from criteo_api_retailmedia_v2024_01.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
-from criteo_api_retailmedia_v2024_01.model.common_line_item_response import CommonLineItemResponse
-from criteo_api_retailmedia_v2024_01.model.common_problem import CommonProblem
-from criteo_api_retailmedia_v2024_01.model.common_warning import CommonWarning
-from criteo_api_retailmedia_v2024_01.model.create_balance_request import CreateBalanceRequest
-from criteo_api_retailmedia_v2024_01.model.creative202110 import Creative202110
-from criteo_api_retailmedia_v2024_01.model.creative202110_list_response import Creative202110ListResponse
-from criteo_api_retailmedia_v2024_01.model.creative202210 import Creative202210
-from criteo_api_retailmedia_v2024_01.model.creative202210_list_response import Creative202210ListResponse
-from criteo_api_retailmedia_v2024_01.model.creative202210_response import Creative202210Response
-from criteo_api_retailmedia_v2024_01.model.creative_create_model202207 import CreativeCreateModel202207
-from criteo_api_retailmedia_v2024_01.model.creative_update_model202207 import CreativeUpdateModel202207
-from criteo_api_retailmedia_v2024_01.model.daily_line_item_budget_override import DailyLineItemBudgetOverride
-from criteo_api_retailmedia_v2024_01.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
-from criteo_api_retailmedia_v2024_01.model.external_account import ExternalAccount
-from criteo_api_retailmedia_v2024_01.model.external_add_funds_to_balance import ExternalAddFundsToBalance
-from criteo_api_retailmedia_v2024_01.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
-from criteo_api_retailmedia_v2024_01.model.external_auction_line_item import ExternalAuctionLineItem
-from criteo_api_retailmedia_v2024_01.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
-from criteo_api_retailmedia_v2024_01.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
-from criteo_api_retailmedia_v2024_01.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.external_audience_target202110 import ExternalAudienceTarget202110
-from criteo_api_retailmedia_v2024_01.model.external_balance_response import ExternalBalanceResponse
-from criteo_api_retailmedia_v2024_01.model.external_brand import ExternalBrand
-from criteo_api_retailmedia_v2024_01.model.external_catalog_request import ExternalCatalogRequest
-from criteo_api_retailmedia_v2024_01.model.external_catalog_status import ExternalCatalogStatus
-from criteo_api_retailmedia_v2024_01.model.external_change_dates_of_balance import ExternalChangeDatesOfBalance
-from criteo_api_retailmedia_v2024_01.model.external_common_line_item import ExternalCommonLineItem
-from criteo_api_retailmedia_v2024_01.model.external_create_balance import ExternalCreateBalance
-from criteo_api_retailmedia_v2024_01.model.external_keyword_target202110 import ExternalKeywordTarget202110
-from criteo_api_retailmedia_v2024_01.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-from criteo_api_retailmedia_v2024_01.model.external_line_item_page202110 import ExternalLineItemPage202110
-from criteo_api_retailmedia_v2024_01.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
-from criteo_api_retailmedia_v2024_01.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
-from criteo_api_retailmedia_v2024_01.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
-from criteo_api_retailmedia_v2024_01.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.external_promoted_product202110 import ExternalPromotedProduct202110
-from criteo_api_retailmedia_v2024_01.model.external_retailer import ExternalRetailer
-from criteo_api_retailmedia_v2024_01.model.external_retailer_pages202110 import ExternalRetailerPages202110
-from criteo_api_retailmedia_v2024_01.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.external_store_target202110 import ExternalStoreTarget202110
-from criteo_api_retailmedia_v2024_01.model.external_update_balance_model import ExternalUpdateBalanceModel
-from criteo_api_retailmedia_v2024_01.model.files_variable_value import FilesVariableValue
-from criteo_api_retailmedia_v2024_01.model.files_variables_specification import FilesVariablesSpecification
-from criteo_api_retailmedia_v2024_01.model.hyperlink_variable_value import HyperlinkVariableValue
-from criteo_api_retailmedia_v2024_01.model.input_keywords_model import InputKeywordsModel
-from criteo_api_retailmedia_v2024_01.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
-from criteo_api_retailmedia_v2024_01.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
-from criteo_api_retailmedia_v2024_01.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
-from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
-from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
-from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
-from criteo_api_retailmedia_v2024_01.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
-from criteo_api_retailmedia_v2024_01.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
-from criteo_api_retailmedia_v2024_01.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
-from criteo_api_retailmedia_v2024_01.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
-from criteo_api_retailmedia_v2024_01.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2024_01.model.keyword_data_model import KeywordDataModel
-from criteo_api_retailmedia_v2024_01.model.keyword_target202110_request import KeywordTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.keyword_target202110_response import KeywordTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.keywords_model import KeywordsModel
-from criteo_api_retailmedia_v2024_01.model.keywords_model_resource import KeywordsModelResource
-from criteo_api_retailmedia_v2024_01.model.keywords_model_response import KeywordsModelResponse
-from criteo_api_retailmedia_v2024_01.model.line_item_bid_multipliers import LineItemBidMultipliers
-from criteo_api_retailmedia_v2024_01.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
-from criteo_api_retailmedia_v2024_01.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
-from criteo_api_retailmedia_v2024_01.model.line_item_budget_overrides import LineItemBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.match_type_model import MatchTypeModel
-from criteo_api_retailmedia_v2024_01.model.monthly_line_item_budeget_override import MonthlyLineItemBudegetOverride
-from criteo_api_retailmedia_v2024_01.model.negotiation_state_model import NegotiationStateModel
-from criteo_api_retailmedia_v2024_01.model.page_metadata import PageMetadata
-from criteo_api_retailmedia_v2024_01.model.page_type_environment import PageTypeEnvironment
-from criteo_api_retailmedia_v2024_01.model.post_campaign_v202301 import PostCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item202110_response import PreferredLineItem202110Response
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.problem_details import ProblemDetails
-from criteo_api_retailmedia_v2024_01.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
-from criteo_api_retailmedia_v2024_01.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
-from criteo_api_retailmedia_v2024_01.model.proposal_status_model import ProposalStatusModel
-from criteo_api_retailmedia_v2024_01.model.proposal_status_model_resource import ProposalStatusModelResource
-from criteo_api_retailmedia_v2024_01.model.proposal_status_model_response import ProposalStatusModelResponse
-from criteo_api_retailmedia_v2024_01.model.put_campaign_v202301 import PutCampaignV202301
-from criteo_api_retailmedia_v2024_01.model.report_outcome import ReportOutcome
-from criteo_api_retailmedia_v2024_01.model.resource_of_add_funds_to_balance import ResourceOfAddFundsToBalance
-from criteo_api_retailmedia_v2024_01.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
-from criteo_api_retailmedia_v2024_01.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
-from criteo_api_retailmedia_v2024_01.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
-from criteo_api_retailmedia_v2024_01.model.resource_of_balance_response import ResourceOfBalanceResponse
-from criteo_api_retailmedia_v2024_01.model.resource_of_category202204 import ResourceOfCategory202204
-from criteo_api_retailmedia_v2024_01.model.resource_of_change_dates_of_balance import ResourceOfChangeDatesOfBalance
-from criteo_api_retailmedia_v2024_01.model.resource_of_common_line_item import ResourceOfCommonLineItem
-from criteo_api_retailmedia_v2024_01.model.resource_of_create_balance import ResourceOfCreateBalance
-from criteo_api_retailmedia_v2024_01.model.resource_of_creative202110 import ResourceOfCreative202110
-from criteo_api_retailmedia_v2024_01.model.resource_of_creative202210 import ResourceOfCreative202210
-from criteo_api_retailmedia_v2024_01.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2024_01.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
-from criteo_api_retailmedia_v2024_01.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
-from criteo_api_retailmedia_v2024_01.model.resource_of_template import ResourceOfTemplate
-from criteo_api_retailmedia_v2024_01.model.resource_of_update_balance_model import ResourceOfUpdateBalanceModel
-from criteo_api_retailmedia_v2024_01.model.resource_outcome import ResourceOutcome
-from criteo_api_retailmedia_v2024_01.model.review_state_model import ReviewStateModel
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v1 import RmLegacyAudienceCreateEntityV1
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v1_resource import RmLegacyAudienceCreateEntityV1Resource
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v1_response import RmLegacyAudienceCreateEntityV1Response
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v2 import RmLegacyAudienceCreateEntityV2
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v2_resource import RmLegacyAudienceCreateEntityV2Resource
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_entity_v2_response import RmLegacyAudienceCreateEntityV2Response
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_input_entity_v1 import RmLegacyAudienceCreateInputEntityV1
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_create_input_entity_v2 import RmLegacyAudienceCreateInputEntityV2
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v1 import RmLegacyAudienceGetEntityV1
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v1_list_response import RmLegacyAudienceGetEntityV1ListResponse
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v1_resource import RmLegacyAudienceGetEntityV1Resource
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v2 import RmLegacyAudienceGetEntityV2
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v2_list_response import RmLegacyAudienceGetEntityV2ListResponse
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_get_entity_v2_resource import RmLegacyAudienceGetEntityV2Resource
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_user_behavior_create_v2 import RmLegacyAudienceUserBehaviorCreateV2
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_audience_user_behavior_details_v2 import RmLegacyAudienceUserBehaviorDetailsV2
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_customer_list import RmLegacySegmentCustomerList
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_user_behavior_create_v2 import RmLegacySegmentUserBehaviorCreateV2
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_user_behavior_v1 import RmLegacySegmentUserBehaviorV1
-from criteo_api_retailmedia_v2024_01.model.rm_legacy_segment_user_behavior_v2 import RmLegacySegmentUserBehaviorV2
-from criteo_api_retailmedia_v2024_01.model.rmca_common_problem import RmcaCommonProblem
-from criteo_api_retailmedia_v2024_01.model.section import Section
-from criteo_api_retailmedia_v2024_01.model.set_bid_model import SetBidModel
-from criteo_api_retailmedia_v2024_01.model.set_bids_model import SetBidsModel
-from criteo_api_retailmedia_v2024_01.model.set_bids_model_request import SetBidsModelRequest
-from criteo_api_retailmedia_v2024_01.model.set_bids_model_resource import SetBidsModelResource
-from criteo_api_retailmedia_v2024_01.model.status_response import StatusResponse
-from criteo_api_retailmedia_v2024_01.model.status_response_resource import StatusResponseResource
-from criteo_api_retailmedia_v2024_01.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2024_01.model.store_target202110_request import StoreTarget202110Request
-from criteo_api_retailmedia_v2024_01.model.store_target202110_response import StoreTarget202110Response
-from criteo_api_retailmedia_v2024_01.model.template import Template
-from criteo_api_retailmedia_v2024_01.model.template_list_response import TemplateListResponse
-from criteo_api_retailmedia_v2024_01.model.template_response import TemplateResponse
-from criteo_api_retailmedia_v2024_01.model.template_variable import TemplateVariable
-from criteo_api_retailmedia_v2024_01.model.template_variable_value import TemplateVariableValue
-from criteo_api_retailmedia_v2024_01.model.text_variable_specification import TextVariableSpecification
-from criteo_api_retailmedia_v2024_01.model.text_variable_value import TextVariableValue
-from criteo_api_retailmedia_v2024_01.model.update_balance_model_request import UpdateBalanceModelRequest
-from criteo_api_retailmedia_v2024_01.model.value_resource_input_of_campaign_budget_overrides import ValueResourceInputOfCampaignBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_input_of_line_item_budget_overrides import ValueResourceInputOfLineItemBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_of_campaign_budget_overrides import ValueResourceOfCampaignBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_of_line_item_budget_overrides import ValueResourceOfLineItemBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_outcome_of_campaign_budget_overrides import ValueResourceOutcomeOfCampaignBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_resource_outcome_of_line_item_budget_overrides import ValueResourceOutcomeOfLineItemBudgetOverrides
-from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
-from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
-from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
-from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
-from criteo_api_retailmedia_v2024_01.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+from criteo_api_retailmedia_v2024_04.model.add_funds_to_balance_request import AddFundsToBalanceRequest
+from criteo_api_retailmedia_v2024_04.model.add_remove_keyword_model import AddRemoveKeywordModel
+from criteo_api_retailmedia_v2024_04.model.add_remove_keywords_model import AddRemoveKeywordsModel
+from criteo_api_retailmedia_v2024_04.model.add_remove_keywords_model_request import AddRemoveKeywordsModelRequest
+from criteo_api_retailmedia_v2024_04.model.add_remove_keywords_model_resource import AddRemoveKeywordsModelResource
+from criteo_api_retailmedia_v2024_04.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.application_summary_model import ApplicationSummaryModel
+from criteo_api_retailmedia_v2024_04.model.application_summary_model_resource import ApplicationSummaryModelResource
+from criteo_api_retailmedia_v2024_04.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_retailmedia_v2024_04.model.approval_status_model import ApprovalStatusModel
+from criteo_api_retailmedia_v2024_04.model.asset import Asset
+from criteo_api_retailmedia_v2024_04.model.asset_resource import AssetResource
+from criteo_api_retailmedia_v2024_04.model.asset_response import AssetResponse
+from criteo_api_retailmedia_v2024_04.model.async_campaigns_report import AsyncCampaignsReport
+from criteo_api_retailmedia_v2024_04.model.async_campaigns_report_request import AsyncCampaignsReportRequest
+from criteo_api_retailmedia_v2024_04.model.async_campaigns_report_resource import AsyncCampaignsReportResource
+from criteo_api_retailmedia_v2024_04.model.async_line_items_report import AsyncLineItemsReport
+from criteo_api_retailmedia_v2024_04.model.async_line_items_report_request import AsyncLineItemsReportRequest
+from criteo_api_retailmedia_v2024_04.model.async_line_items_report_resource import AsyncLineItemsReportResource
+from criteo_api_retailmedia_v2024_04.model.async_report_response import AsyncReportResponse
+from criteo_api_retailmedia_v2024_04.model.async_revenue_report import AsyncRevenueReport
+from criteo_api_retailmedia_v2024_04.model.async_revenue_report_request import AsyncRevenueReportRequest
+from criteo_api_retailmedia_v2024_04.model.async_revenue_report_resource import AsyncRevenueReportResource
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_response import AuctionLineItemResponse
+from criteo_api_retailmedia_v2024_04.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
+from criteo_api_retailmedia_v2024_04.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.audience_target202110_request import AudienceTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.audience_target202110_response import AudienceTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
+from criteo_api_retailmedia_v2024_04.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
+from criteo_api_retailmedia_v2024_04.model.balance_response import BalanceResponse
+from criteo_api_retailmedia_v2024_04.model.balance_response_paged_list_response import BalanceResponsePagedListResponse
+from criteo_api_retailmedia_v2024_04.model.campaign_attributes_v202301 import CampaignAttributesV202301
+from criteo_api_retailmedia_v2024_04.model.campaign_budget_overrides import CampaignBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.campaign_daily_budget_override import CampaignDailyBudgetOverride
+from criteo_api_retailmedia_v2024_04.model.campaign_monthly_budget_override import CampaignMonthlyBudgetOverride
+from criteo_api_retailmedia_v2024_04.model.campaign_v202301 import CampaignV202301
+from criteo_api_retailmedia_v2024_04.model.category202204 import Category202204
+from criteo_api_retailmedia_v2024_04.model.category202204_list_response import Category202204ListResponse
+from criteo_api_retailmedia_v2024_04.model.change_dates_of_balance_request import ChangeDatesOfBalanceRequest
+from criteo_api_retailmedia_v2024_04.model.change_details import ChangeDetails
+from criteo_api_retailmedia_v2024_04.model.choice_option import ChoiceOption
+from criteo_api_retailmedia_v2024_04.model.choice_variable_specification import ChoiceVariableSpecification
+from criteo_api_retailmedia_v2024_04.model.choice_variable_value import ChoiceVariableValue
+from criteo_api_retailmedia_v2024_04.model.color_variable_value import ColorVariableValue
+from criteo_api_retailmedia_v2024_04.model.common_error import CommonError
+from criteo_api_retailmedia_v2024_04.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
+from criteo_api_retailmedia_v2024_04.model.common_line_item_response import CommonLineItemResponse
+from criteo_api_retailmedia_v2024_04.model.common_problem import CommonProblem
+from criteo_api_retailmedia_v2024_04.model.common_warning import CommonWarning
+from criteo_api_retailmedia_v2024_04.model.create_balance_request import CreateBalanceRequest
+from criteo_api_retailmedia_v2024_04.model.creative202110 import Creative202110
+from criteo_api_retailmedia_v2024_04.model.creative202110_list_response import Creative202110ListResponse
+from criteo_api_retailmedia_v2024_04.model.creative202210 import Creative202210
+from criteo_api_retailmedia_v2024_04.model.creative202210_list_response import Creative202210ListResponse
+from criteo_api_retailmedia_v2024_04.model.creative202210_response import Creative202210Response
+from criteo_api_retailmedia_v2024_04.model.creative_create_model202207 import CreativeCreateModel202207
+from criteo_api_retailmedia_v2024_04.model.creative_update_model202207 import CreativeUpdateModel202207
+from criteo_api_retailmedia_v2024_04.model.daily_line_item_budget_override import DailyLineItemBudgetOverride
+from criteo_api_retailmedia_v2024_04.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
+from criteo_api_retailmedia_v2024_04.model.external_account import ExternalAccount
+from criteo_api_retailmedia_v2024_04.model.external_add_funds_to_balance import ExternalAddFundsToBalance
+from criteo_api_retailmedia_v2024_04.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
+from criteo_api_retailmedia_v2024_04.model.external_auction_line_item import ExternalAuctionLineItem
+from criteo_api_retailmedia_v2024_04.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
+from criteo_api_retailmedia_v2024_04.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
+from criteo_api_retailmedia_v2024_04.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.external_audience_target202110 import ExternalAudienceTarget202110
+from criteo_api_retailmedia_v2024_04.model.external_balance_response import ExternalBalanceResponse
+from criteo_api_retailmedia_v2024_04.model.external_brand import ExternalBrand
+from criteo_api_retailmedia_v2024_04.model.external_catalog_request import ExternalCatalogRequest
+from criteo_api_retailmedia_v2024_04.model.external_catalog_status import ExternalCatalogStatus
+from criteo_api_retailmedia_v2024_04.model.external_change_dates_of_balance import ExternalChangeDatesOfBalance
+from criteo_api_retailmedia_v2024_04.model.external_common_line_item import ExternalCommonLineItem
+from criteo_api_retailmedia_v2024_04.model.external_create_balance import ExternalCreateBalance
+from criteo_api_retailmedia_v2024_04.model.external_keyword_target202110 import ExternalKeywordTarget202110
+from criteo_api_retailmedia_v2024_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+from criteo_api_retailmedia_v2024_04.model.external_line_item_page202110 import ExternalLineItemPage202110
+from criteo_api_retailmedia_v2024_04.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
+from criteo_api_retailmedia_v2024_04.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
+from criteo_api_retailmedia_v2024_04.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
+from criteo_api_retailmedia_v2024_04.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.external_promoted_product202110 import ExternalPromotedProduct202110
+from criteo_api_retailmedia_v2024_04.model.external_retailer import ExternalRetailer
+from criteo_api_retailmedia_v2024_04.model.external_retailer_pages202110 import ExternalRetailerPages202110
+from criteo_api_retailmedia_v2024_04.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.external_store_target202110 import ExternalStoreTarget202110
+from criteo_api_retailmedia_v2024_04.model.external_update_balance_model import ExternalUpdateBalanceModel
+from criteo_api_retailmedia_v2024_04.model.files_variable_value import FilesVariableValue
+from criteo_api_retailmedia_v2024_04.model.files_variables_specification import FilesVariablesSpecification
+from criteo_api_retailmedia_v2024_04.model.hyperlink_variable_value import HyperlinkVariableValue
+from criteo_api_retailmedia_v2024_04.model.input_keywords_model import InputKeywordsModel
+from criteo_api_retailmedia_v2024_04.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
+from criteo_api_retailmedia_v2024_04.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
+from criteo_api_retailmedia_v2024_04.model.insertion_order_history_change_data_capture import InsertionOrderHistoryChangeDataCapture
+from criteo_api_retailmedia_v2024_04.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
+from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
+from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
+from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
+from criteo_api_retailmedia_v2024_04.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
+from criteo_api_retailmedia_v2024_04.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
+from criteo_api_retailmedia_v2024_04.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
+from criteo_api_retailmedia_v2024_04.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
+from criteo_api_retailmedia_v2024_04.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2024_04.model.keyword_data_model import KeywordDataModel
+from criteo_api_retailmedia_v2024_04.model.keyword_target202110_request import KeywordTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.keyword_target202110_response import KeywordTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.keywords_model import KeywordsModel
+from criteo_api_retailmedia_v2024_04.model.keywords_model_resource import KeywordsModelResource
+from criteo_api_retailmedia_v2024_04.model.keywords_model_response import KeywordsModelResponse
+from criteo_api_retailmedia_v2024_04.model.line_item_bid_multipliers import LineItemBidMultipliers
+from criteo_api_retailmedia_v2024_04.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
+from criteo_api_retailmedia_v2024_04.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
+from criteo_api_retailmedia_v2024_04.model.line_item_budget_overrides import LineItemBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.match_type_model import MatchTypeModel
+from criteo_api_retailmedia_v2024_04.model.metadata import Metadata
+from criteo_api_retailmedia_v2024_04.model.monthly_line_item_budeget_override import MonthlyLineItemBudegetOverride
+from criteo_api_retailmedia_v2024_04.model.negotiation_state_model import NegotiationStateModel
+from criteo_api_retailmedia_v2024_04.model.page_metadata import PageMetadata
+from criteo_api_retailmedia_v2024_04.model.page_of_insertion_order_history_change_data_capture import PageOfInsertionOrderHistoryChangeDataCapture
+from criteo_api_retailmedia_v2024_04.model.page_type_environment import PageTypeEnvironment
+from criteo_api_retailmedia_v2024_04.model.post_campaign_v202301 import PostCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item202110_response import PreferredLineItem202110Response
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.problem_details import ProblemDetails
+from criteo_api_retailmedia_v2024_04.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
+from criteo_api_retailmedia_v2024_04.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
+from criteo_api_retailmedia_v2024_04.model.proposal_status_model import ProposalStatusModel
+from criteo_api_retailmedia_v2024_04.model.proposal_status_model_resource import ProposalStatusModelResource
+from criteo_api_retailmedia_v2024_04.model.proposal_status_model_response import ProposalStatusModelResponse
+from criteo_api_retailmedia_v2024_04.model.put_campaign_v202301 import PutCampaignV202301
+from criteo_api_retailmedia_v2024_04.model.report_outcome import ReportOutcome
+from criteo_api_retailmedia_v2024_04.model.resource_of_add_funds_to_balance import ResourceOfAddFundsToBalance
+from criteo_api_retailmedia_v2024_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+from criteo_api_retailmedia_v2024_04.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
+from criteo_api_retailmedia_v2024_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+from criteo_api_retailmedia_v2024_04.model.resource_of_balance_response import ResourceOfBalanceResponse
+from criteo_api_retailmedia_v2024_04.model.resource_of_category202204 import ResourceOfCategory202204
+from criteo_api_retailmedia_v2024_04.model.resource_of_change_dates_of_balance import ResourceOfChangeDatesOfBalance
+from criteo_api_retailmedia_v2024_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
+from criteo_api_retailmedia_v2024_04.model.resource_of_create_balance import ResourceOfCreateBalance
+from criteo_api_retailmedia_v2024_04.model.resource_of_creative202110 import ResourceOfCreative202110
+from criteo_api_retailmedia_v2024_04.model.resource_of_creative202210 import ResourceOfCreative202210
+from criteo_api_retailmedia_v2024_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2024_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+from criteo_api_retailmedia_v2024_04.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+from criteo_api_retailmedia_v2024_04.model.resource_of_retail_media_account import ResourceOfRetailMediaAccount
+from criteo_api_retailmedia_v2024_04.model.resource_of_template import ResourceOfTemplate
+from criteo_api_retailmedia_v2024_04.model.resource_of_update_balance_model import ResourceOfUpdateBalanceModel
+from criteo_api_retailmedia_v2024_04.model.resource_outcome import ResourceOutcome
+from criteo_api_retailmedia_v2024_04.model.resource_outcome_of_retail_media_account import ResourceOutcomeOfRetailMediaAccount
+from criteo_api_retailmedia_v2024_04.model.retail_media_account import RetailMediaAccount
+from criteo_api_retailmedia_v2024_04.model.retail_media_brand_account_creation import RetailMediaBrandAccountCreation
+from criteo_api_retailmedia_v2024_04.model.retail_media_brands import RetailMediaBrands
+from criteo_api_retailmedia_v2024_04.model.review_state_model import ReviewStateModel
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v1 import RmLegacyAudienceCreateEntityV1
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v1_resource import RmLegacyAudienceCreateEntityV1Resource
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v1_response import RmLegacyAudienceCreateEntityV1Response
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v2 import RmLegacyAudienceCreateEntityV2
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v2_resource import RmLegacyAudienceCreateEntityV2Resource
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_entity_v2_response import RmLegacyAudienceCreateEntityV2Response
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_input_entity_v1 import RmLegacyAudienceCreateInputEntityV1
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_create_input_entity_v2 import RmLegacyAudienceCreateInputEntityV2
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v1 import RmLegacyAudienceGetEntityV1
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v1_list_response import RmLegacyAudienceGetEntityV1ListResponse
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v1_resource import RmLegacyAudienceGetEntityV1Resource
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v2 import RmLegacyAudienceGetEntityV2
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v2_list_response import RmLegacyAudienceGetEntityV2ListResponse
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_get_entity_v2_resource import RmLegacyAudienceGetEntityV2Resource
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_user_behavior_create_v2 import RmLegacyAudienceUserBehaviorCreateV2
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_audience_user_behavior_details_v2 import RmLegacyAudienceUserBehaviorDetailsV2
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_customer_list import RmLegacySegmentCustomerList
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_user_behavior_create_v2 import RmLegacySegmentUserBehaviorCreateV2
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_user_behavior_v1 import RmLegacySegmentUserBehaviorV1
+from criteo_api_retailmedia_v2024_04.model.rm_legacy_segment_user_behavior_v2 import RmLegacySegmentUserBehaviorV2
+from criteo_api_retailmedia_v2024_04.model.rmca_common_problem import RmcaCommonProblem
+from criteo_api_retailmedia_v2024_04.model.section import Section
+from criteo_api_retailmedia_v2024_04.model.set_bid_model import SetBidModel
+from criteo_api_retailmedia_v2024_04.model.set_bids_model import SetBidsModel
+from criteo_api_retailmedia_v2024_04.model.set_bids_model_request import SetBidsModelRequest
+from criteo_api_retailmedia_v2024_04.model.set_bids_model_resource import SetBidsModelResource
+from criteo_api_retailmedia_v2024_04.model.status_response import StatusResponse
+from criteo_api_retailmedia_v2024_04.model.status_response_resource import StatusResponseResource
+from criteo_api_retailmedia_v2024_04.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2024_04.model.store_target202110_request import StoreTarget202110Request
+from criteo_api_retailmedia_v2024_04.model.store_target202110_response import StoreTarget202110Response
+from criteo_api_retailmedia_v2024_04.model.template import Template
+from criteo_api_retailmedia_v2024_04.model.template_list_response import TemplateListResponse
+from criteo_api_retailmedia_v2024_04.model.template_response import TemplateResponse
+from criteo_api_retailmedia_v2024_04.model.template_variable import TemplateVariable
+from criteo_api_retailmedia_v2024_04.model.template_variable_value import TemplateVariableValue
+from criteo_api_retailmedia_v2024_04.model.text_variable_specification import TextVariableSpecification
+from criteo_api_retailmedia_v2024_04.model.text_variable_value import TextVariableValue
+from criteo_api_retailmedia_v2024_04.model.update_balance_model_request import UpdateBalanceModelRequest
+from criteo_api_retailmedia_v2024_04.model.value_resource_input_of_campaign_budget_overrides import ValueResourceInputOfCampaignBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_input_of_line_item_budget_overrides import ValueResourceInputOfLineItemBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_input_of_retail_media_brand_account_creation import ValueResourceInputOfRetailMediaBrandAccountCreation
+from criteo_api_retailmedia_v2024_04.model.value_resource_input_of_retail_media_brands import ValueResourceInputOfRetailMediaBrands
+from criteo_api_retailmedia_v2024_04.model.value_resource_of_campaign_budget_overrides import ValueResourceOfCampaignBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_of_line_item_budget_overrides import ValueResourceOfLineItemBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_of_retail_media_brand_account_creation import ValueResourceOfRetailMediaBrandAccountCreation
+from criteo_api_retailmedia_v2024_04.model.value_resource_of_retail_media_brands import ValueResourceOfRetailMediaBrands
+from criteo_api_retailmedia_v2024_04.model.value_resource_outcome_of_campaign_budget_overrides import ValueResourceOutcomeOfCampaignBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_resource_outcome_of_line_item_budget_overrides import ValueResourceOutcomeOfLineItemBudgetOverrides
+from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
+from criteo_api_retailmedia_v2024_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/criteo_api_retailmedia_v2024_01/rest.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/criteo_api_retailmedia_v2024_04/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
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
 
-from criteo_api_retailmedia_v2024_01.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from criteo_api_retailmedia_v2024_04.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/setup.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-retailmedia-sdk"
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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240515
+pip install criteo-api-retailmedia-sdk==2024.04.0.240515
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240515`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.04.0.240515`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2024_01
+import criteo_api_retailmedia_v2024_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo_api_retailmedia_sdk-2024.1.0.240515/test/test_gateway_api.py` & `criteo_api_retailmedia_sdk-2024.4.0.240515/test/test_gateway_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 
-from criteo_api_retailmedia_v2024_01.api.gateway_api import GatewayApi
-from criteo_api_retailmedia_v2024_01.api_client_builder import ApiClientBuilder
-from criteo_api_retailmedia_v2024_01.rest import ApiException
+from criteo_api_retailmedia_v2024_04.api.gateway_api import GatewayApi
+from criteo_api_retailmedia_v2024_04.api_client_builder import ApiClientBuilder
+from criteo_api_retailmedia_v2024_04.rest import ApiException
 from example_application_with_client_credentials import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
```

