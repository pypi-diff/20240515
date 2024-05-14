# Comparing `tmp/invariant_client-1.1.2.tar.gz` & `tmp/invariant_client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invariant_client-1.1.2.tar", max compression
+gzip compressed data, was "invariant_client-1.3.0.tar", max compression
```

## Comparing `invariant_client-1.1.2.tar` & `invariant_client-1.3.0.tar`

### file list

```diff
@@ -1,128 +1,137 @@
--rw-r--r--   0        0        0     1069 2024-04-20 17:20:31.942692 invariant_client-1.1.2/LICENSE
--rw-r--r--   0        0        0     1262 2024-04-20 17:20:31.942785 invariant_client-1.1.2/README.md
--rw-r--r--   0        0        0     6148 2024-04-20 17:21:49.048467 invariant_client-1.1.2/invariant_client/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.942933 invariant_client-1.1.2/invariant_client/__init__.py
--rw-r--r--   0        0        0       67 2024-04-20 17:20:31.943029 invariant_client-1.1.2/invariant_client/__main__.py
--rw-r--r--   0        0        0      169 2024-04-20 17:20:31.943153 invariant_client-1.1.2/invariant_client/auth/__init__.py
--rw-r--r--   0        0        0     4213 2024-04-20 17:20:31.943252 invariant_client-1.1.2/invariant_client/auth/auth.py
--rw-r--r--   0        0        0      162 2024-04-20 17:20:31.943422 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-20 17:20:31.943537 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.943620 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/__init__.py
--rw-r--r--   0        0        0     6126 2024-04-20 17:20:31.943790 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py
--rw-r--r--   0        0        0     5813 2024-04-20 17:20:31.943953 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py
--rw-r--r--   0        0        0     5527 2024-04-20 17:20:31.944096 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py
--rw-r--r--   0        0        0     5488 2024-04-20 17:20:31.944189 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py
--rw-r--r--   0        0        0     6052 2024-04-20 17:20:31.944302 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py
--rw-r--r--   0        0        0     6763 2024-04-20 17:20:31.944389 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py
--rw-r--r--   0        0        0     6298 2024-04-20 17:20:31.944542 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py
--rw-r--r--   0        0        0     5825 2024-04-20 17:20:31.944639 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py
--rw-r--r--   0        0        0     5582 2024-04-20 17:20:31.944739 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py
--rw-r--r--   0        0        0     5794 2024-04-20 17:20:31.944850 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py
--rw-r--r--   0        0        0     5584 2024-04-20 17:20:31.944995 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py
--rw-r--r--   0        0        0     5753 2024-04-20 17:20:31.945105 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py
--rw-r--r--   0        0        0     5838 2024-04-20 17:20:31.945212 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py
--rw-r--r--   0        0        0     5303 2024-04-20 17:20:31.945318 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py
--rw-r--r--   0        0        0     7002 2024-04-20 17:20:31.945428 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py
--rw-r--r--   0        0        0     6131 2024-04-20 17:20:31.945554 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.945670 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_css_js/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.945787 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_html/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.945910 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_images/__init__.py
--rw-r--r--   0        0        0     3588 2024-04-20 17:20:31.946019 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py
--rw-r--r--   0        0        0    12209 2024-04-20 17:20:31.946149 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/client.py
--rw-r--r--   0        0        0      470 2024-04-20 17:20:31.946241 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/errors.py
--rw-r--r--   0        0        0     4051 2024-04-20 17:20:31.946396 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/__init__.py
--rw-r--r--   0        0        0     3027 2024-04-20 17:20:31.946507 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/base_error_response.py
--rw-r--r--   0        0        0     3710 2024-04-20 17:20:31.946630 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py
--rw-r--r--   0        0        0     3944 2024-04-20 17:20:31.946762 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/challenge_response.py
--rw-r--r--   0        0        0      261 2024-04-20 17:20:31.946878 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/challenge_response_challenge.py
--rw-r--r--   0        0        0     2654 2024-04-20 17:20:31.947013 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py
--rw-r--r--   0        0        0     1304 2024-04-20 17:20:31.947125 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py
--rw-r--r--   0        0        0     2579 2024-04-20 17:20:31.947265 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py
--rw-r--r--   0        0        0     2269 2024-04-20 17:20:31.947387 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py
--rw-r--r--   0        0        0     2164 2024-04-20 17:20:31.947507 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_token_request.py
--rw-r--r--   0        0        0     3580 2024-04-20 17:20:31.947595 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py
--rw-r--r--   0        0        0     2682 2024-04-20 17:20:31.947679 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py
--rw-r--r--   0        0        0      151 2024-04-20 17:20:31.947757 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/generic_state.py
--rw-r--r--   0        0        0     2723 2024-04-20 17:20:31.947851 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py
--rw-r--r--   0        0        0     1335 2024-04-20 17:20:31.947930 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py
--rw-r--r--   0        0        0     1340 2024-04-20 17:20:31.948014 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py
--rw-r--r--   0        0        0     2788 2024-04-20 17:20:31.948090 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration.py
--rw-r--r--   0        0        0     2434 2024-04-20 17:20:31.948168 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py
--rw-r--r--   0        0        0     3335 2024-04-20 17:20:31.948241 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py
--rw-r--r--   0        0        0     1416 2024-04-20 17:20:31.948309 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py
--rw-r--r--   0        0        0     2193 2024-04-20 17:20:31.948381 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py
--rw-r--r--   0        0        0     1481 2024-04-20 17:20:31.948476 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py
--rw-r--r--   0        0        0     2004 2024-04-20 17:20:31.948566 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py
--rw-r--r--   0        0        0     1572 2024-04-20 17:20:31.948656 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/metadata.py
--rw-r--r--   0        0        0     2709 2024-04-20 17:20:31.948753 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/organization.py
--rw-r--r--   0        0        0     2621 2024-04-20 17:20:31.948876 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py
--rw-r--r--   0        0        0     2352 2024-04-20 17:20:31.948966 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/refresh_response.py
--rw-r--r--   0        0        0     3375 2024-04-20 17:20:31.949030 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report.py
--rw-r--r--   0        0        0     1914 2024-04-20 17:20:31.949118 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_request.py
--rw-r--r--   0        0        0     2256 2024-04-20 17:20:31.949199 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py
--rw-r--r--   0        0        0     4949 2024-04-20 17:20:31.949275 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py
--rw-r--r--   0        0        0     1297 2024-04-20 17:20:31.949345 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py
--rw-r--r--   0        0        0     4420 2024-04-20 17:20:31.949430 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info.py
--rw-r--r--   0        0        0     2821 2024-04-20 17:20:31.949517 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py
--rw-r--r--   0        0        0     1270 2024-04-20 17:20:31.949584 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py
--rw-r--r--   0        0        0     3093 2024-04-20 17:20:31.949661 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py
--rw-r--r--   0        0        0     1546 2024-04-20 17:20:31.949728 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py
--rw-r--r--   0        0        0     1795 2024-04-20 17:20:31.949807 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py
--rw-r--r--   0        0        0     4555 2024-04-20 17:20:31.949876 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user.py
--rw-r--r--   0        0        0     1525 2024-04-20 17:20:31.949952 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_metadata.py
--rw-r--r--   0        0        0     1922 2024-04-20 17:20:31.950031 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py
--rw-r--r--   0        0        0     3945 2024-04-20 17:20:31.950114 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py
--rw-r--r--   0        0        0     1850 2024-04-20 17:20:31.950209 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py
--rw-r--r--   0        0        0      968 2024-04-20 17:20:31.950282 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/types.py
--rw-r--r--   0        0        0      159 2024-04-20 17:20:31.950405 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/__init__.py
--rw-r--r--   0        0        0       47 2024-04-20 17:20:31.950508 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.950584 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/__init__.py
--rw-r--r--   0        0        0     4700 2024-04-20 17:20:31.950675 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py
--rw-r--r--   0        0        0     5770 2024-04-20 17:20:31.950772 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py
--rw-r--r--   0        0        0     4590 2024-04-20 17:20:31.950852 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.950928 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/__init__.py
--rw-r--r--   0        0        0     5085 2024-04-20 17:20:31.951007 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py
--rw-r--r--   0        0        0     7153 2024-04-20 17:20:31.951092 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py
--rw-r--r--   0        0        0     4746 2024-04-20 17:20:31.951178 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py
--rw-r--r--   0        0        0     3948 2024-04-20 17:20:31.951263 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py
--rw-r--r--   0        0        0    14437 2024-04-20 17:20:31.951340 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py
--rw-r--r--   0        0        0     4470 2024-04-20 17:20:31.951418 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py
--rw-r--r--   0        0        0     5473 2024-04-20 17:20:31.951497 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py
--rw-r--r--   0        0        0     4492 2024-04-20 17:20:31.951579 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.951659 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/static/__init__.py
--rw-r--r--   0        0        0     4042 2024-04-20 17:20:31.951744 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py
--rw-r--r--   0        0        0        0 2024-04-20 17:20:31.951818 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/webhooks/__init__.py
--rw-r--r--   0        0        0     4347 2024-04-20 17:20:31.951910 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py
--rw-r--r--   0        0        0    12209 2024-04-20 17:20:31.952005 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/client.py
--rw-r--r--   0        0        0      470 2024-04-20 17:20:31.952082 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/errors.py
--rw-r--r--   0        0        0     1900 2024-04-20 17:20:31.952192 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/__init__.py
--rw-r--r--   0        0        0     3027 2024-04-20 17:20:31.952282 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/base_error_response.py
--rw-r--r--   0        0        0     3944 2024-04-20 17:20:31.952344 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/challenge_response.py
--rw-r--r--   0        0        0      261 2024-04-20 17:20:31.952411 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/challenge_response_challenge.py
--rw-r--r--   0        0        0     2241 2024-04-20 17:20:31.952479 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/check_invite_response.py
--rw-r--r--   0        0        0     3324 2024-04-20 17:20:31.952549 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py
--rw-r--r--   0        0        0     2708 2024-04-20 17:20:31.952613 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py
--rw-r--r--   0        0        0     1481 2024-04-20 17:20:31.952673 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_check_request.py
--rw-r--r--   0        0        0     1668 2024-04-20 17:20:31.952742 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_password_login.py
--rw-r--r--   0        0        0     1776 2024-04-20 17:20:31.952803 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py
--rw-r--r--   0        0        0     1506 2024-04-20 17:20:31.952865 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/get_version_response.py
--rw-r--r--   0        0        0     1557 2024-04-20 17:20:31.952932 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login.py
--rw-r--r--   0        0        0    10565 2024-04-20 17:20:31.953000 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login_request.py
--rw-r--r--   0        0        0     2461 2024-04-20 17:20:31.953068 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/new_password_request.py
--rw-r--r--   0        0        0      168 2024-04-20 17:20:31.953142 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/new_password_request_authn_type.py
--rw-r--r--   0        0        0     2220 2024-04-20 17:20:31.953210 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/organization.py
--rw-r--r--   0        0        0     1786 2024-04-20 17:20:31.953289 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py
--rw-r--r--   0        0        0     1603 2024-04-20 17:20:31.953351 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py
--rw-r--r--   0        0        0     1453 2024-04-20 17:20:31.953410 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_request.py
--rw-r--r--   0        0        0     2678 2024-04-20 17:20:31.953472 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/user.py
--rw-r--r--   0        0        0     3945 2024-04-20 17:20:31.953536 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response.py
--rw-r--r--   0        0        0     1850 2024-04-20 17:20:31.953604 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py
--rw-r--r--   0        0        0     1458 2024-04-20 17:20:31.953667 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_request.py
--rw-r--r--   0        0        0      968 2024-04-20 17:20:31.953734 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/types.py
--rw-r--r--   0        0        0    15895 2024-04-20 17:20:31.953883 invariant_client-1.1.2/invariant_client/cli.py
--rw-r--r--   0        0        0     3010 2024-04-20 17:20:31.953974 invariant_client-1.1.2/invariant_client/display.py
--rw-r--r--   0        0        0    18041 2024-04-20 17:20:31.954113 invariant_client-1.1.2/invariant_client/pysdk.py
--rw-r--r--   0        0        0     1616 2024-04-20 17:20:31.954189 invariant_client-1.1.2/invariant_client/version.py
--rw-r--r--   0        0        0     2481 2024-04-20 17:20:31.954277 invariant_client-1.1.2/invariant_client/zip_util.py
--rw-r--r--   0        0        0      800 2024-04-20 23:49:40.609789 invariant_client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 invariant_client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-14 22:39:38.663987 invariant_client-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5549 2024-05-14 22:39:38.665882 invariant_client-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:38.673328 invariant_client-1.3.0/invariant_client/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-14 22:39:38.675829 invariant_client-1.3.0/invariant_client/__main__.py
+-rw-r--r--   0        0        0      169 2024-05-14 22:39:38.677498 invariant_client-1.3.0/invariant_client/auth/__init__.py
+-rw-r--r--   0        0        0     4213 2024-05-14 22:39:38.678400 invariant_client-1.3.0/invariant_client/auth/auth.py
+-rw-r--r--   0        0        0      162 2024-05-14 22:39:38.684853 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-14 22:39:38.686660 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:38.688511 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/__init__.py
+-rw-r--r--   0        0        0     6126 2024-05-14 22:39:38.690242 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py
+-rw-r--r--   0        0        0     5813 2024-05-14 22:39:38.691230 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py
+-rw-r--r--   0        0        0     5527 2024-05-14 22:39:38.692403 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py
+-rw-r--r--   0        0        0     5488 2024-05-14 22:39:38.693421 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py
+-rw-r--r--   0        0        0     6052 2024-05-14 22:39:38.694486 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py
+-rw-r--r--   0        0        0     6771 2024-05-14 22:39:38.695644 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_text_summary_organization_name_api_v_1_reports_report_id_summary_text_get.py
+-rw-r--r--   0        0        0     6763 2024-05-14 22:39:38.697003 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py
+-rw-r--r--   0        0        0     5743 2024-05-14 22:39:38.698121 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_settings_organization_name_api_v_1_flags_get.py
+-rw-r--r--   0        0        0     6298 2024-05-14 22:39:38.699156 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py
+-rw-r--r--   0        0        0     5825 2024-05-14 22:39:38.699823 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py
+-rw-r--r--   0        0        0     5714 2024-05-14 22:39:38.700710 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/list_report_tasks_organization_name_api_v_1_reports_in_progress_get.py
+-rw-r--r--   0        0        0     5582 2024-05-14 22:39:38.701235 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py
+-rw-r--r--   0        0        0     5794 2024-05-14 22:39:38.702341 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py
+-rw-r--r--   0        0        0     5584 2024-05-14 22:39:38.711548 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py
+-rw-r--r--   0        0        0     5753 2024-05-14 22:39:38.714936 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py
+-rw-r--r--   0        0        0     5838 2024-05-14 22:39:38.716893 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py
+-rw-r--r--   0        0        0     5303 2024-05-14 22:39:38.719130 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py
+-rw-r--r--   0        0        0     7002 2024-05-14 22:39:38.729096 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py
+-rw-r--r--   0        0        0     6131 2024-05-14 22:39:38.732628 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:38.737245 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/static_css_js/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:38.752143 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/static_html/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:38.755109 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/static_images/__init__.py
+-rw-r--r--   0        0        0     3588 2024-05-14 22:39:38.758349 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:38.760008 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/static_third_party_javascript/__init__.py
+-rw-r--r--   0        0        0    12209 2024-05-14 22:39:38.761785 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/client.py
+-rw-r--r--   0        0        0      470 2024-05-14 22:39:38.763150 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/errors.py
+-rw-r--r--   0        0        0     4527 2024-05-14 22:39:38.778958 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/__init__.py
+-rw-r--r--   0        0        0     3027 2024-05-14 22:39:38.782498 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/base_error_response.py
+-rw-r--r--   0        0        0     3710 2024-05-14 22:39:38.784132 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py
+-rw-r--r--   0        0        0     3944 2024-05-14 22:39:38.785483 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/challenge_response.py
+-rw-r--r--   0        0        0      261 2024-05-14 22:39:38.786472 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/challenge_response_challenge.py
+-rw-r--r--   0        0        0     2654 2024-05-14 22:39:38.787855 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py
+-rw-r--r--   0        0        0     1304 2024-05-14 22:39:38.788894 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py
+-rw-r--r--   0        0        0     3324 2024-05-14 22:39:38.790770 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/console_request_options.py
+-rw-r--r--   0        0        0     2579 2024-05-14 22:39:38.793146 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py
+-rw-r--r--   0        0        0     2269 2024-05-14 22:39:38.793888 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py
+-rw-r--r--   0        0        0     2164 2024-05-14 22:39:38.794876 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/create_token_request.py
+-rw-r--r--   0        0        0     3580 2024-05-14 22:39:38.795526 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py
+-rw-r--r--   0        0        0     2682 2024-05-14 22:39:38.796161 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py
+-rw-r--r--   0        0        0     2328 2024-05-14 22:39:38.797459 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/flags_response.py
+-rw-r--r--   0        0        0     1840 2024-05-14 22:39:38.798936 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/flags_response_environment.py
+-rw-r--r--   0        0        0     1850 2024-05-14 22:39:38.802996 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/flags_response_flags.py
+-rw-r--r--   0        0        0      151 2024-05-14 22:39:38.805887 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/generic_state.py
+-rw-r--r--   0        0        0     2723 2024-05-14 22:39:38.807774 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py
+-rw-r--r--   0        0        0     1335 2024-05-14 22:39:38.809311 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py
+-rw-r--r--   0        0        0     1340 2024-05-14 22:39:38.815753 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py
+-rw-r--r--   0        0        0     2788 2024-05-14 22:39:38.817282 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration.py
+-rw-r--r--   0        0        0     2434 2024-05-14 22:39:38.820195 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py
+-rw-r--r--   0        0        0     3335 2024-05-14 22:39:38.825931 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py
+-rw-r--r--   0        0        0     1416 2024-05-14 22:39:38.829957 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py
+-rw-r--r--   0        0        0     2193 2024-05-14 22:39:38.834250 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py
+-rw-r--r--   0        0        0     1481 2024-05-14 22:39:38.841034 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py
+-rw-r--r--   0        0        0     2145 2024-05-14 22:39:38.843743 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/list_report_tasks_response.py
+-rw-r--r--   0        0        0     2004 2024-05-14 22:39:38.846261 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py
+-rw-r--r--   0        0        0     1572 2024-05-14 22:39:38.847422 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/metadata.py
+-rw-r--r--   0        0        0     2709 2024-05-14 22:39:38.849376 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/organization.py
+-rw-r--r--   0        0        0     2621 2024-05-14 22:39:38.850848 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py
+-rw-r--r--   0        0        0     2352 2024-05-14 22:39:38.858046 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/refresh_response.py
+-rw-r--r--   0        0        0     3375 2024-05-14 22:39:38.861144 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/report.py
+-rw-r--r--   0        0        0     2925 2024-05-14 22:39:38.863548 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/report_task.py
+-rw-r--r--   0        0        0     4029 2024-05-14 22:39:38.869934 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/report_text_summary_request.py
+-rw-r--r--   0        0        0     2256 2024-05-14 22:39:38.877234 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py
+-rw-r--r--   0        0        0     4949 2024-05-14 22:39:38.885651 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py
+-rw-r--r--   0        0        0     1297 2024-05-14 22:39:38.894995 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py
+-rw-r--r--   0        0        0     4420 2024-05-14 22:39:38.897921 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/tab_info.py
+-rw-r--r--   0        0        0     2821 2024-05-14 22:39:38.902071 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py
+-rw-r--r--   0        0        0     1270 2024-05-14 22:39:38.909364 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py
+-rw-r--r--   0        0        0     3093 2024-05-14 22:39:38.911241 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py
+-rw-r--r--   0        0        0     1546 2024-05-14 22:39:38.913170 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py
+-rw-r--r--   0        0        0     1795 2024-05-14 22:39:38.914934 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py
+-rw-r--r--   0        0        0     4555 2024-05-14 22:39:38.916612 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/user.py
+-rw-r--r--   0        0        0     1525 2024-05-14 22:39:38.918361 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/user_metadata.py
+-rw-r--r--   0        0        0     1922 2024-05-14 22:39:38.921393 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py
+-rw-r--r--   0        0        0     3945 2024-05-14 22:39:38.928190 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py
+-rw-r--r--   0        0        0     1850 2024-05-14 22:39:38.930531 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py
+-rw-r--r--   0        0        0      968 2024-05-14 22:39:38.931817 invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/types.py
+-rw-r--r--   0        0        0      159 2024-05-14 22:39:38.937802 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-14 22:39:38.940323 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:38.984997 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/client_login/__init__.py
+-rw-r--r--   0        0        0     4700 2024-05-14 22:39:38.986805 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py
+-rw-r--r--   0        0        0     5770 2024-05-14 22:39:38.989751 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py
+-rw-r--r--   0        0        0     4590 2024-05-14 22:39:38.995375 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:39.001186 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/__init__.py
+-rw-r--r--   0        0        0     5085 2024-05-14 22:39:39.003341 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py
+-rw-r--r--   0        0        0     7153 2024-05-14 22:39:39.004861 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py
+-rw-r--r--   0        0        0     4746 2024-05-14 22:39:39.006283 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py
+-rw-r--r--   0        0        0     3948 2024-05-14 22:39:39.007648 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py
+-rw-r--r--   0        0        0    14437 2024-05-14 22:39:39.015341 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py
+-rw-r--r--   0        0        0     4470 2024-05-14 22:39:39.041062 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py
+-rw-r--r--   0        0        0     5473 2024-05-14 22:39:39.076703 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py
+-rw-r--r--   0        0        0     4492 2024-05-14 22:39:39.085836 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:39.093896 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/static/__init__.py
+-rw-r--r--   0        0        0     4042 2024-05-14 22:39:39.123145 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:39:39.126339 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/webhooks/__init__.py
+-rw-r--r--   0        0        0     4347 2024-05-14 22:39:39.134657 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py
+-rw-r--r--   0        0        0    12209 2024-05-14 22:39:39.143916 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/client.py
+-rw-r--r--   0        0        0      470 2024-05-14 22:39:39.147552 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/errors.py
+-rw-r--r--   0        0        0     1900 2024-05-14 22:39:39.165855 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/__init__.py
+-rw-r--r--   0        0        0     3027 2024-05-14 22:39:39.185276 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/base_error_response.py
+-rw-r--r--   0        0        0     3944 2024-05-14 22:39:39.192291 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/challenge_response.py
+-rw-r--r--   0        0        0      261 2024-05-14 22:39:39.203550 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/challenge_response_challenge.py
+-rw-r--r--   0        0        0     2241 2024-05-14 22:39:39.207494 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/check_invite_response.py
+-rw-r--r--   0        0        0     3324 2024-05-14 22:39:39.210380 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py
+-rw-r--r--   0        0        0     2708 2024-05-14 22:39:39.222763 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py
+-rw-r--r--   0        0        0     1481 2024-05-14 22:39:39.229110 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/email_check_request.py
+-rw-r--r--   0        0        0     1668 2024-05-14 22:39:39.230323 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/email_password_login.py
+-rw-r--r--   0        0        0     1776 2024-05-14 22:39:39.231302 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py
+-rw-r--r--   0        0        0     1506 2024-05-14 22:39:39.232819 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/get_version_response.py
+-rw-r--r--   0        0        0     1557 2024-05-14 22:39:39.235225 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/login.py
+-rw-r--r--   0        0        0    10565 2024-05-14 22:39:39.238788 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/login_request.py
+-rw-r--r--   0        0        0     2461 2024-05-14 22:39:39.244893 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/new_password_request.py
+-rw-r--r--   0        0        0      168 2024-05-14 22:39:39.246797 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/new_password_request_authn_type.py
+-rw-r--r--   0        0        0     2220 2024-05-14 22:39:39.249342 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/organization.py
+-rw-r--r--   0        0        0     1786 2024-05-14 22:39:39.262260 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py
+-rw-r--r--   0        0        0     1603 2024-05-14 22:39:39.267584 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py
+-rw-r--r--   0        0        0     1453 2024-05-14 22:39:39.273513 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/reset_request.py
+-rw-r--r--   0        0        0     2678 2024-05-14 22:39:39.277557 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/user.py
+-rw-r--r--   0        0        0     3945 2024-05-14 22:39:39.282249 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/validation_error_response.py
+-rw-r--r--   0        0        0     1850 2024-05-14 22:39:39.285572 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py
+-rw-r--r--   0        0        0     1458 2024-05-14 22:39:39.286246 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/validation_request.py
+-rw-r--r--   0        0        0      968 2024-05-14 22:39:39.292225 invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/types.py
+-rw-r--r--   0        0        0    19172 2024-05-14 22:39:39.297580 invariant_client-1.3.0/invariant_client/cli.py
+-rw-r--r--   0        0        0     3231 2024-05-14 22:39:39.299643 invariant_client-1.3.0/invariant_client/display.py
+-rw-r--r--   0        0        0    19323 2024-05-14 22:39:39.302424 invariant_client-1.3.0/invariant_client/pysdk.py
+-rw-r--r--   0        0        0     1616 2024-05-14 22:39:39.303909 invariant_client-1.3.0/invariant_client/version.py
+-rw-r--r--   0        0        0     2481 2024-05-14 22:39:39.305373 invariant_client-1.3.0/invariant_client/zip_util.py
+-rw-r--r--   0        0        0      800 2024-05-14 22:39:39.327469 invariant_client-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6310 1970-01-01 00:00:00.000000 invariant_client-1.3.0/PKG-INFO
```

### Comparing `invariant_client-1.1.2/LICENSE` & `invariant_client-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/auth/auth.py` & `invariant_client-1.3.0/invariant_client/auth/auth.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.create_integration_request_github_app_installation import (
-    CreateIntegrationRequestGithubAppInstallation,
-)
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import cast
 from typing import Dict
+from ...models.create_integration_request_github_app_installation import (
+    CreateIntegrationRequestGithubAppInstallation,
+)
 
 
 def _get_kwargs(
     organization_name: str,
     *,
     json_body: CreateIntegrationRequestGithubAppInstallation,
 ) -> Dict[str, Any]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
-from ...models.create_token_request import CreateTokenRequest
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import cast
 from typing import Dict
+from ...models.create_token_request import CreateTokenRequest
 
 
 def _get_kwargs(
     organization_name: str,
     *,
     json_body: CreateTokenRequest,
 ) -> Dict[str, Any]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import cast
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
     report_id: str,
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
     report_id: str,
 ) -> Dict[str, Any]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.get_report_summary_response import GetReportSummaryResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
     report_id: str,
 ) -> Dict[str, Any]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.report_text_summary_response import ReportTextSummaryResponse
-from ...models.report_text_summary_request import ReportTextSummaryRequest
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
+from ...models.report_text_summary_response import ReportTextSummaryResponse
 from typing import Dict
+from ...models.report_text_summary_request import ReportTextSummaryRequest
 
 
 def _get_kwargs(
     organization_name: str,
     report_id: str,
     *,
     json_body: ReportTextSummaryRequest,
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
+from ...models.validation_error_response import ValidationErrorResponse
 from ...models.invite_user_request import InviteUserRequest
-from ...models.challenge_response import ChallengeResponse
 from ...models.base_error_response import BaseErrorResponse
-from ...models.validation_error_response import ValidationErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import cast
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
     *,
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
+from ...models.validation_error_response import ValidationErrorResponse
 from ...models.base_error_response import BaseErrorResponse
 from ...models.integration_with_status import IntegrationWithStatus
-from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
 from typing import List
+from ...models.challenge_response import ChallengeResponse
+from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
 ) -> Dict[str, Any]:
     return {
         "method": "get",
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
 from ...models.list_reports_response import ListReportsResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
+from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
 ) -> Dict[str, Any]:
     return {
         "method": "get",
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
+from ...models.validation_error_response import ValidationErrorResponse
 from ...models.base_error_response import BaseErrorResponse
 from ...models.integration_with_status import IntegrationWithStatus
-from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
 from typing import List
+from ...models.challenge_response import ChallengeResponse
+from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
 ) -> Dict[str, Any]:
     return {
         "method": "get",
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import cast
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
     integration_uuid: str,
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
+from ...models.validation_error_response import ValidationErrorResponse
 from ...models.base_error_response import BaseErrorResponse
+from ...models.challenge_response import ChallengeResponse
 from ...models.refresh_response import RefreshResponse
-from ...models.validation_error_response import ValidationErrorResponse
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
 ) -> Dict[str, Any]:
     return {
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from ...models.user_tabs_config import UserTabsConfig
 from ...models.ui_status_response import UIStatusResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import Dict
-from ...models.user_tabs_config import UserTabsConfig
 
 
 def _get_kwargs(
     organization_name: str,
     *,
     json_body: UserTabsConfig,
 ) -> Dict[str, Any]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
 from ...models.ui_status_response import UIStatusResponse
+from ...models.challenge_response import ChallengeResponse
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
 ) -> Dict[str, Any]:
     return {
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
+from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
 from ...models.body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post import (
     BodyUploadSnapshotOrganizationNameApiV1UploadsnapshotPost,
 )
-from ...models.base_error_response import BaseErrorResponse
-from ...models.validation_error_response import ValidationErrorResponse
-from typing import cast
 from ...models.upload_snapshot_response import UploadSnapshotResponse
+from ...models.challenge_response import ChallengeResponse
+from typing import cast
 from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
     *,
     multipart_data: BodyUploadSnapshotOrganizationNameApiV1UploadsnapshotPost,
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response, UNSET
 from ... import errors
 
-from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
+from ...models.base_error_response import BaseErrorResponse
 from ...models.upload_snapshot_status_response import UploadSnapshotStatusResponse
+from ...models.challenge_response import ChallengeResponse
+from typing import Dict
 
 
 def _get_kwargs(
     organization_name: str,
     *,
     uuid: str,
 ) -> Dict[str, Any]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
-from typing import Dict
 from ...models.validation_error_response import ValidationErrorResponse
+from typing import Dict
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "get",
         "url": "/favicon.ico",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/client.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/client.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/__init__.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 from .body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post import (
     BodyUploadSnapshotOrganizationNameApiV1UploadsnapshotPost,
 )
 from .challenge_response import ChallengeResponse
 from .challenge_response_challenge import ChallengeResponseChallenge
 from .comparison_reportdata import ComparisonReportdata
 from .comparison_reportdata_files import ComparisonReportdataFiles
+from .console_request_options import ConsoleRequestOptions
 from .create_integration_request_github_app_installation import (
     CreateIntegrationRequestGithubAppInstallation,
 )
 from .create_integration_request_github_app_installation_data import (
     CreateIntegrationRequestGithubAppInstallationData,
 )
 from .create_token_request import CreateTokenRequest
 from .external_status_data_integration import ExternalStatusDataIntegration
 from .external_status_integration import ExternalStatusIntegration
+from .flags_response import FlagsResponse
+from .flags_response_environment import FlagsResponseEnvironment
+from .flags_response_flags import FlagsResponseFlags
 from .generic_state import GenericState
 from .get_report_summary_response import GetReportSummaryResponse
 from .get_report_summary_response_status import GetReportSummaryResponseStatus
 from .get_report_summary_response_summary import GetReportSummaryResponseSummary
 from .integration import Integration
 from .integration_data_github_app_installation import (
     IntegrationDataGithubAppInstallation,
@@ -29,20 +33,22 @@
     IntegrationDataGithubAppInstallationData,
 )
 from .integration_data_github_app_installation_data_extra import (
     IntegrationDataGithubAppInstallationDataExtra,
 )
 from .integration_with_status import IntegrationWithStatus
 from .invite_user_request import InviteUserRequest
+from .list_report_tasks_response import ListReportTasksResponse
 from .list_reports_response import ListReportsResponse
 from .metadata import Metadata
 from .organization import Organization
 from .poc_report_data import POCReportData
 from .refresh_response import RefreshResponse
 from .report import Report
+from .report_task import ReportTask
 from .report_text_summary_request import ReportTextSummaryRequest
 from .report_text_summary_response import ReportTextSummaryResponse
 from .snapshot_report_data import SnapshotReportData
 from .snapshot_report_data_files import SnapshotReportDataFiles
 from .tab_info import TabInfo
 from .tab_info_parameters_type_0 import TabInfoParametersType0
 from .tab_info_state_type_0 import TabInfoStateType0
@@ -58,35 +64,41 @@
 __all__ = (
     "BaseErrorResponse",
     "BodyUploadSnapshotOrganizationNameApiV1UploadsnapshotPost",
     "ChallengeResponse",
     "ChallengeResponseChallenge",
     "ComparisonReportdata",
     "ComparisonReportdataFiles",
+    "ConsoleRequestOptions",
     "CreateIntegrationRequestGithubAppInstallation",
     "CreateIntegrationRequestGithubAppInstallationData",
     "CreateTokenRequest",
     "ExternalStatusDataIntegration",
     "ExternalStatusIntegration",
+    "FlagsResponse",
+    "FlagsResponseEnvironment",
+    "FlagsResponseFlags",
     "GenericState",
     "GetReportSummaryResponse",
     "GetReportSummaryResponseStatus",
     "GetReportSummaryResponseSummary",
     "Integration",
     "IntegrationDataGithubAppInstallation",
     "IntegrationDataGithubAppInstallationData",
     "IntegrationDataGithubAppInstallationDataExtra",
     "IntegrationWithStatus",
     "InviteUserRequest",
     "ListReportsResponse",
+    "ListReportTasksResponse",
     "Metadata",
     "Organization",
     "POCReportData",
     "RefreshResponse",
     "Report",
+    "ReportTask",
     "ReportTextSummaryRequest",
     "ReportTextSummaryResponse",
     "SnapshotReportData",
     "SnapshotReportDataFiles",
     "TabInfo",
     "TabInfoParametersType0",
     "TabInfoStateType0",
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/base_error_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/base_error_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 import json
 
 from ..types import UNSET
 
 from typing import Union
-from typing import List
 from io import BytesIO
+from typing import List
 from ..types import File, FileJsonType
 
 
 T = TypeVar("T", bound="BodyUploadSnapshotOrganizationNameApiV1UploadsnapshotPost")
 
 
 @_attrs_define
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/challenge_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/challenge_response.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import Union
-from typing import Literal
+from ..models.challenge_response_challenge import ChallengeResponseChallenge
 from typing import cast, Union
 from ..types import UNSET, Unset
-from ..models.challenge_response_challenge import ChallengeResponseChallenge
+from typing import Union
+from typing import Literal
 
 
 T = TypeVar("T", bound="ChallengeResponse")
 
 
 @_attrs_define
 class ChallengeResponse:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import Union
+from ..types import UNSET, Unset
 from typing import cast, Union
 from typing import cast
+from typing import Union
 from typing import Dict
-from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.comparison_reportdata_files import ComparisonReportdataFiles
 
 
 T = TypeVar("T", bound="ComparisonReportdata")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_token_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/create_token_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
-from dateutil.parser import isoparse
-from typing import Literal
-from typing import cast, Union
+import datetime
 from ..models.generic_state import GenericState
+from typing import cast, Union
 from typing import cast
+from typing import Literal
 from typing import Dict
-import datetime
+from dateutil.parser import isoparse
 
 if TYPE_CHECKING:
     from ..models.base_error_response import BaseErrorResponse
 
 
 T = TypeVar("T", bound="ExternalStatusDataIntegration")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
+from dateutil.parser import isoparse
 import datetime
 from typing import Dict
-from dateutil.parser import isoparse
 
 if TYPE_CHECKING:
     from ..models.external_status_data_integration import ExternalStatusDataIntegration
 
 
 T = TypeVar("T", bound="ExternalStatusIntegration")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 from typing import Dict
 
 if TYPE_CHECKING:
     from ..models.get_report_summary_response_status import (
         GetReportSummaryResponseStatus,
     )
+    from ..models.report import Report
     from ..models.get_report_summary_response_summary import (
         GetReportSummaryResponseSummary,
     )
-    from ..models.report import Report
 
 
 T = TypeVar("T", bound="GetReportSummaryResponse")
 
 
 @_attrs_define
 class GetReportSummaryResponse:
@@ -56,18 +56,18 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_report_summary_response_status import (
             GetReportSummaryResponseStatus,
         )
+        from ..models.report import Report
         from ..models.get_report_summary_response_summary import (
             GetReportSummaryResponseSummary,
         )
-        from ..models.report import Report
 
         d = src_dict.copy()
         report = Report.from_dict(d.pop("report"))
 
         summary = GetReportSummaryResponseSummary.from_dict(d.pop("summary"))
 
         status = GetReportSummaryResponseStatus.from_dict(d.pop("status"))
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
+from dateutil.parser import isoparse
 import datetime
 from typing import Dict
-from dateutil.parser import isoparse
 
 if TYPE_CHECKING:
     from ..models.integration_data_github_app_installation import (
         IntegrationDataGithubAppInstallation,
     )
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
+from typing import Dict
 from typing import cast, List
 from typing import cast
-from typing import Dict
 
 if TYPE_CHECKING:
     from ..models.integration_data_github_app_installation_data_extra import (
         IntegrationDataGithubAppInstallationDataExtra,
     )
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
 from typing import Dict
 
 if TYPE_CHECKING:
-    from ..models.integration import Integration
     from ..models.external_status_integration import ExternalStatusIntegration
+    from ..models.integration import Integration
 
 
 T = TypeVar("T", bound="IntegrationWithStatus")
 
 
 @_attrs_define
 class IntegrationWithStatus:
@@ -43,16 +43,16 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.integration import Integration
         from ..models.external_status_integration import ExternalStatusIntegration
+        from ..models.integration import Integration
 
         d = src_dict.copy()
         integration = Integration.from_dict(d.pop("integration"))
 
         status = ExternalStatusIntegration.from_dict(d.pop("status"))
 
         integration_with_status = cls(
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
-from typing import List
 from typing import Dict
+from typing import List
 
 if TYPE_CHECKING:
     from ..models.report import Report
 
 
 T = TypeVar("T", bound="ListReportsResponse")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/metadata.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/organization.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/organization.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
+from dateutil.parser import isoparse
 import datetime
 from typing import Dict
-from dateutil.parser import isoparse
 
 if TYPE_CHECKING:
     from ..models.metadata import Metadata
 
 
 T = TypeVar("T", bound="Organization")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/refresh_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/refresh_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/report.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
-from dateutil.parser import isoparse
+import datetime
 from typing import Union
 from typing import Dict
-import datetime
+from dateutil.parser import isoparse
 
 if TYPE_CHECKING:
     from ..models.poc_report_data import POCReportData
     from ..models.snapshot_report_data import SnapshotReportData
 
 
 T = TypeVar("T", bound="Report")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,61 +4,76 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
+from typing import cast, Union
 from ..types import UNSET, Unset
 from typing import Union
 
 
-T = TypeVar("T", bound="ReportTextSummaryRequest")
+T = TypeVar("T", bound="ReportTextSummaryResponse")
 
 
 @_attrs_define
-class ReportTextSummaryRequest:
+class ReportTextSummaryResponse:
     """
     Attributes:
-        mode (Union[Unset, str]):  Default: 'text'.
-        traces (Union[Unset, bool]):
+        text (str):
+        json (Union[None, Unset, str]):
     """
 
-    mode: Union[Unset, str] = "text"
-    traces: Union[Unset, bool] = False
+    text: str
+    json: Union[None, Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        mode = self.mode
-        traces = self.traces
+        text = self.text
+        json: Union[None, Unset, str]
+        if isinstance(self.json, Unset):
+            json = UNSET
+
+        else:
+            json = self.json
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if mode is not UNSET:
-            field_dict["mode"] = mode
-        if traces is not UNSET:
-            field_dict["traces"] = traces
+        field_dict.update(
+            {
+                "text": text,
+            }
+        )
+        if json is not UNSET:
+            field_dict["json"] = json
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        mode = d.pop("mode", UNSET)
-
-        traces = d.pop("traces", UNSET)
+        text = d.pop("text")
 
-        report_text_summary_request = cls(
-            mode=mode,
-            traces=traces,
+        def _parse_json(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        json = _parse_json(d.pop("json", UNSET))
+
+        report_text_summary_response = cls(
+            text=text,
+            json=json,
         )
 
-        report_text_summary_request.additional_properties = d
-        return report_text_summary_request
+        report_text_summary_response.additional_properties = d
+        return report_text_summary_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,76 +4,94 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import cast, Union
 from ..types import UNSET, Unset
-from typing import Union
+from typing import Literal, Union
 
 
-T = TypeVar("T", bound="ReportTextSummaryResponse")
+T = TypeVar("T", bound="CreateClientLoginSessionResponse")
 
 
 @_attrs_define
-class ReportTextSummaryResponse:
+class CreateClientLoginSessionResponse:
     """
     Attributes:
-        text (str):
-        json (Union[None, Unset, str]):
+        status (int):
+        pin (str):
+        url (str):
+        uuid (str):
+        token (str):
+        type (Union[Literal['urn:invariant:responses:init_client_login_response'], Unset]):  Default:
+            'urn:invariant:responses:init_client_login_response'.
     """
 
-    text: str
-    json: Union[None, Unset, str] = UNSET
+    status: int
+    pin: str
+    url: str
+    uuid: str
+    token: str
+    type: Union[
+        Literal["urn:invariant:responses:init_client_login_response"], Unset
+    ] = "urn:invariant:responses:init_client_login_response"
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        text = self.text
-        json: Union[None, Unset, str]
-        if isinstance(self.json, Unset):
-            json = UNSET
-
-        else:
-            json = self.json
+        status = self.status
+        pin = self.pin
+        url = self.url
+        uuid = self.uuid
+        token = self.token
+        type = self.type
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "text": text,
+                "status": status,
+                "pin": pin,
+                "url": url,
+                "uuid": uuid,
+                "token": token,
             }
         )
-        if json is not UNSET:
-            field_dict["json"] = json
+        if type is not UNSET:
+            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        text = d.pop("text")
+        status = d.pop("status")
+
+        pin = d.pop("pin")
+
+        url = d.pop("url")
+
+        uuid = d.pop("uuid")
+
+        token = d.pop("token")
+
+        type = d.pop("type", UNSET)
 
-        def _parse_json(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        json = _parse_json(d.pop("json", UNSET))
-
-        report_text_summary_response = cls(
-            text=text,
-            json=json,
+        create_client_login_session_response = cls(
+            status=status,
+            pin=pin,
+            url=url,
+            uuid=uuid,
+            token=token,
+            type=type,
         )
 
-        report_text_summary_response.additional_properties = d
-        return report_text_summary_response
+        create_client_login_session_response.additional_properties = d
+        return create_client_login_session_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import Union
+from ..types import UNSET, Unset
 from typing import cast, Union
 from typing import cast
+from typing import Union
 from typing import Dict
-from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.snapshot_report_data_files import SnapshotReportDataFiles
     from ..models.comparison_reportdata import ComparisonReportdata
 
 
 T = TypeVar("T", bound="SnapshotReportData")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/tab_info.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
 from typing import cast, Union
-from typing import cast
 from typing import Dict
+from typing import cast
 
 if TYPE_CHECKING:
-    from ..models.tab_info_state_type_0 import TabInfoStateType0
     from ..models.tab_info_parameters_type_0 import TabInfoParametersType0
+    from ..models.tab_info_state_type_0 import TabInfoStateType0
 
 
 T = TypeVar("T", bound="TabInfo")
 
 
 @_attrs_define
 class TabInfo:
@@ -34,16 +34,16 @@
     active: bool
     override_name: Union[None, str]
     parameters: Union["TabInfoParametersType0", None]
     state: Union["TabInfoStateType0", None]
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.tab_info_state_type_0 import TabInfoStateType0
         from ..models.tab_info_parameters_type_0 import TabInfoParametersType0
+        from ..models.tab_info_state_type_0 import TabInfoStateType0
 
         urn = self.urn
         active = self.active
         override_name: Union[None, str]
 
         override_name = self.override_name
 
@@ -75,16 +75,16 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.tab_info_state_type_0 import TabInfoStateType0
         from ..models.tab_info_parameters_type_0 import TabInfoParametersType0
+        from ..models.tab_info_state_type_0 import TabInfoStateType0
 
         d = src_dict.copy()
         urn = d.pop("urn")
 
         active = d.pop("active")
 
         def _parse_override_name(data: object) -> Union[None, str]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
 from typing import cast, Union
-from typing import cast
 from typing import Dict
+from typing import cast
 
 if TYPE_CHECKING:
+    from ..models.user import User
     from ..models.user_tabs_config import UserTabsConfig
     from ..models.organization import Organization
-    from ..models.user import User
 
 
 T = TypeVar("T", bound="UIStatusResponse")
 
 
 @_attrs_define
 class UIStatusResponse:
@@ -59,17 +59,17 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.user import User
         from ..models.user_tabs_config import UserTabsConfig
         from ..models.organization import Organization
-        from ..models.user import User
 
         d = src_dict.copy()
         user = User.from_dict(d.pop("user"))
 
         organization = Organization.from_dict(d.pop("organization"))
 
         def _parse_tabs(data: object) -> Union["UserTabsConfig", None]:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/user.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import Union
-from dateutil.parser import isoparse
+import datetime
+from ..types import UNSET, Unset
 from typing import cast, Union
 from typing import cast
-import datetime
+from typing import Union
 from typing import Dict
-from ..types import UNSET, Unset
+from dateutil.parser import isoparse
 
 if TYPE_CHECKING:
     from ..models.user_metadata import UserMetadata
 
 
 T = TypeVar("T", bound="User")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_metadata.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/user_metadata.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
-from typing import List
 from typing import Dict
+from typing import List
 
 if TYPE_CHECKING:
     from ..models.tab_info import TabInfo
 
 
 T = TypeVar("T", bound="UserTabsConfig")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/validation_error_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
+from typing import Dict
+from typing import cast, Union
+from ..types import UNSET, Unset
 from typing import Union
 from typing import Literal
-from typing import cast, Union
 from typing import cast
-from typing import Dict
-from ..types import UNSET, Unset
 from typing import cast, List
 
 if TYPE_CHECKING:
     from ..models.validation_error_response_part import ValidationErrorResponsePart
 
 
 T = TypeVar("T", bound="ValidationErrorResponse")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/types.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/types.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
 from ...models.base_error_response import BaseErrorResponse
+from typing import Dict
 from ...models.consume_client_login_session_response import (
     ConsumeClientLoginSessionResponse,
 )
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from ...models.fulfill_client_login_request import FulfillClientLoginRequest
+from ...models.base_error_response import BaseErrorResponse
 from typing import Dict
 from typing import cast
-from ...models.base_error_response import BaseErrorResponse
 from ...models.challenge_response import ChallengeResponse
+from ...models.fulfill_client_login_request import FulfillClientLoginRequest
 
 
 def _get_kwargs(
     *,
     json_body: FulfillClientLoginRequest,
 ) -> Dict[str, Any]:
     json_json_body = json_body.to_dict()
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
+from typing import Dict
 from ...models.create_client_login_session_response import (
     CreateClientLoginSessionResponse,
 )
-from typing import Dict
-from ...models.base_error_response import BaseErrorResponse
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "post",
         "url": "/api/v1/client-login",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from ...models.email_check_request import EmailCheckRequest
+from ...models.base_error_response import BaseErrorResponse
 from typing import Dict
+from ...models.email_check_request import EmailCheckRequest
 from typing import cast
-from ...models.base_error_response import BaseErrorResponse
 
 
 def _get_kwargs(
     *,
     json_body: EmailCheckRequest,
 ) -> Dict[str, Any]:
     json_json_body = json_body.to_dict()
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from ...models.check_invite_response import CheckInviteResponse
+from ...models.base_error_response import BaseErrorResponse
 from typing import Dict
+from ...models.check_invite_response import CheckInviteResponse
 from ...models.challenge_response import ChallengeResponse
-from ...models.base_error_response import BaseErrorResponse
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "post",
         "url": "/api/v1/login/check_invite",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
 from typing import Dict
-from typing import List
-from ...models.challenge_response import ChallengeResponse
 from ...models.user import User
+from ...models.challenge_response import ChallengeResponse
+from typing import List
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "post",
         "url": "/api/v1/login/get_instances",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
 from ...models.get_version_response import GetVersionResponse
+from typing import Dict
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "get",
         "url": "/api/v1/login/version",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
+from ...models.base_error_response import BaseErrorResponse
 from typing import Dict
-from ...models.login_request import LoginRequest
 from typing import cast
-from ...models.base_error_response import BaseErrorResponse
 from ...models.challenge_response import ChallengeResponse
+from ...models.login_request import LoginRequest
 
 
 def _get_kwargs(
     *,
     json_body: LoginRequest,
 ) -> Dict[str, Any]:
     json_json_body = json_body.to_dict()
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
+from typing import cast
 from ...models.challenge_response import ChallengeResponse
 from typing import Dict
-from typing import cast
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "post",
         "url": "/api/v1/login/refresh",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from ...models.register_organization_request_body import RegisterOrganizationRequestBody
+from ...models.base_error_response import BaseErrorResponse
 from typing import Dict
 from typing import cast
-from ...models.base_error_response import BaseErrorResponse
+from ...models.register_organization_request_body import RegisterOrganizationRequestBody
 
 
 def _get_kwargs(
     *,
     json_body: RegisterOrganizationRequestBody,
 ) -> Dict[str, Any]:
     json_json_body = json_body.to_dict()
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
 from ...models.base_error_response import BaseErrorResponse
-from ...models.challenge_response import ChallengeResponse
+from typing import Dict
 from typing import cast
+from ...models.challenge_response import ChallengeResponse
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "post",
         "url": "/api/v1/login/resend_validation_pin",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import httpx
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response
 from ... import errors
 
 from ...models.validation_error_response import ValidationErrorResponse
-from typing import Dict
 from typing import cast
 from ...models.base_error_response import BaseErrorResponse
+from typing import Dict
 
 
 def _get_kwargs() -> Dict[str, Any]:
     return {
         "method": "post",
         "url": "/api/v1/github-webhook",
     }
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/client.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/client.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/__init__.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/base_error_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/base_error_response.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from ..types import UNSET, Unset
 from typing import cast, Union
 from typing import Union
+from ..types import UNSET, Unset
 
 
 T = TypeVar("T", bound="BaseErrorResponse")
 
 
 @_attrs_define
 class BaseErrorResponse:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/challenge_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/challenge_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import Union
-from typing import Literal
 from ..types import UNSET, Unset
-from ..models.challenge_response_challenge import ChallengeResponseChallenge
 from typing import cast, Union
+from ..models.challenge_response_challenge import ChallengeResponseChallenge
+from typing import Literal
+from typing import Union
 
 
 T = TypeVar("T", bound="ChallengeResponse")
 
 
 @_attrs_define
 class ChallengeResponse:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/check_invite_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/check_invite_response.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import Literal, Union
 from ..types import UNSET, Unset
+from typing import Literal, Union
 
 
 T = TypeVar("T", bound="CheckInviteResponse")
 
 
 @_attrs_define
 class CheckInviteResponse:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import cast, Union
-from typing import Literal, Union
 from ..types import UNSET, Unset
+from typing import Literal, Union
+from typing import cast, Union
 
 
 T = TypeVar("T", bound="ConsumeClientLoginSessionResponse")
 
 
 @_attrs_define
 class ConsumeClientLoginSessionResponse:
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/report_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,96 +2,106 @@
 
 from typing import List
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..types import UNSET, Unset
 
-from typing import Literal, Union
-from ..types import UNSET, Unset
+import datetime
+from dateutil.parser import isoparse
 
 
-T = TypeVar("T", bound="CreateClientLoginSessionResponse")
+T = TypeVar("T", bound="ReportTask")
 
 
 @_attrs_define
-class CreateClientLoginSessionResponse:
+class ReportTask:
     """
     Attributes:
-        status (int):
-        pin (str):
-        url (str):
         uuid (str):
-        token (str):
-        type (Union[Literal['urn:invariant:responses:init_client_login_response'], Unset]):  Default:
-            'urn:invariant:responses:init_client_login_response'.
+        organization_uuid (str):
+        created_at (datetime.datetime):
+        urn (str):
+        type (str):
+        initiator_urn (str):
+        worker_pod (str):
+        was_killed (bool):
     """
 
-    status: int
-    pin: str
-    url: str
     uuid: str
-    token: str
-    type: Union[
-        Literal["urn:invariant:responses:init_client_login_response"], Unset
-    ] = "urn:invariant:responses:init_client_login_response"
+    organization_uuid: str
+    created_at: datetime.datetime
+    urn: str
+    type: str
+    initiator_urn: str
+    worker_pod: str
+    was_killed: bool
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        status = self.status
-        pin = self.pin
-        url = self.url
         uuid = self.uuid
-        token = self.token
+        organization_uuid = self.organization_uuid
+        created_at = self.created_at.isoformat()
+
+        urn = self.urn
         type = self.type
+        initiator_urn = self.initiator_urn
+        worker_pod = self.worker_pod
+        was_killed = self.was_killed
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "status": status,
-                "pin": pin,
-                "url": url,
                 "uuid": uuid,
-                "token": token,
+                "organization_uuid": organization_uuid,
+                "created_at": created_at,
+                "urn": urn,
+                "type": type,
+                "initiator_urn": initiator_urn,
+                "worker_pod": worker_pod,
+                "was_killed": was_killed,
             }
         )
-        if type is not UNSET:
-            field_dict["type"] = type
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        status = d.pop("status")
+        uuid = d.pop("uuid")
 
-        pin = d.pop("pin")
+        organization_uuid = d.pop("organization_uuid")
 
-        url = d.pop("url")
+        created_at = isoparse(d.pop("created_at"))
 
-        uuid = d.pop("uuid")
+        urn = d.pop("urn")
+
+        type = d.pop("type")
+
+        initiator_urn = d.pop("initiator_urn")
 
-        token = d.pop("token")
+        worker_pod = d.pop("worker_pod")
 
-        type = d.pop("type", UNSET)
+        was_killed = d.pop("was_killed")
 
-        create_client_login_session_response = cls(
-            status=status,
-            pin=pin,
-            url=url,
+        report_task = cls(
             uuid=uuid,
-            token=token,
+            organization_uuid=organization_uuid,
+            created_at=created_at,
+            urn=urn,
             type=type,
+            initiator_urn=initiator_urn,
+            worker_pod=worker_pod,
+            was_killed=was_killed,
         )
 
-        create_client_login_session_response.additional_properties = d
-        return create_client_login_session_response
+        report_task.additional_properties = d
+        return report_task
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_check_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/email_check_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_password_login.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/email_password_login.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/get_version_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/get_version_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/login.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/login_request.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from ..types import UNSET, Unset
 from typing import Dict
-from typing import cast
-from typing import Union
+from ..types import UNSET, Unset
 from typing import cast, Union
+from typing import Union
+from typing import cast
 
 if TYPE_CHECKING:
-    from ..models.email_password_login import EmailPasswordLogin
-    from ..models.reset_pin_request import ResetPINRequest
-    from ..models.reset_request import ResetRequest
     from ..models.validation_request import ValidationRequest
     from ..models.new_password_request import NewPasswordRequest
+    from ..models.reset_pin_request import ResetPINRequest
+    from ..models.reset_request import ResetRequest
+    from ..models.email_password_login import EmailPasswordLogin
 
 
 T = TypeVar("T", bound="LoginRequest")
 
 
 @_attrs_define
 class LoginRequest:
@@ -41,19 +41,19 @@
     email_valid: Union["ValidationRequest", None, Unset] = UNSET
     reset_request: Union["ResetRequest", None, Unset] = UNSET
     reset_pin_request: Union["ResetPINRequest", None, Unset] = UNSET
     new_password: Union["NewPasswordRequest", None, Unset] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.email_password_login import EmailPasswordLogin
-        from ..models.reset_pin_request import ResetPINRequest
-        from ..models.reset_request import ResetRequest
         from ..models.validation_request import ValidationRequest
         from ..models.new_password_request import NewPasswordRequest
+        from ..models.reset_pin_request import ResetPINRequest
+        from ..models.reset_request import ResetRequest
+        from ..models.email_password_login import EmailPasswordLogin
 
         basic_auth: Union[Dict[str, Any], None, Unset]
         if isinstance(self.basic_auth, Unset):
             basic_auth = UNSET
 
         elif isinstance(self.basic_auth, EmailPasswordLogin):
             basic_auth = UNSET
@@ -125,19 +125,19 @@
         if new_password is not UNSET:
             field_dict["new_password"] = new_password
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.email_password_login import EmailPasswordLogin
-        from ..models.reset_pin_request import ResetPINRequest
-        from ..models.reset_request import ResetRequest
         from ..models.validation_request import ValidationRequest
         from ..models.new_password_request import NewPasswordRequest
+        from ..models.reset_pin_request import ResetPINRequest
+        from ..models.reset_request import ResetRequest
+        from ..models.email_password_login import EmailPasswordLogin
 
         d = src_dict.copy()
 
         def _parse_basic_auth(data: object) -> Union["EmailPasswordLogin", None, Unset]:
             if data is None:
                 return data
             if isinstance(data, Unset):
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/new_password_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/new_password_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/organization.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/reset_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/user.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/user.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 
 from typing import Dict
 
 if TYPE_CHECKING:
-    from ..models.login import Login
     from ..models.organization import Organization
+    from ..models.login import Login
 
 
 T = TypeVar("T", bound="User")
 
 
 @_attrs_define
 class User:
@@ -60,16 +60,16 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.login import Login
         from ..models.organization import Organization
+        from ..models.login import Login
 
         d = src_dict.copy()
         uuid = d.pop("uuid")
 
         organization = Organization.from_dict(d.pop("organization"))
 
         login = Login.from_dict(d.pop("login"))
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import UNSET, Unset
 
-from typing import Dict
-from typing import cast, List
-from typing import Union
-from typing import Literal
-from typing import cast
 from ..types import UNSET, Unset
+from typing import cast, List
 from typing import cast, Union
+from typing import cast
+from typing import Literal
+from typing import Dict
+from typing import Union
 
 if TYPE_CHECKING:
     from ..models.validation_error_response_part import ValidationErrorResponsePart
 
 
 T = TypeVar("T", bound="ValidationErrorResponse")
```

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_request.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/models/validation_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/types.py` & `invariant_client-1.3.0/invariant_client/bindings/invariant_login_client/types.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/cli.py` & `invariant_client-1.3.0/invariant_client/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import datetime
 import io
 import json
 import logging
 import logging.config
 import os
 import pathlib
-from retry.api import retry_call
 import ssl
 import stat
 import sys
 import time
 import uuid
 
 from attrs import asdict
+from retry.api import retry_call
+from rich import print_json
 from tabulate import tabulate
 
 from invariant_client import auth, display, zip_util
 from invariant_client import pysdk
 from invariant_client.bindings.invariant_instance_client.models.snapshot_report_data import SnapshotReportData
 from invariant_client.display import OutputFormat
 from invariant_client.version import VersionClient
@@ -69,14 +70,20 @@
         parser.add_argument(
             '--json',
             dest='json',
             action='store_true',
             help='Output data as JSON.',
         )
         parser.add_argument(
+            '--fast-json',
+            dest='fast_json',
+            action='store_true',
+            help='Output data as JSON (unformatted).',
+        )
+        parser.add_argument(
             '--tsv',
             dest='tsv',
             action='store_true',
             help='Output data as TSV.',
         )
 
     
@@ -95,24 +102,25 @@
     command_run.add_argument(
         '--target',
         dest='target',
         help='An Invariant project root directory. Default is current directory.',
     )
 
     command_show.add_argument(
-        'snapshot_name',
-        help='The snapshot to examine.'
-    )
-
-    command_show.add_argument(
         'file_name',
         nargs="?",
         help='The snapshot file to examine.'
     )
 
+    command_show.add_argument(
+        '--snapshot',
+        dest='snapshot_name',
+        help='The snapshot to examine. If unset, environment variable INVARIANT_SNAPSHOT is used.'
+    )
+
     command_solution.add_argument(
         'snapshot_name',
         help='The snapshot to examine.'
     )
 
     command_solution.add_argument(
         'solution_name',
@@ -187,14 +195,16 @@
         format = None
     else:
         command = getattr(args, 'command')
 
         format = OutputFormat.TABULATE
         if getattr(args, 'json'):
             format = OutputFormat.JSON
+        elif getattr(args, 'fast_json'):
+            format = OutputFormat.FAST_JSON
         elif getattr(args, 'tsv'):
             format = OutputFormat.TSV
         
     debug = getattr(args, 'debug') or False
     configure_logging(debug)
     
     try:
@@ -209,15 +219,16 @@
 def EntryPoint_inner(args, command, format, debug):
     settings: pysdk.Settings = {
         'format': format,
         'debug': debug,
     }
 
     env = dict(os.environ)
-    invariant_domain = env.get('INVARIANT_DOMAIN', 'https://invariant.tech')
+    invariant_domain = env.get('INVARIANT_DOMAIN', 'https://prod.invariant.tech')
+    env_snapshot = env.get('INVARIANT_SNAPSHOT', None)
 
     creds = None
 
     if args.version:
         with open(pathlib.Path(__file__).parent.parent.joinpath("VERSION"), "r") as f:
             print(f"client: {f.read().strip()}")
         print(f"server: {VersionClient(invariant_domain, ssl.create_default_context()).get_version()}")
@@ -240,25 +251,25 @@
                     creds = result
                     break
                 elif isinstance(result, int):
                     time.sleep(result)
                 else:
                     time.sleep(2)
             if not creds:
-                print("Timed out.")
+                print("Timed out.", file=sys.stderr)
                 exit(1)
             with open(CREDS_FILE_PATH, 'w') as f:
                 f.write(creds.to_json())
             CREDS_FILE_PATH.chmod(
                 stat.S_IRUSR |
                 stat.S_IWUSR
             )
             print("Login successful.")
         except KeyboardInterrupt as e:
-            print("Exiting...")
+            print("Exiting...", file=sys.stderr)
             exit(1)
 
         exit(0)
     
     # Load credentials or error
     try:
         creds = pysdk.AccessCredential.from_env(env, base_url=invariant_domain)
@@ -300,24 +311,41 @@
             zip_util.zip_dir(target, bytes)  # Write a zip file into 'bytes'
         else:
             print("Unacceptable target", file=sys.stderr)
             print(str(target), file=sys.stderr)
             exit(1)
 
         compare_to = getattr(args, 'compare_to')
-        exec_uuid = retry_call(upload_snapshot, fargs=[sdk, bytes, compare_to], exceptions=UploadTerminationError,tries=3, delay=30, backoff=2)
+        try:
+            exec_uuid = retry_call(
+                upload_snapshot,
+                fargs=[sdk, bytes, compare_to],
+                exceptions=UploadTerminationError,
+                tries=3,
+                delay=2,
+                backoff=2)
+        except KeyboardInterrupt as e:
+            print("Exiting...", file=sys.stderr)
+            exit(1)
+
         print("Analysis complete.")
         response = sdk.snapshot_detail(exec_uuid)
         # pprint.pprint(asdict(response), width=200)
         display.snapshot_status(response)
         if response.status['state'] == 'COMPLETE':
             display.snapshot_halted(response)
             print('')
-            display.snapshot_summary_table(response, format)
-            print(f"\nRun 'invariant show {exec_uuid} <file>' to examine any file.")
+            summary = sdk.snapshot_detail_text(str(exec_uuid), json_mode=False)
+            if summary.text:
+                print(summary.text)
+            else:
+                display.snapshot_summary_table(response, format)
+
+            print(f"\nRun 'invariant show <file> --snapshot {exec_uuid}' to examine any file,")
+            print(f"or run 'export INVARIANT_SNAPSHOT={exec_uuid}' to skip the --snapshot argument.")
 
             if response.summary['errors'] > 0:
                 print(f"\n{response.summary['errors']} {'error' if response.summary['errors'] == 1 else 'errors'} found.")
                 errors_uuid = response.report.reports.errors
                 errors_response = sdk.snapshot_file(errors_uuid)
                 display.snapshot_errors(errors_response, format)
 
@@ -326,36 +354,39 @@
                 errors_uuid = response.report.reports.errors
                 errors_response = sdk.snapshot_file(errors_uuid)
                 display.snapshot_errors(errors_response, format)
 
     elif command == "snapshots":
         snapshots = sdk.list_snapshots()
         if format == OutputFormat.JSON:
+            print_json(data=asdict(snapshots, value_serializer=serialize), default=vars)
+        elif format == OutputFormat.FAST_JSON:
             print(json.dumps(asdict(snapshots, value_serializer=serialize), default=vars))
         elif format == OutputFormat.TSV:
             reports = asdict(snapshots)
             reports = reports['reports']
             print(tabulate(reports, headers='keys', tablefmt='tsv'))
         # if format == 'markdown':
         #     return tabulate(result, headers='keys', tablefmt='github')
         else:
             reports = asdict(snapshots)
             reports = reports['reports']
             print(tabulate(reports, headers='keys', tablefmt='psql'))
 
-    elif command == "snapshot":
-        sdk.snapshot_detail(
-            report_uuid=args.snapshot_name)
-
     elif command == "show":
+        snapshot_name = args.snapshot_name
+        if not snapshot_name:
+            snapshot_name = env_snapshot
+        if not snapshot_name:
+            raise ValueError(f"Missing --snapshot <name> argument or INVARIANT_SNAPSHOT environment variable.")
+
         try:
-            exec_uuid = uuid.UUID(args.snapshot_name, version=4)
+            exec_uuid = uuid.UUID(snapshot_name, version=4)
         except ValueError as e:
-            # TODO we could permit something like 'latest'
-            raise ValueError(f"Expected {args.snapshot_name} to be a UUID like f5b4e387-e336-499e-b3a0-d6186c590572.") from e
+            raise ValueError(f"Expected {snapshot_name} to be a UUID like f5b4e387-e336-499e-b3a0-d6186c590572.") from e
 
         if args.file_name is not None:
             # Access a specific file
             try:
                 file = uuid.UUID(args.file_name, version=4)
             except ValueError:
                 # OK if the file is the file key (e.g. errors)
@@ -372,21 +403,31 @@
                         raise ValueError(f"Report {file} not found for snapshot {exec_uuid}.") from e
                     try:
                         file: str = reports.files[file]
                         file = uuid.UUID(file, version=4)
                     except KeyError as e:
                         raise ValueError(f"Report {file} not found for snapshot {exec_uuid}.") from e
 
-            if format == OutputFormat.JSON:
+            if format == OutputFormat.JSON or format == OutputFormat.FAST_JSON:
                 file_summary = sdk.snapshot_file_text(str(file), False, json_mode=True)
                 if file_summary.json:
-                    print(file_summary.json)
+                    if format == OutputFormat.JSON:
+                        try:
+                            print_json(file_summary.json)
+                        except:
+                            print(file_summary.json)
+                    elif format == OutputFormat.FAST_JSON:
+                        print(file_summary.json)
                 else:
                     file_data = sdk.snapshot_file(str(file))
-                    print(file_data.to_json(orient='records'))
+                    if format == OutputFormat.JSON:
+                        print_json(file_data.to_json(orient='records'))
+                    elif format == OutputFormat.FAST_JSON:
+                        print(file_data.to_json(orient='records'))
+
             elif format == OutputFormat.TSV:
                 file_data = sdk.snapshot_file(str(file))
                 display.print_frame(file_data, format)
             else:
                 file_summary = sdk.snapshot_file_text(str(file), False, json_mode=False)
                 if file_summary.text:
                     print(file_summary.text)
@@ -395,33 +436,60 @@
                     display.print_frame(file_data, format)
                 # print("Set --traces to display all example traces")
                 print("Set --json to get JSON")
                 print("See 'show --help' for more options")
 
         else:
             # Display the process summary for the snapshot
-            response = sdk.snapshot_detail(exec_uuid)
-            display.snapshot_status(response)
+            if format == OutputFormat.TABULATE:
+                print(f"Snapshot {exec_uuid}")
+            response = sdk.snapshot_detail(str(exec_uuid))
+            if format == OutputFormat.TABULATE:
+                display.snapshot_status(response)
             if response.status['state'] == 'COMPLETE':
-                display.snapshot_halted(response)
-                print('')
-                display.snapshot_summary_table(response, format)
-                print(f"\nRun 'invariant show {exec_uuid} <file>' to examine any file.")
-
-                if response.summary['errors'] > 0:
-                    print(f"\n{response.summary['errors']} {'error' if response.summary['errors'] == 1 else 'errors'} found.")
-                    errors_uuid = response.report.reports.errors
-                    errors_response = sdk.snapshot_file(errors_uuid)
-                    display.snapshot_errors(errors_response, format)
-
-            else:
-                if response.summary['errors'] > 0:
-                    errors_uuid = response.report.reports.errors
-                    errors_response = sdk.snapshot_file(errors_uuid)
-                    display.snapshot_errors(errors_response, format)
+                if format == OutputFormat.TABULATE:
+                    display.snapshot_halted(response)
+                    print('')
+                if format == OutputFormat.TABULATE:
+                    summary = sdk.snapshot_detail_text(str(exec_uuid), json_mode=False)
+                    if summary.text:
+                        print(summary.text)
+                    else:
+                        display.snapshot_summary_table(response, format)
+
+                elif format == OutputFormat.JSON or format == OutputFormat.FAST_JSON:
+                    summary = sdk.snapshot_detail_text(str(exec_uuid), json_mode=True)
+                    if summary.json:
+                        if format == OutputFormat.JSON:
+                            try:
+                                print_json(summary.json)
+                            except:
+                                print(summary.json)
+                        elif format == OutputFormat.FAST_JSON:
+                            print(summary.json)
+                    else:
+                        display.snapshot_summary_table(response, format)
+                else:
+                    display.snapshot_summary_table(response, format)
+                if format == OutputFormat.TABULATE:
+                    if env_snapshot:
+                        print(f"\nRun 'invariant show <file>' to examine any file.")
+                    else:
+                        print(f"\nRun 'invariant show <file> --snapshot {exec_uuid}' to examine any file,")
+                        print(f"or run 'export INVARIANT_SNAPSHOT={exec_uuid}' to skip the --snapshot argument.")
+
+                    if response.summary['errors'] > 0:
+                        print(f"\n{response.summary['errors']} {'error' if response.summary['errors'] == 1 else 'errors'} found.", file=sys.stderr)
+                        errors_uuid = response.report.reports.errors
+                        errors_response = sdk.snapshot_file(errors_uuid)
+                        display.snapshot_errors(errors_response, format)
+            elif response.summary['errors'] > 0:
+                errors_uuid = response.report.reports.errors
+                errors_response = sdk.snapshot_file(errors_uuid)
+                display.snapshot_errors(errors_response, format)
 
     elif command == "show_solution":
         sdk.show_solution(
             snapshot=args.snapshot_name,
             solution=args.solution_name)
 
     else:
@@ -443,10 +511,10 @@
         if not response.is_running:
             break
         
         # TODO send some RetryAfter header to control this
         # TODO separately, exponential back-off on error
         time.sleep(4)
     if not response:
-        print("Timed out.")
+        print("Timed out.", file=sys.stderr)
         exit(1)
     return exec_uuid
```

### Comparing `invariant_client-1.1.2/invariant_client/display.py` & `invariant_client-1.3.0/invariant_client/display.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import enum
 import json
+import sys
 from attr import asdict
 import pandas
+from rich import print_json
 from tabulate import tabulate
 from invariant_client.bindings.invariant_instance_client.models.get_report_summary_response import GetReportSummaryResponse
 
 
 class OutputFormat(enum.Enum):
     TABULATE = enum.auto()
     JSON = enum.auto()
     TSV = enum.auto()
+    FAST_JSON = enum.auto()
     # etc
 
 
 def snapshot_status(response: GetReportSummaryResponse):
     """Display a message indicating the overall status of the analysis user task."""
     status = response.status.to_dict()
     status = status.get('state')
@@ -24,15 +27,17 @@
     elif status == 'INCOMPLETE':
         print("Error: Snapshot evaluation did not finish.")
 
 
 def snapshot_summary_table(response: GetReportSummaryResponse, format: OutputFormat):
     """Display a table containing row counts for all emitted reports."""
     if format == OutputFormat.JSON:
-        pass
+        print_json(data=response.to_dict())
+    elif format == OutputFormat.FAST_JSON:
+        print(json.dumps(response.to_dict()))
     else:
         print_frame(pandas.DataFrame(response.summary.to_dict().items(), columns=['File', 'RowCount']), format)
 
 
 def snapshot_halted(response: GetReportSummaryResponse):
     """Describe each halted step."""
     status = response.status.to_dict()
@@ -61,18 +66,18 @@
             prefix = ""
             if not i % 10:
                 prefix = f"In {label}{' (continued)' if i > 0 else ''}:\n\n"
             data = json.loads(error['detail'])
             if data['type'] == 'urn:invariant:errors:child_step_failed':
                 continue
             if data['type'] == 'urn:invariant:errors:internal_exception':
-                print(f"\nInternal error in {label}:\n    {data['detail']}")
+                print(f"\nInternal error in {label}:\n    {data['detail']}", file=sys.stderr)
                 continue
 
-            print(f"\n{prefix}    {data['title']}\n    {data['detail']}")
+            print(f"\n{prefix}    {data['title']}\n    {data['detail']}", file=sys.stderr)
 
 
 def print_frame(data: pandas.DataFrame, format: OutputFormat):
     if format == OutputFormat.TSV:
         print(tabulate(data, headers='keys', tablefmt='tsv'))
     elif format == OutputFormat.TABULATE:
         print(tabulate(data, headers='keys', tablefmt='psql'))
```

### Comparing `invariant_client-1.1.2/invariant_client/pysdk.py` & `invariant_client-1.3.0/invariant_client/pysdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 from invariant_client.bindings.invariant_instance_client.api.organization.list_reports_organization_name_api_v_1_reports_get import sync_detailed as list_reports_organization_name_api_v_1_reports_get
 from invariant_client.bindings.invariant_instance_client.api.organization.refresh_organization_name_api_v1_refresh_post import sync_detailed as refresh_organization_name_api_v1_refresh_post
 from invariant_client.bindings.invariant_instance_client.models.report_text_summary_request import ReportTextSummaryRequest
 from invariant_client.bindings.invariant_login_client.client import AuthenticatedClient as LoginAuthenticatedClient, Client as LoginClient
 from invariant_client.bindings.invariant_instance_client.api.organization.upload_snapshot_organization_name_api_v_1_uploadsnapshot_post import sync_detailed as upload_snapshot_organization_name_api_v_1_uploadsnapshot_post
 from invariant_client.bindings.invariant_instance_client.api.organization.upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get import sync_detailed as upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get
 from invariant_client.bindings.invariant_instance_client.api.organization.get_report_summary_organization_name_api_v_1_reports_report_id_summary_get import sync_detailed as get_report_summary_organization_name_api_v_1_reports_report_id_summary_get
+from invariant_client.bindings.invariant_instance_client.api.organization.get_report_summary_text_summary_organization_name_api_v_1_reports_report_id_summary_text_get import sync_detailed as get_report_summary_text_summary_organization_name_api_v_1_reports_report_id_summary_text_get
 from invariant_client.bindings.invariant_instance_client.api.organization.get_report_organization_name_api_v_1_reports_report_id_get import _get_kwargs as get_report_organization_name_api_v_1_reports_report_id_get__get_kwargs
 from invariant_client.bindings.invariant_instance_client.api.organization.get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get import sync_detailed as get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get
 
 from invariant_client.bindings.invariant_login_client.api.login.get_instances_api_v1_login_get_instances_post import sync_detailed as get_instances_api_v1_login_get_instances_post
 from invariant_client.bindings.invariant_login_client.models.base_error_response import BaseErrorResponse
 from invariant_client.bindings.invariant_login_client.models.validation_error_response import ValidationErrorResponse
 
 
-DOMAIN_NAME = "https://invariant.tech"
+
+DOMAIN_NAME = "https://prod.invariant.tech"
 
 
 class NoOrganization(Exception):
     """Credentials must be paired with an organization name."""
 
 
 ErrorResponseType: TypeAlias = BaseErrorResponse | ValidationErrorResponse
@@ -206,38 +208,60 @@
             raise RemoteError(f"Unable to connect to {self.base_url}")
         if isinstance(response, models.ChallengeResponse):
             raise AuthorizationException(f"{response.title}: {response.detail}")
         if not isinstance(response, models.UploadSnapshotStatusResponse):
             raise RemoteError(response)
         return response
 
-    def list_snapshots(self):
+    def list_snapshots(self) -> models.ListReportsResponse:
         response = list_reports_organization_name_api_v_1_reports_get(self.creds.organization_name, client=self.client)
         response = response.parsed
         if not response:
             raise RemoteError(f"Unable to connect to {self.base_url}")
         if isinstance(response, models.ChallengeResponse):
             raise AuthorizationException(f"{response.title}: {response.detail}")
         if not isinstance(response, models.ListReportsResponse):
             raise RemoteError(response)
         return response
 
     def snapshot_detail(
             self,
-            report_uuid: str):
+            report_uuid: str) -> models.GetReportSummaryResponse:
         response = get_report_summary_organization_name_api_v_1_reports_report_id_summary_get(self.creds.organization_name, report_uuid, client=self.client)
         response = response.parsed
         if not response:
             raise RemoteError(f"Unable to connect to {self.base_url}")
         if isinstance(response, models.ChallengeResponse):
             raise AuthorizationException(f"{response.title}: {response.detail}")
         if not isinstance(response, models.GetReportSummaryResponse):
             raise RemoteError(response)
         return response
 
+    def snapshot_detail_text(
+            self,
+            report_uuid: str,
+            json_mode: bool
+        ) -> models.ReportTextSummaryResponse:
+        json_body = ReportTextSummaryRequest(
+            traces=False,
+            mode='json' if json_mode else 'text')
+        response = get_report_summary_text_summary_organization_name_api_v_1_reports_report_id_summary_text_get(
+            self.creds.organization_name,
+            report_uuid,
+            client=self.client,
+            json_body=json_body)
+        response = response.parsed
+        if not response:
+            raise RemoteError(f"Unable to connect to {self.base_url}")
+        if isinstance(response, models.ChallengeResponse):
+            raise AuthorizationException(f"{response.title}: {response.detail}")
+        if not isinstance(response, models.ReportTextSummaryResponse):
+            raise RemoteError(response)
+        return response
+
     def snapshot_file(
             self,
             file_uuid: str) -> pandas.DataFrame:
         kwargs = get_report_organization_name_api_v_1_reports_report_id_get__get_kwargs(
             organization_name=self.creds.organization_name,
             report_id=file_uuid,
         )
```

### Comparing `invariant_client-1.1.2/invariant_client/version.py` & `invariant_client-1.3.0/invariant_client/version.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/invariant_client/zip_util.py` & `invariant_client-1.3.0/invariant_client/zip_util.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.2/pyproject.toml` & `invariant_client-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "invariant-client"
-version = "1.1.2"
+version = "1.3.0"
 description = "Invariant: manage ACLs in an entirely new way"
 authors = ["Rob Ankeny <ankenyr@gmail.com>", "Jason Benterou <jason.benterou@invariant.tech>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 invariant = "invariant_client.cli:EntryPoint"
```

