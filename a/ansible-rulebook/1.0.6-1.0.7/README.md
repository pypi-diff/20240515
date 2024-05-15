# Comparing `tmp/ansible_rulebook-1.0.6.tar.gz` & `tmp/ansible_rulebook-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_rulebook-1.0.6.tar", last modified: Tue Mar 12 12:28:14 2024, max compression
+gzip compressed data, was "ansible_rulebook-1.0.7.tar", last modified: Wed May 15 14:39:53 2024, max compression
```

## Comparing `ansible_rulebook-1.0.6.tar` & `ansible_rulebook-1.0.7.tar`

### file list

```diff
@@ -1,463 +1,463 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.841500 ansible_rulebook-1.0.6/
--rw-r--r--   0 alex      (1000) alex      (1000)    11358 2022-07-11 07:18:31.000000 ansible_rulebook-1.0.6/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      312 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     4324 2024-03-12 12:28:14.841500 ansible_rulebook-1.0.6/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     3353 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.6/README.rst
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.759501 ansible_rulebook-1.0.6/ansible_rulebook/
--rw-r--r--   0 alex      (1000) alex      (1000)      655 2024-03-12 12:25:44.000000 ansible_rulebook-1.0.6/ansible_rulebook/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      634 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/ansible_rulebook/__main__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.763501 ansible_rulebook-1.0.6/ansible_rulebook/action/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1853 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/control.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2875 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/debug.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5450 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/helper.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1271 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/metadata.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1151 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/noop.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1555 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/post_event.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1532 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/print_event.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1891 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/retract_fact.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6316 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/run_job_template.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2397 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/run_module.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10326 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/run_playbook.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6490 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/run_workflow_template.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3906 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/runner.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1691 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/set_fact.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2154 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/action/shutdown.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9389 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/app.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10697 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/cli.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4775 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/collection.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1136 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/common.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8512 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/ansible_rulebook/condition_parser.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2659 2023-02-23 16:22:58.000000 ansible_rulebook-1.0.6/ansible_rulebook/condition_types.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1110 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/conf.py
--rw-r--r--   0 alex      (1000) alex      (1000)    11493 2024-02-05 12:43:06.000000 ansible_rulebook-1.0.6/ansible_rulebook/engine.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.763501 ansible_rulebook-1.0.6/ansible_rulebook/event_filter/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.6/ansible_rulebook/event_filter/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1346 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.6/ansible_rulebook/event_filter/insert_meta_info.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2494 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/exception.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7860 2024-02-07 17:45:38.000000 ansible_rulebook-1.0.6/ansible_rulebook/job_template_runner.py
--rw-r--r--   0 alex      (1000) alex      (1000)    12203 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/ansible_rulebook/json_generator.py
--rw-r--r--   0 alex      (1000) alex      (1000)      827 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/ansible_rulebook/messages.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3183 2023-11-30 12:34:41.000000 ansible_rulebook-1.0.6/ansible_rulebook/rule_generator.py
--rw-r--r--   0 alex      (1000) alex      (1000)    19689 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/rule_set_runner.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2457 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/ansible_rulebook/rule_types.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6797 2023-11-30 12:34:41.000000 ansible_rulebook-1.0.6/ansible_rulebook/rules_parser.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.763501 ansible_rulebook-1.0.6/ansible_rulebook/schema/
--rw-r--r--   0 alex      (1000) alex      (1000)    22926 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/schema/ruleset_schema.json
--rw-r--r--   0 alex      (1000) alex      (1000)     5486 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/terminal.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1836 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/token.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8118 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/util.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1428 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/ansible_rulebook/validators.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8137 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/ansible_rulebook/websocket.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.841500 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     4324 2024-03-12 12:28:14.000000 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)    14555 2024-03-12 12:28:14.000000 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-03-12 12:28:14.000000 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       63 2024-03-12 12:28:14.000000 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-03-12 12:28:14.000000 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/not-zip-safe
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2024-03-12 12:28:14.000000 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       17 2024-03-12 12:28:14.000000 ansible_rulebook-1.0.6/ansible_rulebook.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.767500 ansible_rulebook-1.0.6/docs/
--rw-r--r--   0 alex      (1000) alex      (1000)      617 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/docs/Makefile
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.751501 ansible_rulebook-1.0.6/docs/_build/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.751501 ansible_rulebook-1.0.6/docs/_build/html/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.768501 ansible_rulebook-1.0.6/docs/_build/html/_static/
--rw-r--r--   0 alex      (1000) alex      (1000)      286 2022-10-20 07:13:59.000000 ansible_rulebook-1.0.6/docs/_build/html/_static/file.png
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.768501 ansible_rulebook-1.0.6/docs/_build/html/_static/images/
--rw-r--r--   0 alex      (1000) alex      (1000)     8664 2023-01-11 10:06:59.000000 ansible_rulebook-1.0.6/docs/_build/html/_static/images/Ansible-Mark-RGB_Black.png
--rw-r--r--   0 alex      (1000) alex      (1000)     5173 2023-01-11 10:06:59.000000 ansible_rulebook-1.0.6/docs/_build/html/_static/images/Ansible-Mark-RGB_White.png
--rw-r--r--   0 alex      (1000) alex      (1000)       90 2022-10-20 07:13:59.000000 ansible_rulebook-1.0.6/docs/_build/html/_static/minus.png
--rw-r--r--   0 alex      (1000) alex      (1000)       90 2022-10-20 07:13:59.000000 ansible_rulebook-1.0.6/docs/_build/html/_static/plus.png
--rw-r--r--   0 alex      (1000) alex      (1000)    15053 2023-12-12 09:58:57.000000 ansible_rulebook-1.0.6/docs/actions.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     2647 2023-06-05 18:56:04.000000 ansible_rulebook-1.0.6/docs/collections.rst
--rw-r--r--   0 alex      (1000) alex      (1000)    37135 2023-12-15 15:20:43.000000 ansible_rulebook-1.0.6/docs/conditions.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     5971 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.6/docs/conf.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2141 2024-01-24 12:42:11.000000 ansible_rulebook-1.0.6/docs/contributing.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     3923 2023-07-18 19:35:09.000000 ansible_rulebook-1.0.6/docs/decision_environment.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     3702 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/docs/development_environment.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     2033 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.6/docs/events_and_facts.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     2714 2024-03-11 14:25:59.000000 ansible_rulebook-1.0.6/docs/filters.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     7006 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.6/docs/getting_started.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      625 2024-03-11 14:25:59.000000 ansible_rulebook-1.0.6/docs/host_limit.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      495 2023-06-05 18:56:04.000000 ansible_rulebook-1.0.6/docs/index.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     2437 2024-01-24 12:42:11.000000 ansible_rulebook-1.0.6/docs/installation.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     5447 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/docs/introduction.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      778 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/docs/make.bat
--rw-r--r--   0 alex      (1000) alex      (1000)     2278 2023-01-16 11:17:52.000000 ansible_rulebook-1.0.6/docs/multi_events.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     5147 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/docs/rulebooks.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     2576 2023-09-26 14:04:44.000000 ansible_rulebook-1.0.6/docs/rules.rst
--rw-r--r--   0 alex      (1000) alex      (1000)       41 2023-01-13 09:14:28.000000 ansible_rulebook-1.0.6/docs/runner.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     8107 2024-02-05 12:43:06.000000 ansible_rulebook-1.0.6/docs/sources.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     5141 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/docs/usage.rst
--rw-r--r--   0 alex      (1000) alex      (1000)     4865 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/docs/variables.rst
--rw-r--r--   0 alex      (1000) alex      (1000)      269 2024-01-18 17:14:56.000000 ansible_rulebook-1.0.6/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)     1458 2024-03-12 12:28:14.842500 ansible_rulebook-1.0.6/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.771500 ansible_rulebook-1.0.6/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)      634 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.782500 ansible_rulebook-1.0.6/tests/asts/
--rw-r--r--   0 alex      (1000) alex      (1000)      516 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/01_noop.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      510 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/02_debug.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      522 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/03_print_event.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      888 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/04_set_fact.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      890 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/05_post_event.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1183 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/06_retract_fact.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      772 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/07_and.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      770 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/08_or.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      522 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/09_gt.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      516 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/10_lt.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      537 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/11_le.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      543 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/12_ge.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      662 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/13_add.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      670 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/14_sub.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      683 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/15_multiple_events_all.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      683 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/16_multiple_events_any.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      783 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/17_multiple_sources_any.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      787 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/18_multiple_sources_all.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1076 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/asts/19_is_defined.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1100 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/20_is_not_defined.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      561 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/21_run_playbook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      565 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/23_nested_data.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      563 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/24_max_attributes.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      604 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/25_max_attributes_nested.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      643 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/26_print_events.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1066 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/27_var_root.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      769 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/28_right_side_condition_template.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      621 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/29_run_module.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      619 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/30_run_module_missing.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      626 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/31_run_module_missing_args.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      641 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/32_run_module_fail.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      649 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/33_run_playbook_retry.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      625 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/34_run_playbook_retries.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1521 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1537 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1090 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/37_hosts_facts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      534 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.6/tests/asts/38_shutdown.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2990 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      694 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_assignment.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      693 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_assignment2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      924 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_multiple_conditions.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      925 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_multiple_conditions2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1441 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_multiple_conditions3.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1605 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_time.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2385 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_timestamp.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      916 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules_with_vars.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      580 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/rules_without_assignment.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1638 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/test_filters.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1963 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/test_host_rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1955 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/test_rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2022 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/test_rules_multiple_hosts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      530 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/test_rules_multiple_hosts2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      530 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/test_rules_multiple_hosts3.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1338 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.6/tests/asts/test_set_facts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1552 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/asts/test_simple.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2754 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/conftest.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.784500 ansible_rulebook-1.0.6/tests/data/
--rw-r--r--   0 alex      (1000) alex      (1000)     2008 2024-02-07 17:45:38.000000 ansible_rulebook-1.0.6/tests/data/awx_test_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)       37 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.6/tests/data/bad_source.py
--rw-r--r--   0 alex      (1000) alex      (1000)      137 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.6/tests/data/not_asyncio.py
--rw-r--r--   0 alex      (1000) alex      (1000)      727 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.6/tests/data/rulebook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)    47616 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.6/tests/data/test.tar
--rw-r--r--   0 alex      (1000) alex      (1000)       68 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.6/tests/data/test_vars.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.787500 ansible_rulebook-1.0.6/tests/e2e/
--rw-r--r--   0 alex      (1000) alex      (1000)      878 2023-02-13 17:29:00.000000 ansible_rulebook-1.0.6/tests/e2e/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/e2e/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.787500 ansible_rulebook-1.0.6/tests/e2e/config/
--rw-r--r--   0 alex      (1000) alex      (1000)      246 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/config/default.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      564 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.6/tests/e2e/conftest.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.752501 ansible_rulebook-1.0.6/tests/e2e/files/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.787500 ansible_rulebook-1.0.6/tests/e2e/files/extra_vars/
--rw-r--r--   0 alex      (1000) alex      (1000)      826 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.6/tests/e2e/files/extra_vars/operator_variables.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      162 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/extra_vars/test_variables_extra_vars.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.788500 ansible_rulebook-1.0.6/tests/e2e/files/inventories/
--rw-r--r--   0 alex      (1000) alex      (1000)       35 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.6/tests/e2e/files/inventories/default_inventory.ini
--rw-r--r--   0 alex      (1000) alex      (1000)       61 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/e2e/files/inventories/default_inventory.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.788500 ansible_rulebook-1.0.6/tests/e2e/files/playbooks/
--rw-r--r--   0 alex      (1000) alex      (1000)      404 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/playbooks/long_running.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      344 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/e2e/files/playbooks/print_event.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      240 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.6/tests/e2e/files/playbooks/print_rule_name.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1522 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.6/tests/e2e/files/playbooks/run_playbook_test_playbook.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.790500 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.791500 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/
--rw-r--r--   0 alex      (1000) alex      (1000)     4727 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2451 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_run_playbook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1611 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1050 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      288 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/hello_events_with_var.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      253 2023-01-12 10:03:30.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/malformed_rulebook.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.793500 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/
--rw-r--r--   0 alex      (1000) alex      (1000)     6613 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_logical_operators.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     6060 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_membership_operators.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     6216 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_relational_operators.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     3476 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_select_operator.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     8092 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2545 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_string_match.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2583 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     2623 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_string_search_search.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1394 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/test_disabled_rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      429 2024-01-18 17:50:10.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/test_hot_reload.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      303 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/test_match_multiple_rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      270 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/test_process_sigint.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      955 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/test_process_source_end.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.794500 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/variables/
--rw-r--r--   0 alex      (1000) alex      (1000)     2070 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.794500 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/websockets/
--rw-r--r--   0 alex      (1000) alex      (1000)      283 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/websockets/test_websocket_range.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      522 2023-02-13 17:29:00.000000 ansible_rulebook-1.0.6/tests/e2e/settings.py
--rw-r--r--   0 alex      (1000) alex      (1000)    11188 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/e2e/test_actions.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2689 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/e2e/test_match_multiple_rules.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3293 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/e2e/test_non_alpha_keys.py
--rw-r--r--   0 alex      (1000) alex      (1000)    20632 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/e2e/test_operators.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3115 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/e2e/test_run_module_output.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7400 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/e2e/test_runtime.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2251 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/e2e/test_skip_audit_events.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2271 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/e2e/test_variables.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3787 2024-01-29 21:36:46.000000 ansible_rulebook-1.0.6/tests/e2e/test_websocket.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.753501 ansible_rulebook-1.0.6/tests/e2e/utils/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.795500 ansible_rulebook-1.0.6/tests/e2e/utils/awx/
--rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/ansible.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.753501 ansible_rulebook-1.0.6/tests/e2e/utils/awx/artifacts/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.795500 ansible_rulebook-1.0.6/tests/e2e/utils/awx/artifacts/localhost/
--rw-r--r--   0 alex      (1000) alex      (1000)      219 2023-03-27 21:29:08.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/artifacts/localhost/awx.yaml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.795500 ansible_rulebook-1.0.6/tests/e2e/utils/awx/artifacts/localhost/kustomization/
--rw-r--r--   0 alex      (1000) alex      (1000)      406 2023-03-27 21:29:08.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/artifacts/localhost/kustomization/kustomization.yaml
--rw-r--r--   0 alex      (1000) alex      (1000)      602 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/create-cluster.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      637 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/install-awx.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      437 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/kind-config.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      855 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/readme.md
--rw-r--r--   0 alex      (1000) alex      (1000)       27 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/requirements.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.753501 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.753501 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.796500 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/defaults/
--rw-r--r--   0 alex      (1000) alex      (1000)      226 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/defaults/main.yaml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.796500 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/tasks/
--rw-r--r--   0 alex      (1000) alex      (1000)     1204 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.796500 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/templates/
--rw-r--r--   0 alex      (1000) alex      (1000)      162 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/templates/admin-password-secret.yml.j2
--rw-r--r--   0 alex      (1000) alex      (1000)      264 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/templates/awx.yaml.j2
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.797500 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/
--rw-r--r--   0 alex      (1000) alex      (1000)      464 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/kustomization.yaml.j2
--rw-r--r--   0 alex      (1000) alex      (1000)     4866 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/tests/e2e/utils.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.797500 ansible_rulebook-1.0.6/tests/event_filter/
--rw-r--r--   0 alex      (1000) alex      (1000)     1615 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.6/tests/event_filter/dashes_to_underscores.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1964 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.6/tests/event_filter/json_filter.py
--rw-r--r--   0 alex      (1000) alex      (1000)      691 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.6/tests/event_filter/noop.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1385 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.6/tests/event_filter/test_insert_meta_info.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.817500 ansible_rulebook-1.0.6/tests/examples/
--rw-r--r--   0 alex      (1000) alex      (1000)      182 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/01_noop.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      176 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/02_debug.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      188 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/03_print_event.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      324 2023-01-23 17:48:15.000000 ansible_rulebook-1.0.6/tests/examples/04_set_fact.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      326 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/05_post_event.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      458 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/06_retract_fact.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      210 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/07_and.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      208 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/08_or.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      165 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/09_gt.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      162 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/10_lt.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      175 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/11_le.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      178 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/12_ge.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      203 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/13_add.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      208 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/14_sub.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      259 2023-01-13 09:14:18.000000 ansible_rulebook-1.0.6/tests/examples/15_multiple_events_all.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      259 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/16_multiple_events_any.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      258 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/17_multiple_sources_any.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      262 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/18_multiple_sources_all.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      402 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/19_is_defined.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      431 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/20_is_not_defined.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      216 2022-11-29 16:59:01.000000 ansible_rulebook-1.0.6/tests/examples/21_run_playbook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      249 2022-11-17 11:07:48.000000 ansible_rulebook-1.0.6/tests/examples/22_run_playbook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      222 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/23_nested_data.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      220 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/24_max_attributes.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      261 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/25_max_attributes_nested.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      240 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/26_print_events.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      906 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/27_var_root.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      205 2023-02-10 11:45:34.000000 ansible_rulebook-1.0.6/tests/examples/28_right_side_condition_template.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      392 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/29_run_module.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      268 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/30_run_module_missing.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      275 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/31_run_module_missing_args.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      278 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/32_run_module_fail.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      359 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.6/tests/examples/33_run_playbook_retry.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      339 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.6/tests/examples/34_run_playbook_retries.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      575 2022-11-08 11:23:52.000000 ansible_rulebook-1.0.6/tests/examples/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      790 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      402 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/examples/37_hosts_facts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      299 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/examples/38_shutdown.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      206 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/39_is_defined.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      183 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/examples/40_in.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      193 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/examples/41_not_in.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      280 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/42_contains.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      288 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/43_not_contains.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      201 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/examples/44_in_and.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      199 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/examples/45_in_or.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      402 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.6/tests/examples/46_job_template.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      323 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/47_generic_plugin.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      206 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/examples/48_echo.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      457 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/49_float.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      672 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/50_negation.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1387 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/51_vars_namespace.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      660 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/52_once_within.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      671 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/53_once_within_multiple_hosts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      554 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/54_time_window.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      634 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/55_not_all.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      810 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/56_once_after.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1902 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/57_once_after_multi.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1465 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/58_string_search.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      444 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/examples/59_multiple_actions.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      725 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/60_json_filter.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      620 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/61_select_1.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      915 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/62_select_2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      950 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/63_selectattr_1.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      601 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/64_selectattr_2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      425 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/65_selectattr_3.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      905 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/66_sleepy_playbook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      859 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/67_shutdown_now.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      347 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/examples/68_disabled_rule.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      619 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/tests/examples/69_enhanced_debug.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      736 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/70_null.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1113 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/72_set_fact_with_type.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      886 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/73_mix_and_match_list.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/74_self_referential.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      550 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/75_all_conditions.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      748 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/76_all_conditions.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      497 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.6/tests/examples/77_default_events_ttl.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      592 2023-05-30 21:59:52.000000 ansible_rulebook-1.0.6/tests/examples/78_complete_retract_fact.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      422 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.6/tests/examples/79_workflow_template.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      301 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/80_match_multiple_rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      269 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/81_match_single_rule.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      658 2023-09-26 14:04:44.000000 ansible_rulebook-1.0.6/tests/examples/82_non_alpha_keys.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      183 2024-01-17 23:06:54.000000 ansible_rulebook-1.0.6/tests/examples/83_boolean_true.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.753501 ansible_rulebook-1.0.6/tests/examples/replays/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.819500 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/00.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/01.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/02.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/03.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/04.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/05.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/06.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/07.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/08.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/09.json
--rw-r--r--   0 alex      (1000) alex      (1000)      833 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/generate_data.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.820500 ansible_rulebook-1.0.6/tests/examples/replays/24_max_attributes/
--rw-r--r--   0 alex      (1000) alex      (1000)     5033 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/24_max_attributes/00.json
--rw-r--r--   0 alex      (1000) alex      (1000)      898 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/24_max_attributes/generate_data.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.820500 ansible_rulebook-1.0.6/tests/examples/replays/25_max_attributes_nested/
--rw-r--r--   0 alex      (1000) alex      (1000)     3792 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/examples/replays/25_max_attributes_nested/00.json
--rw-r--r--   0 alex      (1000) alex      (1000)     1107 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/25_max_attributes_nested/generate_data.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.823500 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/00.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/01.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/02.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/03.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/04.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/05.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/06.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/07.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/08.json
--rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/09.json
--rw-r--r--   0 alex      (1000) alex      (1000)      833 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/generate_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1696 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/generate_asts.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.825500 ansible_rulebook-1.0.6/tests/playbooks/
--rw-r--r--   0 alex      (1000) alex      (1000)      618 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/playbooks/check_facts_playbook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      370 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/playbooks/compare_value.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      829 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.6/tests/playbooks/fail_and_succeed.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      400 2023-02-17 18:46:04.000000 ansible_rulebook-1.0.6/tests/playbooks/hello.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      309 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/playbooks/hello_events.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      290 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/playbooks/hello_world_set_fact.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      129 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.6/tests/playbooks/inventory.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/playbooks/inventory1.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      260 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/playbooks/sleeper.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      704 2023-02-23 16:22:58.000000 ansible_rulebook-1.0.6/tests/playbooks/validate_args_playbook.yml
--rw-r--r--   0 alex      (1000) alex      (1000)       13 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/playbooks/vars.yml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.833500 ansible_rulebook-1.0.6/tests/rules/
--rw-r--r--   0 alex      (1000) alex      (1000)      300 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.6/tests/rules/rule_names_with_substitution.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1410 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      252 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_assignment.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      251 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_assignment2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      307 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_multiple_conditions.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      308 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_multiple_conditions2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      475 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_multiple_conditions3.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      741 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_time.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1070 2022-10-13 21:12:04.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_timestamp.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      281 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/rules_with_vars.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      244 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/rules_without_assignment.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      203 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/rules/test_blank_rule_name.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      171 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/rules/test_blank_ruleset_name.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      282 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/rules/test_combine_hosts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      329 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/rules/test_combine_hosts_module.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      286 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_duplicate_rule_names.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      348 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/rules/test_duplicate_ruleset_names.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      199 2022-10-13 20:51:42.000000 ansible_rulebook-1.0.6/tests/rules/test_empty_rule_names.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      618 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_filters.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      754 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_host_rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1463 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_kafka.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      189 2022-10-13 20:51:42.000000 ansible_rulebook-1.0.6/tests/rules/test_missing_rule_names.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      159 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.6/tests/rules/test_missing_ruleset_name.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      337 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/test_multiple_sources.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      746 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_rules.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      461 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/test_rules_expanded_conditions.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      813 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_rules_multiple_hosts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      195 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_rules_multiple_hosts2.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      195 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_rules_multiple_hosts3.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      244 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/test_rules_playbooks.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      728 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.6/tests/rules/test_set_facts.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      587 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_simple.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      985 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.6/tests/rules/test_states.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      944 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.6/tests/rules/webserver_down.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      275 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/run_examples.sh
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.836500 ansible_rulebook-1.0.6/tests/sources/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2022-11-17 11:54:27.000000 ansible_rulebook-1.0.6/tests/sources/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2613 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/sources/file.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4945 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.6/tests/sources/generic.py
--rw-r--r--   0 alex      (1000) alex      (1000)      963 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.6/tests/sources/hosts.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1613 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/sources/infrange.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2841 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/sources/log_scraper.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1258 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.6/tests/sources/nested.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1210 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/sources/ping.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/sources/process_check.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1026 2024-01-17 23:03:29.000000 ansible_rulebook-1.0.6/tests/sources/range.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1014 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/sources/range2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1578 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/sources/replay.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.837500 ansible_rulebook-1.0.6/tests/sources/replays/
--rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/sources/replays/01.json
--rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/sources/replays/02.json
--rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/sources/replays/03.json
--rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/sources/replays/04.json
--rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.6/tests/sources/replays/05.json
--rw-r--r--   0 alex      (1000) alex      (1000)     1224 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/sources/template.py
--rw-r--r--   0 alex      (1000) alex      (1000)      891 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.6/tests/sources/tick.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1024 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/sources/timestamp.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1908 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/sources/url_check.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1120 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.6/tests/test_ansible_events.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6053 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/test_app.py
--rw-r--r--   0 alex      (1000) alex      (1000)    20803 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/test_ast.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2206 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/tests/test_collection.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9128 2024-02-07 17:45:38.000000 ansible_rulebook-1.0.6/tests/test_controller.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16132 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/test_engine.py
--rw-r--r--   0 alex      (1000) alex      (1000)    71559 2024-02-05 12:43:06.000000 ansible_rulebook-1.0.6/tests/test_examples.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8114 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/test_rules.py
--rw-r--r--   0 alex      (1000) alex      (1000)      576 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/tests/test_simple.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1851 2024-03-11 14:29:05.000000 ansible_rulebook-1.0.6/tests/test_token.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6205 2024-01-29 21:36:46.000000 ansible_rulebook-1.0.6/tests/test_websocket.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.837500 ansible_rulebook-1.0.6/tests/unit/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.840500 ansible_rulebook-1.0.6/tests/unit/action/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/tests/unit/action/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      599 2023-12-12 09:58:57.000000 ansible_rulebook-1.0.6/tests/unit/action/conftest.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-12 12:28:14.841500 ansible_rulebook-1.0.6/tests/unit/action/playbooks/
--rw-r--r--   0 alex      (1000) alex      (1000)      249 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/tests/unit/action/playbooks/fail.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      459 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/tests/unit/action/playbooks/rule_name.yml
--rw-r--r--   0 alex      (1000) alex      (1000)     1603 2023-12-12 09:58:57.000000 ansible_rulebook-1.0.6/tests/unit/action/test_controller.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5122 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/action/test_debug.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2954 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/tests/unit/action/test_noop.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3262 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/unit/action/test_post_event.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4930 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/action/test_print_event.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3561 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.6/tests/unit/action/test_retract_fact.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7273 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/action/test_run_job_template.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3299 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.6/tests/unit/action/test_run_module.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6265 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/action/test_run_playbook.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7462 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/action/test_run_workflow_template.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3201 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/action/test_set_fact.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3116 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/action/test_shutdown.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3050 2023-07-28 10:10:50.000000 ansible_rulebook-1.0.6/tests/unit/test_cli.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3323 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.6/tests/unit/test_terminal.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1147 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.6/tests/unit/test_util.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.479470 ansible_rulebook-1.0.7/
+-rw-r--r--   0 alex      (1000) alex      (1000)    11358 2022-07-11 07:18:31.000000 ansible_rulebook-1.0.7/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      312 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     4324 2024-05-15 14:39:53.479470 ansible_rulebook-1.0.7/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     3353 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.7/README.rst
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.442470 ansible_rulebook-1.0.7/ansible_rulebook/
+-rw-r--r--   0 alex      (1000) alex      (1000)      655 2024-05-15 14:38:06.000000 ansible_rulebook-1.0.7/ansible_rulebook/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      634 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/ansible_rulebook/__main__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.444471 ansible_rulebook-1.0.7/ansible_rulebook/action/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1853 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/control.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2875 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/debug.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5450 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/helper.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1271 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/metadata.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1151 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/noop.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1555 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/post_event.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1532 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/print_event.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1891 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/retract_fact.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6316 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/run_job_template.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2397 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/run_module.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10326 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/run_playbook.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6490 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/run_workflow_template.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3906 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/runner.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1691 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/set_fact.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2154 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/action/shutdown.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9389 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/app.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10697 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/cli.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4775 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/collection.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1136 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/common.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8512 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/ansible_rulebook/condition_parser.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2659 2023-02-23 16:22:58.000000 ansible_rulebook-1.0.7/ansible_rulebook/condition_types.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1110 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/conf.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11493 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/engine.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.444471 ansible_rulebook-1.0.7/ansible_rulebook/event_filter/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.7/ansible_rulebook/event_filter/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1346 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.7/ansible_rulebook/event_filter/insert_meta_info.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2494 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/exception.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7860 2024-03-15 13:55:25.000000 ansible_rulebook-1.0.7/ansible_rulebook/job_template_runner.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    12203 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/json_generator.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      827 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/ansible_rulebook/messages.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3183 2023-11-30 12:34:41.000000 ansible_rulebook-1.0.7/ansible_rulebook/rule_generator.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    19689 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/rule_set_runner.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2457 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/ansible_rulebook/rule_types.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6797 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/rules_parser.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.444471 ansible_rulebook-1.0.7/ansible_rulebook/schema/
+-rw-r--r--   0 alex      (1000) alex      (1000)    22926 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/schema/ruleset_schema.json
+-rw-r--r--   0 alex      (1000) alex      (1000)     5486 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/ansible_rulebook/terminal.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1836 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/token.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8118 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/util.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1428 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/ansible_rulebook/validators.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8137 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/ansible_rulebook/websocket.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.478470 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     4324 2024-05-15 14:39:53.000000 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)    14555 2024-05-15 14:39:53.000000 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-05-15 14:39:53.000000 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       63 2024-05-15 14:39:53.000000 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-05-15 14:39:53.000000 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/not-zip-safe
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2024-05-15 14:39:53.000000 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       17 2024-05-15 14:39:53.000000 ansible_rulebook-1.0.7/ansible_rulebook.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.446471 ansible_rulebook-1.0.7/docs/
+-rw-r--r--   0 alex      (1000) alex      (1000)      617 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/docs/Makefile
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.437471 ansible_rulebook-1.0.7/docs/_build/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.437471 ansible_rulebook-1.0.7/docs/_build/html/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.447471 ansible_rulebook-1.0.7/docs/_build/html/_static/
+-rw-r--r--   0 alex      (1000) alex      (1000)      286 2024-01-18 17:46:51.000000 ansible_rulebook-1.0.7/docs/_build/html/_static/file.png
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.447471 ansible_rulebook-1.0.7/docs/_build/html/_static/images/
+-rw-r--r--   0 alex      (1000) alex      (1000)     8664 2024-01-18 17:47:13.000000 ansible_rulebook-1.0.7/docs/_build/html/_static/images/Ansible-Mark-RGB_Black.png
+-rw-r--r--   0 alex      (1000) alex      (1000)     5173 2024-01-18 17:47:13.000000 ansible_rulebook-1.0.7/docs/_build/html/_static/images/Ansible-Mark-RGB_White.png
+-rw-r--r--   0 alex      (1000) alex      (1000)       90 2024-01-18 17:46:51.000000 ansible_rulebook-1.0.7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 alex      (1000) alex      (1000)       90 2024-01-18 17:46:51.000000 ansible_rulebook-1.0.7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 alex      (1000) alex      (1000)    15053 2023-12-12 09:58:57.000000 ansible_rulebook-1.0.7/docs/actions.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2647 2023-06-05 18:56:04.000000 ansible_rulebook-1.0.7/docs/collections.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)    37135 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/conditions.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     5971 2023-06-22 15:56:59.000000 ansible_rulebook-1.0.7/docs/conf.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2141 2024-04-22 19:07:36.000000 ansible_rulebook-1.0.7/docs/contributing.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     3923 2023-07-18 19:35:09.000000 ansible_rulebook-1.0.7/docs/decision_environment.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     3702 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/development_environment.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2033 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.7/docs/events_and_facts.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2714 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/filters.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     7006 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.7/docs/getting_started.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      625 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/host_limit.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      495 2023-06-05 18:56:04.000000 ansible_rulebook-1.0.7/docs/index.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2437 2024-04-22 19:07:36.000000 ansible_rulebook-1.0.7/docs/installation.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     5447 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/introduction.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      778 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/docs/make.bat
+-rw-r--r--   0 alex      (1000) alex      (1000)     2278 2023-01-16 11:17:52.000000 ansible_rulebook-1.0.7/docs/multi_events.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     5147 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/rulebooks.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     2576 2023-09-26 14:04:44.000000 ansible_rulebook-1.0.7/docs/rules.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)       41 2023-01-13 09:14:28.000000 ansible_rulebook-1.0.7/docs/runner.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     8107 2024-02-05 12:43:06.000000 ansible_rulebook-1.0.7/docs/sources.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     5141 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/usage.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)     4865 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/docs/variables.rst
+-rw-r--r--   0 alex      (1000) alex      (1000)      269 2024-01-18 17:14:56.000000 ansible_rulebook-1.0.7/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1458 2024-05-15 14:39:53.479470 ansible_rulebook-1.0.7/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.449470 ansible_rulebook-1.0.7/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)      634 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.454470 ansible_rulebook-1.0.7/tests/asts/
+-rw-r--r--   0 alex      (1000) alex      (1000)      516 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/01_noop.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      510 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/02_debug.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      522 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/03_print_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      888 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/04_set_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      890 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/05_post_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1183 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/06_retract_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      772 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/07_and.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      770 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/08_or.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      522 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/09_gt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      516 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/10_lt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      537 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/11_le.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      543 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/12_ge.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      662 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/13_add.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      670 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/14_sub.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      683 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/15_multiple_events_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      683 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/16_multiple_events_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      783 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/17_multiple_sources_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      787 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/18_multiple_sources_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1076 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/asts/19_is_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1100 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/20_is_not_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      561 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/21_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      565 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/23_nested_data.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      563 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/24_max_attributes.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      604 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/25_max_attributes_nested.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      643 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/26_print_events.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1066 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/27_var_root.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      769 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/28_right_side_condition_template.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      621 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/29_run_module.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      619 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/30_run_module_missing.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      626 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/31_run_module_missing_args.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      641 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/32_run_module_fail.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      649 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/33_run_playbook_retry.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      625 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/34_run_playbook_retries.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1521 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1537 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1090 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/37_hosts_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      534 2022-10-18 10:19:58.000000 ansible_rulebook-1.0.7/tests/asts/38_shutdown.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2990 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      694 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      693 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_assignment2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      924 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_multiple_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      925 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1441 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1605 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_time.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2385 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_timestamp.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      916 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules_with_vars.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      580 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/rules_without_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1638 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/test_filters.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1963 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/test_host_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1955 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/test_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2022 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/test_rules_multiple_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      530 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      530 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1338 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.7/tests/asts/test_set_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1552 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/asts/test_simple.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2754 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/conftest.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.455470 ansible_rulebook-1.0.7/tests/data/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2008 2024-03-15 13:55:25.000000 ansible_rulebook-1.0.7/tests/data/awx_test_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       37 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.7/tests/data/bad_source.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      137 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.7/tests/data/not_asyncio.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      727 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.7/tests/data/rulebook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)    47616 2023-03-13 17:20:20.000000 ansible_rulebook-1.0.7/tests/data/test.tar
+-rw-r--r--   0 alex      (1000) alex      (1000)       68 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.7/tests/data/test_vars.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.456470 ansible_rulebook-1.0.7/tests/e2e/
+-rw-r--r--   0 alex      (1000) alex      (1000)      878 2023-02-13 17:29:00.000000 ansible_rulebook-1.0.7/tests/e2e/README.md
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/e2e/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.456470 ansible_rulebook-1.0.7/tests/e2e/config/
+-rw-r--r--   0 alex      (1000) alex      (1000)      246 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/config/default.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      564 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.7/tests/e2e/conftest.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.437471 ansible_rulebook-1.0.7/tests/e2e/files/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.456470 ansible_rulebook-1.0.7/tests/e2e/files/extra_vars/
+-rw-r--r--   0 alex      (1000) alex      (1000)      826 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.7/tests/e2e/files/extra_vars/operator_variables.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      162 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/extra_vars/test_variables_extra_vars.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.457471 ansible_rulebook-1.0.7/tests/e2e/files/inventories/
+-rw-r--r--   0 alex      (1000) alex      (1000)       35 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.7/tests/e2e/files/inventories/default_inventory.ini
+-rw-r--r--   0 alex      (1000) alex      (1000)       61 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/e2e/files/inventories/default_inventory.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.457471 ansible_rulebook-1.0.7/tests/e2e/files/playbooks/
+-rw-r--r--   0 alex      (1000) alex      (1000)      404 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/playbooks/long_running.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      344 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/e2e/files/playbooks/print_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      240 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.7/tests/e2e/files/playbooks/print_rule_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1522 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.7/tests/e2e/files/playbooks/run_playbook_test_playbook.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.458470 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.458470 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/
+-rw-r--r--   0 alex      (1000) alex      (1000)     4727 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2451 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1611 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1050 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      288 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/hello_events_with_var.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      253 2023-01-12 10:03:30.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/malformed_rulebook.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.459470 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6613 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_logical_operators.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     6060 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_membership_operators.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     6216 2023-03-09 21:28:22.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_relational_operators.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     3476 2023-04-18 09:33:50.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_select_operator.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     8092 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2545 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_string_match.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2583 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     2623 2023-02-23 17:58:50.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_string_search_search.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1394 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/test_disabled_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      429 2024-01-18 17:50:10.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/test_hot_reload.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      303 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/test_match_multiple_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      270 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/test_process_sigint.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      955 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/test_process_source_end.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.459470 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/variables/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2070 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.459470 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/websockets/
+-rw-r--r--   0 alex      (1000) alex      (1000)      283 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/websockets/test_websocket_range.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      522 2023-02-13 17:29:00.000000 ansible_rulebook-1.0.7/tests/e2e/settings.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11188 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/e2e/test_actions.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2689 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/e2e/test_match_multiple_rules.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3293 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/e2e/test_non_alpha_keys.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    20632 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/e2e/test_operators.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3115 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/e2e/test_run_module_output.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7400 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/e2e/test_runtime.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2251 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/e2e/test_skip_audit_events.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2271 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/e2e/test_variables.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3787 2024-01-29 21:36:46.000000 ansible_rulebook-1.0.7/tests/e2e/test_websocket.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.438470 ansible_rulebook-1.0.7/tests/e2e/utils/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.459470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/
+-rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/ansible.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.438470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/artifacts/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.460470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/artifacts/localhost/
+-rw-r--r--   0 alex      (1000) alex      (1000)      219 2023-03-27 21:29:08.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/artifacts/localhost/awx.yaml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.460470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/artifacts/localhost/kustomization/
+-rw-r--r--   0 alex      (1000) alex      (1000)      406 2023-03-27 21:29:08.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/artifacts/localhost/kustomization/kustomization.yaml
+-rw-r--r--   0 alex      (1000) alex      (1000)      602 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/create-cluster.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      637 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/install-awx.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      437 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/kind-config.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      855 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/readme.md
+-rw-r--r--   0 alex      (1000) alex      (1000)       27 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/requirements.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.438470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.438470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.460470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/defaults/
+-rw-r--r--   0 alex      (1000) alex      (1000)      226 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/defaults/main.yaml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.460470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/tasks/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1204 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.460470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/templates/
+-rw-r--r--   0 alex      (1000) alex      (1000)      162 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/templates/admin-password-secret.yml.j2
+-rw-r--r--   0 alex      (1000) alex      (1000)      264 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/templates/awx.yaml.j2
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.460470 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/
+-rw-r--r--   0 alex      (1000) alex      (1000)      464 2023-04-10 16:23:06.000000 ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/templates/kustomization/kustomization.yaml.j2
+-rw-r--r--   0 alex      (1000) alex      (1000)     4866 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/e2e/utils.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.460470 ansible_rulebook-1.0.7/tests/event_filter/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1615 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.7/tests/event_filter/dashes_to_underscores.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1964 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.7/tests/event_filter/json_filter.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      691 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.7/tests/event_filter/noop.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1385 2023-04-25 19:09:45.000000 ansible_rulebook-1.0.7/tests/event_filter/test_insert_meta_info.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.468470 ansible_rulebook-1.0.7/tests/examples/
+-rw-r--r--   0 alex      (1000) alex      (1000)      182 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/01_noop.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      176 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/02_debug.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      188 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/03_print_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      324 2023-01-23 17:48:15.000000 ansible_rulebook-1.0.7/tests/examples/04_set_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      326 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/05_post_event.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      458 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/06_retract_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      210 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/07_and.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      208 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/08_or.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      165 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/09_gt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      162 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/10_lt.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      175 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/11_le.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      178 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/12_ge.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      203 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/13_add.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      208 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/14_sub.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      259 2023-01-13 09:14:18.000000 ansible_rulebook-1.0.7/tests/examples/15_multiple_events_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      259 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/16_multiple_events_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      258 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/17_multiple_sources_any.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      262 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/18_multiple_sources_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      402 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/19_is_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      431 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/20_is_not_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      216 2022-11-29 16:59:01.000000 ansible_rulebook-1.0.7/tests/examples/21_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      249 2022-11-17 11:07:48.000000 ansible_rulebook-1.0.7/tests/examples/22_run_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      222 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/23_nested_data.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      220 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/24_max_attributes.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      261 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/25_max_attributes_nested.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      240 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/26_print_events.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      906 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/27_var_root.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      205 2023-02-10 11:45:34.000000 ansible_rulebook-1.0.7/tests/examples/28_right_side_condition_template.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      392 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/29_run_module.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      268 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/30_run_module_missing.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      275 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/31_run_module_missing_args.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      278 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/32_run_module_fail.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      359 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.7/tests/examples/33_run_playbook_retry.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      339 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.7/tests/examples/34_run_playbook_retries.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      575 2022-11-08 11:23:52.000000 ansible_rulebook-1.0.7/tests/examples/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      790 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      402 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/examples/37_hosts_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      299 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/examples/38_shutdown.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      206 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/39_is_defined.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      183 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/examples/40_in.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      193 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/examples/41_not_in.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      280 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/42_contains.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      288 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/43_not_contains.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      201 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/examples/44_in_and.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      199 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/examples/45_in_or.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      402 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.7/tests/examples/46_job_template.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      323 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/47_generic_plugin.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      206 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/examples/48_echo.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      457 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/49_float.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      672 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/50_negation.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1387 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/51_vars_namespace.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      660 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/52_once_within.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      671 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/53_once_within_multiple_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      554 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/54_time_window.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      634 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/55_not_all.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      810 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/56_once_after.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1902 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/57_once_after_multi.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1465 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/58_string_search.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      444 2023-03-31 11:28:05.000000 ansible_rulebook-1.0.7/tests/examples/59_multiple_actions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      725 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/60_json_filter.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      620 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/61_select_1.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      915 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/62_select_2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      950 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/63_selectattr_1.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      601 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/64_selectattr_2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      425 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/65_selectattr_3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      905 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/66_sleepy_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      859 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/67_shutdown_now.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      347 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/examples/68_disabled_rule.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      619 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/tests/examples/69_enhanced_debug.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      736 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/70_null.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1113 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/72_set_fact_with_type.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      886 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/73_mix_and_match_list.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/74_self_referential.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      550 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/75_all_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      748 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/76_all_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      497 2023-08-21 10:42:02.000000 ansible_rulebook-1.0.7/tests/examples/77_default_events_ttl.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      592 2023-05-30 21:59:52.000000 ansible_rulebook-1.0.7/tests/examples/78_complete_retract_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      422 2023-08-09 08:47:09.000000 ansible_rulebook-1.0.7/tests/examples/79_workflow_template.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      301 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/80_match_multiple_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      269 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/81_match_single_rule.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      658 2023-09-26 14:04:44.000000 ansible_rulebook-1.0.7/tests/examples/82_non_alpha_keys.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      183 2024-01-17 23:06:54.000000 ansible_rulebook-1.0.7/tests/examples/83_boolean_true.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.439471 ansible_rulebook-1.0.7/tests/examples/replays/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.469470 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-08-02 08:07:43.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/01.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/02.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/03.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/04.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/05.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/06.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/07.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/08.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/09.json
+-rw-r--r--   0 alex      (1000) alex      (1000)      833 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/generate_data.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.469470 ansible_rulebook-1.0.7/tests/examples/replays/24_max_attributes/
+-rw-r--r--   0 alex      (1000) alex      (1000)     5033 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/24_max_attributes/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)      898 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/24_max_attributes/generate_data.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.469470 ansible_rulebook-1.0.7/tests/examples/replays/25_max_attributes_nested/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3792 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/examples/replays/25_max_attributes_nested/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)     1107 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/25_max_attributes_nested/generate_data.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.470470 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/00.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/01.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/02.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/03.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/04.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/05.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/06.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/07.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/08.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       73 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/09.json
+-rw-r--r--   0 alex      (1000) alex      (1000)      833 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/generate_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1696 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/generate_asts.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.472470 ansible_rulebook-1.0.7/tests/playbooks/
+-rw-r--r--   0 alex      (1000) alex      (1000)      618 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/playbooks/check_facts_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      370 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/playbooks/compare_value.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      829 2023-05-25 18:22:55.000000 ansible_rulebook-1.0.7/tests/playbooks/fail_and_succeed.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      400 2023-02-17 18:46:04.000000 ansible_rulebook-1.0.7/tests/playbooks/hello.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      309 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/playbooks/hello_events.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      290 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/playbooks/hello_world_set_fact.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      129 2023-02-15 09:00:47.000000 ansible_rulebook-1.0.7/tests/playbooks/inventory.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/playbooks/inventory1.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      260 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/playbooks/sleeper.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      704 2023-02-23 16:22:58.000000 ansible_rulebook-1.0.7/tests/playbooks/validate_args_playbook.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)       13 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/playbooks/vars.yml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.475470 ansible_rulebook-1.0.7/tests/rules/
+-rw-r--r--   0 alex      (1000) alex      (1000)      300 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.7/tests/rules/rule_names_with_substitution.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1410 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      252 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      251 2023-02-22 09:24:10.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_assignment2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      307 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_multiple_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      308 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      475 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      741 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_time.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1070 2022-10-13 21:12:04.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_timestamp.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      281 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/rules_with_vars.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      244 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/rules_without_assignment.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      203 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/rules/test_blank_rule_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      171 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/rules/test_blank_ruleset_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      282 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/rules/test_combine_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      329 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/rules/test_combine_hosts_module.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      286 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_duplicate_rule_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      348 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/rules/test_duplicate_ruleset_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      199 2022-10-13 20:51:42.000000 ansible_rulebook-1.0.7/tests/rules/test_empty_rule_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      618 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_filters.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      754 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_host_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1463 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_kafka.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      189 2022-10-13 20:51:42.000000 ansible_rulebook-1.0.7/tests/rules/test_missing_rule_names.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      159 2023-02-10 11:45:23.000000 ansible_rulebook-1.0.7/tests/rules/test_missing_ruleset_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      337 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/test_multiple_sources.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      746 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_rules.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      461 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/test_rules_expanded_conditions.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      813 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_rules_multiple_hosts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      195 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      195 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      244 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/test_rules_playbooks.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      728 2023-02-17 17:05:14.000000 ansible_rulebook-1.0.7/tests/rules/test_set_facts.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      587 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_simple.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      985 2022-10-13 09:57:55.000000 ansible_rulebook-1.0.7/tests/rules/test_states.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      944 2022-08-05 10:45:58.000000 ansible_rulebook-1.0.7/tests/rules/webserver_down.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      275 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/run_examples.sh
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.476470 ansible_rulebook-1.0.7/tests/sources/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2022-11-17 11:54:27.000000 ansible_rulebook-1.0.7/tests/sources/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2613 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/sources/file.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4945 2023-03-01 10:31:11.000000 ansible_rulebook-1.0.7/tests/sources/generic.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      963 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.7/tests/sources/hosts.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1613 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/sources/infrange.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2841 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/sources/log_scraper.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1258 2023-01-11 09:45:44.000000 ansible_rulebook-1.0.7/tests/sources/nested.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1210 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/sources/ping.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/sources/process_check.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1026 2024-01-17 23:03:29.000000 ansible_rulebook-1.0.7/tests/sources/range.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1014 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/sources/range2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1578 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/sources/replay.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.476470 ansible_rulebook-1.0.7/tests/sources/replays/
+-rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/sources/replays/01.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/sources/replays/02.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/sources/replays/03.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/sources/replays/04.json
+-rw-r--r--   0 alex      (1000) alex      (1000)       15 2023-08-28 19:03:25.000000 ansible_rulebook-1.0.7/tests/sources/replays/05.json
+-rw-r--r--   0 alex      (1000) alex      (1000)     1224 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/sources/template.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      891 2023-03-08 18:26:26.000000 ansible_rulebook-1.0.7/tests/sources/tick.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1024 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/sources/timestamp.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1908 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/sources/url_check.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1120 2022-12-13 15:51:52.000000 ansible_rulebook-1.0.7/tests/test_ansible_events.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6053 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/test_app.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    20803 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/test_ast.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2206 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/test_collection.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9128 2024-03-15 13:55:25.000000 ansible_rulebook-1.0.7/tests/test_controller.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16132 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/test_engine.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    71559 2024-02-05 12:43:06.000000 ansible_rulebook-1.0.7/tests/test_examples.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8114 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/test_rules.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      576 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/test_simple.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1851 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/test_token.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6205 2024-01-29 21:36:46.000000 ansible_rulebook-1.0.7/tests/test_websocket.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.477470 ansible_rulebook-1.0.7/tests/unit/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.478470 ansible_rulebook-1.0.7/tests/unit/action/
+-rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/tests/unit/action/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      599 2023-12-12 09:58:57.000000 ansible_rulebook-1.0.7/tests/unit/action/conftest.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-15 14:39:53.478470 ansible_rulebook-1.0.7/tests/unit/action/playbooks/
+-rw-r--r--   0 alex      (1000) alex      (1000)      249 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/tests/unit/action/playbooks/fail.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)      459 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/tests/unit/action/playbooks/rule_name.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1603 2023-12-12 09:58:57.000000 ansible_rulebook-1.0.7/tests/unit/action/test_controller.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5122 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/action/test_debug.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2954 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/tests/unit/action/test_noop.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3262 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/unit/action/test_post_event.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4930 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/action/test_print_event.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3561 2023-10-30 10:24:52.000000 ansible_rulebook-1.0.7/tests/unit/action/test_retract_fact.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7273 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/action/test_run_job_template.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3299 2023-10-16 10:39:40.000000 ansible_rulebook-1.0.7/tests/unit/action/test_run_module.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6265 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/action/test_run_playbook.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     7462 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/action/test_run_workflow_template.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3201 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/action/test_set_fact.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3116 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/action/test_shutdown.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3050 2023-07-28 10:10:50.000000 ansible_rulebook-1.0.7/tests/unit/test_cli.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3323 2024-01-12 19:09:05.000000 ansible_rulebook-1.0.7/tests/unit/test_terminal.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1147 2024-05-15 14:37:38.000000 ansible_rulebook-1.0.7/tests/unit/test_util.py
```

### Comparing `ansible_rulebook-1.0.6/LICENSE` & `ansible_rulebook-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/PKG-INFO` & `ansible_rulebook-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible_rulebook
-Version: 1.0.6
+Version: 1.0.7
 Summary: Event driven automation for Ansible
 Home-page: https://github.com/ansible/ansible-rulebook
 License: Apache-2.0
 Keywords: ansible_rulebook
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ansible_rulebook-1.0.6/README.rst` & `ansible_rulebook-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/__init__.py` & `ansible_rulebook-1.0.7/ansible_rulebook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Top-level package for Ansible Events."""
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
```

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/__main__.py` & `ansible_rulebook-1.0.7/ansible_rulebook/__main__.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/control.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/control.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/debug.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/debug.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/helper.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/helper.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/metadata.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/metadata.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/noop.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/noop.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/post_event.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/post_event.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/print_event.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/print_event.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/retract_fact.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/retract_fact.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/run_job_template.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/run_job_template.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/run_module.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/run_module.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/run_playbook.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/run_playbook.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/run_workflow_template.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/run_workflow_template.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/runner.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/runner.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/set_fact.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/action/shutdown.py` & `ansible_rulebook-1.0.7/ansible_rulebook/action/shutdown.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/app.py` & `ansible_rulebook-1.0.7/ansible_rulebook/app.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/cli.py` & `ansible_rulebook-1.0.7/ansible_rulebook/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/collection.py` & `ansible_rulebook-1.0.7/ansible_rulebook/collection.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/common.py` & `ansible_rulebook-1.0.7/ansible_rulebook/common.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/condition_parser.py` & `ansible_rulebook-1.0.7/ansible_rulebook/condition_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/condition_types.py` & `ansible_rulebook-1.0.7/ansible_rulebook/condition_types.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/conf.py` & `ansible_rulebook-1.0.7/ansible_rulebook/conf.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/engine.py` & `ansible_rulebook-1.0.7/ansible_rulebook/engine.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/event_filter/insert_meta_info.py` & `ansible_rulebook-1.0.7/ansible_rulebook/event_filter/insert_meta_info.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/exception.py` & `ansible_rulebook-1.0.7/ansible_rulebook/exception.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/job_template_runner.py` & `ansible_rulebook-1.0.7/ansible_rulebook/job_template_runner.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/json_generator.py` & `ansible_rulebook-1.0.7/ansible_rulebook/json_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/messages.py` & `ansible_rulebook-1.0.7/ansible_rulebook/messages.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/rule_generator.py` & `ansible_rulebook-1.0.7/ansible_rulebook/rule_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/rule_set_runner.py` & `ansible_rulebook-1.0.7/ansible_rulebook/rule_set_runner.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/rule_types.py` & `ansible_rulebook-1.0.7/ansible_rulebook/rule_types.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/rules_parser.py` & `ansible_rulebook-1.0.7/ansible_rulebook/rules_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/schema/ruleset_schema.json` & `ansible_rulebook-1.0.7/ansible_rulebook/schema/ruleset_schema.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/terminal.py` & `ansible_rulebook-1.0.7/ansible_rulebook/terminal.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/token.py` & `ansible_rulebook-1.0.7/ansible_rulebook/token.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/util.py` & `ansible_rulebook-1.0.7/ansible_rulebook/util.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/validators.py` & `ansible_rulebook-1.0.7/ansible_rulebook/validators.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook/websocket.py` & `ansible_rulebook-1.0.7/ansible_rulebook/websocket.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook.egg-info/PKG-INFO` & `ansible_rulebook-1.0.7/ansible_rulebook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible_rulebook
-Version: 1.0.6
+Version: 1.0.7
 Summary: Event driven automation for Ansible
 Home-page: https://github.com/ansible/ansible-rulebook
 License: Apache-2.0
 Keywords: ansible_rulebook
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ansible_rulebook-1.0.6/ansible_rulebook.egg-info/SOURCES.txt` & `ansible_rulebook-1.0.7/ansible_rulebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/Makefile` & `ansible_rulebook-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/_build/html/_static/images/Ansible-Mark-RGB_Black.png` & `ansible_rulebook-1.0.7/docs/_build/html/_static/images/Ansible-Mark-RGB_Black.png`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/_build/html/_static/images/Ansible-Mark-RGB_White.png` & `ansible_rulebook-1.0.7/docs/_build/html/_static/images/Ansible-Mark-RGB_White.png`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/actions.rst` & `ansible_rulebook-1.0.7/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/collections.rst` & `ansible_rulebook-1.0.7/docs/collections.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/conditions.rst` & `ansible_rulebook-1.0.7/docs/conditions.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/conf.py` & `ansible_rulebook-1.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/contributing.rst` & `ansible_rulebook-1.0.7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/decision_environment.rst` & `ansible_rulebook-1.0.7/docs/decision_environment.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/development_environment.rst` & `ansible_rulebook-1.0.7/docs/development_environment.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/events_and_facts.rst` & `ansible_rulebook-1.0.7/docs/events_and_facts.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/filters.rst` & `ansible_rulebook-1.0.7/docs/filters.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/getting_started.rst` & `ansible_rulebook-1.0.7/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/host_limit.rst` & `ansible_rulebook-1.0.7/docs/host_limit.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/installation.rst` & `ansible_rulebook-1.0.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/introduction.rst` & `ansible_rulebook-1.0.7/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/make.bat` & `ansible_rulebook-1.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/multi_events.rst` & `ansible_rulebook-1.0.7/docs/multi_events.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/rulebooks.rst` & `ansible_rulebook-1.0.7/docs/rulebooks.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/rules.rst` & `ansible_rulebook-1.0.7/docs/rules.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/sources.rst` & `ansible_rulebook-1.0.7/docs/sources.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/usage.rst` & `ansible_rulebook-1.0.7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/docs/variables.rst` & `ansible_rulebook-1.0.7/docs/variables.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/setup.cfg` & `ansible_rulebook-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible_rulebook
-version = 1.0.6
+version = 1.0.7
 description = Event driven automation for Ansible
 url = https://github.com/ansible/ansible-rulebook
 license = Apache-2.0
 keywords = ansible_rulebook
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 classifiers =
```

### Comparing `ansible_rulebook-1.0.6/tests/__init__.py` & `ansible_rulebook-1.0.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/01_noop.yml` & `ansible_rulebook-1.0.7/tests/asts/01_noop.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/03_print_event.yml` & `ansible_rulebook-1.0.7/tests/asts/03_print_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/04_set_fact.yml` & `ansible_rulebook-1.0.7/tests/asts/04_set_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/05_post_event.yml` & `ansible_rulebook-1.0.7/tests/asts/05_post_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/06_retract_fact.yml` & `ansible_rulebook-1.0.7/tests/asts/06_retract_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/07_and.yml` & `ansible_rulebook-1.0.7/tests/asts/07_and.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/08_or.yml` & `ansible_rulebook-1.0.7/tests/asts/08_or.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/09_gt.yml` & `ansible_rulebook-1.0.7/tests/asts/09_gt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/10_lt.yml` & `ansible_rulebook-1.0.7/tests/asts/10_lt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/11_le.yml` & `ansible_rulebook-1.0.7/tests/asts/11_le.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/12_ge.yml` & `ansible_rulebook-1.0.7/tests/asts/12_ge.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/13_add.yml` & `ansible_rulebook-1.0.7/tests/asts/13_add.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/14_sub.yml` & `ansible_rulebook-1.0.7/tests/asts/14_sub.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/15_multiple_events_all.yml` & `ansible_rulebook-1.0.7/tests/asts/15_multiple_events_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/16_multiple_events_any.yml` & `ansible_rulebook-1.0.7/tests/asts/16_multiple_events_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/17_multiple_sources_any.yml` & `ansible_rulebook-1.0.7/tests/asts/17_multiple_sources_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/18_multiple_sources_all.yml` & `ansible_rulebook-1.0.7/tests/asts/18_multiple_sources_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/19_is_defined.yml` & `ansible_rulebook-1.0.7/tests/asts/19_is_defined.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/20_is_not_defined.yml` & `ansible_rulebook-1.0.7/tests/asts/20_is_not_defined.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/21_run_playbook.yml` & `ansible_rulebook-1.0.7/tests/asts/21_run_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/23_nested_data.yml` & `ansible_rulebook-1.0.7/tests/asts/23_nested_data.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/24_max_attributes.yml` & `ansible_rulebook-1.0.7/tests/asts/24_max_attributes.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/25_max_attributes_nested.yml` & `ansible_rulebook-1.0.7/tests/asts/25_max_attributes_nested.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/26_print_events.yml` & `ansible_rulebook-1.0.7/tests/asts/26_print_events.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/27_var_root.yml` & `ansible_rulebook-1.0.7/tests/asts/27_var_root.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/28_right_side_condition_template.yml` & `ansible_rulebook-1.0.7/tests/asts/28_right_side_condition_template.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/29_run_module.yml` & `ansible_rulebook-1.0.7/tests/asts/29_run_module.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/30_run_module_missing.yml` & `ansible_rulebook-1.0.7/tests/asts/30_run_module_missing.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/31_run_module_missing_args.yml` & `ansible_rulebook-1.0.7/tests/asts/31_run_module_missing_args.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/32_run_module_fail.yml` & `ansible_rulebook-1.0.7/tests/asts/32_run_module_fail.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/33_run_playbook_retry.yml` & `ansible_rulebook-1.0.7/tests/asts/33_run_playbook_retry.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/34_run_playbook_retries.yml` & `ansible_rulebook-1.0.7/tests/asts/34_run_playbook_retries.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-1.0.7/tests/asts/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/36_multiple_rulesets_both_fired.yml` & `ansible_rulebook-1.0.7/tests/asts/36_multiple_rulesets_both_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/37_hosts_facts.yml` & `ansible_rulebook-1.0.7/tests/asts/37_hosts_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/38_shutdown.yml` & `ansible_rulebook-1.0.7/tests/asts/38_shutdown.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules.yml` & `ansible_rulebook-1.0.7/tests/asts/rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_assignment.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_assignment.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_assignment2.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_assignment2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_multiple_conditions.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_multiple_conditions.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_multiple_conditions2.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_multiple_conditions2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_multiple_conditions3.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_multiple_conditions3.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_time.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_time.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_timestamp.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_timestamp.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_with_vars.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_with_vars.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/rules_without_assignment.yml` & `ansible_rulebook-1.0.7/tests/asts/rules_without_assignment.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_filters.yml` & `ansible_rulebook-1.0.7/tests/asts/test_filters.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_host_rules.yml` & `ansible_rulebook-1.0.7/tests/asts/test_host_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_rules.yml` & `ansible_rulebook-1.0.7/tests/asts/test_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_rules_multiple_hosts.yml` & `ansible_rulebook-1.0.7/tests/asts/test_rules_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_rules_multiple_hosts2.yml` & `ansible_rulebook-1.0.7/tests/asts/test_rules_multiple_hosts2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_rules_multiple_hosts3.yml` & `ansible_rulebook-1.0.7/tests/asts/test_rules_multiple_hosts3.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_set_facts.yml` & `ansible_rulebook-1.0.7/tests/asts/test_set_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/asts/test_simple.yml` & `ansible_rulebook-1.0.7/tests/asts/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/conftest.py` & `ansible_rulebook-1.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/data/awx_test_data.py` & `ansible_rulebook-1.0.7/tests/data/awx_test_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/data/rulebook.yml` & `ansible_rulebook-1.0.7/tests/data/rulebook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/data/test.tar` & `ansible_rulebook-1.0.7/tests/data/test.tar`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/README.md` & `ansible_rulebook-1.0.7/tests/e2e/README.md`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/conftest.py` & `ansible_rulebook-1.0.7/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/extra_vars/operator_variables.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/extra_vars/operator_variables.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/playbooks/run_playbook_test_playbook.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/playbooks/run_playbook_test_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_actions_sanity.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_run_playbook.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_run_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_shutdown_graceful.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/actions/test_shutdown_now.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_logical_operators.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_logical_operators.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_membership_operators.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_membership_operators.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_relational_operators.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_relational_operators.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_select_operator.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_select_operator.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_selectattr_operator.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_string_match.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_string_match.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_string_search_regex.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/operators/test_string_search_search.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/operators/test_string_search_search.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/test_disabled_rules.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/test_disabled_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/test_process_source_end.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/test_process_source_end.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml` & `ansible_rulebook-1.0.7/tests/e2e/files/rulebooks/variables/test_variables_sanity.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/settings.py` & `ansible_rulebook-1.0.7/tests/e2e/settings.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_actions.py` & `ansible_rulebook-1.0.7/tests/e2e/test_actions.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_match_multiple_rules.py` & `ansible_rulebook-1.0.7/tests/e2e/test_match_multiple_rules.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_non_alpha_keys.py` & `ansible_rulebook-1.0.7/tests/e2e/test_non_alpha_keys.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_operators.py` & `ansible_rulebook-1.0.7/tests/e2e/test_operators.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_run_module_output.py` & `ansible_rulebook-1.0.7/tests/e2e/test_run_module_output.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_runtime.py` & `ansible_rulebook-1.0.7/tests/e2e/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_skip_audit_events.py` & `ansible_rulebook-1.0.7/tests/e2e/test_skip_audit_events.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_variables.py` & `ansible_rulebook-1.0.7/tests/e2e/test_variables.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/test_websocket.py` & `ansible_rulebook-1.0.7/tests/e2e/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/utils/awx/create-cluster.yml` & `ansible_rulebook-1.0.7/tests/e2e/utils/awx/create-cluster.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/utils/awx/install-awx.yml` & `ansible_rulebook-1.0.7/tests/e2e/utils/awx/install-awx.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/utils/awx/readme.md` & `ansible_rulebook-1.0.7/tests/e2e/utils/awx/readme.md`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml` & `ansible_rulebook-1.0.7/tests/e2e/utils/awx/roles/install-awx/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/e2e/utils.py` & `ansible_rulebook-1.0.7/tests/e2e/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/event_filter/dashes_to_underscores.py` & `ansible_rulebook-1.0.7/tests/event_filter/dashes_to_underscores.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/event_filter/json_filter.py` & `ansible_rulebook-1.0.7/tests/event_filter/json_filter.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/event_filter/noop.py` & `ansible_rulebook-1.0.7/tests/event_filter/noop.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/event_filter/test_insert_meta_info.py` & `ansible_rulebook-1.0.7/tests/event_filter/test_insert_meta_info.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/27_var_root.yml` & `ansible_rulebook-1.0.7/tests/examples/27_var_root.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-1.0.7/tests/examples/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/36_multiple_rulesets_both_fired.yml` & `ansible_rulebook-1.0.7/tests/examples/36_multiple_rulesets_both_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/50_negation.yml` & `ansible_rulebook-1.0.7/tests/examples/50_negation.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/51_vars_namespace.yml` & `ansible_rulebook-1.0.7/tests/examples/51_vars_namespace.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/52_once_within.yml` & `ansible_rulebook-1.0.7/tests/examples/52_once_within.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/53_once_within_multiple_hosts.yml` & `ansible_rulebook-1.0.7/tests/examples/53_once_within_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/54_time_window.yml` & `ansible_rulebook-1.0.7/tests/examples/54_time_window.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/55_not_all.yml` & `ansible_rulebook-1.0.7/tests/examples/55_not_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/56_once_after.yml` & `ansible_rulebook-1.0.7/tests/examples/56_once_after.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/57_once_after_multi.yml` & `ansible_rulebook-1.0.7/tests/examples/57_once_after_multi.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/58_string_search.yml` & `ansible_rulebook-1.0.7/tests/examples/58_string_search.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/60_json_filter.yml` & `ansible_rulebook-1.0.7/tests/examples/60_json_filter.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/61_select_1.yml` & `ansible_rulebook-1.0.7/tests/examples/61_select_1.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/62_select_2.yml` & `ansible_rulebook-1.0.7/tests/examples/62_select_2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/63_selectattr_1.yml` & `ansible_rulebook-1.0.7/tests/examples/63_selectattr_1.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/64_selectattr_2.yml` & `ansible_rulebook-1.0.7/tests/examples/64_selectattr_2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/66_sleepy_playbook.yml` & `ansible_rulebook-1.0.7/tests/examples/66_sleepy_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/67_shutdown_now.yml` & `ansible_rulebook-1.0.7/tests/examples/67_shutdown_now.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/69_enhanced_debug.yml` & `ansible_rulebook-1.0.7/tests/examples/69_enhanced_debug.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/70_null.yml` & `ansible_rulebook-1.0.7/tests/examples/70_null.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/72_set_fact_with_type.yml` & `ansible_rulebook-1.0.7/tests/examples/72_set_fact_with_type.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/73_mix_and_match_list.yml` & `ansible_rulebook-1.0.7/tests/examples/73_mix_and_match_list.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/75_all_conditions.yml` & `ansible_rulebook-1.0.7/tests/examples/75_all_conditions.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/76_all_conditions.yml` & `ansible_rulebook-1.0.7/tests/examples/76_all_conditions.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/78_complete_retract_fact.yml` & `ansible_rulebook-1.0.7/tests/examples/78_complete_retract_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/82_non_alpha_keys.yml` & `ansible_rulebook-1.0.7/tests/examples/82_non_alpha_keys.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/replays/23_nested_data/generate_data.py` & `ansible_rulebook-1.0.7/tests/examples/replays/23_nested_data/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/replays/24_max_attributes/00.json` & `ansible_rulebook-1.0.7/tests/examples/replays/24_max_attributes/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/replays/24_max_attributes/generate_data.py` & `ansible_rulebook-1.0.7/tests/examples/replays/24_max_attributes/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/replays/25_max_attributes_nested/00.json` & `ansible_rulebook-1.0.7/tests/examples/replays/25_max_attributes_nested/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/replays/25_max_attributes_nested/generate_data.py` & `ansible_rulebook-1.0.7/tests/examples/replays/25_max_attributes_nested/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/examples/replays/39_is_defined/generate_data.py` & `ansible_rulebook-1.0.7/tests/examples/replays/39_is_defined/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/generate_asts.py` & `ansible_rulebook-1.0.7/tests/generate_asts.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/playbooks/check_facts_playbook.yml` & `ansible_rulebook-1.0.7/tests/playbooks/check_facts_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/playbooks/fail_and_succeed.yml` & `ansible_rulebook-1.0.7/tests/playbooks/fail_and_succeed.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/playbooks/validate_args_playbook.yml` & `ansible_rulebook-1.0.7/tests/playbooks/validate_args_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/rules.yml` & `ansible_rulebook-1.0.7/tests/rules/rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/rules_with_time.yml` & `ansible_rulebook-1.0.7/tests/rules/rules_with_time.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/rules_with_timestamp.yml` & `ansible_rulebook-1.0.7/tests/rules/rules_with_timestamp.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_filters.yml` & `ansible_rulebook-1.0.7/tests/rules/test_filters.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_host_rules.yml` & `ansible_rulebook-1.0.7/tests/rules/test_host_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_kafka.yml` & `ansible_rulebook-1.0.7/tests/rules/test_kafka.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_rules.yml` & `ansible_rulebook-1.0.7/tests/rules/test_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_rules_multiple_hosts.yml` & `ansible_rulebook-1.0.7/tests/rules/test_rules_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_set_facts.yml` & `ansible_rulebook-1.0.7/tests/rules/test_set_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_simple.yml` & `ansible_rulebook-1.0.7/tests/rules/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/test_states.yml` & `ansible_rulebook-1.0.7/tests/rules/test_states.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/rules/webserver_down.yml` & `ansible_rulebook-1.0.7/tests/rules/webserver_down.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/file.py` & `ansible_rulebook-1.0.7/tests/sources/file.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/generic.py` & `ansible_rulebook-1.0.7/tests/sources/generic.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/hosts.py` & `ansible_rulebook-1.0.7/tests/sources/hosts.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/infrange.py` & `ansible_rulebook-1.0.7/tests/sources/infrange.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/log_scraper.py` & `ansible_rulebook-1.0.7/tests/sources/log_scraper.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/nested.py` & `ansible_rulebook-1.0.7/tests/sources/nested.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/ping.py` & `ansible_rulebook-1.0.7/tests/sources/ping.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/process_check.py` & `ansible_rulebook-1.0.7/tests/sources/process_check.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/range.py` & `ansible_rulebook-1.0.7/tests/sources/range.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/range2.py` & `ansible_rulebook-1.0.7/tests/sources/range2.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/replay.py` & `ansible_rulebook-1.0.7/tests/sources/replay.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/template.py` & `ansible_rulebook-1.0.7/tests/sources/template.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/tick.py` & `ansible_rulebook-1.0.7/tests/sources/tick.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/timestamp.py` & `ansible_rulebook-1.0.7/tests/sources/timestamp.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/sources/url_check.py` & `ansible_rulebook-1.0.7/tests/sources/url_check.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_ansible_events.py` & `ansible_rulebook-1.0.7/tests/test_ansible_events.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_app.py` & `ansible_rulebook-1.0.7/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_ast.py` & `ansible_rulebook-1.0.7/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_collection.py` & `ansible_rulebook-1.0.7/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_controller.py` & `ansible_rulebook-1.0.7/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_engine.py` & `ansible_rulebook-1.0.7/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_examples.py` & `ansible_rulebook-1.0.7/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_rules.py` & `ansible_rulebook-1.0.7/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_simple.yml` & `ansible_rulebook-1.0.7/tests/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_token.py` & `ansible_rulebook-1.0.7/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/test_websocket.py` & `ansible_rulebook-1.0.7/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/conftest.py` & `ansible_rulebook-1.0.7/tests/unit/action/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_controller.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_controller.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_debug.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_debug.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_noop.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_noop.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_post_event.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_post_event.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_print_event.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_print_event.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_retract_fact.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_retract_fact.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_run_job_template.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_run_job_template.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_run_module.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_run_module.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_run_playbook.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_run_playbook.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_run_workflow_template.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_run_workflow_template.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_set_fact.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_set_fact.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/action/test_shutdown.py` & `ansible_rulebook-1.0.7/tests/unit/action/test_shutdown.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/test_cli.py` & `ansible_rulebook-1.0.7/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/test_terminal.py` & `ansible_rulebook-1.0.7/tests/unit/test_terminal.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-1.0.6/tests/unit/test_util.py` & `ansible_rulebook-1.0.7/tests/unit/test_util.py`

 * *Files identical despite different names*

