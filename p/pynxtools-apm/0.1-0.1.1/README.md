# Comparing `tmp/pynxtools_apm-0.1.tar.gz` & `tmp/pynxtools_apm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynxtools_apm-0.1.tar", last modified: Fri Apr 26 16:00:58 2024, max compression
+gzip compressed data, was "pynxtools_apm-0.1.1.tar", last modified: Wed May 15 07:36:32 2024, max compression
```

## Comparing `pynxtools_apm-0.1.tar` & `pynxtools_apm-0.1.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.694215 pynxtools_apm-0.1/.github/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/.github/workflows/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      753 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/.github/workflows/build_docs.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      745 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/.github/workflows/publish.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      858 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/.github/workflows/pylint.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      764 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/.github/workflows/pytest.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3882 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/.gitignore
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      200 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/.precommit-config.yaml
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/.vscode/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      541 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/.vscode/settings.json
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11357 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/LICENSE
--rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     4926 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/PKG-INFO
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3571 2024-04-24 14:31:32.000000 pynxtools_apm-0.1/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      753 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/build_docs.yml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10270 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/dev-requirements.txt
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/explanation/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      796 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/explanation/learn.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/explanation/media/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      439 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/explanation/media/workflow.mermaid
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   108134 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/explanation/media/workflow.png
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2090 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/explanation/performance.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/how-tos/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        9 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/how-tos/howto.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2317 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/index.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      526 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/macros.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/reference/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      693 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/apt.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1102 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/ato.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      358 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/atomtypes.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1642 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/camecaroot.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2682 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/contextualization.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1517 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/csv.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      856 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/env.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      547 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/epos.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1453 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/faufig.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      360 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/inspico.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      368 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/mqanalysis.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      357 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/pos.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1120 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/pyccapt.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      967 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/rng.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      972 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/reference/rrng.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/stylesheets/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1097 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/stylesheets/extra.css
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/tutorial/
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/docs/tutorial/media/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    69876 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/tutorial/media/upload-processing.gif
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      172 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/tutorial/nexusio.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      513 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/tutorial/oasis.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1040 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/docs/tutorial/standalone.md
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/examples/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7086 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/examples/HowToUseNXapmNeXusFileTutorial.ipynb
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10705 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/examples/HowToUseTutorial.ipynb
--rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      391 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/examples/apm.batch.sh
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      940 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/examples/apm.oasis.specific.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2451 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/examples/eln_data.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1449 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/mkdocs.yaml
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/pynxtools_apm/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3104 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/README.md
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/__init__.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/pynxtools_apm/concepts/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/concepts/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    16376 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/pynxtools_apm/concepts/mapping_functors.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.698215 pynxtools_apm-0.1/pynxtools_apm/config/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6328 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/config/eln_cfg.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3915 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/config/oasis_cfg.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6926 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/pynxtools_apm/reader.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/pynxtools_apm/utils/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/__init__.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9402 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/create_nx_default_plots.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    27427 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/generate_synthetic_data.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1124 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/get_file_checksum.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1195 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/get_gitrepo_commit.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1249 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/interpret_boolean.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7206 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/io_case_logic.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    15230 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/pynxtools_apm/utils/load_ranging.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11041 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/load_reconstruction.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3655 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/pynxtools_apm/utils/oasis_config_reader.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10998 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/pynxtools_apm/utils/oasis_eln_reader.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8371 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/parse_composition_table.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1498 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/string_conversions.py
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1286 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/pynxtools_apm/utils/versioning.py
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/pynxtools_apm.egg-info/
--rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     4926 2024-04-26 16:00:58.000000 pynxtools_apm-0.1/pynxtools_apm.egg-info/PKG-INFO
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2278 2024-04-26 16:00:58.000000 pynxtools_apm-0.1/pynxtools_apm.egg-info/SOURCES.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        1 2024-04-26 16:00:58.000000 pynxtools_apm-0.1/pynxtools_apm.egg-info/dependency_links.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       56 2024-04-26 16:00:58.000000 pynxtools_apm-0.1/pynxtools_apm.egg-info/entry_points.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      183 2024-04-26 16:00:58.000000 pynxtools_apm-0.1/pynxtools_apm.egg-info/requires.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       14 2024-04-26 16:00:58.000000 pynxtools_apm-0.1/pynxtools_apm.egg-info/top_level.txt
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2531 2024-04-26 15:52:22.000000 pynxtools_apm-0.1/pyproject.toml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       38 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/setup.cfg
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/tests/
--rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)     4302 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/tests/batch_queue.04.sh
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/tests/data/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        2 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/tests/data/config_file.json
-drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-04-26 16:00:58.702215 pynxtools_apm-0.1/tests/data/nomad_oasis_eln_schema_for_nx_apm/
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    31218 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/tests/data/nomad_oasis_eln_schema_for_nx_apm/nxapm.schema.archive.yaml
--rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1864 2024-04-24 13:25:57.000000 pynxtools_apm-0.1/tests/test_reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.089683 pynxtools_apm-0.1.1/.github/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.089683 pynxtools_apm-0.1.1/.github/workflows/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      753 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/.github/workflows/build_docs.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      745 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/.github/workflows/publish.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      858 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/.github/workflows/pylint.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      764 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/.github/workflows/pytest.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3882 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/.gitignore
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      200 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/.precommit-config.yaml
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.089683 pynxtools_apm-0.1.1/.vscode/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      541 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/.vscode/settings.json
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11357 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/LICENSE
+-rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     5271 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/PKG-INFO
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3785 2024-05-11 10:23:55.000000 pynxtools_apm-0.1.1/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      753 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/build_docs.yml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10403 2024-05-10 11:48:45.000000 pynxtools_apm-0.1.1/dev-requirements.txt
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.089683 pynxtools_apm-0.1.1/docs/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.089683 pynxtools_apm-0.1.1/docs/explanation/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      796 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/explanation/learn.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.089683 pynxtools_apm-0.1.1/docs/explanation/media/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      439 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/explanation/media/workflow.mermaid
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)   108134 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/explanation/media/workflow.png
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2090 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/explanation/performance.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.089683 pynxtools_apm-0.1.1/docs/how-tos/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        9 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/how-tos/howto.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2317 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/index.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      526 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/macros.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.093683 pynxtools_apm-0.1.1/docs/reference/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      693 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/apt.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1102 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/ato.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      358 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/atomtypes.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1642 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/camecaroot.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2682 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/contextualization.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1517 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/csv.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      856 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/env.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      547 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/epos.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1453 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/faufig.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      360 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/inspico.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      368 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/mqanalysis.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      357 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/pos.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1120 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/pyccapt.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      967 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/rng.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      972 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/reference/rrng.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.093683 pynxtools_apm-0.1.1/docs/stylesheets/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1097 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/stylesheets/extra.css
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.093683 pynxtools_apm-0.1.1/docs/tutorial/
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.093683 pynxtools_apm-0.1.1/docs/tutorial/media/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    69876 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/tutorial/media/upload-processing.gif
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      172 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/tutorial/nexusio.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      513 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/tutorial/oasis.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1040 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/docs/tutorial/standalone.md
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.093683 pynxtools_apm-0.1.1/examples/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7086 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/examples/HowToUseNXapmNeXusFileTutorial.ipynb
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10709 2024-05-10 11:48:45.000000 pynxtools_apm-0.1.1/examples/HowToUseTutorial.ipynb
+-rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)      391 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/examples/apm.batch.sh
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      940 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/examples/apm.oasis.specific.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2451 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/examples/eln_data.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1449 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/mkdocs.yaml
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.093683 pynxtools_apm-0.1.1/pynxtools_apm/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3104 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/README.md
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/__init__.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/pynxtools_apm/concepts/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/concepts/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    16376 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/concepts/mapping_functors.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/pynxtools_apm/config/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6327 2024-05-10 11:48:45.000000 pynxtools_apm-0.1.1/pynxtools_apm/config/eln_cfg.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3806 2024-05-15 07:34:46.000000 pynxtools_apm-0.1.1/pynxtools_apm/config/oasis_cfg.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     6926 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/reader.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/pynxtools_apm/utils/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/__init__.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     9418 2024-05-10 11:48:45.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/create_nx_default_plots.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    27343 2024-05-15 07:34:46.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/generate_synthetic_data.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1124 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/get_file_checksum.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1195 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/get_gitrepo_commit.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1249 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/interpret_boolean.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     7206 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/io_case_logic.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    15230 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/load_ranging.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    11041 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/load_reconstruction.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     3655 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/oasis_config_reader.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    10998 2024-05-10 11:48:45.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/oasis_eln_reader.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     8371 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/parse_composition_table.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1498 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/string_conversions.py
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1257 2024-05-15 07:34:46.000000 pynxtools_apm-0.1.1/pynxtools_apm/utils/versioning.py
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/pynxtools_apm.egg-info/
+-rw-r--r--   0 kaiobach  (1000) kaiobach  (1000)     5271 2024-05-15 07:36:32.000000 pynxtools_apm-0.1.1/pynxtools_apm.egg-info/PKG-INFO
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2278 2024-05-15 07:36:32.000000 pynxtools_apm-0.1.1/pynxtools_apm.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        1 2024-05-15 07:36:32.000000 pynxtools_apm-0.1.1/pynxtools_apm.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       56 2024-05-15 07:36:32.000000 pynxtools_apm-0.1.1/pynxtools_apm.egg-info/entry_points.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)      219 2024-05-15 07:36:32.000000 pynxtools_apm-0.1.1/pynxtools_apm.egg-info/requires.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       14 2024-05-15 07:36:32.000000 pynxtools_apm-0.1.1/pynxtools_apm.egg-info/top_level.txt
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     2587 2024-05-10 11:48:45.000000 pynxtools_apm-0.1.1/pyproject.toml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)       38 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/setup.cfg
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/tests/
+-rwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)     4302 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/tests/batch_queue.04.sh
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/tests/data/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)        2 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/tests/data/config_file.json
+drwxrwxr-x   0 kaiobach  (1000) kaiobach  (1000)        0 2024-05-15 07:36:32.097684 pynxtools_apm-0.1.1/tests/data/nomad_oasis_eln_schema_for_nx_apm/
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)    31218 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/tests/data/nomad_oasis_eln_schema_for_nx_apm/nxapm.schema.archive.yaml
+-rw-rw-r--   0 kaiobach  (1000) kaiobach  (1000)     1864 2024-05-08 10:25:24.000000 pynxtools_apm-0.1.1/tests/test_reader.py
```

### Comparing `pynxtools_apm-0.1/.github/workflows/build_docs.yml` & `pynxtools_apm-0.1.1/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/.github/workflows/publish.yml` & `pynxtools_apm-0.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/.github/workflows/pylint.yml` & `pynxtools_apm-0.1.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/.github/workflows/pytest.yml` & `pynxtools_apm-0.1.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/.gitignore` & `pynxtools_apm-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/.vscode/settings.json` & `pynxtools_apm-0.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/LICENSE` & `pynxtools_apm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/PKG-INFO` & `pynxtools_apm-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-apm
-Version: 0.1
+Version: 0.1.1
 Summary: Make atom probe tomography and field-ion microscopy results interoperable via NeXus
 Author-email: Markus Kühbach <markus.kuehbach@physik.hu-berlin.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-apm
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-apm/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,14 +25,17 @@
 Requires-Dist: mkdocs-macros-plugin; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: jupyterlab-h5web; extra == "dev"
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-apm/actions/workflows/pytest.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-apm/actions/workflows/pylint.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-apm/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/pynxtools-apm)
 ![](https://img.shields.io/pypi/l/pynxtools-apm)
@@ -60,32 +63,31 @@
 
 ## Supported file formats
 This plugin supports the majority of the file formats that are currently used for atom probe.
 A detailed summary is available in the [reference section of the documentation](https://fairmat-nfdi.github.io/pynxtools-apm).
 
 # Getting started
 [A getting started tutorial](https://github.com/FAIRmat-NFDI/pynxtools-apm/tree/main/examples) is offered that guides you
-how to use the apm reader for converting your data to NeXus from a Jupyter notebook. Note that not every combination of
-supported file formats and input for the parser allows to fill required and recommended fields and attributes of the NXapm
-application definition. Therefore, you may need to provide an ELN file that contains the missing values in order for the
+how to use the apm reader for converting your data to NeXus using a Jupyter notebook. That notebook details also the commands how to convert data via command line calls. Note that not every combination of input from a supported file format and other, typically electronic lab notebook, input for the parser allows filling the required and recommended fields and attributes of the NXapm application definition.
+Therefore, you may need to provide an ELN file that contains the missing values in order for the
 validation step of the APM reader to pass.
 
 # Contributing
 We are continously working on adding parsers for other data formats, technology partners, and atom probers.
 If you would like to implement a parser for your data, feel free to get in contact.
 
 ## Development install
 Install the package with its dependencies:
 
 ```shell
 git clone https://github.com/FAIRmat-NFDI/pynxtools-apm.git --branch main --recursive pynxtools_apm
 cd pynxtools_apm
 python -m pip install --upgrade pip
 python -m pip install -e .
-python -m pip install -e ".[dev]"
+python -m pip install -e ".[dev,docs]"
 ```
 
 <!---There is also a [pre-commit hook](https://pre-commit.com/#intro) available
 which formats the code and checks the linting before actually commiting.
 It can be installed with
 ```shell
 pre-commit install
@@ -99,8 +101,8 @@
 [pytest](https://docs.pytest.org/en/stable/) which can be used as follows:
 
 ```shell
 python -m pytest -sv tests
 ```
 
 ## Contact person in FAIRmat for this reader
-Markus Kühbach
+[Markus Kühbach](https://www.fairmat-nfdi.eu/fairmat/about-fairmat/team-fairmat)
```

### Comparing `pynxtools_apm-0.1/README.md` & `pynxtools_apm-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,32 +28,31 @@
 
 ## Supported file formats
 This plugin supports the majority of the file formats that are currently used for atom probe.
 A detailed summary is available in the [reference section of the documentation](https://fairmat-nfdi.github.io/pynxtools-apm).
 
 # Getting started
 [A getting started tutorial](https://github.com/FAIRmat-NFDI/pynxtools-apm/tree/main/examples) is offered that guides you
-how to use the apm reader for converting your data to NeXus from a Jupyter notebook. Note that not every combination of
-supported file formats and input for the parser allows to fill required and recommended fields and attributes of the NXapm
-application definition. Therefore, you may need to provide an ELN file that contains the missing values in order for the
+how to use the apm reader for converting your data to NeXus using a Jupyter notebook. That notebook details also the commands how to convert data via command line calls. Note that not every combination of input from a supported file format and other, typically electronic lab notebook, input for the parser allows filling the required and recommended fields and attributes of the NXapm application definition.
+Therefore, you may need to provide an ELN file that contains the missing values in order for the
 validation step of the APM reader to pass.
 
 # Contributing
 We are continously working on adding parsers for other data formats, technology partners, and atom probers.
 If you would like to implement a parser for your data, feel free to get in contact.
 
 ## Development install
 Install the package with its dependencies:
 
 ```shell
 git clone https://github.com/FAIRmat-NFDI/pynxtools-apm.git --branch main --recursive pynxtools_apm
 cd pynxtools_apm
 python -m pip install --upgrade pip
 python -m pip install -e .
-python -m pip install -e ".[dev]"
+python -m pip install -e ".[dev,docs]"
 ```
 
 <!---There is also a [pre-commit hook](https://pre-commit.com/#intro) available
 which formats the code and checks the linting before actually commiting.
 It can be installed with
 ```shell
 pre-commit install
@@ -67,8 +66,8 @@
 [pytest](https://docs.pytest.org/en/stable/) which can be used as follows:
 
 ```shell
 python -m pytest -sv tests
 ```
 
 ## Contact person in FAIRmat for this reader
-Markus Kühbach
+[Markus Kühbach](https://www.fairmat-nfdi.eu/fairmat/about-fairmat/team-fairmat)
```

### Comparing `pynxtools_apm-0.1/build_docs.yml` & `pynxtools_apm-0.1.1/build_docs.yml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/dev-requirements.txt` & `pynxtools_apm-0.1.1/dev-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,17 @@
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter==1.0.0
-    # via ifes-apt-tc-data-modeling
+    # via
+    #   ifes-apt-tc-data-modeling
+    #   pynxtools-apm (pyproject.toml)
 jupyter-client==8.6.1
     # via
     #   ipykernel
     #   jupyter-console
     #   jupyter-server
     #   nbclient
     #   qtconsole
@@ -182,16 +184,19 @@
     #   notebook-shim
 jupyter-server-terminals==0.5.3
     # via jupyter-server
 jupyterlab==4.1.7
     # via
     #   ifes-apt-tc-data-modeling
     #   notebook
+    #   pynxtools-apm (pyproject.toml)
 jupyterlab-h5web==12.1.0
-    # via ifes-apt-tc-data-modeling
+    # via
+    #   ifes-apt-tc-data-modeling
+    #   pynxtools-apm (pyproject.toml)
 jupyterlab-pygments==0.3.0
     # via nbconvert
 jupyterlab-server==2.27.1
     # via
     #   jupyterlab
     #   notebook
 jupyterlab-widgets==3.0.10
```

### Comparing `pynxtools_apm-0.1/docs/explanation/learn.md` & `pynxtools_apm-0.1.1/docs/explanation/learn.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/explanation/media/workflow.png` & `pynxtools_apm-0.1.1/docs/explanation/media/workflow.png`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/explanation/performance.md` & `pynxtools_apm-0.1.1/docs/explanation/performance.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/index.md` & `pynxtools_apm-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/macros.py` & `pynxtools_apm-0.1.1/docs/macros.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/apt.md` & `pynxtools_apm-0.1.1/docs/reference/apt.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/ato.md` & `pynxtools_apm-0.1.1/docs/reference/ato.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/camecaroot.md` & `pynxtools_apm-0.1.1/docs/reference/camecaroot.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/contextualization.md` & `pynxtools_apm-0.1.1/docs/reference/contextualization.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/csv.md` & `pynxtools_apm-0.1.1/docs/reference/csv.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/env.md` & `pynxtools_apm-0.1.1/docs/reference/env.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/epos.md` & `pynxtools_apm-0.1.1/docs/reference/epos.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/faufig.md` & `pynxtools_apm-0.1.1/docs/reference/faufig.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/pyccapt.md` & `pynxtools_apm-0.1.1/docs/reference/pyccapt.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/rng.md` & `pynxtools_apm-0.1.1/docs/reference/rng.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/reference/rrng.md` & `pynxtools_apm-0.1.1/docs/reference/rrng.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/stylesheets/extra.css` & `pynxtools_apm-0.1.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/tutorial/media/upload-processing.gif` & `pynxtools_apm-0.1.1/docs/tutorial/media/upload-processing.gif`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/tutorial/oasis.md` & `pynxtools_apm-0.1.1/docs/tutorial/oasis.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/docs/tutorial/standalone.md` & `pynxtools_apm-0.1.1/docs/tutorial/standalone.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/examples/HowToUseNXapmNeXusFileTutorial.ipynb` & `pynxtools_apm-0.1.1/examples/HowToUseNXapmNeXusFileTutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/examples/HowToUseTutorial.ipynb` & `pynxtools_apm-0.1.1/examples/HowToUseTutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996204278812975%*

 * *Differences: {"'cells'": "{12: {'source': {insert: [(5, '  lab equipment. The benefit of such an approach is "*

 * *            "that eventual all relevant metadata to an instrument can be read from<br>\\n')], "*

 * *            "delete: [5]}}, 21: {'source': {insert: [(1, 'Dr.-Ing. Markus Kühbach, "*

 * *            "2024/05/10<br>\\n')], delete: [1]}}}"}*

```diff
@@ -123,15 +123,15 @@
             "metadata": {},
             "source": [
                 "This example shows the types of files from which the parser collects and normalizes pieces of information:<br>\n",
                 "* **eln_data_apm.yaml** metadata collected with an electronic lab notebook (ELN) such as a NOMAD Oasis custom schema<br>\n",
                 "* **apm.oasis.specific.yaml** frequently used metadata that are often the same for many datasets to avoid having to<br>\n",
                 "  type it every time in ELN templates. This file can be considered a configuration file whereby e.g. coordinate system<br>\n",
                 "  conventions can be injected or details about the atom probe instrument communicated if that is part of frequently used<br>\n",
-                "  lab equipment. The benefit of such an approach is that eventual all relevant metadata to an instrument can be read from\n",
+                "  lab equipment. The benefit of such an approach is that eventual all relevant metadata to an instrument can be read from<br>\n",
                 "  this configuration file via guiding the user e.g. through the ELN with an option to select the instrument.<br>\n",
                 "* **reconstructed ion positions** in community, technology partner format with<br>\n",
                 "  the ion positions and mass-to-charge state ratio values for the tomographic reconstruction.<br>\n",
                 "* **ranging definitions** in community / technology partner formatting with<br>\n",
                 "  the definitions how mass-to-charge-state-ratio values map on ion species.<br>\n",
                 "\n",
                 "The tool supports the most commonly used information exchange formats of the atom probe community.<br>\n",
@@ -234,15 +234,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Contact person for pynxtools-apm and related examples in FAIRmat:\n",
-                "Dr.-Ing. Markus K\u00fchbach, 2024/04/18<br>\n",
+                "Dr.-Ing. Markus K\u00fchbach, 2024/05/10<br>\n",
                 "\n",
                 "### Funding\n",
                 "<a href=\"https://www.fairmat-nfdi.eu/fairmat\">FAIRmat</a> is a consortium on research data management which is part of the German NFDI.<br>\n",
                 "The project is funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) \u2013 project 460197019."
             ]
         },
         {
```

### Comparing `pynxtools_apm-0.1/examples/apm.oasis.specific.yaml` & `pynxtools_apm-0.1.1/examples/apm.oasis.specific.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/examples/eln_data.yaml` & `pynxtools_apm-0.1.1/examples/eln_data.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/mkdocs.yaml` & `pynxtools_apm-0.1.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/README.md` & `pynxtools_apm-0.1.1/pynxtools_apm/README.md`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/concepts/mapping_functors.py` & `pynxtools_apm-0.1.1/pynxtools_apm/concepts/mapping_functors.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/config/eln_cfg.py` & `pynxtools_apm-0.1.1/pynxtools_apm/config/eln_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         ("shank_angle/@units", "shank_angle/unit"),
     ],
 }
 
 
 APM_INSTRUMENT_STATIC_TO_NEXUS = {
     "prefix_trg": "/ENTRY[entry*]/measurement/instrument",
-    "prefix_src": "atom_probe/",
+    "prefix_src": "instrument/",
     "map": [("analysis_chamber/flight_path", "nominal_flight_path/value")],
     "map_to_str": [
         "status",
         "instrument_name",
         "location",
         ("FABRICATION[fabrication]/vendor", "fabrication_vendor"),
         ("FABRICATION[fabrication]/model", "fabrication_model"),
@@ -101,15 +101,15 @@
         ("analysis_chamber/flight_path/@units", "nominal_flight_path/unit"),
     ],
 }
 
 
 APM_INSTRUMENT_DYNAMIC_TO_NEXUS = {
     "prefix_trg": "/ENTRY[entry*]/measurement/event_data_apm_set/EVENT_DATA_APM[event_data_apm]/instrument",
-    "prefix_src": "atom_probe/",
+    "prefix_src": "instrument/",
     "use": [("control/target_detection_rate/@units", "ions/pulse")],
     "map": [
         ("control/target_detection_rate", "target_detection_rate"),
         ("pulser/pulse_frequency", "pulser/pulse_frequency/value"),
         ("pulser/pulse_fraction", "pulser/pulse_fraction"),
         ("analysis_chamber/chamber_pressure", "chamber_pressure/value"),
         ("stage_lab/base_temperature", "base_temperature/value"),
@@ -176,14 +176,14 @@
     ],
 }
 
 
 APM_IDENTIFIER_TO_NEXUS = {
     "prefix_trg": "/ENTRY[entry*]/USER[user*]",
     "use": [
-        ("IDENTIFIER[identifier]/is_persistent", False),
+        ("IDENTIFIER[identifier]/is_persistent", True),
         ("IDENTIFIER[identifier]/service", "orcid"),
     ],
     "map_to_str": [
         ("IDENTIFIER[identifier]/identifier", "orcid"),
     ],
 }
```

### Comparing `pynxtools_apm-0.1/pynxtools_apm/config/oasis_cfg.py` & `pynxtools_apm-0.1.1/pynxtools_apm/config/oasis_cfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,21 +36,17 @@
 # this is the scenario for which deployment_specific mapping shines
 # parsing of deployment specific details in the apm reader is currently implemented
 # such that it executes after reading generic ELN data (eventually available entries)
 # in the template get overwritten
 
 import datetime as dt
 
-from pynxtools_apm.utils.versioning import NX_APM_ADEF_NAME
-
-
 APM_OASISCONFIG_TO_NEXUS = {
     "prefix_trg": "/ENTRY[entry*]",
     "use": [
-        ("definition", f"{NX_APM_ADEF_NAME}"),
         (
             "start_time",
             f"{dt.datetime.now(dt.timezone.utc).isoformat().replace('+00:00', 'Z')}",
         ),
     ],
     "map_to_str": [("operation_mode")],
 }
```

### Comparing `pynxtools_apm-0.1/pynxtools_apm/reader.py` & `pynxtools_apm-0.1.1/pynxtools_apm/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/create_nx_default_plots.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/create_nx_default_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     # template[f"{trg}@long_name"] = "Discretized reconstruction space"
     template[f"{trg}@signal"] = "intensity"
     col = 0
     dims = ["x", "y", "z"]
     axes = []
     for dim in dims:
         axes.append(f"axis_{dim}")
-        template[f"{trg}@AXISNAME_indices[axis_{dim}]"] = np.uint32(col)
+        template[f"{trg}@AXISNAME_indices[axis_{dim}_indices]"] = np.uint32(col)
         col += 1
     template[f"{trg}@axes"] = axes
 
     # mind that histogram does not follow Cartesian conventions so a transpose
     # might be necessary, for now we implement the transpose in the appdef
     template[f"{trg}intensity"] = {
         "compress": np.asarray(hist3d[0], np.uint32),
@@ -165,15 +165,15 @@
         f"mass_to_charge_distribution/mass_spectrum/"
     )
     template[f"{trg}title"] = (
         f"Mass spectrum ({MASS_SPECTRUM_DEFAULT_BINNING} Da binning)"
     )
     template[f"{trg}@signal"] = "intensity"
     template[f"{trg}@axes"] = "axis_mass_to_charge"
-    template[f"{trg}@AXISNAME_indices[axis_mass_to_charge]"] = np.uint32(0)
+    template[f"{trg}@AXISNAME_indices[axis_mass_to_charge_indices]"] = np.uint32(0)
     template[f"{trg}DATA[intensity]"] = {
         "compress": np.asarray(hist1d[0], np.uint32),
         "strength": 1,
     }
     template[f"{trg}DATA[intensity]/@long_name"] = "Intensity (1)"  # Counts (1)"
     template[f"{trg}AXISNAME[axis_mass_to_charge]"] = {
         "compress": np.asarray(hist1d[1][1::], np.float32),
```

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/generate_synthetic_data.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/generate_synthetic_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,49 +16,42 @@
 # limitations under the License.
 #
 """Utility functions for generation of atom probe NeXus datasets for dev purposes."""
 
 # MK::2023/05/04 the code in this file can currently not be used when
 # developers have an environment which uses ase==3.19.0 and numpy>=1.2x
 
-import hashlib
-
 import datetime
-
+import hashlib
 from typing import List
 
-import numpy as np
-
 import ase
+import numpy as np
+from ase.data import atomic_masses, atomic_numbers, chemical_symbols
 from ase.lattice.cubic import FaceCenteredCubic
-from ase.data import atomic_numbers, atomic_masses, chemical_symbols
-
 from ifes_apt_tc_data_modeling.utils.utils import (
-    create_nuclide_hash,
-    nuclide_hash_to_nuclide_list,
-    nuclide_hash_to_human_readable_name,
     MAX_NUMBER_OF_ATOMS_PER_ION,
     MQ_EPSILON,
+    create_nuclide_hash,
+    nuclide_hash_to_human_readable_name,
+    nuclide_hash_to_nuclide_list,
+)
+
+from pynxtools_apm.utils.load_ranging import (
+    add_unknown_iontype,
 )
 
 # do not use ase directly any longer for NIST isotopes, instead this syntatic equivalent
 # from ifes_apt_tc_data_modeling.utils.nist_isotope_data \
 #     import isotopes
-
 from pynxtools_apm.utils.versioning import (
-    NX_APM_ADEF_NAME,
     NX_APM_EXEC_NAME,
     NX_APM_EXEC_VERSION,
 )
 
-from pynxtools_apm.utils.load_ranging import (
-    add_unknown_iontype,
-)
-
-
 # parameter affecting reconstructed positions and size
 CRYSTAL_ORIENTATION = [[1, 0, 0], [0, 1, 0], [0, 0, 1]]
 # MK::add analysis how large aggregate has to be
 RECON_SIZE = (50, 50, 300)
 RECON_ATOM_SPACING = 5.0
 RECON_HEIGHT = 300.0  # angstroem
 RECON_RADIUS = 50.0  # angstroem
@@ -309,15 +302,14 @@
         return template
 
     def emulate_entry(self, template: dict) -> dict:
         """Copy data in entry section."""
         # check if required fields exists and are valid
         # print("Parsing entry...")
         trg = f"/ENTRY[entry{self.entry_id}]/"
-        template[f"{trg}definition"] = NX_APM_ADEF_NAME
         template[f"{trg}programID[program1]/program"] = NX_APM_EXEC_NAME
         template[f"{trg}programID[program1]/program/@version"] = NX_APM_EXEC_VERSION
         template[f"{trg}start_time"] = datetime.datetime.now().astimezone().isoformat()
         template[f"{trg}end_time"] = datetime.datetime.now().astimezone().isoformat()
         msg = """
               WARNING: These are mocked data !!
               They are meant to be used exclusively
```

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/get_file_checksum.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/get_file_checksum.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/get_gitrepo_commit.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/get_gitrepo_commit.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/interpret_boolean.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/interpret_boolean.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/io_case_logic.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/io_case_logic.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/load_ranging.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/load_ranging.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/load_reconstruction.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/load_reconstruction.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/oasis_config_reader.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/oasis_config_reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/oasis_eln_reader.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/oasis_eln_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,19 +144,19 @@
             APM_INSTRUMENT_DYNAMIC_TO_NEXUS, self.yml, identifier, template
         )
         return template
 
     def parse_pulser_source(self, template: dict) -> dict:
         """Copy data into the (laser)/source section of the pulser."""
         # additional laser-specific details only relevant when the laser was used
-        if "atom_probe/pulser/pulse_mode" in self.yml:
-            if self.yml["atom_probe/pulser/pulse_mode"] == "voltage":
+        if "instrument/pulser/pulse_mode" in self.yml:
+            if self.yml["instrument/pulser/pulse_mode"] == "voltage":
                 return template
 
-        src = "atom_probe/pulser/laser_source"
+        src = "instrument/pulser/laser_source"
         if src in self.yml.keys():
             if isinstance(self.yml[src], list):
                 if all(isinstance(entry, dict) for entry in self.yml[src]) is True:
                     laser_id = 1
                     # custom schema delivers a list of dictionaries...
                     for ldct in self.yml[src]:
                         trg_sta = (
```

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/parse_composition_table.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/parse_composition_table.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/string_conversions.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/string_conversions.py`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pynxtools_apm/utils/versioning.py` & `pynxtools_apm-0.1.1/pynxtools_apm/utils/versioning.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,26 +16,23 @@
 # limitations under the License.
 #
 """Utility tool constants and versioning."""
 
 from pynxtools_apm.utils.get_gitrepo_commit import get_repo_last_commit
 
 
-NX_APM_ADEF_NAME = "NXapm"
-NX_APM_EXEC_NAME = "pynxtools-apm/reader.py"
-
-
 def get_apm_exec_version() -> str:
     tag = get_repo_last_commit()
     if tag is not None:
         return f"https://github.com/FAIRmat-NFDI/pynxtools-apm/commit/{tag}"
     else:
         return (
             f"https://github.com/FAIRmat-NFDI/pynxtools-apm/commit/ UNKNOWN COMMIT !!"
         )
 
 
+NX_APM_EXEC_NAME = "pynxtools-apm/reader.py"
 NX_APM_EXEC_VERSION = get_apm_exec_version()
 
 # numerics
 MASS_SPECTRUM_DEFAULT_BINNING = 0.01  # u
 NAIVE_GRID_DEFAULT_VOXEL_SIZE = 1.0  # nm
```

### Comparing `pynxtools_apm-0.1/pynxtools_apm.egg-info/PKG-INFO` & `pynxtools_apm-0.1.1/pynxtools_apm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools-apm
-Version: 0.1
+Version: 0.1.1
 Summary: Make atom probe tomography and field-ion microscopy results interoperable via NeXus
 Author-email: Markus Kühbach <markus.kuehbach@physik.hu-berlin.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/FAIRmat-NFDI/pynxtools-apm
 Project-URL: Bug Tracker, https://github.com/FAIRmat-NFDI/pynxtools-apm/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,14 +25,17 @@
 Requires-Dist: mkdocs-macros-plugin; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff==0.3.4; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: jupyterlab-h5web; extra == "dev"
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-apm/actions/workflows/pytest.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-apm/actions/workflows/pylint.yml/badge.svg)
 ![](https://github.com/FAIRmat-NFDI/pynxtools-apm/actions/workflows/publish.yml/badge.svg)
 ![](https://img.shields.io/pypi/pyversions/pynxtools-apm)
 ![](https://img.shields.io/pypi/l/pynxtools-apm)
@@ -60,32 +63,31 @@
 
 ## Supported file formats
 This plugin supports the majority of the file formats that are currently used for atom probe.
 A detailed summary is available in the [reference section of the documentation](https://fairmat-nfdi.github.io/pynxtools-apm).
 
 # Getting started
 [A getting started tutorial](https://github.com/FAIRmat-NFDI/pynxtools-apm/tree/main/examples) is offered that guides you
-how to use the apm reader for converting your data to NeXus from a Jupyter notebook. Note that not every combination of
-supported file formats and input for the parser allows to fill required and recommended fields and attributes of the NXapm
-application definition. Therefore, you may need to provide an ELN file that contains the missing values in order for the
+how to use the apm reader for converting your data to NeXus using a Jupyter notebook. That notebook details also the commands how to convert data via command line calls. Note that not every combination of input from a supported file format and other, typically electronic lab notebook, input for the parser allows filling the required and recommended fields and attributes of the NXapm application definition.
+Therefore, you may need to provide an ELN file that contains the missing values in order for the
 validation step of the APM reader to pass.
 
 # Contributing
 We are continously working on adding parsers for other data formats, technology partners, and atom probers.
 If you would like to implement a parser for your data, feel free to get in contact.
 
 ## Development install
 Install the package with its dependencies:
 
 ```shell
 git clone https://github.com/FAIRmat-NFDI/pynxtools-apm.git --branch main --recursive pynxtools_apm
 cd pynxtools_apm
 python -m pip install --upgrade pip
 python -m pip install -e .
-python -m pip install -e ".[dev]"
+python -m pip install -e ".[dev,docs]"
 ```
 
 <!---There is also a [pre-commit hook](https://pre-commit.com/#intro) available
 which formats the code and checks the linting before actually commiting.
 It can be installed with
 ```shell
 pre-commit install
@@ -99,8 +101,8 @@
 [pytest](https://docs.pytest.org/en/stable/) which can be used as follows:
 
 ```shell
 python -m pytest -sv tests
 ```
 
 ## Contact person in FAIRmat for this reader
-Markus Kühbach
+[Markus Kühbach](https://www.fairmat-nfdi.eu/fairmat/about-fairmat/team-fairmat)
```

### Comparing `pynxtools_apm-0.1/pynxtools_apm.egg-info/SOURCES.txt` & `pynxtools_apm-0.1.1/pynxtools_apm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/pyproject.toml` & `pynxtools_apm-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 ]
 dev = [
     "mypy",
     "ruff==0.3.4",
     "pytest",
     "types-pyyaml",
     "pip-tools",
+    "jupyter",
+    "jupyterlab",
+    "jupyterlab-h5web"
 ]
 
 [project.entry-points."pynxtools.reader"]
 apm = "pynxtools_apm.reader:APMReader"
 
 [tool.setuptools_scm]
 version_scheme = "no-guess-dev"
```

### Comparing `pynxtools_apm-0.1/tests/batch_queue.04.sh` & `pynxtools_apm-0.1.1/tests/batch_queue.04.sh`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/tests/data/nomad_oasis_eln_schema_for_nx_apm/nxapm.schema.archive.yaml` & `pynxtools_apm-0.1.1/tests/data/nomad_oasis_eln_schema_for_nx_apm/nxapm.schema.archive.yaml`

 * *Files identical despite different names*

### Comparing `pynxtools_apm-0.1/tests/test_reader.py` & `pynxtools_apm-0.1.1/tests/test_reader.py`

 * *Files identical despite different names*

