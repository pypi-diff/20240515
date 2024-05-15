# Comparing `tmp/ophyd_devices-1.0.0.tar.gz` & `tmp/ophyd_devices-1.0.1.tar.gz`

## Comparing `ophyd_devices-1.0.0.tar` & `ophyd_devices-1.0.1.tar`

### file list

```diff
@@ -1,379 +1,385 @@
--rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/README.md
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/.git_hooks/pre-commit
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.gitignore
--rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.gitlab-ci.yml
--rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.pylintrc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.readthedocs.yaml
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/CHANGELOG.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/LICENSE
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/README.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_config_template.yaml
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.git_hooks/post-commit
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.git_hooks/pre-commit
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/demo.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
--rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/main.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py
--rw-r--r--   0        0        0    11083 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/signals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
--rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/scan_progress.py
--rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/conftest.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_scan_progress.py
--rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
--rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/README.md
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/pyproject.toml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bec_service.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bec_yaml_loader.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/client.py
--rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/connector.py
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    30862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/device.py
--rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    38065 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/logger.py
--rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/plugin_helper.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/queue_items.py
--rw-r--r--   0        0        0    41414 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/request_items.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_data.py
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_report.py
--rw-r--r--   0        0        0    17050 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/serialization.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_bec_logger.py
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_callback_handler.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_config_helper.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_core_utils.py
--rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_device_manager.py
--rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_file_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_pdf_writer.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_plugin_helper.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_redis_connector.py
--rw-r--r--   0        0        0    22103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_data.py
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_items.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_object.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/tests/test_yaml_loader.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/init_config.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/README.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/pyproject.toml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    18918 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18406 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    52628 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    27483 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
--rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/bin/install_bec_dev.sh
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/ci/Dockerfile.run_pytest
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/ci/Dockerfile.run_server
--rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/ci/build_python_services.sh
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/ci/docker-compose.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/ci/functionalAccounts.json
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/ci/semantic_release.toml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/ci/test_config.yaml
--rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/architecture/BEC.drawio
--rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/architecture/BEC_config_db.drawio
--rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/architecture/BEC_config_db.svg
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/architecture/bec_architecture.png
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/Makefile
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/conf.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/make.bat
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/requirements.txt
--rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/_static/bec.png
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/_static/switcher.json
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/_static/css/custom.css
--rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/_static/gif/bec_plotter.gif
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/BEC_context_user_centric.png
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/bec_architecture.png
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/bec_device_structure.drawio
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/bec_device_structure.png
--rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/gauss_scatter_plot.png
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/simulation_context_diagram.drawio
--rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/simulation_context_diagram.png
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/tab-complete-devices.png
--rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/vscode_debug_button.png
--rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/vscode_with_annotations.drawio
--rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/vscode_with_annotations.png
--rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/assets/wm-devices.png
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/architecture.md
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/bec_cli.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/bec_config.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/bec_gui.md
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/bec_plugins.md
--rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/bec_sim.md
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/contributing.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/data_access.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/developer.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/event_data.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/external_sources.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/glossary.md
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/install_developer_env.md
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/logs.md
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/modules.rst
--rw-r--r--   0        0        0    17431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/ophyd.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/reference.md
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/tests.md
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/developer/vscode.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/introduction/introduction.md
--rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/user/command_line_interface.md
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/user/data_access_and_plotting.md
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/user/devices.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/user/graphical_user_interface.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/user/installation.md
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/docs/source/user/user.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/pytest_bec_e2e/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/ophyd_patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/configs/__init__.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/configs/ophyd_devices_simulation.yaml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/configs/ophyd_simulation.yaml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/configs/sls_devices.yaml
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/SpmBase.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/XbpmBase.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/__init__.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/epics_motor_ex.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/mono_dccm.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/slits.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/slsDetector.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/sls_devices.py
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/devices/specMotors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/interfaces/base_classes/__init__.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
--rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/interfaces/protocols/__init__.py
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/interfaces/protocols/bec_protocols.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/__init__.py
--rw-r--r--   0        0        0    27733 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/sim.py
--rw-r--r--   0        0        0    28125 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/sim_data.py
--rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/sim_frameworks.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/sim_signals.py
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/sim_test_devices.py
--rw-r--r--   0        0        0    13630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/sim_xtreme.py
--rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/__init__.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/bec_device_base.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/bec_scaninfo_mixin.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/bec_utils.py
--rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/controller.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/dynamic_pseudo.py
--rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/socket.py
--rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/ophyd_devices/utils/static_device_test.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/tests/test_controller.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/tests/test_dynamic_pseudo.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/tests/test_ophyd_status_obj.py
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/tests/test_simulation.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/tests/test_socket.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/tests/test_static_device_test.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/LICENSE
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/README.md
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitignore
+-rw-r--r--   0        0        0    19162 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab-ci.yml
+-rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.pylintrc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.readthedocs.yaml
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/CHANGELOG.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/LICENSE
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/README.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_config_template.yaml
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.git_hooks/post-commit
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/demo.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8571 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11083 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/scan_progress.py
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/conftest.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_scan_progress.py
+-rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/README.md
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/pyproject.toml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_yaml_loader.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/client.py
+-rw-r--r--   0        0        0     9096 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/connector.py
+-rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    30862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/device.py
+-rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    38065 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logger.py
+-rw-r--r--   0        0        0    24024 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    41414 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    17050 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/import_utils.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/proxy.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/rpc_utils.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/scan_utils.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/threading_utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_file_utils.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_import_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    22103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/tests/test_yaml_loader.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/init_config.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/pyproject.toml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    18918 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22491 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18406 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    52628 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25388 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    27483 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
+-rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/bin/install_bec_dev.sh
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/Dockerfile.run_pytest
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/Dockerfile.run_server
+-rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/build_python_services.sh
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/docker-compose.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/functionalAccounts.json
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/semantic_release.toml
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/ci/test_config.yaml
+-rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/BEC.drawio
+-rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.drawio
+-rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.svg
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/architecture/bec_architecture.png
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/Makefile
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/conf.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/make.bat
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/requirements.txt
+-rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/bec.png
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/switcher.json
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/css/custom.css
+-rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_static/gif/bec_plotter.gif
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/BEC_context_user_centric.png
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/bec_architecture.png
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.drawio
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.png
+-rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/gauss_scatter_plot.png
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.drawio
+-rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.png
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/tab-complete-devices.png
+-rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/vscode_debug_button.png
+-rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.drawio
+-rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.png
+-rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/assets/wm-devices.png
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/architecture.md
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_cli.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_config.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_gui.md
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_plugins.md
+-rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/bec_sim.md
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/contributing.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/data_access.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/developer.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/event_data.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/external_sources.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/glossary.md
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/install_developer_env.md
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/logs.md
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/modules.rst
+-rw-r--r--   0        0        0    17431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/ophyd.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/reference.md
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/tests.md
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/developer/vscode.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/introduction/introduction.md
+-rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/command_line_interface.md
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/data_access_and_plotting.md
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/devices.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/graphical_user_interface.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/installation.md
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/docs/source/user/user.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/pytest_bec_e2e/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/ophyd_patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_devices_simulation.yaml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_simulation.yaml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/configs/sls_devices.yaml
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/SpmBase.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/XbpmBase.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/__init__.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/epics_motor_ex.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/mono_dccm.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/slits.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/slsDetector.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/sls_devices.py
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/devices/specMotors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/__init__.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
+-rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_detector_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/interfaces/protocols/bec_protocols.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/__init__.py
+-rw-r--r--   0        0        0    27788 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim.py
+-rw-r--r--   0        0        0    28125 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_data.py
+-rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_frameworks.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_signals.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_test_devices.py
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/sim_xtreme.py
+-rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/__init__.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/bec_device_base.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/bec_scaninfo_mixin.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/bec_utils.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/controller.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/dynamic_pseudo.py
+-rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/socket.py
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/ophyd_devices/utils/static_device_test.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_controller.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_dynamic_pseudo.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_ophyd_status_obj.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_simulation.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_socket.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/tests/test_static_device_test.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ophyd_devices-1.0.1/PKG-INFO
```

### Comparing `ophyd_devices-1.0.0/.gitlab-ci.yml` & `ophyd_devices-1.0.1/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is a template, and might need editing before it works on your project.
 # Official language image. Look for the different tagged releases at:
 # https://hub.docker.com/r/library/python/tags/
 image: $CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX/python:3.10
 
 variables:
   BEC_CORE_BRANCH: "main"
-  CHILD_PIPELINE_BRANCH: "main"
+  CHILD_PIPELINE_BRANCH: $CI_DEFAULT_BRANCH
   CSAXS_BEC_BRANCH: "main"
   PXIII_BEC_BRANCH: "main"
   DEBYE_BEC_BRANCH: "main"
   TOMCAT_BEC_BRANCH: "main"
   XTREME_BEC_BRANCH: "main"
 
 workflow:
@@ -34,15 +34,16 @@
       stage: test
       path: "."
       pytest_args: "-v --random-order tests/"
       exclude_packages: ""
 
 #commands to run in the Docker container before starting each job.
 before_script:
-  - if [[ "$CI_PROJECT_PATH" != "bec/ophyd_devices" ]]; then 
+  - if [[ "$CI_PROJECT_PATH" != "bec/ophyd_devices" ]]; then
+    echo -e "\033[35;1m Using branch $CHILD_PIPELINE_BRANCH of Ophyd Devices \033[0;m"; 
     test -d ophyd_devices || git clone --branch $CHILD_PIPELINE_BRANCH https://gitlab.psi.ch/bec/ophyd_devices.git; cd ophyd_devices;
     fi
   - pip install -e .[dev]
   - git clone --branch $BEC_CORE_BRANCH https://gitlab.psi.ch/bec/bec.git
   - pip install -e ./bec/bec_lib[dev]
   - pip install -e ./bec/bec_server[dev]
 
@@ -198,15 +199,17 @@
   trigger:
     strategy: depend
     include:
       - project: bec/$CHILD_PROJECT
         ref: $CHILD_PIPELINE_BRANCH
         file: /.gitlab-ci.yml
   variables:
-    BEC_CORE_BRANCH: $CI_COMMIT_REF_NAME
+    BEC_CORE_BRANCH: ${BEC_CORE_BRANCH}
+    OPHYD_DEVICES_BRANCH: $CI_COMMIT_REF_NAME
+    BEC_WIDGETS_BRANCH: ${BEC_WIDGETS_BRANCH}
     CHILD_PROJECTS: ""
   rules:
     - if: '$CI_PIPELINE_SOURCE == "web" && $CI_PROJECT_PATH == "bec/ophyd_devices"'
     - if: '$CI_MERGE_REQUEST_TARGET_BRANCH_NAME == "main" && $CI_PROJECT_PATH == "bec/ophyd_devices"'
     - if: '$CI_MERGE_REQUEST_TARGET_BRANCH_NAME == "production" && $CI_PROJECT_PATH == "bec/ophyd_devices"'
   interruptible: true
```

### Comparing `ophyd_devices-1.0.0/CHANGELOG.md` & `ophyd_devices-1.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v1.0.1 (2024-05-15)
+
+### Ci
+
+* ci: fixed bec_widgets env var ([`e900a4c`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/e900a4cb47c5ecaae8eca30d106771034dc9296d))
+
+* ci: fixed bec core dependency ([`8158e14`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/8158e145fe2358a736a2fb9d2d3de7e6c8db021c))
+
+* ci: added echo to highlight the current branch ([`68b593f`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/68b593f20d73c6463d5e97ddf7dcf94a5b036b06))
+
+### Fix
+
+* fix: bec_lib imports ([`3d8b023`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/3d8b0231a3359db9a5430e49912147c049dbfab9))
+
+
 ## v1.0.0 (2024-05-08)
 
 ### Breaking
 
 * refactor!: moved to new ophyd_devices repo structure
 
 BREAKING CHANGE: cleaned up and migrated to the new repo structure. Only shared devices will be hosted in ophyd_devices. Everything else will be in the beamline-specific repositories ([`3415ae2`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/3415ae2007cc447835906271de23e5f7a41ba373))
@@ -139,23 +154,7 @@
 
 ### Feature
 
 * feat: added support for directories as input for the static device test ([`9748ca6`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/9748ca666c3c8668e8ced80e7d24eeaf7f19c28e))
 
 
 ## v0.30.5 (2024-04-12)
-
-### Ci
-
-* ci: fixed bec install ([`a954640`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/a9546402f5b2f1a43e1c4e17f977c544c326e5dc))
-
-### Fix
-
-* fix: fixed bec_server import ([`434fa36`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/434fa36ca43f8dacd9c4f8fdd7556d77bd0a4b03))
-
-### Refactor
-
-* refactor(device_config): removed outdated config file ([`80a964f`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/80a964fae7203cbfb642980e3f89ed35ad6ff0da))
-
-* refactor(device_config): fixed device schema ([`0f3665c`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/0f3665c32fec2f0f95cc57af81d448eca6978919))
-
-* refactor(device_config): upgraded device configs; closes #56 ([`65c72c9`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/65c72c924847644f80fac768ed35e995a6999404))
```

### Comparing `ophyd_devices-1.0.0/README.md` & `ophyd_devices-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.0.1/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.0.1/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.0.1/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/.gitignore` & `ophyd_devices-1.0.1/bec/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/.gitlab-ci.yml` & `ophyd_devices-1.0.1/bec/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,37 @@
     - if: $CI_COMMIT_BRANCH && $CI_OPEN_MERGE_REQUESTS
       when: never
     - if: $CI_COMMIT_BRANCH
 
 
 include:
   - template: Security/Secret-Detection.gitlab-ci.yml
+  - project: "bec/awi_utils"
+    file: "/templates/check-packages-job.yml"
+    inputs:
+      stage: test
+      path: "bec_lib"
+      job_name: "check_dep_bec_lib"
+  - project: "bec/awi_utils"
+    file: "/templates/check-packages-job.yml"
+    inputs:
+      stage: test
+      path: "bec_server"
+      exclude_packages: "bec_lib"
+      job_name: "check_dep_bec_server"
+  - project: "bec/awi_utils"
+    file: "/templates/check-packages-job.yml"
+    inputs:
+      stage: test
+      path: "bec_ipython_client"
+      pytest_args: "-v --random-order tests/client_tests"
+      exclude_packages: "bec_lib"
+      job_name: "check_dep_ipython_client"
+
+
 
 # different stages in the pipeline
 stages:
   - Formatter
   - test # must be called test for security/secret-detection to work
   - AdditionalTests
   - End2End
```

### Comparing `ophyd_devices-1.0.0/bec/.pylintrc` & `ophyd_devices-1.0.1/bec/.pylintrc`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/.readthedocs.yaml` & `ophyd_devices-1.0.1/bec/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/CHANGELOG.md` & `ophyd_devices-1.0.1/bec/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,48 @@
 # CHANGELOG
 
 
 
+## v2.11.0 (2024-05-15)
+
+### Feature
+
+* feat: add utility function to determine instance of an object by class name ([`0ccd13c`](https://gitlab.psi.ch/bec/bec/-/commit/0ccd13cd738dc12d4a587b4c5e0d6b447d7cfc50))
+
+* feat: add utilities to lazy import a module ([`a37ae57`](https://gitlab.psi.ch/bec/bec/-/commit/a37ae577f68c154dc3da544816b7c7f0cb532c50))
+
+* feat: add &#39;Proxy&#39; to bec_lib utils ([`11a3f6d`](https://gitlab.psi.ch/bec/bec/-/commit/11a3f6daa46b3e6a82b66bd781b7590d01478b54))
+
+### Style
+
+* style: create directory to contain utils ([`549994d`](https://gitlab.psi.ch/bec/bec/-/commit/549994d0fdffcd4f5ed0948e1cd4cd4a0d0092af))
+
+
+## v2.10.4 (2024-05-14)
+
+### Build
+
+* build: fixed fakeredis version for now ([`51dfe69`](https://gitlab.psi.ch/bec/bec/-/commit/51dfe69298170eba7220fcb506d99515c46ea32a))
+
+### Ci
+
+* ci: update dependencies and add ci job to check for package versions ([`2aafb24`](https://gitlab.psi.ch/bec/bec/-/commit/2aafb249e8f0b8afa8ede0dc4ba0a811ecb2a70f))
+
+### Fix
+
+* fix: disabled script linter for now ([`5c5c18e`](https://gitlab.psi.ch/bec/bec/-/commit/5c5c18ef0eab33ebaa33d1a0daa846ea7f2f59a8))
+
+
+## v2.10.3 (2024-05-08)
+
+### Fix
+
+* fix: upgraded to ophyd_devices v1 ([`3077dbe`](https://gitlab.psi.ch/bec/bec/-/commit/3077dbe22ae50e6aae317c72022df6ea88b14cce))
+
+
 ## v2.10.2 (2024-05-08)
 
 ### Ci
 
 * ci: added ds pipeline for tomcat ([`55d210c`](https://gitlab.psi.ch/bec/bec/-/commit/55d210c7ae06ea509328510e6aec636caf009cfd))
 
 ### Fix
@@ -137,36 +174,14 @@
 
 ## v2.7.3 (2024-04-26)
 
 ### Documentation
 
 * docs: fixed bec config template ([`87d0986`](https://gitlab.psi.ch/bec/bec/-/commit/87d0986f21ba367dbb23db50c7c13f10b4007030))
 
-* docs: review docs, fix ScanModificationMessage, monitor callback and DAPRequestMessage ([`6b89240`](https://gitlab.psi.ch/bec/bec/-/commit/6b89240f46b2f892847e81963b7898649cb1c8d9))
-
 ### Fix
 
 * fix: fixed loading of plugin-based configs ([`f927735`](https://gitlab.psi.ch/bec/bec/-/commit/f927735cd4012d4e4182596dc2ac2735d5ec4697))
 
 ### Test
 
 * test(bec_lib): added test for unregistering callbacks ([`6e14de3`](https://gitlab.psi.ch/bec/bec/-/commit/6e14de35dc43b7eed3244f5fe327d79ddc1302ae))
-
-
-## v2.7.2 (2024-04-25)
-
-### Fix
-
-* fix(channel_monitor): register.start removed since connector.register do not have any .start method ([`1eaefc1`](https://gitlab.psi.ch/bec/bec/-/commit/1eaefc1c8ab08e8c4939c05912d476b08bdcc2c9))
-
-* fix(redis_connector): unregister is not killing communication ([`b31d506`](https://gitlab.psi.ch/bec/bec/-/commit/b31d506c9f7b541e0b8022aafdb8d44e0478ea3c))
-
-### Refactor
-
-* refactor: add file_writer and readme for tests ([`d8f76f5`](https://gitlab.psi.ch/bec/bec/-/commit/d8f76f505726fe12bdf572a9b5659a3c04620fde))
-
-### Unknown
-
-* Refactor(bec_lib.utils_script): Update util script for new plugin structure ([`6e36eaf`](https://gitlab.psi.ch/bec/bec/-/commit/6e36eaf3b1c7c77ba78e956613c9ac7f3d6865db))
-
-
-## v2.7.1 (2024-04-23)
```

### Comparing `ophyd_devices-1.0.0/bec/LICENSE` & `ophyd_devices-1.0.1/bec/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/README.md` & `ophyd_devices-1.0.1/bec/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.0.1/bec/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.0.1/bec/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.0.1/bec/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/demo.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/pyproject.toml` & `ophyd_devices-1.0.1/bec/bec_ipython_client/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_ipython_client"
-version = "2.10.2"
+version = "2.11.0"
 description = "BEC IPython client"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
@@ -21,15 +21,15 @@
     "rich~=13.7",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black~=24.0",
     "coverage~=7.0",
-    "isort~=5.0",
+    "isort~=5.13, >=5.13.2",
     "pylint~=3.0",
     "pytest-bec-e2e",
     "pytest-random-order~=1.1",
     "pytest-redis~=3.0",
     "pytest-retry~=1.1",
     "pytest-timeout~=2.2",
     "pytest~=8.0",
```

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/main.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/signals.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/scan_progress.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml` & `ophyd_devices-1.0.1/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_bec_client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_move_callback.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/client_tests/test_scan_progress.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/client_tests/test_scan_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py` & `ophyd_devices-1.0.1/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/README.md` & `ophyd_devices-1.0.1/bec/bec_lib/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/pyproject.toml` & `ophyd_devices-1.0.1/bec/bec_lib/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_lib"
-version = "2.10.2"
+version = "2.11.0"
 description = "BEC library"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "fastjsonschema~=2.19",
-    "fpdf2~=2.7",
+    "fpdf2~=2.7, >=2.7.7",
     "hiredis~=2.3",
     "lmfit~=1.3",
     "loguru~=0.7",
     "louie~=2.0",
     "msgpack~=1.0",
     "numpy~=1.24",
     "psutil~=5.9",
@@ -26,24 +26,25 @@
     "pylint~=3.0",
     "pyyaml~=6.0",
     "redis~=5.0",
     "requests~=2.31",
     "rich~=13.7",
     "scipy~=1.12",
     "toolz~=0.12",
-    "typeguard~=4.1",
+    "typeguard ~= 4.1, >=4.1.4",
 ]
 
 
+
 [project.optional-dependencies]
 dev = [
     "black~=24.0",
     "coverage~=7.0",
-    "fakeredis",
-    "isort~=5.0",
+    "fakeredis~=2.21, <2.23",
+    "isort~=5.13, >=5.13.2",
     "pandas~=2.0",
     "pytest~=8.0",
     "pytest-random-order~=1.1",
     "pytest-timeout~=2.2",
     "pytest-redis~=3.0",
 ]
```

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/__init__.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/alarm_handler.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/async_data.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bec_service.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bec_yaml_loader.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bec_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bl_checks.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/bl_conditions.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/callback_handler.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/channel_monitor.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/client.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/config_helper.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/connector.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/dap_plugin_objects.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/dap_plugins.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/device.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/devicemanager.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/endpoints.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/file_utils.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/lmfit_serializer.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/logbook_connector.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/logger.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/messages.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/numpy_encoder.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/observer.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/pdf_writer.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/plugin_helper.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/queue_items.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/redis_connector.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/request_items.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_data.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_items.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_manager.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scan_report.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scans.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/scibec_validator.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/serialization.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/service_config.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/signature_serializer.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/user_scripts_mixin.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/user_scripts_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,16 @@
 
     def load_user_script(self, file: str) -> None:
         """load a user script file and import all its definitions
 
         Args:
             file (str): Full path to the script file.
         """
-        self._run_linter_on_file(file)
+        # TODO: re-enable linter
+        # self._run_linter_on_file(file)
         module_members = self._load_script_module(file)
         for name, cls in module_members:
             if not callable(cls):
                 continue
             # ignore imported classes
             if cls.__module__ != "scripts":
                 continue
```

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/utils.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/utils/scan_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,25 @@
 """
-Utility functions for the bec_lib package.
+Scan-related utils
 """
 
 from __future__ import annotations
 
 import csv
 import datetime
-import functools
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 from typeguard import typechecked
 
 if TYPE_CHECKING:
     from bec_lib.scan_items import ScanItem
     from bec_lib.scan_report import ScanReport
 
 
-class user_access:
-
-    def __init__(self, meth):
-        """
-        Decorator to mark <device_class> methods to be accessible from the bec client
-
-        Args:
-            meth: method to be marked as accessible
-
-        Examples:
-            >>> @user_access
-            >>> def my_method(self, *args, **kwargs):
-            >>>     return fcn(self, *args, **kwargs)
-
-        """
-        self.meth = meth
-
-    def __set_name__(self, owner, name):
-        """Write registered method into the owner class USER_ACCESS list for the bec_ipython_client"""
-        if not hasattr(owner, "USER_ACCESS"):
-            owner.USER_ACCESS = []
-        if name not in owner.USER_ACCESS:
-            owner.USER_ACCESS.append(name)
-
-        setattr(owner, name, self.meth)
-
-
-def threadlocked(fcn):
-    """Ensure that the thread acquires and releases the lock."""
-
-    @functools.wraps(fcn)
-    def wrapper(self, *args, **kwargs):
-        # pylint: disable=protected-access
-        with self._lock:
-            return fcn(self, *args, **kwargs)
-
-    return wrapper
-
-
 @typechecked
 def scan_to_csv(
     scan_report: ScanReport | ScanItem | list[ScanReport] | list[ScanItem],
     output_name: str,
     delimiter: str = ",",
     dialect: str | None = None,
     header: list | None = None,
```

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/configs/demo_config.yaml` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/configs/openapi_schema.json` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/fixtures.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/test_config.yaml` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/bec_lib/tests/utils.py` & `ophyd_devices-1.0.1/bec/bec_lib/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_async_data.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_beamline_checks.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_bec_logger.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_bec_messages.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_bec_service.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bec_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,10 +141,13 @@
     with bec_service(
         f"{os.path.dirname(bec_lib.__file__)}/tests/test_service_config.yaml", unique_service=True
     ) as service:
         assert service._service_config.service_config["file_writer"]["base_path"] == "./"
 
     config = ServiceConfig(redis={"host": "localhost", "port": 6379})
     with bec_service(config=config, unique_service=True) as service:
-        assert os.path.abspath(
-            service._service_config.service_config["file_writer"]["base_path"]
-        ) == str(Path(bec_lib.service_config.__file__).resolve().parent.parent.parent)
+        bec_lib_path = str(Path(bec_lib.service_config.__file__).resolve().parent.parent.parent)
+        if "nox" not in bec_lib_path:
+            assert (
+                os.path.abspath(service._service_config.service_config["file_writer"]["base_path"])
+                == bec_lib_path
+            )
```

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_bl_conditions.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_callback_handler.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_channel_monitor.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_config_helper.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_core_utils.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_core_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import pytest
 
 from bec_lib import messages
 from bec_lib.scan_data import ScanData
 from bec_lib.scan_items import ScanItem
 from bec_lib.scan_report import ScanReport
-from bec_lib.utils import _extract_scan_data, _write_csv, scan_to_csv, scan_to_dict, user_access
+from bec_lib.utils.rpc_utils import user_access
+from bec_lib.utils.scan_utils import _extract_scan_data, _write_csv, scan_to_csv, scan_to_dict
 
 
 class ScanReportMock(ScanReport):
     def __init__(self, scan_id: str) -> None:
         super().__init__()
         self.request = mock.MagicMock()
         self.request.scan.scan_id = scan_id
```

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_dap_plugins.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_device_manager.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_devices.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_file_utils.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_lmfit_serializer.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_observer.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_plugin_helper.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_redis_connector.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_redis_connector_fakeredis.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_context.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_data.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_items.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_manager.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_object.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_object.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_scan_report.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_serializer.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_signature_serializer.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_user_scripts_mixin.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_user_scripts_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             assert load_script.call_args == mock.call("dummy")
             assert "test" in scripts._scripts
             assert mock_run.call_count == 1
             assert mock_run.call_args == mock.call(
                 EventType.NAMESPACE_UPDATE, action="add", ns_objects={"test": dummy_func}
             )
             assert "wrong_test" not in scripts._scripts
-        linter.assert_called_once_with("dummy")
+        # linter.assert_called_once_with("dummy") #TODO: re-enable this test once issue #298 is fixed
 
 
 # def test_user_script_linter():
 #     scripts = UserScriptsMixin()
 #     current_path = pathlib.Path(__file__).parent.resolve()
 #     script_path = os.path.join(current_path, "test_data", "user_script_with_bug.py")
 #     builtins.__dict__["dev"] = scripts
```

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/tests/test_yaml_loader.py` & `ophyd_devices-1.0.1/bec/bec_lib/tests/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/create_plugin_structure.py` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/create_plugin_structure.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/init_config.py` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py` & `ophyd_devices-1.0.1/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/pyproject.toml` & `ophyd_devices-1.0.1/bec/bec_server/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.10.2"
+version = "2.11.0"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
@@ -16,27 +16,27 @@
     "bec-lib",
     "h5py~=3.10",
     "libtmux~=0.37",
     "lmfit~=1.3",
     "msgpack~=1.0",
     "numpy~=1.24",
     "ophyd~=1.9",
-    "ophyd_devices~=0.33",
+    "ophyd_devices~=1.0",
     "pydantic~=2.0",
     "py-scibec~=1.14",
     "pyyaml~=6.0",
     "python-dotenv~=1.0",
     "rich~=13.7",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black~=24.0",
     "coverage~=7.0",
-    "isort~=5.0",
+    "isort~=5.13, >=5.13.2",
     "pylint~=3.0",
     "pytest~=8.0",
     "pytest-random-order~=1.1",
     "pytest-timeout~=2.2",
 ]
 
 [project.scripts]
```

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/dap_server.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/dap_service.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/data_processing/cli/launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/device_server.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/rpc_mixin.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/cli/launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/device_server/tests/utils.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/default_writer.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/file_writer.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/merged_dicts.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer/cli/launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/emitter.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/device_validation.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/path_optimization.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_assembler.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_guard.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_manager.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_queue.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_server.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_stubs.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_worker.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scans.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/cli/launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scan_server/tests/utils.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scan_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/repeated_timer.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scihub.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/cli/launch.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/bec_server/scihub/scilog/scilog.py` & `ophyd_devices-1.0.1/bec/bec_server/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/conftest.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_config_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_server.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/conftest.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scan_server/test_scans.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scan_server/test_scans.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/conftest.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py` & `ophyd_devices-1.0.1/bec/bec_server/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/bin/install_bec_dev.sh` & `ophyd_devices-1.0.1/bec/bin/install_bec_dev.sh`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/ci/Dockerfile.run_pytest` & `ophyd_devices-1.0.1/bec/ci/Dockerfile.run_pytest`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/ci/Dockerfile.run_server` & `ophyd_devices-1.0.1/bec/ci/Dockerfile.run_server`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/ci/docker-compose.yaml` & `ophyd_devices-1.0.1/bec/ci/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/ci/semantic_release.toml` & `ophyd_devices-1.0.1/bec/ci/semantic_release.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/architecture/BEC.drawio` & `ophyd_devices-1.0.1/bec/docs/architecture/BEC.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/architecture/BEC_config_db.drawio` & `ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/architecture/BEC_config_db.svg` & `ophyd_devices-1.0.1/bec/docs/architecture/BEC_config_db.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/architecture/bec_architecture.png` & `ophyd_devices-1.0.1/bec/docs/architecture/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/Makefile` & `ophyd_devices-1.0.1/bec/docs/source/Makefile`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/conf.py` & `ophyd_devices-1.0.1/bec/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/make.bat` & `ophyd_devices-1.0.1/bec/docs/source/make.bat`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/_static/bec.png` & `ophyd_devices-1.0.1/bec/docs/source/_static/bec.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/_static/css/custom.css` & `ophyd_devices-1.0.1/bec/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/_static/gif/bec_plotter.gif` & `ophyd_devices-1.0.1/bec/docs/source/_static/gif/bec_plotter.gif`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/_templates/custom-class-template.rst` & `ophyd_devices-1.0.1/bec/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/_templates/custom-module-template.rst` & `ophyd_devices-1.0.1/bec/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/BEC_context_user_centric.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/BEC_context_user_centric.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/bec_architecture.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/bec_device_structure.drawio` & `ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/bec_device_structure.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/bec_device_structure.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/gauss_scatter_plot.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/gauss_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/simulation_context_diagram.drawio` & `ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/simulation_context_diagram.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/simulation_context_diagram.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/tab-complete-devices.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/tab-complete-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/vscode_debug_button.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/vscode_debug_button.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/vscode_with_annotations.drawio` & `ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/vscode_with_annotations.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/vscode_with_annotations.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/assets/wm-devices.png` & `ophyd_devices-1.0.1/bec/docs/source/assets/wm-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/architecture.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/architecture.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/bec_plugins.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/bec_plugins.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/bec_sim.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/bec_sim.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/contributing.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/contributing.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/developer.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/developer.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/external_sources.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/external_sources.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/glossary.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/glossary.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/install_developer_env.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/install_developer_env.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/logs.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/logs.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/ophyd.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/ophyd.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/tests.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/developer/vscode.md` & `ophyd_devices-1.0.1/bec/docs/source/developer/vscode.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/introduction/introduction.md` & `ophyd_devices-1.0.1/bec/docs/source/introduction/introduction.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/user/command_line_interface.md` & `ophyd_devices-1.0.1/bec/docs/source/user/command_line_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/user/data_access_and_plotting.md` & `ophyd_devices-1.0.1/bec/docs/source/user/data_access_and_plotting.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/user/devices.md` & `ophyd_devices-1.0.1/bec/docs/source/user/devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/user/graphical_user_interface.md` & `ophyd_devices-1.0.1/bec/docs/source/user/graphical_user_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/user/installation.md` & `ophyd_devices-1.0.1/bec/docs/source/user/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/docs/source/user/user.md` & `ophyd_devices-1.0.1/bec/docs/source/user/user.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/bec/pytest_bec_e2e/pyproject.toml` & `ophyd_devices-1.0.1/bec/pytest_bec_e2e/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytest-bec-e2e"
-version = "2.10.2"
+version = "2.11.0"
 description = "BEC pytest plugin for end-to-end tests"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.0.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py` & `ophyd_devices-1.0.1/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/__init__.py` & `ophyd_devices-1.0.1/ophyd_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/ophyd_patch.py` & `ophyd_devices-1.0.1/ophyd_devices/ophyd_patch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/configs/ophyd_devices_simulation.yaml` & `ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_devices_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/configs/ophyd_simulation.yaml` & `ophyd_devices-1.0.1/ophyd_devices/configs/ophyd_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/SpmBase.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/XbpmBase.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/XbpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/__init__.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/epics_motor_ex.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/epics_motor_ex.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/mono_dccm.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/mono_dccm.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/slits.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/slits.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/slsDetector.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/slsDetector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/sls_devices.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/sls_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/devices/specMotors.py` & `ophyd_devices-1.0.1/ophyd_devices/devices/specMotors.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py` & `ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py` & `ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py` & `ophyd_devices-1.0.1/ophyd_devices/interfaces/base_classes/psi_detector_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/interfaces/protocols/bec_protocols.py` & `ophyd_devices-1.0.1/ophyd_devices/interfaces/protocols/bec_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/sim.py` & `ophyd_devices-1.0.1/ophyd_devices/sim/sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import threading
 import time as ttime
 
 import numpy as np
-from bec_lib import MessageEndpoints, bec_logger, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
+from bec_lib.logger import bec_logger
 from ophyd import Component as Cpt
 from ophyd import Device, DeviceStatus
 from ophyd import DynamicDeviceComponent as Dcpt
 from ophyd import Kind, PositionerBase
 from ophyd.flyers import FlyerInterface
 from ophyd.sim import SynSignal
 from ophyd.status import StatusBase
```

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/sim_data.py` & `ophyd_devices-1.0.1/ophyd_devices/sim/sim_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/sim_frameworks.py` & `ophyd_devices-1.0.1/ophyd_devices/sim/sim_frameworks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/sim_signals.py` & `ophyd_devices-1.0.1/ophyd_devices/sim/sim_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/sim_test_devices.py` & `ophyd_devices-1.0.1/ophyd_devices/sim/sim_test_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import threading
 import time as ttime
 
 import numpy as np
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from ophyd import Device, OphydObject, PositionerBase
 
 
 class DummyControllerDevice(Device):
     USER_ACCESS = ["controller"]
```

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-1.0.1/ophyd_devices/sim/sim_xtreme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import threading
 import time
 
 import numpy as np
-from bec_lib import MessageEndpoints, messages
+from bec_lib import messages
+from bec_lib.endpoints import MessageEndpoints
 from ophyd import Component as Cpt
 from ophyd import Device, Kind, Signal
 from ophyd.flyers import FlyerInterface
 from ophyd.ophydobj import Kind
 from ophyd.status import DeviceStatus, SubscriptionStatus
 from ophyd.utils import ReadOnlyError
```

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.0.1/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/tests/utils.py` & `ophyd_devices-1.0.1/ophyd_devices/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/utils/bec_device_base.py` & `ophyd_devices-1.0.1/ophyd_devices/utils/bec_device_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/utils/bec_scaninfo_mixin.py` & `ophyd_devices-1.0.1/ophyd_devices/utils/bec_scaninfo_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import getpass
 
-from bec_lib import DeviceManagerBase, MessageEndpoints, bec_logger, messages
+from bec_lib import bec_logger, messages
+from bec_lib.devicemanager import DeviceManagerBase
+from bec_lib.endpoints import MessageEndpoints
 
 logger = bec_logger.logger
 
 
 class BECInfoMsgMock:
     """Mock BECInfoMsg class
```

### Comparing `ophyd_devices-1.0.0/ophyd_devices/utils/bec_utils.py` & `ophyd_devices-1.0.1/ophyd_devices/utils/bec_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/utils/controller.py` & `ophyd_devices-1.0.1/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/utils/dynamic_pseudo.py` & `ophyd_devices-1.0.1/ophyd_devices/utils/dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/utils/socket.py` & `ophyd_devices-1.0.1/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/ophyd_devices/utils/static_device_test.py` & `ophyd_devices-1.0.1/ophyd_devices/utils/static_device_test.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/tests/test_controller.py` & `ophyd_devices-1.0.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/tests/test_dynamic_pseudo.py` & `ophyd_devices-1.0.1/tests/test_dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/tests/test_ophyd_status_obj.py` & `ophyd_devices-1.0.1/tests/test_ophyd_status_obj.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/tests/test_simulation.py` & `ophyd_devices-1.0.1/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/tests/test_socket.py` & `ophyd_devices-1.0.1/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/.gitignore` & `ophyd_devices-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/LICENSE` & `ophyd_devices-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.0.0/pyproject.toml` & `ophyd_devices-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ophyd_devices"
-version = "1.0.0"
+version = "1.0.1"
 description = "Custom device implementations based on the ophyd hardware abstraction layer"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.0.0/PKG-INFO` & `ophyd_devices-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ophyd_devices
-Version: 1.0.0
+Version: 1.0.1
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/ophyd_devices
 Project-URL: documentation, https://bec.readthedocs.org
 Project-URL: changelog, https://gitlab.psi.ch/bec/ophyd_devices/blob/main/CHANGELOG.md
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

