# Comparing `tmp/pinjected-0.2.61.tar.gz` & `tmp/pinjected-0.2.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.61.tar", max compression
+gzip compressed data, was "pinjected-0.2.62.tar", max compression
```

## Comparing `pinjected-0.2.61.tar` & `pinjected-0.2.62.tar`

### file list

```diff
@@ -1,91 +1,93 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.61/LICENSE
--rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.61/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.61/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.61/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.61/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.61/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.61/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5851 2024-05-10 02:53:28.124125 pinjected-0.2.61/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.61/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7866 2024-05-10 03:03:16.666241 pinjected-0.2.61/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.61/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.61/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.61/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14766 2024-05-08 06:09:38.125434 pinjected-0.2.61/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.61/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.61/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.61/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.61/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.61/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54691 2024-05-10 03:24:47.083934 pinjected-0.2.61/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.61/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.61/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.61/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.61/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.61/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.61/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.61/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.61/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.61/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.61/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.61/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.61/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.61/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.61/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.61/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.61/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.61/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.61/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.61/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.61/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.61/pinjected/di/util.py
--rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.61/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.61/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.61/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.61/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.61/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.61/pinjected/global_configs.py
--rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.61/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.61/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.61/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.61/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.61/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.61/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.61/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.61/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.61/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.61/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.61/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.61/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.61/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.61/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.61/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.61/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.61/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.61/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.61/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.61/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.61/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.61/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.61/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.61/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.61/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9601 2024-05-01 11:59:22.455243 pinjected-0.2.61/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.61/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.61/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.61/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.61/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.61/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.61/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.61/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.61/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.61/pinjected/v2/di.py
--rw-r--r--   0        0        0      524 2024-05-01 08:03:21.521914 pinjected-0.2.61/pinjected/v2/keys.py
--rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.61/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0    24362 2024-05-10 07:07:48.783021 pinjected-0.2.61/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19559 2024-05-10 07:01:11.242869 pinjected-0.2.61/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.61/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.61/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.61/pinjected/with_context.py
--rw-r--r--   0        0        0      656 2024-05-10 07:09:18.019487 pinjected-0.2.61/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.61/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.62/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.62/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.62/pinjected/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:51:53.980366 pinjected-0.2.62/pinjected/compatibility/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-14 16:55:01.337952 pinjected-0.2.62/pinjected/compatibility/task_group.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.62/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.62/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.62/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.62/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5898 2024-05-13 08:52:30.783178 pinjected-0.2.62/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.62/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7866 2024-05-10 03:03:16.666241 pinjected-0.2.62/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.62/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.62/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-05-14 11:27:40.261061 pinjected-0.2.62/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14572 2024-05-14 13:17:02.297068 pinjected-0.2.62/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.62/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.62/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.62/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.62/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.62/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    56046 2024-05-14 11:34:43.296359 pinjected-0.2.62/pinjected/di/injected.py
+-rw-r--r--   0        0        0     2988 2024-05-14 06:50:46.840175 pinjected-0.2.62/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.62/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.62/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.62/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.62/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.62/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.62/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.62/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.62/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.62/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.62/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.62/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.62/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.62/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.62/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.62/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.62/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-05-14 10:11:59.767149 pinjected-0.2.62/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.62/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.62/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.62/pinjected/di/util.py
+-rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.62/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.62/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.62/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.62/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.62/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.62/pinjected/global_configs.py
+-rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.62/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.62/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.62/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.62/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.62/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.62/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.62/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.62/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.62/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.62/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.62/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.62/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.62/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.62/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.62/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.62/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.62/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.62/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.62/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.62/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.62/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.62/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.62/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.62/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.62/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9628 2024-05-14 16:55:01.331049 pinjected-0.2.62/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.62/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.62/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.62/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.62/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.62/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.62/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.62/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.62/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.62/pinjected/v2/di.py
+-rw-r--r--   0        0        0      524 2024-05-01 08:03:21.521914 pinjected-0.2.62/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.62/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0    24649 2024-05-14 09:53:00.963950 pinjected-0.2.62/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    20026 2024-05-14 08:55:44.478760 pinjected-0.2.62/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.62/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.62/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.62/pinjected/with_context.py
+-rw-r--r--   0        0        0      656 2024-05-14 16:55:07.998714 pinjected-0.2.62/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.62/PKG-INFO
```

### Comparing `pinjected-0.2.61/LICENSE` & `pinjected-0.2.62/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/decoration.py` & `pinjected-0.2.62/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/demo.py` & `pinjected-0.2.62/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/app_designed.py` & `pinjected-0.2.62/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/app_injected.py` & `pinjected-0.2.62/pinjected/di/app_injected.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     def dependencies(self) -> Set[str]:
         return self.value.dependencies()
 
     def get_provider(self):
         return self.value.get_provider()
 
     def __str__(self):
-        return f"EvaledInjected(value={self.value},ast={show_expr(self.ast, reduce_injected_expr)})"
+        #return f"EvaledInjected(value={self.value},ast={show_expr(self.ast, reduce_injected_expr)})"
+        return f"Eval({show_expr(self.ast)})"
 
     def __repr__(self):
         return str(self)
 
     def repr_ast(self):
         return show_expr(self.ast, reduce_injected_expr)
```

### Comparing `pinjected-0.2.61/pinjected/di/applicative.py` & `pinjected-0.2.62/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/ast.py` & `pinjected-0.2.62/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/decorators.py` & `pinjected-0.2.62/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/design.py` & `pinjected-0.2.62/pinjected/di/design.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import inspect
 from copy import copy
 from dataclasses import dataclass, field, replace
 from functools import wraps
-from pathlib import Path
-from pprint import pformat
-from typing import TypeVar, List, Dict, Union, Callable, Type, Self
+from typing import TypeVar, List, Dict, Union, Callable, Type
 
 from cytoolz import merge
 from makefun import create_function
 
 from pinjected.di.app_injected import EvaledInjected
 from pinjected.di.graph import DependencyResolver
 from pinjected.di.implicit_globals import IMPLICIT_BINDINGS
@@ -213,15 +211,14 @@
             res += Design(
                 bindings={key: bind.update_metadata(meta)}
             )
         return res
 
     def to_resolver(self):
         from pinjected.v2.resolver import AsyncResolver,BaseResolverCallback
-        from loguru import logger
         bindings = {**IMPLICIT_BINDINGS, **self.bindings}
         callback = BaseResolverCallback()
         return AsyncResolver(
             Design(bindings=bindings, modules=self.modules),
             callbacks=[
                 callback
             ]
@@ -393,24 +390,21 @@
     src: Design
     init_frame: inspect.FrameInfo
 
     def __post_init__(self):
         # get parent global variables
         parent_globals = self.init_frame.f_globals
         global_ids = {k: id(v) for k, v in parent_globals.items()}
-        from loguru import logger
         # logger.debug(f"enter->\n"+pformat(global_ids))
         self.last_global_ids = global_ids
 
     def exit(self, frame: inspect.FrameInfo) -> list[ModuleVarPath]:
-        from loguru import logger
         # get parent global variables
         parent_globals = frame.f_globals
         global_ids = {k: id(v) for k, v in parent_globals.items()}
-        from loguru import logger
         # logger.debug("exit->\n"+pformat(global_ids))
         changed_keys = []
         for k in global_ids:
             if k in self.last_global_ids:
                 if global_ids[k] != self.last_global_ids[k]:
                     changed_keys.append(k)
             else:
```

### Comparing `pinjected-0.2.61/pinjected/di/designed.py` & `pinjected-0.2.62/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.62/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/graph.py` & `pinjected-0.2.62/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/injected.py` & `pinjected-0.2.62/pinjected/di/injected.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 import functools
 import hashlib
 import inspect
 import sys
 from copy import copy
 from dataclasses import dataclass, field
-from inspect import Traceback
+from inspect import Traceback, iscoroutinefunction
 from pathlib import Path
 from typing import List, Generic, Union, Callable, TypeVar, Tuple, Set, Dict, Any, Awaitable
 
 from frozendict import frozendict
 from loguru import logger
 from makefun import create_function
 from returns.result import safe
@@ -367,15 +367,15 @@
         # logger.info(f"injection_targets:{injection_targets}")
         injected_kwargs = Injected.dict(**injection_targets)
         # logger.info(f"injected_kwargs:{injected_kwargs}")
         # hmm?
         # Ah, so upon calling instance.method(), we need to manually check if __self__ is present?
         bound_func = Injected.bind(makefun_impl, injected_kwargs=injected_kwargs)
         bound_func.__is_async_function__ = inspect.iscoroutinefunction(original_function)
-        bound_func.__is_partial__ = True # this is to indicate that the bound_func is supposed to be used with PartialInjectedFunction.
+        bound_func.__is_partial__ = True  # this is to indicate that the bound_func is supposed to be used with PartialInjectedFunction.
         injected_factory = PartialInjectedFunction(src=bound_func)
         # the inner will be called upon calling the injection result.
         # This involves many internal Injecte instances. can I make it simler?
         # it takes *by_name, mzip, and map.
         injected_factory.__is_async_function__ = bound_func.__is_async_function__
         injected_factory.__runnable_metadata__ = {
             "kind": "callable"
@@ -496,29 +496,44 @@
         else:
             new_f = f
         return MappedInjected(self, new_f, original_mapper=f)
 
     def from_impl(impl: Callable, dependencies: Set[str]):
         return GeneratedInjected(impl, dependencies)
 
+    def _faster_get_metadata(self):
+        # logger.info(f"faster_get_metadata for Injected.pure")
+        try:
+            frame = sys._getframe().f_back.f_back
+            mod = frame.f_globals["__name__"]
+            name = frame.f_code.co_filename
+            # return f"{mod.replace('.', '_')}_L_{name}".replace("<", "__").replace(">", "__")
+            return mod, name
+        except Exception as e:
+            # from loguru import logger
+            logger.warning(f"failed to get name of the injected location, due to {e}")
+            return f"__unknown_module__maybe_due_to_pickling__", "unknown_location"
+
     @staticmethod
     def pure(value):
         res = InjectedPure(value)
         # I need to set the file that called this function.
-        #res.__definition_frame__ = get_frame_info(2)
-        fi = get_frame_info(2)
-        res.__definition_module__ = fi.original_frame.f_globals["__name__"]
-        res.__original_file__ = fi.filename
+        # res.__definition_frame__ = get_frame_info(2)
+        # fi = get_frame_info(2)
+        res.__definition_module__, res.__original_file__ = res._faster_get_metadata()
+        # res.__definition_module__ = fi.original_frame.f_globals["__name__"]
+        # res.__original_file__ = fi.filename
         return res
 
     @staticmethod
     def by_name(name: str):
         return InjectedByName(name, )
 
     def zip(self, other: "Injected[U]") -> "Injected[Tuple[T,U]]":
+        other = Injected.ensure_injected(other)
         assert isinstance(self, Injected)
         assert isinstance(other, Injected)
         return Injected.mzip(self, other)
 
     @staticmethod
     def mzip(*srcs: "Injected"):
         srcs = [Injected.ensure_injected(s) for s in srcs]
@@ -569,17 +584,17 @@
         return self.zip(other).map(
             lambda t: lambda *args, **kwargs: t[1](t[0](*args, **kwargs))
         )
 
     @staticmethod
     def dict(**kwargs: "Injected") -> "Injected[Dict]":
         # raise RuntimeError("disabled")
-        #keys = list(kwargs.keys())
+        # keys = list(kwargs.keys())
 
-        #return Injected.mzip(*[kwargs[k] for k in keys]).map(lambda t: {k: v for k, v in zip(keys, t)})
+        # return Injected.mzip(*[kwargs[k] for k in keys]).map(lambda t: {k: v for k, v in zip(keys, t)})
         return DictInjected(**kwargs)
 
     @property
     def proxy(self) -> DelegatedVar:
         """use this to modify injected variables freely without map.
         call eval() at the end to finish modification
         # it seems this thing is preventing from pickling?
@@ -741,29 +756,28 @@
     program: Injected[T]
     program_dependencies: List[Injected]
 
     def __post_init__(self):
         self.program = Injected.ensure_injected(self.program)
 
         async def impl(t):
-            resolver,cache,*deps = t
+            resolver, cache, *deps = t
             logger.info(f"Checking for cache with deps:{deps}")
             sha256_key = hashlib.sha256(str(deps).encode()).hexdigest()
             hash_key = sha256_key
             if hash_key not in cache:
                 logger.info(f"Cache miss for {deps}")
                 data = await resolver[self.program]
                 cache[hash_key] = data
             else:
                 logger.info(f"Cache hit for {deps},loading ...")
             res = cache[hash_key]
             logger.info(f"Cache hit for {deps}, loaded")
             return res
 
-
         self.impl = Injected.list(
             Injected.by_name("__resolver__"),
             self.cache,
             *self.program_dependencies
         ).map(impl)
         assert isinstance(self.impl, Injected)
         assert isinstance(self.program, Injected)
@@ -1008,32 +1022,39 @@
         return kwargs[dep]
     elif isinstance(dep, DelegatedVar):
         return await solve_injection(dep.eval(), kwargs)
     elif isinstance(dep, Injected):
         return await solve_injection(dep.get_provider(), kwargs)
     elif isinstance(dep, (type, Callable)) and inspect.iscoroutinefunction(dep):
         return await dep(**{k: kwargs[k] for k in extract_dependency(dep)})
+    elif isinstance(dep, (type, Callable)):
+        return dep(**{k: kwargs[k] for k in extract_dependency(dep)})
     else:
         raise RuntimeError(f"dep must be one of str/type/Callable/Injected. got {type(dep)}")
 
 
 def combine_image_store(a, b):
     # do anything
     return a + b
 
 
 def assert_kwargs_type(v):
+    if isinstance(v, DelegatedVar):
+        return
+    if v == abc.ABCMeta:
+        raise TypeError(f"Unexpected: {v}")
     if isinstance(v, str):
         return
     if isinstance(v, type):
         return
     if isinstance(v, Callable):
         return
     if isinstance(v, Injected):
         return
+
     else:
         raise TypeError(f"{type(v)} is not any of [str,type,Callable,Injected],but {v}")
 
 
 class InjectedFunction(Injected[T]):
     # since the behavior differs in classes extending Generic[T]
     __match_args__ = ("target_function", "kwargs_mapping")
@@ -1049,17 +1070,20 @@
         super().__init__()
         assert not isinstance(target_function, (Injected, DelegatedVar))
         assert callable(target_function)
         self.target_function = target_function
         assert inspect.iscoroutinefunction(self.target_function), f"{self.target_function} is not a coroutine function"
         self.kwargs_mapping = copy(kwargs_mapping)
         for k, v in self.kwargs_mapping.items():
-            assert_kwargs_type(v)
             if isinstance(v, DelegatedVar):
-                self.kwargs_mapping[k] = v.eval()
+                v = v.eval()
+                self.kwargs_mapping[k] = v
+            assert_kwargs_type(v)
+            if v == abc.ABCMeta:
+                raise TypeError(f"Unexpected kwargs set.{k}:{v}")
         # logger.info(f"InjectedFunction:{self.target_function} kwargs_mapping:{self.kwargs_mapping}")
         org_deps = extract_dependency(self.target_function)
         logger.trace(f"tgt:{target_function} original dependency:{org_deps}")
         missings = {d for d in org_deps if d not in self.kwargs_mapping}
         logger.trace(f"now missing {missings}")
         # logger.warning(f"created InjectedFunction:{inspect.signature(target_function)}")
         # assert "self" not in inspect.signature(target_function).parameters
@@ -1076,15 +1100,19 @@
 
             async def update(key):
                 if key not in deps:
                     if key in self.kwargs_mapping:
                         mapped = self.kwargs_mapping[key]
                     else:
                         mapped = key
-                    deps[key] = await solve_injection(mapped, kwargs)
+                    try:
+                        deps[key] = await solve_injection(mapped, kwargs)
+                    except Exception as e:
+                        logger.error(f"failed to solve injection for {key}:{mapped} from {kwargs}")
+                        raise e
 
             tasks = []
             logger.trace(f"missings:{self.missings},kwargs_mapping:{self.kwargs_mapping}")
             for mdep in self.missings:
                 tasks.append(update(mdep))
             for k, dep in self.kwargs_mapping.items():
                 tasks.append(update(k))
@@ -1117,18 +1145,18 @@
 
     # def __str__(self):
     #    return f"""InjectedFunction(target={self.target_function},kwargs_mapping={self.kwargs_mapping})"""
     def dynamic_dependencies(self) -> Set[str]:
         return set()
 
     def __repr_expr__(self):
-        func_name = self.original_function.__name__
-        orig_file = Path(self.original_function.__original_file__)
-        orig_line = self.original_function.__original_code__
-        #return f"<f {func_name}@{orig_file.name}>"
+        # func_name = self.original_function.__name__
+        # orig_file = Path(self.original_function.__original_file__)
+        # orig_line = self.original_function.__original_code__
+        # return f"<f {func_name}@{orig_file.name}>"
         return self.original_function.__name__
 
 
 class InjectedPure(Injected[T]):
     __match_args__ = ("value",)
 
     def __init__(self, value):
@@ -1244,14 +1272,15 @@
     def dynamic_dependencies(self) -> Set[str]:
         res = set()
         for s in self.srcs:
             res |= s.dynamic_dependencies()
 
         return res
 
+
 class DictInjected(Injected):
     __match_args__ = ("srcs",)
 
     def __init__(self, **srcs: Injected):
         super().__init__()
         self.srcs = {k: Injected.ensure_injected(v) for k, v in srcs.items()}
         assert all(isinstance(s, Injected) for s in self.srcs.values()), self.srcs
@@ -1279,14 +1308,15 @@
     def dynamic_dependencies(self) -> Set[str]:
         res = set()
         for s in self.srcs.values():
             res |= s.dynamic_dependencies()
 
         return res
 
+
 def _injected_factory(**targets: Injected):
     def _impl(f):
         return Injected.partial(f, **targets)
 
     return _impl
```

### Comparing `pinjected-0.2.61/pinjected/di/injected_analysis.py` & `pinjected-0.2.62/pinjected/di/injected_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import sys
+from loguru import logger
 
-def get_instance_origin(package_name):
+def get_instance_origin_slow(package_name):
     from loguru import logger
     # Get the current frame
     #logger.debug(f"trying to get the instance origin")
 
 
     current_frame = sys._getframe()
 
@@ -27,14 +28,44 @@
             # maybe this is taking so much time?
             #logger.debug(f"found instance origin:{frame_info.filename}")
             return frame_info
 
         # Move to the next frame in the call stack
         current_frame = current_frame.f_back
 
+
+def get_instance_origin(package_name):
+    #logger.debug("Trying to get the instance origin")
+
+    current_frame = sys._getframe()
+
+    # Go up the call stack to find the frame outside the given package
+    while current_frame:
+        # Check if the frame's module is not in the specified package
+        module_name = current_frame.f_globals.get("__name__")
+        if module_name and not module_name.startswith(package_name):
+            filename = current_frame.f_code.co_filename
+            lineno = current_frame.f_lineno
+            function_name = current_frame.f_code.co_name
+            # Log and return the frame information
+            #logger.debug(f"Found instance origin: {filename}")
+            return {
+                "filename": filename,
+                "lineno": lineno,
+                "function_name": function_name,
+                "module_name": module_name,
+            }
+
+        # Move to the next frame in the call stack
+        current_frame = current_frame.f_back
+
+    # Return None if no suitable frame is found
+    return None
+
+
 def get_instance_origin2(package_name):
     # Get the current frame
 
     current_frame = inspect.currentframe()
 
     # Go up the call stack to find the frame outside the given package
     while current_frame:
```

### Comparing `pinjected-0.2.61/pinjected/di/modular_injected.py` & `pinjected-0.2.62/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/overload_experimental.py` & `pinjected-0.2.62/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/proxiable.py` & `pinjected-0.2.62/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/session.py` & `pinjected-0.2.62/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/sessioned.py` & `pinjected-0.2.62/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/static_proxy.py` & `pinjected-0.2.62/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.62/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/test_graph.py` & `pinjected-0.2.62/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/test_injected.py` & `pinjected-0.2.62/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/tools/add_overload.py` & `pinjected-0.2.62/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/di/util.py` & `pinjected-0.2.62/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/exceptions.py` & `pinjected-0.2.62/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.62/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.62/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/graph_inspection.py` & `pinjected-0.2.62/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/helper_structure.py` & `pinjected-0.2.62/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/helpers.py` & `pinjected-0.2.62/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.62/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.62/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/ide_supports/default_design.py` & `pinjected-0.2.62/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.62/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.62/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/main_impl.py` & `pinjected-0.2.62/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/maybe_patch.py` & `pinjected-0.2.62/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/module_helper.py` & `pinjected-0.2.62/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/module_inspector.py` & `pinjected-0.2.62/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/module_var_path.py` & `pinjected-0.2.62/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/notification.py` & `pinjected-0.2.62/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/nx_graph_util.py` & `pinjected-0.2.62/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/run_config_utils.py` & `pinjected-0.2.62/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/run_config_utils_v2.py` & `pinjected-0.2.62/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/run_helpers/config.py` & `pinjected-0.2.62/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.62/pinjected/run_helpers/run_injected.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import inspect
 import os
-from asyncio import TaskGroup
 from pathlib import Path
 
 from pprint import pformat
 
 import asyncio
 
 from typing import Coroutine, Awaitable
 
 from loguru import logger
 from returns.result import safe, Result
 
 from pinjected import instances, Injected, Design, providers, Designed
+from pinjected.compatibility.task_group import TaskGroup
 from pinjected.di.design import DESIGN_OVERRIDES_STORE
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.helper_structure import MetaContext
 from pinjected.helpers import get_design_path_from_var_path
 from pinjected.module_var_path import ModuleVarPath, load_variable_by_module_path
 from pinjected.logging_helper import disable_internal_logging
 from pinjected.notification import notify
```

### Comparing `pinjected-0.2.61/pinjected/runnables.py` & `pinjected-0.2.62/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/test_package/__init__.py` & `pinjected-0.2.62/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/test_package/child/module1.py` & `pinjected-0.2.62/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/v2/ainjected.py` & `pinjected-0.2.62/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/v2/binds.py` & `pinjected-0.2.62/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/v2/di.py` & `pinjected-0.2.62/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/v2/keys.py` & `pinjected-0.2.62/pinjected/v2/keys.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/v2/provide_context.py` & `pinjected-0.2.62/pinjected/v2/provide_context.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.61/pinjected/v2/resolver.py` & `pinjected-0.2.62/pinjected/v2/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+from loguru import logger
+try:
+    import nest_asyncio
+    import uvloop
+    logger.error(f"nest_asyncio is disabled since uvloop is also installed! nest_asyncio.apply do not work with uvloop!")
+    nest_asyncio.apply = lambda:None
+except ImportError:
+    pass
+
+
+
+
 import asyncio
 import datetime
 import inspect
 import operator
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
@@ -325,42 +337,41 @@
                 if inspect.iscoroutinefunction(tgt):
                     return await data
                 else:
                     return data
             case _:
                 raise TypeError(f"tgt must be str, IBindKey, Callable or IBind, got {tgt}")
 
-    async def validate_provision(self,tgt:Providable):
+    async def validate_provision(self, tgt: Providable):
         logger.debug(f"validating provision...")
         from pinjected import Design
         from pinjected import providers
-        d:Design = self.design
+        d: Design = self.design
         errors = []
         match tgt:
             case Injected():
                 tmp_design = d + providers(__root__=tgt)
-                digraph:DIGraph = tmp_design.to_vis_graph()
+                digraph: DIGraph = tmp_design.to_vis_graph()
                 errors = list(digraph.di_dfs_validation("__root__"))
             case str():
-                digraph:DIGraph = d.to_vis_graph()
+                digraph: DIGraph = d.to_vis_graph()
                 errors = list(digraph.di_dfs_validation(tgt))
             case DelegatedVar() as dv:
                 tmp_design = d + providers(__root__=tgt)
-                digraph:DIGraph = tmp_design.to_vis_graph()
+                digraph: DIGraph = tmp_design.to_vis_graph()
                 errors = list(digraph.di_dfs_validation("__root__"))
             case f if callable(f):
                 tmp_design = d + providers(__root__=tgt)
-                digraph:DIGraph = tmp_design.to_vis_graph()
+                digraph: DIGraph = tmp_design.to_vis_graph()
                 errors = list(digraph.di_dfs_validation("__root__"))
 
         if errors:
-            raise DependencyResolutionError(f"Errors in dependency resolution: {pformat(errors)}",causes=errors)
+            raise DependencyResolutionError(f"Errors in dependency resolution: {pformat(errors)}", causes=errors)
         logger.debug(f"provision validated.")
 
-
     async def provide(self, tgt: Providable):
         await self.validate_provision(tgt)
         match tgt:
             case EvaledInjected(val, ast):
                 repr = show_expr(ast)
             case DelegatedVar(value, cxt) as dv:
                 repr = show_expr(dv.eval().ast)
@@ -399,30 +410,31 @@
             logger.info(f"waiting for {len(destructions)} destructors to finish.")
             results = await asyncio.gather(*destructions)
             logger.success(f"all destructors finished with results:{results}")
             self.destructed = True
             logger.success(f"Resolver destructed")
             return results
 
+
 @dataclass
 class ResolveStatus:
-    key:Any
-    kind:str # eval or provide
-    status:str
+    key: Any
+    kind: str  # eval or provide
+    status: str
     start: Optional[datetime.datetime]
     end: Optional[datetime.datetime]
 
 
 @dataclass
 class BaseResolverCallback(IResolverCallback):
     def __post_init__(self):
         self.request_status: dict[IBindKey, str] = {}
         self.logger = logger.opt(colors=True, ansi=True)
         self.eval_status: dict[str, str] = {}
-        self.total_status:dict[Union[IBindKey,str]] = {}
+        self.total_status: dict[Union[IBindKey, str]] = {}
 
     def __call__(self, event: ResolverEvent):
         if isinstance(event, RequestEvent):
             self.on_request(event)
         elif isinstance(event, ProvideEvent):
             self.on_provide(event)
         elif isinstance(event, DepsReadyEvent):
@@ -458,40 +470,39 @@
         done = ", ".join([self._colored_eval_key(k) for k in done])
         evaluating = ", ".join([self._colored_eval_key(k) for k in evaluating])
         calling = ", ".join([self._colored_eval_key(k) for k in calling])
         res = f"Awaiting:\t [{awaiting}]\nEvaluating:\t [{evaluating}]\nDone:\t\t [{done}]\nCalling:\t [{calling}]"
         return res
 
     def total_status_string(self):
-        res ="\n===== RESOLVER STATUS =====\n"
-        for k,v in self.state_string_dict().items():
+        res = "\n===== RESOLVER STATUS =====\n"
+        for k, v in self.state_string_dict().items():
             vals = list(v.values())
             res += f"{k}:\t"
             if vals:
                 res += f"[{', '.join(vals[:10])}]\n"
             else:
                 res += "[]\n"
             if len(v.values()) >= 10:
-                res += f"and {len(vals)-10} more...\n"
+                res += f"and {len(vals) - 10} more...\n"
         return res
 
-
     def state_string_dict(self):
         provided = [k for k in self.request_status if self.request_status[k] == "provided"]
         provided = {k: self._colored_key(k) for k in provided[:10]}
         running = [k for k in self.request_status if self.request_status[k] == "running"]
         running = {k: self._colored_key(k) for k in running}
         waiting = [k for k in self.request_status if self.request_status[k] == "waiting"]
         waiting = {k: self._colored_key(k) for k in waiting}
 
         eval_awaiting = [k for k in self.eval_status if self.eval_status[k] == "await"]
         eval_awaiting = {k: self._colored_eval_key(k) for k in eval_awaiting}
         eval_done = [k for k in self.eval_status if self.eval_status[k] == "done"]
         eval_done = {k: self._colored_eval_key(k) for k in eval_done}
-        #eval_done = dict(TOTAL=f"{len(eval_done)} evaluations done.")
+        # eval_done = dict(TOTAL=f"{len(eval_done)} evaluations done.")
 
         eval_evaluating = [k for k in self.eval_status if self.eval_status[k] == "eval"]
         eval_evaluating = {k: self._colored_eval_key(k) for k in eval_evaluating}
         eval_calling = [k for k in self.eval_status if self.eval_status[k] == "calling"]
         eval_calling = {k: self._colored_eval_key(k) for k in eval_calling}
         return dict(
             Pending=waiting,
@@ -533,21 +544,21 @@
 
     def on_provide(self, event: ProvideEvent):
         self.total_status[event.key].status = "provided"
         self.request_status[event.key] = "provided"
         data_str = str(event.data)[:50]
         data_str = self.clean_msg(data_str)
         self.logger.info(f"{event.cxt.trace_str} := {data_str}")
-        #self.logger.info(f"{self.provider_status_string()}")
+        # self.logger.info(f"{self.provider_status_string()}")
 
     def on_deps_ready(self, event: DepsReadyEvent):
         self.total_status[event.key].status = "running"
         self.request_status[event.key] = "running"
         self.logger.info(f"{event.cxt.trace_str}")
-        #self.logger.info(f"{self.provider_status_string()}")
+        # self.logger.info(f"{self.provider_status_string()}")
 
     def clean_msg(self, msg):
         return msg.replace("<", "\<").replace(">", "\>")
 
     def on_eval_request(self, event):
         expr = show_expr(event.expr)
         expr = self.clean_msg(expr)
@@ -561,15 +572,15 @@
                 self.total_status[expr] = ResolveStatus(expr, "eval", "await", datetime.datetime.now(), None)
                 self.eval_status[expr] = "await"
                 # self.logger.debug(f"await\t -> <red>{expr}</red>")
             case _:
                 self.total_status[expr] = ResolveStatus(expr, "eval", "eval", datetime.datetime.now(), None)
                 self.eval_status[expr] = "eval"
                 # self.logger.debug(f"eval\t-> <magenta>{expr}</magenta>")
-        #self.logger.info(f"\n{self.eval_status_string()}")
+        # self.logger.info(f"\n{self.eval_status_string()}")
 
     def on_eval_result(self, event):
         expr = show_expr(event.expr)
         expr = self.clean_msg(expr)
         res_msg = self.clean_msg(str(event.result))
         match event.expr:
             case Cache(_):
@@ -580,15 +591,15 @@
             case UnaryOp('await', _):
                 self.logger.success(f"await <- <red>{expr}</red> := {res_msg}")
             case _:
                 self.logger.debug(f"eval<- <magenta>{expr}</magenta> := {res_msg}")
         self.total_status[expr].status = "done"
 
         self.eval_status[expr] = "done"
-        #self.logger.info(f"\n{self.eval_status_string()}")
+        # self.logger.info(f"\n{self.eval_status_string()}")
 
     def on_call_in_eval_start(self, event: CallInEvalStart):
         expr_str = self.clean_msg(show_expr(event.expr))
         self.logger.debug(f"call\t-> <magenta>{expr_str}</magenta>")
 
     def on_call_in_eval_end(self, event: CallInEvalEnd):
         expr_str = self.clean_msg(show_expr(event.expr))
```

### Comparing `pinjected-0.2.61/pinjected/visualize_di.py` & `pinjected-0.2.62/pinjected/visualize_di.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 import networkx as nx
 from cytoolz import memoize
 from loguru import logger
 from returns.pipeline import is_successful
 from returns.result import safe, Result, Failure
 
+from pinjected.di.app_injected import EvaledInjected
+from pinjected.di.ast import show_expr
 from pinjected.di.graph import providable_to_injected
 from pinjected.providable import Providable
 from pinjected.di.injected import Injected, InjectedFunction, InjectedPure, MappedInjected, \
     ZippedInjected, MZippedInjected, InjectedByName, extract_dependency, InjectedWithDefaultDesign, \
     PartialInjectedFunction
 from pinjected.di.proxiable import DelegatedVar
 from pinjected import Design
@@ -60,15 +62,15 @@
     src: Design
 
     def new_name(self, base: str):
         return f"{base}_{str(uuid.uuid4())[:6]}"
 
     def __post_init__(self):
         self.helper = DIGraphHelper(self.src)
-        self.explicit_mappings:dict[str,Injected] = self.helper.total_mappings()
+        self.explicit_mappings: dict[str, Injected] = self.helper.total_mappings()
 
         self.direct_injected = dict()
         self.injected_to_id = dict()
 
         @memoize
         def deps_impl(src: str):
             if "provide_" in src:
@@ -186,29 +188,29 @@
                         yield current, n, trace
                         yield from dfs(current, n, trace + [n])
 
         yield from dfs(src, src, [src])
 
     def di_dfs_validation(self, src):
         def dfs(node: str, trace=[]):
-            #logger.info(f"dfs:{node},{trace}")
+            # logger.info(f"dfs:{node},{trace}")
             nexts = []
             try:
                 nexts: List[str] = self.dependencies_of(node)
             except Exception as e:
                 yield DependencyResolutionFailure(node, trace, e)
             for n in nexts:
                 if n in trace:
-                    yield CyclicDependency(n,trace)
+                    yield CyclicDependency(n, trace)
                 else:
                     yield from dfs(n, trace + [n])
 
         yield from dfs(src, [src])
 
-    def distilled(self,tgt:Providable)->Design:
+    def distilled(self, tgt: Providable) -> Design:
         match tgt:
             case str():
                 deps = set([t[1] for t in self.di_dfs(tgt)])
                 nodes = set([t[0] for t in self.di_dfs(tgt)])
                 distilled = Design(
                     {k: self.src[k] for k in deps | nodes}
                 )
@@ -236,31 +238,34 @@
 
         except Exception as e:
             from loguru import logger
             logger.warning(f"{repr(e)[:100]} error from {repr(f)[:100]}")
             res = f"failed:{f} from {f}"
         return res
 
-
     @staticmethod
     def get_source_repr(f):
         res = DIGraph.get_source(f)
 
         res = res.replace("<", "").replace(">", "")
         res = res.replace("\t", "....").replace(" ", ".")
         # logger.info(f"extracted sources:\n{res}")
         return res
 
     def parse_injected(self, tgt: Injected):
         # from archpainter.my_artifacts.artifact_object import IArtifactObject
         match tgt:
             case InjectedWithDefaultDesign(src, default_design):
                 return self.parse_injected(src)
-            case InjectedFunction(f):
-                desc = f"Injected:{safe(getattr)(f, '__name__').value_or(repr(f))}"
+            case InjectedFunction(f) as _if:
+                try:
+                    desc = f"Injected:{safe(getattr)(_if.original_function, '__name__').value_or(repr(f))}"
+                except Exception as e:
+                    logger.error(f"failed to get func info from {f} due to {e}")
+                    raise e
                 return ("injected", desc, self.get_source_repr(f))
             case InjectedPure(v):
                 desc = f"Pure:{v}"
                 return ("injected", desc, self.get_source_repr(v) if isinstance(v, Callable) else str(v))
             case PartialInjectedFunction(InjectedFunction(src)):
                 desc = f"partial=>{src.__name__}"
                 return ("injected", desc, self.get_source_repr(src))
@@ -275,14 +280,18 @@
                 return ("injected", desc, "zipped")
             case MZippedInjected(srcs) as mzi:
                 desc = f"{mzi.__class__.__name__}"
                 return ("injected", desc, "mzipped")
             case InjectedByName(name):
                 desc = f"{name}"
                 return ("injected", desc, "by_name")
+            case EvaledInjected(val, ast):
+                expr = show_expr(ast)
+                desc = f"Eval({expr})"
+                return ("injected", desc, expr)
             case Injected() as injected:
                 desc = f"{injected.__class__.__name__}"
                 return ("injected", desc, str(injected))
             case unknown:
                 raise ValueError(f"unknown injected type {unknown}")
 
     def create_dependency_digraph_rooted(self, root: Injected, root_name="__root__",
@@ -310,15 +319,15 @@
     def get_node_to_sl(self, nx_graph, replace_missing):
         @memoize
         def node_to_sl(n):
             def parse(tgt):
                 match tgt:
                     case Injected():
                         return self.parse_injected(tgt)
-                    case BindInjected(tgt,_):
+                    case BindInjected(tgt, _):
                         return self.parse_injected(tgt)
                     case cls if isinstance(cls, type):
                         return ("class", cls.__name__, self.get_source_repr(cls))
                     case [*providers]:
                         return ("multi_binding", repr(providers), repr(providers))
                     case _:
                         return ("unknown", repr(tgt), repr(tgt))
@@ -491,15 +500,14 @@
         nx_graph.show_html_temp()
 
     def show_whole_html(self):
         roots = list(self.explicit_mappings.keys())
         self.create_dependency_digraph(roots, replace_missing=True, root_group=None).show_html_temp()
 
 
-
 def create_dependency_graph(d: Design, roots: List[str], output_file="dependencies.html"):
     dig = DIGraph(d.bind_instance(
         job_type="net_visualization"
     ))
     nt = dig.create_dependency_network(roots)
     nt.show(output_file)
     return nt
```

### Comparing `pinjected-0.2.61/pyproject.toml` & `pinjected-0.2.62/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.61"
+version = "0.2.62"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.61/PKG-INFO` & `pinjected-0.2.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.61
+Version: 0.2.62
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

