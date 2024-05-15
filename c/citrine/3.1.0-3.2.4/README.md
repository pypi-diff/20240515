# Comparing `tmp/citrine-3.1.0.tar.gz` & `tmp/citrine-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrine-3.1.0.tar", last modified: Tue Mar 19 16:41:47 2024, max compression
+gzip compressed data, was "citrine-3.2.4.tar", last modified: Wed May 15 16:10:41 2024, max compression
```

## Comparing `citrine-3.1.0.tar` & `citrine-3.2.4.tar`

### file list

```diff
@@ -1,178 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.199694 citrine-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-19 16:41:46.000000 citrine-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-19 16:41:47.199694 citrine-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-19 16:41:46.000000 citrine-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:41:47.199694 citrine-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-19 16:41:46.000000 citrine-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.175694 citrine-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.179695 citrine-3.1.0/src/citrine/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.179695 citrine-3.1.0/src/citrine/_rest/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/admin_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/ai_resource_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/asynchronous_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/engine_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/pageable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_rest/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.179695 citrine-3.1.0/src/citrine/_serialization/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_serialization/include_parent_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_serialization/polymorphic_serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)    40562 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_serialization/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.179695 citrine-3.1.0/src/citrine/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_utils/batcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/_utils/template_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/citrine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.183694 citrine-3.1.0/src/citrine/gemd_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemd_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemd_queries/criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemd_queries/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemd_queries/gemd_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.183694 citrine-3.1.0/src/citrine/gemtables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemtables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemtables/columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemtables/rows.py
--rw-r--r--   0 runner    (1001) docker     (127)    48906 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/gemtables/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.183694 citrine-3.1.0/src/citrine/informatics/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.183694 citrine-3.1.0/src/citrine/informatics/catalyst/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/catalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/catalyst/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/catalyst/insights.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/catalyst/language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.187694 citrine-3.1.0/src/citrine/informatics/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/categorical_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/ingredient_count_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/ingredient_fraction_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/ingredient_ratio_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/integer_range_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/label_fraction_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/constraints/scalar_range_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_candidate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.187694 citrine-3.1.0/src/citrine/informatics/design_spaces/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/data_source_design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/enumerated_design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/formulation_design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/hierarchical_design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/product_design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/design_spaces/sample_design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/dimensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.187694 citrine-3.1.0/src/citrine/informatics/executions/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/executions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/executions/design_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/executions/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/executions/generative_design_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/executions/predictor_evaluation_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/executions/sample_design_space_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/experiment_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/generative_design.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predict_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictor_evaluation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictor_evaluation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictor_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.191694 citrine-3.1.0/src/citrine/informatics/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/auto_ml_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/chemical_formula_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/expression_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/graph_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/ingredient_fractions_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/ingredients_to_formulation_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/label_fractions_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/mean_property_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/molecular_structure_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/simple_mixture_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/single_predict_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/predictors/single_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.191694 citrine-3.1.0/src/citrine/informatics/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/workflows/design_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/workflows/predictor_evaluation_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/informatics/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.191694 citrine-3.1.0/src/citrine/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/jobs/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/jobs/waiting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.199694 citrine-3.1.0/src/citrine/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/attribute_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/audit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/condition_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    29166 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/data_concepts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/data_version_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    21552 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/design_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/design_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/design_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/experiment_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    33514 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/file_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/gemd_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/gemtables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/generative_design_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/ingestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/ingredient_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/ingredient_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/material_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/material_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/material_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/measurement_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/measurement_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/measurement_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/object_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/object_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/object_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/parameter_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    24327 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/predictor_evaluation_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/predictor_evaluation_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/process_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/process_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/process_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/project_member.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/project_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/property_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/sample_design_space_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/status_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/table_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14231 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/team.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/resources/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.199694 citrine-3.1.0/src/citrine/seeding/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/seeding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/seeding/find_or_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-19 16:41:46.000000 citrine-3.1.0/src/citrine/seeding/sort_gems.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:41:47.179695 citrine-3.1.0/src/citrine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-19 16:41:47.000000 citrine-3.1.0/src/citrine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-03-19 16:41:47.000000 citrine-3.1.0/src/citrine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:41:47.000000 citrine-3.1.0/src/citrine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-19 16:41:47.000000 citrine-3.1.0/src/citrine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-19 16:41:47.000000 citrine-3.1.0/src/citrine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.149609 citrine-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-15 16:10:36.000000 citrine-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-15 16:10:41.149609 citrine-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-15 16:10:36.000000 citrine-3.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:10:41.149609 citrine-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-15 16:10:36.000000 citrine-3.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.125609 citrine-3.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.129609 citrine-3.2.4/src/citrine/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.129609 citrine-3.2.4/src/citrine/_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/admin_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/ai_resource_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/asynchronous_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/engine_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/pageable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_rest/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.133609 citrine-3.2.4/src/citrine/_serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_serialization/include_parent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_serialization/polymorphic_serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40661 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_serialization/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.133609 citrine-3.2.4/src/citrine/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_utils/batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/_utils/template_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/citrine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.133609 citrine-3.2.4/src/citrine/gemd_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemd_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemd_queries/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemd_queries/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemd_queries/gemd_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.133609 citrine-3.2.4/src/citrine/gemtables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemtables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemtables/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemtables/rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48906 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/gemtables/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.137609 citrine-3.2.4/src/citrine/informatics/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.137609 citrine-3.2.4/src/citrine/informatics/catalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/catalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/catalyst/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/catalyst/insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/catalyst/language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.137609 citrine-3.2.4/src/citrine/informatics/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/categorical_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/ingredient_count_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/ingredient_fraction_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/ingredient_ratio_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/integer_range_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/label_fraction_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/constraints/scalar_range_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_candidate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.137609 citrine-3.2.4/src/citrine/informatics/design_spaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/data_source_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/enumerated_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/formulation_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/hierarchical_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/product_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/design_spaces/sample_design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/dimensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.137609 citrine-3.2.4/src/citrine/informatics/executions/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/executions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/executions/design_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/executions/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/executions/generative_design_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/executions/predictor_evaluation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/executions/sample_design_space_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/experiment_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/generative_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predict_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictor_evaluation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictor_evaluation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictor_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.141609 citrine-3.2.4/src/citrine/informatics/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/auto_ml_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/chemical_formula_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/expression_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/graph_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/ingredient_fractions_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/ingredients_to_formulation_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/label_fractions_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/mean_property_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/molecular_structure_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/simple_mixture_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/single_predict_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/predictors/single_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.141609 citrine-3.2.4/src/citrine/informatics/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/workflows/analysis_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/workflows/design_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/workflows/predictor_evaluation_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/informatics/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.141609 citrine-3.2.4/src/citrine/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/jobs/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/jobs/waiting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.149609 citrine-3.2.4/src/citrine/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/analysis_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/attribute_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/audit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/condition_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29166 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/data_concepts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/data_version_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21552 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/design_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/design_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/design_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/experiment_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33514 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/file_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/gemd_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/gemtables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/generative_design_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/ingredient_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/ingredient_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/material_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/material_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/material_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/measurement_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/measurement_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/measurement_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/object_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/object_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/object_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/parameter_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24327 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/predictor_evaluation_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/predictor_evaluation_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/process_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/process_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/process_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/project_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/project_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/property_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/sample_design_space_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26139 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/table_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/resources/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.149609 citrine-3.2.4/src/citrine/seeding/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/seeding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/seeding/find_or_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-15 16:10:36.000000 citrine-3.2.4/src/citrine/seeding/sort_gems.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:10:41.129609 citrine-3.2.4/src/citrine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-15 16:10:41.000000 citrine-3.2.4/src/citrine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-15 16:10:41.000000 citrine-3.2.4/src/citrine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:10:41.000000 citrine-3.2.4/src/citrine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-15 16:10:41.000000 citrine-3.2.4/src/citrine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 16:10:41.000000 citrine-3.2.4/src/citrine.egg-info/top_level.txt
```

### Comparing `citrine-3.1.0/LICENSE` & `citrine-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/PKG-INFO` & `citrine-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrine
-Version: 3.1.0
+Version: 3.2.4
 Summary: Python library for the Citrine Platform
 Home-page: http://github.com/CitrineInformatics/citrine-python
 Author: Citrine Informatics
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `citrine-3.1.0/README.md` & `citrine-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/setup.py` & `citrine-3.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_rest/admin_collection.py` & `citrine-3.2.4/src/citrine/_rest/admin_collection.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_rest/ai_resource_metadata.py` & `citrine-3.2.4/src/citrine/_rest/ai_resource_metadata.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_rest/asynchronous_object.py` & `citrine-3.2.4/src/citrine/_rest/asynchronous_object.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_rest/collection.py` & `citrine-3.2.4/src/citrine/_rest/collection.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_rest/engine_resource.py` & `citrine-3.2.4/src/citrine/_rest/engine_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 from citrine._serialization import properties
 from citrine._serialization.include_parent_properties import IncludeParentProperties
 from citrine.resources.status_detail import StatusDetail
 
 Self = TypeVar('Self', bound='Resource')
 
 
-# This class is the base type for the new module endpoints which do not support versions. If/once
-# they support versioning, they should be switched to inherit from VersionedEngineResource.
-class EngineResource(Resource[Self]):
+class EngineResourceWithoutStatus(Resource[Self]):
     """Base resource for metadata from stand-alone AI Engine modules."""
 
     created_by = properties.Optional(properties.UUID, 'metadata.created.user', serializable=False)
     """:Optional[UUID]: id of the user who created the resource"""
     create_time = properties.Optional(properties.Datetime, 'metadata.created.time',
                                       serializable=False)
     """:Optional[datetime]: date and time at which the resource was created"""
@@ -32,38 +30,50 @@
                                       serializable=False)
     """:Optional[UUID]: id of the user who archived the resource, if it has been archived"""
     archive_time = properties.Optional(properties.Datetime, 'metadata.archived.time',
                                        serializable=False)
     """:Optional[datetime]: date and time at which the resource was archived,
     if it has been archived"""
 
-    status = properties.Optional(properties.String(), 'metadata.status.name', serializable=False)
-    """:Optional[str]: short description of the resource's status"""
-    status_detail = properties.List(properties.Object(StatusDetail), 'metadata.status.detail',
-                                    default=[], serializable=False)
-    """:List[StatusDetail]: a list of structured status info, containing the message and level"""
-
     _resource_type = ResourceTypeEnum.MODULE
 
     @property
     def is_archived(self):
         """:bool: whether the resource is archived (hidden but not deleted)."""
         return self.archived_by is not None
 
     def _post_dump(self, data: dict) -> dict:
         # Only the data portion of an entity is sent to the server.
         data = data["data"]
 
-        # Currently, name and description exists on both the data envelope and the config.
-        data["instance"]["name"] = data["name"]
-        data["instance"]["description"] = data["description"]
+        if "instance" in data:
+            # Currently, name and description exists on both the data envelope and the config.
+            data["instance"]["name"] = data["name"]
+            data["instance"]["description"] = data["description"]
 
         return super()._post_dump(data)
 
 
+# This class is the base type for the new module endpoints which do not support versions. If/once
+# they support versioning, they should be switched to inherit from VersionedEngineResource.
+class EngineResource(EngineResourceWithoutStatus[Self], IncludeParentProperties[Self]):
+    """Base resource for metadata from stand-alone AI Engine modules."""
+
+    status = properties.Optional(properties.String(), 'metadata.status.name', serializable=False)
+    """:Optional[str]: short description of the resource's status"""
+    status_detail = properties.List(properties.Object(StatusDetail), 'metadata.status.detail',
+                                    default=[], serializable=False)
+    """:List[StatusDetail]: a list of structured status info, containing the message and level"""
+
+    @classmethod
+    def build(cls, data: dict):
+        """Build an instance of this object from given data."""
+        return super().build_with_parent(data, __class__)
+
+
 class VersionedEngineResource(EngineResource[Self], IncludeParentProperties[Self]):
     """Base resource for metadata from stand-alone AI Engine modules which support versioning."""
 
     """:Integer: The version number of the resource."""
     version = properties.Optional(properties.Integer, 'metadata.version', serializable=False)
 
     """:Boolean: The draft status of the resource."""
```

### Comparing `citrine-3.1.0/src/citrine/_rest/pageable.py` & `citrine-3.2.4/src/citrine/_rest/pageable.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_rest/paginator.py` & `citrine-3.2.4/src/citrine/_rest/paginator.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_rest/resource.py` & `citrine-3.2.4/src/citrine/_rest/resource.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_serialization/include_parent_properties.py` & `citrine-3.2.4/src/citrine/_serialization/include_parent_properties.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_serialization/polymorphic_serializable.py` & `citrine-3.2.4/src/citrine/_serialization/polymorphic_serializable.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_serialization/properties.py` & `citrine-3.2.4/src/citrine/_serialization/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,16 @@
             return arrow.get(value).datetime
         if isinstance(value, int):
             # Backend returns time as ms since epoch, but arrow expects seconds since epoch
             return arrow.get(value / 1000).datetime
         raise TypeError("{} must be an int or a string".format(value))
 
     def _serialize(self, value: datetime) -> int:
-        return int(arrow.get(value).float_timestamp * 1000)
+        # Add 100 nanoseconds to avoid floating point truncation issues from microseconds
+        return int(arrow.get(value).float_timestamp * 1000 + 0.0001)
 
 
 class List(PropertyCollection[list, list]):
 
     def __init__(self,
                  element_type: typing.Union[Property, typing.Type[Property]],
                  serialization_path: typing.Optional[str] = None,
```

### Comparing `citrine-3.1.0/src/citrine/_serialization/serializable.py` & `citrine-3.2.4/src/citrine/_serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_session.py` & `citrine-3.2.4/src/citrine/_session.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_utils/batcher.py` & `citrine-3.2.4/src/citrine/_utils/batcher.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_utils/functions.py` & `citrine-3.2.4/src/citrine/_utils/functions.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/_utils/template_util.py` & `citrine-3.2.4/src/citrine/_utils/template_util.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/citrine.py` & `citrine-3.2.4/src/citrine/citrine.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/exceptions.py` & `citrine-3.2.4/src/citrine/exceptions.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/gemd_queries/criteria.py` & `citrine-3.2.4/src/citrine/gemd_queries/criteria.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/gemd_queries/filter.py` & `citrine-3.2.4/src/citrine/gemd_queries/filter.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/gemd_queries/gemd_query.py` & `citrine-3.2.4/src/citrine/gemd_queries/gemd_query.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/gemtables/columns.py` & `citrine-3.2.4/src/citrine/gemtables/columns.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/gemtables/rows.py` & `citrine-3.2.4/src/citrine/gemtables/rows.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/gemtables/variables.py` & `citrine-3.2.4/src/citrine/gemtables/variables.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/catalyst/assistant.py` & `citrine-3.2.4/src/citrine/informatics/catalyst/assistant.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/catalyst/insights.py` & `citrine-3.2.4/src/citrine/informatics/catalyst/insights.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/categorical_constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/categorical_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/ingredient_count_constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/ingredient_count_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/ingredient_fraction_constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/ingredient_fraction_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/ingredient_ratio_constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/ingredient_ratio_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/integer_range_constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/integer_range_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/label_fraction_constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/label_fraction_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/constraints/scalar_range_constraint.py` & `citrine-3.2.4/src/citrine/informatics/constraints/scalar_range_constraint.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/data_sources.py` & `citrine-3.2.4/src/citrine/informatics/data_sources.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/descriptors.py` & `citrine-3.2.4/src/citrine/informatics/descriptors.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_candidate.py` & `citrine-3.2.4/src/citrine/informatics/design_candidate.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_spaces/data_source_design_space.py` & `citrine-3.2.4/src/citrine/informatics/design_spaces/data_source_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_spaces/design_space.py` & `citrine-3.2.4/src/citrine/informatics/design_spaces/design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_spaces/enumerated_design_space.py` & `citrine-3.2.4/src/citrine/informatics/design_spaces/enumerated_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_spaces/formulation_design_space.py` & `citrine-3.2.4/src/citrine/informatics/design_spaces/formulation_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_spaces/hierarchical_design_space.py` & `citrine-3.2.4/src/citrine/informatics/design_spaces/hierarchical_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_spaces/product_design_space.py` & `citrine-3.2.4/src/citrine/informatics/design_spaces/product_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/design_spaces/sample_design_space.py` & `citrine-3.2.4/src/citrine/informatics/design_spaces/sample_design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/dimensions.py` & `citrine-3.2.4/src/citrine/informatics/dimensions.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/executions/design_execution.py` & `citrine-3.2.4/src/citrine/informatics/executions/design_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/executions/execution.py` & `citrine-3.2.4/src/citrine/informatics/executions/execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/executions/generative_design_execution.py` & `citrine-3.2.4/src/citrine/informatics/executions/generative_design_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/executions/predictor_evaluation_execution.py` & `citrine-3.2.4/src/citrine/informatics/executions/predictor_evaluation_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/executions/sample_design_space_execution.py` & `citrine-3.2.4/src/citrine/informatics/executions/sample_design_space_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     """The execution of a Sample Design Space task.
 
     Possible statuses are INPROGRESS, SUCCEEDED, and FAILED.
     Additional fields ``status_description`` and ``status_detail`` provide more information.
 
     """
 
+    _api_version = 'v3'
     design_space_id: Optional[UUID] = None
 
     def _path(self):
         return format_escaped_url(
             '/projects/{project_id}/design-spaces/{design_space_id}/sample/',
             project_id=self.project_id,
             design_space_id=self.design_space_id,
```

### Comparing `citrine-3.1.0/src/citrine/informatics/experiment_values.py` & `citrine-3.2.4/src/citrine/informatics/experiment_values.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/generative_design.py` & `citrine-3.2.4/src/citrine/informatics/generative_design.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/objectives.py` & `citrine-3.2.4/src/citrine/informatics/objectives.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predict_request.py` & `citrine-3.2.4/src/citrine/informatics/predict_request.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictor_evaluation_metrics.py` & `citrine-3.2.4/src/citrine/informatics/predictor_evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictor_evaluation_result.py` & `citrine-3.2.4/src/citrine/informatics/predictor_evaluation_result.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictor_evaluator.py` & `citrine-3.2.4/src/citrine/informatics/predictor_evaluator.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/__init__.py` & `citrine-3.2.4/src/citrine/informatics/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/auto_ml_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/auto_ml_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/chemical_formula_featurizer.py` & `citrine-3.2.4/src/citrine/informatics/predictors/chemical_formula_featurizer.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/expression_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/expression_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/graph_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/graph_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/ingredient_fractions_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/ingredient_fractions_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/ingredients_to_formulation_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/ingredients_to_formulation_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/label_fractions_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/label_fractions_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/mean_property_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/mean_property_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/molecular_structure_featurizer.py` & `citrine-3.2.4/src/citrine/informatics/predictors/molecular_structure_featurizer.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/node.py` & `citrine-3.2.4/src/citrine/informatics/predictors/node.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/simple_mixture_predictor.py` & `citrine-3.2.4/src/citrine/informatics/predictors/simple_mixture_predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/single_predict_request.py` & `citrine-3.2.4/src/citrine/informatics/predictors/single_predict_request.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/predictors/single_prediction.py` & `citrine-3.2.4/src/citrine/informatics/predictors/single_prediction.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/reports.py` & `citrine-3.2.4/src/citrine/informatics/reports.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/scores.py` & `citrine-3.2.4/src/citrine/informatics/scores.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/workflows/design_workflow.py` & `citrine-3.2.4/src/citrine/informatics/workflows/design_workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/workflows/predictor_evaluation_workflow.py` & `citrine-3.2.4/src/citrine/informatics/workflows/predictor_evaluation_workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/informatics/workflows/workflow.py` & `citrine-3.2.4/src/citrine/informatics/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/jobs/job.py` & `citrine-3.2.4/src/citrine/jobs/job.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/jobs/waiting.py` & `citrine-3.2.4/src/citrine/jobs/waiting.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/api_error.py` & `citrine-3.2.4/src/citrine/resources/api_error.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/attribute_templates.py` & `citrine-3.2.4/src/citrine/resources/attribute_templates.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/audit_info.py` & `citrine-3.2.4/src/citrine/resources/audit_info.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/branch.py` & `citrine-3.2.4/src/citrine/resources/branch.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/catalyst.py` & `citrine-3.2.4/src/citrine/resources/catalyst.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/condition_template.py` & `citrine-3.2.4/src/citrine/resources/condition_template.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/data_concepts.py` & `citrine-3.2.4/src/citrine/resources/data_concepts.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/data_objects.py` & `citrine-3.2.4/src/citrine/resources/data_objects.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/data_version_update.py` & `citrine-3.2.4/src/citrine/resources/data_version_update.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/dataset.py` & `citrine-3.2.4/src/citrine/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/delete.py` & `citrine-3.2.4/src/citrine/resources/delete.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/descriptors.py` & `citrine-3.2.4/src/citrine/resources/descriptors.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/design_execution.py` & `citrine-3.2.4/src/citrine/resources/design_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/design_space.py` & `citrine-3.2.4/src/citrine/resources/design_space.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/design_workflow.py` & `citrine-3.2.4/src/citrine/resources/design_workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/experiment_datasource.py` & `citrine-3.2.4/src/citrine/resources/experiment_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,24 @@
     def __init__(self, *args, **kwargs):
         """Experiment data sources are not directly instantiated by the user."""
         pass  # pragma: no cover
 
     def read(self) -> str:
         """Read this experiment data source into a CSV.
 
-        Each row will be a single experiement from this data source, and each column is a variable
-        which is overriden in any of the experiements in this data source. If an experiement did
+        Each row will be a single experiment from this data source, and each column is a variable
+        which is overriden in any of the experiments in this data source. If an experiment did
         not override a variable, its cell will be left empty.
 
         All cells can be deserialized as JSON. Most of them will simply be strings or numbers. But
         if present,the "Formulation" cell will contain an escaped JSON string, which will
         deserialize into a mapping from ingredient names to floating-point values.
         """
         overrides = [experiment._overrides_json() for experiment in self.experiments]
-        columns = {key for override in overrides for key in override.keys()}
+        columns = {key for override in overrides for key in override}
         sorted_columns = sorted(list(columns), key=str.lower)
 
         buffer = StringIO()
         writer = csv.DictWriter(buffer, sorted_columns)
         writer.writeheader()
         writer.writerows(overrides)
```

### Comparing `citrine-3.1.0/src/citrine/resources/file_link.py` & `citrine-3.2.4/src/citrine/resources/file_link.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/gemd_resource.py` & `citrine-3.2.4/src/citrine/resources/gemd_resource.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/gemtables.py` & `citrine-3.2.4/src/citrine/resources/gemtables.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/generative_design_execution.py` & `citrine-3.2.4/src/citrine/resources/generative_design_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/ingestion.py` & `citrine-3.2.4/src/citrine/resources/ingestion.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/ingredient_run.py` & `citrine-3.2.4/src/citrine/resources/ingredient_run.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/ingredient_spec.py` & `citrine-3.2.4/src/citrine/resources/ingredient_spec.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/material_run.py` & `citrine-3.2.4/src/citrine/resources/material_run.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/material_spec.py` & `citrine-3.2.4/src/citrine/resources/material_spec.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/material_template.py` & `citrine-3.2.4/src/citrine/resources/material_template.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/measurement_run.py` & `citrine-3.2.4/src/citrine/resources/measurement_run.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/measurement_spec.py` & `citrine-3.2.4/src/citrine/resources/measurement_spec.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/measurement_template.py` & `citrine-3.2.4/src/citrine/resources/measurement_template.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/object_runs.py` & `citrine-3.2.4/src/citrine/resources/object_runs.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/object_specs.py` & `citrine-3.2.4/src/citrine/resources/object_specs.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/object_templates.py` & `citrine-3.2.4/src/citrine/resources/object_templates.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/parameter_template.py` & `citrine-3.2.4/src/citrine/resources/parameter_template.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/predictor.py` & `citrine-3.2.4/src/citrine/resources/predictor.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/predictor_evaluation_execution.py` & `citrine-3.2.4/src/citrine/resources/predictor_evaluation_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/predictor_evaluation_workflow.py` & `citrine-3.2.4/src/citrine/resources/predictor_evaluation_workflow.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/process_run.py` & `citrine-3.2.4/src/citrine/resources/process_run.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/process_spec.py` & `citrine-3.2.4/src/citrine/resources/process_spec.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/process_template.py` & `citrine-3.2.4/src/citrine/resources/process_template.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/project.py` & `citrine-3.2.4/src/citrine/resources/project.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/project_member.py` & `citrine-3.2.4/src/citrine/resources/project_member.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/property_template.py` & `citrine-3.2.4/src/citrine/resources/property_template.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/report.py` & `citrine-3.2.4/src/citrine/resources/report.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/response.py` & `citrine-3.2.4/src/citrine/resources/response.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/sample_design_space_execution.py` & `citrine-3.2.4/src/citrine/resources/sample_design_space_execution.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/status_detail.py` & `citrine-3.2.4/src/citrine/resources/status_detail.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/table_config.py` & `citrine-3.2.4/src/citrine/resources/table_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,25 @@
       material, splitting the graph at branches.
     """
 
     SINGLE_ROW = "single_row"
     FORMULATIONS = "formulations"
 
 
+class TableConfigInitiator(BaseEnumeration):
+    """Which client registered this table config.
+
+    * CITRINE_PYTHON corresponds to this library
+    * UI corresponds to the Citrine Platform browser interface
+    """
+
+    CITRINE_PYTHON = "CITRINE_PYTHON"
+    UI = "UI"
+
+
 class TableConfig(Resource["TableConfig"]):
     """
     The Table Configuration used to build GEM Tables.
 
     Parameters
     ----------
     name: str
```

### Comparing `citrine-3.1.0/src/citrine/resources/team.py` & `citrine-3.2.4/src/citrine/resources/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from uuid import UUID
 
 from citrine._rest.admin_collection import AdminCollection
 from citrine._rest.resource import Resource, ResourceTypeEnum
 from citrine._serialization import properties
 from citrine._session import Session
 from citrine._utils.functions import format_escaped_url
+from citrine.resources.analysis_workflow import AnalysisWorkflowCollection
 from citrine.resources.project import ProjectCollection
 from citrine.resources.user import User, UserCollection
 
 WRITE = "WRITE"
 READ = "READ"
 SHARE = "SHARE"
 TEAM_ACTIONS = Union[WRITE, READ, SHARE]
@@ -355,14 +356,19 @@
 
     @property
     def projects(self) -> ProjectCollection:
         """Return a resource representing all visible projects in this team."""
         return ProjectCollection(self.session, team_id=self.uid)
 
     @property
+    def analyses(self) -> AnalysisWorkflowCollection:
+        """Return a resource representing all visible analysis workflows in this team."""
+        return AnalysisWorkflowCollection(session=self.session, team_id=self.uid)
+
+    @property
     def dataset_ids(self) -> TeamResourceIDs:
         """Return a TeamResourceIDs instance for listing published dataset IDs."""
         return TeamResourceIDs(session=self.session,
                                team_id=self.uid,
                                resource_type=ResourceTypeEnum.DATASET.value)
 
     @property
```

### Comparing `citrine-3.1.0/src/citrine/resources/templates.py` & `citrine-3.2.4/src/citrine/resources/templates.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/resources/user.py` & `citrine-3.2.4/src/citrine/resources/user.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/seeding/find_or_create.py` & `citrine-3.2.4/src/citrine/seeding/find_or_create.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine/seeding/sort_gems.py` & `citrine-3.2.4/src/citrine/seeding/sort_gems.py`

 * *Files identical despite different names*

### Comparing `citrine-3.1.0/src/citrine.egg-info/PKG-INFO` & `citrine-3.2.4/src/citrine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrine
-Version: 3.1.0
+Version: 3.2.4
 Summary: Python library for the Citrine Platform
 Home-page: http://github.com/CitrineInformatics/citrine-python
 Author: Citrine Informatics
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `citrine-3.1.0/src/citrine.egg-info/SOURCES.txt` & `citrine-3.2.4/src/citrine.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -90,21 +90,23 @@
 src/citrine/informatics/predictors/molecular_structure_featurizer.py
 src/citrine/informatics/predictors/node.py
 src/citrine/informatics/predictors/predictor.py
 src/citrine/informatics/predictors/simple_mixture_predictor.py
 src/citrine/informatics/predictors/single_predict_request.py
 src/citrine/informatics/predictors/single_prediction.py
 src/citrine/informatics/workflows/__init__.py
+src/citrine/informatics/workflows/analysis_workflow.py
 src/citrine/informatics/workflows/design_workflow.py
 src/citrine/informatics/workflows/predictor_evaluation_workflow.py
 src/citrine/informatics/workflows/workflow.py
 src/citrine/jobs/__init__.py
 src/citrine/jobs/job.py
 src/citrine/jobs/waiting.py
 src/citrine/resources/__init__.py
+src/citrine/resources/analysis_workflow.py
 src/citrine/resources/api_error.py
 src/citrine/resources/attribute_templates.py
 src/citrine/resources/audit_info.py
 src/citrine/resources/branch.py
 src/citrine/resources/catalyst.py
 src/citrine/resources/condition_template.py
 src/citrine/resources/data_concepts.py
```

