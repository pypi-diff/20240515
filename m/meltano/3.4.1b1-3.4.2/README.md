# Comparing `tmp/meltano-3.4.1b1.tar.gz` & `tmp/meltano-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltano-3.4.1b1.tar", max compression
+gzip compressed data, was "meltano-3.4.2.tar", max compression
```

## Comparing `meltano-3.4.1b1.tar` & `meltano-3.4.2.tar`

### file list

```diff
@@ -1,298 +1,298 @@
--rw-r--r--   0        0        0     1048 2024-05-06 16:59:49.770012 meltano-3.4.1b1/LICENSE
--rw-r--r--   0        0        0     5237 2024-05-06 16:59:49.770012 meltano-3.4.1b1/README.md
--rw-r--r--   0        0        0    20170 2024-05-06 16:59:49.906013 meltano-3.4.1b1/pyproject.toml
--rw-r--r--   0        0        0      100 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/__init__.py
--rw-r--r--   0        0        0       73 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/__main__.py
--rw-r--r--   0        0        0     6770 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/add.py
--rw-r--r--   0        0        0     6018 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/cli.py
--rw-r--r--   0        0        0     3806 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/compile.py
--rw-r--r--   0        0        0    14501 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/config.py
--rw-r--r--   0        0        0      406 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/docs.py
--rw-r--r--   0        0        0      507 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/dragon.py
--rw-r--r--   0        0        0    17244 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/elt.py
--rw-r--r--   0        0        0     2548 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/environment.py
--rw-r--r--   0        0        0     1671 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/hub.py
--rw-r--r--   0        0        0     2232 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/initialize.py
--rw-r--r--   0        0        0     4099 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/install.py
--rw-r--r--   0        0        0      181 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/interactive/__init__.py
--rw-r--r--   0        0        0    16395 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/interactive/config.py
--rw-r--r--   0        0        0      241 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/interactive/utils.py
--rw-r--r--   0        0        0     6287 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/invoke.py
--rw-r--r--   0        0        0    10060 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/job.py
--rw-r--r--   0        0        0     3804 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/lock.py
--rw-r--r--   0        0        0     2242 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/params.py
--rw-r--r--   0        0        0     2789 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/remove.py
--rw-r--r--   0        0        0     7804 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/run.py
--rw-r--r--   0        0        0    12993 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/schedule.py
--rw-r--r--   0        0        0      770 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/schema.py
--rw-r--r--   0        0        0     4446 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/select.py
--rw-r--r--   0        0        0    10590 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/state.py
--rw-r--r--   0        0        0     4344 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/upgrade.py
--rw-r--r--   0        0        0    24048 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/utils.py
--rw-r--r--   0        0        0     4185 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/cli/validate.py
--rw-r--r--   0        0        0        0 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/__init__.py
--rw-r--r--   0        0        0       64 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/__init__.py
--rw-r--r--   0        0        0    13060 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/canonical.py
--rw-r--r--   0        0        0     3975 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/hookable.py
--rw-r--r--   0        0        0      192 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/name_eq.py
--rw-r--r--   0        0        0     1187 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/versioned.py
--rw-r--r--   0        0        0      406 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/behavior/visitor.py
--rw-r--r--   0        0        0      117 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/block/__init__.py
--rw-r--r--   0        0        0     1582 2024-05-06 16:59:49.906013 meltano-3.4.1b1/src/meltano/core/block/blockset.py
--rw-r--r--   0        0        0    30262 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/extract_load.py
--rw-r--r--   0        0        0     2753 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/future_utils.py
--rw-r--r--   0        0        0     3946 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/ioblock.py
--rw-r--r--   0        0        0    11405 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/parser.py
--rw-r--r--   0        0        0     5745 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/plugin_command.py
--rw-r--r--   0        0        0    12260 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/block/singer.py
--rw-r--r--   0        0        0      128 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/bundle/__init__.py
--rw-r--r--   0        0        0      460 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/bundle/initialize.yml
--rw-r--r--   0        0        0     2773 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/bundle/settings.yml
--rw-r--r--   0        0        0    10326 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/cli_messages.py
--rw-r--r--   0        0        0     3106 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/config_service.py
--rw-r--r--   0        0        0       81 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/container/__init__.py
--rw-r--r--   0        0        0     2130 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/container/container_service.py
--rw-r--r--   0        0        0     2997 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/container/container_spec.py
--rw-r--r--   0        0        0     7435 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/db.py
--rw-r--r--   0        0        0    14979 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/elt_context.py
--rw-r--r--   0        0        0     6924 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/environment.py
--rw-r--r--   0        0        0     2797 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/environment_service.py
--rw-r--r--   0        0        0     3747 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/error.py
--rw-r--r--   0        0        0      181 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/hub/__init__.py
--rw-r--r--   0        0        0    11085 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/hub/client.py
--rw-r--r--   0        0        0      896 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/hub/schema.py
--rw-r--r--   0        0        0      103 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/__init__.py
--rw-r--r--   0        0        0     5940 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/finder.py
--rw-r--r--   0        0        0    11544 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/job.py
--rw-r--r--   0        0        0     1049 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job/stale_job_failer.py
--rw-r--r--   0        0        0     6015 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/job_state.py
--rw-r--r--   0        0        0     2974 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/locked_definition_service.py
--rw-r--r--   0        0        0      699 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/__init__.py
--rw-r--r--   0        0        0     4530 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/formatters.py
--rw-r--r--   0        0        0     5622 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/job_logging_service.py
--rw-r--r--   0        0        0     7383 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/output_logger.py
--rw-r--r--   0        0        0     7100 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/logging/utils.py
--rw-r--r--   0        0        0     3453 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/__init__.py
--rw-r--r--   0        0        0      365 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/cache.py
--rw-r--r--   0        0        0     4835 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/contexts.py
--rw-r--r--   0        0        0     4867 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/jsonschema.py
--rw-r--r--   0        0        0    18190 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/manifest/manifest.py
--rw-r--r--   0        0        0     5137 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/meltano_file.py
--rw-r--r--   0        0        0     2679 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/meltano_invoker.py
--rw-r--r--   0        0        0     3744 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/migration_service.py
--rw-r--r--   0        0        0      481 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/models.py
--rw-r--r--   0        0        0      188 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/__init__.py
--rw-r--r--   0        0        0     5751 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/airflow.py
--rw-r--r--   0        0        0    27362 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/base.py
--rw-r--r--   0        0        0     3638 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/command.py
--rw-r--r--   0        0        0     1472 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/config_service.py
--rw-r--r--   0        0        0      139 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/dbt/__init__.py
--rw-r--r--   0        0        0     4085 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/dbt/base.py
--rw-r--r--   0        0        0     2703 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/error.py
--rw-r--r--   0        0        0     1849 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/factory.py
--rw-r--r--   0        0        0     9890 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/file.py
--rw-r--r--   0        0        0     2708 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/meltano_file.py
--rw-r--r--   0        0        0    14849 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/project_plugin.py
--rw-r--r--   0        0        0     1135 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/requirements.py
--rw-r--r--   0        0        0     7651 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/settings_service.py
--rw-r--r--   0        0        0      282 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/__init__.py
--rw-r--r--   0        0        0     2601 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/base.py
--rw-r--r--   0        0        0    19824 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/catalog.py
--rw-r--r--   0        0        0     2512 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/mapper.py
--rw-r--r--   0        0        0    23895 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/tap.py
--rw-r--r--   0        0        0     5592 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/singer/target.py
--rw-r--r--   0        0        0     5831 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/superset.py
--rw-r--r--   0        0        0      269 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin/utility.py
--rw-r--r--   0        0        0    17363 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin_install_service.py
--rw-r--r--   0        0        0    17290 2024-05-06 16:59:49.910013 meltano-3.4.1b1/src/meltano/core/plugin_invoker.py
--rw-r--r--   0        0        0     6473 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_location_remove.py
--rw-r--r--   0        0        0     3931 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_lock_service.py
--rw-r--r--   0        0        0     2817 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_remove_service.py
--rw-r--r--   0        0        0     2180 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_repository.py
--rw-r--r--   0        0        0     3264 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/plugin_test_service.py
--rw-r--r--   0        0        0    20318 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project.py
--rw-r--r--   0        0        0     3999 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_add_service.py
--rw-r--r--   0        0        0    14192 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_files.py
--rw-r--r--   0        0        0     6581 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_init_service.py
--rw-r--r--   0        0        0    18330 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_plugins_service.py
--rw-r--r--   0        0        0     5118 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/project_settings_service.py
--rw-r--r--   0        0        0      262 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/runner/__init__.py
--rw-r--r--   0        0        0     2149 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/runner/dbt.py
--rw-r--r--   0        0        0    10225 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/runner/singer.py
--rw-r--r--   0        0        0     3769 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/schedule.py
--rw-r--r--   0        0        0    10967 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/schedule_service.py
--rw-r--r--   0        0        0     3384 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/select_service.py
--rw-r--r--   0        0        0      926 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/setting.py
--rw-r--r--   0        0        0    15809 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/setting_definition.py
--rw-r--r--   0        0        0    21258 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/settings_service.py
--rw-r--r--   0        0        0    46409 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/settings_store.py
--rw-r--r--   0        0        0     2573 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/sqlalchemy.py
--rw-r--r--   0        0        0     7282 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_service.py
--rw-r--r--   0        0        0     3728 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/__init__.py
--rw-r--r--   0        0        0     5482 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/azure.py
--rw-r--r--   0        0        0     2116 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/base.py
--rw-r--r--   0        0        0     3831 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/db.py
--rw-r--r--   0        0        0    17960 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/filesystem.py
--rw-r--r--   0        0        0     4170 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/google.py
--rw-r--r--   0        0        0     4860 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/state_store/s3.py
--rw-r--r--   0        0        0     4461 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/task_sets.py
--rw-r--r--   0        0        0     3993 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/task_sets_service.py
--rw-r--r--   0        0        0        0 2024-05-06 17:00:07.430114 meltano-3.4.1b1/src/meltano/core/tracking/.release_marker
--rw-r--r--   0        0        0     3614 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/README.md
--rw-r--r--   0        0        0      125 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/__init__.py
--rw-r--r--   0        0        0      470 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/__init__.py
--rw-r--r--   0        0        0     2515 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/cli.py
--rw-r--r--   0        0        0     6044 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/environment.py
--rw-r--r--   0        0        0     3790 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/exception.py
--rw-r--r--   0        0        0     4942 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/plugins.py
--rw-r--r--   0        0        0     4128 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/contexts/project.py
--rw-r--r--   0        0        0      918 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1051 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1194 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
--rw-r--r--   0        0        0      720 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      748 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     6002 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     6501 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     6963 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
--rw-r--r--   0        0        0     7408 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
--rw-r--r--   0        0        0     4449 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1403 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1462 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     3920 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2109 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2812 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     1202 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      404 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/iglu.json
--rw-r--r--   0        0        0     9688 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/micro.conf
--rw-r--r--   0        0        0     1112 2024-05-06 16:59:49.914013 meltano-3.4.1b1/src/meltano/core/tracking/schemas.py
--rw-r--r--   0        0        0    18604 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/tracking/tracker.py
--rw-r--r--   0        0        0     3562 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/transform_add_service.py
--rw-r--r--   0        0        0     7708 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/upgrade_service.py
--rw-r--r--   0        0        0    25167 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/utils/__init__.py
--rw-r--r--   0        0        0     1463 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/utils/pidfile.py
--rw-r--r--   0        0        0     4095 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/validation_service.py
--rw-r--r--   0        0        0    23746 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/venv_service.py
--rw-r--r--   0        0        0     1521 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/core/yaml.py
--rw-r--r--   0        0        0      508 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/__init__.py
--rw-r--r--   0        0        0       12 2024-05-06 17:00:07.346114 meltano-3.4.1b1/src/meltano/migrations/db.lock
--rw-r--r--   0        0        0     1490 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/env.py
--rw-r--r--   0        0        0      495 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/script.py.mako
--rw-r--r--   0        0        0       67 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/utils/__init__.py
--rw-r--r--   0        0        0     1261 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/utils/dialect_typing.py
--rw-r--r--   0        0        0     1814 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
--rw-r--r--   0        0        0      972 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
--rw-r--r--   0        0        0      674 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
--rw-r--r--   0        0        0      802 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
--rw-r--r--   0        0        0      563 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
--rw-r--r--   0        0        0    11827 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
--rw-r--r--   0        0        0     2877 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py
--rw-r--r--   0        0        0     1095 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
--rw-r--r--   0        0        0      643 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
--rw-r--r--   0        0        0      786 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
--rw-r--r--   0        0        0     2026 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/b4c05e463b53_.py
--rw-r--r--   0        0        0      972 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
--rw-r--r--   0        0        0      699 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
--rw-r--r--   0        0        0      679 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
--rw-r--r--   0        0        0      486 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
--rw-r--r--   0        0        0    37573 2024-05-06 16:59:49.918013 meltano-3.4.1b1/src/meltano/schemas/meltano.schema.json
--rw-r--r--   0        0        0      438 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/asserts.py
--rw-r--r--   0        0        0     7479 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/conftest.py
--rw-r--r--   0        0        0     2190 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/cli.py
--rw-r--r--   0        0        0   125892 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/core.py
--rw-r--r--   0        0        0     2845 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/__init__.py
--rw-r--r--   0        0        0     2518 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/mssql.py
--rw-r--r--   0        0        0     1227 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/postgresql.py
--rw-r--r--   0        0        0     1222 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/postgresql_psycopg3.py
--rw-r--r--   0        0        0      328 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/db/sqlite.py
--rw-r--r--   0        0        0      752 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/docker/__init__.py
--rw-r--r--   0        0        0      276 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/docker/docker-compose.yml
--rw-r--r--   0        0        0     4132 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/docker/snowplow.py
--rw-r--r--   0        0        0     1535 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/fs.py
--rw-r--r--   0        0        0     3135 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/large_config_project/meltano.yml
--rw-r--r--   0        0        0    30013 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/large_config_project/schedule.yml
--rw-r--r--   0        0        0     1086 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/multifile_project/meltano.yml
--rw-r--r--   0        0        0      469 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/multifile_project/subconfig_2.yml
--rw-r--r--   0        0        0      394 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
--rw-r--r--   0        0        0      631 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/plugins/extractors/tap-custom/test.yml
--rw-r--r--   0        0        0     1152 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/fixtures/utils.py
--rw-r--r--   0        0        0    31067 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_add.py
--rw-r--r--   0        0        0    15154 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_cli.py
--rw-r--r--   0        0        0     5174 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_compile.py
--rw-r--r--   0        0        0     8634 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_config.py
--rw-r--r--   0        0        0    42021 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_elt.py
--rw-r--r--   0        0        0     1585 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_hub.py
--rw-r--r--   0        0        0     3577 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_initialize.py
--rw-r--r--   0        0        0    12665 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_install.py
--rw-r--r--   0        0        0     9285 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_invoke.py
--rw-r--r--   0        0        0     6777 2024-05-06 16:59:49.918013 meltano-3.4.1b1/tests/meltano/cli/test_job_cmd.py
--rw-r--r--   0        0        0     3771 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_lock.py
--rw-r--r--   0        0        0     1864 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_remove.py
--rw-r--r--   0        0        0    48146 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_run.py
--rw-r--r--   0        0        0     8502 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_schedule.py
--rw-r--r--   0        0        0     1140 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_select.py
--rw-r--r--   0        0        0    11532 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_state.py
--rw-r--r--   0        0        0     8268 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/cli/test_upgrade.py
--rw-r--r--   0        0        0     5381 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/behavior/test_canonical.py
--rw-r--r--   0        0        0     2155 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/behavior/test_hookable.py
--rw-r--r--   0        0        0    22553 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_extract_load.py
--rw-r--r--   0        0        0      241 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_parser.py
--rw-r--r--   0        0        0      933 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_plugin_command.py
--rw-r--r--   0        0        0     7736 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/block/test_singer.py
--rw-r--r--   0        0        0     2302 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/container/test_container_spec.py
--rw-r--r--   0        0        0     6783 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/hub/test_meltano_hub_service.py
--rw-r--r--   0        0        0     2076 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/job/test_finder.py
--rw-r--r--   0        0        0     6240 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/job/test_job.py
--rw-r--r--   0        0        0     2579 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/job/test_stale_job_failer.py
--rw-r--r--   0        0        0     3357 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/logging/test_formatters.py
--rw-r--r--   0        0        0      806 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/logging/test_logging_utils.py
--rw-r--r--   0        0        0     7590 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/logging/test_output_logger.py
--rw-r--r--   0        0        0    32646 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_catalog.py
--rw-r--r--   0        0        0     3185 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_mapper.py
--rw-r--r--   0        0        0    37606 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_tap.py
--rw-r--r--   0        0        0     3690 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_target.py
--rw-r--r--   0        0        0     3921 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_airflow.py
--rw-r--r--   0        0        0     2396 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_command.py
--rw-r--r--   0        0        0    22146 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin.py
--rw-r--r--   0        0        0      174 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin_config_service.py
--rw-r--r--   0        0        0    35208 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin_settings.py
--rw-r--r--   0        0        0     5963 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/plugin/test_superset.py
--rw-r--r--   0        0        0     7999 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/runner/test_runner.py
--rw-r--r--   0        0        0     2807 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/state_store/test_db.py
--rw-r--r--   0        0        0    21574 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/state_store/test_filesystem.py
--rw-r--r--   0        0        0     6765 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/state_store/test_state_store.py
--rw-r--r--   0        0        0     1558 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_db_compat.py
--rw-r--r--   0        0        0     1813 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_db_connection.py
--rw-r--r--   0        0        0     5217 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_elt_context.py
--rw-r--r--   0        0        0     2610 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_environment_service.py
--rw-r--r--   0        0        0    13772 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_environment_variables.py
--rw-r--r--   0        0        0     2274 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_locked_definition_service.py
--rw-r--r--   0        0        0     2108 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_meltano_file.py
--rw-r--r--   0        0        0     3128 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_meltano_invoker.py
--rw-r--r--   0        0        0     4094 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_install_service.py
--rw-r--r--   0        0        0     6101 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_invoker.py
--rw-r--r--   0        0        0     3127 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_lock_service.py
--rw-r--r--   0        0        0     5749 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_remove_service.py
--rw-r--r--   0        0        0     5815 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_plugin_test_service.py
--rw-r--r--   0        0        0     4319 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project.py
--rw-r--r--   0        0        0     8892 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_add_service.py
--rw-r--r--   0        0        0    16326 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_files.py
--rw-r--r--   0        0        0     3281 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_init_service.py
--rw-r--r--   0        0        0     8071 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_plugins_service.py
--rw-r--r--   0        0        0     7238 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_project_settings_service.py
--rw-r--r--   0        0        0     9759 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_schedule_service.py
--rw-r--r--   0        0        0     5865 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_setting_definition.py
--rw-r--r--   0        0        0    22226 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_settings_store.py
--rw-r--r--   0        0        0     3665 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_state_service.py
--rw-r--r--   0        0        0     2430 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_task_sets.py
--rw-r--r--   0        0        0     2645 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_task_sets_service.py
--rw-r--r--   0        0        0     7126 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_utils.py
--rw-r--r--   0        0        0     1813 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_validation_service.py
--rw-r--r--   0        0        0    12257 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/test_venv_service.py
--rw-r--r--   0        0        0     1980 2024-05-06 16:59:49.922013 meltano-3.4.1b1/tests/meltano/core/tracking/test_environment_context.py
--rw-r--r--   0        0        0     5708 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_exception.py
--rw-r--r--   0        0        0     3061 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_plugins.py
--rw-r--r--   0        0        0     1271 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_project_context.py
--rw-r--r--   0        0        0      684 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_schemas.py
--rw-r--r--   0        0        0    19720 2024-05-06 16:59:49.926013 meltano-3.4.1b1/tests/meltano/core/tracking/test_tracker.py
--rw-r--r--   0        0        0     9032 1970-01-01 00:00:00.000000 meltano-3.4.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1048 2024-05-15 21:30:22.632114 meltano-3.4.2/LICENSE
+-rw-r--r--   0        0        0     5237 2024-05-15 21:30:22.632114 meltano-3.4.2/README.md
+-rw-r--r--   0        0        0    20168 2024-05-15 21:30:22.764114 meltano-3.4.2/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/__main__.py
+-rw-r--r--   0        0        0     6770 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/add.py
+-rw-r--r--   0        0        0     6018 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/cli.py
+-rw-r--r--   0        0        0     3806 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/compile.py
+-rw-r--r--   0        0        0    14501 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/config.py
+-rw-r--r--   0        0        0      406 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/docs.py
+-rw-r--r--   0        0        0      507 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/dragon.py
+-rw-r--r--   0        0        0    17244 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/elt.py
+-rw-r--r--   0        0        0     2548 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/environment.py
+-rw-r--r--   0        0        0     1671 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/hub.py
+-rw-r--r--   0        0        0     2232 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/initialize.py
+-rw-r--r--   0        0        0     4099 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/install.py
+-rw-r--r--   0        0        0      181 2024-05-15 21:30:22.764114 meltano-3.4.2/src/meltano/cli/interactive/__init__.py
+-rw-r--r--   0        0        0    16395 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/interactive/config.py
+-rw-r--r--   0        0        0      241 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/interactive/utils.py
+-rw-r--r--   0        0        0     6287 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/invoke.py
+-rw-r--r--   0        0        0    10060 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/job.py
+-rw-r--r--   0        0        0     3804 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/lock.py
+-rw-r--r--   0        0        0     2242 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/params.py
+-rw-r--r--   0        0        0     2789 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/remove.py
+-rw-r--r--   0        0        0     7804 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/run.py
+-rw-r--r--   0        0        0    12993 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/schedule.py
+-rw-r--r--   0        0        0      770 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/schema.py
+-rw-r--r--   0        0        0     4446 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/select.py
+-rw-r--r--   0        0        0    10590 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/state.py
+-rw-r--r--   0        0        0     4344 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/upgrade.py
+-rw-r--r--   0        0        0    24048 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/utils.py
+-rw-r--r--   0        0        0     4185 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/cli/validate.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/__init__.py
+-rw-r--r--   0        0        0       64 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/behavior/__init__.py
+-rw-r--r--   0        0        0    13060 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/behavior/canonical.py
+-rw-r--r--   0        0        0     3975 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/behavior/hookable.py
+-rw-r--r--   0        0        0      192 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/behavior/name_eq.py
+-rw-r--r--   0        0        0     1187 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/behavior/versioned.py
+-rw-r--r--   0        0        0      406 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/behavior/visitor.py
+-rw-r--r--   0        0        0      117 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/blockset.py
+-rw-r--r--   0        0        0    30262 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/extract_load.py
+-rw-r--r--   0        0        0     2753 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/future_utils.py
+-rw-r--r--   0        0        0     3946 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/ioblock.py
+-rw-r--r--   0        0        0    11405 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/parser.py
+-rw-r--r--   0        0        0     5745 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/plugin_command.py
+-rw-r--r--   0        0        0    12260 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/block/singer.py
+-rw-r--r--   0        0        0      128 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/bundle/__init__.py
+-rw-r--r--   0        0        0      460 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/bundle/initialize.yml
+-rw-r--r--   0        0        0     2773 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/bundle/settings.yml
+-rw-r--r--   0        0        0    10326 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/cli_messages.py
+-rw-r--r--   0        0        0     3106 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/config_service.py
+-rw-r--r--   0        0        0       81 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/container/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/container/container_service.py
+-rw-r--r--   0        0        0     2997 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/container/container_spec.py
+-rw-r--r--   0        0        0     7435 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/db.py
+-rw-r--r--   0        0        0    14979 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/elt_context.py
+-rw-r--r--   0        0        0     6924 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/environment.py
+-rw-r--r--   0        0        0     2797 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/environment_service.py
+-rw-r--r--   0        0        0     3747 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/error.py
+-rw-r--r--   0        0        0      181 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/hub/__init__.py
+-rw-r--r--   0        0        0    11085 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/hub/client.py
+-rw-r--r--   0        0        0      896 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/hub/schema.py
+-rw-r--r--   0        0        0      103 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/job/__init__.py
+-rw-r--r--   0        0        0     5940 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/job/finder.py
+-rw-r--r--   0        0        0    11544 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/job/job.py
+-rw-r--r--   0        0        0     1049 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/job/stale_job_failer.py
+-rw-r--r--   0        0        0     6015 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/job_state.py
+-rw-r--r--   0        0        0     2974 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/locked_definition_service.py
+-rw-r--r--   0        0        0      699 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/logging/__init__.py
+-rw-r--r--   0        0        0     4530 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/logging/formatters.py
+-rw-r--r--   0        0        0     5622 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/logging/job_logging_service.py
+-rw-r--r--   0        0        0     7383 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/logging/output_logger.py
+-rw-r--r--   0        0        0     7100 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/logging/utils.py
+-rw-r--r--   0        0        0     3453 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/manifest/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/manifest/cache.py
+-rw-r--r--   0        0        0     4835 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/manifest/contexts.py
+-rw-r--r--   0        0        0     4867 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/manifest/jsonschema.py
+-rw-r--r--   0        0        0    18190 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/manifest/manifest.py
+-rw-r--r--   0        0        0     5137 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/meltano_file.py
+-rw-r--r--   0        0        0     2679 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/meltano_invoker.py
+-rw-r--r--   0        0        0     3744 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/migration_service.py
+-rw-r--r--   0        0        0      481 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/models.py
+-rw-r--r--   0        0        0      188 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/plugin/__init__.py
+-rw-r--r--   0        0        0     5751 2024-05-15 21:30:22.768114 meltano-3.4.2/src/meltano/core/plugin/airflow.py
+-rw-r--r--   0        0        0    27362 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/base.py
+-rw-r--r--   0        0        0     3638 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/command.py
+-rw-r--r--   0        0        0     1472 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/config_service.py
+-rw-r--r--   0        0        0      139 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/dbt/__init__.py
+-rw-r--r--   0        0        0     4085 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/dbt/base.py
+-rw-r--r--   0        0        0     2703 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/error.py
+-rw-r--r--   0        0        0     1849 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/factory.py
+-rw-r--r--   0        0        0     9890 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/file.py
+-rw-r--r--   0        0        0     2708 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/meltano_file.py
+-rw-r--r--   0        0        0    14849 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/project_plugin.py
+-rw-r--r--   0        0        0     1135 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/requirements.py
+-rw-r--r--   0        0        0     7651 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/settings_service.py
+-rw-r--r--   0        0        0      282 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/singer/__init__.py
+-rw-r--r--   0        0        0     2601 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/singer/base.py
+-rw-r--r--   0        0        0    19824 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/singer/catalog.py
+-rw-r--r--   0        0        0     2512 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/singer/mapper.py
+-rw-r--r--   0        0        0    23895 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/singer/tap.py
+-rw-r--r--   0        0        0     5679 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/singer/target.py
+-rw-r--r--   0        0        0     5831 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/superset.py
+-rw-r--r--   0        0        0      269 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin/utility.py
+-rw-r--r--   0        0        0    17363 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin_install_service.py
+-rw-r--r--   0        0        0    17290 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin_invoker.py
+-rw-r--r--   0        0        0     6473 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin_location_remove.py
+-rw-r--r--   0        0        0     3931 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin_lock_service.py
+-rw-r--r--   0        0        0     2817 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin_remove_service.py
+-rw-r--r--   0        0        0     2180 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin_repository.py
+-rw-r--r--   0        0        0     3264 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/plugin_test_service.py
+-rw-r--r--   0        0        0    20318 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/project.py
+-rw-r--r--   0        0        0     3999 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/project_add_service.py
+-rw-r--r--   0        0        0    14192 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/project_files.py
+-rw-r--r--   0        0        0     6581 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/project_init_service.py
+-rw-r--r--   0        0        0    18330 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/project_plugins_service.py
+-rw-r--r--   0        0        0     5118 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/project_settings_service.py
+-rw-r--r--   0        0        0      262 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/runner/__init__.py
+-rw-r--r--   0        0        0     2149 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/runner/dbt.py
+-rw-r--r--   0        0        0    10225 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/runner/singer.py
+-rw-r--r--   0        0        0     3769 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/schedule.py
+-rw-r--r--   0        0        0    10967 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/schedule_service.py
+-rw-r--r--   0        0        0     3384 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/select_service.py
+-rw-r--r--   0        0        0      926 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/setting.py
+-rw-r--r--   0        0        0    15809 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/setting_definition.py
+-rw-r--r--   0        0        0    21258 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/settings_service.py
+-rw-r--r--   0        0        0    46409 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/settings_store.py
+-rw-r--r--   0        0        0     2573 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/sqlalchemy.py
+-rw-r--r--   0        0        0     7282 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_service.py
+-rw-r--r--   0        0        0     3728 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_store/__init__.py
+-rw-r--r--   0        0        0     5482 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_store/azure.py
+-rw-r--r--   0        0        0     2116 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_store/base.py
+-rw-r--r--   0        0        0     3831 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_store/db.py
+-rw-r--r--   0        0        0    17998 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_store/filesystem.py
+-rw-r--r--   0        0        0     4170 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_store/google.py
+-rw-r--r--   0        0        0     4860 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/state_store/s3.py
+-rw-r--r--   0        0        0     4461 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/task_sets.py
+-rw-r--r--   0        0        0     3993 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/task_sets_service.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:30:43.452045 meltano-3.4.2/src/meltano/core/tracking/.release_marker
+-rw-r--r--   0        0        0     3614 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/README.md
+-rw-r--r--   0        0        0      125 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/__init__.py
+-rw-r--r--   0        0        0      470 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/contexts/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/contexts/cli.py
+-rw-r--r--   0        0        0     6044 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/contexts/environment.py
+-rw-r--r--   0        0        0     3790 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/contexts/exception.py
+-rw-r--r--   0        0        0     4942 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/contexts/plugins.py
+-rw-r--r--   0        0        0     4128 2024-05-15 21:30:22.772114 meltano-3.4.2/src/meltano/core/tracking/contexts/project.py
+-rw-r--r--   0        0        0      918 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1051 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1194 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0      720 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      748 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     6002 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     6501 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     6963 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
+-rw-r--r--   0        0        0     7408 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
+-rw-r--r--   0        0        0     4449 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1403 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1462 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     3920 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2109 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2812 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     1202 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      404 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/iglu.json
+-rw-r--r--   0        0        0     9688 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/micro.conf
+-rw-r--r--   0        0        0     1112 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/schemas.py
+-rw-r--r--   0        0        0    18604 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/tracking/tracker.py
+-rw-r--r--   0        0        0     3562 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/transform_add_service.py
+-rw-r--r--   0        0        0     7708 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/upgrade_service.py
+-rw-r--r--   0        0        0    25167 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/utils/__init__.py
+-rw-r--r--   0        0        0     1463 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/utils/pidfile.py
+-rw-r--r--   0        0        0     4095 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/validation_service.py
+-rw-r--r--   0        0        0    23746 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/venv_service.py
+-rw-r--r--   0        0        0     1521 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/core/yaml.py
+-rw-r--r--   0        0        0      508 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2024-05-15 21:30:43.364045 meltano-3.4.2/src/meltano/migrations/db.lock
+-rw-r--r--   0        0        0     1490 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/env.py
+-rw-r--r--   0        0        0      495 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/script.py.mako
+-rw-r--r--   0        0        0       67 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/utils/__init__.py
+-rw-r--r--   0        0        0     1261 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/utils/dialect_typing.py
+-rw-r--r--   0        0        0     1814 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
+-rw-r--r--   0        0        0      972 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
+-rw-r--r--   0        0        0      674 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
+-rw-r--r--   0        0        0      802 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
+-rw-r--r--   0        0        0      563 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
+-rw-r--r--   0        0        0    11827 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
+-rw-r--r--   0        0        0     2877 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/6ef30ab7b8e5_.py
+-rw-r--r--   0        0        0     1095 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
+-rw-r--r--   0        0        0      643 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
+-rw-r--r--   0        0        0      786 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
+-rw-r--r--   0        0        0     2026 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/b4c05e463b53_.py
+-rw-r--r--   0        0        0      972 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
+-rw-r--r--   0        0        0      699 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
+-rw-r--r--   0        0        0      679 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
+-rw-r--r--   0        0        0      486 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
+-rw-r--r--   0        0        0    37573 2024-05-15 21:30:22.776114 meltano-3.4.2/src/meltano/schemas/meltano.schema.json
+-rw-r--r--   0        0        0      438 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/asserts.py
+-rw-r--r--   0        0        0     7479 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     2190 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/cli.py
+-rw-r--r--   0        0        0   125892 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/core.py
+-rw-r--r--   0        0        0     2845 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/db/__init__.py
+-rw-r--r--   0        0        0     2518 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/db/mssql.py
+-rw-r--r--   0        0        0     1227 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/db/postgresql.py
+-rw-r--r--   0        0        0     1222 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/db/postgresql_psycopg3.py
+-rw-r--r--   0        0        0      328 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/db/sqlite.py
+-rw-r--r--   0        0        0      752 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/docker/__init__.py
+-rw-r--r--   0        0        0      276 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/docker/docker-compose.yml
+-rw-r--r--   0        0        0     4132 2024-05-15 21:30:22.776114 meltano-3.4.2/tests/fixtures/docker/snowplow.py
+-rw-r--r--   0        0        0     1535 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/fs.py
+-rw-r--r--   0        0        0     3135 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/large_config_project/meltano.yml
+-rw-r--r--   0        0        0    30013 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/large_config_project/schedule.yml
+-rw-r--r--   0        0        0     1086 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/multifile_project/meltano.yml
+-rw-r--r--   0        0        0      469 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/multifile_project/subconfig_2.yml
+-rw-r--r--   0        0        0      394 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
+-rw-r--r--   0        0        0      631 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/plugins/extractors/tap-custom/test.yml
+-rw-r--r--   0        0        0     1152 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/fixtures/utils.py
+-rw-r--r--   0        0        0    31067 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_add.py
+-rw-r--r--   0        0        0    15154 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_cli.py
+-rw-r--r--   0        0        0     5174 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_compile.py
+-rw-r--r--   0        0        0     8634 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_config.py
+-rw-r--r--   0        0        0    42021 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_elt.py
+-rw-r--r--   0        0        0     1585 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_hub.py
+-rw-r--r--   0        0        0     3577 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_initialize.py
+-rw-r--r--   0        0        0    12665 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_install.py
+-rw-r--r--   0        0        0     9285 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_invoke.py
+-rw-r--r--   0        0        0     6777 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_job_cmd.py
+-rw-r--r--   0        0        0     3771 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_lock.py
+-rw-r--r--   0        0        0     1864 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_remove.py
+-rw-r--r--   0        0        0    48146 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_run.py
+-rw-r--r--   0        0        0     8502 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_schedule.py
+-rw-r--r--   0        0        0     1140 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_select.py
+-rw-r--r--   0        0        0    11532 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_state.py
+-rw-r--r--   0        0        0     8268 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/cli/test_upgrade.py
+-rw-r--r--   0        0        0     5381 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/behavior/test_canonical.py
+-rw-r--r--   0        0        0     2155 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/behavior/test_hookable.py
+-rw-r--r--   0        0        0    22553 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/block/test_extract_load.py
+-rw-r--r--   0        0        0      241 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/block/test_parser.py
+-rw-r--r--   0        0        0      933 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/block/test_plugin_command.py
+-rw-r--r--   0        0        0     7736 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/block/test_singer.py
+-rw-r--r--   0        0        0     2302 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/container/test_container_spec.py
+-rw-r--r--   0        0        0     6783 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/hub/test_meltano_hub_service.py
+-rw-r--r--   0        0        0     2076 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/job/test_finder.py
+-rw-r--r--   0        0        0     6240 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/job/test_job.py
+-rw-r--r--   0        0        0     2579 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/job/test_stale_job_failer.py
+-rw-r--r--   0        0        0     3357 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/logging/test_formatters.py
+-rw-r--r--   0        0        0      806 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/logging/test_logging_utils.py
+-rw-r--r--   0        0        0     7590 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/logging/test_output_logger.py
+-rw-r--r--   0        0        0    32646 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/singer/test_catalog.py
+-rw-r--r--   0        0        0     3185 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/singer/test_mapper.py
+-rw-r--r--   0        0        0    37606 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/singer/test_tap.py
+-rw-r--r--   0        0        0     3690 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/singer/test_target.py
+-rw-r--r--   0        0        0     3921 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/test_airflow.py
+-rw-r--r--   0        0        0     2396 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/test_command.py
+-rw-r--r--   0        0        0    22146 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/test_plugin.py
+-rw-r--r--   0        0        0      174 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/test_plugin_config_service.py
+-rw-r--r--   0        0        0    35208 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/test_plugin_settings.py
+-rw-r--r--   0        0        0     5963 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/plugin/test_superset.py
+-rw-r--r--   0        0        0     7999 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/runner/test_runner.py
+-rw-r--r--   0        0        0     2807 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/state_store/test_db.py
+-rw-r--r--   0        0        0    22779 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/state_store/test_filesystem.py
+-rw-r--r--   0        0        0     6765 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/state_store/test_state_store.py
+-rw-r--r--   0        0        0     1558 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/test_db_compat.py
+-rw-r--r--   0        0        0     1813 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/test_db_connection.py
+-rw-r--r--   0        0        0     5217 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/test_elt_context.py
+-rw-r--r--   0        0        0     2610 2024-05-15 21:30:22.780114 meltano-3.4.2/tests/meltano/core/test_environment_service.py
+-rw-r--r--   0        0        0    13772 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_environment_variables.py
+-rw-r--r--   0        0        0     2274 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_locked_definition_service.py
+-rw-r--r--   0        0        0     2108 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_meltano_file.py
+-rw-r--r--   0        0        0     3128 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_meltano_invoker.py
+-rw-r--r--   0        0        0     4094 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_plugin_install_service.py
+-rw-r--r--   0        0        0     6101 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_plugin_invoker.py
+-rw-r--r--   0        0        0     3127 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_plugin_lock_service.py
+-rw-r--r--   0        0        0     5749 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_plugin_remove_service.py
+-rw-r--r--   0        0        0     5815 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_plugin_test_service.py
+-rw-r--r--   0        0        0     4319 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_project.py
+-rw-r--r--   0        0        0     8892 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_project_add_service.py
+-rw-r--r--   0        0        0    16326 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_project_files.py
+-rw-r--r--   0        0        0     3281 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_project_init_service.py
+-rw-r--r--   0        0        0     8071 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_project_plugins_service.py
+-rw-r--r--   0        0        0     7238 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_project_settings_service.py
+-rw-r--r--   0        0        0     9759 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_schedule_service.py
+-rw-r--r--   0        0        0     5865 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_setting_definition.py
+-rw-r--r--   0        0        0    22226 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_settings_store.py
+-rw-r--r--   0        0        0     3665 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_state_service.py
+-rw-r--r--   0        0        0     2430 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_task_sets.py
+-rw-r--r--   0        0        0     2645 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_task_sets_service.py
+-rw-r--r--   0        0        0     7126 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_utils.py
+-rw-r--r--   0        0        0     1813 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_validation_service.py
+-rw-r--r--   0        0        0    12257 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/test_venv_service.py
+-rw-r--r--   0        0        0     1980 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/tracking/test_environment_context.py
+-rw-r--r--   0        0        0     5708 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/tracking/test_exception.py
+-rw-r--r--   0        0        0     3061 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/tracking/test_plugins.py
+-rw-r--r--   0        0        0     1271 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/tracking/test_project_context.py
+-rw-r--r--   0        0        0      684 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/tracking/test_schemas.py
+-rw-r--r--   0        0        0    19720 2024-05-15 21:30:22.784114 meltano-3.4.2/tests/meltano/core/tracking/test_tracker.py
+-rw-r--r--   0        0        0     9031 1970-01-01 00:00:00.000000 meltano-3.4.2/PKG-INFO
```

### Comparing `meltano-3.4.1b1/LICENSE` & `meltano-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/README.md` & `meltano-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/pyproject.toml` & `meltano-3.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltano"
-version = "3.4.1b1"
+version = "3.4.2"
 description = "Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love."
 authors = ["Meltano <hello@meltano.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/meltano/meltano"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -42,31 +42,31 @@
 [tool.poetry.dependencies]
 aiodocker = "^0.21.0"
 alembic = "^1.13.1"
 atomicwrites = "^1.2.1"
 azure-common = {version = "^1.1.28", optional = true}
 azure-core = {version = "^1.30.1", optional = true}
 azure-identity = {version = "^1.16.0", optional = true}
-azure-storage-blob = {version = "^12.19.1", optional = true}
-boto3 = {version = "^1.34.98", optional = true}
-check-jsonschema = "^0.28.2"
+azure-storage-blob = {version = "^12.20.0", optional = true}
+boto3 = {version = "^1.34.103", optional = true}
+check-jsonschema = "^0.28.3"
 click = "^8.1"
 click-default-group = "^1.2.4"
 click-didyoumean = "^0.3.1"
 croniter = "^2.0.5"
 fasteners = "^0.19"
 flatten-dict = "^0"
 google-cloud-storage = {version = ">=1.31.0", optional = true}
 importlib-resources = "^6.4.0"
 jinja2 = "^3.1.4"
 jsonschema = "^4.22"
 packaging = "^24.0"
 platformdirs = "^4.2.1"
 psutil = "^5.9.8"
-psycopg = {version = "^3.1.18", extras = ["binary"], optional = true}
+psycopg = {version = "^3.1.19", extras = ["binary"], optional = true}
 psycopg2-binary = {version="^2.9.9", optional=true}
 pyjwt = "^2.6.0"
 pymssql = {version = "^2.3.0", optional = true}
 python = ">=3.8,<3.13"
 python-dateutil = "^2.9.0"
 python-dotenv = "^1.0.1"
 python-slugify = "^8.0.4"
@@ -98,22 +98,22 @@
 psycopg2 = ["psycopg2-binary"]
 s3 = ["boto3"]
 uv = ["uv"]
 
 [tool.poetry.group.dev.dependencies]
 backoff = "^2.1.2"
 black = "^24.4.2"
-boto3-stubs = {extras = ["essential"], version = "1.34.98"}
+boto3-stubs = {extras = ["essential"], version = "1.34.103"}
 bumpversion = "^0.6.0"
 colorama = "^0.4.4"
 coverage = {extras = ["toml"], version = ">=7.3.2,!=7.3.3"}
-freezegun = "^1.5.0"
-hypothesis = "^6.100.4"
+freezegun = "^1.5.1"
+hypothesis = "^6.101.0"
 mock = "^5.0.2"
-moto = "^5.0.6"
+moto = "^5.0.7"
 mypy = "^1.10.0"
 pre-commit = "^3.5.0"
 pytest = "^8.2.0"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
 pytest-docker = "^3.1"
 pytest-httpserver = "^1.0.10"
@@ -122,15 +122,15 @@
 pytest-rerunfailures = "^14.0"
 pytest-structlog = "^0.8"
 pytest-xdist = "^3.6"
 requests-mock = "^1.12.1"
 setproctitle = "^1.3" # Used by pytest-xdist to aid with handling resource intensive processes.
 types-croniter = "^2.0.0"
 types-jsonschema = "^4.22.0.20240501"
-types-psutil = "^5.9.5.20240423"
+types-psutil = "^5.9.5.20240511"
 types-python-dateutil = "^2.9.0.20240316"
 types-python-slugify = "^8.0.2.20240310"
 types-pyyaml = "^6.0.12.20240311"
 types-requests = "^2.31.0"
 types-tabulate = "^0.9.0.20240106"
 
 [tool.poetry.scripts]
@@ -470,15 +470,15 @@
 skip_covered = true
 
 [tool.commitizen]
 name = "cz_version_bump"
 prerelease_offset = 1
 tag_format = "v$major.$minor.$patch$prerelease"
 changelog_merge_prerelease = true
-version = "3.4.1b1"
+version = "3.4.2"
 version_files = [
   "pyproject.toml:^version =",
   "src/meltano/__init__.py:^__version__ =",
   'docs/package.json:^  "version":',
 ]
 
 [tool.mypy]
```

### Comparing `meltano-3.4.1b1/src/meltano/cli/__init__.py` & `meltano-3.4.2/src/meltano/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/add.py` & `meltano-3.4.2/src/meltano/cli/add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/cli.py` & `meltano-3.4.2/src/meltano/cli/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/compile.py` & `meltano-3.4.2/src/meltano/cli/compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/config.py` & `meltano-3.4.2/src/meltano/cli/config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/elt.py` & `meltano-3.4.2/src/meltano/cli/elt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/environment.py` & `meltano-3.4.2/src/meltano/cli/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/hub.py` & `meltano-3.4.2/src/meltano/cli/hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/initialize.py` & `meltano-3.4.2/src/meltano/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/install.py` & `meltano-3.4.2/src/meltano/cli/install.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/interactive/config.py` & `meltano-3.4.2/src/meltano/cli/interactive/config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/invoke.py` & `meltano-3.4.2/src/meltano/cli/invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/job.py` & `meltano-3.4.2/src/meltano/cli/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/lock.py` & `meltano-3.4.2/src/meltano/cli/lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/params.py` & `meltano-3.4.2/src/meltano/cli/params.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/remove.py` & `meltano-3.4.2/src/meltano/cli/remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/run.py` & `meltano-3.4.2/src/meltano/cli/run.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/schedule.py` & `meltano-3.4.2/src/meltano/cli/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/schema.py` & `meltano-3.4.2/src/meltano/cli/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/select.py` & `meltano-3.4.2/src/meltano/cli/select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/state.py` & `meltano-3.4.2/src/meltano/cli/state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/upgrade.py` & `meltano-3.4.2/src/meltano/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/utils.py` & `meltano-3.4.2/src/meltano/cli/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/cli/validate.py` & `meltano-3.4.2/src/meltano/cli/validate.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/behavior/canonical.py` & `meltano-3.4.2/src/meltano/core/behavior/canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/behavior/hookable.py` & `meltano-3.4.2/src/meltano/core/behavior/hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/behavior/versioned.py` & `meltano-3.4.2/src/meltano/core/behavior/versioned.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/block/blockset.py` & `meltano-3.4.2/src/meltano/core/block/blockset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/block/extract_load.py` & `meltano-3.4.2/src/meltano/core/block/extract_load.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/block/future_utils.py` & `meltano-3.4.2/src/meltano/core/block/future_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/block/ioblock.py` & `meltano-3.4.2/src/meltano/core/block/ioblock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/block/parser.py` & `meltano-3.4.2/src/meltano/core/block/parser.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/block/plugin_command.py` & `meltano-3.4.2/src/meltano/core/block/plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/block/singer.py` & `meltano-3.4.2/src/meltano/core/block/singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/bundle/settings.yml` & `meltano-3.4.2/src/meltano/core/bundle/settings.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/cli_messages.py` & `meltano-3.4.2/src/meltano/core/cli_messages.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/config_service.py` & `meltano-3.4.2/src/meltano/core/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/container/container_service.py` & `meltano-3.4.2/src/meltano/core/container/container_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/container/container_spec.py` & `meltano-3.4.2/src/meltano/core/container/container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/db.py` & `meltano-3.4.2/src/meltano/core/db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/elt_context.py` & `meltano-3.4.2/src/meltano/core/elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/environment.py` & `meltano-3.4.2/src/meltano/core/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/environment_service.py` & `meltano-3.4.2/src/meltano/core/environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/error.py` & `meltano-3.4.2/src/meltano/core/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/hub/client.py` & `meltano-3.4.2/src/meltano/core/hub/client.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/hub/schema.py` & `meltano-3.4.2/src/meltano/core/hub/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/job/finder.py` & `meltano-3.4.2/src/meltano/core/job/finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/job/job.py` & `meltano-3.4.2/src/meltano/core/job/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/job/stale_job_failer.py` & `meltano-3.4.2/src/meltano/core/job/stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/job_state.py` & `meltano-3.4.2/src/meltano/core/job_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/locked_definition_service.py` & `meltano-3.4.2/src/meltano/core/locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/logging/__init__.py` & `meltano-3.4.2/src/meltano/core/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/logging/formatters.py` & `meltano-3.4.2/src/meltano/core/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/logging/job_logging_service.py` & `meltano-3.4.2/src/meltano/core/logging/job_logging_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/logging/output_logger.py` & `meltano-3.4.2/src/meltano/core/logging/output_logger.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/logging/utils.py` & `meltano-3.4.2/src/meltano/core/logging/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/manifest/__init__.py` & `meltano-3.4.2/src/meltano/core/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/manifest/contexts.py` & `meltano-3.4.2/src/meltano/core/manifest/contexts.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/manifest/jsonschema.py` & `meltano-3.4.2/src/meltano/core/manifest/jsonschema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/manifest/manifest.py` & `meltano-3.4.2/src/meltano/core/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/meltano_file.py` & `meltano-3.4.2/src/meltano/core/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/meltano_invoker.py` & `meltano-3.4.2/src/meltano/core/meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/migration_service.py` & `meltano-3.4.2/src/meltano/core/migration_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/airflow.py` & `meltano-3.4.2/src/meltano/core/plugin/airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/base.py` & `meltano-3.4.2/src/meltano/core/plugin/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/command.py` & `meltano-3.4.2/src/meltano/core/plugin/command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/config_service.py` & `meltano-3.4.2/src/meltano/core/plugin/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/dbt/base.py` & `meltano-3.4.2/src/meltano/core/plugin/dbt/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/error.py` & `meltano-3.4.2/src/meltano/core/plugin/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/factory.py` & `meltano-3.4.2/src/meltano/core/plugin/factory.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/file.py` & `meltano-3.4.2/src/meltano/core/plugin/file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/meltano_file.py` & `meltano-3.4.2/src/meltano/core/plugin/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/project_plugin.py` & `meltano-3.4.2/src/meltano/core/plugin/project_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/requirements.py` & `meltano-3.4.2/src/meltano/core/plugin/requirements.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/settings_service.py` & `meltano-3.4.2/src/meltano/core/plugin/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/singer/base.py` & `meltano-3.4.2/src/meltano/core/plugin/singer/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/singer/catalog.py` & `meltano-3.4.2/src/meltano/core/plugin/singer/catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/singer/mapper.py` & `meltano-3.4.2/src/meltano/core/plugin/singer/mapper.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/singer/tap.py` & `meltano-3.4.2/src/meltano/core/plugin/singer/tap.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/singer/target.py` & `meltano-3.4.2/src/meltano/core/plugin/singer/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         try:
             job.save(self.session)
             self.state_service.add_state(
                 job,
                 json.dumps(job.payload),
                 job.payload_flags,
             )
-        except Exception:
+        except Exception:  # pragma: no cover
+            logger.debug("Failed to persist state", exc_info=True)
             logger.warning(
                 "Unable to persist state, or received state is invalid, "
                 "incremental state has not been updated",
             )
         else:
             logger.info(f"Incremental state has been updated at {datetime.utcnow()}.")  # noqa: G004
             logger.debug(f"Incremental state: {new_state}")  # noqa: G004
```

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin/superset.py` & `meltano-3.4.2/src/meltano/core/plugin/superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin_install_service.py` & `meltano-3.4.2/src/meltano/core/plugin_install_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin_invoker.py` & `meltano-3.4.2/src/meltano/core/plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin_location_remove.py` & `meltano-3.4.2/src/meltano/core/plugin_location_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin_lock_service.py` & `meltano-3.4.2/src/meltano/core/plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin_remove_service.py` & `meltano-3.4.2/src/meltano/core/plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin_repository.py` & `meltano-3.4.2/src/meltano/core/plugin_repository.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/plugin_test_service.py` & `meltano-3.4.2/src/meltano/core/plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/project.py` & `meltano-3.4.2/src/meltano/core/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/project_add_service.py` & `meltano-3.4.2/src/meltano/core/project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/project_files.py` & `meltano-3.4.2/src/meltano/core/project_files.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/project_init_service.py` & `meltano-3.4.2/src/meltano/core/project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/project_plugins_service.py` & `meltano-3.4.2/src/meltano/core/project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/project_settings_service.py` & `meltano-3.4.2/src/meltano/core/project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/runner/dbt.py` & `meltano-3.4.2/src/meltano/core/runner/dbt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/runner/singer.py` & `meltano-3.4.2/src/meltano/core/runner/singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/schedule.py` & `meltano-3.4.2/src/meltano/core/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/schedule_service.py` & `meltano-3.4.2/src/meltano/core/schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/select_service.py` & `meltano-3.4.2/src/meltano/core/select_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/setting.py` & `meltano-3.4.2/src/meltano/core/setting.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/setting_definition.py` & `meltano-3.4.2/src/meltano/core/setting_definition.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/settings_service.py` & `meltano-3.4.2/src/meltano/core/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/settings_store.py` & `meltano-3.4.2/src/meltano/core/settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/sqlalchemy.py` & `meltano-3.4.2/src/meltano/core/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/state_service.py` & `meltano-3.4.2/src/meltano/core/state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/state_store/__init__.py` & `meltano-3.4.2/src/meltano/core/state_store/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/state_store/azure.py` & `meltano-3.4.2/src/meltano/core/state_store/azure.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/state_store/base.py` & `meltano-3.4.2/src/meltano/core/state_store/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/state_store/db.py` & `meltano-3.4.2/src/meltano/core/state_store/db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/state_store/filesystem.py` & `meltano-3.4.2/src/meltano/core/state_store/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,16 @@
             else:
                 try:
                     with self.get_reader(filepath) as current_state_reader:
                         current_state = JobState.from_file(
                             state.state_id,
                             current_state_reader,
                         )
-                        state_to_write = current_state.merge_partial(state)
+                        current_state.merge_partial(state)
+                        state_to_write = current_state
                 except Exception as e:
                     if self.is_file_not_found_error(e):
                         state_to_write = state
                     raise e
             with self.get_writer(filepath) as writer:
                 writer.write(state_to_write.json())
```

### Comparing `meltano-3.4.1b1/src/meltano/core/state_store/google.py` & `meltano-3.4.2/src/meltano/core/state_store/google.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/state_store/s3.py` & `meltano-3.4.2/src/meltano/core/state_store/s3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/task_sets.py` & `meltano-3.4.2/src/meltano/core/task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/task_sets_service.py` & `meltano-3.4.2/src/meltano/core/task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/README.md` & `meltano-3.4.2/src/meltano/core/tracking/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/contexts/cli.py` & `meltano-3.4.2/src/meltano/core/tracking/contexts/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/contexts/environment.py` & `meltano-3.4.2/src/meltano/core/tracking/contexts/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/contexts/exception.py` & `meltano-3.4.2/src/meltano/core/tracking/contexts/exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/contexts/plugins.py` & `meltano-3.4.2/src/meltano/core/tracking/contexts/plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/contexts/project.py` & `meltano-3.4.2/src/meltano/core/tracking/contexts/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0` & `meltano-3.4.2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/micro.conf` & `meltano-3.4.2/src/meltano/core/tracking/micro.conf`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/schemas.py` & `meltano-3.4.2/src/meltano/core/tracking/schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/tracking/tracker.py` & `meltano-3.4.2/src/meltano/core/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/transform_add_service.py` & `meltano-3.4.2/src/meltano/core/transform_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/upgrade_service.py` & `meltano-3.4.2/src/meltano/core/upgrade_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/utils/__init__.py` & `meltano-3.4.2/src/meltano/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/utils/pidfile.py` & `meltano-3.4.2/src/meltano/core/utils/pidfile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/validation_service.py` & `meltano-3.4.2/src/meltano/core/validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/venv_service.py` & `meltano-3.4.2/src/meltano/core/venv_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/core/yaml.py` & `meltano-3.4.2/src/meltano/core/yaml.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/env.py` & `meltano-3.4.2/src/meltano/migrations/env.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/utils/dialect_typing.py` & `meltano-3.4.2/src/meltano/migrations/utils/dialect_typing.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py` & `meltano-3.4.2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py` & `meltano-3.4.2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py` & `meltano-3.4.2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py` & `meltano-3.4.2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py` & `meltano-3.4.2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py` & `meltano-3.4.2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/6ef30ab7b8e5_.py` & `meltano-3.4.2/src/meltano/migrations/versions/6ef30ab7b8e5_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py` & `meltano-3.4.2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py` & `meltano-3.4.2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py` & `meltano-3.4.2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/b4c05e463b53_.py` & `meltano-3.4.2/src/meltano/migrations/versions/b4c05e463b53_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py` & `meltano-3.4.2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py` & `meltano-3.4.2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py` & `meltano-3.4.2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/src/meltano/schemas/meltano.schema.json` & `meltano-3.4.2/src/meltano/schemas/meltano.schema.json`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/conftest.py` & `meltano-3.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/cli.py` & `meltano-3.4.2/tests/fixtures/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/core.py` & `meltano-3.4.2/tests/fixtures/core.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/db/__init__.py` & `meltano-3.4.2/tests/fixtures/db/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/db/mssql.py` & `meltano-3.4.2/tests/fixtures/db/mssql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/db/postgresql.py` & `meltano-3.4.2/tests/fixtures/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/db/postgresql_psycopg3.py` & `meltano-3.4.2/tests/fixtures/db/postgresql_psycopg3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/docker/__init__.py` & `meltano-3.4.2/tests/fixtures/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/docker/snowplow.py` & `meltano-3.4.2/tests/fixtures/docker/snowplow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/fs.py` & `meltano-3.4.2/tests/fixtures/fs.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/large_config_project/meltano.yml` & `meltano-3.4.2/tests/fixtures/large_config_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/large_config_project/schedule.yml` & `meltano-3.4.2/tests/fixtures/large_config_project/schedule.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/multifile_project/meltano.yml` & `meltano-3.4.2/tests/fixtures/multifile_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/plugins/extractors/tap-custom/test.yml` & `meltano-3.4.2/tests/fixtures/plugins/extractors/tap-custom/test.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/fixtures/utils.py` & `meltano-3.4.2/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_add.py` & `meltano-3.4.2/tests/meltano/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_cli.py` & `meltano-3.4.2/tests/meltano/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_compile.py` & `meltano-3.4.2/tests/meltano/cli/test_compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_config.py` & `meltano-3.4.2/tests/meltano/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_elt.py` & `meltano-3.4.2/tests/meltano/cli/test_elt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_hub.py` & `meltano-3.4.2/tests/meltano/cli/test_hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_initialize.py` & `meltano-3.4.2/tests/meltano/cli/test_initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_install.py` & `meltano-3.4.2/tests/meltano/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_invoke.py` & `meltano-3.4.2/tests/meltano/cli/test_invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_job_cmd.py` & `meltano-3.4.2/tests/meltano/cli/test_job_cmd.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_lock.py` & `meltano-3.4.2/tests/meltano/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_remove.py` & `meltano-3.4.2/tests/meltano/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_run.py` & `meltano-3.4.2/tests/meltano/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_schedule.py` & `meltano-3.4.2/tests/meltano/cli/test_schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_select.py` & `meltano-3.4.2/tests/meltano/cli/test_select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_state.py` & `meltano-3.4.2/tests/meltano/cli/test_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/cli/test_upgrade.py` & `meltano-3.4.2/tests/meltano/cli/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/behavior/test_canonical.py` & `meltano-3.4.2/tests/meltano/core/behavior/test_canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/behavior/test_hookable.py` & `meltano-3.4.2/tests/meltano/core/behavior/test_hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/block/test_extract_load.py` & `meltano-3.4.2/tests/meltano/core/block/test_extract_load.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/block/test_plugin_command.py` & `meltano-3.4.2/tests/meltano/core/block/test_plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/block/test_singer.py` & `meltano-3.4.2/tests/meltano/core/block/test_singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/container/test_container_spec.py` & `meltano-3.4.2/tests/meltano/core/container/test_container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/hub/test_meltano_hub_service.py` & `meltano-3.4.2/tests/meltano/core/hub/test_meltano_hub_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/job/test_finder.py` & `meltano-3.4.2/tests/meltano/core/job/test_finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/job/test_job.py` & `meltano-3.4.2/tests/meltano/core/job/test_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/job/test_stale_job_failer.py` & `meltano-3.4.2/tests/meltano/core/job/test_stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/logging/test_formatters.py` & `meltano-3.4.2/tests/meltano/core/logging/test_formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/logging/test_logging_utils.py` & `meltano-3.4.2/tests/meltano/core/logging/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/logging/test_output_logger.py` & `meltano-3.4.2/tests/meltano/core/logging/test_output_logger.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_catalog.py` & `meltano-3.4.2/tests/meltano/core/plugin/singer/test_catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_mapper.py` & `meltano-3.4.2/tests/meltano/core/plugin/singer/test_mapper.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_tap.py` & `meltano-3.4.2/tests/meltano/core/plugin/singer/test_tap.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/singer/test_target.py` & `meltano-3.4.2/tests/meltano/core/plugin/singer/test_target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/test_airflow.py` & `meltano-3.4.2/tests/meltano/core/plugin/test_airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/test_command.py` & `meltano-3.4.2/tests/meltano/core/plugin/test_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin.py` & `meltano-3.4.2/tests/meltano/core/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/test_plugin_settings.py` & `meltano-3.4.2/tests/meltano/core/plugin/test_plugin_settings.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/plugin/test_superset.py` & `meltano-3.4.2/tests/meltano/core/plugin/test_superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/runner/test_runner.py` & `meltano-3.4.2/tests/meltano/core/runner/test_runner.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/state_store/test_db.py` & `meltano-3.4.2/tests/meltano/core/state_store/test_db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/state_store/test_filesystem.py` & `meltano-3.4.2/tests/meltano/core/state_store/test_filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,14 +174,44 @@
                 os.path.join(state_path, encode_if_on_windows(state_id), "state.json"),
             ) as state_file:
                 assert JobState.from_json(
                     state_id,
                     json.dumps({"completed": expected_state}),
                 ) == JobState.from_file(state_id, state_file)
 
+    def test_set_partial_state(
+        self,
+        subject: LocalFilesystemStateStoreManager,
+        state_path: str,
+        state_ids_with_expected_states,
+    ):
+        def _get_state_path(state_id: str) -> str:
+            return os.path.join(
+                state_path,
+                encode_if_on_windows(state_id),
+                "state.json",
+            )
+
+        def _seed_state(state_id: str, state: dict) -> None:
+            state_file = Path(_get_state_path(state_id))
+            state_file.parent.mkdir(parents=True, exist_ok=True)
+            state_file.write_text(json.dumps({"partial": state}))
+
+        for state_id, expected_state in state_ids_with_expected_states:
+            _seed_state(state_id, expected_state)
+            subject.set(
+                JobState.from_json(state_id, json.dumps({"partial": expected_state})),
+            )
+        for state_id, expected_state in state_ids_with_expected_states:
+            with open(_get_state_path(state_id)) as state_file:
+                assert JobState.from_json(
+                    state_id,
+                    json.dumps({"partial": expected_state}),
+                ) == JobState.from_file(state_id, state_file)
+
     def test_delete(
         self,
         subject: LocalFilesystemStateStoreManager,
         state_path,
         state_ids_with_expected_states,
     ):
         # Delete files
```

### Comparing `meltano-3.4.1b1/tests/meltano/core/state_store/test_state_store.py` & `meltano-3.4.2/tests/meltano/core/state_store/test_state_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_db_compat.py` & `meltano-3.4.2/tests/meltano/core/test_db_compat.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_db_connection.py` & `meltano-3.4.2/tests/meltano/core/test_db_connection.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_elt_context.py` & `meltano-3.4.2/tests/meltano/core/test_elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_environment_service.py` & `meltano-3.4.2/tests/meltano/core/test_environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_environment_variables.py` & `meltano-3.4.2/tests/meltano/core/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_locked_definition_service.py` & `meltano-3.4.2/tests/meltano/core/test_locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_meltano_file.py` & `meltano-3.4.2/tests/meltano/core/test_meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_meltano_invoker.py` & `meltano-3.4.2/tests/meltano/core/test_meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_plugin_install_service.py` & `meltano-3.4.2/tests/meltano/core/test_plugin_install_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_plugin_invoker.py` & `meltano-3.4.2/tests/meltano/core/test_plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_plugin_lock_service.py` & `meltano-3.4.2/tests/meltano/core/test_plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_plugin_remove_service.py` & `meltano-3.4.2/tests/meltano/core/test_plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_plugin_test_service.py` & `meltano-3.4.2/tests/meltano/core/test_plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_project.py` & `meltano-3.4.2/tests/meltano/core/test_project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_project_add_service.py` & `meltano-3.4.2/tests/meltano/core/test_project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_project_files.py` & `meltano-3.4.2/tests/meltano/core/test_project_files.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_project_init_service.py` & `meltano-3.4.2/tests/meltano/core/test_project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_project_plugins_service.py` & `meltano-3.4.2/tests/meltano/core/test_project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_project_settings_service.py` & `meltano-3.4.2/tests/meltano/core/test_project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_schedule_service.py` & `meltano-3.4.2/tests/meltano/core/test_schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_setting_definition.py` & `meltano-3.4.2/tests/meltano/core/test_setting_definition.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_settings_store.py` & `meltano-3.4.2/tests/meltano/core/test_settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_state_service.py` & `meltano-3.4.2/tests/meltano/core/test_state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_task_sets.py` & `meltano-3.4.2/tests/meltano/core/test_task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_task_sets_service.py` & `meltano-3.4.2/tests/meltano/core/test_task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_utils.py` & `meltano-3.4.2/tests/meltano/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_validation_service.py` & `meltano-3.4.2/tests/meltano/core/test_validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/test_venv_service.py` & `meltano-3.4.2/tests/meltano/core/test_venv_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/tracking/test_environment_context.py` & `meltano-3.4.2/tests/meltano/core/tracking/test_environment_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/tracking/test_exception.py` & `meltano-3.4.2/tests/meltano/core/tracking/test_exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/tracking/test_plugins.py` & `meltano-3.4.2/tests/meltano/core/tracking/test_plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/tracking/test_project_context.py` & `meltano-3.4.2/tests/meltano/core/tracking/test_project_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/tracking/test_schemas.py` & `meltano-3.4.2/tests/meltano/core/tracking/test_schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/tests/meltano/core/tracking/test_tracker.py` & `meltano-3.4.2/tests/meltano/core/tracking/test_tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.1b1/PKG-INFO` & `meltano-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltano
-Version: 3.4.1b1
+Version: 3.4.2
 Summary: Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love.
 Home-page: https://meltano.com
 License: MIT
 Keywords: Meltano,ELT,Data integration,singer-io,dbt
 Author: Meltano
 Author-email: hello@meltano.com
 Requires-Python: >=3.8,<3.13
@@ -27,32 +27,32 @@
 Provides-Extra: uv
 Requires-Dist: aiodocker (>=0.21.0,<0.22.0)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: atomicwrites (>=1.2.1,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-core (>=1.30.1,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0) ; extra == "azure"
-Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0) ; extra == "azure"
-Requires-Dist: boto3 (>=1.34.98,<2.0.0) ; extra == "s3"
-Requires-Dist: check-jsonschema (>=0.28.2,<0.29.0)
+Requires-Dist: azure-storage-blob (>=12.20.0,<13.0.0) ; extra == "azure"
+Requires-Dist: boto3 (>=1.34.103,<2.0.0) ; extra == "s3"
+Requires-Dist: check-jsonschema (>=0.28.3,<0.29.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
 Requires-Dist: click-didyoumean (>=0.3.1,<0.4.0)
 Requires-Dist: croniter (>=2.0.5,<3.0.0)
 Requires-Dist: fasteners (>=0.19,<0.20)
 Requires-Dist: flatten-dict (>=0,<1)
 Requires-Dist: google-cloud-storage (>=1.31.0) ; extra == "gcs"
 Requires-Dist: importlib-resources (>=6.4.0,<7.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: jsonschema (>=4.22,<5.0)
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: platformdirs (>=4.2.1,<5.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "psycopg2"
-Requires-Dist: psycopg[binary] (>=3.1.18,<4.0.0) ; extra == "postgres"
+Requires-Dist: psycopg[binary] (>=3.1.19,<4.0.0) ; extra == "postgres"
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pymssql (>=2.3.0,<3.0.0) ; extra == "mssql"
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: python-ulid (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
```

