# Comparing `tmp/cylc_flow-8.2.6.tar.gz` & `tmp/cylc_flow-8.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc_flow-8.2.6.tar", last modified: Thu May  2 11:24:53 2024, max compression
+gzip compressed data, was "cylc_flow-8.2.7.tar", last modified: Wed May 15 14:37:09 2024, max compression
```

## Comparing `cylc_flow-8.2.6.tar` & `cylc_flow-8.2.7.tar`

### file list

```diff
@@ -1,321 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.788079 cylc_flow-8.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-02 11:24:53.788079 cylc_flow-8.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15539 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/async_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/broadcast_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/broadcast_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/c3mro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/cfgspec/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/glbl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    73285 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/globalcfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    85291 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/command_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)    98634 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/context_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/cycling/
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cylc_subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/data_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   103056 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/data_store_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/dbstatecheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/cylc
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/cylc-completion.bash
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/job.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc-mode.el
--rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.lang
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.nanorc
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.vim
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/message-trigger-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/.validate
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.732078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35829 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/flow_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    36301 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/graphnode.py
--rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/host_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/hostuserutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/id.py
--rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/id_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/id_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    21546 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/install_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/install_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/install_plugins/log_vc_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.732078 cylc_flow-8.2.6/cylc/flow/jinja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/jinja/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/jinja/filters/duration_as.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/jinja/filters/pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/jinja/filters/strftime.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/at.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/background.py
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/loadleveler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm_packjob.py
--rw-r--r--   0 runner    (1001) docker     (127)    33926 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/listify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/log_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/loggingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.764078 cylc_flow-8.2.6/cylc/flow/main_loop/
--rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/auto_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_data_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_main_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/reset_bad_hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.764078 cylc_flow-8.2.6/cylc/flow/network/
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/replier.py
--rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    80335 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/ssh_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)    30974 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/option_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/param_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.768079 cylc_flow-8.2.6/cylc/flow/parsec/
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/empysupport.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/fileparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/include.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/jinja2support.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    43559 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/pathutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/pipe_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/prerequisite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/print_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    39982 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/rundb.py
--rw-r--r--   0 runner    (1001) docker     (127)    86354 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20636 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scheduler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15378 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/broadcast.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21078 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/cat_log.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4986 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/check_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2617 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/completion_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8932 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/cycle_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/cylc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5986 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8083 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/dump.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4460 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/ext_trigger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1491 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/function_run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/get_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1871 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2311 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/graph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4638 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10942 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/install.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/jobs_kill.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/jobs_poll.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/jobs_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2503 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/kill.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40024 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/lint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6417 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/pause.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/play.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/reinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3266 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/reload.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/remote_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/remote_tidy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13206 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/report_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/scan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3516 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/set_outputs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/set_verbosity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13108 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/show.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8380 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/stop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3658 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/subscribe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5272 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/tui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6488 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/validate_install_play.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/validate_reinstall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/view.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10163 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/subprocctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    23937 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/subprocpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_action_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    65738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_events_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55839 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_job_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    80634 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_qualifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/task_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_queues/independent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_remote_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_remote_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_state_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/taskdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/templatevars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/tui/
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/unicode_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/wallclock.py
--rw-r--r--   0 runner    (1001) docker     (127)    32499 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_db_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    34487 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtrigger_mgr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/xtriggers/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/echo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/xrandom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.780079 cylc_flow-8.2.6/cylc_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-02 11:24:53.788079 cylc_flow-8.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.676231 cylc_flow-8.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-15 14:37:09.676231 cylc_flow-8.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.616231 cylc_flow-8.2.7/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.640231 cylc_flow-8.2.7/cylc/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15539 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/async_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/broadcast_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/broadcast_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/c3mro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.640231 cylc_flow-8.2.7/cylc/flow/cfgspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cfgspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cfgspec/glbl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73285 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cfgspec/globalcfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85291 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cfgspec/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/command_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98634 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/context_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.640231 cylc_flow-8.2.7/cylc/flow/cycling/
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cycling/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cycling/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cycling/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cycling/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/cylc_subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/data_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103205 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/data_store_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/dbstatecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.640231 cylc_flow-8.2.7/cylc/flow/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/cylc
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/cylc-completion.bash
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/job.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.640231 cylc_flow-8.2.7/cylc/flow/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc-mode.el
+-rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.lang
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.nanorc
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.vim
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.640231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.616231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.620231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/forecast-script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.644231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/inheritance-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.620231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/message-trigger-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/retries-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/retries-tutorial/.validate
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.620231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/runtime
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35829 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/flow_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36301 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/graphnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/hostuserutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/id_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/id_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21546 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.648231 cylc_flow-8.2.7/cylc/flow/install_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/install_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/install_plugins/log_vc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.620231 cylc_flow-8.2.7/cylc/flow/jinja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.652231 cylc_flow-8.2.7/cylc/flow/jinja/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/jinja/filters/duration_as.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/jinja/filters/pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/jinja/filters/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.652231 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/loadleveler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_handlers/slurm_packjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33926 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/job_runner_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/listify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/log_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/loggingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.652231 cylc_flow-8.2.7/cylc/flow/main_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/auto_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/log_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/log_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/log_main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/log_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/main_loop/reset_bad_hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.656231 cylc_flow-8.2.7/cylc/flow/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/replier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80335 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/ssh_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/network/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30949 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/option_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/param_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.656231 cylc_flow-8.2.7/cylc/flow/parsec/
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/empysupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/fileparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/jinja2support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43559 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/parsec/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/pathutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/pipe_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/prerequisite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/print_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39982 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86354 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20636 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scheduler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.664230 cylc_flow-8.2.7/cylc/flow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15378 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/broadcast.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21078 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/cat_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4986 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/check_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2617 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/completion_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8932 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/cycle_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/cylc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5986 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8083 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4460 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/ext_trigger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1491 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/function_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/get_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1871 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/get_workflow_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2311 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/get_workflow_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4638 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10942 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/jobs_kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/jobs_poll.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/jobs_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2503 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40024 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/lint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6417 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/pause.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/play.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/reinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3266 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/remote_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/remote_tidy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13206 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/report_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3516 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/set_outputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/set_verbosity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13108 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/show.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8380 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/stop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3658 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/subscribe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5272 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/tui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6488 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/validate_install_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/validate_reinstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/view.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10163 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/scripts/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/subprocctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23937 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/subprocpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_action_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65738 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_events_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55839 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_job_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80634 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_qualifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.668231 cylc_flow-8.2.7/cylc/flow/task_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_queues/independent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_remote_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_remote_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_state_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/task_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/taskdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/templatevars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.668231 cylc_flow-8.2.7/cylc/flow/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/tui/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/tui/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/tui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/unicode_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/wallclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32499 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/workflow_db_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/workflow_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34487 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/workflow_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/workflow_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/xtrigger_mgr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.668231 cylc_flow-8.2.7/cylc/flow/xtriggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/xtriggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/xtriggers/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/xtriggers/wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/xtriggers/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/cylc/flow/xtriggers/xrandom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:09.668231 cylc_flow-8.2.7/cylc_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-15 14:37:09.000000 cylc_flow-8.2.7/cylc_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-15 14:37:09.000000 cylc_flow-8.2.7/cylc_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:37:09.000000 cylc_flow-8.2.7/cylc_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-15 14:37:09.000000 cylc_flow-8.2.7/cylc_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-15 14:37:09.000000 cylc_flow-8.2.7/cylc_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 14:37:09.000000 cylc_flow-8.2.7/cylc_flow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-15 14:37:09.676231 cylc_flow-8.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-15 14:37:05.000000 cylc_flow-8.2.7/setup.py
```

### Comparing `cylc_flow-8.2.6/COPYING` & `cylc_flow-8.2.7/COPYING`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/PKG-INFO` & `cylc_flow-8.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.2.6
+Version: 8.2.7
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
```

### Comparing `cylc_flow-8.2.6/README.md` & `cylc_flow-8.2.7/README.md`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/__init__.py` & `cylc_flow-8.2.7/cylc/flow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # running pre-5.0 cylc via the posix nohup command; is it still the
     # case in post-5.0 daemon-mode cylc?)
     os.environ['PYTHONUNBUFFERED'] = 'true'
 
 
 environ_init()
 
-__version__ = '8.2.6'
+__version__ = '8.2.7'
 
 
 def iter_entry_points(entry_point_name):
     """Iterate over Cylc entry points."""
     import pkg_resources
     yield from (
         entry_point
```

### Comparing `cylc_flow-8.2.6/cylc/flow/async_util.py` & `cylc_flow-8.2.7/cylc/flow/async_util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/broadcast_mgr.py` & `cylc_flow-8.2.7/cylc/flow/broadcast_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/broadcast_report.py` & `cylc_flow-8.2.7/cylc/flow/broadcast_report.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/c3mro.py` & `cylc_flow-8.2.7/cylc/flow/c3mro.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cfgspec/__init__.py` & `cylc_flow-8.2.7/cylc/flow/cfgspec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cfgspec/glbl_cfg.py` & `cylc_flow-8.2.7/cylc/flow/cfgspec/glbl_cfg.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cfgspec/globalcfg.py` & `cylc_flow-8.2.7/cylc/flow/cfgspec/globalcfg.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cfgspec/workflow.py` & `cylc_flow-8.2.7/cylc/flow/cfgspec/workflow.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/clean.py` & `cylc_flow-8.2.7/cylc/flow/clean.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/command_polling.py` & `cylc_flow-8.2.7/cylc/flow/command_polling.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/config.py` & `cylc_flow-8.2.7/cylc/flow/config.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/context_node.py` & `cylc_flow-8.2.7/cylc/flow/context_node.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cycling/__init__.py` & `cylc_flow-8.2.7/cylc/flow/cycling/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cycling/integer.py` & `cylc_flow-8.2.7/cylc/flow/cycling/integer.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cycling/iso8601.py` & `cylc_flow-8.2.7/cylc/flow/cycling/iso8601.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cycling/loader.py` & `cylc_flow-8.2.7/cylc/flow/cycling/loader.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cycling/util.py` & `cylc_flow-8.2.7/cylc/flow/cycling/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/cylc_subproc.py` & `cylc_flow-8.2.7/cylc/flow/cylc_subproc.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/daemonize.py` & `cylc_flow-8.2.7/cylc/flow/daemonize.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/data_messages_pb2.py` & `cylc_flow-8.2.7/cylc/flow/data_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/data_store_mgr.py` & `cylc_flow-8.2.7/cylc/flow/data_store_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1968,18 +1968,20 @@
             if tp_id in tp_updated:
                 if tp_id in tp_data:
                     node = tp_data[tp_id]
                 elif tp_id in tp_added:
                     node = tp_added[tp_id]
                 else:
                     continue
-                for j_id in list(node.jobs) + list(tp_updated[tp_id].jobs):
+                update_node = tp_updated.pop(tp_id)
+                for j_id in list(node.jobs) + list(update_node.jobs):
                     if j_id in j_updated:
                         del j_updated[j_id]
-                del tp_updated[tp_id]
+                self.n_window_edges.difference_update(update_node.edges)
+                self.deltas[EDGES].pruned.extend(update_node.edges)
         self.pruned_task_proxies.clear()
 
     def update_family_proxies(self):
         """Update state & summary of flagged families and ancestors.
 
         Tasks whose state are updated flag their first parent, as a family
         to be updated, by adding their ID to a set.
```

### Comparing `cylc_flow-8.2.6/cylc/flow/dbstatecheck.py` & `cylc_flow-8.2.7/cylc/flow/dbstatecheck.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/cylc` & `cylc_flow-8.2.7/cylc/flow/etc/cylc`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/cylc-completion.bash` & `cylc_flow-8.2.7/cylc/flow/etc/cylc-completion.bash`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/job.sh` & `cylc_flow-8.2.7/cylc/flow/etc/job.sh`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc-mode.el` & `cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc-mode.el`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.lang` & `cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.lang`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.nanorc` & `cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.nanorc`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.vim` & `cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.vim`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.xml` & `cylc_flow-8.2.7/cylc/flow/etc/syntax/cylc.xml`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/.validate` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/forecast` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/forecast-script/forecast`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/util.py` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/forecast-script/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/map-template/map-template.html` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/map-template/map-template.html`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/.validate` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/retries-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/.validate` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/.validate`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/runtime` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/runtime-tutorial/runtime`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/rainfall.csv` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `cylc_flow-8.2.7/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/exceptions.py` & `cylc_flow-8.2.7/cylc/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/flags.py` & `cylc_flow-8.2.7/cylc/flow/flags.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/flow_mgr.py` & `cylc_flow-8.2.7/cylc/flow/flow_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/graph_parser.py` & `cylc_flow-8.2.7/cylc/flow/graph_parser.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/graphnode.py` & `cylc_flow-8.2.7/cylc/flow/graphnode.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/host_select.py` & `cylc_flow-8.2.7/cylc/flow/host_select.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/hostuserutil.py` & `cylc_flow-8.2.7/cylc/flow/hostuserutil.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/id.py` & `cylc_flow-8.2.7/cylc/flow/id.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/id_cli.py` & `cylc_flow-8.2.7/cylc/flow/id_cli.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/id_match.py` & `cylc_flow-8.2.7/cylc/flow/id_match.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/install.py` & `cylc_flow-8.2.7/cylc/flow/install.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/install_plugins/__init__.py` & `cylc_flow-8.2.7/cylc/flow/install_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/install_plugins/log_vc_info.py` & `cylc_flow-8.2.7/cylc/flow/install_plugins/log_vc_info.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/jinja/filters/duration_as.py` & `cylc_flow-8.2.7/cylc/flow/jinja/filters/duration_as.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/jinja/filters/pad.py` & `cylc_flow-8.2.7/cylc/flow/jinja/filters/pad.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/jinja/filters/strftime.py` & `cylc_flow-8.2.7/cylc/flow/jinja/filters/strftime.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_file.py` & `cylc_flow-8.2.7/cylc/flow/job_file.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/__init__.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/at.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/at.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/background.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/background.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/documentation.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/documentation.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/loadleveler.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/loadleveler.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/lsf.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/lsf.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/moab.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/moab.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/pbs.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs_multi_cluster.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/pbs_multi_cluster.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/sge.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/sge.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/slurm.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm_packjob.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_handlers/slurm_packjob.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/job_runner_mgr.py` & `cylc_flow-8.2.7/cylc/flow/job_runner_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/listify.py` & `cylc_flow-8.2.7/cylc/flow/listify.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/log_diagnosis.py` & `cylc_flow-8.2.7/cylc/flow/log_diagnosis.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/loggingutil.py` & `cylc_flow-8.2.7/cylc/flow/loggingutil.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/__init__.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/auto_restart.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/auto_restart.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/health_check.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/health_check.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/log_data_store.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/log_data_store.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/log_db.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/log_db.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/log_main_loop.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/log_main_loop.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/log_memory.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/log_memory.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/main_loop/reset_bad_hosts.py` & `cylc_flow-8.2.7/cylc/flow/main_loop/reset_bad_hosts.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/__init__.py` & `cylc_flow-8.2.7/cylc/flow/network/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/authentication.py` & `cylc_flow-8.2.7/cylc/flow/network/authentication.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/authorisation.py` & `cylc_flow-8.2.7/cylc/flow/network/authorisation.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/client.py` & `cylc_flow-8.2.7/cylc/flow/network/client.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/client_factory.py` & `cylc_flow-8.2.7/cylc/flow/network/client_factory.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/graphql.py` & `cylc_flow-8.2.7/cylc/flow/network/graphql.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/multi.py` & `cylc_flow-8.2.7/cylc/flow/network/multi.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/publisher.py` & `cylc_flow-8.2.7/cylc/flow/network/publisher.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/replier.py` & `cylc_flow-8.2.7/cylc/flow/network/replier.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/resolvers.py` & `cylc_flow-8.2.7/cylc/flow/network/resolvers.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/scan.py` & `cylc_flow-8.2.7/cylc/flow/network/scan.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/schema.py` & `cylc_flow-8.2.7/cylc/flow/network/schema.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/server.py` & `cylc_flow-8.2.7/cylc/flow/network/server.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/ssh_client.py` & `cylc_flow-8.2.7/cylc/flow/network/ssh_client.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/network/subscriber.py` & `cylc_flow-8.2.7/cylc/flow/network/subscriber.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/option_parsers.py` & `cylc_flow-8.2.7/cylc/flow/option_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from ansimarkup import (
     parse as cparse,
     strip as cstrip
 )
 
 import sys
 from textwrap import dedent
-from typing import Any, Dict, Iterable, Optional, List, Tuple, Union
+from typing import Any, Dict, Iterable, Optional, List, Set, Tuple, Union
 
 from cylc.flow import LOG
 from cylc.flow.terminal import supports_color, DIM
 import cylc.flow.flags
 from cylc.flow.loggingutil import (
     CylcLogFormatter,
     setup_segregated_log_streams,
@@ -58,30 +58,33 @@
 
     Despite some similarities this is not to be confused with
     optparse.Option: This a container for information which may or may
     not be passed to optparse depending on the results of
     cylc.flow.option_parsers(thismodule).combine_options_pair.
     """
 
-    def __init__(self, argslist, sources=None, useif=None, **kwargs):
+    def __init__(
+        self,
+        argslist: List[str],
+        sources: Optional[Set[str]] = None,
+        useif: str = '',
+        **kwargs
+    ):
         """Init function:
 
         Args:
             arglist: list of arguments for optparse.Option.
             sources: set of CLI scripts which use this option.
             useif: badge for use by Cylc optionparser.
             **kwargs: kwargs for optparse.option.
         """
-        self.kwargs: Dict[str, str] = {}
-        self.sources: set = sources if sources is not None else set()
-        self.useif: str = useif if useif is not None else ''
-
-        self.args: list[str] = argslist
-        for kwarg, value in kwargs.items():
-            self.kwargs.update({kwarg: value})
+        self.args: List[str] = argslist
+        self.kwargs: Dict[str, Any] = kwargs
+        self.sources: Set[str] = sources if sources is not None else set()
+        self.useif: str = useif
 
     def __eq__(self, other):
         """Args and Kwargs, but not other props equal.
 
         (Also make an exception for kwargs['help'] to allow lists of sources
         prepended to 'help' to be passed through.)
         """
@@ -858,15 +861,15 @@
         x.kwargs.get('dest', x.args[0].strip(DOUBLEDASH)): x
         for x in compound_script_opts
     }
 
     # Get a list of unwanted args:
     unwanted_compound: List[str] = []
     unwanted_simple: List[str] = []
-    for unwanted_dest in (set(options.__dict__)) - set(script_opts_by_dest):
+    for unwanted_dest in set(options.__dict__) - set(script_opts_by_dest):
         for unwanted_arg in compound_opts_by_dest[unwanted_dest].args:
             if (
                 compound_opts_by_dest[unwanted_dest].kwargs.get('action', None)
                 in ['store_true', 'store_false']
             ):
                 unwanted_simple.append(unwanted_arg)
             else:
```

### Comparing `cylc_flow-8.2.6/cylc/flow/param_expand.py` & `cylc_flow-8.2.7/cylc/flow/param_expand.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/OrderedDict.py` & `cylc_flow-8.2.7/cylc/flow/parsec/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/__init__.py` & `cylc_flow-8.2.7/cylc/flow/parsec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/config.py` & `cylc_flow-8.2.7/cylc/flow/parsec/config.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/empysupport.py` & `cylc_flow-8.2.7/cylc/flow/parsec/empysupport.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/exceptions.py` & `cylc_flow-8.2.7/cylc/flow/parsec/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/fileparse.py` & `cylc_flow-8.2.7/cylc/flow/parsec/fileparse.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/include.py` & `cylc_flow-8.2.7/cylc/flow/parsec/include.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/jinja2support.py` & `cylc_flow-8.2.7/cylc/flow/parsec/jinja2support.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/upgrade.py` & `cylc_flow-8.2.7/cylc/flow/parsec/upgrade.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/util.py` & `cylc_flow-8.2.7/cylc/flow/parsec/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/parsec/validate.py` & `cylc_flow-8.2.7/cylc/flow/parsec/validate.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/pathutil.py` & `cylc_flow-8.2.7/cylc/flow/pathutil.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/pipe_poller.py` & `cylc_flow-8.2.7/cylc/flow/pipe_poller.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/platforms.py` & `cylc_flow-8.2.7/cylc/flow/platforms.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/prerequisite.py` & `cylc_flow-8.2.7/cylc/flow/prerequisite.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/print_tree.py` & `cylc_flow-8.2.7/cylc/flow/print_tree.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/profiler.py` & `cylc_flow-8.2.7/cylc/flow/profiler.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/remote.py` & `cylc_flow-8.2.7/cylc/flow/remote.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/resources.py` & `cylc_flow-8.2.7/cylc/flow/resources.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/rundb.py` & `cylc_flow-8.2.7/cylc/flow/rundb.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scheduler.py` & `cylc_flow-8.2.7/cylc/flow/scheduler.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scheduler_cli.py` & `cylc_flow-8.2.7/cylc/flow/scheduler_cli.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/__init__.py` & `cylc_flow-8.2.7/cylc/flow/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/broadcast.py` & `cylc_flow-8.2.7/cylc/flow/scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/cat_log.py` & `cylc_flow-8.2.7/cylc/flow/scripts/cat_log.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/check_versions.py` & `cylc_flow-8.2.7/cylc/flow/scripts/check_versions.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/clean.py` & `cylc_flow-8.2.7/cylc/flow/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/client.py` & `cylc_flow-8.2.7/cylc/flow/scripts/client.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/common.py` & `cylc_flow-8.2.7/cylc/flow/scripts/common.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/completion_server.py` & `cylc_flow-8.2.7/cylc/flow/scripts/completion_server.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/config.py` & `cylc_flow-8.2.7/cylc/flow/scripts/config.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/cycle_point.py` & `cylc_flow-8.2.7/cylc/flow/scripts/cycle_point.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/cylc.py` & `cylc_flow-8.2.7/cylc/flow/scripts/cylc.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/diff.py` & `cylc_flow-8.2.7/cylc/flow/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/dump.py` & `cylc_flow-8.2.7/cylc/flow/scripts/dump.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/ext_trigger.py` & `cylc_flow-8.2.7/cylc/flow/scripts/ext_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/function_run.py` & `cylc_flow-8.2.7/cylc/flow/scripts/function_run.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/get_resources.py` & `cylc_flow-8.2.7/cylc/flow/scripts/get_resources.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_contact.py` & `cylc_flow-8.2.7/cylc/flow/scripts/get_workflow_contact.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_version.py` & `cylc_flow-8.2.7/cylc/flow/scripts/get_workflow_version.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/graph.py` & `cylc_flow-8.2.7/cylc/flow/scripts/graph.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/hold.py` & `cylc_flow-8.2.7/cylc/flow/scripts/hold.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/install.py` & `cylc_flow-8.2.7/cylc/flow/scripts/install.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/jobs_kill.py` & `cylc_flow-8.2.7/cylc/flow/scripts/jobs_kill.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/jobs_poll.py` & `cylc_flow-8.2.7/cylc/flow/scripts/jobs_poll.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/jobs_submit.py` & `cylc_flow-8.2.7/cylc/flow/scripts/jobs_submit.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/kill.py` & `cylc_flow-8.2.7/cylc/flow/scripts/kill.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/lint.py` & `cylc_flow-8.2.7/cylc/flow/scripts/lint.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/list.py` & `cylc_flow-8.2.7/cylc/flow/scripts/list.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/message.py` & `cylc_flow-8.2.7/cylc/flow/scripts/message.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/pause.py` & `cylc_flow-8.2.7/cylc/flow/scripts/pause.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/ping.py` & `cylc_flow-8.2.7/cylc/flow/scripts/ping.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/play.py` & `cylc_flow-8.2.7/cylc/flow/scripts/play.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/poll.py` & `cylc_flow-8.2.7/cylc/flow/scripts/poll.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/psutil.py` & `cylc_flow-8.2.7/cylc/flow/scripts/psutil.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/reinstall.py` & `cylc_flow-8.2.7/cylc/flow/scripts/reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/release.py` & `cylc_flow-8.2.7/cylc/flow/scripts/release.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/reload.py` & `cylc_flow-8.2.7/cylc/flow/scripts/reload.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/remote_init.py` & `cylc_flow-8.2.7/cylc/flow/scripts/remote_init.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/remote_tidy.py` & `cylc_flow-8.2.7/cylc/flow/scripts/remote_tidy.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/remove.py` & `cylc_flow-8.2.7/cylc/flow/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/report_timings.py` & `cylc_flow-8.2.7/cylc/flow/scripts/report_timings.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/scan.py` & `cylc_flow-8.2.7/cylc/flow/scripts/scan.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/set_outputs.py` & `cylc_flow-8.2.7/cylc/flow/scripts/set_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/set_verbosity.py` & `cylc_flow-8.2.7/cylc/flow/scripts/set_verbosity.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/show.py` & `cylc_flow-8.2.7/cylc/flow/scripts/show.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/stop.py` & `cylc_flow-8.2.7/cylc/flow/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/subscribe.py` & `cylc_flow-8.2.7/cylc/flow/scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/trigger.py` & `cylc_flow-8.2.7/cylc/flow/scripts/trigger.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/tui.py` & `cylc_flow-8.2.7/cylc/flow/scripts/tui.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/validate.py` & `cylc_flow-8.2.7/cylc/flow/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/validate_install_play.py` & `cylc_flow-8.2.7/cylc/flow/scripts/validate_install_play.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,14 @@
     _, workflow_id = cylc_install(options, workflow_id)
 
     cleanup_sysargv(
         'play',
         workflow_id,
         options,
         compound_script_opts=VIP_OPTIONS,
-        script_opts=(
-            PLAY_OPTIONS + CYLC_ROSE_OPTIONS
-            + parser.get_std_options()
-        ),
+        script_opts=(*PLAY_OPTIONS, *parser.get_std_options()),
         source=orig_source,
     )
 
     set_timestamps(LOG, options.log_timestamp)
     log_subcommand(*sys.argv[1:])
     _play(parser, options, workflow_id)
```

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/validate_reinstall.py` & `cylc_flow-8.2.7/cylc/flow/scripts/validate_reinstall.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,12 @@
     else:
         set_timestamps(LOG, options.log_timestamp)
         cleanup_sysargv(
             'play',
             unparsed_wid,
             options,
             compound_script_opts=VR_OPTIONS,
-            script_opts=(
-                PLAY_OPTIONS + CYLC_ROSE_OPTIONS
-                + parser.get_std_options()
-            ),
+            script_opts=(*PLAY_OPTIONS, *parser.get_std_options()),
             source='',  # Intentionally blank
         )
         log_subcommand(*sys.argv[1:])
         scheduler_cli(options, workflow_id)
```

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/view.py` & `cylc_flow-8.2.7/cylc/flow/scripts/view.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/scripts/workflow_state.py` & `cylc_flow-8.2.7/cylc/flow/scripts/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/subprocctx.py` & `cylc_flow-8.2.7/cylc/flow/subprocctx.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/subprocpool.py` & `cylc_flow-8.2.7/cylc/flow/subprocpool.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_action_timer.py` & `cylc_flow-8.2.7/cylc/flow/task_action_timer.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_events_mgr.py` & `cylc_flow-8.2.7/cylc/flow/task_events_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_id.py` & `cylc_flow-8.2.7/cylc/flow/task_id.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_job_logs.py` & `cylc_flow-8.2.7/cylc/flow/task_job_logs.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_job_mgr.py` & `cylc_flow-8.2.7/cylc/flow/task_job_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_message.py` & `cylc_flow-8.2.7/cylc/flow/task_message.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_outputs.py` & `cylc_flow-8.2.7/cylc/flow/task_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_pool.py` & `cylc_flow-8.2.7/cylc/flow/task_pool.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_proxy.py` & `cylc_flow-8.2.7/cylc/flow/task_proxy.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_qualifiers.py` & `cylc_flow-8.2.7/cylc/flow/task_qualifiers.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_queues/__init__.py` & `cylc_flow-8.2.7/cylc/flow/task_queues/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_queues/independent.py` & `cylc_flow-8.2.7/cylc/flow/task_queues/independent.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_remote_cmd.py` & `cylc_flow-8.2.7/cylc/flow/task_remote_cmd.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_remote_mgr.py` & `cylc_flow-8.2.7/cylc/flow/task_remote_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_state.py` & `cylc_flow-8.2.7/cylc/flow/task_state.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_state_prop.py` & `cylc_flow-8.2.7/cylc/flow/task_state_prop.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/task_trigger.py` & `cylc_flow-8.2.7/cylc/flow/task_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/taskdef.py` & `cylc_flow-8.2.7/cylc/flow/taskdef.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/templatevars.py` & `cylc_flow-8.2.7/cylc/flow/templatevars.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/terminal.py` & `cylc_flow-8.2.7/cylc/flow/terminal.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/time_parser.py` & `cylc_flow-8.2.7/cylc/flow/time_parser.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/timer.py` & `cylc_flow-8.2.7/cylc/flow/timer.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/tui/__init__.py` & `cylc_flow-8.2.7/cylc/flow/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/tui/app.py` & `cylc_flow-8.2.7/cylc/flow/tui/app.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/tui/data.py` & `cylc_flow-8.2.7/cylc/flow/tui/data.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/tui/overlay.py` & `cylc_flow-8.2.7/cylc/flow/tui/overlay.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/tui/tree.py` & `cylc_flow-8.2.7/cylc/flow/tui/tree.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/tui/util.py` & `cylc_flow-8.2.7/cylc/flow/tui/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/unicode_rules.py` & `cylc_flow-8.2.7/cylc/flow/unicode_rules.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/util.py` & `cylc_flow-8.2.7/cylc/flow/util.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/wallclock.py` & `cylc_flow-8.2.7/cylc/flow/wallclock.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/workflow_db_mgr.py` & `cylc_flow-8.2.7/cylc/flow/workflow_db_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/workflow_events.py` & `cylc_flow-8.2.7/cylc/flow/workflow_events.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/workflow_files.py` & `cylc_flow-8.2.7/cylc/flow/workflow_files.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/workflow_status.py` & `cylc_flow-8.2.7/cylc/flow/workflow_status.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/xtrigger_mgr.py` & `cylc_flow-8.2.7/cylc/flow/xtrigger_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/xtriggers/__init__.py` & `cylc_flow-8.2.7/cylc/flow/xtriggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/xtriggers/echo.py` & `cylc_flow-8.2.7/cylc/flow/xtriggers/echo.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/xtriggers/wall_clock.py` & `cylc_flow-8.2.7/cylc/flow/xtriggers/wall_clock.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/xtriggers/workflow_state.py` & `cylc_flow-8.2.7/cylc/flow/xtriggers/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc/flow/xtriggers/xrandom.py` & `cylc_flow-8.2.7/cylc/flow/xtriggers/xrandom.py`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc_flow.egg-info/PKG-INFO` & `cylc_flow-8.2.7/cylc_flow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.2.6
+Version: 8.2.7
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
```

### Comparing `cylc_flow-8.2.6/cylc_flow.egg-info/SOURCES.txt` & `cylc_flow-8.2.7/cylc_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc_flow.egg-info/entry_points.txt` & `cylc_flow-8.2.7/cylc_flow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/cylc_flow.egg-info/requires.txt` & `cylc_flow-8.2.7/cylc_flow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/pyproject.toml` & `cylc_flow-8.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/setup.cfg` & `cylc_flow-8.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `cylc_flow-8.2.6/setup.py` & `cylc_flow-8.2.7/setup.py`

 * *Files identical despite different names*

