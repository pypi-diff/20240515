# Comparing `tmp/agentMET4FOF-0.8.1.tar.gz` & `tmp/agentMET4FOF-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentMET4FOF-0.8.1.tar", last modified: Thu Jun 10 10:23:25 2021, max compression
+gzip compressed data, was "agentMET4FOF-0.9.0.tar", last modified: Thu Jul  8 13:46:27 2021, max compression
```

## Comparing `agentMET4FOF-0.8.1.tar` & `agentMET4FOF-0.9.0.tar`

### file list

```diff
@@ -1,114 +1,144 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.837016 agentMET4FOF-0.8.1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.821016 agentMET4FOF-0.8.1/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10400 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/.coveragerc
--rw-r--r--   0 circleci  (3434) circleci  (3434)      379 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      555 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/.readthedocs.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5462 2021-06-10 10:23:20.000000 agentMET4FOF-0.8.1/CHANGELOG.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11614 2021-06-10 10:23:25.837016 agentMET4FOF-0.8.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8655 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.821016 agentMET4FOF-0.8.1/agentMET4FOF/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2021-06-10 10:23:20.000000 agentMET4FOF-0.8.1/agentMET4FOF/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    80250 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/agents.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.821016 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10572 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2060 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard_Control.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35125 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard_agt_net.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1438 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard_layout_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5516 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/LayoutHelper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.821016 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/assets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2251 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/assets/render_mpld3.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/assets/stylesheet.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/dashboard/default_network_stylesheet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12842 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/metrological_agents.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13689 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/metrological_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17160 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF/streams.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.821016 agentMET4FOF-0.8.1/agentMET4FOF.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11614 2021-06-10 10:23:25.000000 agentMET4FOF-0.8.1/agentMET4FOF.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3668 2021-06-10 10:23:25.000000 agentMET4FOF-0.8.1/agentMET4FOF.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-06-10 10:23:25.000000 agentMET4FOF-0.8.1/agentMET4FOF.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2021-06-10 10:23:25.000000 agentMET4FOF-0.8.1/agentMET4FOF.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       36 2021-06-10 10:23:25.000000 agentMET4FOF-0.8.1/agentMET4FOF.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.825016 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.825016 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/agent_module/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/agent_module/ui_main_example.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/agent_module/ui_module_example.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.825016 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/buffering/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4148 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/buffering/basic_buffering.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3914 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/buffering/metrological_buffering.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3932 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/buffering/moving_average.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.825016 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/datastreams/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2415 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/datastreams/gaussianshock_generator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4840 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/datastreams/multi_generator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2730 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/datastreams/simple_generator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.825016 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3919 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/basic_memory_plot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3560 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/basic_send_plot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2679 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/custom_memory_multiple_plot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2978 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/custom_memory_plot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3507 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/list_of_plots.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12416 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_1_generator_agent.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1851 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_1_generator_agent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11361 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_2_math_agent.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2032 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_2_math_agent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12255 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_3_multi_channel.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2461 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_3_multi_channel.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12216 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_4_metrological_streams.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2515 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_4_metrological_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15107 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_5_coalition.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1006 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_5_coalition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4124 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_6_mesa_backend.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)      682 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_6_mesa_backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    32218 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2374 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      152 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/dev-requirements.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6023 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/dev-requirements.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.837016 agentMET4FOF-0.8.1/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10377 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/CONTRIBUTING.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2951 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/INSTALL.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)  2375645 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/Pandas-intersphinx-mappings-objects.inv
--rw-r--r--   0 circleci  (3434) circleci  (3434)   998341 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/PyDynamic-intersphinx-mappings-objects.inv
--rw-r--r--   0 circleci  (3434) circleci  (3434)   965388 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/SciPy-intersphinx-mappings-objects.inv
--rw-r--r--   0 circleci  (3434) circleci  (3434)    59325 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/UML_agentMET4FOF_classes_only.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34207 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/UML_agents_full.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)   140724 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/UML_dashboard_full.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)   488641 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/UML_metrological_agents_full.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)   169510 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/UML_metrological_streams_full.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)   129661 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/UML_streams_full.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1311 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/UMLs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       91 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/agentMET4FOF_agents.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/agentMET4FOF_dashboard.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      172 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/agentMET4FOF_metrological_agents.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      175 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/agentMET4FOF_metrological_streams.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      116 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/agentMET4FOF_streams.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14175 2021-06-10 10:23:20.000000 agentMET4FOF-0.8.1/docs/conf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1369 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/index.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25487 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/matplotlib3.3_pytest_error_log
--rw-r--r--   0 circleci  (3434) circleci  (3434)   791798 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/numpy-intersphinx-mappings.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)  2374912 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/pandas-intersphinx-mappings.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)  1213296 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/python-intersphinx-mappings-objects.inv
--rw-r--r--   0 circleci  (3434) circleci  (3434)   161853 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/screenshot_met4fof.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/sphinx-requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1313 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/time-series-buffer-intersphinx-mappings.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1581 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/docs/time-series-metadata-intersphinx-mappings-objects.inv
--rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/environment.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7561 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/license.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2903 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      527 2021-06-10 10:23:25.837016 agentMET4FOF-0.8.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:23:25.837016 agentMET4FOF-0.8.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      564 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3334 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_addremove_metrological_agents.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      728 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_all_imports.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1136 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_dashboard.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6230 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_memory_monitor_agent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4143 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_metadata_metrological_agent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_network.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1648 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_remove_agent.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1622 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_send_plot_image.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1623 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_send_plot_plotly.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1459 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tests/test_tutorials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2021-06-10 10:22:33.000000 agentMET4FOF-0.8.1/tox.ini
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.698446 agentMET4FOF-0.9.0/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.670445 agentMET4FOF-0.9.0/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10400 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/.coveragerc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      379 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      555 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/.readthedocs.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12228 2021-07-08 13:46:22.000000 agentMET4FOF-0.9.0/CHANGELOG.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11614 2021-07-08 13:46:27.698446 agentMET4FOF-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8655 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.670445 agentMET4FOF-0.9.0/agentMET4FOF/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2021-07-08 13:46:22.000000 agentMET4FOF-0.9.0/agentMET4FOF/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF/agents/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      675 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/agents/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37619 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/agents/base_agents.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7318 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/agents/metrological_base_agents.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    44456 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/agents/metrological_redundancy_agents.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1733 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/agents/metrological_signal_agents.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1538 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/agents/signal_agents.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10572 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2060 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard_Control.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35125 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard_agt_net.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1438 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard_layout_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5516 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/LayoutHelper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/assets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2251 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/assets/render_mpld3.js
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      220 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/assets/stylesheet.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/dashboard/default_network_stylesheet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      386 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF/metrological_agents/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1049 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/metrological_agents/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF/metrological_streams/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1128 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/metrological_streams/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33035 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/network.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF/streams/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      963 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/streams/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14455 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/streams/base_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8106 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/streams/metrological_base_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6235 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/streams/metrological_signal_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3414 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/streams/signal_streams.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      199 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/utils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17252 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF/utils/buffer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.674445 agentMET4FOF-0.9.0/agentMET4FOF.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11614 2021-07-08 13:46:27.000000 agentMET4FOF-0.9.0/agentMET4FOF.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4744 2021-07-08 13:46:27.000000 agentMET4FOF-0.9.0/agentMET4FOF.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-07-08 13:46:27.000000 agentMET4FOF-0.9.0/agentMET4FOF.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2021-07-08 13:46:27.000000 agentMET4FOF-0.9.0/agentMET4FOF.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       36 2021-07-08 13:46:27.000000 agentMET4FOF-0.9.0/agentMET4FOF.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.678445 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.678445 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/agent_module/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/agent_module/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/agent_module/ui_main_example.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1450 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/agent_module/ui_module_example.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.678445 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4148 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/basic_buffering.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3914 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/metrological_buffering.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3932 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/moving_average.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.678445 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2415 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/gaussianshock_generator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4816 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/multi_generator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2840 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/simple_generator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.678445 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3919 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/basic_memory_plot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3560 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/basic_send_plot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2679 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/custom_memory_multiple_plot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2978 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/custom_memory_plot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3507 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/list_of_plots.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.678445 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/redundancy/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/redundancy/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   210926 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/redundancy/redundancy_agent_four_signals.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2828 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/redundancy/redundancy_agent_four_signals.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26075 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/redundancy/redundancy_agent_one_signal.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3154 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/redundancy/redundancy_agent_one_signal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12416 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_1_generator_agent.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1851 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_1_generator_agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11361 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_2_math_agent.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2032 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_2_math_agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25871 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_3_multi_channel.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2460 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_3_multi_channel.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12216 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_4_metrological_streams.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2515 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_4_metrological_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15107 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_5_coalition.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1006 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_5_coalition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4124 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_6_mesa_backend.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      682 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_6_mesa_backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    32218 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2374 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      152 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/dev-requirements.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6023 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/dev-requirements.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.694446 agentMET4FOF-0.9.0/docs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10378 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2951 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/INSTALL.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  2375645 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/Pandas-intersphinx-mappings-objects.inv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   998341 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/PyDynamic-intersphinx-mappings-objects.inv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   965388 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/SciPy-intersphinx-mappings-objects.inv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    59325 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/UML_agentMET4FOF_classes_only.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34207 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/UML_agents_full.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   140724 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/UML_dashboard_full.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   488641 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/UML_metrological_agents_full.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   169510 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/UML_metrological_streams_full.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   129661 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/UML_streams_full.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1311 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/UMLs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/agentMET4FOF_agents.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      132 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/agentMET4FOF_dashboard.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      128 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/agentMET4FOF_network.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      627 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/agentMET4FOF_streams.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      167 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/agentMET4FOF_utilities.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13685 2021-07-08 13:46:22.000000 agentMET4FOF-0.9.0/docs/conf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/index.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25487 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/matplotlib3.3_pytest_error_log
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   791798 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/numpy-intersphinx-mappings.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  2374912 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/pandas-intersphinx-mappings.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  1213296 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/python-intersphinx-mappings-objects.inv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   161853 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/screenshot_met4fof.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/sphinx-requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1313 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/time-series-buffer-intersphinx-mappings.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1581 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/time-series-metadata-intersphinx-mappings-objects.inv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      812 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/docs/tutorials.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      234 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/environment.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7561 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/license.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2903 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2021-07-08 13:46:27.698446 agentMET4FOF-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3390 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:46:27.698446 agentMET4FOF-0.9.0/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1559 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3252 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_addremove_metrological_agents.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2008 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_all_imports.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1136 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_dashboard.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6242 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_memory_monitor_agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4166 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_metadata_metrological_agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_network.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7685 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_redundancy_agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_remove_agent.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      651 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_send_plot_image.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      652 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_send_plot_plotly.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2056 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tests/test_tutorials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2021-07-08 13:45:05.000000 agentMET4FOF-0.9.0/tox.ini
```

### Comparing `agentMET4FOF-0.8.1/.circleci/config.yml` & `agentMET4FOF-0.9.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/.readthedocs.yml` & `agentMET4FOF-0.9.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/PKG-INFO` & `agentMET4FOF-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentMET4FOF
-Version: 0.8.1
+Version: 0.9.0
 Summary: A software package for the integration of metrological input into an agent-based system for the consideration of measurement uncertainty in current industrial manufacturing processes.
 Home-page: https://github.com/bangxiangyong/agentMET4FOF
 Author: Bang Xiang Yong, Björn Ludwig, Anupam Prasad Vedurmudi, Maximilian Gruber, Haris Lulic
 Author-email: bxy20@cam.ac.uk
 License: UNKNOWN
 Project-URL: Documentation, https://agentmet4fof.readthedocs.io/
 Project-URL: Source, https://github.com/bangxiangyong/agentMET4FOF
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentMET4FOF Version: 0.8.1 Summary: A software
+Metadata-Version: 2.1 Name: agentMET4FOF Version: 0.9.0 Summary: A software
 package for the integration of metrological input into an agent-based system
 for the consideration of measurement uncertainty in current industrial
 manufacturing processes. Home-page: https://github.com/bangxiangyong/
 agentMET4FOF Author: Bang Xiang Yong, BjÃ¶rn Ludwig, Anupam Prasad Vedurmudi,
 Maximilian Gruber, Haris Lulic Author-email: bxy20@cam.ac.uk License: UNKNOWN
 Project-URL: Documentation, https://agentmet4fof.readthedocs.io/ Project-URL:
 Source, https://github.com/bangxiangyong/agentMET4FOF Project-URL: Tracker,
```

### Comparing `agentMET4FOF-0.8.1/README.md` & `agentMET4FOF-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard.py` & `agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard_Control.py` & `agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard_Control.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard_agt_net.py` & `agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard_agt_net.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/dashboard/Dashboard_layout_base.py` & `agentMET4FOF-0.9.0/agentMET4FOF/dashboard/Dashboard_layout_base.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/dashboard/LayoutHelper.py` & `agentMET4FOF-0.9.0/agentMET4FOF/dashboard/LayoutHelper.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/dashboard/assets/render_mpld3.js` & `agentMET4FOF-0.9.0/agentMET4FOF/dashboard/assets/render_mpld3.js`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/dashboard/default_network_stylesheet.py` & `agentMET4FOF-0.9.0/agentMET4FOF/dashboard/default_network_stylesheet.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF/streams.py` & `agentMET4FOF-0.9.0/agentMET4FOF/streams/base_streams.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import warnings
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from pandas import DataFrame
 from time_series_metadata.scheme import MetaData
-import warnings
 
-class DataStreamMET4FOF():
-    """
-    Abstract class for creating datastreams.
+__all__ = ["DataStreamMET4FOF"]
+
+
+class DataStreamMET4FOF:
+    """Abstract class for creating datastreams
 
     Data can be fetched sequentially using :func:`next_sample` or all at once
     :func:`all_samples`. This increments the internal sample index :attr:`_sample_idx`.
 
     For sensors data, we assume:
 
     - The format shape for 2D data stream (timesteps, n_sensors)
@@ -75,18 +77,18 @@
         super().__init__()
         self._quantities: Union[List, DataFrame, np.ndarray]
         self._target: Union[List, DataFrame, np.ndarray]
         self._time: Union[List, DataFrame, np.ndarray]
         self._current_sample_quantities: Union[List, DataFrame, np.ndarray]
         self._current_sample_target: Union[List, DataFrame, np.ndarray]
         self._current_sample_time: Union[List, DataFrame, np.ndarray]
-        self._sample_idx: int = 0 #current sample index
-        self._n_samples: int = 0 #total number of samples
+        self._sample_idx: int = 0  # current sample index
+        self._n_samples: int = 0  # total number of samples
         self._data_source_type: str = "function"
-        self._generator_function : Callable
+        self._generator_function: Callable
         self._generator_parameters: Dict = {}
         self.sfreq: int = 1
         self._metadata: MetaData
 
     def _set_data_source_type(self, dt_type: str = "function"):
         """
         To explicitly account for the type of data source: either from dataset,
@@ -101,35 +103,38 @@
 
     def randomize_data(self):
         """Randomizes the provided quantities, useful in machine learning contexts"""
         random_index = np.arange(self._quantities.shape[0])
         np.random.shuffle(random_index)
         self._quantities = self._quantities[random_index]
 
-        if type(self._target).__name__ == "ndarray" or type(self._target).__name__ == "list":
+        if (
+            type(self._target).__name__ == "ndarray"
+            or type(self._target).__name__ == "list"
+        ):
             self._target = self._target[random_index]
         elif type(self._target).__name__ == "DataFrame":
             self._target = self._target.iloc[random_index]
 
     @property
     def metadata(self):
         return self._metadata
 
     @property
     def sample_idx(self):
         return self._sample_idx
 
     def set_metadata(
-            self,
-            device_id: str,
-            time_name: str,
-            time_unit: str,
-            quantity_names: Union[str, Tuple[str, ...]],
-            quantity_units: Union[str, Tuple[str, ...]],
-            misc: Optional[Any] = None
+        self,
+        device_id: str,
+        time_name: str,
+        time_unit: str,
+        quantity_names: Union[str, Tuple[str, ...]],
+        quantity_units: Union[str, Tuple[str, ...]],
+        misc: Optional[Any] = None,
     ):
         """Set the quantities metadata as a ``MetaData`` object
 
         Details you find in the :class:`time_series_metadata.scheme.MetaData`
         documentation.
 
         Parameters
@@ -150,29 +155,29 @@
         """
         self._metadata = MetaData(
             device_id=device_id,
             time_name=time_name,
             time_unit=time_unit,
             quantity_names=quantity_names,
             quantity_units=quantity_units,
-            misc=misc
+            misc=misc,
         )
 
     def _default_generator_function(self, time):
         """This is the default generator function used, if non was specified
 
         Parameters
         ----------
         time : Union[List, DataFrame, np.ndarray]
         """
-        amplitude = np.sin(2*np.pi*self.F*time)
-        return amplitude
+        value = np.sin(2 * np.pi * self.F * time)
+        return value
 
     def set_generator_function(
-            self, generator_function: Callable = None, sfreq: int = None, **kwargs: Any
+        self, generator_function: Callable = None, sfreq: int = None, **kwargs: Any
     ):
         """
         Sets the data source to a generator function. By default, this function resorts
         to a sine wave generator function. Initialisation of the generator's
         parameters should be done here such as setting the sampling frequency and
         wave frequency. For setting it with a dataset instead,
         see :func:`set_data_source`.
@@ -187,22 +192,22 @@
             Sampling frequency.
         **kwargs : Any
             Any additional keyword arguments to be supplied to the generator function.
             The ``**kwargs`` will be saved as :attr:`_generator_parameters`.
             The generator function call for every sample will be supplied with the
             ``**generator_parameters``.
         """
-        #save the kwargs into generator_parameters
+        # save the kwargs into generator_parameters
         self._generator_parameters = kwargs
 
         if sfreq is not None:
             self.sfreq = sfreq
         self._set_data_source_type("function")
 
-        #resort to default wave generator if one is not supplied
+        # resort to default wave generator if one is not supplied
         if generator_function is None:
             warnings.warn(
                 "No uncertainty generator function specified. Setting to default ("
                 "sine wave)."
             )
             self.F = 50
             self._generator_function = self._default_generator_function
@@ -210,29 +215,28 @@
             self._generator_function = generator_function
         return self._generator_function
 
     def _next_sample_generator(self, batch_size: int = 1) -> Dict[str, np.ndarray]:
         """
         Internal method for generating a batch of samples from the generator function.
         """
-        time: np.ndarray = np.arange(self._sample_idx, self._sample_idx + batch_size,
-                                     1)/self.sfreq
+        time: np.ndarray = (
+            np.arange(self._sample_idx, self._sample_idx + batch_size, 1) / self.sfreq
+        )
         self._sample_idx += batch_size
 
-        amplitude: np.ndarray = self._generator_function(
-            time, **self._generator_parameters
-        )
+        value: np.ndarray = self._generator_function(time, **self._generator_parameters)
 
-        return {'quantities': amplitude, 'time': time}
+        return {"quantities": value, "time": time}
 
     def set_data_source(
-            self,
-            quantities: Union[List, DataFrame, np.ndarray]=None,
-            target: Optional[Union[List, DataFrame, np.ndarray]]=None,
-            time: Optional[Union[List, DataFrame, np.ndarray]]=None
+        self,
+        quantities: Union[List, DataFrame, np.ndarray] = None,
+        target: Optional[Union[List, DataFrame, np.ndarray]] = None,
+        time: Optional[Union[List, DataFrame, np.ndarray]] = None,
     ):
         """
         This sets the data source by providing up to three iterables: ``quantities`` ,
         ``time`` and ``target`` which are assumed to be aligned.
 
         For sensors data, we assume:
         The format shape for 2D data stream (timesteps, n_sensors)
@@ -265,18 +269,18 @@
             self._time = list(np.arange(10))
             self._target.reverse()
         else:
             self._quantities = quantities
             self._target = target
             self._time = time
 
-        #infer number of samples
+        # infer number of samples
         if type(self._quantities).__name__ == "list":
             self._n_samples = len(self._quantities)
-        elif type(self._quantities).__name__ == "DataFrame": #dataframe or numpy
+        elif type(self._quantities).__name__ == "DataFrame":  # dataframe or numpy
             self._quantities = self._quantities.to_numpy()
             self._n_samples = self._quantities.shape[0]
         elif type(self._quantities).__name__ == "ndarray":
             self._n_samples = self._quantities.shape[0]
         self._set_data_source_type("dataset")
 
     def prepare_for_use(self):
@@ -308,17 +312,17 @@
         Returns
         -------
         samples : Dict
             ``{'time':current_sample_time, 'quantities':current_sample_quantities,
             'target':current_sample_target}``
         """
 
-        if self._data_source_type == 'function':
+        if self._data_source_type == "function":
             return self._next_sample_generator(batch_size)
-        elif self._data_source_type == 'dataset':
+        elif self._data_source_type == "dataset":
             return self._next_sample_data_source(batch_size)
 
     def _next_sample_data_source(
         self, batch_size: int = 1
     ) -> Dict[str, Union[List, DataFrame, np.ndarray]]:
         """
         Internal method for fetching latest samples from a dataset.
@@ -336,110 +340,42 @@
         """
         if batch_size < 0:
             batch_size = self._quantities.shape[0]
 
         self._sample_idx += batch_size
 
         try:
-            self._current_sample_quantities = self._quantities[self._sample_idx - batch_size:self._sample_idx]
+            self._current_sample_quantities = self._quantities[
+                self._sample_idx - batch_size : self._sample_idx
+            ]
 
-            #if target is available
+            # if target is available
             if self._target is not None:
-                self._current_sample_target = self._target[self._sample_idx - batch_size:self._sample_idx]
+                self._current_sample_target = self._target[
+                    self._sample_idx - batch_size : self._sample_idx
+                ]
             else:
                 self._current_sample_target = None
 
-            #if time is available
+            # if time is available
             if self._time is not None:
-                self._current_sample_time = self._time[self._sample_idx - batch_size
-                                                       :self._sample_idx]
+                self._current_sample_time = self._time[
+                    self._sample_idx - batch_size : self._sample_idx
+                ]
             else:
                 self._current_sample_time = None
         except IndexError:
             self._current_sample_quantities = None
             self._current_sample_target = None
             self._current_sample_time = None
 
-        return {'time':self._current_sample_time, 'quantities': self._current_sample_quantities, 'target': self._current_sample_target}
+        return {
+            "time": self._current_sample_time,
+            "quantities": self._current_sample_quantities,
+            "target": self._current_sample_target,
+        }
 
     def reset(self):
         self._sample_idx = 0
 
     def has_more_samples(self):
         return self._sample_idx < self._n_samples
-
-
-# Built-in classes with DataStreamMET4FOF
-class SineGenerator(DataStreamMET4FOF):
-    """
-    Built-in class of sine wave generator which inherits all
-    methods and attributes from :class:`DataStreamMET4FOF`.
-    :func:`sine_wave_function` is a custom defined function which has a required
-    keyword ``time`` as argument and any number of optional additional arguments
-    (e.g ``F``) to be supplied to the :meth:`.DataStreamMET4FOF.set_generator_function`.
-
-    Parameters
-    ----------
-    sfreq : int
-        sampling frequency which determines the time step when :meth:`.next_sample`
-        is called
-    sine_freq : float
-        frequency of wave function
-    """
-    def __init__(self, sfreq=500, sine_freq=50):
-        super().__init__()
-        self.set_metadata("SineGenerator","time","s",("Voltage"),("V"),"Simple sine wave generator")
-        self.set_generator_function(generator_function=self.sine_wave_function, sfreq=sfreq, sine_freq=sine_freq)
-
-    def sine_wave_function(self, time, sine_freq):
-        """A simple sine wave generator"""
-        amplitude = np.sin(2 * np.pi * sine_freq * time)
-        return amplitude
-
-
-class CosineGenerator(DataStreamMET4FOF):
-    """
-    Built-in class of cosine wave generator which inherits all
-    methods and attributes from :class:`DataStreamMET4FOF`.
-    :func:`cosine_wave_function` is a custom defined function which has a required
-    keyword ``time`` as argument and any number of
-    optional additional arguments (e.g ``cosine_freq``) to be supplied to the
-    :meth:`.DataStreamMET4FOF.set_generator_function`.
-
-    Parameters
-    ----------
-    sfreq : int
-        sampling frequency which determines the time step when :meth:`.next_sample`
-        is called
-    F : int
-        frequency of wave function
-    """
-    def __init__(self, sfreq = 500, cosine_freq=5):
-        super().__init__()
-        self.set_metadata("CosineGenerator","time","s",("Voltage"),("V"),"Simple cosine wave generator")
-        self.set_generator_function(generator_function=self.cosine_wave_function, sfreq=sfreq, cosine_freq=cosine_freq)
-
-    def cosine_wave_function(self, time, cosine_freq=50):
-        """A simple cosine wave generator"""
-        amplitude = np.cos(2 * np.pi * cosine_freq * time)
-        return amplitude
-
-
-def extract_x_y(message):
-    """
-    Extracts features & target from ``message['data']`` with expected structure such as:
-
-    1. tuple - (x,y)
-    2. dict - {'x':x_data,'y':y_data}
-
-    Handle data structures of dictionary to extract features & target
-    """
-    if type(message['data']) == tuple:
-        x = message['data'][0]
-        y = message['data'][1]
-    elif type(message['data']) == dict:
-        x = message['data']['x']
-        y = message['data']['y']
-    else:
-        return 1
-    return x, y
-
```

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF.egg-info/PKG-INFO` & `agentMET4FOF-0.9.0/agentMET4FOF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentMET4FOF
-Version: 0.8.1
+Version: 0.9.0
 Summary: A software package for the integration of metrological input into an agent-based system for the consideration of measurement uncertainty in current industrial manufacturing processes.
 Home-page: https://github.com/bangxiangyong/agentMET4FOF
 Author: Bang Xiang Yong, Björn Ludwig, Anupam Prasad Vedurmudi, Maximilian Gruber, Haris Lulic
 Author-email: bxy20@cam.ac.uk
 License: UNKNOWN
 Project-URL: Documentation, https://agentmet4fof.readthedocs.io/
 Project-URL: Source, https://github.com/bangxiangyong/agentMET4FOF
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agentMET4FOF Version: 0.8.1 Summary: A software
+Metadata-Version: 2.1 Name: agentMET4FOF Version: 0.9.0 Summary: A software
 package for the integration of metrological input into an agent-based system
 for the consideration of measurement uncertainty in current industrial
 manufacturing processes. Home-page: https://github.com/bangxiangyong/
 agentMET4FOF Author: Bang Xiang Yong, BjÃ¶rn Ludwig, Anupam Prasad Vedurmudi,
 Maximilian Gruber, Haris Lulic Author-email: bxy20@cam.ac.uk License: UNKNOWN
 Project-URL: Documentation, https://agentmet4fof.readthedocs.io/ Project-URL:
 Source, https://github.com/bangxiangyong/agentMET4FOF Project-URL: Tracker,
```

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF.egg-info/SOURCES.txt` & `agentMET4FOF-0.9.0/agentMET4FOF.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,32 +9,45 @@
 license.md
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .circleci/config.yml
 agentMET4FOF/__init__.py
-agentMET4FOF/agents.py
-agentMET4FOF/metrological_agents.py
-agentMET4FOF/metrological_streams.py
-agentMET4FOF/streams.py
+agentMET4FOF/exceptions.py
+agentMET4FOF/network.py
 agentMET4FOF.egg-info/PKG-INFO
 agentMET4FOF.egg-info/SOURCES.txt
 agentMET4FOF.egg-info/dependency_links.txt
 agentMET4FOF.egg-info/requires.txt
 agentMET4FOF.egg-info/top_level.txt
+agentMET4FOF/agents/__init__.py
+agentMET4FOF/agents/base_agents.py
+agentMET4FOF/agents/metrological_base_agents.py
+agentMET4FOF/agents/metrological_redundancy_agents.py
+agentMET4FOF/agents/metrological_signal_agents.py
+agentMET4FOF/agents/signal_agents.py
 agentMET4FOF/dashboard/Dashboard.py
 agentMET4FOF/dashboard/Dashboard_Control.py
 agentMET4FOF/dashboard/Dashboard_agt_net.py
 agentMET4FOF/dashboard/Dashboard_layout_base.py
 agentMET4FOF/dashboard/LayoutHelper.py
 agentMET4FOF/dashboard/__init__.py
 agentMET4FOF/dashboard/default_network_stylesheet.py
 agentMET4FOF/dashboard/assets/render_mpld3.js
 agentMET4FOF/dashboard/assets/stylesheet.css
+agentMET4FOF/metrological_agents/__init__.py
+agentMET4FOF/metrological_streams/__init__.py
+agentMET4FOF/streams/__init__.py
+agentMET4FOF/streams/base_streams.py
+agentMET4FOF/streams/metrological_base_streams.py
+agentMET4FOF/streams/metrological_signal_streams.py
+agentMET4FOF/streams/signal_streams.py
+agentMET4FOF/utils/__init__.py
+agentMET4FOF/utils/buffer.py
 agentMET4FOF_tutorials/__init__.py
 agentMET4FOF_tutorials/tutorial_1_generator_agent.ipynb
 agentMET4FOF_tutorials/tutorial_1_generator_agent.py
 agentMET4FOF_tutorials/tutorial_2_math_agent.ipynb
 agentMET4FOF_tutorials/tutorial_2_math_agent.py
 agentMET4FOF_tutorials/tutorial_3_multi_channel.ipynb
 agentMET4FOF_tutorials/tutorial_3_multi_channel.py
@@ -42,59 +55,70 @@
 agentMET4FOF_tutorials/tutorial_4_metrological_streams.py
 agentMET4FOF_tutorials/tutorial_5_coalition.ipynb
 agentMET4FOF_tutorials/tutorial_5_coalition.py
 agentMET4FOF_tutorials/tutorial_6_mesa_backend.ipynb
 agentMET4FOF_tutorials/tutorial_6_mesa_backend.py
 agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.ipynb
 agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.py
+agentMET4FOF_tutorials/agent_module/__init__.py
 agentMET4FOF_tutorials/agent_module/ui_main_example.py
 agentMET4FOF_tutorials/agent_module/ui_module_example.py
+agentMET4FOF_tutorials/buffering/__init__.py
 agentMET4FOF_tutorials/buffering/basic_buffering.py
 agentMET4FOF_tutorials/buffering/metrological_buffering.py
 agentMET4FOF_tutorials/buffering/moving_average.py
+agentMET4FOF_tutorials/datastreams/__init__.py
 agentMET4FOF_tutorials/datastreams/gaussianshock_generator.py
 agentMET4FOF_tutorials/datastreams/multi_generator.py
 agentMET4FOF_tutorials/datastreams/simple_generator.py
+agentMET4FOF_tutorials/plotting/__init__.py
 agentMET4FOF_tutorials/plotting/basic_memory_plot.py
 agentMET4FOF_tutorials/plotting/basic_send_plot.py
 agentMET4FOF_tutorials/plotting/custom_memory_multiple_plot.py
 agentMET4FOF_tutorials/plotting/custom_memory_plot.py
 agentMET4FOF_tutorials/plotting/list_of_plots.py
+agentMET4FOF_tutorials/redundancy/__init__.py
+agentMET4FOF_tutorials/redundancy/redundancy_agent_four_signals.ipynb
+agentMET4FOF_tutorials/redundancy/redundancy_agent_four_signals.py
+agentMET4FOF_tutorials/redundancy/redundancy_agent_one_signal.ipynb
+agentMET4FOF_tutorials/redundancy/redundancy_agent_one_signal.py
 docs/CONTRIBUTING.md
 docs/INSTALL.md
 docs/Pandas-intersphinx-mappings-objects.inv
 docs/PyDynamic-intersphinx-mappings-objects.inv
 docs/SciPy-intersphinx-mappings-objects.inv
 docs/UML_agentMET4FOF_classes_only.png
 docs/UML_agents_full.png
 docs/UML_dashboard_full.png
 docs/UML_metrological_agents_full.png
 docs/UML_metrological_streams_full.png
 docs/UML_streams_full.png
 docs/UMLs.md
 docs/agentMET4FOF_agents.rst
 docs/agentMET4FOF_dashboard.rst
-docs/agentMET4FOF_metrological_agents.rst
-docs/agentMET4FOF_metrological_streams.rst
+docs/agentMET4FOF_network.rst
 docs/agentMET4FOF_streams.rst
+docs/agentMET4FOF_utilities.rst
 docs/conf.py
 docs/index.rst
 docs/matplotlib3.3_pytest_error_log
 docs/numpy-intersphinx-mappings.txt
 docs/pandas-intersphinx-mappings.txt
 docs/python-intersphinx-mappings-objects.inv
 docs/screenshot_met4fof.png
 docs/sphinx-requirements.txt
 docs/time-series-buffer-intersphinx-mappings.txt
 docs/time-series-metadata-intersphinx-mappings-objects.inv
+docs/tutorials.rst
 tests/__init__.py
 tests/conftest.py
 tests/test_addremove_metrological_agents.py
 tests/test_all_imports.py
 tests/test_dashboard.py
 tests/test_memory_monitor_agent.py
 tests/test_metadata_metrological_agent.py
 tests/test_network.py
+tests/test_redundancy_agent.py
 tests/test_remove_agent.py
 tests/test_send_plot_image.py
 tests/test_send_plot_plotly.py
 tests/test_tutorials.py
```

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/agent_module/ui_main_example.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/agent_module/ui_main_example.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/agent_module/ui_module_example.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/agent_module/ui_module_example.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/buffering/basic_buffering.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/basic_buffering.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/buffering/metrological_buffering.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/metrological_buffering.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/buffering/moving_average.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/buffering/moving_average.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/datastreams/gaussianshock_generator.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/gaussianshock_generator.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/datastreams/multi_generator.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/multi_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     """
     def __init__(self,sfreq = 500, F=5):
         super().__init__()
         self.set_metadata("SineGenerator","time","s",("Voltage"),("V"),"Simple sine wave generator")
         self.set_generator_function(generator_function=self.sine_wave_function, sfreq=sfreq, F=F)
 
     def sine_wave_function(self, time, F=50):
-        amplitude = np.sin(2*np.pi*F*time)
-        return amplitude
+        value = np.sin(2*np.pi*F*time)
+        return value
 
 class SawToothGenerator(DataStreamMET4FOF):
     """
     Sawtooth function generator inherited from `DataStreamMET4FOF`
 
     `sawtooth_function` is a custom defined function which has a required keyword `time` as argument and any number of optional additional arguments (`F`).
     to be supplied to the `set_generator_function`
@@ -34,16 +34,16 @@
     """
     def __init__(self,sfreq = 500, F=5):
         super().__init__()
         self.set_metadata("SawToothGenerator","time","s",("Voltage"),("V"), "Simple sawtooth generator using scipy function")
         self.set_generator_function(generator_function=self.sawtooth_wave_function, sfreq=sfreq, F=F)
 
     def sawtooth_wave_function(self, time, F):
-        amplitude = signal.sawtooth(2 * np.pi * F * time)
-        return amplitude
+        value = signal.sawtooth(2 * np.pi * F * time)
+        return value
 
 class SquareGenerator(DataStreamMET4FOF):
     """
     Built-in class of square wave generator inherited from `DataStreamMET4FOF`.
 
     `square_wave_function` is a custom defined function which has a required keyword `time` as argument and any number of optional additional arguments (`F`).
     to be supplied to the `set_generator_function`
@@ -51,16 +51,16 @@
     """
     def __init__(self,sfreq = 500, F=5):
         super().__init__()
         self.set_metadata("SquareGenerator","time","s",("Voltage"),("V"), "Simple square wave generator using scipy functio")
         self.set_generator_function(generator_function=self.square_wave_function, sfreq=sfreq, F=F)
 
     def square_wave_function(self, time, F):
-        amplitude = signal.square(2 * np.pi * F * time)
-        return amplitude
+        value = signal.square(2 * np.pi * F * time)
+        return value
 
 class MultiGeneratorAgent(AgentMET4FOF):
     """
     An agent streaming a multiple signals from SineGenerator, SawToothGenerator and SquareGenerator
     """
 
     # The datatype of the stream will be SineGenerator, SawToothGenerator and SquareGenerator.
```

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/datastreams/simple_generator.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/datastreams/simple_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 from agentMET4FOF.agents import AgentMET4FOF, AgentNetwork, MonitorAgent
 from agentMET4FOF.streams import DataStreamMET4FOF
 import numpy as np
 
+
 class SineGenerator(DataStreamMET4FOF):
     """
     Built-in class of sine wave generator.
     `sfreq` is sampling frequency which determines the time step when next_sample is called
     `F` is frequency of wave function
     `sine_wave_function` is a custom defined function which has a required keyword `time` as argument and any number of optional additional arguments (e.g `F`).
     to be supplied to the `set_generator_function`
 
     """
-    def __init__(self,sfreq = 500, F=5):
+
+    def __init__(self, sfreq=500, F=5):
         super().__init__()
-        self.set_metadata("SineGenerator","time","s",("Voltage"),("V"),"Simple sine wave generator")
-        self.set_generator_function(generator_function=self.sine_wave_function, sfreq=sfreq, F=F)
+        self.set_metadata(
+            "SineGenerator",
+            "time",
+            "s",
+            ("Voltage"),
+            ("V"),
+            "Simple sine wave generator",
+        )
+        self.set_generator_function(
+            generator_function=self.sine_wave_function, sfreq=sfreq, F=F
+        )
 
     def sine_wave_function(self, time, F=50):
-        amplitude = np.sin(2*np.pi*F*time)
-        return amplitude
+        value = np.sin(2 * np.pi * F * time)
+        return value
+
 
 class SineGeneratorAgent(AgentMET4FOF):
     """An agent streaming a sine signal
 
     Takes samples from the :py:mod:`SineGenerator` and pushes them sample by sample
     to connected agents via its output channel.
     """
```

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/basic_memory_plot.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/basic_memory_plot.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/basic_send_plot.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/basic_send_plot.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/custom_memory_multiple_plot.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/custom_memory_multiple_plot.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/custom_memory_plot.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/custom_memory_plot.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/plotting/list_of_plots.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/plotting/list_of_plots.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_1_generator_agent.ipynb` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_1_generator_agent.ipynb`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_1_generator_agent.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_1_generator_agent.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_2_math_agent.ipynb` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_2_math_agent.ipynb`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_2_math_agent.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_2_math_agent.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_3_multi_channel.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_3_multi_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def init_parameters(self):
         self._sine_stream = SineGenerator()
         self._cos_stream = CosineGenerator()
 
     def agent_loop(self):
         if self.current_state == "Running":
             sine_data = self._sine_stream.next_sample()  # dictionary
-            cosine_data = self._sine_stream.next_sample()  # dictionary
+            cosine_data = self._cos_stream.next_sample()  # dictionary
             self.send_output(sine_data["quantities"], channel="sine")
             self.send_output(cosine_data["quantities"], channel="cosine")
 
 
 class MultiOutputMathAgent(AgentMET4FOF):
 
     _minus_param: float
```

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_4_metrological_streams.ipynb` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_4_metrological_streams.ipynb`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_4_metrological_streams.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_4_metrological_streams.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_5_coalition.ipynb` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_5_coalition.ipynb`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_5_coalition.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_5_coalition.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_6_mesa_backend.ipynb` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_6_mesa_backend.ipynb`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_6_mesa_backend.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_6_mesa_backend.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.ipynb` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.ipynb`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.py` & `agentMET4FOF-0.9.0/agentMET4FOF_tutorials/tutorial_7_generic_metrological_agent.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/dev-requirements.txt` & `agentMET4FOF-0.9.0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/CONTRIBUTING.md` & `agentMET4FOF-0.9.0/docs/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 consequence, at any time commits may changes parts of agentMET4FOF's public interface so
 that previously written code may no longer be executable. If this occurs we try though,
 to mention migration strategies in the corresponding release descriptions.
 
 #### Commit message examples
 
 For examples please checkout the
-[Git Log](https://github.com/Met4FoF/agentMET4FOF/commits/master).
+[Git Log](https://github.com/Met4FoF/agentMET4FOF/commits/develop).
 
 ###  Testing
 
 We strive to increase [our code coverage](https://codecov.io/gh/Met4FoF/agentMET4FOF)
 with every change introduced. This requires that every new feature and every change to 
 existing features is accompanied by appropriate _pytest_ testing. We test the basic
 components for correctness and, if necessary, the integration into the big picture.
```

### Comparing `agentMET4FOF-0.8.1/docs/INSTALL.md` & `agentMET4FOF-0.9.0/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/Pandas-intersphinx-mappings-objects.inv` & `agentMET4FOF-0.9.0/docs/Pandas-intersphinx-mappings-objects.inv`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/PyDynamic-intersphinx-mappings-objects.inv` & `agentMET4FOF-0.9.0/docs/PyDynamic-intersphinx-mappings-objects.inv`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/SciPy-intersphinx-mappings-objects.inv` & `agentMET4FOF-0.9.0/docs/SciPy-intersphinx-mappings-objects.inv`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/UML_agentMET4FOF_classes_only.png` & `agentMET4FOF-0.9.0/docs/UML_agentMET4FOF_classes_only.png`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/UML_agents_full.png` & `agentMET4FOF-0.9.0/docs/UML_agents_full.png`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/UML_dashboard_full.png` & `agentMET4FOF-0.9.0/docs/UML_dashboard_full.png`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/UML_metrological_agents_full.png` & `agentMET4FOF-0.9.0/docs/UML_metrological_agents_full.png`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/UML_metrological_streams_full.png` & `agentMET4FOF-0.9.0/docs/UML_metrological_streams_full.png`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/UML_streams_full.png` & `agentMET4FOF-0.9.0/docs/UML_streams_full.png`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/UMLs.md` & `agentMET4FOF-0.9.0/docs/UMLs.md`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/conf.py` & `agentMET4FOF-0.9.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,43 +64,27 @@
         "https://time-series-metadata.readthedocs.io/en/latest/",
         None,
     ),
     "np": (
         "https://numpy.org/doc/stable/",
         None,
     ),
+    "time-series-buffer": (
+        "https://time-series-buffer.readthedocs.io/en/latest/",
+        None,
+    ),
 }
 # We keep the objects.inv files in our docs folder to get hints on how to specify the
 # cross-references. More on the topic can be found here:
 # https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
 # The objects.inv we gathered by the command:
 # $ python -msphinx.ext.intersphinx https://docs.python.org/3/objects.inv
 # which we took from the linked page (almost at the very bottom at the time of
 # writing this).
 
-
-# This should make SciPy documentation available inside our docs.
-intersphinx_mapping = {
-    "NumPy": ("https://numpy.org/doc/stable/", None),
-    "Pandas": ("http://pandas.pydata.org/pandas-docs/dev", None),
-    "SciPy": ("https://docs.scipy.org/doc/scipy/reference", None),
-    "PyDynamic": (
-        "https://pydynamic.readthedocs.io/en/latest/",
-        None,
-    ),
-    "time-series-metadata": (
-        "https://time-series-metadata.readthedocs.io/en/latest/",
-        None,
-    ),
-    "time-series-buffer": (
-        "https://time-series-buffer.readthedocs.io/en/latest/",
-        None,
-    ),
-}
-
 nbsphinx_allow_errors = True
 
 ################################################################################
 # This part is originally taken from
 # https://github.com/cornellius-gp/gpytorch/issues/new/choose?permalink=https%3A%2F%2Fgithub.com%2Fcornellius-gp%2Fgpytorch%2Fblob%2F0b28dd0b8430a0df9838593e7e632dc01d20bcf4%2Fdocs%2Fsource%2Fconf.py%23L107
 #
 # Copy over examples and tutorials and all other folders to docs' source
@@ -109,15 +93,15 @@
 # Copy over README.md from root folder.
 shutil.copyfile(
     os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "README.md")),
     os.path.join(os.path.dirname(__file__), "README.md"),
 )
 # Copy over CHANGELOG from root folder.
 shutil.copyfile(
-    os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "CHANGELOG")),
+    os.path.abspath(os.path.join(os.path.dirname(__file__), "..", "CHANGELOG.md")),
     os.path.join(os.path.dirname(__file__), "CHANGELOG.md"),
 )
 
 # Copy over all other specified folders from repository tree.
 
 
 def make_path_dict(source: str, destination: str) -> dict:
@@ -182,15 +166,15 @@
 )
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.8.1'
+version = "0.9.0"
 # The full version, including alpha/beta/rc tags.
 # release = '0.0.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `agentMET4FOF-0.8.1/docs/matplotlib3.3_pytest_error_log` & `agentMET4FOF-0.9.0/docs/matplotlib3.3_pytest_error_log`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/numpy-intersphinx-mappings.txt` & `agentMET4FOF-0.9.0/docs/numpy-intersphinx-mappings.txt`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/pandas-intersphinx-mappings.txt` & `agentMET4FOF-0.9.0/docs/pandas-intersphinx-mappings.txt`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/python-intersphinx-mappings-objects.inv` & `agentMET4FOF-0.9.0/docs/python-intersphinx-mappings-objects.inv`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/screenshot_met4fof.png` & `agentMET4FOF-0.9.0/docs/screenshot_met4fof.png`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/time-series-buffer-intersphinx-mappings.txt` & `agentMET4FOF-0.9.0/docs/time-series-buffer-intersphinx-mappings.txt`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/docs/time-series-metadata-intersphinx-mappings-objects.inv` & `agentMET4FOF-0.9.0/docs/time-series-metadata-intersphinx-mappings-objects.inv`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/license.md` & `agentMET4FOF-0.9.0/license.md`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/requirements.txt` & `agentMET4FOF-0.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/setup.cfg` & `agentMET4FOF-0.9.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 commit_parser = semantic_release.history.angular_parser
 upload_to_pypi = true
 upload_to_release = true
 branch = develop
 hvcs = github
 commit_version_number = true
 changelog_file = CHANGELOG.md
-changelog_sections = feature,fix,breaking,documentation,performance
+changelog_sections = feature,fix,refactor,breaking,documentation,performance
 changelog_components = semantic_release.changelog.changelog_headers,semantic_release.changelog.compare_url
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `agentMET4FOF-0.8.1/setup.py` & `agentMET4FOF-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/tests/test_addremove_metrological_agents.py` & `agentMET4FOF-0.9.0/tests/test_addremove_metrological_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import time
-
 import pytest
 
-from agentMET4FOF.metrological_agents import MetrologicalAgent, MetrologicalMonitorAgent
-
-# Create a list of permutations with which we want to test creation of agents and
-# binding.
+from agentMET4FOF.agents.metrological_base_agents import (
+    MetrologicalAgent,
+    MetrologicalMonitorAgent,
+)
 from tests.conftest import test_timeout
 
 agent_type_permutations = [
     [MetrologicalAgent],
     [MetrologicalMonitorAgent],
     [MetrologicalAgent, MetrologicalAgent],
     [MetrologicalAgent, MetrologicalMonitorAgent],
```

### Comparing `agentMET4FOF-0.8.1/tests/test_dashboard.py` & `agentMET4FOF-0.9.0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `agentMET4FOF-0.8.1/tests/test_memory_monitor_agent.py` & `agentMET4FOF-0.9.0/tests/test_memory_monitor_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 import pytest
 
-from agentMET4FOF.agents import AgentMET4FOF, MonitorAgent
+from agentMET4FOF.agents.base_agents import AgentMET4FOF, MonitorAgent
 from tests.conftest import test_timeout
 
 num_samples = 10
 
 # prepare dummy data stream
 datastream_x = list(np.arange(num_samples))
 datastream_y = list(np.arange(num_samples))
```

### Comparing `agentMET4FOF-0.8.1/tests/test_metadata_metrological_agent.py` & `agentMET4FOF-0.9.0/tests/test_metadata_metrological_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import time
 from typing import Dict
 
 import numpy as np
 import pytest
 from time_series_metadata.scheme import MetaData
 
-from agentMET4FOF.metrological_agents import MetrologicalAgent, MetrologicalMonitorAgent
+from agentMET4FOF.agents.metrological_base_agents import (
+    MetrologicalAgent,
+    MetrologicalMonitorAgent,
+)
 from tests.conftest import test_timeout
 
 
 class Signal:
     """
     Simple class to request time-series datapoints of a signal
     """
@@ -125,13 +128,11 @@
         try:
             # Run actual check. This reduces test runtime in case of passed tests but
             # results in quite cryptic error messages in case it fails due to the
             # timeout causing the actual fail. So, if this line fails, regardless of
             # the error message, it means, the addressed attribute's content does not
             # match the expected expression.
             # Check if key 'metadata' is present in the received data
-            buffer_dict = list(monitor_agent_1.get_attr('buffer').values())[0]
+            buffer_dict = list(monitor_agent_1.get_attr("buffer").values())[0]
             is_present = "metadata" in buffer_dict.keys()
         except IndexError:
             pass
-
-
```

### Comparing `agentMET4FOF-0.8.1/tests/test_remove_agent.py` & `agentMET4FOF-0.9.0/tests/test_remove_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 
 import pytest
 
-from agentMET4FOF.agents import AgentMET4FOF
+from agentMET4FOF.agents.base_agents import AgentMET4FOF
 from tests.conftest import test_timeout
 
 
 @pytest.mark.timeout(test_timeout)
 def test_remove_agent(agent_network):
     # init agents by adding into the agent network
     dummy_agent1 = agent_network.add_agent(agentType=AgentMET4FOF)
```

