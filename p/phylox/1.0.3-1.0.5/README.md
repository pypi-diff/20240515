# Comparing `tmp/phylox-1.0.3.tar.gz` & `tmp/phylox-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylox-1.0.3.tar", last modified: Sat Jan 20 20:30:35 2024, max compression
+gzip compressed data, was "phylox-1.0.5.tar", last modified: Wed May 15 10:51:50 2024, max compression
```

## Comparing `phylox-1.0.3.tar` & `phylox-1.0.5.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.341910 phylox-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-01-20 20:30:28.000000 phylox-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-01-20 20:30:35.341910 phylox-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-20 20:30:28.000000 phylox-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-20 20:30:28.000000 phylox-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 20:30:35.341910 phylox-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.329909 phylox-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.333910 phylox-1.0.3/src/phylox/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.333910 phylox-1.0.3/src/phylox/cherrypicking/
--rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/cherrypicking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18121 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/cherrypicking/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/cherrypicking/best_subnetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    27789 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/cherrypicking/combining_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/cherrypicking/tree_child_sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.333910 phylox-1.0.3/src/phylox/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/classes/dinetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/classes/networkclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/dinetwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.333910 phylox-1.0.3/src/phylox/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/exceptions/invalidmovedefinitionexception.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/exceptions/invalidmoveexception.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/exceptions/nosolutionexception.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/exceptions/timeoutexception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.333910 phylox-1.0.3/src/phylox/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/generators/heath/
--rw-r--r--   0 runner    (1001) docker     (127)    24298 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/heath/heath.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/heath/heath_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/generators/lgt/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/lgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/lgt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/generators/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/mcmc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/generators/randomTC/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/randomTC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/randomTC/random_tc_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/generators/trees/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/trees/add_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/trees/beta_splitting_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/trees/well_known.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/generators/zods/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/zods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/zods/zods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/generators/zods/zods_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/isomorphism/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/isomorphism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/isomorphism/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/networkproperties/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/networkproperties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/networkproperties/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.337910 phylox-1.0.3/src/phylox/rearrangement/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.341910 phylox-1.0.3/src/phylox/rearrangement/exact_distance/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/exact_distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/exact_distance/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.341910 phylox-1.0.3/src/phylox/rearrangement/heuristics/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/heuristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/heuristics/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    29569 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/heuristics/green_line_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (127)    27078 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/heuristics/red_line_heuristic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10366 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/heuristics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/invertsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/movability.py
--rw-r--r--   0 runner    (1001) docker     (127)    19824 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/move.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/movetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-01-20 20:30:28.000000 phylox-1.0.3/src/phylox/rearrangement/rearrangementproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.341910 phylox-1.0.3/src/phylox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-01-20 20:30:35.000000 phylox-1.0.3/src/phylox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-01-20 20:30:35.000000 phylox-1.0.3/src/phylox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 20:30:35.000000 phylox-1.0.3/src/phylox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-20 20:30:35.000000 phylox-1.0.3/src/phylox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-20 20:30:35.000000 phylox-1.0.3/src/phylox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-20 20:30:35.000000 phylox-1.0.3/src/phylox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:30:35.341910 phylox-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-01-20 20:30:28.000000 phylox-1.0.3/tests/test_dinetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-01-20 20:30:28.000000 phylox-1.0.3/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-15 10:51:46.000000 phylox-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-15 10:51:50.429508 phylox-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-15 10:51:46.000000 phylox-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-15 10:51:46.000000 phylox-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:51:50.429508 phylox-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.417508 phylox-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.421508 phylox-1.0.5/src/phylox/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/cherrypicking/
+-rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/cherrypicking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18630 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/cherrypicking/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/cherrypicking/best_subnetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28326 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/cherrypicking/combining_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/cherrypicking/tree_child_sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/classes/dinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/classes/networkclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/dinetwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/exceptions/invalidmovedefinitionexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/exceptions/invalidmoveexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/exceptions/nosolutionexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/exceptions/timeoutexception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/generators/heath/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/heath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29068 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/heath/heath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/heath/heath_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/generators/lgt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/lgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11165 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/lgt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/generators/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/mcmc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/generators/randomTC/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/randomTC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/randomTC/random_tc_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.425508 phylox-1.0.5/src/phylox/generators/trees/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/trees/add_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/trees/beta_splitting_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/trees/well_known.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/src/phylox/generators/zods/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/zods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/zods/zods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/generators/zods/zods_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/src/phylox/isomorphism/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/isomorphism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/isomorphism/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/src/phylox/networkproperties/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/networkproperties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/networkproperties/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/src/phylox/rearrangement/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/src/phylox/rearrangement/exact_distance/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/exact_distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/exact_distance/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/src/phylox/rearrangement/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/heuristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/heuristics/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29569 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/heuristics/green_line_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27078 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/heuristics/red_line_heuristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10366 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/heuristics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/invertsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/movability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19824 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/movetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-15 10:51:46.000000 phylox-1.0.5/src/phylox/rearrangement/rearrangementproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/src/phylox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-15 10:51:50.000000 phylox-1.0.5/src/phylox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 10:51:50.000000 phylox-1.0.5/src/phylox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:51:50.000000 phylox-1.0.5/src/phylox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 10:51:50.000000 phylox-1.0.5/src/phylox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 10:51:50.000000 phylox-1.0.5/src/phylox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 10:51:50.000000 phylox-1.0.5/src/phylox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:51:50.429508 phylox-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-15 10:51:46.000000 phylox-1.0.5/tests/test_dinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-15 10:51:46.000000 phylox-1.0.5/tests/test_parser.py
```

### Comparing `phylox-1.0.3/LICENSE` & `phylox-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/PKG-INFO` & `phylox-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylox
-Version: 1.0.3
+Version: 1.0.5
 Summary: A package with tools for constructing, manipulating, and analyzing phylogenetic networks.
 Author-email: Remie Janssen <remiejanssen92@gmail.com>
 Project-URL: Homepage, https://github.com/RemieJanssen/PhyloX
 Project-URL: Bug Tracker, https://github.com/RemieJanssen/PhyloX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,12 +67,28 @@
 ### Linting
 
 precommit is yet to be configured, for now, simply run black and isort.
 
 ### Documentation
 
 Documentation is in the docs folder, and is created uses sphinx.
-to build the documentation, go to the docs folder and do:
+
+#### Requirements
+You may need to install the requirements from `docs/requirements.txt` first. Make sure to use python<=3.11.*, for example:
+```
+conda create -n phylox-sphinx
+conda activate phylox-sphinx
+python install python==3.11.*
+pip install -r docs/requirements.txt
+```
+
+#### Creating documentation
+to build the documentation, go to the docs folder and run:
 ```
 make html
 ```
 the docs will be in `docs/build/html`.
+
+If you re-run the build, you can first remove the old autosummary files. If you do not, it will not update them.
+
+
+
```

### Comparing `phylox-1.0.3/README.md` & `phylox-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,12 +49,28 @@
 ### Linting
 
 precommit is yet to be configured, for now, simply run black and isort.
 
 ### Documentation
 
 Documentation is in the docs folder, and is created uses sphinx.
-to build the documentation, go to the docs folder and do:
+
+#### Requirements
+You may need to install the requirements from `docs/requirements.txt` first. Make sure to use python<=3.11.*, for example:
+```
+conda create -n phylox-sphinx
+conda activate phylox-sphinx
+python install python==3.11.*
+pip install -r docs/requirements.txt
+```
+
+#### Creating documentation
+to build the documentation, go to the docs folder and run:
 ```
 make html
 ```
 the docs will be in `docs/build/html`.
+
+If you re-run the build, you can first remove the old autosummary files. If you do not, it will not update them.
+
+
+
```

### Comparing `phylox-1.0.3/pyproject.toml` & `phylox-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phylox"
-version = "1.0.3"
+version = "1.0.5"
 authors = [
   { name="Remie Janssen", email="remiejanssen92@gmail.com" },
 ]
 description = "A package with tools for constructing, manipulating, and analyzing phylogenetic networks."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `phylox-1.0.3/src/phylox/base.py` & `phylox-1.0.5/src/phylox/base.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py` & `phylox-1.0.5/src/phylox/cherrypicking/Heuristic_Main_UserFriendly.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/cherrypicking/__init__.py` & `phylox-1.0.5/src/phylox/cherrypicking/__init__.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/cherrypicking/base.py` & `phylox-1.0.5/src/phylox/cherrypicking/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,15 @@
         suppress_node(network, px)
     if cherry_type == CHERRYTYPE.RETICULATEDCHERRY:
         px = network.parent(x)
         py = network.parent(y)
         network.remove_edge(py, px)
         suppress_node(network, px)
         suppress_node(network, py)
+    network._clear_cached()
     return network, cherry_type
 
 
 def check_reducible_pair(network, x, y):
     """
     Checks whether the pair (x,y) is a reducible pair in the network.
 
@@ -395,15 +396,15 @@
     network.remove_edge(parent_node_x, node_x)
     network.add_edges_from(
         [
             (parent_node_x, new_parent_of_x, old_edge_data),
             (
                 new_parent_of_x,
                 node_x,
-                {LENGTH_ATTR: length_incoming_x - height_pair_x},
+                {LENGTH_ATTR: height_pair_x},
             ),  # "no_of_trees": no_of_trees_incoming_x + len(red_trees)
             (
                 new_parent_of_y,
                 new_parent_of_x,
                 {LENGTH_ATTR: height_goal_x - height_pair_x},
             ),  # "no_of_trees": len(red_trees)
         ]
@@ -506,17 +507,14 @@
         The second element of the pair
 
     Returns
     -------
     float
         The height of the cherry (x,y) if it is a cherry, False otherwise
     """
-    print("cherry_height")
-    print(network.edges(data=True))
-
     if (not x in network.leaves) or (not y in network.leaves):
         return False
     px = network.parent(x)
     py = network.parent(y)
     if px == py:
         height = [network[px][x][LENGTH_ATTR], network[py][y][LENGTH_ATTR]]
         return height
@@ -528,15 +526,26 @@
         return height
     raise ValueError("x and y are not in the same cherry")
 
 
 class CherryPickingMixin:
     @classmethod
     def from_cherry_picking_sequence(cls, sequence, heights=None, label_leaves=True):
+        """
+        Creates a PhyloX DiNetwork network from a cherry picking sequence,
+        and possibly a matching sequence of heights of the cherries.
+
+        :param sequence: a cherry picking sequence (i.e., a list of 2-tuples)
+        :param heights: a list of positive floats with the same length as
+          `sequence`. If None, the heights will be set to consecutive integers
+        :param label_leaves: Bool, whether to label the leaves
+          with the nodes/labels used in the sequence
+        :return: a network.
+        """
         network = cls()
-        heights = heights or [[1, 1]] * len(sequence)
+        heights = heights or [[h, h] for h in range(1, len(sequence) + 1)]
         for pair, height in zip(reversed(sequence), reversed(heights)):
             add_pair(
                 network, *pair, height=height, inplace=True, nodes_by_label=label_leaves
             )
         network._clear_cached()
         return network
```

### Comparing `phylox-1.0.3/src/phylox/cherrypicking/best_subnetwork.py` & `phylox-1.0.5/src/phylox/cherrypicking/best_subnetwork.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/cherrypicking/combining_networks.py` & `phylox-1.0.5/src/phylox/cherrypicking/combining_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     find_reducible_pairs_with_first,
     find_reducible_pairs_with_second,
     find_reticulated_cherry_with_first,
     get_indices_of_reducing_pairs,
     reduce_pair,
 )
 from phylox.constants import LABEL_ATTR, LENGTH_ATTR
+from phylox.exceptions import NoSolutionException
 
 # prefix for harmonized node names
 HARMONIZE_NODES_BY_LABEL_PREFIX = "hnbl__"
 
 
 class HybridizationProblem:
     """
     A class to represent a hybridization problem.
     I.e. a set of phylogenetic networks that need to be combined into a single phylogenetic network.
+    The networks all need to have a unique root with out-degree 1.
 
     :param list_of_networks: a list of phylogenetic networks, each given as a phylox.DiNetwork.
     :param newick_strings: if True, the input trees are given as newick strings, otherwise as phylox.DiNetworks.
     """
 
     def __init__(self, list_of_networks=None, newick_strings=True):
         # The dictionary of trees
@@ -55,17 +57,20 @@
         # true if distances are used
         self.distances = True
 
         # read the input trees in 'newick_strings'
         list_of_networks = list_of_networks or []
         for n in list_of_networks:
             if newick_strings:
-                network = DiNetwork(newick=n)
+                network = DiNetwork.from_newick(n, add_root_edge=True)
             else:
                 network = n
+                for root in network.roots:
+                    if network.out_degree(root) > 1:
+                        raise NoSolutionException("No solution can be found, as an input network has a root with out-degree > 1.")
             self.trees[len(self.trees)] = network
             self.distances = self.distances and all(
                 [LENGTH_ATTR in edge[2] for edge in network.edges(data=True)]
             )
 
         # check that the labels are unique in each tree
         # and that all leaves have a label
@@ -338,16 +343,21 @@
             dict()
         )  # for each reducible pair: [0] gives height, [1] the number of trees it was computed in.
 
         if progress:
             print("found all reducible pairs")
         while copy_of_inputs.trees:
             if progress:
-                print("Sequence has length: " + str(len(CPS)))
-                print(str(len(copy_of_inputs.trees)) + " trees left.\n")
+                print()
+                print(f"Sequence has length: {len(CPS)}")
+                print(f"Current sequence: {CPS}")
+                print(f"Networks left: {len(copy_of_inputs.trees)}\n")
+                for nw_index, nw in copy_of_inputs.trees.items():
+                    print(f"  Network {nw_index}: {nw.newick()}\n    {nw.edges()}")
+                print()
                 # First reduce trivial cherries
                 print("Reducing trivial pairs")
             (
                 new_seq,
                 new_red_trees,
                 reducible_pairs,
                 new_heights_seq,
@@ -445,22 +455,22 @@
         # Remove trees to update from all pairs
         for pair, trees in list(reducible_pairs.items()):
             trees.difference_update(new_red_trees)
             if len(trees) == 0:
                 del reducible_pairs[pair]
         # Add the trees to the right pairs again
         for index in new_red_trees:
-            if index in self.trees:
-                t = self.trees[index]
-                red_pairs_t = find_all_reducible_pairs(t)
-                for pair in red_pairs_t:
-                    if pair in reducible_pairs:
-                        reducible_pairs[pair].add(index)
-                    else:
-                        reducible_pairs[pair] = set([index])
+            if index not in self.trees:
+                continue
+            t = self.trees[index]
+            red_pairs_t = find_all_reducible_pairs(t)
+            for pair in red_pairs_t:
+                if pair not in reducible_pairs:
+                    reducible_pairs[pair] = set()
+                reducible_pairs[pair].add(index)
         return reducible_pairs
 
     def Reduce_Pair_In_All(self, pair, reducible_pairs=dict()):
         """
         Reduces the given pair in all networks in the problem.
         Returns the set of networks that were reduced.
 
@@ -480,15 +490,14 @@
             if i in self.trees:
                 t = self.trees[i]
                 t, cherry_type = reduce_pair(t, *pair, inplace=True)
                 if cherry_type == CHERRYTYPE.RETICULATEDCHERRY:
                     reduced_trees_for_pair += [i]
                 elif cherry_type == CHERRYTYPE.CHERRY:
                     reduced_trees_for_pair += [i]
-                    t.leaves.remove(pair[0])
                 if len(t.edges()) <= 1:
                     del self.trees[i]
         return set(reduced_trees_for_pair)
 
     def Reduce_Trivial_Pairs(self, candidate_leaves):
         """
         Reduces the trivial pairs in the current set of networks.
```

### Comparing `phylox-1.0.3/src/phylox/cherrypicking/tree_child_sequences.py` & `phylox-1.0.5/src/phylox/cherrypicking/tree_child_sequences.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/classes/dinetwork.py` & `phylox-1.0.5/src/phylox/classes/dinetwork.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,24 +63,24 @@
     ...     edges=[(0,1),(1,2),(1,3),(2,4),(3,5),(2,5),(3,4),(4,6),(5,7)],
     ... )
     >>> is_orchard(network)
     False
     """
     if len(network) == 0:
         return True
-    leaves = network.leaves
     root = list(network.roots)[0]
 
     # make a copy and fix a root edge
     network_copy = deepcopy(network)
     if network_copy.out_degree(root) > 1:
         new_node = -1
         while new_node in network_copy.nodes:
             new_node -= 1
         network_copy.add_edge(new_node, root)
+    leaves = network_copy.leaves
 
     # try to reduce the network copy
     done = False
     while not done:
         checked_all_leaves = True
         for leaf in leaves:
             pair = is_second_in_reducible_pair(network_copy, leaf)
```

### Comparing `phylox-1.0.3/src/phylox/dinetwork.py` & `phylox-1.0.5/src/phylox/dinetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 
 import networkx as nx
 from networkx.utils.decorators import np_random_state, py_random_state
 
 from phylox.cherrypicking.base import CherryPickingMixin
 from phylox.constants import LABEL_ATTR, LENGTH_ATTR
-
+from phylox.base import find_unused_node
 
 class DiNetwork(nx.DiGraph, CherryPickingMixin):
     """
     A class for representing a directed phylogenetic network.
     Inherits from networkx.DiGraph.
 
     :param edges: a list of edges of the network.
@@ -32,31 +32,45 @@
 
         :return: None
         """
         for attr in [
             "_leaves",
             "_reticulations",
             "_roots",
-            "_reticulation_number, _labels, _label_to_node_dict",
+            "_reticulation_number",
+            "_labels",
+            "_label_to_node_dict",
         ]:
             if hasattr(self, attr):
                 delattr(self, attr)
 
     @classmethod
-    def from_newick(cls, newick):
+    def from_newick(cls, newick, add_root_edge=False):
         """
-        Creates a network from a newick string.
-        Not implemented.
+        Creates a PhyloX DiNetwork network from a newick string.
 
         :param newick: a newick string.
+        :param add_root_edge: whether to add a root edge of length 0
+          if not explicitly defined by the newick string.
         :return: a network.
         """
         from phylox.parser import extended_newick_to_dinetwork
 
-        return extended_newick_to_dinetwork(newick)
+        network = extended_newick_to_dinetwork(newick)
+        if not add_root_edge:
+            return network
+
+        for root in network.roots:
+            if network.out_degree(root) > 1:
+                new_root = find_unused_node(network)
+                network.add_edges_from([(new_root, root, {LENGTH_ATTR: 0})])
+                root = new_root
+        network._clear_cached()
+        return network
+
 
     def _set_leaves(self):
         """
         Sets the set of leaves of the network as a cached property.
 
         :return: the set of leaves of the network.
         """
@@ -258,16 +272,17 @@
         I.e., whether it has in-degree <= 1 and out-degree > 1.
 
         :param node: a node in the network.
         :return: a boolean value.
         """
         return self.out_degree(node) > 1 and self.in_degree(node) <= 1
 
-    def newick(self):
+    def newick(self, simple=False):
         """
         Returns a newick string representing the network.
 
+        :param simple: Boolean, indicating whether to create a simple newick string without parameters
         :return: a newick string.
         """
         from phylox.parser import dinetwork_to_extended_newick
 
-        return dinetwork_to_extended_newick(self)
+        return dinetwork_to_extended_newick(self, simple=simple)
```

### Comparing `phylox-1.0.3/src/phylox/generators/__init__.py` & `phylox-1.0.5/src/phylox/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/generators/heath/heath.py` & `phylox-1.0.5/src/phylox/generators/heath/heath.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,91 +17,128 @@
 import random
 import sys
 
 import networkx as nx
 import numpy as np
 import scipy.stats
 
+from networkx.utils.decorators import np_random_state, py_random_state
 
-# For each choice of reticulation arcs, calculate the distance between all pairs of taxa
-# Add up all these distances for each pair, weighed by the probability of this embedded tree
-# The hyb rates are e^(-hybridization_rate*sum_for_pair-offset) for each pair.
-#####
-# Updating distances between pairs can be done smartly:
-#  for a speciation event, the distances simply increase by two times the time to speciation, and the new species copies the distances from its sister species
-#  for an extinction event, the distances simply increase by two times the time to speciation, and the distances to the extinct species are removed.
-#  for a HGT event, only the rates for the receiving taxon have to be updated. They can be computed from the distances to the receiving and the donating easily
-#  for a hyb event, all paths go via exactly one of the parent species, so we can use those distances again.
-def UpdateHybridizationRates():
-    return False
-    # This is done within the CalculateNetwork function
+from phylox import DiNetwork
+from phylox.constants import LENGTH_ATTR, PROBABILITY_ATTR, LABEL_ATTR
 
 
-def GammaDistributionPDF(value, mean, shape):
+def gamma_distribution_pdf(value, mean, shape):
+    """
+    A reparameterization of the Gamma Distribution from scipy stats,
+    with mean parameter instead of a shape parameter.
+
+    """
     scale = mean / shape
     return scipy.stats.gamma.pdf(value, shape, 0, scale)
 
 
-def CalculateNewRate(parent_rate, prior_mean, prior_shape, update_shape):
-    proposed_rate = parent_rate * random.gammavariate(update_shape, 1 / update_shape)
-    if random.random() < GammaDistributionPDF(
+@np_random_state("seed")
+def update_rate(parent_rate, prior_mean, prior_shape, update_shape, seed=None):
+    """
+    Generates the new value for a rate used in the Heath generator based on
+     - the current value,
+     - the multiplicative update factor `np.random.gamma(<update_shape>, 1 / <update_shape>)`
+     - the prior Gamma Distribution for the rate type `GammaDistributionPDF(rate_value, prior_mean, prior_shape)`
+    """
+
+    proposed_rate = parent_rate * seed.gamma(update_shape, 1 / update_shape)
+    if seed.random() < gamma_distribution_pdf(
         proposed_rate, prior_mean, prior_shape
-    ) / GammaDistributionPDF(parent_rate, prior_mean, prior_shape):
+    ) / gamma_distribution_pdf(parent_rate, prior_mean, prior_shape):
         return proposed_rate
     return parent_rate
 
-
-def CalculateAllNewRates(
+@np_random_state("seed")
+def update_all_rates(
     parent_rates,
     update_shape,
     speciation_rate_mean,
     speciation_rate_shape,
     ext_used,
     extinction_rate_mean,
     extinction_rate_shape,
     hgt_used,
     hgt_rate_mean,
     hgt_rate_shape,
+    seed=None,
 ):
-    sp_rate = CalculateNewRate(
-        parent_rates[0], speciation_rate_mean, speciation_rate_shape, update_shape
+    """
+    Updates all rates for the Heath generator using the `update_rate` function.
+    """
+    sp_rate = update_rate(
+        parent_rates[0], speciation_rate_mean, speciation_rate_shape, update_shape, seed=seed
     )
     ext_rate = 0
     if ext_used:
-        ext_rate = CalculateNewRate(
-            parent_rates[1], extinction_rate_mean, extinction_rate_shape, update_shape
+        ext_rate = update_rate(
+            parent_rates[1], extinction_rate_mean, extinction_rate_shape, update_shape, seed=seed
         )
     hgt_rate = 0
     if hgt_used:
-        hgt_rate = CalculateNewRate(
-            parent_rates[2], hgt_rate_mean, hgt_rate_shape, update_shape
+        hgt_rate = update_rate(
+            parent_rates[2], hgt_rate_mean, hgt_rate_shape, update_shape, seed=seed
         )
     return (sp_rate, ext_rate, hgt_rate)
 
 
-def DistanceToRate(
+def graph_distance_to_hybridization_rate(
     distance,
     hybridization_left_bound,
     hybridization_right_bound,
     hybridization_left_rate,
     hybridization_right_rate,
 ):
-    # TODO Update this rate function, make it more of a gradual switch?
+    """
+    Returns a hybdridization rate for a given distance.
+    The distance represents the evolutionary distance between two extant species.
+    The function is used in the Heath generator to determine the hybdridization rate between two current taxa,
+    where the distance is a weighthed sum of all up-down distances between the two taxa in the current network.
+    The dependency on the distance takes the following shape:
+     - hybridization_left_bound:  l
+     - hybridization_right_bound: r
+     - hybridization_left_rate:   rl
+     - hybridization_right_rate:  rr.
+
+    ::
+
+           |
+        lr +---
+           |   \\
+           |    \\
+           |     \\
+        rr +      -----
+           |
+         0 +---+----+-----
+           0   l    r
+
+    where the distance is on the x-axis, and the hybridization rate on the y-axis.
+    """
     if distance <= hybridization_left_bound:
         return hybridization_left_rate
     elif distance >= hybridization_right_bound:
         return hybridization_right_rate
     return hybridization_left_rate + (
         hybridization_right_rate - hybridization_left_rate
     ) * (distance - hybridization_left_bound) / (
         hybridization_right_bound - hybridization_left_bound
     )
 
 
-def RestrictToLeafSet(network, leaves_to_keep, suppress_trivial_blobs=False):
+def restrict_network_to_leaf_set(network, leaves_to_keep):
+    """
+    Removes all leaves in the network that are not in the `leaves_to_keep` container.
+    Then cleans up the network, by iteratively removing out-degree 0 nodes that are not in the `leaves_to_keep` set, and suppressing in-degree 1 out-degree 1 nodes.
+    Modifies the network in place and returns it.
+    """
     # find leaves to remove
     leaves_to_keep = set(leaves_to_keep)
     remove_nodes = set()
     for v in network.nodes():
         if network.out_degree(v) == 0 and v not in leaves_to_keep:
             remove_nodes.add(v)
 
@@ -110,167 +147,232 @@
         removed_node = remove_nodes.pop()
         parents = list(network.predecessors(removed_node))
         network.remove_node(removed_node)
         for p in parents:
             if network.out_degree(p) == 0:
                 remove_nodes.add(p)
 
-    # optionally: suppress biconnected components with indegree-1 and outdegree-1
-    if suppress_trivial_blobs:
-        # TODO: write this function.
-        # What to do with the length of the resulting arc? the blob may have multiple paths, do we average?
-        print("suppressing trivial blobs is not implemented yet")
-
     # suppress degree-2 nodes
-    network = SuppressDegree2(network)
+    network = suppress_degree_two_nodes(network)
     return network
 
 
-def SuppressDegree2(network):
+def suppress_degree_two_nodes(network):
+    """
+    Suppresses degree 2 (in-degree 1 out-degree 1) nodes of the network in place and
+    returns the network. The length of the new edge is the sum of the lengths of the old two edges.
+    If the bottom edge had a probability, then this probability is given to the new edge.
+    """
     to_remove = []
     to_check = set(list(network.nodes())[:])
     while to_check:
         v = to_check.pop()
         if network.in_degree(v) == 1 and network.out_degree(v) == 1:
             to_remove += [v]
             parent = list(network.predecessors(v))[0]
             child = list(network.successors(v))[0]
             if network.has_edge(parent, child):
                 to_check.add(parent)
                 to_check.add(child)
-            in_edge_length = network[parent][v]["length"]
-            out_edge_length = network[v][child]["length"]
-            out_edge_prob = network[v][child].get("prob")
+            in_edge_length = network[parent][v][LENGTH_ATTR]
+            out_edge_length = network[v][child][LENGTH_ATTR]
+            out_edge_prob = network[v][child].get(PROBABILITY_ATTR)
             network.remove_edges_from([(parent, v), (v, child)])
             network.add_weighted_edges_from(
-                [(parent, child, in_edge_length + out_edge_length)], weight="length"
+                [(parent, child, in_edge_length + out_edge_length)], weight=LENGTH_ATTR
             )
             if out_edge_prob != None:
-                network[parent][child]["prob"] = out_edge_prob
+                network[parent][child][PROBABILITY_ATTR] = out_edge_prob
     network.remove_nodes_from(to_remove)
     return network
 
 
+# For each choice of reticulation arcs, calculate the distance between all pairs of taxa
+# Add up all these distances for each pair, weighed by the probability of this embedded tree
+# The hyb rates are e^(-hybridization_rate*sum_for_pair-offset) for each pair.
+#####
+# Updating distances between pairs can be done smartly:
+#  for a speciation event, the distances simply increase by two times the time to speciation, and the new species copies the distances from its sister species
+#  for an extinction event, the distances simply increase by two times the time to speciation, and the distances to the extinct species are removed.
+#  for a HGT event, only the rates for the receiving taxon have to be updated. They can be computed from the distances to the receiving and the donating easily
+#  for a hyb event, all paths go via exactly one of the parent species, so we can use those distances again.
+# Updating hybridization rates is done within the generate_heath_network function
+@np_random_state("seed")
 def generate_heath_network(
     time_limit=1.0,
     taxa_limit=None,
     update_shape=2.0,
     speciation_rate_mean=2.0,
     speciation_rate_shape=2.0,
     ext_used=True,
-    count_extinct=0,
-    extinction_rate_mean=2.0,
-    extinction_rate_shape=2.0,
+    count_extinct=False,
+    extinction_rate_mean=1.0,
+    extinction_rate_shape=1.0,
     hgt_used=False,
     hgt_rate_mean=None,
     hgt_rate_shape=None,
     hgt_inheritance=0.05,
     hyb_used=False,
     hybridization_left_bound=None,
     hybridization_right_bound=None,
     hybridization_left_rate=None,
     hybridization_right_rate=None,
     simple_output=False,
+    seed=None,
 ):
+    """
+    Runs a speciation-extinction-HGT-hybridization model for the given time (`time_limit`)
+    or until a certain number of extant taxa (`taxa_limit`) is reached.
+    If all lineages go extinct before the given time is reached, another attempt is made.
+    Each extant taxon has its own speciation, HGT, and extinction rates (`rate=1/mean_time_until_next_event`).
+    Hybridization rates are `evolutionary distance` dependent, with a function determined by global parameters
+
+    There are prior speciation/extinction/HGT rate distributions:
+    gamma distributions with a given mean and a shape parameter for speciation
+    (`speciation_rate_mean` and `speciation_rate_shape`)
+    and extinction (`extinction_rate_mean` and `extinction_rate_shape`),
+    HGT (Horizontal gene transfer) is turned off by default, bu can be turned on by setting `hgt_used=True`.
+    This also requires you to set the paramaters for the HGT rate distribution (`hgt_rate_mean` and `hgt_rate_shape`).
+    Extinction can be turned off by setting `ext_used=False`.
+
+    If an HGT event happens for a given taxon, another taxon (including itself) is chosen
+    uniformly at random to donate genetic material (uniformly distributed contribution in `[0,max_hgt]`
+    where `max_hgt` is determined by the `hgt_inheritance`).
+
+    If hybridization is turned on (`hyb_used=True`), the hybdridization rate between two taxa
+    is calculated as a function of the distance between those taxa. This distance is a weighthed
+    sum of all up-down distances between the two taxa in the current network.
+    The dependency on the distance takes the following shape:
+     - `hybridization_left_bound`:  l
+     - `hybridization_right_bound`: r
+     - `hybridization_left_rate`:   rl
+     - `hybridization_right_rate`:  rr.
+
+    ::
+
+           |
+        lr +---
+           |   \\
+           |    \\
+           |     \\
+        rr +      -----
+           |
+         0 +---+----+-----
+           0   l    r
+
+    where the distance is on the x-axis, and the hybridization rate on the y-axis.
+
+    After speciation or hybridization, each rate of the new lineages is set by multiplying the
+    (weighted mean) rate of the parent lineage(s) by a gamma-distributed factor with mean 1 and
+    a shape parameter (`update_shape`), and then accepting this rate with a probability
+    proportional to the prior distribution for this rate.
+    This gives an ultrametric network on the extant species.
+
+    The random seed can be set with the `seed` parameter.
+
+    Returns a network without leaf labels, the set of hybrid nodes,
+    the set of extant taxa, and the number of extinct taxa.
+    """
     # Initiate the network
-    nw = nx.DiGraph()
+    nw = DiNetwork()
     nw.add_node(0)
-    leaves = set([0])
+    extant_taxa = set([0])
     current_node = 1
     no_of_extinct = 0
+    hybrid_nodes = dict()
+    no_of_hybrids = 0
 
-    # Set initial rates and distances
-    current_speciation_rate = random.gammavariate(
+    # Draw initial rates and distances
+    current_speciation_rate = seed.gamma(
         speciation_rate_shape, speciation_rate_mean / speciation_rate_shape
     )
     current_extinction_rate = 0.0
     if ext_used:
-        current_extinction_rate = random.gammavariate(
+        current_extinction_rate = seed.gamma(
             extinction_rate_shape, extinction_rate_mean / extinction_rate_shape
         )
     current_hgt_rate = 0.0
     if hgt_used:
-        current_hgt_rate = random.gammavariate(
+        current_hgt_rate = seed.gamma(
             hgt_rate_shape, hgt_rate_mean / hgt_rate_shape
         )
     current_hybridization_rate = float(0)
-    # Force the first event to be a speciation
-    total_rate = current_speciation_rate
-    distances = dict()
 
     # Set the initial leaf rates per leaf
     leaf_rates = dict()
     leaf_rates[0] = (current_speciation_rate, current_extinction_rate, current_hgt_rate)
 
+
+    # Force the first event to be a speciation
+    total_rate = current_speciation_rate
+    distances = dict()
     # Pick a time for the first event
-    extra_time = np.random.exponential(1 / float(total_rate))
+    extra_time = seed.exponential(1 / float(total_rate))
     current_time = extra_time
 
-    #####First create the network as a MUL-tree, to make it easier to convert to Newick (not currently implemented)
-    hybrid_nodes = dict()
-    no_of_hybrids = 0
-
-    while len(leaves) > 0 and (
+    while len(extant_taxa) > 0 and (
         (not taxa_limit and current_time < time_limit)
-        or (taxa_limit and len(leaves) + count_extinct * no_of_extinct < taxa_limit)
+        or (taxa_limit and len(extant_taxa) + count_extinct * no_of_extinct < taxa_limit)
     ):
-        random_number = random.random()
+        random_number = seed.random()
         splitting_leaf = None
         extinction_leaf = None
         hgt_donor_leaf = None
         parent_acceptor = None
         hgt_acceptor_leaf = None
         hyb_pair = None
         if random_number < current_speciation_rate / total_rate:
             ######################
             #     Speciation     #
             ######################
             if not simple_output:
                 print("speciation")
-            random_number = random.random() * current_speciation_rate
+            random_number = seed.random() * current_speciation_rate
             for leaf, rates in leaf_rates.items():
                 if random_number < rates[0]:
                     splitting_leaf = leaf
                     break
                 random_number -= rates[0]
             if splitting_leaf == None:
                 if not simple_output:
-                    print("ouch, speciation rate computed wrong")
+                    print("error, speciation rate computed wrong")
             nw.add_weighted_edges_from(
                 [
                     (splitting_leaf, current_node, 0),
                     (splitting_leaf, current_node + 1, 0),
                 ],
-                weight="length",
+                weight=LENGTH_ATTR,
             )
             # Update the rates and distances
             # rates
-            leaf_rates[current_node] = CalculateAllNewRates(
+            leaf_rates[current_node] = update_all_rates(
                 leaf_rates[splitting_leaf],
                 update_shape,
                 speciation_rate_mean,
                 speciation_rate_shape,
                 ext_used,
                 extinction_rate_mean,
                 extinction_rate_shape,
                 hgt_used,
                 hgt_rate_mean,
                 hgt_rate_shape,
+                seed=seed,
             )
-            leaf_rates[current_node + 1] = CalculateAllNewRates(
+            leaf_rates[current_node + 1] = update_all_rates(
                 leaf_rates[splitting_leaf],
                 update_shape,
                 speciation_rate_mean,
                 speciation_rate_shape,
                 ext_used,
                 extinction_rate_mean,
                 extinction_rate_shape,
                 hgt_used,
                 hgt_rate_mean,
                 hgt_rate_shape,
+                seed=seed,
             )
             current_speciation_rate += (
                 leaf_rates[current_node][0]
                 + leaf_rates[current_node + 1][0]
                 - leaf_rates[splitting_leaf][0]
             )
             current_extinction_rate += (
@@ -281,44 +383,44 @@
             current_hgt_rate += (
                 leaf_rates[current_node][2]
                 + leaf_rates[current_node + 1][2]
                 - leaf_rates[splitting_leaf][2]
             )
             # distances
             if hyb_used:
-                for l in leaves:
+                for l in extant_taxa:
                     if l != splitting_leaf:
                         pair = (splitting_leaf, l)
                         if pair in distances.keys():
                             new_distance = distances[pair]
                         else:
                             pair = (l, splitting_leaf)
                             new_distance = distances[pair]
                         distances[(l, current_node)] = new_distance
                         distances[(l, current_node + 1)] = new_distance
                         del distances[pair]
                 distances[(current_node, current_node + 1)] = 0
 
-            leaves.add(current_node)
-            leaves.add(current_node + 1)
-            leaves.remove(splitting_leaf)
+            extant_taxa.add(current_node)
+            extant_taxa.add(current_node + 1)
+            extant_taxa.remove(splitting_leaf)
             del leaf_rates[splitting_leaf]
             current_node += 2
 
         elif (
             random_number
             < (current_extinction_rate + current_speciation_rate) / total_rate
         ):
             ######################
             #     Extinction     #
             ######################
             if not simple_output:
                 print("extinction")
 
-            random_number = random.random() * current_extinction_rate
+            random_number = seed.random() * current_extinction_rate
             for leaf, rates in leaf_rates.items():
                 if random_number < rates[1]:
                     extinction_leaf = leaf
                     break
                 random_number -= rates[1]
             if extinction_leaf == None:
                 if not simple_output:
@@ -327,66 +429,66 @@
             # Update the rates and distances
             # rates
             current_speciation_rate -= leaf_rates[extinction_leaf][0]
             current_extinction_rate -= leaf_rates[extinction_leaf][1]
             current_hgt_rate -= leaf_rates[extinction_leaf][2]
             # distances
             if hyb_used:
-                for l in leaves:
+                for l in extant_taxa:
                     if l != extinction_leaf:
                         if (extinction_leaf, l) in distances.keys():
                             del distances[(extinction_leaf, l)]
                         else:
                             del distances[(l, extinction_leaf)]
 
             del leaf_rates[extinction_leaf]
-            leaves.remove(extinction_leaf)
+            extant_taxa.remove(extinction_leaf)
             no_of_extinct += 1
 
         elif (
             random_number
             < (current_extinction_rate + current_speciation_rate + current_hgt_rate)
             / total_rate
         ):
             ######################
             #      HGT event     #
             ######################
             if not simple_output:
                 print("HGT")
 
-            random_number = random.random() * current_hgt_rate
+            random_number = seed.random() * current_hgt_rate
             for leaf, rates in leaf_rates.items():
                 if random_number < rates[2]:
                     hgt_acceptor_leaf = leaf
                     break
                 random_number -= rates[2]
             if hgt_acceptor_leaf == None:
                 if not simple_output:
                     print("ouch, hgt rate computed wrong")
-            if len(leaves) > 1:
-                hgt_donor_leaf = random.sample(leaves - set([hgt_acceptor_leaf]), 1)[0]
+            if len(extant_taxa) > 1:
+                hgt_donor_leaf = seed.choice(list(extant_taxa - set([hgt_acceptor_leaf])))
                 for p in nw.predecessors(hgt_acceptor_leaf):
                     parent_acceptor = p
                 nw.add_weighted_edges_from(
                     [
                         (hgt_donor_leaf, hgt_acceptor_leaf, 0),
                         (hgt_donor_leaf, current_node, 0),
                         (hgt_acceptor_leaf, current_node + 1, 0),
                     ],
-                    weight="length",
+                    weight=LENGTH_ATTR,
                 )
-                prob = hgt_inheritance * random.random()
-                nw[parent_acceptor][hgt_acceptor_leaf]["prob"] = 1 - prob
-                nw[hgt_donor_leaf][hgt_acceptor_leaf]["prob"] = prob
+                prob = hgt_inheritance * seed.random()
+                nw[parent_acceptor][hgt_acceptor_leaf][PROBABILITY_ATTR] = 1 - prob
+                nw[hgt_donor_leaf][hgt_acceptor_leaf][PROBABILITY_ATTR] = prob
 
                 hybrid_nodes[hgt_acceptor_leaf] = no_of_hybrids
                 no_of_hybrids += 1
                 # Update the rates and distances
                 # rates
-                leaf_rates[current_node + 1] = CalculateAllNewRates(
+                leaf_rates[current_node + 1] = update_all_rates(
                     tuple(
                         prob * x + (1 - prob) * y
                         for x, y in zip(
                             leaf_rates[hgt_acceptor_leaf], leaf_rates[hgt_donor_leaf]
                         )
                     ),
                     update_shape,
@@ -394,14 +496,15 @@
                     speciation_rate_shape,
                     ext_used,
                     extinction_rate_mean,
                     extinction_rate_shape,
                     hgt_used,
                     hgt_rate_mean,
                     hgt_rate_shape,
+                    seed=seed,
                 )
                 leaf_rates[current_node] = leaf_rates[hgt_donor_leaf]
                 current_speciation_rate += (
                     leaf_rates[current_node + 1][0] - leaf_rates[hgt_acceptor_leaf][0]
                 )
                 current_extinction_rate += (
                     leaf_rates[current_node + 1][1] - leaf_rates[hgt_acceptor_leaf][1]
@@ -409,15 +512,15 @@
                 current_hgt_rate += (
                     leaf_rates[current_node + 1][2] - leaf_rates[hgt_acceptor_leaf][2]
                 )
                 del leaf_rates[hgt_donor_leaf]
                 del leaf_rates[hgt_acceptor_leaf]
                 # distances
                 if hyb_used:
-                    for l in leaves:
+                    for l in extant_taxa:
                         if l != hgt_acceptor_leaf:
                             acceptor_pair = (hgt_acceptor_leaf, l)
                             if acceptor_pair in distances.keys():
                                 acceptor_distance = distances[acceptor_pair]
                             else:
                                 acceptor_pair = (l, hgt_acceptor_leaf)
                                 acceptor_distance = distances[acceptor_pair]
@@ -435,91 +538,92 @@
                                 1 - prob
                             ) * acceptor_distance + prob * donor_distance
                             del distances[acceptor_pair]
                     distances[(current_node, current_node + 1)] = distances[
                         (hgt_donor_leaf, current_node + 1)
                     ]
                     del distances[(hgt_donor_leaf, current_node + 1)]
-                leaves.remove(hgt_donor_leaf)
-                leaves.remove(hgt_acceptor_leaf)
-                leaves.add(current_node)
-                leaves.add(current_node + 1)
+                extant_taxa.remove(hgt_donor_leaf)
+                extant_taxa.remove(hgt_acceptor_leaf)
+                extant_taxa.add(current_node)
+                extant_taxa.add(current_node + 1)
                 current_node += 2
 
         #        else:
         #            print("trying HGT with only one leaf")
         #             #Do nothing, there is only one leaf.
 
         else:
             ######################
             #    Hybridization   #
             ######################
             if not simple_output:
                 print("hybridization")
             # i.e.: pick two leaf nodes, create a hybrid between these two leaves
-            random_number = random.random() * current_hybridization_rate
+            random_number = seed.random() * current_hybridization_rate
             for pair, distance in distances.items():
-                pair_rate = DistanceToRate(
+                pair_rate = graph_distance_to_hybridization_rate(
                     distance,
                     hybridization_left_bound,
                     hybridization_right_bound,
                     hybridization_left_rate,
                     hybridization_right_rate,
                 )
                 if random_number < pair_rate:
                     hyb_pair = pair
                     break
                 random_number -= pair_rate
             if hyb_pair == None and not simple_output:
-                if len(leaves) == 1:
+                if len(extant_taxa) == 1:
                     print("ah, no leaves for hyb")
                 else:
                     print("ouch, hybridization rate computed wrong")
             nw.add_weighted_edges_from(
                 [
                     (current_node, current_node + 1, 0),
                     (hyb_pair[0], current_node, 0),
                     (hyb_pair[1], current_node, 0),
                     (hyb_pair[0], current_node + 2, 0),
                     (hyb_pair[1], current_node + 3, 0),
                 ],
-                weight="length",
+                weight=LENGTH_ATTR,
             )
-            prob = random.random()
-            nw[hyb_pair[0]][current_node]["prob"] = prob
-            nw[hyb_pair[1]][current_node]["prob"] = 1 - prob
+            prob = seed.random()
+            nw[hyb_pair[0]][current_node][PROBABILITY_ATTR] = prob
+            nw[hyb_pair[1]][current_node][PROBABILITY_ATTR] = 1 - prob
             hybrid_nodes[current_node] = no_of_hybrids
             no_of_hybrids += 1
 
             # Update the rates and distances
             # rates
-            leaf_rates[current_node + 1] = CalculateAllNewRates(
+            leaf_rates[current_node + 1] = update_all_rates(
                 tuple(
                     prob * x + (1 - prob) * y
                     for x, y in zip(leaf_rates[hyb_pair[0]], leaf_rates[hyb_pair[1]])
                 ),
                 update_shape,
                 speciation_rate_mean,
                 speciation_rate_shape,
                 ext_used,
                 extinction_rate_mean,
                 extinction_rate_shape,
                 hgt_used,
                 hgt_rate_mean,
                 hgt_rate_shape,
+                seed=seed,
             )
             leaf_rates[current_node + 2] = leaf_rates[hyb_pair[0]]
             leaf_rates[current_node + 3] = leaf_rates[hyb_pair[1]]
             current_speciation_rate += leaf_rates[current_node + 1][0]
             current_extinction_rate += leaf_rates[current_node + 1][1]
             current_hgt_rate += leaf_rates[current_node + 1][2]
             # distances
             # TODO FIXED?!: The order may still be wrong. It seems I already delete some distances when I still need them later.
             # These are probably the distances related to the hybrid parent species.
-            for l in leaves:
+            for l in extant_taxa:
                 if l == hyb_pair[0]:
                     pair_0_distance = 0
                 else:
                     pair_0 = (hyb_pair[0], l)
                     if pair_0 not in distances.keys():
                         pair_0 = (l, hyb_pair[0])
                     pair_0_distance = distances[pair_0]
@@ -558,36 +662,36 @@
                 if hyb_pair[0] in pair or hyb_pair[1] in pair:
                     remove_pairs += [pair]
             for pair in remove_pairs:
                 del distances[pair]
 
             del leaf_rates[hyb_pair[0]]
             del leaf_rates[hyb_pair[1]]
-            leaves.remove(hyb_pair[0])
-            leaves.remove(hyb_pair[1])
-            leaves.add(current_node + 1)
-            leaves.add(current_node + 2)
-            leaves.add(current_node + 3)
+            extant_taxa.remove(hyb_pair[0])
+            extant_taxa.remove(hyb_pair[1])
+            extant_taxa.add(current_node + 1)
+            extant_taxa.add(current_node + 2)
+            extant_taxa.add(current_node + 3)
             current_node += 4
 
         # Now extend all pendant edges of extant taxa
-        if len(leaves) == 0:
+        if len(extant_taxa) == 0:
             break
-        for l in leaves:
+        for l in extant_taxa:
             pl = -1
             for p in nw.predecessors(l):
                 pl = p
-            nw[pl][l]["length"] += extra_time
+            nw[pl][l][LENGTH_ATTR] += extra_time
 
         # Compute the new rates
         current_hybridization_rate = 0
         if hyb_used:
             for pair, distance in distances.items():
                 distances[pair] += 2 * extra_time
-                current_hybridization_rate += DistanceToRate(
+                current_hybridization_rate += graph_distance_to_hybridization_rate(
                     distances[pair],
                     hybridization_left_bound,
                     hybridization_right_bound,
                     hybridization_left_rate,
                     hybridization_right_rate,
                 )
 
@@ -595,25 +699,25 @@
             current_speciation_rate
             + current_extinction_rate
             + current_hgt_rate
             + current_hybridization_rate
         )
 
         # Compute the time of the next event
-        extra_time = np.random.exponential(1 / total_rate)
+        extra_time = seed.exponential(1 / total_rate)
         current_time += extra_time
 
     # The following corrects for overshooting the time limit
     extra_time += time_limit - current_time
     # nothing has happened yet, and there is only one node
     if len(nw) == 1:
-        nw.add_weighted_edges_from([(0, 1, time_limit)], weight="length")
-        leaves = set([1])
+        nw.add_weighted_edges_from([(0, 1, time_limit)], weight=LENGTH_ATTR)
+        extant_taxa = set([1])
     # each leaf has a parent node, and we can extend each parent edge to time_limit
     else:
-        for l in leaves:
+        for l in extant_taxa:
             pl = -1
             for p in nw.predecessors(l):
                 pl = p
-            nw[pl][l]["length"] += extra_time
+            nw[pl][l][LENGTH_ATTR] += extra_time
 
-    return nw, hybrid_nodes, leaves, no_of_extinct
+    return nw, hybrid_nodes, extant_taxa, no_of_extinct
```

### Comparing `phylox-1.0.3/src/phylox/generators/heath/heath_cli.py` & `phylox-1.0.5/src/phylox/generators/heath/heath_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,65 +5,71 @@
 import sys
 
 import networkx as nx
 import numpy as np
 import scipy.stats
 
 # from AddEdgesToTree import *
-from phylox.generators.heath.heath import RestrictToLeafSet, generate_heath_network
+from phylox.generators.heath.heath import (
+    restrict_network_to_leaf_set,
+    generate_heath_network,
+)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description="""
         Runs a speciation-extinction-HGT-hybridization model for the given time (--time) or until a certain number of extant taxa (--taxa) is reached. If all lineages go extinct before the given time is reached, another attempt is made.
-        
-        Each extant taxon has its own speciation, HGT, and extinction rates (1/mean_time_until_next_event). 
-        
-        The hybridization rate of a pair of species is a function of the weighed distance between these species (sum of all up-down distances, weighed by their probability). 
-        
-        There are prior speciation/extinction/HGT rate distributions: gamma distributions with a given mean and a shape parameter for speciation (--speciation_parameters) and extinction (--extinction_parameters), HGT is turned off by default. 
-        
-        If a HGT event happens for a given taxon, another taxon (including itself) is chosen uniformly at random to donate genetic material (uniformly distributed contribution in [0,max_hgt] where max_hgt is determined by the --hgt_inheritance parameter). After speciation or hybridization, each rate of the new lineages is set by multiplying the (weighted mean) rate of the parent lineage(s) by a gamma-distributed factor with mean 1 and a shape parameter (--update-shape-parameter), and then accepting this rate with a probability proportional to the prior distribution for this rate. This gives an ultrametric network on the extant species.
-        
+
+        Each extant taxon has its own speciation, HGT, and extinction rates (1/mean_time_until_next_event).
+
+        The hybridization rate of a pair of species is a function of the weighed distance between these species (sum of all up-down distances, weighed by their probability).
+
+        There are prior speciation/extinction/HGT rate distributions: gamma distributions with a given mean and a shape parameter for speciation (--speciation_parameters) and extinction (--extinction_parameters), HGT is turned off by default.
+
+        If an HGT event happens for a given taxon, another taxon (including itself) is chosen uniformly at random to donate genetic material (uniformly distributed contribution in [0,max_hgt] where max_hgt is determined by the --hgt_inheritance parameter). After speciation or hybridization, each rate of the new lineages is set by multiplying the (weighted mean) rate of the parent lineage(s) by a gamma-distributed factor with mean 1 and a shape parameter (--update-shape-parameter), and then accepting this rate with a probability proportional to the prior distribution for this rate. This gives an ultrametric network on the extant species.
+
         Optional arguments:
-            -ti or --time followed by the total length (float) for the network. 
+            -ti or --time followed by the total length (float) for the network.
             -ta or --taxa followed by the number of taxa at which the simulation stops. If all lineages go extinct before the given number of taxa is reached, another attempt is made.
-            -ce or --count_extinct to also count the extinct taxa as part of the taxa limit.-oe or --only_extant to return the network restricted to the extant leaves
+            -ce or --count_extinct to also count the extinct taxa as part of the taxa limit.
+            -oe or --only_extant to return the network restricted to the extant leaves
         Rates:
             -sp or --speciation_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the speciation rate.
             -ext or --extinction_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the extinction rate.
             -noext or --no_extinction to turn off extinction altogether.
             -hgt or --hgt_parameters followed by a mean (float) and a shape parameter (float) for the gamma distribution of the HGT rate.
             -upd or --update_shape_parameter followed by a shape parameter (float) for the update gamma distribution.
             -hyb or --hyb_factor followed by four floats for the piecewise linear dependence of hybridization rate on the distance:
 
         left bound:  l
         right bound: r
         left rate:   rl
         right rate:  rr.
-        
-        |
-        lr+---
-        |     \
-        |      \
-        |       \
-        rr+      -----
-        |
-        0 +---+----+-----
-        0   l    r""",
+
+           |
+        lr +---
+           |   \\
+           |    \\
+           |     \\
+        rr +      -----
+           |
+         0 +---+----+-----
+           0   l    r
+        """,
         formatter_class=argparse.RawTextHelpFormatter,
     )
 
     parser.add_argument(
         "-ti",
         "--time",
         dest="time_limit",
         type=float,
         help="Total length for the network",
+        default=1.0,
     )
     parser.add_argument(
         "-ta",
         "--taxa",
         dest="taxa_limit",
         type=float,
         help="Number of taxa at which the simulation stops",
@@ -71,28 +77,36 @@
     parser.add_argument(
         "-ce",
         "--count_extinct",
         action="store_true",
         help="Count extinct taxa as part of the taxa limit",
     )
     parser.add_argument(
+        "-oe",
+        "--only_extant",
+        action="store_true",
+        help="Return the generated network restricted to the extant leaves, by removing extinct species and cleaning up the network.",
+    )
+    parser.add_argument(
         "-sp",
         "--speciation_parameters",
         nargs=2,
         type=float,
         metavar=("mean", "shape"),
         help="Mean and shape parameter for the gamma distribution of the speciation rate",
+        default=(2.0, 2.0),
     )
     parser.add_argument(
         "-ext",
         "--extinction_parameters",
         nargs=2,
         type=float,
         metavar=("mean", "shape"),
         help="Mean and shape parameter for the gamma distribution of the extinction rate",
+        default=(1.0, 1.0)
     )
     parser.add_argument(
         "-noext",
         "--no_extinction",
         action="store_true",
         help="Turn off extinction altogether",
     )
@@ -104,97 +118,114 @@
         metavar=("mean", "shape"),
         help="Mean and shape parameter for the gamma distribution of the HGT rate",
     )
     parser.add_argument(
         "--hgt_inheritance",
         type=float,
         help="Maximum contribution of a donor taxon to the genome of the recipient taxon",
+        default=.05,
     )
     parser.add_argument(
         "-hyb",
         "--hybridization_factor",
         nargs=4,
         type=float,
         metavar=("l", "r", "rl", "rr"),
         help="Piecewise linear dependence of hybridization rate on the distance",
     )
     parser.add_argument(
         "-upd",
         "--update_shape_parameter",
         type=float,
         help="Shape parameter for the update gamma distribution",
+        default=2.0,
+    )
+    parser.add_argument(
+        "-s",
+        "--seed",
+        type=int,
+        help="Seed for the random generator",
+        default=1,
     )
     parser.add_argument(
-        "-s", "--simple", action="store_true", help="Enable simple output"
+        "-si", "--simple", action="store_true", help="Enable simple output: i.e. less print statements"
     )
 
     args = parser.parse_args()
 
     params = {
         "time_limit": args.time_limit,
         "taxa_limit": args.taxa_limit,
         "count_extinct": args.count_extinct,
-        "speciation_rate_mean": args.speciation_parameters[0]
-        if args.speciation_parameters
-        else None,
-        "speciation_rate_shape": args.speciation_parameters[1]
-        if args.speciation_parameters
-        else None,
-        "extinction_rate_mean": args.extinction_parameters[0]
-        if args.extinction_parameters
-        else None,
-        "extinction_rate_shape": args.extinction_parameters[1]
-        if args.extinction_parameters
-        else None,
+        "only_extant": args.only_extant,
+        "speciation_rate_mean": (
+            args.speciation_parameters[0] if args.speciation_parameters else None
+        ),
+        "speciation_rate_shape": (
+            args.speciation_parameters[1] if args.speciation_parameters else None
+        ),
+        "extinction_rate_mean": (
+            args.extinction_parameters[0] if args.extinction_parameters else None
+        ),
+        "extinction_rate_shape": (
+            args.extinction_parameters[1] if args.extinction_parameters else None
+        ),
         "ext_used": not args.no_extinction,
         "hgt_rate_mean": args.hgt_parameters[0] if args.hgt_parameters else None,
         "hgt_rate_shape": args.hgt_parameters[1] if args.hgt_parameters else None,
         "hgt_used": args.hgt_parameters is not None,
-        "hybridization_left_bound": args.hybridization_factor[0]
-        if args.hybridization_factor
-        else None,
+        "hybridization_left_bound": (
+            args.hybridization_factor[0] if args.hybridization_factor else None
+        ),
         "hgt_inheritance": args.hgt_inheritance,
-        "hybridization_right_bound": args.hybridization_factor[1]
-        if args.hybridization_factor
-        else None,
-        "hybridization_left_rate": args.hybridization_factor[2]
-        if args.hybridization_factor
-        else None,
-        "hybridization_right_rate": args.hybridization_factor[3]
-        if args.hybridization_factor
-        else None,
+        "hybridization_right_bound": (
+            args.hybridization_factor[1] if args.hybridization_factor else None
+        ),
+        "hybridization_left_rate": (
+            args.hybridization_factor[2] if args.hybridization_factor else None
+        ),
+        "hybridization_right_rate": (
+            args.hybridization_factor[3] if args.hybridization_factor else None
+        ),
         "hyb_used": args.hybridization_factor is not None,
         "update_shape": args.update_shape_parameter,
         "simple_output": args.simple,
+        "seed": args.seed,
     }
     return params
 
 
 def main():
+    """
+    A command line tool `phylox-generator-heath` for generating networks with the heath generator in this module.
+    Type `phylox-generator-heath --help` in the command line for usage guidance.
+    """
     params = parse_args()
+    generator_params = {**params}
+    generator_params.pop("only_extant")
     # Find a network
     if params["taxa_limit"]:
         leaves = []
         no_of_extinct = 0
         while (
             len(leaves) + params["count_extinct"] * no_of_extinct
             != params["taxa_limit"]
         ):
             if not params["simple_output"]:
                 print("starting over")
             network, hybrid_nodes, leaves, no_of_extinct = generate_heath_network(
-                **params
+                **generator_params
             )
     else:
-        print(params)
-        network, hybrid_nodes, leaves, no_of_extinct = generate_heath_network(**params)
+        print(generator_params)
+        network, hybrid_nodes, leaves, no_of_extinct = generate_heath_network(**generator_params)
 
     # Restrict to extant leaves if wanted
-    if only_extant:
-        network = RestrictToLeafSet(network, leaves)
+    if params["only_extant"]:
+        network = restrict_network_to_leaf_set(network, leaves)
 
     for e in network.edges:
         info = ""
         if e[0] in hybrid_nodes:
             info += "H" + str(hybrid_nodes[e[0]])
         else:
             info += str(e[0])
```

### Comparing `phylox-1.0.3/src/phylox/generators/mcmc/base.py` & `phylox-1.0.5/src/phylox/generators/mcmc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     True
     """
     network = starting_network.copy()
     current_reticulation_number = network.reticulation_number
     number_of_leaves = len(network.leaves)
     if add_root_if_necessary:
         for root in network.roots:
-            if network.out_degree(root) >= 1:
+            if network.out_degree(root) > 1:
                 new_root = find_unused_node(network)
                 network.add_edges_from([(new_root, root)])
                 root = new_root
         roots = network._set_roots()
     available_reticulations = set()
     available_tree_nodes = set()
```

### Comparing `phylox-1.0.3/src/phylox/generators/randomTC/random_tc_network.py` & `phylox-1.0.5/src/phylox/generators/randomTC/random_tc_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         if i in indices:
             newSeq.append(pair)
     return newSeq
 
 
 @py_random_state("seed")
 def generate_network_random_tree_child_sequence(
-    leaves, reticulations, label_leaves=False, seed=None
+    leaves, reticulations, label_leaves=True, seed=None
 ):
     """
     Returns a random tree-child network with a given number of leaves and reticulations
     :param leaves: number of leaves
     :param reticulations: number of reticulations
     :param label_leaves: whether to label the leaves
     :return: a random tree-child network
```

### Comparing `phylox-1.0.3/src/phylox/generators/trees/add_edges.py` & `phylox-1.0.5/src/phylox/generators/trees/add_edges.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/generators/trees/beta_splitting_tree.py` & `phylox-1.0.5/src/phylox/generators/trees/beta_splitting_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from phylox import DiNetwork
 from phylox.constants import LABEL_ATTR
 
 ############################################
 # Simulation functions
 ############################################
 
+
 # _a_n is a normalizing constant defined in
 # Equation (2) of Aldous1996 (so the sum of
 # the values is equal to 1. It is not
 # computed here to save time.
 def _a_n(beta):
     return 1
```

### Comparing `phylox-1.0.3/src/phylox/generators/trees/well_known.py` & `phylox-1.0.5/src/phylox/generators/trees/well_known.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/generators/zods/zods.py` & `phylox-1.0.5/src/phylox/generators/zods/zods.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/generators/zods/zods_cli.py` & `phylox-1.0.5/src/phylox/generators/zods/zods_cli.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/isomorphism/base.py` & `phylox-1.0.5/src/phylox/isomorphism/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #: The node attribute used to store the isometry label of a node.
 ISOMETRY_LABEL_ATTR = "isometry_label"
 #: The prefix used for isometry labels.
 ISOMETRY_LABEL_PREFIX = "isometry_label_prefix_"
 #: The prefix used for automorphism labels.
 AUTOMORPHISM_LABEL_PREFIX = "automorphism_label_prefix_"
 
+
 # Checks whether the nodes with the given attributes have the same label
 def _same_isometry_labels(node1_attributes, node2_attributes):
     """
     Checks whether two nodes have the same label
 
     :param node1_attributes: the attributes of a node
     :param node2_attributes: the attributes of a node
```

### Comparing `phylox-1.0.3/src/phylox/networkproperties/properties.py` & `phylox-1.0.5/src/phylox/networkproperties/properties.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/parser.py` & `phylox-1.0.5/src/phylox/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import json
 import re
 from copy import deepcopy
 
 from phylox import DiNetwork
 from phylox.base import find_unused_node
-from phylox.constants import LABEL_ATTR, LENGTH_ATTR, RETIC_PREFIX
+from phylox.constants import LABEL_ATTR, LENGTH_ATTR, PROBABILITY_ATTR, RETIC_PREFIX
 
 
-def dinetwork_to_extended_newick(network):
+def dinetwork_to_extended_newick(network, simple=False):
     """
     Converts a phylogenetic network to a Newick string.
     The newick string has :length:bootstrap:probability annotations if any edge has a bootstrap or probability.
     If only lengths are available, the newick string has :length annotations.
 
     :param network: a phylogenetic network, i.e., a phylox DiNetwork.
+    :param simple: Boolean, indicating whether to create a simple newick string without parameters
     :return: a string in extended Newick format for phylogenetic networks.
 
     :example:
     >>> from phylox import DiNetwork
     >>> from phylox.constants import LENGTH_ATTR
     >>> from phylox.parser import dinetwork_to_extended_newick
     >>> network = DiNetwork(
@@ -52,33 +53,33 @@
     has_lengths = any(
         LENGTH_ATTR in cut_network[parent][child] for parent, child in cut_network.edges
     )
     has_bootstraps = any(
         "bootstrap" in cut_network[parent][child] for parent, child in cut_network.edges
     )
     has_probabilities = any(
-        "probability" in cut_network[parent][child]
+        PROBABILITY_ATTR in cut_network[parent][child]
         for parent, child in cut_network.edges
     )
 
     def node_to_newick(node):
         node_label = cut_network.nodes[node].get(LABEL_ATTR, "")
 
         if cut_network.is_leaf(node):
             return node_label
 
         children_strings = []
         for child in cut_network.successors(node):
-            child_str = node_to_newick(child)
-            if has_bootstraps or has_probabilities:
+            child_str = str(node_to_newick(child))
+            if (has_bootstraps or has_probabilities) and not simple:
                 length = cut_network[node][child].get(LENGTH_ATTR, "")
                 bootstrap = cut_network[node][child].get("bootstrap", "")
-                probability = cut_network[node][child].get("probability", "")
+                probability = cut_network[node][child].get(PROBABILITY_ATTR, "")
                 child_str += f":{length}:{bootstrap}:{probability}"
-            elif has_lengths:
+            elif has_lengths and not simple:
                 child_str += f":{cut_network[node][child].get(LENGTH_ATTR, '')}"
             children_strings.append(child_str)
 
         return "(" + ",".join(children_strings) + ")" + node_label
 
     newick = node_to_newick(root)
     return newick + ";"
@@ -92,15 +93,15 @@
     :param node: a node of network, indicating the reticulation node to be split.
     :return: a phylogenetic network, i.e., a phylox DiNetwork.
 
     :note: This function is used by dinetwork_to_extended_newick. It modifies the network in place.
     """
 
     parents = [
-        (parent, network[parent][node].get("probability", 0))
+        (parent, network[parent][node].get(PROBABILITY_ATTR, 0))
         for parent in network.predecessors(node)
     ]
     parents.sort(key=lambda x: -x[1])
     keep_parent, keep_probability = parents[0]
     node_label = network.nodes[node].get(LABEL_ATTR, "")
     network.nodes[node][LABEL_ATTR] = node_label + "#R" + str(retic_id)
     new_node_label = node_label + "#H" + str(retic_id)
@@ -111,17 +112,17 @@
 
         length = network[parent][node].get(LENGTH_ATTR)
         if length is not None:
             network[parent][new_node][LENGTH_ATTR] = length
         bootstrap = network[parent][node].get("bootstrap")
         if bootstrap is not None:
             network[parent][new_node]["bootstrap"] = bootstrap
-        probability = network[parent][node].get("probability")
+        probability = network[parent][node].get(PROBABILITY_ATTR)
         if probability is not None:
-            network[parent][new_node]["probability"] = probability
+            network[parent][new_node][PROBABILITY_ATTR] = probability
         network.remove_edge(parent, node)
     return network
 
 
 def extended_newick_to_dinetwork(newick, internal_labels=False):
     """
     Converts a Newick string to a networkx DAG with leaf labels.
@@ -190,52 +191,54 @@
     :note: This function is used by extended_newick_to_dinetwork. It modifies the network in place.
     """
     network = network or DiNetwork()
 
     node_attrs = _label_and_attrs_to_dict(json["label_and_attr"])
     node = json.get("retic_id") or root_node or find_unused_node(network)
     network.add_node(node)
-    if "label" in node_attrs:
-        network.nodes[node]["label"] = node_attrs["label"]
+    if LABEL_ATTR in node_attrs:
+        network.nodes[node][LABEL_ATTR] = node_attrs[LABEL_ATTR]
     for child_dict in json.get("children", []):
         child_attrs = _label_and_attrs_to_dict(child_dict["label_and_attr"])
         child_attrs_without_label_and_children = {
             k: v
             for k, v in child_attrs.items()
-            if k not in ("label", "children", "retic_id")
+            if k not in (LABEL_ATTR, "children", "retic_id")
         }
         child = child_attrs.get("retic_id", find_unused_node(network))
         network.add_edge(node, child, **child_attrs_without_label_and_children)
         _json_to_dinetwork(child_dict, network, root_node=child)
     return network
 
 
 def _label_and_attrs_to_dict(label_and_attrs):
     """
     converts the label and attr part of an extended newick string
     for one node to a dictionary.
     For example, the string "A:1.1:0.9:0.8" is converted to
     {"label": "A", "length": 1.1, "bootstrap": 0.9, "probability": 0.8}
     """
-    attrs_dict = {"label": label_and_attrs}
+    attrs_dict = {LABEL_ATTR: label_and_attrs}
     if ":" in label_and_attrs:
         label = label_and_attrs.split(":")[0]
         attrs = label_and_attrs.split(":")[1:]
         if len(attrs) == 1:
             attrs_dict = {
-                "label": label,
-                "length": float(attrs[0]),
+                LABEL_ATTR: label,
+                LENGTH_ATTR: float(attrs[0]),
             }
         elif len(attrs) == 3:
-            attrs_dict = {
-                "label": label,
-                "length": float(attrs[0]),
-                "bootstrap": float(attrs[1]),
-                "probability": float(attrs[2]),
-            }
-    if "#" in attrs_dict["label"]:
-        label, retic_id = attrs_dict["label"].split("#")
-        attrs_dict["label"] = label
+            attrs_dict = {LABEL_ATTR: label}
+            if attrs[0]:
+                attrs_dict[LENGTH_ATTR] = float(attrs[0])
+            if attrs[1]:
+                attrs_dict["bootstrap"] = float(attrs[1])
+            if attrs[2]:
+                attrs_dict[PROBABILITY_ATTR] = float(attrs[2])
+
+    if "#" in attrs_dict[LABEL_ATTR]:
+        label, retic_id = attrs_dict[LABEL_ATTR].split("#")
+        attrs_dict[LABEL_ATTR] = label
         attrs_dict["retic_id"] = RETIC_PREFIX + retic_id[1:]
-    if "label" in attrs_dict and attrs_dict["label"] == "":
-        attrs_dict.pop("label")
+    if LABEL_ATTR in attrs_dict and attrs_dict[LABEL_ATTR] == "":
+        attrs_dict.pop(LABEL_ATTR)
     return attrs_dict
```

### Comparing `phylox-1.0.3/src/phylox/rearrangement/__init__.py` & `phylox-1.0.5/src/phylox/rearrangement/__init__.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/exact_distance/base.py` & `phylox-1.0.5/src/phylox/rearrangement/exact_distance/base.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/heuristics/__init__.py` & `phylox-1.0.5/src/phylox/rearrangement/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/heuristics/cli_main.py` & `phylox-1.0.5/src/phylox/rearrangement/heuristics/cli_main.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/heuristics/green_line_heuristic.py` & `phylox-1.0.5/src/phylox/rearrangement/heuristics/green_line_heuristic.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/heuristics/red_line_heuristic.py` & `phylox-1.0.5/src/phylox/rearrangement/heuristics/red_line_heuristic.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/heuristics/utils.py` & `phylox-1.0.5/src/phylox/rearrangement/heuristics/utils.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/invertsequence.py` & `phylox-1.0.5/src/phylox/rearrangement/invertsequence.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/movability.py` & `phylox-1.0.5/src/phylox/rearrangement/movability.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/move.py` & `phylox-1.0.5/src/phylox/rearrangement/move.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox/rearrangement/rearrangementproblem.py` & `phylox-1.0.5/src/phylox/rearrangement/rearrangementproblem.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/src/phylox.egg-info/PKG-INFO` & `phylox-1.0.5/src/phylox.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylox
-Version: 1.0.3
+Version: 1.0.5
 Summary: A package with tools for constructing, manipulating, and analyzing phylogenetic networks.
 Author-email: Remie Janssen <remiejanssen92@gmail.com>
 Project-URL: Homepage, https://github.com/RemieJanssen/PhyloX
 Project-URL: Bug Tracker, https://github.com/RemieJanssen/PhyloX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,12 +67,28 @@
 ### Linting
 
 precommit is yet to be configured, for now, simply run black and isort.
 
 ### Documentation
 
 Documentation is in the docs folder, and is created uses sphinx.
-to build the documentation, go to the docs folder and do:
+
+#### Requirements
+You may need to install the requirements from `docs/requirements.txt` first. Make sure to use python<=3.11.*, for example:
+```
+conda create -n phylox-sphinx
+conda activate phylox-sphinx
+python install python==3.11.*
+pip install -r docs/requirements.txt
+```
+
+#### Creating documentation
+to build the documentation, go to the docs folder and run:
 ```
 make html
 ```
 the docs will be in `docs/build/html`.
+
+If you re-run the build, you can first remove the old autosummary files. If you do not, it will not update them.
+
+
+
```

### Comparing `phylox-1.0.3/src/phylox.egg-info/SOURCES.txt` & `phylox-1.0.5/src/phylox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/phylox/classes/networkclass.py
 src/phylox/exceptions/__init__.py
 src/phylox/exceptions/invalidmovedefinitionexception.py
 src/phylox/exceptions/invalidmoveexception.py
 src/phylox/exceptions/nosolutionexception.py
 src/phylox/exceptions/timeoutexception.py
 src/phylox/generators/__init__.py
+src/phylox/generators/heath/__init__.py
 src/phylox/generators/heath/heath.py
 src/phylox/generators/heath/heath_cli.py
 src/phylox/generators/lgt/__init__.py
 src/phylox/generators/lgt/base.py
 src/phylox/generators/mcmc/__init__.py
 src/phylox/generators/mcmc/base.py
 src/phylox/generators/randomTC/__init__.py
```

### Comparing `phylox-1.0.3/tests/test_dinetwork.py` & `phylox-1.0.5/tests/test_dinetwork.py`

 * *Files identical despite different names*

### Comparing `phylox-1.0.3/tests/test_parser.py` & `phylox-1.0.5/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,43 @@
         )
         self.assertTrue(is_isomorphic(network, network2))
         node_a = network.label_to_node_dict["a"]
         parent_a = network.parent(node_a)
         self.assertEqual(network[parent_a][node_a]["length"], 1.0)
 
     def test_small_tree_with_more_attrs(self):
+        newick = "(a:::3.0,b:1.1,(c,d:1.3)::1.4:);"
+        network = extended_newick_to_dinetwork(newick)
+        print(network.edges)
+        network2 = DiNetwork(
+            edges=[(1, 2), (1, 3), (1, 4), (4, 5), (4, 6)],
+            labels=[(2, "a"), (3, "b"), (5, "c"),(6, "d")],
+        )
+        self.assertTrue(is_isomorphic(network, network2))
+        node_a = network.label_to_node_dict["a"]
+        parent_a = network.parent(node_a)
+        self.assertEqual(network[parent_a][node_a].get("length"), None)
+        self.assertEqual(network[parent_a][node_a].get("bootstrap"), None)
+        self.assertEqual(network[parent_a][node_a]["probability"], 3.0)
+
+    def test_small_tree_with_partial_attrs(self):
         newick = "(a:1.0:2.0:3.0,b:1.1,(c:1.2,d:1.3):1.4);"
         network = extended_newick_to_dinetwork(newick)
         network2 = DiNetwork(
             edges=[(1, 2), (1, 3), (1, 4), (4, 5), (4, 6)],
             labels=[(2, "a"), (3, "b"), (5, "c"), (6, "d")],
         )
         self.assertTrue(is_isomorphic(network, network2))
         node_a = network.label_to_node_dict["a"]
         parent_a = network.parent(node_a)
         self.assertEqual(network[parent_a][node_a]["length"], 1.0)
         self.assertEqual(network[parent_a][node_a]["bootstrap"], 2.0)
         self.assertEqual(network[parent_a][node_a]["probability"], 3.0)
 
+
     def test_network(self):
         newick = "(a,(b)#R1,(#H1,c));"
         network = extended_newick_to_dinetwork(newick)
         network2 = DiNetwork(
             edges=[(1, 2), (1, 3), (3, 7), (1, 4), (4, 3), (4, 6)],
             labels=[(2, "a"), (7, "b"), (6, "c")],
         )
```

