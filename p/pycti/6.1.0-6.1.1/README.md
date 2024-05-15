# Comparing `tmp/pycti-6.1.0.tar.gz` & `tmp/pycti-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.1.0.tar", last modified: Mon May 13 08:06:32 2024, max compression
+gzip compressed data, was "pycti-6.1.1.tar", last modified: Wed May 15 09:35:07 2024, max compression
```

## Comparing `pycti-6.1.0.tar` & `pycti-6.1.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.225975 pycti-6.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-13 08:06:17.000000 pycti-6.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-13 08:06:32.225975 pycti-6.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-13 08:06:17.000000 pycti-6.1.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.213975 pycti-6.1.0/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.213975 pycti-6.1.0/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.213975 pycti-6.1.0/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60538 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.221975 pycti-6.1.0/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18990 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78434 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16641 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.225975 pycti-6.1.0/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   120458 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-13 08:06:17.000000 pycti-6.1.0/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-13 08:06:32.225975 pycti-6.1.0/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-13 08:06:32.000000 pycti-6.1.0/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-13 08:06:17.000000 pycti-6.1.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-13 08:06:32.229975 pycti-6.1.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-15 09:34:55.000000 pycti-6.1.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-15 09:35:07.657570 pycti-6.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-15 09:34:55.000000 pycti-6.1.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.645570 pycti-6.1.1/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.649570 pycti-6.1.1/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.649570 pycti-6.1.1/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60606 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   115786 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-15 09:34:55.000000 pycti-6.1.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-15 09:35:07.661570 pycti-6.1.1/setup.cfg
```

### Comparing `pycti-6.1.0/LICENSE` & `pycti-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/PKG-INFO` & `pycti-6.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.0
+Version: 6.1.1
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.0/README.md` & `pycti-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/__init__.py` & `pycti-6.1.1/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.1.0"
+__version__ = "6.1.1"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-6.1.0/pycti/api/opencti_api_client.py` & `pycti-6.1.1/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/api/opencti_api_connector.py` & `pycti-6.1.1/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/api/opencti_api_playbook.py` & `pycti-6.1.1/pycti/api/opencti_api_playbook.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/api/opencti_api_work.py` & `pycti-6.1.1/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/connector/opencti_connector.py` & `pycti-6.1.1/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/connector/opencti_connector_helper.py` & `pycti-6.1.1/pycti/connector/opencti_connector_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,17 @@
                     event_data["stix_objects"] = stix_objects
                     stix_entity = [e for e in stix_objects if e["id"] == entity_id][0]
                     event_data["stix_entity"] = stix_entity
                 else:
                     # If not playbook but enrichment, compute object on enrichment_entity
                     opencti_entity = event_data["enrichment_entity"]
                     stix_objects = self.helper.api.stix2.prepare_export(
-                        self.helper.api.stix2.generate_export(copy.copy(opencti_entity))
+                        entity=self.helper.api.stix2.generate_export(
+                            copy.copy(opencti_entity)
+                        )
                     )
                     stix_entity = [
                         e
                         for e in stix_objects
                         if e["id"] == opencti_entity["standard_id"]
                     ][0]
                     event_data["stix_objects"] = stix_objects
@@ -1563,15 +1565,15 @@
 
     def get_data_from_enrichment(self, data, standard_id, opencti_entity):
         bundle = data.get("bundle", None)
         # Extract main entity from bundle in case of playbook
         if bundle is None:
             # Generate bundle
             stix_objects = self.api.stix2.prepare_export(
-                self.api.stix2.generate_export(copy.copy(opencti_entity))
+                entity=self.api.stix2.generate_export(copy.copy(opencti_entity))
             )
         else:
             stix_objects = bundle["objects"]
         stix_entity = [e for e in stix_objects if e["id"] == standard_id][0]
         return {
             "stix_entity": stix_entity,
             "stix_objects": stix_objects,
```

### Comparing `pycti-6.1.0/pycti/connector/opencti_metric_handler.py` & `pycti-6.1.1/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_attack_pattern.py` & `pycti-6.1.1/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_campaign.py` & `pycti-6.1.1/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_case_incident.py` & `pycti-6.1.1/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_case_rfi.py` & `pycti-6.1.1/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_case_rft.py` & `pycti-6.1.1/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_channel.py` & `pycti-6.1.1/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_course_of_action.py` & `pycti-6.1.1/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_data_component.py` & `pycti-6.1.1/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_data_source.py` & `pycti-6.1.1/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_event.py` & `pycti-6.1.1/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_external_reference.py` & `pycti-6.1.1/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_feedback.py` & `pycti-6.1.1/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_grouping.py` & `pycti-6.1.1/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_identity.py` & `pycti-6.1.1/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_incident.py` & `pycti-6.1.1/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_indicator.py` & `pycti-6.1.1/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_infrastructure.py` & `pycti-6.1.1/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_intrusion_set.py` & `pycti-6.1.1/pycti/entities/opencti_intrusion_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,25 +271,23 @@
                         hasPreviousPage
                         globalCount
                     }
                 }
             }
         """
         )
-        result = self.opencti.query(
-            query,
-            {
-                "filters": filters,
-                "search": search,
-                "first": first,
-                "after": after,
-                "orderBy": order_by,
-                "orderMode": order_mode,
-            },
-        )
+        variables = {
+            "filters": filters,
+            "search": search,
+            "first": first,
+            "after": after,
+            "orderBy": order_by,
+            "orderMode": order_mode,
+        }
+        result = self.opencti.query(query, variables)
         if get_all:
             final_data = []
             data = self.opencti.process_multiple(result["data"]["intrusionSets"])
             final_data = final_data + data
             while result["data"]["intrusionSets"]["pageInfo"]["hasNextPage"]:
                 after = result["data"]["intrusionSets"]["pageInfo"]["endCursor"]
                 self.opencti.app_logger.info("Listing Intrusion-Sets", {"after": after})
```

### Comparing `pycti-6.1.0/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.1.1/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_label.py` & `pycti-6.1.1/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_language.py` & `pycti-6.1.1/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_location.py` & `pycti-6.1.1/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_malware.py` & `pycti-6.1.1/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_malware_analysis.py` & `pycti-6.1.1/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_marking_definition.py` & `pycti-6.1.1/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_narrative.py` & `pycti-6.1.1/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_note.py` & `pycti-6.1.1/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_observed_data.py` & `pycti-6.1.1/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_opinion.py` & `pycti-6.1.1/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_report.py` & `pycti-6.1.1/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix.py` & `pycti-6.1.1/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix_core_object.py` & `pycti-6.1.1/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.1.1/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.1.1/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.1.1/pycti/entities/opencti_stix_domain_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1351,16 +1351,18 @@
                 "file": file,
                 "file_markings": file_markings,
                 "listFilters": list_filters,
             },
         )
 
     def push_entity_export(
-        self, entity_id, file_name, data, file_markings, mime_type=None
+        self, entity_id, file_name, data, file_markings=None, mime_type=None
     ):
+        if file_markings is None:
+            file_markings = []
         query = """
             mutation StixDomainObjectEdit(
                 $id: ID!, $file: Upload!,
                 $file_markings: [String]!
             ) {
                 stixDomainObjectEdit(id: $id) {
                     exportPush(
```

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.1.1/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.1.1/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files 4% similar despite different names*

```diff
@@ -509,14 +509,15 @@
             return None
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
         first = kwargs.get("first", 100)
         after = kwargs.get("after", None)
+        get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("with_pagination", False)
         custom_attributes = kwargs.get("customAttributes", None)
 
         self.opencti.app_logger.info(
             "Listing StixObjectOrStixRelationships with filters",
             {"filters": json.dumps(filters)},
         )
@@ -538,20 +539,44 @@
                                 hasPreviousPage
                                 globalCount
                             }
                         }
                     }
                 """
         )
+        variables = {
+            "filters": filters,
+            "search": search,
+            "first": first,
+            "after": after,
+        }
         result = self.opencti.query(
             query,
-            {
-                "filters": filters,
-                "search": search,
-                "first": first,
-                "after": after,
-            },
+            variables,
         )
 
-        return self.opencti.process_multiple(
-            result["data"]["stixObjectOrStixRelationships"], with_pagination
-        )
+        if get_all:
+            final_data = []
+            data = self.opencti.process_multiple(
+                result["data"]["stixObjectOrStixRelationships"]
+            )
+            final_data = final_data + data
+            while result["data"]["stixObjectOrStixRelationships"]["pageInfo"][
+                "hasNextPage"
+            ]:
+                after = result["data"]["stixObjectOrStixRelationships"]["pageInfo"][
+                    "endCursor"
+                ]
+                self.opencti.app_logger.info(
+                    "Listing stixObjectOrStixRelationships", {"after": after}
+                )
+                after_variables = {**variables, **{"after": after}}
+                result = self.opencti.query(query, after_variables)
+                data = self.opencti.process_multiple(
+                    result["data"]["stixObjectOrStixRelationships"]
+                )
+                final_data = final_data + data
+            return final_data
+        else:
+            return self.opencti.process_multiple(
+                result["data"]["stixObjectOrStixRelationships"], with_pagination
+            )
```

### Comparing `pycti-6.1.0/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.1.1/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_task.py` & `pycti-6.1.1/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_threat_actor.py` & `pycti-6.1.1/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.1.1/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.1.1/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_tool.py` & `pycti-6.1.1/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_vocabulary.py` & `pycti-6.1.1/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/entities/opencti_vulnerability.py` & `pycti-6.1.1/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/utils/constants.py` & `pycti-6.1.1/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/utils/opencti_logger.py` & `pycti-6.1.1/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/utils/opencti_stix2.py` & `pycti-6.1.1/pycti/utils/opencti_stix2.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,51 +131,14 @@
             return stix_object["x_mitre_aliases"]
         elif "x_amitt_aliases" in stix_object:
             return stix_object["x_amitt_aliases"]
         elif "aliases" in stix_object:
             return stix_object["aliases"]
         return None
 
-    def check_max_marking_definition(
-        self, max_marking_definition_entity: Dict, entity_marking_definitions: List
-    ) -> bool:
-        """checks if a list of marking definitions conforms with a given max level
-
-        :param max_marking_definition_entity: the maximum allowed marking definition level
-        :type max_marking_definition_entity: str, optional
-        :param entity_marking_definitions: list of entities to check
-        :type entity_marking_definitions: list
-        :return: `True` if the list conforms with max marking definition
-        :rtype: bool
-        """
-
-        # Max is not set, return True
-        if max_marking_definition_entity is None:
-            return True
-        # Filter entity markings definition to the max_marking_definition type
-        typed_entity_marking_definitions = []
-        for entity_marking_definition in entity_marking_definitions:
-            if (
-                entity_marking_definition["definition_type"]
-                == max_marking_definition_entity["definition_type"]
-            ):
-                typed_entity_marking_definitions.append(entity_marking_definition)
-        # No entity marking defintions of the max_marking_definition type
-        if len(typed_entity_marking_definitions) == 0:
-            return True
-
-        # Check if level is less or equal to max
-        for typed_entity_marking_definition in typed_entity_marking_definitions:
-            if (
-                typed_entity_marking_definition["x_opencti_order"]
-                <= max_marking_definition_entity["x_opencti_order"]
-            ):
-                return True
-        return False
-
     def import_bundle_from_file(
         self, file_path: str, update: bool = False, types: List = None
     ) -> Optional[List]:
         """import a stix2 bundle from a file
 
         :param file_path: valid path to the file
         :type file_path: str
@@ -1655,105 +1618,80 @@
         if "created_at" in entity:
             del entity["created_at"]
         if "updated_at" in entity:
             del entity["updated_at"]
 
         return {k: v for k, v in entity.items() if self.opencti.not_empty(v)}
 
-    def prepare_filters_export(self, id: str, access_filter: Dict = None) -> Dict:
+    @staticmethod
+    def prepare_id_filters_export(
+        id: Union[str, List[str]], access_filter: Dict = None
+    ) -> Dict:
         if access_filter is not None:
             return {
                 "mode": "and",
                 "filterGroups": [
                     {
                         "mode": "or",
                         "filters": [
                             {
-                                "key": "id",
-                                "values": [id],
+                                "key": "ids",
+                                "values": id if isinstance(id, list) else [id],
                             }
                         ],
                         "filterGroups": [],
                     },
                     access_filter,
                 ],
                 "filters": [],
             }
         else:
             return {
                 "mode": "and",
-                "filterGroups": [
+                "filterGroups": [],
+                "filters": [
                     {
+                        "key": "ids",
                         "mode": "or",
-                        "filters": [
-                            {
-                                "key": "id",
-                                "values": [id],
-                            }
-                        ],
-                        "filterGroups": [],
-                    },
+                        "values": id if isinstance(id, list) else [id],
+                    }
                 ],
-                "filters": [],
             }
 
     def prepare_export(
         self,
         entity: Dict,
         mode: str = "simple",
-        max_marking_definition_entity: Dict = None,
-        main_filter: Dict = None,
         access_filter: Dict = None,
         no_custom_attributes: bool = False,
     ) -> List:
         result = []
         objects_to_get = []
         relations_to_get = []
 
         # Container
         if "objects" in entity and len(entity["objects"]) > 0:
-            del entity["objects"]
-            regarding_of_filter = {
-                "mode": "and",
-                "filterGroups": [],
-                "filters": [
-                    {
-                        "key": "regardingOf",
-                        "mode": "and",
-                        "operator": "eq",
-                        "values": [
-                            {"key": "id", "values": [entity["x_opencti_id"]]},
-                            {"key": "relationship_type", "values": ["object"]},
-                        ],
-                    }
-                ],
-            }
-            filter_groups = []
-            if regarding_of_filter is not None:
-                filter_groups.append(regarding_of_filter)
-            if access_filter is not None:
-                filter_groups.append(access_filter)
-            export_query_filter = {
-                "mode": "and",
-                "filterGroups": filter_groups,
-                "filters": [],
-            }
-            entity["objects"] = (
+            object_ids = list(map(lambda e: e["standard_id"], entity["objects"]))
+            export_query_filter = self.prepare_id_filters_export(
+                id=object_ids, access_filter=access_filter
+            )
+            filtered_objects = (
                 self.opencti.opencti_stix_object_or_stix_relationship.list(
-                    filters=export_query_filter
+                    filters=export_query_filter, getAll=True
                 )
             )
+            entity["objects"] = filtered_objects
 
         # CreatedByRef
         if (
             not no_custom_attributes
             and "createdBy" in entity
             and entity["createdBy"] is not None
         ):
-            created_by = self.generate_export(entity["createdBy"])
+            created_by = self.generate_export(entity=entity["createdBy"])
             if entity["type"] in STIX_CYBER_OBSERVABLE_MAPPING:
                 entity["x_opencti_created_by_ref"] = created_by["id"]
             else:
                 entity["created_by_ref"] = created_by["id"]
             result.append(created_by)
         # Labels
         if entity["type"] in STIX_CYBER_OBSERVABLE_MAPPING and "labels" in entity:
@@ -1923,29 +1861,29 @@
             del entity["objectsIds"]
         # Stix Sighting Relationship
         if entity["type"] == "stix-sighting-relationship":
             entity["type"] = "sighting"
             entity["count"] = entity["attribute_count"]
             del entity["attribute_count"]
             from_to_check = entity["from"]["id"]
-            relationships_from_filter = self.prepare_filters_export(
+            relationships_from_filter = self.prepare_id_filters_export(
                 id=from_to_check, access_filter=access_filter
             )
             x = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_from_filter
             )
             if len(x) > 0:
                 entity["sighting_of_ref"] = entity["from"]["id"]
                 # handle from and to separately like Stix Core Relationship and call 2 requests
                 objects_to_get.append(
                     entity["from"]
                 )  # what happen with unauthorized objects ?
 
             to_to_check = [entity["to"]["id"]]
-            relationships_to_filter = self.prepare_filters_export(
+            relationships_to_filter = self.prepare_id_filters_export(
                 id=to_to_check, access_filter=access_filter
             )
             y = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_to_filter
             )
             if len(y) > 0:
                 entity["where_sighted_refs"] = [entity["to"]["id"]]
@@ -1954,30 +1892,30 @@
             del entity["from"]
             del entity["to"]
         # Stix Core Relationship
         if "from" in entity or "to" in entity:
             entity["type"] = "relationship"
         if "from" in entity:
             from_to_check = entity["from"]["id"]
-            relationships_from_filter = self.prepare_filters_export(
+            relationships_from_filter = self.prepare_id_filters_export(
                 id=from_to_check, access_filter=access_filter
             )
             x = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_from_filter
             )
             if len(x) > 0:
                 entity["source_ref"] = entity["from"]["id"]
                 # handle from and to separately like Stix Core Relationship and call 2 requests
                 objects_to_get.append(
                     entity["from"]
                 )  # what happen with unauthorized objects ?
             del entity["from"]
         if "to" in entity:
             to_to_check = [entity["to"]["id"]]
-            relationships_to_filter = self.prepare_filters_export(
+            relationships_to_filter = self.prepare_id_filters_export(
                 id=to_to_check, access_filter=access_filter
             )
             y = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_to_filter
             )
             if len(y) > 0:
                 entity["target_ref"] = entity["to"]["id"]
@@ -2110,92 +2048,55 @@
                                 }
                             )
             # Get extra relations (from AND to)
             stix_core_relationships = self.opencti.stix_core_relationship.list(
                 fromOrToId=entity["x_opencti_id"], getAll=True, filters=access_filter
             )
             for stix_core_relationship in stix_core_relationships:
-                if self.check_max_marking_definition(
-                    max_marking_definition_entity,
-                    (
-                        stix_core_relationship["objectMarking"]
-                        if "objectMarking" in stix_core_relationship
-                        else None
-                    ),
-                ):
-                    objects_to_get.append(
-                        stix_core_relationship["to"]
-                        if stix_core_relationship["to"]["id"] != entity["x_opencti_id"]
-                        else stix_core_relationship["from"]
-                    )
-                    relation_object_data = (
-                        self.prepare_export(  # ICI -> remove max marking ?
-                            self.generate_export(stix_core_relationship),
-                            "simple",
-                            max_marking_definition_entity,
-                            main_filter,
-                            access_filter,
-                        )
-                    )
-                    relation_object_bundle = self.filter_objects(
-                        uuids, relation_object_data
-                    )
-                    uuids = uuids + [x["id"] for x in relation_object_bundle]
-                    result = result + relation_object_bundle
-                else:
-                    self.opencti.app_logger.info(
-                        "Marking definitions are less than max definition, "
-                        "not exporting the relation AND the target entity.",
-                        {
-                            "type": stix_core_relationship["entity_type"],
-                            "id": stix_core_relationship["id"],
-                        },
+                objects_to_get.append(
+                    stix_core_relationship["to"]
+                    if stix_core_relationship["to"]["id"] != entity["x_opencti_id"]
+                    else stix_core_relationship["from"]
+                )
+                relation_object_data = (
+                    self.prepare_export(  # ICI -> remove max marking ?
+                        entity=self.generate_export(stix_core_relationship),
+                        mode="simple",
+                        access_filter=access_filter,
                     )
+                )
+                relation_object_bundle = self.filter_objects(
+                    uuids, relation_object_data
+                )
+                uuids = uuids + [x["id"] for x in relation_object_bundle]
+                result = result + relation_object_bundle
+
             # Get sighting
             stix_sighting_relationships = self.opencti.stix_sighting_relationship.list(
                 fromOrToId=entity["x_opencti_id"], getAll=True, filters=access_filter
             )
             for stix_sighting_relationship in stix_sighting_relationships:
-                if self.check_max_marking_definition(
-                    max_marking_definition_entity,
-                    (
-                        stix_sighting_relationship["objectMarking"]
-                        if "objectMarking" in stix_sighting_relationship
-                        else None
-                    ),
-                ):
-                    objects_to_get.append(
-                        stix_sighting_relationship["to"]
-                        if stix_sighting_relationship["to"]["id"]
-                        != entity["x_opencti_id"]
-                        else stix_sighting_relationship["from"]
-                    )
-                    relation_object_data = (
-                        self.prepare_export(  # ICI -> remove max marking ?
-                            self.generate_export(stix_sighting_relationship),
-                            "simple",
-                            max_marking_definition_entity,
-                            main_filter,
-                            access_filter,
-                        )
-                    )
-                    relation_object_bundle = self.filter_objects(
-                        uuids, relation_object_data
-                    )
-                    uuids = uuids + [x["id"] for x in relation_object_bundle]
-                    result = result + relation_object_bundle
-                else:
-                    self.opencti.app_logger.info(
-                        "Marking definitions are less than max definition, "
-                        "not exporting the relation AND the target entity.",
-                        {
-                            "type": stix_sighting_relationship["entity_type"],
-                            "id": stix_sighting_relationship["id"],
-                        },
+                objects_to_get.append(
+                    stix_sighting_relationship["to"]
+                    if stix_sighting_relationship["to"]["id"] != entity["x_opencti_id"]
+                    else stix_sighting_relationship["from"]
+                )
+                relation_object_data = (
+                    self.prepare_export(  # ICI -> remove max marking ?
+                        entity=self.generate_export(stix_sighting_relationship),
+                        mode="simple",
+                        access_filter=access_filter,
                     )
+                )
+                relation_object_bundle = self.filter_objects(
+                    uuids, relation_object_data
+                )
+                uuids = uuids + [x["id"] for x in relation_object_bundle]
+                result = result + relation_object_bundle
+
             if no_custom_attributes:
                 del entity["x_opencti_id"]
             # Export
             reader = self.get_readers()
             # Get extra objects
             for entity_object in objects_to_get:
                 # Map types
@@ -2215,24 +2116,24 @@
 
                 do_read = reader.get(
                     entity_object["entity_type"],
                     lambda **kwargs: self.unknown_type(
                         {"type": entity_object["entity_type"]}
                     ),
                 )
-                entity_object_data = do_read(
-                    id=entity_object["id"], filters=access_filter
+
+                query_filters = self.prepare_id_filters_export(
+                    entity_object["id"], access_filter
                 )
+                entity_object_data = do_read(filters=query_filters)
                 if entity_object_data is not None:
                     stix_entity_object = self.prepare_export(
-                        self.generate_export(entity_object_data),
-                        "simple",
-                        max_marking_definition_entity,
-                        main_filter,
-                        access_filter,
+                        entity=self.generate_export(entity_object_data),
+                        mode="simple",
+                        access_filter=access_filter,
                     )
                     # Add to result
                     entity_object_bundle = self.filter_objects(
                         uuids, stix_entity_object
                     )
                     uuids = uuids + [x["id"] for x in entity_object_bundle]
                     result = result + entity_object_bundle
@@ -2240,15 +2141,15 @@
                 relation_object
             ) in relations_to_get:  # never appended after initialization
 
                 def find_relation_object_data(current_relation_object):
                     return current_relation_object.id == relation_object["id"]
 
                 relation_object_data = self.prepare_export(
-                    filter(
+                    entity=filter(
                         find_relation_object_data,
                         self.opencti.stix_core_relationship.list(filters=access_filter),
                     )
                 )
                 relation_object_bundle = self.filter_objects(
                     uuids, relation_object_data
                 )
@@ -2260,15 +2161,14 @@
             for uuid in uuids:
                 if "marking-definition" not in uuid:
                     reports = self.opencti.opencti_stix_object_or_stix_relationship.reports(id=uuid)
                     for report in reports:
                         report_object_data = self.opencti.report.to_stix2(
                             entity=report,
                             mode="simple",
-                            max_marking_definition_entity=max_marking_definition_entity,
                         )
                         report_object_bundle = self.filter_objects(
                             uuids, report_object_data
                         )
                         uuids = uuids + [x["id"] for x in report_object_bundle]
                         result = result + report_object_bundle
             """
@@ -2279,15 +2179,14 @@
             #        notes = self.opencti.opencti_stix_object_or_stix_relationship.notes(
             #            id=export_uuid
             #        )
             #        for note in notes:
             #            note_object_data = self.opencti.note.to_stix2(
             #                entity=note,
             #                mode="simple",
-            #                max_marking_definition_entity=max_marking_definition_entity,
             #            )
             #            note_object_bundle = self.filter_objects(
             #                uuids, note_object_data
             #            )
             #            uuids = uuids + [x["id"] for x in note_object_bundle]
             #            result = result + note_object_bundle
 
@@ -2308,22 +2207,20 @@
                     final_result.append(entity)
                 else:
                     final_result.append(entity)
             return final_result
         else:
             return []
 
-    def export_entity(
+    def get_stix_bundle_or_object_from_entity_id(
         self,
         entity_type: str,
         entity_id: str,
         mode: str = "simple",
-        main_filter: Dict = None,
         access_filter: Dict = None,
-        max_marking_definition: Dict = None,
         no_custom_attributes: bool = False,
         only_entity: bool = False,
     ) -> Dict:
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
@@ -2334,51 +2231,68 @@
 
         # Map types
         if IdentityTypes.has_value(entity_type):
             entity_type = "Identity"
         if LocationTypes.has_value(entity_type):
             entity_type = "Location"
 
-        # Lister
-        listers = self.get_listers()
-        do_list = listers.get(
+        readers = self.get_readers()
+        do_read = readers.get(
             entity_type, lambda **kwargs: self.unknown_type({"type": entity_type})
         )
-        entity = do_list(filters=main_filter)[0]
+        entity = do_read(id=entity_id)
         if entity is None:
             self.opencti.app_logger.error(
                 "Cannot export entity (not found)", {"id": entity_id}
             )
             return bundle
         entity_standard_id = entity["standard_id"]
         stix_objects = self.prepare_export(
-            self.generate_export(entity, no_custom_attributes),
-            mode,
-            None,
-            main_filter,
-            access_filter,
-            no_custom_attributes,
+            entity=self.generate_export(entity, no_custom_attributes),
+            mode=mode,
+            access_filter=access_filter,
+            no_custom_attributes=no_custom_attributes,
         )
         if stix_objects is not None:
             bundle["objects"].extend(stix_objects)
         if only_entity:
             return [e for e in bundle["objects"] if e.get("id") == entity_standard_id][
                 0
             ]
         return bundle
 
+    # Please use get_stix_bundle_or_object_from_entity_id instead
+    @DeprecationWarning
+    def export_entity(
+        self,
+        entity_type: str,
+        entity_id: str,
+        mode: str = "simple",
+        access_filter: Dict = None,
+        no_custom_attributes: bool = False,
+        only_entity: bool = False,
+    ) -> Dict:
+        return self.get_stix_bundle_or_object_from_entity_id(
+            entity_type=entity_type,
+            entity_id=entity_id,
+            mode=mode,
+            access_filter=access_filter,
+            no_custom_attributes=no_custom_attributes,
+            only_entity=only_entity,
+        )
+
     def export_entities_list(
         self,
         entity_type: str,
         search: Dict = None,
         filters: Dict = None,
         orderBy: str = None,
         orderMode: str = None,
         getAll: bool = True,
-    ) -> Dict:
+    ) -> [Dict]:
         if IdentityTypes.has_value(entity_type):
             entity_type = "Identity"
 
         if LocationTypes.has_value(entity_type):
             entity_type = "Location"
 
         if StixCyberObservableTypes.has_value(entity_type):
@@ -2443,98 +2357,81 @@
         self,
         entity_type: str,
         search: Dict = None,
         filters: Dict = None,
         order_by: str = None,
         order_mode: str = None,
         mode: str = "simple",
-        main_filter: Dict = None,
         access_filter: Dict = None,
     ) -> Dict:
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
-        filterGroups = []
+        filter_groups = []
         if filters is not None:
-            filterGroups.append(filters)
+            filter_groups.append(filters)
         if access_filter is not None:
-            filterGroups.append(access_filter)
+            filter_groups.append(access_filter)
         export_query_filter = {
             "mode": "and",
-            "filterGroups": filterGroups,
+            "filterGroups": filter_groups,
             "filters": [],
         }
         entities_list = self.export_entities_list(
             entity_type=entity_type,
             search=search,
             filters=export_query_filter,
             orderBy=order_by,
             orderMode=order_mode,
             getAll=True,
         )
         if entities_list is not None:
             uuids = []
             for entity in entities_list:
                 entity_bundle = self.prepare_export(
-                    self.generate_export(entity),
-                    mode,
-                    None,
-                    main_filter,
-                    access_filter,
+                    entity=self.generate_export(entity),
+                    mode=mode,
+                    access_filter=access_filter,
                 )
                 if entity_bundle is not None:
                     entity_bundle_filtered = self.filter_objects(uuids, entity_bundle)
                     for x in entity_bundle_filtered:
                         uuids.append(x["id"])
                     bundle["objects"] = bundle["objects"] + entity_bundle_filtered
         return bundle
 
     def export_selected(
         self,
-        entities_list: [str],
+        entities_list: [dict],
         mode: str = "simple",
-        main_filter: Dict = None,
         access_filter: Dict = None,
     ) -> Dict:
 
-        entity_data_sdo = self.opencti.stix_domain_object.list(filters=main_filter)
-        entity_data_sco = self.opencti.stix_cyber_observable.list(filters=main_filter)
-        entity_data_scr = self.opencti.stix_core_relationship.list(filters=main_filter)
-        entity_data_ssr = self.opencti.stix_sighting_relationship.list(
-            filters=main_filter
-        )
-
-        entities_list = (
-            entity_data_sdo + entity_data_sco + entity_data_scr + entity_data_ssr
-        )
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
 
-        if entities_list is not None:
-            uuids = []
-            for entity in entities_list:
-                entity_bundle = self.prepare_export(
-                    self.generate_export(entity),
-                    mode,
-                    None,
-                    main_filter,
-                    access_filter,
-                )
-                if entity_bundle is not None:
-                    entity_bundle_filtered = self.filter_objects(uuids, entity_bundle)
-                    for x in entity_bundle_filtered:
-                        uuids.append(x["id"])
-                    bundle["objects"] = (
-                        bundle["objects"] + entity_bundle_filtered
-                    )  # unsupported operand type(s) for +: 'dict' and 'list'
+        uuids = []
+        for entity in entities_list:
+            entity_bundle = self.prepare_export(
+                entity=self.generate_export(entity),
+                mode=mode,
+                access_filter=access_filter,
+            )
+            if entity_bundle is not None:
+                entity_bundle_filtered = self.filter_objects(uuids, entity_bundle)
+                for x in entity_bundle_filtered:
+                    uuids.append(x["id"])
+                bundle["objects"] = (
+                    bundle["objects"] + entity_bundle_filtered
+                )  # unsupported operand type(s) for +: 'dict' and 'list'
 
         return bundle
 
     def import_bundle(
         self,
         stix_bundle: Dict,
         update: bool = False,
```

### Comparing `pycti-6.1.0/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.1.1/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/utils/opencti_stix2_update.py` & `pycti-6.1.1/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti/utils/opencti_stix2_utils.py` & `pycti-6.1.1/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti.egg-info/PKG-INFO` & `pycti-6.1.1/pycti.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.0
+Version: 6.1.1
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.0/pycti.egg-info/SOURCES.txt` & `pycti-6.1.1/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pycti.egg-info/requires.txt` & `pycti-6.1.1/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/pyproject.toml` & `pycti-6.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.1.0/setup.cfg` & `pycti-6.1.1/setup.cfg`

 * *Files identical despite different names*

