# Comparing `tmp/freva-2309.0.1.tar.gz` & `tmp/freva-2309.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva-2309.0.1.tar", last modified: Tue Sep 12 15:51:39 2023, max compression
+gzip compressed data, was "freva-2309.0.2.tar", last modified: Thu Sep 28 12:33:00 2023, max compression
```

## Comparing `freva-2309.0.1.tar` & `freva-2309.0.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.825362 freva-2309.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-09-12 15:51:29.000000 freva-2309.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-09-12 15:51:29.000000 freva-2309.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-09-12 15:51:39.825362 freva-2309.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-09-12 15:51:29.000000 freva-2309.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.805362 freva-2309.0.1/assets/completions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/assets/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/bash/freva
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/assets/completions/fish/
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/fish/freva.fish
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/assets/completions/tcsh/
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/tcsh/tcsh-completion.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/assets/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/_freva
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/_freva_crawl_my_data
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/_freva_databrowser
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/_freva_esgf
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/_freva_history
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/_freva_plugin
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/completions.zsh
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/completions/zsh/source.zsh
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/drs_config.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-09-12 15:51:29.000000 freva-2309.0.1/assets/evaluation_system.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)    15489 2023-09-12 15:51:29.000000 freva-2309.0.1/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 15:51:39.825362 freva-2309.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7204 2023-09-12 15:51:29.000000 freva-2309.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.805362 freva-2309.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/src/evaluation_system/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/src/evaluation_system/api/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36523 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    47785 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47863 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8766 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.809362 freva-2309.0.1/src/evaluation_system/api/workload_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/oar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/api/workload_manager/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.813362 freva-2309.0.1/src/evaluation_system/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/misc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/misc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19287 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/misc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.813362 freva-2309.0.1/src/evaluation_system/model/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14711 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/esgf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21425 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.813362 freva-2309.0.1/src/evaluation_system/model/history/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/history/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.813362 freva-2309.0.1/src/evaluation_system/model/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/plugins/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/solr.py
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/solr_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.813362 freva-2309.0.1/src/evaluation_system/model/solr_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/solr_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/solr_models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/model/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.813362 freva-2309.0.1/src/evaluation_system/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/settings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1023 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/settings/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.817362 freva-2309.0.1/src/evaluation_system/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/cli_argcomplete_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/cli_help_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13879 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13362 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/crawl_my_data_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/databrowser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/db_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/esgf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/history_command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/history_models_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.817362 freva-2309.0.1/src/evaluation_system/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/mocks/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/mocks/dummyfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/mocks/result_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    14770 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/parameters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/plugin_command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13174 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/plugin_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23067 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/solr_core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/solr_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/user_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/user_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.817362 freva-2309.0.1/src/evaluation_system/tests/workload_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_oar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-09-12 15:51:29.000000 freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.817362 freva-2309.0.1/src/freva/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14110 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/_databrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/_esgf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18224 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/_user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.821362 freva-2309.0.1/src/freva/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/databrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/esgf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2023-09-12 15:51:29.000000 freva-2309.0.1/src/freva/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 15:51:39.821362 freva-2309.0.1/src/freva.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-09-12 15:51:39.000000 freva-2309.0.1/src/freva.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-09-12 15:51:39.000000 freva-2309.0.1/src/freva.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 15:51:39.000000 freva-2309.0.1/src/freva.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-09-12 15:51:39.000000 freva-2309.0.1/src/freva.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-12 15:51:39.000000 freva-2309.0.1/src/freva.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 15:51:39.000000 freva-2309.0.1/src/freva.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.673969 freva-2309.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-09-28 12:32:50.000000 freva-2309.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-09-28 12:32:50.000000 freva-2309.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-09-28 12:33:00.673969 freva-2309.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-09-28 12:32:50.000000 freva-2309.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.657969 freva-2309.0.2/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.657969 freva-2309.0.2/assets/completions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.657969 freva-2309.0.2/assets/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/bash/freva
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.657969 freva-2309.0.2/assets/completions/fish/
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/fish/freva.fish
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.661969 freva-2309.0.2/assets/completions/tcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/tcsh/tcsh-completion.bash
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.661969 freva-2309.0.2/assets/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/_freva
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/_freva_crawl_my_data
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/_freva_databrowser
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/_freva_esgf
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/_freva_history
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/_freva_plugin
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/completions.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/completions/zsh/source.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/drs_config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-09-28 12:32:50.000000 freva-2309.0.2/assets/evaluation_system.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15489 2023-09-28 12:32:50.000000 freva-2309.0.2/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 12:33:00.673969 freva-2309.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7204 2023-09-28 12:32:50.000000 freva-2309.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.657969 freva-2309.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.661969 freva-2309.0.2/src/evaluation_system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.661969 freva-2309.0.2/src/evaluation_system/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36523 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47785 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47863 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.661969 freva-2309.0.2/src/evaluation_system/api/workload_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/oar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/api/workload_manager/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.661969 freva-2309.0.2/src/evaluation_system/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/misc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/misc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19287 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/misc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.665969 freva-2309.0.2/src/evaluation_system/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14711 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21425 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.665969 freva-2309.0.2/src/evaluation_system/model/history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/history/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.665969 freva-2309.0.2/src/evaluation_system/model/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/plugins/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/solr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16739 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/solr_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.665969 freva-2309.0.2/src/evaluation_system/model/solr_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/solr_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/solr_models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/model/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.665969 freva-2309.0.2/src/evaluation_system/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/settings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1023 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/settings/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.665969 freva-2309.0.2/src/evaluation_system/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/cli_argcomplete_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/cli_help_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13879 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13362 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/crawl_my_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/databrowser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/esgf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/history_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/history_models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.665969 freva-2309.0.2/src/evaluation_system/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/mocks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/mocks/dummyfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/mocks/result_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14770 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/parameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/plugin_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/plugin_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23067 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/solr_core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/solr_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/user_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/user_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.669969 freva-2309.0.2/src/evaluation_system/tests/workload_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_oar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-09-28 12:32:50.000000 freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.669969 freva-2309.0.2/src/freva/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14110 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/_databrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/_esgf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/_user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.669969 freva-2309.0.2/src/freva/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/databrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2023-09-28 12:32:50.000000 freva-2309.0.2/src/freva/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 12:33:00.669969 freva-2309.0.2/src/freva.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-09-28 12:33:00.000000 freva-2309.0.2/src/freva.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-09-28 12:33:00.000000 freva-2309.0.2/src/freva.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 12:33:00.000000 freva-2309.0.2/src/freva.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-09-28 12:33:00.000000 freva-2309.0.2/src/freva.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-28 12:33:00.000000 freva-2309.0.2/src/freva.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-28 12:33:00.000000 freva-2309.0.2/src/freva.egg-info/top_level.txt
```

### Comparing `freva-2309.0.1/LICENSE.md` & `freva-2309.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/PKG-INFO` & `freva-2309.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva
-Version: 2309.0.1
+Version: 2309.0.2
 Summary: Free Evaluation and Analysis Framework (Freva) 
 Author: German Climate Computing Centre (DKRZ)
 Maintainer: Climate Informatics and Technology (CLINT)
 License: BSD-3-Clause
 Project-URL: Documentation, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/index.html
 Project-URL: Release notes, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/whats-new.html
 Project-URL: Issues, https://gitlab.dkrz.de/freva/evaluation_system/-/issues
```

### Comparing `freva-2309.0.1/README.md` & `freva-2309.0.2/README.md`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/assets/completions/bash/freva` & `freva-2309.0.2/assets/completions/bash/freva`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/assets/completions/fish/freva.fish` & `freva-2309.0.2/assets/completions/fish/freva.fish`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/assets/completions/tcsh/tcsh-completion.bash` & `freva-2309.0.2/assets/completions/tcsh/tcsh-completion.bash`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/assets/completions/zsh/_freva` & `freva-2309.0.2/assets/completions/zsh/_freva`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/assets/completions/zsh/completions.zsh` & `freva-2309.0.2/assets/completions/zsh/completions.zsh`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/assets/drs_config.toml` & `freva-2309.0.2/assets/drs_config.toml`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/assets/evaluation_system.conf` & `freva-2309.0.2/assets/evaluation_system.conf`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/deploy.py` & `freva-2309.0.2/deploy.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/setup.py` & `freva-2309.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/__init__.py` & `freva-2309.0.2/src/evaluation_system/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 import warnings
 
 warnings.filterwarnings(
     "always", category=PendingDeprecationWarning, module="evaluation_system.*"
 )
 
 
-__version__ = "2309.0.1"
+__version__ = "2309.0.2"
```

### Comparing `freva-2309.0.1/src/evaluation_system/api/parameters.py` & `freva-2309.0.2/src/evaluation_system/api/parameters.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/plugin.py` & `freva-2309.0.2/src/evaluation_system/api/plugin.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/plugin_manager.py` & `freva-2309.0.2/src/evaluation_system/api/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/user_data.py` & `freva-2309.0.2/src/evaluation_system/api/user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/__init__.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/core.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/core.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/local.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/local.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/lsf.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/lsf.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/oar.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/oar.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/pbs.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/pbs.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/sge.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/sge.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/api/workload_manager/slurm.py` & `freva-2309.0.2/src/evaluation_system/api/workload_manager/slurm.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/misc/__init__.py` & `freva-2309.0.2/src/evaluation_system/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/misc/config.py` & `freva-2309.0.2/src/evaluation_system/misc/config.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/misc/exceptions.py` & `freva-2309.0.2/src/evaluation_system/misc/exceptions.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/misc/utils.py` & `freva-2309.0.2/src/evaluation_system/misc/utils.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/db.py` & `freva-2309.0.2/src/evaluation_system/model/db.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/esgf.py` & `freva-2309.0.2/src/evaluation_system/model/esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/file.py` & `freva-2309.0.2/src/evaluation_system/model/file.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/history/models.py` & `freva-2309.0.2/src/evaluation_system/model/history/models.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/plugins/models.py` & `freva-2309.0.2/src/evaluation_system/model/plugins/models.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/repository.py` & `freva-2309.0.2/src/evaluation_system/model/repository.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/solr.py` & `freva-2309.0.2/src/evaluation_system/model/solr.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/solr_core.py` & `freva-2309.0.2/src/evaluation_system/model/solr_core.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/solr_models/models.py` & `freva-2309.0.2/src/evaluation_system/model/solr_models/models.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/model/user.py` & `freva-2309.0.2/src/evaluation_system/model/user.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/settings/database.py` & `freva-2309.0.2/src/evaluation_system/settings/database.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/__init__.py` & `freva-2309.0.2/src/evaluation_system/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/cli_argcomplete_test.py` & `freva-2309.0.2/src/evaluation_system/tests/cli_argcomplete_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/cli_help_test.py` & `freva-2309.0.2/src/evaluation_system/tests/cli_help_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/conftest.py` & `freva-2309.0.2/src/evaluation_system/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/crawl_my_data_test.py` & `freva-2309.0.2/src/evaluation_system/tests/crawl_my_data_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/databrowser_test.py` & `freva-2309.0.2/src/evaluation_system/tests/databrowser_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/db_test.py` & `freva-2309.0.2/src/evaluation_system/tests/db_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/esgf_test.py` & `freva-2309.0.2/src/evaluation_system/tests/esgf_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/file_test.py` & `freva-2309.0.2/src/evaluation_system/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/history_command_test.py` & `freva-2309.0.2/src/evaluation_system/tests/history_command_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/history_models_test.py` & `freva-2309.0.2/src/evaluation_system/tests/history_models_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/mocks/__init__.py` & `freva-2309.0.2/src/evaluation_system/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/mocks/dummy.py` & `freva-2309.0.2/src/evaluation_system/tests/mocks/dummy.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/mocks/dummyfolder.py` & `freva-2309.0.2/src/evaluation_system/tests/mocks/dummyfolder.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/mocks/result_tags.py` & `freva-2309.0.2/src/evaluation_system/tests/mocks/result_tags.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/parameters_test.py` & `freva-2309.0.2/src/evaluation_system/tests/parameters_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/plugin_command_test.py` & `freva-2309.0.2/src/evaluation_system/tests/plugin_command_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/plugin_manager_test.py` & `freva-2309.0.2/src/evaluation_system/tests/plugin_manager_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/plugin_test.py` & `freva-2309.0.2/src/evaluation_system/tests/plugin_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/solr_core_test.py` & `freva-2309.0.2/src/evaluation_system/tests/solr_core_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/solr_test.py` & `freva-2309.0.2/src/evaluation_system/tests/solr_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/user_config_test.py` & `freva-2309.0.2/src/evaluation_system/tests/user_config_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/user_test.py` & `freva-2309.0.2/src/evaluation_system/tests/user_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/utils_test.py` & `freva-2309.0.2/src/evaluation_system/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_local.py` & `freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_local.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_lsf.py` & `freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_lsf.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_oar.py` & `freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_oar.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_pbs.py` & `freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_pbs.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_sge.py` & `freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_sge.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/evaluation_system/tests/workload_manager/test_slurm.py` & `freva-2309.0.2/src/evaluation_system/tests/workload_manager/test_slurm.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/__init__.py` & `freva-2309.0.2/src/freva/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/_databrowser.py` & `freva-2309.0.2/src/freva/_databrowser.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/_esgf.py` & `freva-2309.0.2/src/freva/_esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/_history.py` & `freva-2309.0.2/src/freva/_history.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/_plugin.py` & `freva-2309.0.2/src/freva/_plugin.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/_user_data.py` & `freva-2309.0.2/src/freva/_user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/cli/__init__.py` & `freva-2309.0.2/src/freva/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/cli/databrowser.py` & `freva-2309.0.2/src/freva/cli/databrowser.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/cli/esgf.py` & `freva-2309.0.2/src/freva/cli/esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/cli/history.py` & `freva-2309.0.2/src/freva/cli/history.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/cli/plugin.py` & `freva-2309.0.2/src/freva/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/cli/user_data.py` & `freva-2309.0.2/src/freva/cli/user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/cli/utils.py` & `freva-2309.0.2/src/freva/cli/utils.py`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva/utils.py` & `freva-2309.0.2/src/freva/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 from fnmatch import fnmatch
 from functools import wraps
 from pathlib import Path
 from types import TracebackType
 from typing import (
     Any,
+    Dict,
     Callable,
     List,
     Literal,
     Optional,
     Tuple,
     Type,
     Union,
@@ -145,20 +146,20 @@
     def __repr__(self) -> str:
         return (
             f"PluginStatus('{self.plugin}', "
             f"config={str(self.configuration)}, status={self.status})"
         )
 
     @property
-    def _hist(self) -> dict[str, Any]:
+    def _hist(self) -> Dict[str, Any]:
         log_level = logger.level
         logger.setLevel(logging.WARNING)
         try:
             hist = cast(
-                list[dict[str, Any]],
+                List[Dict[str, Any]],
                 freva.history(entry_ids=self._id, return_results=True),
             )[0]
         except IndexError:
             logger.setLevel(log_level)
             return {}
         finally:
             logger.setLevel(log_level)
@@ -170,15 +171,15 @@
         """Get the state of the current plugin run."""
         hist = self._hist
         status_dict = hist.get("status_dict", {})
         status = hist.get("status")
         return cast(str, status_dict.get(status, "unkown"))
 
     @property
-    def configuration(self) -> dict[str, Any]:
+    def configuration(self) -> Dict[str, Any]:
         """Get the plugin configuration."""
         return self._hist.get("configuration", {})
 
     @property
     def stdout(self) -> str:
         """Get the stdout of the plugin.
```

### Comparing `freva-2309.0.1/src/freva.egg-info/PKG-INFO` & `freva-2309.0.2/src/freva.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva
-Version: 2309.0.1
+Version: 2309.0.2
 Summary: Free Evaluation and Analysis Framework (Freva) 
 Author: German Climate Computing Centre (DKRZ)
 Maintainer: Climate Informatics and Technology (CLINT)
 License: BSD-3-Clause
 Project-URL: Documentation, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/index.html
 Project-URL: Release notes, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/whats-new.html
 Project-URL: Issues, https://gitlab.dkrz.de/freva/evaluation_system/-/issues
```

### Comparing `freva-2309.0.1/src/freva.egg-info/SOURCES.txt` & `freva-2309.0.2/src/freva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freva-2309.0.1/src/freva.egg-info/requires.txt` & `freva-2309.0.2/src/freva.egg-info/requires.txt`

 * *Files identical despite different names*

