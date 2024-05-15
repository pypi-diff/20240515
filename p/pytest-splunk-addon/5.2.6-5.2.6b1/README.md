# Comparing `tmp/pytest_splunk_addon-5.2.6.tar.gz` & `tmp/pytest_splunk_addon-5.2.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon-5.2.6.tar", max compression
+gzip compressed data, was "pytest_splunk_addon-5.2.6b1.tar", max compression
```

## Comparing `pytest_splunk_addon-5.2.6.tar` & `pytest_splunk_addon-5.2.6b1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0    11341 2024-05-15 08:53:50.578272 pytest_splunk_addon-5.2.6/LICENSE
--rw-r--r--   0        0        0     2153 2024-05-15 08:54:24.278028 pytest_splunk_addon-5.2.6/pyproject.toml
--rw-r--r--   0        0        0     1886 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/.ignore_splunk_internal_errors
--rw-r--r--   0        0        0      744 2024-05-15 08:54:24.274028 pytest_splunk_addon-5.2.6/pytest_splunk_addon/__init__.py
--rw-r--r--   0        0        0     5364 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/docker_class.py
--rw-r--r--   0        0        0     8543 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/plugin.py
--rw-r--r--   0        0        0    34181 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/splunk.py
--rw-r--r--   0        0        0      579 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
--rw-r--r--   0        0        0    46781 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
--rw-r--r--   0        0        0     1220 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/__init__.py
--rw-r--r--   0        0        0     2791 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_basic.py
--rw-r--r--   0        0        0     3312 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
--rw-r--r--   0        0        0     2082 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
--rw-r--r--   0        0        0     3136 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/fields.py
--rw-r--r--   0        0        0    13284 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
--rw-r--r--   0        0        0     2760 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
--rw-r--r--   0        0        0     2447 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
--rw-r--r--   0        0        0     5391 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
--rw-r--r--   0        0        0     6168 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/app_test_generator.py
--rw-r--r--   0        0        0      754 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
--rw-r--r--   0        0        0     1130 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
--rw-r--r--   0        0        0     9586 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
--rw-r--r--   0        0        0     2351 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
--rw-r--r--   0        0        0     2801 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
--rw-r--r--   0        0        0     2442 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
--rw-r--r--   0        0        0     3553 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
--rw-r--r--   0        0        0     3699 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
--rw-r--r--   0        0        0      970 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
--rw-r--r--   0        0        0     2024 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
--rw-r--r--   0        0        0     2386 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
--rw-r--r--   0        0        0     3937 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
--rw-r--r--   0        0        0     3267 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
--rw-r--r--   0        0        0     4226 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
--rw-r--r--   0        0        0     9218 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
--rw-r--r--   0        0        0     2965 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
--rw-r--r--   0        0        0    11204 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
--rw-r--r--   0        0        0    20768 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
--rw-r--r--   0        0        0     2390 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Alerts.json
--rw-r--r--   0        0        0     5281 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Authentication.json
--rw-r--r--   0        0        0     9626 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Certificates.json
--rw-r--r--   0        0        0     8173 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Change.json
--rw-r--r--   0        0        0     2814 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/DLP.json
--rw-r--r--   0        0        0     8598 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Email.json
--rw-r--r--   0        0        0    18855 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
--rw-r--r--   0        0        0     9890 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
--rw-r--r--   0        0        0     4255 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Malware.json
--rw-r--r--   0        0        0     7098 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
--rw-r--r--   0        0        0     5599 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
--rw-r--r--   0        0        0    18953 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
--rw-r--r--   0        0        0     3862 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Updates.json
--rw-r--r--   0        0        0     5184 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
--rw-r--r--   0        0        0     7178 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Web.json
--rw-r--r--   0        0        0      889 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
--rw-r--r--   0        0        0      862 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
--rw-r--r--   0        0        0     7339 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
--rw-r--r--   0        0        0     5002 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
--rw-r--r--   0        0        0     4418 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
--rw-r--r--   0        0        0     4995 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
--rw-r--r--   0        0        0     3615 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
--rw-r--r--   0        0        0     3015 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
--rw-r--r--   0        0        0      812 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
--rw-r--r--   0        0        0     5420 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
--rw-r--r--   0        0        0    11040 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
--rw-r--r--   0        0        0    10360 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
--rw-r--r--   0        0        0    21984 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
--rw-r--r--   0        0        0      766 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/__init__.py
--rw-r--r--   0        0        0      711 2024-05-15 08:53:50.582272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
--rw-r--r--   0        0        0    11987 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
--rw-r--r--   0        0        0    11457 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
--rw-r--r--   0        0        0      909 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
--rw-r--r--   0        0        0     7291 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
--rw-r--r--   0        0        0    46400 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/rule.py
--rw-r--r--   0        0        0    15413 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
--rw-r--r--   0        0        0     2290 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
--rw-r--r--   0        0        0    16792 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
--rw-r--r--   0        0        0     6032 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
--rw-r--r--   0        0        0     9990 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
--rw-r--r--   0        0        0     6217 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
--rw-r--r--   0        0        0      834 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/__init__.py
--rw-r--r--   0        0        0     4634 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
--rw-r--r--   0        0        0     1627 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/log_helper.py
--rw-r--r--   0        0        0     3034 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
--rw-r--r--   0        0        0     3414 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
--rw-r--r--   0        0        0    17585 2024-05-15 08:53:50.586272 pytest_splunk_addon-5.2.6/pytest_splunk_addon/tools/cim_field_report.py
--rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-04-19 15:14:44.549955 pytest_splunk_addon-5.2.6b1/LICENSE
+-rw-r--r--   0        0        0     2322 2024-04-19 15:15:27.394245 pytest_splunk_addon-5.2.6b1/pyproject.toml
+-rw-r--r--   0        0        0     1886 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/.ignore_splunk_internal_errors
+-rw-r--r--   0        0        0      751 2024-04-19 15:15:27.394245 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/__init__.py
+-rw-r--r--   0        0        0     5364 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/docker_class.py
+-rw-r--r--   0        0        0     8543 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/plugin.py
+-rw-r--r--   0        0        0    34048 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/splunk.py
+-rw-r--r--   0        0        0      579 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
+-rw-r--r--   0        0        0    46781 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
+-rw-r--r--   0        0        0     1220 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/__init__.py
+-rw-r--r--   0        0        0     2791 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_basic.py
+-rw-r--r--   0        0        0     3312 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
+-rw-r--r--   0        0        0     2082 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
+-rw-r--r--   0        0        0     3136 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py
+-rw-r--r--   0        0        0    13284 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
+-rw-r--r--   0        0        0     2760 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
+-rw-r--r--   0        0        0     2447 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
+-rw-r--r--   0        0        0     5391 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
+-rw-r--r--   0        0        0     6168 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/app_test_generator.py
+-rw-r--r--   0        0        0      754 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
+-rw-r--r--   0        0        0     1130 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
+-rw-r--r--   0        0        0     9586 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
+-rw-r--r--   0        0        0     2351 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
+-rw-r--r--   0        0        0     2801 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
+-rw-r--r--   0        0        0     2442 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
+-rw-r--r--   0        0        0     3553 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
+-rw-r--r--   0        0        0     3699 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
+-rw-r--r--   0        0        0      970 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
+-rw-r--r--   0        0        0     2386 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
+-rw-r--r--   0        0        0     3937 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
+-rw-r--r--   0        0        0     3267 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
+-rw-r--r--   0        0        0     4226 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
+-rw-r--r--   0        0        0     9218 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
+-rw-r--r--   0        0        0     2965 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
+-rw-r--r--   0        0        0    11204 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
+-rw-r--r--   0        0        0    20768 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
+-rw-r--r--   0        0        0     2390 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json
+-rw-r--r--   0        0        0     5281 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json
+-rw-r--r--   0        0        0     9626 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json
+-rw-r--r--   0        0        0     8173 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Change.json
+-rw-r--r--   0        0        0     2814 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/DLP.json
+-rw-r--r--   0        0        0     8598 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Email.json
+-rw-r--r--   0        0        0    18855 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
+-rw-r--r--   0        0        0     9400 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
+-rw-r--r--   0        0        0     4255 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Malware.json
+-rw-r--r--   0        0        0     6608 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
+-rw-r--r--   0        0        0     5599 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
+-rw-r--r--   0        0        0    17483 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
+-rw-r--r--   0        0        0     3862 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Updates.json
+-rw-r--r--   0        0        0     5184 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
+-rw-r--r--   0        0        0     7178 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Web.json
+-rw-r--r--   0        0        0      889 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
+-rw-r--r--   0        0        0     7339 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
+-rw-r--r--   0        0        0     5002 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
+-rw-r--r--   0        0        0     4418 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
+-rw-r--r--   0        0        0     4995 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
+-rw-r--r--   0        0        0     3615 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
+-rw-r--r--   0        0        0     3015 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
+-rw-r--r--   0        0        0      812 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
+-rw-r--r--   0        0        0     5420 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
+-rw-r--r--   0        0        0    11040 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
+-rw-r--r--   0        0        0    10360 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
+-rw-r--r--   0        0        0    21984 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
+-rw-r--r--   0        0        0      766 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py
+-rw-r--r--   0        0        0      711 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
+-rw-r--r--   0        0        0    11987 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
+-rw-r--r--   0        0        0    11457 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
+-rw-r--r--   0        0        0      909 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
+-rw-r--r--   0        0        0     7291 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
+-rw-r--r--   0        0        0    46400 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py
+-rw-r--r--   0        0        0    15413 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
+-rw-r--r--   0        0        0     2290 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
+-rw-r--r--   0        0        0    16792 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
+-rw-r--r--   0        0        0     6032 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
+-rw-r--r--   0        0        0     9990 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
+-rw-r--r--   0        0        0     6217 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
+-rw-r--r--   0        0        0      834 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/__init__.py
+-rw-r--r--   0        0        0     4634 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
+-rw-r--r--   0        0        0     1627 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py
+-rw-r--r--   0        0        0     3034 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
+-rw-r--r--   0        0        0     3414 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
+-rw-r--r--   0        0        0    17585 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/tools/cim_field_report.py
+-rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.2.6b1/PKG-INFO
```

### Comparing `pytest_splunk_addon-5.2.6/LICENSE` & `pytest_splunk_addon-5.2.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pyproject.toml` & `pytest_splunk_addon-5.2.6b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "pytest-splunk-addon"
-version = "5.2.6"
+version = "5.2.6-beta.1"
 description = "A Dynamic test tool for Splunk Apps and Add-ons"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "APACHE-2.0"
 classifiers = [
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
@@ -32,32 +32,41 @@
 include = ["pytest_splunk_addon/**/*.json", "pytest_splunk_addon/**/*.txt"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pytest = ">5.4.0,<8"
 splunk-sdk = ">=1.6"
 requests = "^2.31.0"
-jsonschema = "^v4.17.3"
-pytest-xdist = "^3.5.0"
+jsonschema = ">=4,<5"
+pytest-xdist = ">=2.3.0"
 filelock = "^3.0"
 pytest-ordering = "~0.6"
 junitparser = "^2.2.0"
 addonfactory-splunk-conf-parser-lib = "*"
 defusedxml = "^0.7.1"
-Faker = "^18.0.0"
+Faker = ">=13.12,<19.0.0"
 xmltodict = "^0.13.0"
-xmlschema = "^2.5.1"
+xmlschema = "^1.11.3"
 splunksplwrapper = "^1.1.1"
 urllib3 = "<2"
 
+
 [tool.poetry.group.dev.dependencies]
-pytest-cov = "^4"
+pytest-cov = "^3.0.0"
 requests-mock = "^1.8.0"
-freezegun = "^1.5.1"
-pytz = "^2024.1"
+freezegun = "^1.2.1"
+pytz = "^2022.1"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+jinja2 = "3.1.3"
+sphinx-rtd-theme = "1.1.1"
+sphinx-panels = "0.6.0"
 
 [tool.poetry.plugins]
 pytest11 = { plugin = "pytest_splunk_addon.plugin", "splunk" = "pytest_splunk_addon.splunk" }
 
 [tool.poetry.scripts]
 cim-report = 'pytest_splunk_addon.standard_lib.utilities.junit_parser:main'
 cim-field-report = 'pytest_splunk_addon.tools.cim_field_report:main'
```

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/.ignore_splunk_internal_errors` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/.ignore_splunk_internal_errors`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # limitations under the License.
 #
 # -*- coding: utf-8 -*-
 """Top-level package for splunk-app-test-lib."""
 
 __author__ = """Splunk Inc."""
 __email__ = "addonfactory@splunk.com"
-__version__ = "5.2.6"
+__version__ = "5.2.6-beta.1"
```

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/docker_class.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/docker_class.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/plugin.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/splunk.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/splunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1015,9 +1015,7 @@
 
 def pytest_unconfigure(config):
     if PYTEST_XDIST_TESTRUNUID:
         if os.path.exists(PYTEST_XDIST_TESTRUNUID + "_wait"):
             os.remove(PYTEST_XDIST_TESTRUNUID + "_wait")
         if os.path.exists(PYTEST_XDIST_TESTRUNUID + "_events"):
             os.remove(PYTEST_XDIST_TESTRUNUID + "_events")
-        if os.path.exists(PYTEST_XDIST_TESTRUNUID + "_events.lock"):
-            os.remove(PYTEST_XDIST_TESTRUNUID + "_events.lock")
```

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_basic.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/fields.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/app_test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/app_test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/data_model.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/data_set.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Alerts.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Authentication.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Certificates.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Change.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Change.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/DLP.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/DLP.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Email.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Email.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Endpoint.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998263888888889%*

 * *Differences: {"'objects'": '{0: {\'fields\': {2: {\'validity\': \'case(in(upper(transport), "HOPOPT", "ICMP", '*

 * *              '"IGMP", "GGP", "IP-IN-IP", "ST", "TCP", "CBT", "EGP", "IGP", "BBN-RCC-MON", '*

 * *              '"NVP-II", "PUP", "ARGUS", "EMCON", "XNET", "CHAOS", "UDP", "MUX", "DCN-MEAS", '*

 * *              '"HMP", "PRM", "XNS-ID", "TRUNK-1", "TRUNK-2", "LEAF-1", "LEAF-2", "RDP", "IRTP", '*

 * *              '"ISO-TP4", "NETBLT", "MFE-NSP", "MERIT-INP", "DCCP", "3CP", "IDPR", "XTP", "DDP", '*

 * *              '"IDPR-CMTP",  […]*

```diff
@@ -59,15 +59,15 @@
                     "type": "required"
                 },
                 {
                     "comment": "The destination of the attack detected by the intrusion detection system (IDS). You can alias this from more specific fields not included in this data model, such as dest_host, dest_ip, or dest_name.",
                     "condition": "ids_type=\"network\"",
                     "name": "dest",
                     "type": "conditional",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
                 },
                 {
                     "comment": "The device that detected the intrusion event. You can alias this from more specific fields not included in this data model, such as dvc_host, dvc_ip, or dvc_name.",
                     "name": "dvc",
                     "type": "required"
                 },
                 {
@@ -115,15 +115,15 @@
                     "type": "required"
                 },
                 {
                     "comment": "The source involved in the attack detected by the IDS. You can alias this from more specific fields not included in this data model, such as src_host, src_ip, or src_name.",
                     "condition": "ids_type=\"network\"",
                     "name": "src",
                     "type": "conditional",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
                 },
                 {
                     "comment": "The OSI layer 4 (transport) protocol of the intrusion, in lower case.",
                     "condition": "ids_type=\"network\"",
                     "name": "transport",
                     "type": "conditional"
                 },
```

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Malware.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Malware.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998263888888889%*

 * *Differences: {"'objects'": '{0: {\'fields\': {4: {\'validity\': \'case(in(upper(transport), "TCP", "UDP"), '*

 * *              'if(match(dest,"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\\\.|$)){4}"), '*

 * *              'dest, null()), match(dest,"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$"), dest, '*

 * *              'true(), null())\'}, 13: {\'validity\': \'case(in(upper(transport), "TCP", "UDP"), '*

 * *              'if(match(src,"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0 […]*

```diff
@@ -28,15 +28,15 @@
                     "type": "required",
                     "validity": "if(isnum(authority_answer_count),authority_answer_count,null())"
                 },
                 {
                     "comment": "The destination of the network resolution event. You can alias this from more specific fields, such as dest_host, dest_ip, or dest_name.",
                     "name": "dest",
                     "type": "required",
-                    "validity": "case(in(upper(transport), \"TCP\", \"UDP\"), if(match(dest,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
+                    "validity": "case(in(upper(transport), \"TCP\", \"UDP\"), if(match(dest,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
                 },
                 {
                     "comment": "Type of DNS message.",
                     "expected_values": [
                         "Query",
                         "Response"
                     ],
@@ -141,15 +141,15 @@
                     "type": "required",
                     "validity": "if(isnum(response_time),response_time,null())"
                 },
                 {
                     "comment": "The source of the network resolution event. You can alias this from more specific fields, such as src_host, src_ip, or src_name.",
                     "name": "src",
                     "type": "required",
-                    "validity": "case(in(upper(transport), \"TCP\", \"UDP\"), if(match(src,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
+                    "validity": "case(in(upper(transport), \"TCP\", \"UDP\"), if(match(src,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
                 },
                 {
                     "comment": "The unique numerical transaction id of the network resolution event",
                     "name": "transaction_id",
                     "type": "required",
                     "validity": "if(isnum(transaction_id),transaction_id,null())"
                 },
```

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998374704491727%*

 * *Differences: {"'objects'": '{0: {\'fields\': {6: {\'validity\': \'case(in(upper(transport), "HOPOPT", "ICMP", '*

 * *              '"IGMP", "GGP", "IP-IN-IP", "ST", "TCP", "CBT", "EGP", "IGP", "BBN-RCC-MON", '*

 * *              '"NVP-II", "PUP", "ARGUS", "EMCON", "XNET", "CHAOS", "UDP", "MUX", "DCN-MEAS", '*

 * *              '"HMP", "PRM", "XNS-ID", "TRUNK-1", "TRUNK-2", "LEAF-1", "LEAF-2", "RDP", "IRTP", '*

 * *              '"ISO-TP4", "NETBLT", "MFE-NSP", "MERIT-INP", "DCCP", "3CP", "IDPR", "XTP", "DDP", '*

 * *              '"IDPR-CMTP",  […]*

```diff
@@ -86,27 +86,27 @@
                     "name": "channel",
                     "type": "not_allowed_in_search"
                 },
                 {
                     "comment": "The destination of the network traffic (the remote host). You can alias this from more specific fields, such as dest_host, dest_ip, or dest_name.",
                     "name": "dest",
                     "type": "required",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
                 },
                 {
                     "comment": "The interface that is listening remotely or receiving packets locally. Can also be referred to as the 'egress interface.'",
                     "name": "dest_interface",
                     "type": "optional"
                 },
                 {
                     "comment": "The IP address of the destination.",
                     "condition": "dest_ip=*",
                     "name": "dest_ip",
                     "type": "conditional",
-                    "validity": "if(match(dest_ip, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"),dest_ip,null())"
+                    "validity": "if(match(dest_ip, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"),dest_ip,null())"
                 },
                 {
                     "comment": "The destination TCP/IP layer 2 Media Access Control (MAC) address of a packet's destination, such as 06:10:9f:eb:8f:14. Note: Always force lower case on this field and use colons instead of dashes, spaces, or no separator.",
                     "condition": "dest_mac=*",
                     "name": "dest_mac",
                     "type": "conditional",
                     "validity": "if(match(dest_mac,\"^([0-9A-F]{2}[:-]){5}([0-9A-F]{2})$\"),dest_mac,null())"
@@ -202,15 +202,15 @@
                     "comment": "The total count of packets transmitted by this device/interface.",
                     "name": "packets_out",
                     "type": "optional",
                     "validity": "if(isnum(packets_out),packets_out,null())"
                 },
                 {
                     "comment": "The OSI layer 3 (network) protocol of the traffic observed, in lower case. For example, ip, appletalk, ipx.",
-                    "condition": "| where match(src, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\") or match(dest, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\")",
+                    "condition": "| where match(src, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\") or match(dest, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\")",
                     "expected_values": [
                         "ip",
                         "icmp"
                     ],
                     "name": "protocol",
                     "type": "conditional"
                 },
@@ -240,15 +240,15 @@
                     "name": "session_id",
                     "type": "optional"
                 },
                 {
                     "comment": "The source of the network traffic (the client requesting the connection). You can alias this from more specific fields, such as src_host, src_ip, or src_name.'",
                     "name": "src",
                     "type": "required",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
                 },
                 {
                     "comment": "The interface that is listening locally or sending packets remotely. Can also be referred to as the 'ingress interface.'",
                     "name": "src_interface",
                     "type": "optional"
                 },
                 {
@@ -323,15 +323,15 @@
                     "type": "required"
                 },
                 {
                     "comment": "The ip address of the source.",
                     "condition": "src_ip=*",
                     "name": "src_ip",
                     "type": "conditional",
-                    "validity": "if(match(src_ip, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"),src_ip,null())"
+                    "validity": "if(match(src_ip, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"),src_ip,null())"
                 },
                 {
                     "comment": "The source TCP/IP layer 2 Media Access Control (MAC) address of a packet's destination, such as 06:10:9f:eb:8f:14. Note: Always force lower case on this field and use colons instead of dashes, spaces, or no separator.",
                     "condition": "src_mac=*",
                     "name": "src_mac",
                     "type": "conditional",
                     "validity": "if(match(src_mac,\"^([0-9A-F]{2}[:-]){5}([0-9A-F]{2})$\"),src_mac,null())"
```

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Updates.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Updates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/data_models/Web.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Web.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/key_fields.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/index_tests/test_templates.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/rule.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/junit_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/log_helper.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/pytest_splunk_addon/tools/cim_field_report.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/tools/cim_field_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6/PKG-INFO` & `pytest_splunk_addon-5.2.6b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon
-Version: 5.2.6
+Version: 5.2.6b1
 Summary: A Dynamic test tool for Splunk Apps and Add-ons
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: Faker (>=18.0.0,<19.0.0)
+Requires-Dist: Faker (>=13.12,<19.0.0)
 Requires-Dist: addonfactory-splunk-conf-parser-lib
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: filelock (>=3.0,<4.0)
-Requires-Dist: jsonschema (>=v4.17.3,<5.0.0)
+Requires-Dist: jsonschema (>=4,<5)
 Requires-Dist: junitparser (>=2.2.0,<3.0.0)
 Requires-Dist: pytest (>5.4.0,<8)
 Requires-Dist: pytest-ordering (>=0.6,<0.7)
-Requires-Dist: pytest-xdist (>=3.5.0,<4.0.0)
+Requires-Dist: pytest-xdist (>=2.3.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: splunk-sdk (>=1.6)
 Requires-Dist: splunksplwrapper (>=1.1.1,<2.0.0)
 Requires-Dist: urllib3 (<2)
-Requires-Dist: xmlschema (>=2.5.1,<3.0.0)
+Requires-Dist: xmlschema (>=1.11.3,<2.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
```

