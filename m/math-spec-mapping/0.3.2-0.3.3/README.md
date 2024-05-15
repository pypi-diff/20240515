# Comparing `tmp/math_spec_mapping-0.3.2.tar.gz` & `tmp/math_spec_mapping-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_spec_mapping-0.3.2.tar", last modified: Mon May  6 21:45:46 2024, max compression
+gzip compressed data, was "math_spec_mapping-0.3.3.tar", last modified: Wed May 15 18:33:39 2024, max compression
```

## Comparing `math_spec_mapping-0.3.2.tar` & `math_spec_mapping-0.3.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.846809 math_spec_mapping-0.3.2/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.2/LICENSE
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-06 21:45:46.846566 math_spec_mapping-0.3.2/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/README.md
--rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-04-20 18:11:50.000000 math_spec_mapping-0.3.2/pyproject.toml
--rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-05-06 21:45:46.846855 math_spec_mapping-0.3.2/setup.cfg
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.811201 math_spec_mapping-0.3.2/src/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.812855 math_spec_mapping-0.3.2/src/math_spec_mapping/
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.838460 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    17302 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Block.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/BoundaryAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/ControlAction.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Entity.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    28854 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/MathSpec.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Metric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Parameter.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Space.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1538 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/State.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/StatefulMetric.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/__init__.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.839409 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      112 2024-05-05 21:14:39.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1625 2024-05-05 21:14:18.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/documentation.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    11010 2024-05-06 05:19:05.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/starter.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.843364 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/
--rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/action_transmission_channel.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2058 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/displays.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1208 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/entities.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/implementations.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/load.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/mechanism.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1393 2024-05-06 21:03:12.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/policy.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/state_update_transmission_channels.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/stateful_metrics.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1290 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/states.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     4356 2024-05-06 05:20:31.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/type.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Load/wiring.py
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.846065 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/
--rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/boundary_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/control_actions.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/general.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/html.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    22505 2024-05-06 02:23:26.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/markdown.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/mechanisms.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/node_map.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/parameters.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/policies.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/spaces.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/state.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/tables.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/wiring.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      961 2024-05-05 21:12:15.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/__init__.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/schema.py
--rw-r--r--   0 seanmcowen   (501) staff       (20)    29400 2024-04-23 15:25:57.000000 math_spec_mapping-0.3.2/src/math_spec_mapping/schema.schema.json
-drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-06 21:45:46.846312 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/
--rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/PKG-INFO
--rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/requires.txt
--rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-05-06 21:45:46.000000 math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.512143 math_spec_mapping-0.3.3/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1069 2023-12-10 00:44:46.000000 math_spec_mapping-0.3.3/LICENSE
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-15 18:33:39.511880 math_spec_mapping-0.3.3/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     5511 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/README.md
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      747 2024-05-12 21:07:44.000000 math_spec_mapping-0.3.3/pyproject.toml
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       38 2024-05-15 18:33:39.512187 math_spec_mapping-0.3.3/setup.cfg
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.500648 math_spec_mapping-0.3.3/src/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.502078 math_spec_mapping-0.3.3/src/math_spec_mapping/
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.505586 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      246 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/ActionTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    17437 2024-05-15 17:30:11.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Block.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      476 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/BoundaryAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      526 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/ControlAction.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1226 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Entity.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    28854 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/MathSpec.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      379 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      581 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Metric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1237 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Parameter.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      530 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      472 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Space.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1599 2024-05-14 15:58:35.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/State.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      257 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/StateUpdateTransmissionChannel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      749 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/StatefulMetric.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      289 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      761 2024-03-31 21:59:52.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/__init__.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.506081 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      112 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1625 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/documentation.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    11010 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/starter.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.509261 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       33 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2561 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/action_transmission_channel.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2142 2024-05-14 16:01:16.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2042 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      414 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/displays.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1289 2024-05-14 15:59:52.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/entities.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4463 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      395 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/implementations.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2484 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/load.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2037 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/mechanism.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3434 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1393 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2444 2024-03-28 12:55:01.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/policy.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1116 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2238 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/state_update_transmission_channels.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1977 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/stateful_metrics.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1313 2024-05-12 21:08:43.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/states.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     4356 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/type.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3083 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Load/wiring.py
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.511448 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      933 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1410 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/boundary_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1216 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/control_actions.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1610 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/general.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     9007 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/html.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    22881 2024-05-15 17:34:54.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/markdown.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1322 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/mechanisms.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     3129 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/node_map.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      535 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/parameters.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1814 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/policies.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      579 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/spaces.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2321 2024-04-17 18:04:23.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/state.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1505 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/tables.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     1618 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/wiring.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      961 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/__init__.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)      233 2024-03-25 05:13:37.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/schema.py
+-rw-r--r--   0 seanmcowen   (501) staff       (20)    29400 2024-05-06 21:48:04.000000 math_spec_mapping-0.3.3/src/math_spec_mapping/schema.schema.json
+drwxr-xr-x   0 seanmcowen   (501) staff       (20)        0 2024-05-15 18:33:39.511653 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     6009 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 seanmcowen   (501) staff       (20)     2610 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)        1 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       44 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/requires.txt
+-rw-r--r--   0 seanmcowen   (501) staff       (20)       18 2024-05-15 18:33:39.000000 math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/top_level.txt
```

### Comparing `math_spec_mapping-0.3.2/LICENSE` & `math_spec_mapping-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/PKG-INFO` & `math_spec_mapping-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.2
+Version: 0.3.3
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.2/README.md` & `math_spec_mapping-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/pyproject.toml` & `math_spec_mapping-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "math-spec-mapping"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Sean McOwen", email="Sean@Block.Science" },
 ]
 description = "A library for easy mapping of mathematical specifications."
 dependencies = [
   "graphviz>=0.20.1",
   "ipython>=7.7.0",
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Block.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Block.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,21 +79,23 @@
     def render_ending_entities(self):
         if self.block_type == "Mechanism":
             updates = self.updates
         elif self.block_type in ["Parallel Block", "Stack Block", "Split Block"]:
             updates = self.all_updates
         else:
             return "\n", {}
+        updates = sorted(updates, key=lambda x: x[0].name + "-" + x[1].name)
 
         out = "\n"
         out += 'subgraph SVS["State Variables"]\n'
 
         # Render the entities
         entity_mapping = {}
         entities = set([x[0] for x in updates])
+        entities = sorted(entities, key=lambda x: x.name)
         for i, x in enumerate(entities):
             entity_mapping[x.name] = "EE{}".format(i)
             out += '{}[("{}")]'.format(entity_mapping[x.name], x.name)
             out += "\n"
 
         entity_variable_mapping = {}
         # Render the state variables
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/ControlAction.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/ControlAction.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Entity.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Entity.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/MathSpec.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/MathSpec.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Metric.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Metric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Parameter.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Parameter.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/Policy.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/Policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/State.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/State.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         # Iterate through
         for var in self.variables:
             key = var.name
 
             # Check variable name not repeated
             assert (
                 var.name not in self.variable_map
-            ), "Variable name {} is already present in variables!".format(key)
+            ), "Variable name {} is already present in variables for the state of {}!".format(
+                key, self.name
+            )
 
             self.variable_map[key] = var
 
 
 class StateVariable:
 
     def __init__(self, data: Dict):
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/StatefulMetric.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/StatefulMetric.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Classes/__init__.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Classes/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/documentation.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/documentation.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Convenience/starter.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Convenience/starter.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/action_transmission_channel.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/action_transmission_channel.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/boundary_actions.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/boundary_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     data["boundary_action_options"] = new_bao
 
     # Assert that the entities in called_by are in math spec
     if data["called_by"]:
         for name in data["called_by"]:
             assert (
                 name in ms["Entities"]
-            ), "{} entity not in entities dictionary".format(name)
+            ), "{} entity not in entities dictionary which is referenced in called_by for {}".format(
+                name, data["name"]
+            )
         data["called_by"] = [ms["Entities"][x] for x in data["called_by"]]
 
     data["codomain"] = tuple(ms["Spaces"][x] for x in data["codomain"])
 
     # Build the boundary action object
     return BoundaryAction(data)
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/control_actions.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/entities.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 
     # Copy
     data = data.copy()
 
     # Assert that the state is in the math spec and assign it here
     if data["state"]:
         name = data["state"]
-        assert name in ms["State"], "{} state not in states dictionary".format(name)
+        assert (
+            name in ms["State"]
+        ), "{} state not in states dictionary for the entity of {}".format(
+            name, data["name"]
+        )
         data["state"] = ms["State"][name]
 
     # Build the state object
     return Entity(data)
 
 
 def load_entities(ms: Dict, json: Dict) -> None:
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/general.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/load.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/load.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/mechanism.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/mechanism.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/metrics.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/parameters.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/parameters.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/policy.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/policy.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/spaces.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/state_update_transmission_channels.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/state_update_transmission_channels.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/stateful_metrics.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/stateful_metrics.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/states.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # Copy
     data = data.copy()
 
     # Convert the variables
     new_variables = []
     for var in data["variables"]:
         check_json_keys(var, "State Variable")
-        assert var["type"] in ms["Types"], "Type not in ms"
+        assert var["type"] in ms["Types"], "Type {} not in ms".format(var["name"])
         var["type"] = ms["Types"][var["type"]]
         if "metadata" not in var:
             var["metadata"] = {}
         new_variables.append(StateVariable(var))
     data["variables"] = new_variables
 
     # Build the state object
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/type.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/type.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Load/wiring.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Load/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/__init__.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/boundary_actions.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/boundary_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/control_actions.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/control_actions.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/general.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/general.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/html.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/html.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/markdown.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
 
     out += "## Constraints\n"
     for i, x in enumerate(policy.constraints):
         out += "{}. {}".format(i + 1, x)
         out += "\n"
 
     out += "## Parameters Used\n"
-    for i, x in enumerate(policy.parameters_used):
+    for i, x in enumerate(sorted(policy.parameters_used, key=lambda x: x)):
         out += "{}. [[{}]]".format(i + 1, x)
         out += "\n"
 
     out += "## Metrics Used\n"
     for i, x in enumerate(policy.metrics_used):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
@@ -423,15 +423,15 @@
     for i, x in enumerate(wiring.components):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
 
     out += "\n"
 
     out += "## All Blocks\n"
-    for i, x in enumerate(wiring.components_full()):
+    for i, x in enumerate(sorted(wiring.components_full(), key=lambda x: x.name)):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
 
     out += "\n"
 
     out += "## Constraints\n"
     for i, x in enumerate(wiring.constraints):
@@ -448,21 +448,21 @@
     out += "## Codomain Spaces\n"
     for i, x in enumerate(wiring.codomain):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
     out += "\n"
 
     out += "## All Spaces Used\n"
-    for i, x in enumerate(wiring.all_spaces_used):
+    for i, x in enumerate(sorted(wiring.all_spaces_used, key=lambda x: x.name)):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
     out += "\n"
 
     out += "## Parameters Used\n"
-    for i, x in enumerate(wiring.parameters_used):
+    for i, x in enumerate(sorted(wiring.parameters_used, key=lambda x: x)):
         out += "{}. [[{}]]".format(i + 1, x)
         out += "\n"
     out += "\n"
 
     out += "## Called By\n"
     for i, x in enumerate(wiring.called_by):
         out += "{}. [[{}]]".format(i + 1, x.name)
@@ -473,15 +473,17 @@
     for i, x in enumerate(wiring.calls):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
     out += "\n"
 
     out += "## All State Updates\n"
 
-    for i, x in enumerate(wiring.all_updates):
+    for i, x in enumerate(
+        sorted(wiring.all_updates, key=lambda x: x[0].name + "-" + x[1].name)
+    ):
         out += "{}. [[{}]].[[{}|{}]]".format(
             i + 1,
             x[0].name,
             ms.entities[x[0].name].state.name + "-" + x[1].name,
             x[1].name,
         )
         out += "\n"
@@ -532,15 +534,15 @@
 
     out += "Description: {}\n\n".format(metric.description)
     out += "Type: [[{}]]\n\n".format(metric.type)
     out += "Symbol: {}\n\n".format(metric.symbol)
     out += "Domain: {}\n\n".format(metric.domain)
 
     out += "## Parameters Used\n"
-    for i, x in enumerate(metric.parameters_used):
+    for i, x in enumerate(sorted(metric.parameters_used, key=lambda x: x.name)):
         out += "{}. [[{}]]".format(i + 1, x)
         out += "\n"
     out += "\n"
 
     out += "## Variables Used\n"
     for i, x in enumerate(metric.variables_used):
         out += "{}. [[{}]].{}".format(i + 1, x[0], x[1])
@@ -571,15 +573,15 @@
     out += "Symbol: {}\n\n".format(metric.symbol)
 
     out += "## Logic\n"
     out += metric.logic
     out += "\n\n"
 
     out += "## Parameters Used\n"
-    for i, x in enumerate(metric.parameters_used):
+    for i, x in enumerate(sorted(metric.parameters_used, key=lambda x: x.name)):
         out += "{}. [[{}]]".format(i + 1, x)
         var = ms.parameters.parameter_map[x]
         if var.symbol:
             out += " , symbol: {}".format(var.symbol)
         out += "\n"
     out += "\n"
 
@@ -679,14 +681,15 @@
         out += "{}. [[{}]]".format(i + 1, x)
         out += "\n"
     out += "\n"
 
     out += "## Unique Components Used\n"
     components = [set(x.components_full()) for x in wirings]
     components = set().union(*components)
+    components = sorted(components, key=lambda x: x.name)
     for i, x in enumerate(components):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
     out += "\n"
 
     """domain = [set(x.domain) for x in wirings]
     domain = set().union(*domain)
@@ -702,16 +705,17 @@
     for i, x in enumerate(codomain):
         out += "{}. [[{}]]".format(i + 1, x.name)
         out += "\n"
     out += "\n"""
 
     parameters = [set(x.parameters_used) for x in wirings]
     parameters = set().union(*parameters)
+    parameters = sorted(parameters, key=lambda x: x)
     out += "## Unique Parameters Used\n"
-    for i, x in enumerate(parameters):
+    for i, x in enumerate(sorted(parameters, key=lambda x: x.name)):
         out += "{}. [[{}]]".format(i + 1, x)
         out += "\n"
     out += "\n"
 
     with open("{}/Displays/Wiring/{}.md".format(path, wiring["name"]), "w") as f:
         f.write(out)
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/mechanisms.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/mechanisms.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/node_map.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/node_map.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/parameters.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/parameters.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/policies.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/policies.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/spaces.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/spaces.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/state.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/state.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/tables.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/tables.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/Reports/wiring.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/Reports/wiring.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/__init__.py` & `math_spec_mapping-0.3.3/src/math_spec_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping/schema.schema.json` & `math_spec_mapping-0.3.3/src/math_spec_mapping/schema.schema.json`

 * *Files identical despite different names*

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/PKG-INFO` & `math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: math-spec-mapping
-Version: 0.3.2
+Version: 0.3.3
 Summary: A library for easy mapping of mathematical specifications.
 Author-email: Sean McOwen <Sean@Block.Science>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `math_spec_mapping-0.3.2/src/math_spec_mapping.egg-info/SOURCES.txt` & `math_spec_mapping-0.3.3/src/math_spec_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

