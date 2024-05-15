# Comparing `tmp/usdm-0.50.0.tar.gz` & `tmp/usdm-0.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.50.0.tar", last modified: Sat Apr 20 07:43:09 2024, max compression
+gzip compressed data, was "usdm-0.51.0.tar", last modified: Wed May 15 06:00:26 2024, max compression
```

## Comparing `usdm-0.50.0.tar` & `usdm-0.51.0.tar`

### file list

```diff
@@ -1,247 +1,256 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.774372 usdm-0.50.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.50.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    38155 2024-04-20 07:43:09.773994 usdm-0.50.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    37497 2024-04-19 04:39:42.000000 usdm-0.50.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.50.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2024-04-20 07:43:09.774435 usdm-0.50.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      972 2023-10-12 07:52:37.000000 usdm-0.50.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.719701 usdm-0.50.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.773427 usdm-0.50.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    38155 2024-04-20 07:43:09.000000 usdm-0.50.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     8436 2024-04-20 07:43:09.000000 usdm-0.50.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2024-04-20 07:43:09.000000 usdm-0.50.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       73 2024-04-20 07:43:09.000000 usdm-0.50.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       40 2024-04-20 07:43:09.000000 usdm-0.50.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.723257 usdm-0.50.0/src/usdm_db/
--rw-r--r--   0 daveih     (501) staff       (20)     2478 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1454 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/cross_reference.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.724271 usdm-0.50.0/src/usdm_db/document/
--rw-r--r--   0 daveih     (501) staff       (20)       27 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/document/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)    13622 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/document/document.py
--rw-r--r--   0 daveih     (501) staff       (20)      758 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/document/utility.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.725190 usdm-0.50.0/src/usdm_db/errors_and_logging/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/errors_and_logging/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      602 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/errors_and_logging/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      696 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/errors_and_logging/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1013 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/errors_and_logging/errors_and_logging.py
--rw-r--r--   0 daveih     (501) staff       (20)     3331 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/neo4j_dict.py
--rw-r--r--   0 daveih     (501) staff       (20)     3608 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_db/timeline.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.730956 usdm-0.50.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)    12623 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      364 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)    18660 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)    16463 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/cdisc_bc_library.py
--rw-r--r--   0 daveih     (501) staff       (20)      987 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     7304 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)      523 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/code_base.py
--rw-r--r--   0 daveih     (501) staff       (20)     1795 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2987 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      478 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.733744 usdm-0.50.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)   833791 2024-03-29 05:59:21.000000 usdm-0.50.0/src/usdm_excel/data/cdisc_bcs.yaml
--rw-r--r--   0 daveih     (501) staff       (20)   994684 2024-03-29 08:02:31.000000 usdm-0.50.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml
--rw-r--r--   0 daveih     (501) staff       (20)     1771 2024-03-29 08:02:31.000000 usdm-0.50.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)    17843 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.737531 usdm-0.50.0/src/usdm_excel/document/
--rw-r--r--   0 daveih     (501) staff       (20)      101 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/document/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5268 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/document/elements.py
--rw-r--r--   0 daveih     (501) staff       (20)     5796 2024-04-19 14:44:40.000000 usdm-0.50.0/src/usdm_excel/document/macros.py
--rw-r--r--   0 daveih     (501) staff       (20)     5087 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/document/soa.py
--rw-r--r--   0 daveih     (501) staff       (20)     1065 2024-04-05 04:37:08.000000 usdm-0.50.0/src/usdm_excel/document/template_base.py
--rw-r--r--   0 daveih     (501) staff       (20)     4803 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/document/template_m11.py
--rw-r--r--   0 daveih     (501) staff       (20)     6608 2024-04-19 11:24:09.000000 usdm-0.50.0/src/usdm_excel/document/template_plain.py
--rw-r--r--   0 daveih     (501) staff       (20)      658 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/document/utility.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.738458 usdm-0.50.0/src/usdm_excel/errors_and_logging/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/errors_and_logging/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      933 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/errors_and_logging/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      632 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/errors_and_logging/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1735 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/errors_and_logging/errors_and_logging.py
--rw-r--r--   0 daveih     (501) staff       (20)     1156 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/globals.py
--rw-r--r--   0 daveih     (501) staff       (20)     2040 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     1250 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      883 2023-10-12 07:51:31.000000 usdm-0.50.0/src/usdm_excel/iso_8601_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      376 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)      854 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      200 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/other_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     1501 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/quantity_type.py
--rw-r--r--   0 daveih     (501) staff       (20)     1604 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/range_type.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.739025 usdm-0.50.0/src/usdm_excel/study_design_activity_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.50.0/src/usdm_excel/study_design_activity_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1305 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.739320 usdm-0.50.0/src/usdm_excel/study_design_amendment_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.50.0/src/usdm_excel/study_design_amendment_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     7916 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.739706 usdm-0.50.0/src/usdm_excel/study_design_arm_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.50.0/src/usdm_excel/study_design_arm_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1702 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.739976 usdm-0.50.0/src/usdm_excel/study_design_characteristics_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/study_design_characteristics_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1527 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/study_design_characteristics_sheet/study_design_characteristics_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.740243 usdm-0.50.0/src/usdm_excel/study_design_conditions_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-17 06:39:55.000000 usdm-0.50.0/src/usdm_excel/study_design_conditions_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2714 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.740596 usdm-0.50.0/src/usdm_excel/study_design_content_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:51:31.000000 usdm-0.50.0/src/usdm_excel/study_design_content_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3275 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.740892 usdm-0.50.0/src/usdm_excel/study_design_dictionary_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.50.0/src/usdm_excel/study_design_dictionary_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2977 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.741286 usdm-0.50.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2051 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.741698 usdm-0.50.0/src/usdm_excel/study_design_eligibility_criteria_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.50.0/src/usdm_excel/study_design_eligibility_criteria_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1872 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.742233 usdm-0.50.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3005 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.742740 usdm-0.50.0/src/usdm_excel/study_design_epoch_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.50.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1342 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.743011 usdm-0.50.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3397 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.743407 usdm-0.50.0/src/usdm_excel/study_design_indication_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.50.0/src/usdm_excel/study_design_indication_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1125 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.744137 usdm-0.50.0/src/usdm_excel/study_design_intervention_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.50.0/src/usdm_excel/study_design_intervention_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5431 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.744439 usdm-0.50.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3502 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.744720 usdm-0.50.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3964 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.744980 usdm-0.50.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1538 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.745359 usdm-0.50.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     9083 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.746301 usdm-0.50.0/src/usdm_excel/study_design_sites_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-02 13:11:00.000000 usdm-0.50.0/src/usdm_excel/study_design_sites_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2187 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_sites_sheet/study_design_sites_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.746836 usdm-0.50.0/src/usdm_excel/study_design_timing_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.50.0/src/usdm_excel/study_design_timing_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3851 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      819 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_design_timing_sheet/window_type.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.747252 usdm-0.50.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2074 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.747527 usdm-0.50.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.50.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     9005 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.751968 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      514 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     4230 2024-04-19 14:44:40.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      686 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/conditons.py
--rw-r--r--   0 daveih     (501) staff       (20)     3872 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)     2494 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py
--rw-r--r--   0 daveih     (501) staff       (20)      292 2023-10-12 07:52:37.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4035 2024-04-18 13:50:02.000000 usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/study_soa_v2_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     1541 2024-04-19 04:16:10.000000 usdm-0.50.0/src/usdm_excel/syntax_template_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.752326 usdm-0.50.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       58 2024-04-20 07:34:32.000000 usdm-0.50.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.762659 usdm-0.50.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     2792 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      481 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      328 2024-03-29 08:02:31.000000 usdm-0.50.0/src/usdm_model/administration_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      420 2024-03-29 08:02:31.000000 usdm-0.50.0/src/usdm_model/agent_administration.py
--rw-r--r--   0 daveih     (501) staff       (20)      238 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      211 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)     1538 2024-02-09 13:14:36.000000 usdm-0.50.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      409 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      353 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/characteristic.py
--rw-r--r--   0 daveih     (501) staff       (20)      208 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      306 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/condition.py
--rw-r--r--   0 daveih     (501) staff       (20)      338 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/eligibility_criterion.py
--rw-r--r--   0 daveih     (501) staff       (20)      573 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      192 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      416 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/geographic_scope.py
--rw-r--r--   0 daveih     (501) staff       (20)      365 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/governance_date.py
--rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      213 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      195 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/masking.py
--rw-r--r--   0 daveih     (501) staff       (20)      362 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/narrative_content.py
--rw-r--r--   0 daveih     (501) staff       (20)      256 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      507 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/organization.py
--rw-r--r--   0 daveih     (501) staff       (20)      913 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/population_definition.py
--rw-r--r--   0 daveih     (501) staff       (20)      292 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      241 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/quantity.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/range.py
--rw-r--r--   0 daveih     (501) staff       (20)      209 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      589 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      171 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      899 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      523 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      499 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_amendment.py
--rw-r--r--   0 daveih     (501) staff       (20)      253 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_amendment_reason.py
--rw-r--r--   0 daveih     (501) staff       (20)      305 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      212 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     2236 2024-02-22 05:10:08.000000 usdm-0.50.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      298 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      549 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/study_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_protocol_document.py
--rw-r--r--   0 daveih     (501) staff       (20)      461 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_protocol_document_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      295 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_site.py
--rw-r--r--   0 daveih     (501) staff       (20)      199 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_title.py
--rw-r--r--   0 daveih     (501) staff       (20)      876 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/study_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      250 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/syntax_template.py
--rw-r--r--   0 daveih     (501) staff       (20)      422 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/syntax_template_dictionary.py
--rw-r--r--   0 daveih     (501) staff       (20)      505 2024-03-23 12:59:10.000000 usdm-0.50.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      203 2024-01-25 11:26:05.000000 usdm-0.50.0/src/usdm_model/transition_rule.py
--rw-r--r--   0 daveih     (501) staff       (20)      233 2024-03-29 05:18:23.000000 usdm-0.50.0/src/usdm_model/wrapper.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-04-20 07:43:09.773054 usdm-0.50.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    22464 2024-04-19 04:16:10.000000 usdm-0.50.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     1102 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      274 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     2684 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5360 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_cross_reference.py
--rw-r--r--   0 daveih     (501) staff       (20)     3035 2024-04-19 04:16:10.000000 usdm-0.50.0/tests/test_data_factory.py
--rw-r--r--   0 daveih     (501) staff       (20)     1521 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_document.py
--rw-r--r--   0 daveih     (501) staff       (20)      561 2024-04-19 04:16:10.000000 usdm-0.50.0/tests/test_document_elements.py
--rw-r--r--   0 daveih     (501) staff       (20)     4606 2024-04-19 14:44:40.000000 usdm-0.50.0/tests/test_document_macros.py
--rw-r--r--   0 daveih     (501) staff       (20)    10171 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_document_soa.py
--rw-r--r--   0 daveih     (501) staff       (20)     1413 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_document_template_plain.py
--rw-r--r--   0 daveih     (501) staff       (20)     1098 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_document_utility.py
--rw-r--r--   0 daveih     (501) staff       (20)      873 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     2278 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1311 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_export.py
--rw-r--r--   0 daveih     (501) staff       (20)     1486 2024-04-19 14:44:40.000000 usdm-0.50.0/tests/test_factory.py
--rw-r--r--   0 daveih     (501) staff       (20)      377 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_globals.py
--rw-r--r--   0 daveih     (501) staff       (20)     5048 2024-04-20 07:40:07.000000 usdm-0.50.0/tests/test_integration.py
--rw-r--r--   0 daveih     (501) staff       (20)     2143 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)     1768 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_iso_8601_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      437 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     1693 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     2293 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_quantity_type.py
--rw-r--r--   0 daveih     (501) staff       (20)     1251 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_range_type.py
--rw-r--r--   0 daveih     (501) staff       (20)     1905 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_activity_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5542 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_arm_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3317 2024-04-19 04:16:10.000000 usdm-0.50.0/tests/test_study_design_characteristic_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     7055 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_conditions_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)    10476 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_content_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4310 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_dictionary_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3750 2024-04-18 14:04:27.000000 usdm-0.50.0/tests/test_study_design_eligibility_criteria_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4901 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_encounter_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4206 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_epoch_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3226 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_indication_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5830 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_intervention_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4848 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_oe_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4503 2024-04-19 04:16:10.000000 usdm-0.50.0/tests/test_study_design_population_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4364 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_sites_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5029 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_design_timing_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     9759 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_identifiers_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     1400 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_study_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      199 2024-02-22 05:10:08.000000 usdm-0.50.0/tests/test_study_soa_v2_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      513 2024-04-18 13:50:02.000000 usdm-0.50.0/tests/test_utility.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.147137 usdm-0.51.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.51.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    40094 2024-05-15 06:00:26.146828 usdm-0.51.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    39406 2024-05-15 05:57:03.000000 usdm-0.51.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.51.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2024-05-15 06:00:26.147310 usdm-0.51.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      990 2024-05-15 05:47:48.000000 usdm-0.51.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.085305 usdm-0.51.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.146320 usdm-0.51.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    40094 2024-05-15 06:00:26.000000 usdm-0.51.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     8676 2024-05-15 06:00:26.000000 usdm-0.51.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2024-05-15 06:00:26.000000 usdm-0.51.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       88 2024-05-15 06:00:26.000000 usdm-0.51.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       40 2024-05-15 06:00:26.000000 usdm-0.51.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.088548 usdm-0.51.0/src/usdm_db/
+-rw-r--r--   0 daveih     (501) staff       (20)     3217 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_db/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1381 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_db/cross_reference.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.089420 usdm-0.51.0/src/usdm_db/document/
+-rw-r--r--   0 daveih     (501) staff       (20)       27 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/document/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)    13622 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/document/document.py
+-rw-r--r--   0 daveih     (501) staff       (20)      758 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/document/utility.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.090443 usdm-0.51.0/src/usdm_db/errors_and_logging/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/errors_and_logging/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      602 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/errors_and_logging/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      696 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/errors_and_logging/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1013 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/errors_and_logging/errors_and_logging.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.091043 usdm-0.51.0/src/usdm_db/fhir/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_db/fhir/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5910 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_db/fhir/from_fhir.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6258 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_db/fhir/to_fhir.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3331 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/neo4j_dict.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3608 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_db/timeline.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.096781 usdm-0.51.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)    13275 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      364 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)      456 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/base_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)    18660 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)    16463 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/cdisc_bc_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)      987 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7304 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)      523 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/code_base.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2680 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2987 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)       93 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.102162 usdm-0.51.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)   833791 2024-03-29 05:59:21.000000 usdm-0.51.0/src/usdm_excel/data/cdisc_bcs.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)   994684 2024-03-29 08:02:31.000000 usdm-0.51.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)     1771 2024-03-29 08:02:31.000000 usdm-0.51.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)    17843 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.104565 usdm-0.51.0/src/usdm_excel/document/
+-rw-r--r--   0 daveih     (501) staff       (20)      101 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/document/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5268 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/document/elements.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5834 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/document/macros.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5087 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/document/soa.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1065 2024-04-05 04:37:08.000000 usdm-0.51.0/src/usdm_excel/document/template_base.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4803 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/document/template_m11.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6608 2024-04-19 11:24:09.000000 usdm-0.51.0/src/usdm_excel/document/template_plain.py
+-rw-r--r--   0 daveih     (501) staff       (20)      658 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/document/utility.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.105537 usdm-0.51.0/src/usdm_excel/errors_and_logging/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/errors_and_logging/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      933 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/errors_and_logging/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      632 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/errors_and_logging/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1735 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/errors_and_logging/errors_and_logging.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1314 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/globals.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2040 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1250 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      883 2023-10-12 07:51:31.000000 usdm-0.51.0/src/usdm_excel/iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      376 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      804 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      200 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/other_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1501 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/quantity_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1604 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/range_type.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.105917 usdm-0.51.0/src/usdm_excel/study_design_activity_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.51.0/src/usdm_excel/study_design_activity_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1305 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.106310 usdm-0.51.0/src/usdm_excel/study_design_amendment_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.51.0/src/usdm_excel/study_design_amendment_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7916 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.106676 usdm-0.51.0/src/usdm_excel/study_design_arm_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.51.0/src/usdm_excel/study_design_arm_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1702 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.106984 usdm-0.51.0/src/usdm_excel/study_design_characteristics_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/study_design_characteristics_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1527 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/study_design_characteristics_sheet/study_design_characteristics_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.107334 usdm-0.51.0/src/usdm_excel/study_design_conditions_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-17 06:39:55.000000 usdm-0.51.0/src/usdm_excel/study_design_conditions_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2714 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.107634 usdm-0.51.0/src/usdm_excel/study_design_content_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:51:31.000000 usdm-0.51.0/src/usdm_excel/study_design_content_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3804 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.107970 usdm-0.51.0/src/usdm_excel/study_design_dictionary_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.51.0/src/usdm_excel/study_design_dictionary_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2966 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.108749 usdm-0.51.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2051 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.109717 usdm-0.51.0/src/usdm_excel/study_design_eligibility_criteria_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-01 11:43:59.000000 usdm-0.51.0/src/usdm_excel/study_design_eligibility_criteria_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1872 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.110533 usdm-0.51.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3005 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.111039 usdm-0.51.0/src/usdm_excel/study_design_epoch_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.51.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1342 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.111531 usdm-0.51.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3397 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.111836 usdm-0.51.0/src/usdm_excel/study_design_indication_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.51.0/src/usdm_excel/study_design_indication_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1125 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.112193 usdm-0.51.0/src/usdm_excel/study_design_intervention_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-11-27 15:49:16.000000 usdm-0.51.0/src/usdm_excel/study_design_intervention_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5431 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.112540 usdm-0.51.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3502 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.112870 usdm-0.51.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3964 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.113342 usdm-0.51.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1538 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.113713 usdm-0.51.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     9051 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.114163 usdm-0.51.0/src/usdm_excel/study_design_sites_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2024-01-02 13:11:00.000000 usdm-0.51.0/src/usdm_excel/study_design_sites_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2187 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_sites_sheet/study_design_sites_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.114776 usdm-0.51.0/src/usdm_excel/study_design_timing_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.51.0/src/usdm_excel/study_design_timing_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3851 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      819 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_design_timing_sheet/window_type.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.115230 usdm-0.51.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2074 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.115635 usdm-0.51.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.51.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     8990 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.118376 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-10-12 07:52:37.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      514 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4230 2024-04-19 14:44:40.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      686 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/conditons.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3872 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2494 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py
+-rw-r--r--   0 daveih     (501) staff       (20)      292 2023-10-12 07:52:37.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4035 2024-04-18 13:50:02.000000 usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/study_soa_v2_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1541 2024-04-19 04:16:10.000000 usdm-0.51.0/src/usdm_excel/syntax_template_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)       92 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_excel/template_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.118653 usdm-0.51.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       58 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.131967 usdm-0.51.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     2792 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      481 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      328 2024-03-29 08:02:31.000000 usdm-0.51.0/src/usdm_model/administration_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      420 2024-03-29 08:02:31.000000 usdm-0.51.0/src/usdm_model/agent_administration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      238 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      211 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1660 2024-05-15 05:47:48.000000 usdm-0.51.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      409 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      353 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      152 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/characteristic.py
+-rw-r--r--   0 daveih     (501) staff       (20)      208 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      306 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/condition.py
+-rw-r--r--   0 daveih     (501) staff       (20)      338 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/eligibility_criterion.py
+-rw-r--r--   0 daveih     (501) staff       (20)      573 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      192 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      414 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      416 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/geographic_scope.py
+-rw-r--r--   0 daveih     (501) staff       (20)      365 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/governance_date.py
+-rw-r--r--   0 daveih     (501) staff       (20)      259 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      213 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      195 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/masking.py
+-rw-r--r--   0 daveih     (501) staff       (20)      362 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/narrative_content.py
+-rw-r--r--   0 daveih     (501) staff       (20)      256 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      507 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/organization.py
+-rw-r--r--   0 daveih     (501) staff       (20)      913 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/population_definition.py
+-rw-r--r--   0 daveih     (501) staff       (20)      292 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      241 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/quantity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      262 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/range.py
+-rw-r--r--   0 daveih     (501) staff       (20)      209 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      589 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      171 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      899 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      523 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      499 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_amendment.py
+-rw-r--r--   0 daveih     (501) staff       (20)      253 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_amendment_reason.py
+-rw-r--r--   0 daveih     (501) staff       (20)      305 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      212 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2236 2024-02-22 05:10:08.000000 usdm-0.51.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      397 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      298 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      260 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      549 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/study_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_protocol_document.py
+-rw-r--r--   0 daveih     (501) staff       (20)      461 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_protocol_document_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      295 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_site.py
+-rw-r--r--   0 daveih     (501) staff       (20)      199 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_title.py
+-rw-r--r--   0 daveih     (501) staff       (20)      876 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/study_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      250 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/syntax_template.py
+-rw-r--r--   0 daveih     (501) staff       (20)      422 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/syntax_template_dictionary.py
+-rw-r--r--   0 daveih     (501) staff       (20)      505 2024-03-23 12:59:10.000000 usdm-0.51.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      203 2024-01-25 11:26:05.000000 usdm-0.51.0/src/usdm_model/transition_rule.py
+-rw-r--r--   0 daveih     (501) staff       (20)      233 2024-03-29 05:18:23.000000 usdm-0.51.0/src/usdm_model/wrapper.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2024-05-15 06:00:26.145901 usdm-0.51.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    22464 2024-04-19 04:16:10.000000 usdm-0.51.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1102 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      273 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4332 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5360 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_cross_reference.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1101 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_ct_version_manger.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3035 2024-04-19 04:16:10.000000 usdm-0.51.0/tests/test_data_factory.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1521 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_document.py
+-rw-r--r--   0 daveih     (501) staff       (20)      561 2024-04-19 04:16:10.000000 usdm-0.51.0/tests/test_document_elements.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4606 2024-04-19 14:44:40.000000 usdm-0.51.0/tests/test_document_macros.py
+-rw-r--r--   0 daveih     (501) staff       (20)    10171 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_document_soa.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1413 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_document_template_plain.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1098 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_document_utility.py
+-rw-r--r--   0 daveih     (501) staff       (20)      873 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2278 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1486 2024-04-19 14:44:40.000000 usdm-0.51.0/tests/test_factory.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2018 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_from_fhir.py
+-rw-r--r--   0 daveih     (501) staff       (20)      418 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_globals.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6919 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_integration.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2143 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1768 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      437 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1284 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2293 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_quantity_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1251 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_range_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1905 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_activity_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5542 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_arm_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3317 2024-04-19 04:16:10.000000 usdm-0.51.0/tests/test_study_design_characteristic_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7055 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_conditions_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)    11120 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_study_design_content_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4299 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_study_design_dictionary_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3750 2024-04-18 14:04:27.000000 usdm-0.51.0/tests/test_study_design_eligibility_criteria_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4901 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_encounter_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4206 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_epoch_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3194 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_study_design_indication_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5830 2024-05-01 15:49:26.000000 usdm-0.51.0/tests/test_study_design_intervention_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4848 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_oe_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4503 2024-04-19 04:16:10.000000 usdm-0.51.0/tests/test_study_design_population_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4364 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_sites_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5029 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_design_timing_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     9759 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_identifiers_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1400 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_study_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      199 2024-02-22 05:10:08.000000 usdm-0.51.0/tests/test_study_soa_v2_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1066 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_template_manger.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3297 2024-05-15 05:47:48.000000 usdm-0.51.0/tests/test_to_fhir.py
+-rw-r--r--   0 daveih     (501) staff       (20)      513 2024-04-18 13:50:02.000000 usdm-0.51.0/tests/test_utility.py
```

### Comparing `usdm-0.50.0/LICENSE` & `usdm-0.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/PKG-INFO` & `usdm-0.51.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: usdm
-Version: 0.50.0
-Summary: A python package for using the CDISC TransCelerate USDM
-Author: D Iberson-Hurst
-Author-email: 
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: openpyxl
-Requires-Dist: pydantic
-Requires-Dist: requests
-Requires-Dist: stringcase
-Requires-Dist: yattag
-Requires-Dist: docraptor
-Requires-Dist: bs4
-Requires-Dist: pyyaml
-
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -660,15 +637,17 @@
 | E | transitionStartRule | Start rule | Text string |	
 | F | transitionEndRule | End rule | Text string |
 
 ### Study Design Content sheet
 
 #### Sheet Name
 
-`studyDesignContent`
+default name: `studyDesignContent`
+
+Several content sheets can be included within the workbook and named as desired. Typical use might be the inclusion of a sponsor protocol format and the new M11 format
 
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, containing the narrative content: 
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
@@ -683,28 +662,31 @@
 
 | Macro Name | Purpose | Attributes |
 | :--- | :--- | :--- |
 | xref | Refer to a data element by name reference | 'klass', 'name' and 'attribute'. The name is the name used within the workbook to define the content. |
 | image | Insert an mage into the document | 'file' and 'type'. The file attribute specifies the name of a file in the same directory as the Excel workbook. |
 | element | Refer to a predefined element | 'name' of the element. Supported element names are 'study_phase', 'study_short_title', 'study_full_title', 'study_acronym', 'study_rationale', 'study_version_identifier', 'study_identifier', 'study_regulatory_identifiers', 'study_date', 'approval_date', 'organization_name_and_address', 'amendment' and 'amendment_scope' |
 | section | Add a pre defined section into the document | 'name' and 'template'. Supported section are 'title_page', 'inclusion', 'exclusion' and 'objective_endpoints'. Supported templates are 'm11' and 'plain' |
+| bc | Add in a reference to a BC | 'name' and 'activity' where the name is the name of the BC as used in the SoA and activity is the name of the activity it is referenced from (in case several activities reference the same BC). This macro is needed as the BCs are not explicitly defined and thus named, they are read from the CDISC library and can appear multiple times. |
 | note | Insert a note into the document | 'text' |
 
 Examples of macros are:
 
 ```<usdm:macro id="xref" klass="Objective" name="OBJ1" attribute="text"/>```
 
 ```<usdm:macro id="xref" klass="StudyDesignPopulation" name="STUDY_POP" attribute="@plannedCompletionNumber/Range/maxValue"/>```
 
 ```<usdm:macro id="element" name="study_identifier"/>```
 
 ```<usdm:macro id="image" file="design.png" type="png"/>```
 
 ```<usdm:macro id="section" name="inclusion" template="plain"/>```
 
+```<usdm:macro id="bc" name="Body temperature" activity="Vital signs / Temperature">```
+
 ```<usdm:macro id="note" text="A note here please"/>```
 
 ### Study Design Sites sheet
 
 #### Sheet Name
 
 `studyDesignSites`
@@ -779,22 +761,51 @@
 
 #### Sheet Contents
 
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
-| CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
+| CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form ctName = Version, for example `SNOMED = 21st June 2012`|
 | Empty None | Allows for string fields to be set to '' rather than null/none values so as to accomodate the SDR validation checks | Set to 'EMPTY' to use ''. Any other value will permit  null values to be used |
+| Template | Configures a protocol template and the associated studyDesignContent sheet | Entries take the form of templateName = sheetName, for example `Sponsor = sponsorContent`. The template name and the sheet name are simple strings. Template names are at the user's discretion but the string `m11` or `M11` is reserved as the template name for the M11 Template format. The sheet name must match a sheet within the workbook that must be structured as per the studyDesignContent sheet format. |
+| Use Template | Indicates which template is to be used | The value should match one of the names defined using the Template configuration parameter |
+| USDM Version | Deprecated | Deprecated |
 | SDR Prev Next | Deprecated | Deprecated |
 | SDR Root | Deprecated | Deprecated |
 | SDR Description | Deprecated | Deprecated |
 
+An example configuration is
+
+| First Column | Second Column |
+| :--- | :--- | 
+| CT Version | SNOMED=January 31, 2018 |
+| CT Version | SPONSOR =   12 |
+| CT Version | ICD-10=1 |
+| Template | lilly=lillyFormat |
+| Template | m11=m11Format |
+| Use Template | m11 |
+
+This sets up three CT versions and two templates. The M11 template will be used.
+
 # Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
 
 # Build Notes
 
-Build with `python3 -m build --sdist --wheel`
+## Checklist
+
+1. Everything on main branch?
+1. Readme updated with any necessary changes?
+1. Version updated?
+1. All tests passing?
+
+Then
+
+1. Build and upload
+1. Write release note
+
+## Build steps for deployment to pypi.org
 
-Upload to pypi using `twine upload dist/* `
+- Build with `python3 -m build --sdist --wheel`
+- Upload to pypi.org using `twine upload dist/* `
```

### Comparing `usdm-0.50.0/README.md` & `usdm-0.51.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: usdm
+Version: 0.51.0
+Summary: A python package for using the CDISC TransCelerate USDM
+Author: D Iberson-Hurst
+Author-email: 
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: openpyxl
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: stringcase
+Requires-Dist: yattag
+Requires-Dist: docraptor
+Requires-Dist: bs4
+Requires-Dist: pyyaml
+Requires-Dist: fhir.resources
+
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -637,15 +661,17 @@
 | E | transitionStartRule | Start rule | Text string |	
 | F | transitionEndRule | End rule | Text string |
 
 ### Study Design Content sheet
 
 #### Sheet Name
 
-`studyDesignContent`
+default name: `studyDesignContent`
+
+Several content sheets can be included within the workbook and named as desired. Typical use might be the inclusion of a sponsor protocol format and the new M11 format
 
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, containing the narrative content: 
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
@@ -660,28 +686,31 @@
 
 | Macro Name | Purpose | Attributes |
 | :--- | :--- | :--- |
 | xref | Refer to a data element by name reference | 'klass', 'name' and 'attribute'. The name is the name used within the workbook to define the content. |
 | image | Insert an mage into the document | 'file' and 'type'. The file attribute specifies the name of a file in the same directory as the Excel workbook. |
 | element | Refer to a predefined element | 'name' of the element. Supported element names are 'study_phase', 'study_short_title', 'study_full_title', 'study_acronym', 'study_rationale', 'study_version_identifier', 'study_identifier', 'study_regulatory_identifiers', 'study_date', 'approval_date', 'organization_name_and_address', 'amendment' and 'amendment_scope' |
 | section | Add a pre defined section into the document | 'name' and 'template'. Supported section are 'title_page', 'inclusion', 'exclusion' and 'objective_endpoints'. Supported templates are 'm11' and 'plain' |
+| bc | Add in a reference to a BC | 'name' and 'activity' where the name is the name of the BC as used in the SoA and activity is the name of the activity it is referenced from (in case several activities reference the same BC). This macro is needed as the BCs are not explicitly defined and thus named, they are read from the CDISC library and can appear multiple times. |
 | note | Insert a note into the document | 'text' |
 
 Examples of macros are:
 
 ```<usdm:macro id="xref" klass="Objective" name="OBJ1" attribute="text"/>```
 
 ```<usdm:macro id="xref" klass="StudyDesignPopulation" name="STUDY_POP" attribute="@plannedCompletionNumber/Range/maxValue"/>```
 
 ```<usdm:macro id="element" name="study_identifier"/>```
 
 ```<usdm:macro id="image" file="design.png" type="png"/>```
 
 ```<usdm:macro id="section" name="inclusion" template="plain"/>```
 
+```<usdm:macro id="bc" name="Body temperature" activity="Vital signs / Temperature">```
+
 ```<usdm:macro id="note" text="A note here please"/>```
 
 ### Study Design Sites sheet
 
 #### Sheet Name
 
 `studyDesignSites`
@@ -756,22 +785,51 @@
 
 #### Sheet Contents
 
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
-| CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
+| CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form ctName = Version, for example `SNOMED = 21st June 2012`|
 | Empty None | Allows for string fields to be set to '' rather than null/none values so as to accomodate the SDR validation checks | Set to 'EMPTY' to use ''. Any other value will permit  null values to be used |
+| Template | Configures a protocol template and the associated studyDesignContent sheet | Entries take the form of templateName = sheetName, for example `Sponsor = sponsorContent`. The template name and the sheet name are simple strings. Template names are at the user's discretion but the string `m11` or `M11` is reserved as the template name for the M11 Template format. The sheet name must match a sheet within the workbook that must be structured as per the studyDesignContent sheet format. |
+| Use Template | Indicates which template is to be used | The value should match one of the names defined using the Template configuration parameter |
+| USDM Version | Deprecated | Deprecated |
 | SDR Prev Next | Deprecated | Deprecated |
 | SDR Root | Deprecated | Deprecated |
 | SDR Description | Deprecated | Deprecated |
 
+An example configuration is
+
+| First Column | Second Column |
+| :--- | :--- | 
+| CT Version | SNOMED=January 31, 2018 |
+| CT Version | SPONSOR =   12 |
+| CT Version | ICD-10=1 |
+| Template | lilly=lillyFormat |
+| Template | m11=m11Format |
+| Use Template | m11 |
+
+This sets up three CT versions and two templates. The M11 template will be used.
+
 # Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
 
 # Build Notes
 
-Build with `python3 -m build --sdist --wheel`
+## Checklist
+
+1. Everything on main branch?
+1. Readme updated with any necessary changes?
+1. Version updated?
+1. All tests passing?
+
+Then
+
+1. Build and upload
+1. Write release note
+
+## Build steps for deployment to pypi.org
 
-Upload to pypi using `twine upload dist/* `
+- Build with `python3 -m build --sdist --wheel`
+- Upload to pypi.org using `twine upload dist/* `
```

### Comparing `usdm-0.50.0/setup.py` & `usdm-0.51.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   name="usdm",
   version=version['__package_version__'],
   author="D Iberson-Hurst",
   author_email="",
   description="A python package for using the CDISC TransCelerate USDM",
   long_description=long_description,
   long_description_content_type="text/markdown",
-  install_requires=['pandas', 'openpyxl', 'pydantic', 'requests', 'stringcase', 'yattag', 'docraptor', 'bs4', 'pyyaml'],
+  install_requires=['pandas', 'openpyxl', 'pydantic', 'requests', 'stringcase', 'yattag', 'docraptor', 'bs4', 'pyyaml', 'fhir.resources'],
   packages=setuptools.find_packages(where="src"),
   package_dir={"": "src"},
   package_data={"usdm_excel": ["data/*.yaml", "data/*.json"]},
   tests_require=['pytest'],
   classifiers=[
     "Intended Audience :: Developers",
     "Programming Language :: Python",
```

### Comparing `usdm-0.50.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.51.0/src/usdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.50.0
+Version: 0.51.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,15 @@
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: stringcase
 Requires-Dist: yattag
 Requires-Dist: docraptor
 Requires-Dist: bs4
 Requires-Dist: pyyaml
+Requires-Dist: fhir.resources
 
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
@@ -660,15 +661,17 @@
 | E | transitionStartRule | Start rule | Text string |	
 | F | transitionEndRule | End rule | Text string |
 
 ### Study Design Content sheet
 
 #### Sheet Name
 
-`studyDesignContent`
+default name: `studyDesignContent`
+
+Several content sheets can be included within the workbook and named as desired. Typical use might be the inclusion of a sponsor protocol format and the new M11 format
 
 #### Sheet Contents
 
 A header row in row 1 followed by repeating rows from row 2, containing the narrative content: 
 
 | Column | Column Name | Purpose | Format and Values |
 | :--- | :--- | :--- | :--- |
@@ -683,28 +686,31 @@
 
 | Macro Name | Purpose | Attributes |
 | :--- | :--- | :--- |
 | xref | Refer to a data element by name reference | 'klass', 'name' and 'attribute'. The name is the name used within the workbook to define the content. |
 | image | Insert an mage into the document | 'file' and 'type'. The file attribute specifies the name of a file in the same directory as the Excel workbook. |
 | element | Refer to a predefined element | 'name' of the element. Supported element names are 'study_phase', 'study_short_title', 'study_full_title', 'study_acronym', 'study_rationale', 'study_version_identifier', 'study_identifier', 'study_regulatory_identifiers', 'study_date', 'approval_date', 'organization_name_and_address', 'amendment' and 'amendment_scope' |
 | section | Add a pre defined section into the document | 'name' and 'template'. Supported section are 'title_page', 'inclusion', 'exclusion' and 'objective_endpoints'. Supported templates are 'm11' and 'plain' |
+| bc | Add in a reference to a BC | 'name' and 'activity' where the name is the name of the BC as used in the SoA and activity is the name of the activity it is referenced from (in case several activities reference the same BC). This macro is needed as the BCs are not explicitly defined and thus named, they are read from the CDISC library and can appear multiple times. |
 | note | Insert a note into the document | 'text' |
 
 Examples of macros are:
 
 ```<usdm:macro id="xref" klass="Objective" name="OBJ1" attribute="text"/>```
 
 ```<usdm:macro id="xref" klass="StudyDesignPopulation" name="STUDY_POP" attribute="@plannedCompletionNumber/Range/maxValue"/>```
 
 ```<usdm:macro id="element" name="study_identifier"/>```
 
 ```<usdm:macro id="image" file="design.png" type="png"/>```
 
 ```<usdm:macro id="section" name="inclusion" template="plain"/>```
 
+```<usdm:macro id="bc" name="Body temperature" activity="Vital signs / Temperature">```
+
 ```<usdm:macro id="note" text="A note here please"/>```
 
 ### Study Design Sites sheet
 
 #### Sheet Name
 
 `studyDesignSites`
@@ -779,22 +785,51 @@
 
 #### Sheet Contents
 
 A set of rows consisting of configuration parameters. The first column is the type of configuration parameter while the second is the value. The values for specific parameters may vary in their format
 
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
-| CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
+| CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form ctName = Version, for example `SNOMED = 21st June 2012`|
 | Empty None | Allows for string fields to be set to '' rather than null/none values so as to accomodate the SDR validation checks | Set to 'EMPTY' to use ''. Any other value will permit  null values to be used |
+| Template | Configures a protocol template and the associated studyDesignContent sheet | Entries take the form of templateName = sheetName, for example `Sponsor = sponsorContent`. The template name and the sheet name are simple strings. Template names are at the user's discretion but the string `m11` or `M11` is reserved as the template name for the M11 Template format. The sheet name must match a sheet within the workbook that must be structured as per the studyDesignContent sheet format. |
+| Use Template | Indicates which template is to be used | The value should match one of the names defined using the Template configuration parameter |
+| USDM Version | Deprecated | Deprecated |
 | SDR Prev Next | Deprecated | Deprecated |
 | SDR Root | Deprecated | Deprecated |
 | SDR Description | Deprecated | Deprecated |
 
+An example configuration is
+
+| First Column | Second Column |
+| :--- | :--- | 
+| CT Version | SNOMED=January 31, 2018 |
+| CT Version | SPONSOR =   12 |
+| CT Version | ICD-10=1 |
+| Template | lilly=lillyFormat |
+| Template | m11=m11Format |
+| Use Template | m11 |
+
+This sets up three CT versions and two templates. The M11 template will be used.
+
 # Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
 
 # Build Notes
 
-Build with `python3 -m build --sdist --wheel`
+## Checklist
+
+1. Everything on main branch?
+1. Readme updated with any necessary changes?
+1. Version updated?
+1. All tests passing?
+
+Then
+
+1. Build and upload
+1. Write release note
+
+## Build steps for deployment to pypi.org
 
-Upload to pypi using `twine upload dist/* `
+- Build with `python3 -m build --sdist --wheel`
+- Upload to pypi.org using `twine upload dist/* `
```

### Comparing `usdm-0.50.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.51.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,20 @@
 src/usdm_db/document/__init__.py
 src/usdm_db/document/document.py
 src/usdm_db/document/utility.py
 src/usdm_db/errors_and_logging/__init__.py
 src/usdm_db/errors_and_logging/error.py
 src/usdm_db/errors_and_logging/errors.py
 src/usdm_db/errors_and_logging/errors_and_logging.py
+src/usdm_db/fhir/__init__.py
+src/usdm_db/fhir/from_fhir.py
+src/usdm_db/fhir/to_fhir.py
 src/usdm_excel/__init__.py
 src/usdm_excel/alias.py
+src/usdm_excel/base_manager.py
 src/usdm_excel/base_sheet.py
 src/usdm_excel/cdisc_bc_library.py
 src/usdm_excel/cdisc_ct.py
 src/usdm_excel/cdisc_ct_library.py
 src/usdm_excel/code_base.py
 src/usdm_excel/configuration_sheet.py
 src/usdm_excel/cross_ref.py
@@ -34,14 +38,15 @@
 src/usdm_excel/iso_8601_duration.py
 src/usdm_excel/ncit.py
 src/usdm_excel/option_manager.py
 src/usdm_excel/other_ct.py
 src/usdm_excel/quantity_type.py
 src/usdm_excel/range_type.py
 src/usdm_excel/syntax_template_sheet.py
+src/usdm_excel/template_manager.py
 src/usdm_excel/data/cdisc_bcs.yaml
 src/usdm_excel/data/cdisc_ct_2023-12-15.yaml
 src/usdm_excel/data/cdisc_ct_config.yaml
 src/usdm_excel/data/iso_3166.json
 src/usdm_excel/data/missing_ct.yaml
 src/usdm_excel/document/__init__.py
 src/usdm_excel/document/elements.py
@@ -165,25 +170,26 @@
 src/usdm_model/transition_rule.py
 src/usdm_model/wrapper.py
 tests/test_base_sheet.py
 tests/test_cdisc_biomedical_concept.py
 tests/test_cdisc_ct.py
 tests/test_configuration_sheet.py
 tests/test_cross_reference.py
+tests/test_ct_version_manger.py
 tests/test_data_factory.py
 tests/test_document.py
 tests/test_document_elements.py
 tests/test_document_macros.py
 tests/test_document_soa.py
 tests/test_document_template_plain.py
 tests/test_document_utility.py
 tests/test_error.py
 tests/test_errors.py
-tests/test_export.py
 tests/test_factory.py
+tests/test_from_fhir.py
 tests/test_globals.py
 tests/test_integration.py
 tests/test_iso_3166.py
 tests/test_iso_8601_duration.py
 tests/test_ncit.py
 tests/test_option_manager.py
 tests/test_quantity_type.py
@@ -202,8 +208,10 @@
 tests/test_study_design_oe_sheet.py
 tests/test_study_design_population_sheet.py
 tests/test_study_design_sites_sheet.py
 tests/test_study_design_timing_sheet.py
 tests/test_study_identifiers_sheet.py
 tests/test_study_sheet.py
 tests/test_study_soa_v2_sheet.py
+tests/test_template_manger.py
+tests/test_to_fhir.py
 tests/test_utility.py
```

### Comparing `usdm-0.50.0/src/usdm_db/__init__.py` & `usdm-0.51.0/src/usdm_db/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import json
 import traceback
+from uuid import uuid4
 from usdm_excel import USDMExcel
 from usdm_model.wrapper import Wrapper
 from usdm_db.document.document import Document
+from usdm_db.fhir.to_fhir import ToFHIR
+from usdm_db.fhir.from_fhir import FromFHIR
 from usdm_db.errors_and_logging.errors_and_logging import ErrorsAndLogging
 from usdm_db.neo4j_dict import Neo4jDict
 from usdm_db.timeline import Timeline
 
 class USDMDb():
 
   SYSTEM_NAME = "CDISC E2J"
@@ -27,27 +30,46 @@
   
   def excel(self):
     return self._excel
 
   def from_json(self, data):
     self._wrapper = Wrapper.model_validate(data)
     
-  def from_excel(self, file_path):
+  def from_excel(self, file_path, override_template: str = None):
     self._excel = USDMExcel(file_path)
-    self._wrapper = self._excel.execute()
+    self._wrapper = self._excel.execute(override_template)
     return self._excel.errors()
 
+  def from_fhir(self, data: str):
+    fhir = FromFHIR(self._errors_and_logging)
+    self._wrapper = fhir.from_fhir(data)
+    return True
+  
+  def was_m11(self) -> bool:
+    return self._excel.was_m11()
+  
   def to_json(self):
     try:
       raw_json = self._wrapper.to_json()
     except Exception as e:
       message = self._format_exception("Failed to generate JSON output", e)
       raw_json = json.dumps({'error': message}, indent = 2)
     return raw_json
 
+  def to_fhir(self):
+    try:
+      study = self._wrapper.study
+      title = self._get_title()
+      fhir = ToFHIR(title, study, self._errors_and_logging)
+      raw_json = fhir.to_fhir(uuid4())
+    except Exception as e:
+      message = self._format_exception("Failed to generate FHIR output", e)
+      raw_json = json.dumps({'error': message}, indent = 2)
+    return raw_json
+
   def to_html(self, highlight=False):
     try:
       study = self._wrapper.study
       title = self._get_title()
       doc = Document(title, study, self._errors_and_logging)
       html = doc.to_html(highlight)
     except Exception as e:
```

### Comparing `usdm-0.50.0/src/usdm_db/cross_reference.py` & `usdm-0.51.0/src/usdm_db/cross_reference.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import logging
 from datetime import date
+from uuid import UUID
 from usdm_db.errors_and_logging.errors_and_logging import ErrorsAndLogging
 
 class CrossReference():
 
   def __init__(self, study, errors_and_logging: ErrorsAndLogging):
     self._errors_and_logging = errors_and_logging
     self._study = study
     self._references = {}
     self._logger = logging.getLogger(__name__)
     self._process_node(self._study)
 
-  # def clear(self):
-  #   self._references = {}
-  
   def get(self, klass, id):
     key = self._key(klass, id)
     if key in self._references:
       return self._references[key]
     else:
       return None
 
-  # def dump(self):
-  #   print(f"\n\n\nREFERENCES\n\n{self._references.keys()}")
-
   def _process_node(self, node):
     if type(node) == list:
       if node:
         for item in node:
           self._process_node(item) 
     elif type(node) == str:
       pass
     elif type(node) == float:
       pass
     elif type(node) == date:
       pass
     elif type(node) == bool:
       pass
+    elif type(node) == UUID:
+      pass
     elif node is None:
       pass
     else:
       if hasattr(node, 'instanceType'):
         key = self._key(node.instanceType, node.id)
         self._references[key] = node
       for name, field in node.model_fields.items():
```

### Comparing `usdm-0.50.0/src/usdm_db/document/document.py` & `usdm-0.51.0/src/usdm_db/document/document.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_db/document/utility.py` & `usdm-0.51.0/src/usdm_db/document/utility.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_db/errors_and_logging/error.py` & `usdm-0.51.0/src/usdm_db/errors_and_logging/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_db/errors_and_logging/errors.py` & `usdm-0.51.0/src/usdm_db/errors_and_logging/errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_db/errors_and_logging/errors_and_logging.py` & `usdm-0.51.0/src/usdm_db/errors_and_logging/errors_and_logging.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_db/neo4j_dict.py` & `usdm-0.51.0/src/usdm_db/neo4j_dict.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_db/timeline.py` & `usdm-0.51.0/src/usdm_db/timeline.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/__init__.py` & `usdm-0.51.0/src/usdm_excel/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,26 +40,36 @@
   STUDY_VERSION_DATE = 'study_version'
   PROTOCOL_VERSION_DATE = 'protocol_document'
 
   def __init__(self, file_path):
     self._globals = Globals()
     self._file_path = file_path
 
-  def execute(self):
+  def execute(self, template_override: str = None):
     self._globals.create()
-    return self._process()
+    return self._process(template_override)
 
   def errors(self):
     return self._globals.errors_and_logging.errors().dump(Errors.WARNING)
   
-  def _process(self):
+  def was_m11(self):
+    return self._globals.option_manager.get(Options.USE_TEMPLATE) == "M11"
+  
+  def _process(self, template_override: str = None):
     try:
     
-      # Process all the sheets
+      # Read the configuration. Override the template if requested and present, otherwise leave as configured
       self.configuration = ConfigurationSheet(self._file_path, self._globals)
+      if template_override:
+        sheet_name = self._globals.template_manager.get(template_override)
+        if sheet_name:
+          self._globals.option_manager.set(Options.USE_TEMPLATE, template_override.upper())
+          self._globals.errors_and_logging.info(f"Template overridden. Using template '{template_override}' and sheet '{sheet_name}'")
+
+      # Process all the remaining sheets
       self.study = StudySheet(self._file_path, self._globals)
       self.timings = StudyDesignTimingSheet(self._file_path, self._globals)
       self.study_amendments = StudyDesignAmendmentSheet(self._file_path, self._globals)
       self.study_identifiers = StudyIdentifiersSheet(self._file_path, self._globals)
       self.procedures = StudyDesignProcedureSheet(self._file_path, self._globals)
       self.encounters = StudyDesignEncounterSheet(self._file_path, self._globals)
       self.elements = StudyDesignElementSheet(self._file_path, self._globals)
```

### Comparing `usdm-0.50.0/src/usdm_excel/base_sheet.py` & `usdm-0.51.0/src/usdm_excel/base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/cdisc_bc_library.py` & `usdm-0.51.0/src/usdm_excel/cdisc_bc_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.51.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.51.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/code_base.py` & `usdm-0.51.0/src/usdm_excel/code_base.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/cross_ref.py` & `usdm-0.51.0/src/usdm_excel/cross_ref.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/data/cdisc_bcs.yaml` & `usdm-0.51.0/src/usdm_excel/data/cdisc_bcs.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml` & `usdm-0.51.0/src/usdm_excel/data/cdisc_ct_2023-12-15.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.51.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.51.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.51.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/document/elements.py` & `usdm-0.51.0/src/usdm_excel/document/elements.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/document/macros.py` & `usdm-0.51.0/src/usdm_excel/document/macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,20 @@
         self.parent._general_error(f"Failed to find BC name '{bc_name}' in activity '{activity_name}'")
         ref.replace_with('Missing BC: failed to find BC in activity')
     else:
       self.parent._general_error(f"Failed to find  activity '{activity_name}'")
       ref.replace_with('Missing activity: failed to find activity')
 
   def _image(self, attributes, soup, ref) -> None:
-    type = {attributes['type']}
+    type = attributes['type']
     data = self._encode_image(attributes['file'])
     if data:
       img_tag = soup.new_tag("img")
       img_tag.attrs['src'] = f"data:image/{type};base64,{data.decode('ascii')}"
+      img_tag.attrs['alt'] = "Alt text"
       ref.replace_with(img_tag)
     else:
       self._note({'text': f"Failed to insert image '{attributes['file']}', ignoring!"}, soup, ref)
 
   def _element(self, attributes, soup, ref) -> None:
     method = attributes['name'].lower()
     if self.elements.valid_method(method):
```

### Comparing `usdm-0.50.0/src/usdm_excel/document/soa.py` & `usdm-0.51.0/src/usdm_excel/document/soa.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/document/template_base.py` & `usdm-0.51.0/src/usdm_excel/document/template_base.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/document/template_m11.py` & `usdm-0.51.0/src/usdm_excel/document/template_m11.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/document/template_plain.py` & `usdm-0.51.0/src/usdm_excel/document/template_plain.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/document/utility.py` & `usdm-0.51.0/src/usdm_excel/document/utility.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/errors_and_logging/error.py` & `usdm-0.51.0/src/usdm_excel/errors_and_logging/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/errors_and_logging/errors.py` & `usdm-0.51.0/src/usdm_excel/errors_and_logging/errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/errors_and_logging/errors_and_logging.py` & `usdm-0.51.0/src/usdm_excel/errors_and_logging/errors_and_logging.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/globals.py` & `usdm-0.51.0/src/usdm_excel/globals.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from usdm_excel.id_manager import IdManager
 from usdm_excel.cross_ref import CrossRef
 from usdm_excel.ct_version_manager import CTVersionManager
+from usdm_excel.template_manager import TemplateManager
 from usdm_excel.errors_and_logging.errors_and_logging import ErrorsAndLogging
 from usdm_excel.option_manager import OptionManager
 from usdm_excel.cdisc_ct_library import CDISCCTLibrary
 from usdm_excel.cdisc_bc_library import CDISCBCLibrary
 
 class Globals():
 
   def __init__(self):
     self.errors_and_logging = None
     self.id_manager = None
     self.ct_version_manager = None
+    self.template_manager = None
     self.option_manager = None
     self.cross_references = None
     self.cdisc_ct_library = None
     self.cdisc_bc_library = None
 
   def create(self):
     self.errors_and_logging = ErrorsAndLogging()
     self.id_manager = IdManager(self.errors_and_logging)
     self.ct_version_manager = CTVersionManager(self.errors_and_logging)
+    self.template_manager = TemplateManager(self.errors_and_logging)
     self.option_manager = OptionManager(self.errors_and_logging)
     self.cross_references = CrossRef(self.errors_and_logging)
     self.cdisc_ct_library = CDISCCTLibrary(self.errors_and_logging)
     self.cdisc_bc_library = CDISCBCLibrary(self.errors_and_logging, self.cdisc_ct_library, self.id_manager)
```

### Comparing `usdm-0.50.0/src/usdm_excel/id_manager.py` & `usdm-0.51.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/iso_3166.py` & `usdm-0.51.0/src/usdm_excel/iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/iso_8601_duration.py` & `usdm-0.51.0/src/usdm_excel/iso_8601_duration.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/option_manager.py` & `usdm-0.51.0/src/usdm_excel/option_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from usdm_excel.errors_and_logging.errors_and_logging import ErrorsAndLogging
 from enum import Enum
 
 class Options(Enum):
   EMPTY_NONE = 'empty_none'
-  USDM_VERSION = 'usdm_version'
+  USE_TEMPLATE = 'use_template'
 
 class EmptyNoneOption(Enum):
   EMPTY = 'empty_string'
   NONE = 'none_value'
 
 class OptionManager():
 
@@ -21,19 +21,13 @@
   def set(self, name, value):
     name = self._to_string(name)
     value = self._to_string(value)
     self._items[name] = value
 
   def get(self, name):
     name = self._to_string(name)
-    if name in self._items:
-      return self._items[name]
-    else:
-      return ""
+    return self._items[name] if name in self._items else ''
   
   def _to_string(self, item):
-    if isinstance(item, Enum):
-      return item.value
-    else:
-      return str(item)
+    return item.value if isinstance(item, Enum) else str(item)
```

### Comparing `usdm-0.50.0/src/usdm_excel/quantity_type.py` & `usdm-0.51.0/src/usdm_excel/quantity_type.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/range_type.py` & `usdm-0.51.0/src/usdm_excel/range_type.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_amendment_sheet/study_design_amendment_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_characteristics_sheet/study_design_characteristics_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_characteristics_sheet/study_design_characteristics_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_conditions_sheet/study_design_conditions_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_content_sheet/study_design_content_sheet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-import traceback
 from usdm_excel.base_sheet import BaseSheet
+from usdm_excel.option_manager import Options
 from usdm_model.narrative_content import NarrativeContent
 from usdm_excel.globals import Globals
 from usdm_excel.document.macros import Macros
 
 class StudyDesignContentSheet(BaseSheet):
 
-  SHEET_NAME = 'studyDesignContent'
+  #SHEET_NAME = 'studyDesignContent'
+  DIV_OPEN_NS = '<div xmlns="http://www.w3.org/1999/xhtml">'
+  DIV_OPEN = '<div>'
+  DIV_CLOSE = '</div>'
 
   def __init__(self, file_path: str, globals: Globals):
     try:
       self.items = []
-      super().__init__(file_path=file_path, globals=globals, sheet_name=self.SHEET_NAME, optional=True, converters={"sectionName": str})
+      template = globals.option_manager.get(Options.USE_TEMPLATE)
+      sheet_name = globals.template_manager.get(template)
+      globals.errors_and_logging.info(f"About to read content sheet '{sheet_name}' based on template '{template}'")  
+      super().__init__(file_path=file_path, globals=globals, sheet_name=sheet_name, optional=True, converters={"sectionName": str})
       if self.success:
         current_level = 0
         new_level = 0
         current_parent = []
         previous_item = NarrativeContent(
           id=self.globals.id_manager.build_id(NarrativeContent), 
           name="ROOT",
@@ -77,9 +83,14 @@
 
   def _get_level(self, section_number):
     sn = section_number[:-1] if section_number.endswith('.') else section_number
     parts = sn.split('.')
     return len(parts)
 
   def _wrap_div(self, text):
-    return text if text.startswith("<div>") else f"<div>{text}</div>"
+    if text.startswith(self.DIV_OPEN_NS):
+      return text
+    elif text.startswith(self.DIV_OPEN):
+      return text.replace(self.DIV_OPEN, self.DIV_OPEN_NS)
+    else:
+      return f'{self.DIV_OPEN_NS}{text}{self.DIV_CLOSE}'
```

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_dictionary_sheet/study_design_dictionary_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
               col = self.column_present(['attribute', 'path'])
               self._error(index, col, str(e))
             if instance:
               map = self.create_object(ParameterMap, {'tag': key, 'reference': f'<usdm:ref klass="{instance.__class__.__name__}" id="{instance.id}" attribute="{attribute}"></usdm:ref>'})
               if map:
                 current_map.append(map)
           else:
-            map = self.create_object(ParameterMap, {'tag': key, 'reference': f"<div>{value}</div>"})
+            map = self.create_object(ParameterMap, {'tag': key, 'reference': f'{value}'})
             if map:
               current_map.append(map)
         # Clean up last dictionary if present
         if current_dictionary:
           current_dictionary.parameterMaps = current_map
         
     except Exception as e:
```

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_eligibility_criteria_sheet/study_design_eligibility_criteria_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_indication_sheet/study_design_indication_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_intervention_sheet/study_design_intervention_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,29 +201,29 @@
       return result
     except Exception as e:
       self._general_error("Failed to create StudyDesign object", e)
       return None
   
 
   def _set_masking(self, rindex, cindex):
-    if self.globals.option_manager.get(Options.USDM_VERSION) == '2':
-      return None
-    else:
-      try:
-        text = self.read_cell(rindex, cindex)
-        parts = text.split('=')
-        if len(parts) == 2: 
-          code = CDISCCT(self.globals).code_for_attribute('Masking', 'role', parts[0].strip())
-          if code:
-            mask = Masking(id=self.globals.id_manager.build_id(Masking), description=parts[1].strip(), role=code)
-            self.masks.append(mask)
-            self.globals.cross_references.add(mask.id, mask)
-            return mask
-          else:
-            self._error(rindex, cindex, f"Failed to decode masking role data '{text}', must be a valid role code '{parts[0]}'")
-            return None
+    # if self.globals.option_manager.get(Options.USDM_VERSION) == '2':
+    #   return None
+    # else:
+    try:
+      text = self.read_cell(rindex, cindex)
+      parts = text.split('=')
+      if len(parts) == 2: 
+        code = CDISCCT(self.globals).code_for_attribute('Masking', 'role', parts[0].strip())
+        if code:
+          mask = Masking(id=self.globals.id_manager.build_id(Masking), description=parts[1].strip(), role=code)
+          self.masks.append(mask)
+          self.globals.cross_references.add(mask.id, mask)
+          return mask
         else:
-          self._error(rindex, cindex, f"Failed to decode masking role data '{text}', no '=' detected")
+          self._error(rindex, cindex, f"Failed to decode masking role data '{text}', must be a valid role code '{parts[0]}'")
           return None
-      except Exception as e:
-        self._error(rindex, cindex, "Failed to create Masking object", e)
+      else:
+        self._error(rindex, cindex, f"Failed to decode masking role data '{text}', no '=' detected")
         return None
+    except Exception as e:
+      self._error(rindex, cindex, "Failed to create Masking object", e)
+      return None
```

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_sites_sheet/study_design_sites_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_sites_sheet/study_design_sites_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_design_timing_sheet/study_design_timing_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_design_timing_sheet/window_type.py` & `usdm-0.51.0/src/usdm_excel/study_design_timing_sheet/window_type.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 
   def _process_sheet(self):
     fields = ['category', 'name', 'description', 'label', 'type', 'date', 'scopes']    
     for rindex, row in self.sheet.iterrows():
       field_name = self.read_cell(rindex, self.PARAMS_NAME_COL)
       if field_name == self.NAME_TITLE:
         self.name = self.read_cell(rindex, self.PARAMS_DATA_COL)
-      elif field_name == self.TITLE_TITLE:
-        if self.globals.option_manager.get(Options.USDM_VERSION) == '2':
-          self.title = self.read_cell(rindex, self.PARAMS_DATA_COL)
+      #elif field_name == self.TITLE_TITLE:
+      #  if self.globals.option_manager.get(Options.USDM_VERSION) == '2':
+      #    self.title = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif field_name == self.VERSION_TITLE:
         self.version = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif field_name == self.TYPE_TITLE:
         self.type = self.read_cdisc_klass_attribute_cell('Study', 'studyType', rindex, self.PARAMS_DATA_COL)
       elif field_name == self.PHASE_TITLE:
         phase = self.read_cdisc_klass_attribute_cell('Study', 'studyPhase', rindex, self.PARAMS_DATA_COL)
         self.phase = Alias(self.globals).code(phase, [])
@@ -181,23 +181,23 @@
           else:
             self._error(row_index, col_index, f"Failed to decode geographic scope data {item}, appears empty")
           if code:
             result.append({'type': CDISCCT(self.globals).code_for_attribute('GeographicScope', 'type', pt), 'code':  Alias(self.globals).code(code, [])})
       return result
 
   def _set_title(self, rindex, cindex, title_type):
-    if self.globals.option_manager.get(Options.USDM_VERSION) == '2':
-      return self.read_cell(rindex, cindex)
-    else:
-      try:
-        text = self.read_cell(rindex, cindex)
-        if text:
-          code = CDISCCT(self.globals).code_for_attribute('StudyVersion', 'titles', title_type)
-          title = StudyTitle(id=self.globals.id_manager.build_id(StudyTitle), text=text, type=code)
-          self.titles.append(title)
-          self.globals.cross_references.add(title.id, title)
-          return title
-        else:
-          return None
-      except Exception as e:
-        self._exception(rindex, cindex, "Failed to create StudyTitle object", e)
+    # if self.globals.option_manager.get(Options.USDM_VERSION) == '2':
+    #   return self.read_cell(rindex, cindex)
+    # else:
+    try:
+      text = self.read_cell(rindex, cindex)
+      if text:
+        code = CDISCCT(self.globals).code_for_attribute('StudyVersion', 'titles', title_type)
+        title = StudyTitle(id=self.globals.id_manager.build_id(StudyTitle), text=text, type=code)
+        self.titles.append(title)
+        self.globals.cross_references.add(title.id, title)
+        return title
+      else:
+        return None
+    except Exception as e:
+      self._exception(rindex, cindex, "Failed to create StudyTitle object", e)
```

### Comparing `usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/activities.py` & `usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/activity.py` & `usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/conditons.py` & `usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/conditons.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py` & `usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py` & `usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/scheduled_instances.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/study_soa_v2_sheet/study_soa_v2_sheet.py` & `usdm-0.51.0/src/usdm_excel/study_soa_v2_sheet/study_soa_v2_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_excel/syntax_template_sheet.py` & `usdm-0.51.0/src/usdm_excel/syntax_template_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/__init__.py` & `usdm-0.51.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/api_base_model.py` & `usdm-0.51.0/src/usdm_model/api_base_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from pydantic import BaseModel, constr
 from typing import Union
 import json
 import enum
 import datetime
+from uuid import UUID
 
 # Example, see https://stackoverflow.com/questions/10252010/serializing-class-instance-to-json
 def _serialize_as_json(obj):
   if isinstance(obj, enum.Enum):
     return obj.value
   elif isinstance(obj, datetime.date):
     return obj.isoformat()
+  elif isinstance(obj, UUID):
+    return str(obj)
   else:
     return obj.__dict__
 
 def _serialize_as_json_with_type(obj):
   if isinstance(obj, enum.Enum):
     return obj.value
   elif isinstance(obj, datetime.date):
     return obj.isoformat()
+  elif isinstance(obj, UUID):
+    return str(obj)
   else:
     result = obj.__dict__
     result['_type'] = obj.__class__.__name__
     return result
 
 class ApiBaseModel(BaseModel):
```

### Comparing `usdm-0.50.0/src/usdm_model/encounter.py` & `usdm-0.51.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/population_definition.py` & `usdm-0.51.0/src/usdm_model/population_definition.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/schedule_timeline.py` & `usdm-0.51.0/src/usdm_model/schedule_timeline.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/scheduled_instance.py` & `usdm-0.51.0/src/usdm_model/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/study.py` & `usdm-0.51.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/study_design.py` & `usdm-0.51.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/study_intervention.py` & `usdm-0.51.0/src/usdm_model/study_intervention.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/src/usdm_model/study_version.py` & `usdm-0.51.0/src/usdm_model/study_version.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_base_sheet.py` & `usdm-0.51.0/tests/test_base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.51.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_configuration_sheet.py` & `usdm-0.51.0/tests/test_configuration_sheet.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,48 @@
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': ['Option X', 'Option 2', 'Option 3'], 'col_2': ['maybe', 'True', '']}
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data)
   configuration = ConfigurationSheet("", globals)
   assert globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.NONE.value
+  assert globals.option_manager.get(Options.USE_TEMPLATE) == 'SPONSOR'
+  assert globals.template_manager.get('sponsor') == 'studyDesignContent'
+
+def test_template(mocker, globals):
+  mocked_open = mocker.mock_open(read_data="File")
+  mocker.patch("builtins.open", mocked_open)
+  data = {'col_1': ['template'], 'col_2': ['xxx =    yyy']}
+  mock_read = mocker.patch("pandas.read_excel")
+  mock_read.return_value = pd.DataFrame(data)
+  configuration = ConfigurationSheet("", globals)
+  assert globals.template_manager.get('Xxx') == 'yyy'
+
+def test_use_template(mocker, globals):
+  mocked_open = mocker.mock_open(read_data="File")
+  mocker.patch("builtins.open", mocked_open)
+  data = {'col_1': ['USE template'], 'col_2': ['   zzzz   ']}
+  mock_read = mocker.patch("pandas.read_excel")
+  mock_read.return_value = pd.DataFrame(data)
+  configuration = ConfigurationSheet("", globals)
+  assert globals.option_manager.get(Options.USE_TEMPLATE) == 'ZZZZ'
+
+def test_usdm_version_deprecated(mocker, globals):
+  mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
+  mocked_open = mocker.mock_open(read_data="File")
+  mocker.patch("builtins.open", mocked_open)
+  data = {'col_1': ['Usdm VERsion'], 'col_2': ['XXX']}
+  mock_read = mocker.patch("pandas.read_excel")
+  mock_read.return_value = pd.DataFrame(data)
+  configuration = ConfigurationSheet("", globals)
+  mock_error.assert_called()
+  assert mock_error.call_args[0][0] == "configuration"
+  assert mock_error.call_args[0][1] == None
+  assert mock_error.call_args[0][2] == None
+  assert mock_error.call_args[0][3] == "The USDM VERSION option is now deprecated and will be ignored."
 
 def test_sdr_deprecated(mocker, globals):
   mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = {'col_1': ['sdr DESCRIPTION'], 'col_2': ['']}
   mock_read = mocker.patch("pandas.read_excel")
```

### Comparing `usdm-0.50.0/tests/test_cross_reference.py` & `usdm-0.51.0/tests/test_cross_reference.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_data_factory.py` & `usdm-0.51.0/tests/test_data_factory.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_document.py` & `usdm-0.51.0/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_document_elements.py` & `usdm-0.51.0/tests/test_document_elements.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_document_macros.py` & `usdm-0.51.0/tests/test_document_macros.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_document_soa.py` & `usdm-0.51.0/tests/test_document_soa.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_document_template_plain.py` & `usdm-0.51.0/tests/test_document_template_plain.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_document_utility.py` & `usdm-0.51.0/tests/test_document_utility.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_error.py` & `usdm-0.51.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_errors.py` & `usdm-0.51.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_factory.py` & `usdm-0.51.0/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_integration.py` & `usdm-0.51.0/tests/test_integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import csv
-from usdm_excel import USDMExcel
+import yaml
 from usdm_db import USDMDb
 from bs4 import BeautifulSoup
+from uuid import UUID
 
 SAVE_ALL = False
 
 def save_error_csv(file, contents):
   writer = csv.DictWriter(file, fieldnames=['sheet','row','column','message','level'])
   writer.writeheader()
   writer.writerows(contents)
@@ -84,14 +85,47 @@
     with open(f"tests/integration_test_files/{filename}_timeline_{level}.html", 'w') as f:
       f.write(result)
   
   with open(f"tests/integration_test_files/{filename}_timeline_{level}.html", 'r') as f:
     expected = f.read()
   assert result == expected
 
+def run_test_neo4j(filename, mocker, save=False):
+  fake_uuids = (UUID(f'00000000-0000-4000-8000-{i:012}', version=4) for i in range(10000))
+  mocker.patch("usdm_db.neo4j_dict.uuid4", side_effect=fake_uuids)
+  usdm = USDMDb()
+  usdm.from_excel(f"tests/integration_test_files/{filename}.xlsx")
+  result = usdm.to_neo4j_dict()
+
+  # Useful if you want to see the results.
+  if save or SAVE_ALL:
+    with open(f"tests/integration_test_files/{filename}_neo4j_dict.yaml", 'w') as f:
+      f.write(yaml.dump(result))
+  
+  with open(f"tests/integration_test_files/{filename}_neo4j_dict.yaml", 'r') as f:
+    expected = yaml.safe_load(f) 
+  assert result == expected
+
+def run_test_fhir(filename, mocker, save=False):
+  fake_uuids = (UUID(f'00000000-0000-4000-8000-{i:012}', version=4) for i in range(1,10))
+  mocker.patch("usdm_db.uuid4", side_effect=fake_uuids)
+  usdm = USDMDb()
+  usdm.from_excel(f"tests/integration_test_files/{filename}.xlsx")
+  result = usdm.to_fhir()
+
+  if save or SAVE_ALL:
+    with open(f"tests/integration_test_files/{filename}_fhir.json", 'w', encoding='utf-8') as f:
+      f.write(json.dumps(json.loads(result), indent=2))
+  
+  with open(f"tests/integration_test_files/{filename}_fhir.json", 'r') as f:
+    expected = json.load(f)
+  result_dict = json.loads(result)
+  result_dict["entry"][0]["resource"]["date"] = expected["entry"][0]["resource"]["date"] # Date is dynamic, bit of a fiddle but datetime mocking is a pain.
+  json.dumps(result_dict) == json.dumps(expected)
+
 def test_full_1():
   run_test('full_1')
 
 def test_full_1_timeline():
   run_test_timeline('full_1')
 
 def test_full_1_timeline_body():
@@ -111,14 +145,17 @@
 
 def test_full_3_html():
   run_test_html('full_3')
 
 def test_full_4():
   run_test('full_4')
 
+def test_full_5():
+  run_test('full_5')
+
 def test_encounter_1():
   run_test('encounter_1')
 
 def test_simple_1():
   run_test('simple_1')
 
 def test_scope_1():
@@ -191,7 +228,22 @@
   run_test('references')
 
 def test_references_html():
   run_test_html('references')
 
 def test_references_html_highlight():
   run_test_html('references', highlight=True)
+
+def test_simple_neo4j_1(mocker):
+  run_test_neo4j('simple_1', mocker)
+
+def test_full_neo4j_1(mocker):
+  run_test_neo4j('full_1', mocker)
+
+def test_full_neo4j_2(mocker):
+  run_test_neo4j('full_2', mocker)
+
+def test_full_neo4j_3(mocker):
+  run_test_neo4j('full_3', mocker)
+
+def test_full_fhir_1(mocker):
+  run_test_fhir('full_1', mocker)
```

### Comparing `usdm-0.50.0/tests/test_iso_3166.py` & `usdm-0.51.0/tests/test_iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_iso_8601_duration.py` & `usdm-0.51.0/tests/test_iso_8601_duration.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_option_manager.py` & `usdm-0.51.0/tests/test_option_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from usdm_excel.option_manager import *
 
-
 def test_create(globals):
   object = OptionManager(globals)
   assert len(object._items.keys()) == 0
   assert object._items == {}
 
 def test_set(globals):
   globals.option_manager._items = {}
@@ -25,15 +24,9 @@
   assert len(globals.option_manager._items.keys()) == 0
 
 def test_options(globals):
   globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.NONE)
   assert globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.NONE.value
   globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.EMPTY)
   assert globals.option_manager.get(Options.EMPTY_NONE) == EmptyNoneOption.EMPTY.value
-  globals.option_manager.set(Options.USDM_VERSION, 2)
-  assert globals.option_manager.get(Options.USDM_VERSION) == '2'
-  globals.option_manager.set(Options.USDM_VERSION, 3)
-  assert globals.option_manager.get(Options.USDM_VERSION) == '3'
-  # globals.option_manager.set(Options.ROOT, RootOption.API_COMPLIANT)
-  # assert globals.option_manager.get(Options.ROOT) == RootOption.API_COMPLIANT.value
-  # globals.option_manager.set(Options.DESCRIPTION, 'Some text')
-  # assert globals.option_manager.get(Options.DESCRIPTION) == 'Some text'
+  globals.option_manager.set(Options.USE_TEMPLATE, "XXX")
+  assert globals.option_manager.get(Options.USE_TEMPLATE) == 'XXX'
```

### Comparing `usdm-0.50.0/tests/test_quantity_type.py` & `usdm-0.51.0/tests/test_quantity_type.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_range_type.py` & `usdm-0.51.0/tests/test_range_type.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_activity_sheet.py` & `usdm-0.51.0/tests/test_study_design_activity_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_arm_sheet.py` & `usdm-0.51.0/tests/test_study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_characteristic_sheet.py` & `usdm-0.51.0/tests/test_study_design_characteristic_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_conditions_sheet.py` & `usdm-0.51.0/tests/test_study_design_conditions_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_content_sheet.py` & `usdm-0.51.0/tests/test_study_design_content_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from usdm_excel.option_manager import Options, EmptyNoneOption
 from tests.test_factory import Factory
 
 xfail = pytest.mark.xfail
 
 def test_create(mocker, globals):
   globals.option_manager.set(Options.EMPTY_NONE, EmptyNoneOption.EMPTY)
+  globals.option_manager.set(Options.USE_TEMPLATE, 'SPONSOR')
 
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
@@ -32,15 +33,15 @@
   assert content.items[0].name == 'ROOT'
   assert content.items[0].previousId == ''
   assert content.items[0].nextId == 'Content_2'  
   assert content.items[1].id == 'Content_2'
   assert content.items[1].name == 'SECTION 1'
   assert content.items[1].sectionNumber == '1'
   assert content.items[1].sectionTitle == 'Section 1'
-  assert content.items[1].text == '<div>Text 1</div>'
+  assert content.items[1].text == '<div xmlns="http://www.w3.org/1999/xhtml">Text 1</div>'
   assert content.items[1].childIds == ['Content_3', 'Content_4']
   assert content.items[1].previousId == 'Content_1'
   assert content.items[1].nextId == 'Content_3'  
   assert content.items[2].name == 'SET NAME'
   assert content.items[2].previousId == 'Content_2'
   assert content.items[2].nextId == 'Content_4'  
   assert content.items[3].name == 'SECTION 1.2'
@@ -73,15 +74,15 @@
   content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 8
   assert content.items[0].name == 'ROOT'
   assert content.items[1].id == 'Content_2'
   assert content.items[1].name == 'SECTION 1'
   assert content.items[1].sectionNumber == '1'
   assert content.items[1].sectionTitle == 'Section 1'
-  assert content.items[1].text == '<div>Text 1</div>'
+  assert content.items[1].text == '<div xmlns="http://www.w3.org/1999/xhtml">Text 1</div>'
   assert content.items[1].childIds == ['Content_3', 'Content_4']
   assert content.items[2].name == 'SET NAME'
   assert content.items[3].name == 'SECTION 1.2'
   assert content.items[4].name == 'SECTION 1.2.1'
   assert content.items[5].name == 'SECTION 2'
   assert content.items[6].name == 'SECTION 2.1'
   assert content.items[7].id == 'Content_8'
@@ -108,21 +109,21 @@
   content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 8
   assert content.items[0].name == 'ROOT'
   assert content.items[4].id == 'Content_5'
   assert content.items[4].name == 'SECTION 1.2.1'
   assert content.items[4].sectionNumber == '1.2.1'
   assert content.items[4].sectionTitle == 'Section 1.2.1'
-  assert content.items[4].text == '<div>Text 1.2.1</div>'
+  assert content.items[4].text == '<div xmlns="http://www.w3.org/1999/xhtml">Text 1.2.1</div>'
   assert content.items[4].childIds == ['Content_6']
   assert content.items[5].id == 'Content_6'
   assert content.items[5].name == 'SECTION 1.2.1.1'
   assert content.items[5].sectionNumber == '1.2.1.1'
   assert content.items[5].sectionTitle == 'Section 1.2.1.1'
-  assert content.items[5].text == '<div>Text 1.2.1.1</div>'
+  assert content.items[5].text == '<div xmlns="http://www.w3.org/1999/xhtml">Text 1.2.1.1</div>'
   assert content.items[5].childIds == []
 
 def test_create_standard_section(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
@@ -136,21 +137,23 @@
     ['2',       '',         'Section 2',       'Text 2'], 
   ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
   content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 6
   assert content.items[0].text == ''
-  assert content.items[1].text == '<div>Text 1</div>'
-  assert content.items[2].text == '<div>Text 1.1</div>'
-  assert content.items[3].text == '<div><usdm:section name="m11-title"></div>'
-  assert content.items[4].text == '<div><usdm:section name="m11-title"></div>'
-  assert content.items[5].text == '<div>Text 2</div>'
+  assert content.items[1].text == '<div xmlns="http://www.w3.org/1999/xhtml">Text 1</div>'
+  assert content.items[2].text == '<div xmlns="http://www.w3.org/1999/xhtml">Text 1.1</div>'
+  assert content.items[3].text == '<div xmlns="http://www.w3.org/1999/xhtml"><usdm:section name="m11-title"></div>'
+  assert content.items[4].text == '<div xmlns="http://www.w3.org/1999/xhtml"><usdm:section name="m11-title"></div>'
+  assert content.items[5].text == '<div xmlns="http://www.w3.org/1999/xhtml">Text 2</div>'
 
 def test_create_invalid_levels(mocker, globals):
+  globals.option_manager.set(Options.USE_TEMPLATE, 'SPONSOR')
+  globals.template_manager.add('sponsor', 'studyDesignContent')
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mock_error = mocker.patch("usdm_excel.errors_and_logging.errors.Errors.add")
   mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Content_1', 'Content_2', 'Content_3', 'Content_4', 'Content_5', 'Content_6', 'Content_7', 'Content_8']
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
@@ -180,15 +183,16 @@
   data = []
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['sectionNumber', 'name', 'sectionTitle', 'text'])
   content = StudyDesignContentSheet("", globals)
   assert len(content.items) == 1
 
 def test_read_cell_by_name_error(mocker, globals):
-  
+  globals.option_manager.set(Options.USE_TEMPLATE, 'SPONSOR')
+  globals.template_manager.add('sponsor', 'studyDesignContent')
   call_parameters = []
   
   def my_add(sheet, row, column, message, level=10):
     call_parameters.append((sheet, row, column, message, level))
     return None
 
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
```

### Comparing `usdm-0.50.0/tests/test_study_design_dictionary_sheet.py` & `usdm-0.51.0/tests/test_study_design_dictionary_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   assert dictionaries.items[0].name == 'Dictionary 1'
   assert dictionaries.items[0].description == 'Dictionary One'
   assert dictionaries.items[0].label == 'Label One'
   assert dictionaries.items[0].parameterMaps[1].tag == 'Key 2'
   assert dictionaries.items[0].parameterMaps[1].reference == '<usdm:ref klass="ApiBaseModelWithId" id="2" attribute="Attribute 2"></usdm:ref>'
   assert [x.tag for x in dictionaries.items[1].parameterMaps] == ['Key 3']
   assert [x.tag for x in dictionaries.items[2].parameterMaps] == ['Key 4', 'Key 5', 'Key 6']
-  assert dictionaries.items[2].parameterMaps[2].reference == "<div>Hello!</div>"
+  assert dictionaries.items[2].parameterMaps[2].reference == "Hello!"
   
 def test_create_empty(mocker, globals):
   mock_present = mocker.patch("usdm_excel.base_sheet.BaseSheet._sheet_present")
   mock_present.side_effect=[True]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = []
```

### Comparing `usdm-0.50.0/tests/test_study_design_eligibility_criteria_sheet.py` & `usdm-0.51.0/tests/test_study_design_eligibility_criteria_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_encounter_sheet.py` & `usdm-0.51.0/tests/test_study_design_encounter_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_epoch_sheet.py` & `usdm-0.51.0/tests/test_study_design_epoch_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_indication_sheet.py` & `usdm-0.51.0/tests/test_study_design_indication_sheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 
 xfail = pytest.mark.xfail
 
 def test_create(mocker, globals):
   mock_id = mocker.patch("usdm_excel.id_manager.IdManager.build_id")
   mock_id.side_effect=['Code_1', 'IndicationId_1', 'Code_2', 'IndicationId_2', 'Code_3', 'Code_4', 'IndicationId_3']
-  expected_1 = Code(id='Code_1', code='X', codeSystem='SPONSOR', codeSystemVersion='None set', decode="Y")
-  expected_2 = Code(id='Code_2', code='AAA', codeSystem='SPONSOR', codeSystemVersion='None set', decode="BBB")
-  expected_3 = Code(id='Code_3', code='WWW', codeSystem='SPONSOR', codeSystemVersion='None set', decode="1234")
-  expected_4 = Code(id='Code_4', code='EEE', codeSystem='SPONSOR', codeSystemVersion='None set', decode="3456")
+  expected_1 = Code(id='Code_1', code='X', codeSystem='SPONSOR', codeSystemVersion='', decode="Y")
+  expected_2 = Code(id='Code_2', code='AAA', codeSystem='SPONSOR', codeSystemVersion='', decode="BBB")
+  expected_3 = Code(id='Code_3', code='WWW', codeSystem='SPONSOR', codeSystemVersion='', decode="1234")
+  expected_4 = Code(id='Code_4', code='EEE', codeSystem='SPONSOR', codeSystemVersion='', decode="3456")
   mock_code = mocker.patch("usdm_excel.cdisc_ct.CDISCCT.code_for_attribute")
   mock_code.side_effect=[expected_1, expected_2, expected_3, expected_4]
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Indication 1', 'Indication One', 'Label One', 'Sponsor:X=Y'], 
           ['Indication 2', 'Indication Two', '', 'SPONSOR: AAA=BBB'], 
           ['Indication 3', 'Indication Three', '', 'SPONSOR: WWW=1234, SPONSOR: EEE=3456']]
```

### Comparing `usdm-0.50.0/tests/test_study_design_intervention_sheet.py` & `usdm-0.51.0/tests/test_study_design_intervention_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_oe_sheet.py` & `usdm-0.51.0/tests/test_study_design_oe_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_population_sheet.py` & `usdm-0.51.0/tests/test_study_design_population_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_sites_sheet.py` & `usdm-0.51.0/tests/test_study_design_sites_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_design_timing_sheet.py` & `usdm-0.51.0/tests/test_study_design_timing_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_identifiers_sheet.py` & `usdm-0.51.0/tests/test_study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_study_sheet.py` & `usdm-0.51.0/tests/test_study_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.50.0/tests/test_utility.py` & `usdm-0.51.0/tests/test_utility.py`

 * *Files identical despite different names*

