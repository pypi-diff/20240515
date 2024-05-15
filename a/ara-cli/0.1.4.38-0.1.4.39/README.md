# Comparing `tmp/ara_cli-0.1.4.38.tar.gz` & `tmp/ara_cli-0.1.4.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ara_cli-0.1.4.38.tar", last modified: Wed May 15 06:36:41 2024, max compression
+gzip compressed data, was "ara_cli-0.1.4.39.tar", last modified: Wed May 15 07:13:35 2024, max compression
```

## Comparing `ara_cli-0.1.4.38.tar` & `ara_cli-0.1.4.39.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.370247 ara_cli-0.1.4.38/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/MANIFEST.in
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 06:36:41.370247 ara_cli-0.1.4.38/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3681 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/README.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.358246 ara_cli-0.1.4.38/ara_cli/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    10783 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/__main__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/ara_config.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/artefact.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/artefact_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/artefact_deleter.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/artefact_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3569 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/chat.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/classifier_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/file_classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/filename_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5242 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/prompt_extractor.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15580 2024-05-15 06:23:20.000000 ara_cli-0.1.4.38/ara_cli/prompt_handler.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5679 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/prompt_rag.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/run_file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/template_manager.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.362246 ara_cli-0.1.4.38/ara_cli/templates/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/agile.artefacts
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.354246 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.362246 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.366246 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/prompts/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.366246 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.358246 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.366246 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1061 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      798 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1414 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      837 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      808 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_empty_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1426 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      933 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.366246 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_classify_task_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_empty_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      448 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_extend_feature_and_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_adaption_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_python_cli_implementation_with_test_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_python_code_understanding_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_python_error_fixing_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/prompts/template_python_implementation_from_task_description_intention_and_context.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.370247 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/template_empty_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1062 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.370247 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.concept.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.customer.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.persona.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.step.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.technology.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.businessgoal
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.businessgoal_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.capability
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.capability_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.epic
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.epic_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.example
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.example_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.feature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.feature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.issue
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.keyfeature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.keyfeature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.steps_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      533 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.task
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.task_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.userstory
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.userstory_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.vision
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/templates/template.vision_exploration.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.370247 ara_cli-0.1.4.38/ara_cli/tests/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/tests/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/tests/test_artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/tests/test_artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/tests/test_directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/tests/test_file_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/tests/test_template_manager.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/ara_cli/vectorDB.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-15 06:29:15.000000 ara_cli-0.1.4.38/ara_cli/version.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 06:36:41.362246 ara_cli-0.1.4.38/ara_cli.egg-info/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 06:36:41.000000 ara_cli-0.1.4.38/ara_cli.egg-info/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6089 2024-05-15 06:36:41.000000 ara_cli-0.1.4.38/ara_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-15 06:36:41.000000 ara_cli-0.1.4.38/ara_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-15 06:36:41.000000 ara_cli-0.1.4.38/ara_cli.egg-info/entry_points.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-15 06:36:41.000000 ara_cli-0.1.4.38/ara_cli.egg-info/requires.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-15 06:36:41.000000 ara_cli-0.1.4.38/ara_cli.egg-info/top_level.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-15 06:36:41.370247 ara_cli-0.1.4.38/setup.cfg
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-14 09:39:23.000000 ara_cli-0.1.4.38/setup.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.701928 ara_cli-0.1.4.39/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/MANIFEST.in
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 07:13:35.701928 ara_cli-0.1.4.39/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3681 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/README.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.685928 ara_cli-0.1.4.39/ara_cli/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    10783 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/__main__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/ara_config.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/artefact.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/artefact_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/artefact_deleter.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/artefact_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3569 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/chat.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/classifier_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/file_classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/filename_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5242 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/prompt_extractor.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15580 2024-05-15 06:23:20.000000 ara_cli-0.1.4.39/ara_cli/prompt_handler.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5674 2024-05-15 07:13:02.000000 ara_cli-0.1.4.39/ara_cli/prompt_rag.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/run_file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/template_manager.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.689928 ara_cli-0.1.4.39/ara_cli/templates/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/agile.artefacts
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.681928 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.689928 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.693928 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/prompts/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.693928 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.681928 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.693928 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1061 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      798 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1414 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      837 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      808 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_empty_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1426 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      933 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.697928 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_classify_task_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_empty_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      448 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_extend_feature_and_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_adaption_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_python_cli_implementation_with_test_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_python_code_understanding_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_python_error_fixing_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/prompts/template_python_implementation_from_task_description_intention_and_context.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.697928 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/template_empty_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1062 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.697928 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.concept.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.customer.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.persona.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.step.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.technology.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.businessgoal
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.businessgoal_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.capability
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.capability_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.epic
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.epic_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.example
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.example_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.feature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.feature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.issue
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.keyfeature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.keyfeature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.steps_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      533 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.task
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.task_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.userstory
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.userstory_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.vision
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/templates/template.vision_exploration.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.701928 ara_cli-0.1.4.39/ara_cli/tests/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/tests/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/tests/test_artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/tests/test_artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/tests/test_directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/tests/test_file_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/tests/test_template_manager.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/ara_cli/vectorDB.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-15 07:13:13.000000 ara_cli-0.1.4.39/ara_cli/version.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-15 07:13:35.685928 ara_cli-0.1.4.39/ara_cli.egg-info/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-15 07:13:35.000000 ara_cli-0.1.4.39/ara_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6089 2024-05-15 07:13:35.000000 ara_cli-0.1.4.39/ara_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-15 07:13:35.000000 ara_cli-0.1.4.39/ara_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-15 07:13:35.000000 ara_cli-0.1.4.39/ara_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-15 07:13:35.000000 ara_cli-0.1.4.39/ara_cli.egg-info/requires.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-15 07:13:35.000000 ara_cli-0.1.4.39/ara_cli.egg-info/top_level.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-15 07:13:35.701928 ara_cli-0.1.4.39/setup.cfg
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-14 09:39:23.000000 ara_cli-0.1.4.39/setup.py
```

### Comparing `ara_cli-0.1.4.38/README.md` & `ara_cli-0.1.4.39/README.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/__main__.py` & `ara_cli-0.1.4.39/ara_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/ara_config.py` & `ara_cli-0.1.4.39/ara_cli/ara_config.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/artefact.py` & `ara_cli-0.1.4.39/ara_cli/artefact.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/artefact_creator.py` & `ara_cli-0.1.4.39/ara_cli/artefact_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/artefact_deleter.py` & `ara_cli-0.1.4.39/ara_cli/artefact_deleter.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/artefact_link_updater.py` & `ara_cli-0.1.4.39/ara_cli/artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/artefact_lister.py` & `ara_cli-0.1.4.39/ara_cli/artefact_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/artefact_renamer.py` & `ara_cli-0.1.4.39/ara_cli/artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/chat.py` & `ara_cli-0.1.4.39/ara_cli/chat.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/classifier.py` & `ara_cli-0.1.4.39/ara_cli/classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/directory_navigator.py` & `ara_cli-0.1.4.39/ara_cli/directory_navigator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/file_classifier.py` & `ara_cli-0.1.4.39/ara_cli/file_classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/file_lister.py` & `ara_cli-0.1.4.39/ara_cli/file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/prompt_extractor.py` & `ara_cli-0.1.4.39/ara_cli/prompt_extractor.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/prompt_handler.py` & `ara_cli-0.1.4.39/ara_cli/prompt_handler.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/prompt_rag.py` & `ara_cli-0.1.4.39/ara_cli/prompt_rag.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     dir_list = ["ara"] + [item for ext in config.ext_code_dirs for key, item in ext.items()]  + [config.doc_dir] + [config.glossary_dir]
     documents = []
     for directory in dir_list:
         if is_directory_not_empty(directory):
             print(f"load {directory} to RAG documents")
             documents += SimpleDirectoryReader(directory).load_data()
 
-    llm = OpenAI(model="gpt-4-turbo")
+    llm = OpenAI(model="gpt-4o")
     service_context = ServiceContext.from_defaults(chunk_size=2024, llm=llm)
     nodes = service_context.node_parser.get_nodes_from_documents(documents)
 
     storage_context = StorageContext.from_defaults()
     storage_context.docstore.add_documents(nodes)
 
     index = VectorStoreIndex(nodes=nodes, storage_context=storage_context, service_context=service_context)
```

### Comparing `ara_cli-0.1.4.38/ara_cli/run_file_lister.py` & `ara_cli-0.1.4.39/ara_cli/run_file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/template_manager.py` & `ara_cli-0.1.4.39/ara_cli/template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/agile.artefacts` & `ara_cli-0.1.4.39/ara_cli/templates/agile.artefacts`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_businessgoal.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_capability.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_epic.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_feature.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_keyfeature.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_task.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_userstory.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/commands/template_vision.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/commands/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_businessgoal.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_capability.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_epic.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_feature.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_keyfeature.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_task.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_userstory.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-creation/rules/template_vision.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-creation/rules/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_empty_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_empty_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md` & `ara_cli-0.1.4.39/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.concept.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.concept.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.customer.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.customer.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.persona.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.persona.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.step.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.step.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.technology.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.technology.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md` & `ara_cli-0.1.4.39/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.businessgoal` & `ara_cli-0.1.4.39/ara_cli/templates/template.businessgoal`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.capability` & `ara_cli-0.1.4.39/ara_cli/templates/template.capability`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.epic` & `ara_cli-0.1.4.39/ara_cli/templates/template.epic`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.feature` & `ara_cli-0.1.4.39/ara_cli/templates/template.feature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.issue` & `ara_cli-0.1.4.39/ara_cli/templates/template.issue`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.keyfeature` & `ara_cli-0.1.4.39/ara_cli/templates/template.keyfeature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.task` & `ara_cli-0.1.4.39/ara_cli/templates/template.task`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.userstory` & `ara_cli-0.1.4.39/ara_cli/templates/template.userstory`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/templates/template.vision` & `ara_cli-0.1.4.39/ara_cli/templates/template.vision`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/tests/test_artefact_link_updater.py` & `ara_cli-0.1.4.39/ara_cli/tests/test_artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/tests/test_artefact_renamer.py` & `ara_cli-0.1.4.39/ara_cli/tests/test_artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/tests/test_file_creator.py` & `ara_cli-0.1.4.39/ara_cli/tests/test_file_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/tests/test_template_manager.py` & `ara_cli-0.1.4.39/ara_cli/tests/test_template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli/vectorDB.py` & `ara_cli-0.1.4.39/ara_cli/vectorDB.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/ara_cli.egg-info/SOURCES.txt` & `ara_cli-0.1.4.39/ara_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.38/setup.py` & `ara_cli-0.1.4.39/setup.py`

 * *Files identical despite different names*

