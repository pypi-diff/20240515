# Comparing `tmp/ignition_api-8.1.40.tar.gz` & `tmp/ignition-api-8.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/8.1/8.1/dist/tmp_SKoQn/ignition_api-8.1.40.tar", last modified: Wed May 15 18:17:36 2024, max compression
+gzip compressed data, was "/Users/thecesrom/github/thecesrom/Ignition/main/dist/tmpjCWm5Y/ignition-api-8.1.9.tar", last modified: Thu Sep  9 00:05:05 2021, max compression
```

## Comparing `ignition_api-8.1.40.tar` & `ignition-api-8.1.9.tar`

### file list

```diff
@@ -1,413 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/
--rw-rw-r--   0 root         (0) root         (0)     1071 2024-05-15 18:14:33.000000 ignition_api-8.1.40/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       79 2024-05-15 18:14:33.000000 ignition_api-8.1.40/setup.py
--rwxrwxr-x   0 root         (0) root         (0)     5809 2024-05-15 18:14:33.000000 ignition_api-8.1.40/README.md
--rw-rw-r--   0 root         (0) root         (0)      101 2024-05-15 18:14:33.000000 ignition_api-8.1.40/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1391 2024-05-15 18:17:36.000000 ignition_api-8.1.40/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)    16613 2024-05-15 18:14:33.000000 ignition_api-8.1.40/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     8580 2024-05-15 18:17:36.000000 ignition_api-8.1.40/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/javax/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/javax/security/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/javax/security/auth/
--rw-rw-r--   0 root         (0) root         (0)      262 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/javax/security/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/javax/security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/javax/swing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/javax/swing/plaf/
--rw-rw-r--   0 root         (0) root         (0)      646 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/javax/swing/plaf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/javax/swing/event/
--rw-rw-r--   0 root         (0) root         (0)     1201 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/javax/swing/event/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12215 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/javax/swing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/javax/swing/text/
--rw-rw-r--   0 root         (0) root         (0)      417 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/javax/swing/text/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/javax/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/system/
--rw-rw-r--   0 root         (0) root         (0)     4900 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/iec61850.py
--rw-rw-r--   0 root         (0) root         (0)     5158 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/sfc.py
--rw-rw-r--   0 root         (0) root         (0)    29165 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/db.py
--rw-rw-r--   0 root         (0) root         (0)     8739 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/opchda.py
--rw-rw-r--   0 root         (0) root         (0)     7654 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/file.py
--rw-rw-r--   0 root         (0) root         (0)    20743 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/date.py
--rw-rw-r--   0 root         (0) root         (0)     5101 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/report.py
--rw-rw-r--   0 root         (0) root         (0)    10793 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/secsgem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/system/bacnet/
--rw-rw-r--   0 root         (0) root         (0)    13377 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/bacnet/enumerated.py
--rw-rw-r--   0 root         (0) root         (0)     7203 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/bacnet/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      977 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/bacnet/enums.py
--rw-rw-r--   0 root         (0) root         (0)     3844 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/device.py
--rw-rw-r--   0 root         (0) root         (0)     2692 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/opcua.py
--rw-rw-r--   0 root         (0) root         (0)     2581 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/twilio.py
--rw-rw-r--   0 root         (0) root         (0)    13636 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/alarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/system/perspective/
--rw-rw-r--   0 root         (0) root         (0)      808 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/perspective/workstation.py
--rw-rw-r--   0 root         (0) root         (0)    32022 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/perspective/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/system/mongodb/
--rw-rw-r--   0 root         (0) root         (0)    11215 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/mongodb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      425 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/mongodb/types.py
--rw-rw-r--   0 root         (0) root         (0)     7340 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/nav.py
--rw-rw-r--   0 root         (0) root         (0)     4437 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/eam.py
--rw-rw-r--   0 root         (0) root         (0)    17236 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/net.py
--rw-rw-r--   0 root         (0) root         (0)    21145 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/gui.py
--rw-rw-r--   0 root         (0) root         (0)     6872 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/dnp3.py
--rw-rw-r--   0 root         (0) root         (0)     1609 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/groups.py
--rw-rw-r--   0 root         (0) root         (0)    37145 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/tag.py
--rw-rw-r--   0 root         (0) root         (0)     2176 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/project.py
--rw-rw-r--   0 root         (0) root         (0)    21611 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/dataset.py
--rw-rw-r--   0 root         (0) root         (0)      486 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8708 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/opc.py
--rw-rw-r--   0 root         (0) root         (0)     3094 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/print.py
--rw-rw-r--   0 root         (0) root         (0)    15323 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/user.py
--rw-rw-r--   0 root         (0) root         (0)    13114 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/serial.py
--rw-rw-r--   0 root         (0) root         (0)    35051 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/util.py
--rw-rw-r--   0 root         (0) root         (0)    16073 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/math.py
--rw-rw-r--   0 root         (0) root         (0)     5333 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/security.py
--rw-rw-r--   0 root         (0) root         (0)     3530 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/roster.py
--rw-rw-r--   0 root         (0) root         (0)     1174 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/vision.py
--rw-rw-r--   0 root         (0) root         (0)       76 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/system/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/palantir/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/palantir/ptoss/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/palantir/ptoss/cinch/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/palantir/ptoss/cinch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/palantir/ptoss/cinch/core/
--rw-rw-r--   0 root         (0) root         (0)      726 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/palantir/ptoss/cinch/core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/palantir/ptoss/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/palantir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/google/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/google/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/google/common/collect/
--rw-rw-r--   0 root         (0) root         (0)     3244 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/google/common/collect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/google/common/eventbus/
--rw-rw-r--   0 root         (0) root         (0)      604 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/google/common/eventbus/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/google/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/client/components/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/client/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/client/components/model/
--rw-rw-r--   0 root         (0) root         (0)      424 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/client/components/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/alarming/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/alarming/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/alarming/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/alarming/common/rosters/
--rw-rw-r--   0 root         (0) root         (0)      892 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/alarming/common/rosters/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/alarming/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/modules/serial/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/modules/serial/scripting/
--rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/modules/serial/scripting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/modules/serial/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/gateway/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/gateway/project/
--rw-rw-r--   0 root         (0) root         (0)     1589 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/gateway/project/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/gateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/gui/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/gui/progress/
--rw-rw-r--   0 root         (0) root         (0)     2391 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/gui/progress/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/gui/scheduling/
--rw-rw-r--   0 root         (0) root         (0)     2120 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/util/gui/scheduling/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/launch/
--rw-rw-r--   0 root         (0) root         (0)    10568 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/launch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/model/
--rw-rw-r--   0 root         (0) root         (0)     6208 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/client/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/alarming/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/alarming/query/
--rw-rw-r--   0 root         (0) root         (0)     1465 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/alarming/query/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/alarming/evaluation/
--rw-rw-r--   0 root         (0) root         (0)     2000 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/alarming/evaluation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5668 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/alarming/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/document/
--rw-rw-r--   0 root         (0) root         (0)      382 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/document/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/execution/
--rw-rw-r--   0 root         (0) root         (0)     1835 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/jsonschema/
--rw-rw-r--   0 root         (0) root         (0)     6114 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/expressions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/expressions/functions/
--rw-rw-r--   0 root         (0) root         (0)     1127 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/expressions/functions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1652 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/expressions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/opc/
--rw-rw-r--   0 root         (0) root         (0)     7252 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/opc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/serialization/
--rw-rw-r--   0 root         (0) root         (0)     3401 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/serialization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/
--rw-rw-r--   0 root         (0) root         (0)      275 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/serialization/equalitydelegates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/deserialization/
--rw-rw-r--   0 root         (0) root         (0)     4568 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/deserialization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1010 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/encoding/
--rw-rw-r--   0 root         (0) root         (0)      153 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/xmlserialization/encoding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/modules/
--rw-rw-r--   0 root         (0) root         (0)     7026 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/logging/
--rw-rw-r--   0 root         (0) root         (0)     1358 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/message/
--rw-rw-r--   0 root         (0) root         (0)     1050 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/message/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/builtin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/builtin/http/
--rw-rw-r--   0 root         (0) root         (0)     4119 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/builtin/http/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14958 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/builtin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/builtin/ialabs/
--rw-rw-r--   0 root         (0) root         (0)     3446 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/builtin/ialabs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/abc/
--rw-rw-r--   0 root         (0) root         (0)     7960 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/abc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3684 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/adapters/
--rw-rw-r--   0 root         (0) root         (0)     2000 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/adapters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/hints/
--rw-rw-r--   0 root         (0) root         (0)      557 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/script/hints/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/project/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/project/resource/
--rw-rw-r--   0 root         (0) root         (0)     8974 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/project/resource/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5063 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/util/
--rw-rw-r--   0 root         (0) root         (0)     9328 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/i18n/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/i18n/keyboard/
--rw-rw-r--   0 root         (0) root         (0)     1554 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/i18n/keyboard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/i18n/translation/
--rw-rw-r--   0 root         (0) root         (0)      416 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/i18n/translation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1391 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/i18n/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/paths/
--rw-rw-r--   0 root         (0) root         (0)     2372 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/paths/parser/
--rw-rw-r--   0 root         (0) root         (0)     1071 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/paths/parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/model/
--rw-rw-r--   0 root         (0) root         (0)     2968 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/config/types/
--rw-rw-r--   0 root         (0) root         (0)      428 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/config/types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/tagpaths/
--rw-rw-r--   0 root         (0) root         (0)      408 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/tags/tagpaths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/licensing/
--rw-rw-r--   0 root         (0) root         (0)     2523 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/licensing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/user/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/user/schedule/
--rw-rw-r--   0 root         (0) root         (0)     8384 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/user/schedule/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8116 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/user/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/browsing/
--rw-rw-r--   0 root         (0) root         (0)     6337 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/browsing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20505 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/model/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/model/values/
--rw-rw-r--   0 root         (0) root         (0)     8892 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/model/values/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7918 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/db/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/db/namedquery/
--rw-rw-r--   0 root         (0) root         (0)     1163 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/db/namedquery/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/history/
--rw-rw-r--   0 root         (0) root         (0)     1611 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/history/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/history/annotations/
--rw-rw-r--   0 root         (0) root         (0)     3104 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/history/annotations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/model/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/model/types/
--rw-rw-r--   0 root         (0) root         (0)     2874 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/model/types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/sqltags/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/config/
--rw-rw-r--   0 root         (0) root         (0)     5761 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/binding/
--rw-rw-r--   0 root         (0) root         (0)      171 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/binding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gson/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gson/stream/
--rw-rw-r--   0 root         (0) root         (0)     3460 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gson/stream/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14019 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gson/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gson/reflect/
--rw-rw-r--   0 root         (0) root         (0)      390 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gson/reflect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/messages/
--rw-rw-r--   0 root         (0) root         (0)     1944 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/messages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gui/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gui/progress/
--rw-rw-r--   0 root         (0) root         (0)     2419 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/gui/progress/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/functional/
--rw-rw-r--   0 root         (0) root         (0)      143 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/ignition/common/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/script/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/script/builtin/
--rw-rw-r--   0 root         (0) root         (0)    11733 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/script/builtin/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      446 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/script/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2506 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/model/
--rw-rw-r--   0 root         (0) root         (0)      348 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/sqltags/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/sqltags/project/
--rw-rw-r--   0 root         (0) root         (0)      294 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/sqltags/project/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/sqltags/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/binding/
--rw-rw-r--   0 root         (0) root         (0)     1318 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/binding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/components/
--rw-rw-r--   0 root         (0) root         (0)      430 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/factorypmi/application/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/perspective/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/perspective/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/perspective/common/
--rw-rw-r--   0 root         (0) root         (0)     1145 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/perspective/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/sfc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/sfc/api/
--rw-rw-r--   0 root         (0) root         (0)      506 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/sfc/api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/sfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/opccom/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/opccom/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/inductiveautomation/opccom/hda/
--rw-rw-r--   0 root         (0) root         (0)     1780 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/inductiveautomation/opccom/hda/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/codahale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/com/codahale/metrics/
--rw-rw-r--   0 root         (0) root         (0)     2347 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/codahale/metrics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/com/codahale/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ignition_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ignition_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    10214 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ignition_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ignition_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8580 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ignition_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ignition_api.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/log4j/
--rw-rw-r--   0 root         (0) root         (0)     3892 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/log4j/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/log4j/spi/
--rw-rw-r--   0 root         (0) root         (0)     3561 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/log4j/spi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/commons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/commons/lang3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/commons/lang3/builder/
--rw-rw-r--   0 root         (0) root         (0)     1050 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/commons/lang3/builder/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/commons/lang3/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/commons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/commons/math3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/commons/math3/exception/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/apache/commons/math3/exception/util/
--rw-rw-r--   0 root         (0) root         (0)     1017 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/commons/math3/exception/util/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1617 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/commons/math3/exception/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/apache/commons/math3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/slf4j/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/slf4j/event/
--rw-rw-r--   0 root         (0) root         (0)      246 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/slf4j/event/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1761 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/slf4j/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/python/expose/
--rw-rw-r--   0 root         (0) root         (0)      683 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/python/expose/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/python/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/python/core/
--rw-rw-r--   0 root         (0) root         (0)    40043 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/python/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/json/
--rw-rw-r--   0 root         (0) root         (0)     6093 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/json/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/bson/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/bson/codecs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/bson/codecs/configuration/
--rw-rw-r--   0 root         (0) root         (0)      186 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/bson/codecs/configuration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       30 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/bson/codecs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/org/bson/types/
--rw-rw-r--   0 root         (0) root         (0)     4757 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/bson/types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3372 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/org/bson/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ch/qos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ch/qos/logback/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/ch/qos/logback/classic/
--rw-rw-r--   0 root         (0) root         (0)      888 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/ch/qos/logback/classic/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/ch/qos/logback/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/ch/qos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/ch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/dev/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/dev/coatl/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/dev/coatl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/dev/coatl/utils/
--rw-rw-r--   0 root         (0) root         (0)      227 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/dev/coatl/utils/decorators.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/dev/coatl/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/dev/coatl/helper/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/dev/coatl/helper/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      151 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/dev/coatl/helper/types.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/dev/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/security/
--rw-rw-r--   0 root         (0) root         (0)      608 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/security/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/nio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/nio/file/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/nio/file/attribute/
--rw-rw-r--   0 root         (0) root         (0)     3077 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/nio/file/attribute/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11663 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/nio/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/nio/channels/
--rw-rw-r--   0 root         (0) root         (0)     7200 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/nio/channels/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12452 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/nio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/nio/charset/
--rw-rw-r--   0 root         (0) root         (0)     3034 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/nio/charset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/util/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/util/stream/
--rw-rw-r--   0 root         (0) root         (0)     2672 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/util/stream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/util/function/
--rw-rw-r--   0 root         (0) root         (0)     2550 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/util/function/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/util/regex/
--rw-rw-r--   0 root         (0) root         (0)     4244 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/util/regex/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    29935 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/util/concurrent/
--rw-rw-r--   0 root         (0) root         (0)     3119 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/util/concurrent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/awt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/awt/event/
--rw-rw-r--   0 root         (0) root         (0)     4383 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/awt/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/awt/geom/
--rw-rw-r--   0 root         (0) root         (0)     2544 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/awt/geom/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/awt/image/
--rw-rw-r--   0 root         (0) root         (0)      277 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/awt/image/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/awt/print/
--rw-rw-r--   0 root         (0) root         (0)     1698 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/awt/print/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5433 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/awt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/beans/
--rw-rw-r--   0 root         (0) root         (0)     1089 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/beans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/net/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/net/http/
--rw-rw-r--   0 root         (0) root         (0)      147 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/net/http/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10514 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/net/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/io/
--rw-rw-r--   0 root         (0) root         (0)     8060 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/io/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/text/
--rw-rw-r--   0 root         (0) root         (0)    12872 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/lang/
--rw-rw-r--   0 root         (0) root         (0)    18162 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/lang/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/lang/reflect/
--rw-rw-r--   0 root         (0) root         (0)      174 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/lang/reflect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/math/
--rw-rw-r--   0 root         (0) root         (0)     2020 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/math/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/org/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/org/jdesktop/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/org/jdesktop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/org/jdesktop/core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/org/jdesktop/core/animation/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/org/jdesktop/core/animation/timing/
--rw-rw-r--   0 root         (0) root         (0)      273 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/org/jdesktop/core/animation/timing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/org/jdesktop/core/animation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/org/jdesktop/core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/org/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/time/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/time/temporal/
--rw-rw-r--   0 root         (0) root         (0)     5969 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/time/temporal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 18:17:36.000000 ignition_api-8.1.40/src/java/time/format/
--rw-rw-r--   0 root         (0) root         (0)      325 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/time/format/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3485 2024-05-15 18:14:33.000000 ignition_api-8.1.40/src/java/time/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       21 2024-05-15 18:14:33.000000 ignition_api-8.1.40/MANIFEST.in
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     9117 2021-09-09 00:05:05.000000 ignition-api-8.1.9/PKG-INFO
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1075 2021-06-30 21:14:38.000000 ignition-api-8.1.9/LICENSE
+-rw-r--r--   0 thecesrom   (501) staff       (20)      197 2021-09-07 17:18:43.000000 ignition-api-8.1.9/pyproject.toml
+-rw-r--r--   0 thecesrom   (501) staff       (20)       26 2021-09-06 00:11:39.000000 ignition-api-8.1.9/MANIFEST.in
+-rwxr-xr-x   0 thecesrom   (501) staff       (20)     6882 2021-09-09 00:04:52.000000 ignition-api-8.1.9/README.md
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1413 2021-09-08 16:24:16.000000 ignition-api-8.1.9/setup.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)       38 2021-09-09 00:05:05.000000 ignition-api-8.1.9/setup.cfg
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/ignition_api.egg-info/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     9117 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/ignition_api.egg-info/PKG-INFO
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1121 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/ignition_api.egg-info/SOURCES.txt
+-rw-r--r--   0 thecesrom   (501) staff       (20)       18 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/ignition_api.egg-info/top_level.txt
+-rw-r--r--   0 thecesrom   (501) staff       (20)        1 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/ignition_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/java/
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/java/util/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     5557 2021-08-13 19:36:22.000000 ignition-api-8.1.9/src/java/util/__init__.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)      100 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/java/__init__.py
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/java/lang/
+-rw-r--r--   0 thecesrom   (501) staff       (20)    10249 2021-08-13 22:16:02.000000 ignition-api-8.1.9/src/java/lang/__init__.py
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/java/awt/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     3003 2021-08-13 22:05:42.000000 ignition-api-8.1.9/src/java/awt/__init__.py
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/java/awt/image/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1585 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/java/awt/image/__init__.py
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/system/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     6150 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/system/dnp3.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     9812 2021-09-06 16:12:00.000000 ignition-api-8.1.9/src/system/opc.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    28095 2021-09-06 16:10:40.000000 ignition-api-8.1.9/src/system/db.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    23250 2021-09-06 16:14:20.000000 ignition-api-8.1.9/src/system/user.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     4004 2021-08-25 23:38:19.000000 ignition-api-8.1.9/src/system/eam.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    10162 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/opchda.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     3004 2021-08-13 00:21:11.000000 ignition-api-8.1.9/src/system/device.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    36829 2021-09-08 16:08:12.000000 ignition-api-8.1.9/src/system/util.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     4927 2021-09-06 16:13:41.000000 ignition-api-8.1.9/src/system/security.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    15393 2021-08-13 00:42:52.000000 ignition-api-8.1.9/src/system/net.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    13700 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/alarm.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)      566 2021-09-02 16:50:02.000000 ignition-api-8.1.9/src/system/__init__.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)      437 2021-09-07 18:09:52.000000 ignition-api-8.1.9/src/system/__version__.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1393 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/system/groups.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     2530 2021-08-13 00:21:46.000000 ignition-api-8.1.9/src/system/opcua.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    22375 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/dataset.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1712 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/system/bacnet.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     6244 2021-08-16 20:25:34.000000 ignition-api-8.1.9/src/system/file.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     5085 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/sfc.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    12026 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/serial.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     3467 2021-08-25 23:38:19.000000 ignition-api-8.1.9/src/system/print.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     8532 2021-08-25 23:38:19.000000 ignition-api-8.1.9/src/system/nav.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    15632 2021-08-13 00:27:48.000000 ignition-api-8.1.9/src/system/math.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     2459 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/system/twilio.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    19111 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/date.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    10202 2021-09-06 16:13:04.000000 ignition-api-8.1.9/src/system/secsgem.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    20734 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/gui.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     2577 2021-08-25 23:38:19.000000 ignition-api-8.1.9/src/system/roster.py
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/system/perspective/
+-rw-r--r--   0 thecesrom   (501) staff       (20)    27094 2021-08-13 00:02:58.000000 ignition-api-8.1.9/src/system/perspective/__init__.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)      819 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/system/perspective/workstation.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     4459 2021-09-02 18:42:45.000000 ignition-api-8.1.9/src/system/report.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1595 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/system/project.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)    45176 2021-08-25 23:38:19.000000 ignition-api-8.1.9/src/system/tag.py
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/javax/
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/javax/swing/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     8612 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/javax/swing/__init__.py
+drwxr-xr-x   0 thecesrom   (501) staff       (20)        0 2021-09-09 00:05:05.000000 ignition-api-8.1.9/src/javax/swing/text/
+-rw-r--r--   0 thecesrom   (501) staff       (20)     1098 2021-08-13 19:47:59.000000 ignition-api-8.1.9/src/javax/swing/text/__init__.py
+-rw-r--r--   0 thecesrom   (501) staff       (20)      101 2021-06-30 21:14:38.000000 ignition-api-8.1.9/src/javax/__init__.py
```

### Comparing `ignition_api-8.1.40/LICENSE` & `ignition-api-8.1.9/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2024 coatl.dev
+Copyright (c) 2017-2021 César Román
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ignition_api-8.1.40/PKG-INFO` & `ignition-api-8.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,207 +1,191 @@
 Metadata-Version: 2.1
-Name: ignition_api
-Version: 8.1.40
-Summary: Ignition Scripting API
-Home-page: https://ignition-api.github.io/8.1
+Name: ignition-api
+Version: 8.1.9
+Summary: Ignition Scripting API.
+Home-page: https://github.com/thecesrom/Ignition
 Author: César Román
-Author-email: cesar@coatl.dev
+Author-email: cesar@thecesrom.dev
 License: MIT
-Project-URL: Source, https://github.com/ignition-api/8.1
-Project-URL: Documentation, https://docs.inductiveautomation.com/display/DOC81/System+Functions
-Project-URL: Funding, https://github.com/sponsors/thecesrom
-Project-URL: Tracker, https://github.com/ignition-api/8.1/issues
-Description: # ignition-api 8.1
+Description: # Ignition
         
         <!--- Badges --->
-        ![GitHub last commit (8.1)](https://img.shields.io/github/last-commit/ignition-api/8.1/main)
-        [![GitHub contributors](https://img.shields.io/github/contributors/ignition-api/8.1)](https://github.com/ignition-api/8.1/graphs/contributors)
-        [![Downloads](https://static.pepy.tech/badge/ignition-api)](https://pepy.tech/project/ignition-api)
+        ![GitHub last commit (main)](https://img.shields.io/github/last-commit/thecesrom/Ignition/main)
+        [![GitHub contributors](https://img.shields.io/github/contributors/thecesrom/Ignition)](https://github.com/thecesrom/Ignition/graphs/contributors)
+        [![GitHub downloads](https://img.shields.io/github/downloads/thecesrom/Ignition/total)](https://github.com/thecesrom/Ignition/releases)
+        [![time tracker](https://wakatime.com/badge/github/thecesrom/Ignition.svg)](https://wakatime.com/badge/github/thecesrom/Ignition)
+        [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Join us on GitHub discussions](https://img.shields.io/badge/github-discussions-informational)](https://github.com/ignition-api/8.1/discussions)
-        
-        ignition-api is a Python package that allows developers to get code completion
-        for Ignition Scripting API scripting functions in their IDE of choice.
-        
-        ## Table of contents
-        
+        [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+        [![Imports: flake8](https://img.shields.io/badge/%20imports-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
+        [![Imports: pydocstyle](https://img.shields.io/badge/%20imports-pydocstyle-%231674b1?style=flat&labelColor=ef8336)](https://www.pydocstyle.org/en/stable/)
+        [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/thecesrom/Ignition/main.svg)](https://results.pre-commit.ci/latest/github/thecesrom/Ignition/main)
+        
+        Ignition is a set of packages and modules that allows developers to get code completion for Ignition Scripting API scripting functions in their IDE of choice.
+        
+        # Table of contents
+        
+        - [Releases](#releases)
+        - [Branches](#branches)
+          - [Cloning a single branch](#cloning-a-single-branch)
         - [Prerequisites](#prerequisites)
+        - [Packages](#packages)
         - [Installation and usage](#installation-and-usage)
+          - [PyCharm installation](#pycharm-installation)
           - [Installing with pip](#installing-with-pip)
-          - [Downloading from releases](#downloading-from-releases)
-            - [Using as a dependency in PyCharm](#using-as-a-dependency-in-pycharm)
-        - [Project structure](#project-structure)
-          - [Packages](#packages)
-        - [Contributing](#contributing)
+        - [Contributing to Ignition](#contributing-to-ignition)
         - [Discussions](#discussions)
         - [Contributors](#contributors)
         - [License](#license)
         - [Code of conduct](#code-of-conduct)
         
-        ## Prerequisites
+        # Releases
         
-        Before you begin, ensure you have met the following requirements:
+        Check the [releases page](https://github.com/thecesrom/Ignition/releases) and download the one for your current version.
         
-        - You have installed [Python 2.7.18]
-        - You are familiar with [Ignition System Functions]
+        If you can't find it, feel free to submit your request on our [Discussions](https://github.com/thecesrom/Ignition/discussions).
         
-        ## Installation and usage
+        ## Branches
         
-        To use ignition-api, you may install it by doing any of the following.
+        This repository consists of the following branches:
         
-        ### Installing with `pip`
+        ### [main](https://github.com/thecesrom/Ignition/tree/main)
         
-        The preferred method is to install it by running `pip`. It requires Python
-        2.7.18.
+        This branch will contain all Scripting Functions from the latest Ignition Release requiring only Python
         
-        ```bash
-        python2 -m pip install ignition-api
-        ```
+        ### [7.9](https://github.com/thecesrom/Ignition/tree/7.9)
         
-        This will install it as package to your Python installation, which will allow
-        you to call Ignition Scripting functions from Python's REPL, and get code
-        completion using an IDE such as PyCharm and Visual Studio Code.
+        This branch will contain all Scripting Functions from the latest Ignition Release for the 7.9 version requiring only Python
         
-        ```bash
-        $ python2
-        Python 2.7.18 (default, Nov  9 2020, 16:23:15)
-        [GCC Apple LLVM 12.0.0 (clang-1200.0.32.21)] on darwin
-        Type "help", "copyright", "credits" or "license" for more information.
-        >>> from __future__ import print_function
-        >>> import system.util
-        >>> print(system.util.__doc__)
-        Utility Functions.
+        ### [8.0](https://github.com/thecesrom/Ignition/tree/8.0)
         
-        The following functions give you access to view various Gateway and
-        Client data, as well as interact with other various systems.
+        This branch will contain all Scripting Functions from the latest Ignition Release for the 8.0 version requiring only Python
         
-        >>> system.util.beep()
-        >>> quit()
-        ```
+        ### [jython](https://github.com/thecesrom/Ignition/tree/jython)
         
-        And to uninstall:
+        This branch will contain all Scripting Functions from the latest Ignition Release requiring Jython (see [jython prerequisites](https://github.com/thecesrom/Ignition/tree/jython#prerequisites))
         
-        ```bash
-        python2 -m pip uninstall ignition-api
-        ```
+        ### Cloning a single branch
         
-        ### Downloading from releases
+        If you wish to clone just one branch in particular, use any of the following commands:
         
-        You may also download the code targeted to your desired version from [releases]
-        and add it as a dependency to your scripting project.
+        - HTTPS
+            ```bash
+            git clone --single-branch --branch <name> https://github.com/thecesrom/Ignition.git [<directory>]
+            ```
+        - SSH
+            ```bash
+            git clone --single-branch --branch <name> git@github.com:thecesrom/Ignition.git [<directory>]
+            ```
+        - GitHub CLI
+            ```bash
+            gh repo clone thecesrom/Ignition [<directory>] -- --single-branch --branch <name>
+            ```
         
-        #### Using as a dependency in PyCharm
+        ## Prerequisites
+        
+        Before you begin, ensure you have met the following requirements:
         
-        To include ignition-api as a dependency in PyCharm, you will need to attach it
-        to your project.
+        * You have installed Python 2.7.18 ([download here](https://www.python.org/downloads/release/python-2718/))
+        * You are familiar with [Ignition 8.1 System Functions](https://docs.inductiveautomation.com/display/DOC81/System+Functions)
         
-        1. Clone the repo or download from [releases]
-        1. With your project open where you want to include `ignition-api`, navigate to
-           `File > Open` and select the `ignition-api` project folder
-        1. Choose `Attach` when prompted
-        1. Under the `ignitition-api` project folder, right-click on the `src/` folder
-           and choose `Mark Directory as > Sources Root`
         
-        ## Project structure
+        ## Packages
         
-        ### Packages
+        Ignition consists of the following packages:
         
-        This project consists of the following packages:
+        * java/javax
+        * system
         
-        - com.inductiveautomation
-        - java
-        - javax
-        - org
-        - system
+        ### java/javax
         
-        #### com.inductiveautomation
+        These are libraries for some Java packages and functions that are imported in `system` packages meant to be used on development environments where no JDK can be installed, and the project interpreter is Python 2.7.
         
-        This package includes supporting Inductive Automation's classes and interfaces.
-        For more information, see documentation here:
-        <https://files.inductiveautomation.com/sdk/javadoc/ignition81/8.1.39/index.html>.
+        ### system
         
-        #### java/javax
+        Is a package that includes all Ignition Scripting Functions.
         
-        These packages include supporting Java classes and interfaces. For more
-        information, see documentation here:
-        <https://docs.oracle.com/en/java/javase/17/docs/api/index.html>.
+        ## Installation and usage
+        
+        To use Ignition, download the code targeted to your desired version from the [releases page](https://github.com/thecesrom/Ignition/releases) and add it as a dependency to your scripting project.
         
-        #### org.apache
+        ### PyCharm Installation
+        To use Ignition in PyCharm, you will need to attach it to your project.
+        1. With your project open that you want to use with Ignition, navigate to `File > Open` and select the `Ignition` project folder.
+        2. Choose `Attach` when you're prompted on how to open the project.
+        3. Under the new `Ignition` project folder, right-click on the `src/` folder and choose `Mark Directory as > Sources Root`.
         
-        This package includes supporting classes and interfaces from Apache Commons Math
-        API. For more information, see documentation here:
-        <https://commons.apache.org/proper/commons-math/javadocs/api-3.6.1/index.html>
+        ### Installing with `pip`
+        Also, it can be installed by running `pip`. It requires Python 2.7 (we recommend version 2.7.18).
         
-        #### org.json
+        ```bash
+        $ python2 -m pip install ignition-api
+        ```
         
-        This package includes supporting classes and interfaces from the Inductive
-        Automation's `org.json` package, see documentation here:
-        <https://files.inductiveautomation.com/sdk/javadoc/ignition81/8.1.39/org/json/package-summary.html>
+        This will install it as package to your Python installation, which will allow you to call Ignition Scripting functions from Python's REPL, and get code completion using and IDE (we recommend PyCharm).
         
-        #### org.python
+        ```bash
+        Python 2.7.18 (default, Nov  9 2020, 16:23:15) 
+        [GCC Apple LLVM 12.0.0 (clang-1200.0.32.21)] on darwin
+        Type "help", "copyright", "credits" or "license" for more information.
+        >>> from __future__ import print_function
+        >>> import system.util
+        >>> print(system.util.__doc__)
+        Utility Functions.
         
-        This package includes supporting Jython classes and interfaces. For more
-        information, see documentation here:
-        <https://www.javadoc.io/doc/org.python/jython-standalone/2.7.3/index.html>.
+        The following functions give you access to view various Gateway and
+        Client data, as well as interact with other various systems.
         
-        #### org.slf4j
+        >>> system.util.beep()
+        >>> quit()
+        ```
         
-        This package includes supporting classes and interfaces from SLF4J API Module.
-        For more information, see documentation here:
-        <https://www.javadoc.io/doc/org.slf4j/slf4j-api/1.7.26/overview-summary.html>.
+        And to uninstall:
+        ```bash
+        $ python2 -m pip uninstall ignition-api
+        ```
         
-        #### system
+        ## Contributing to Ignition
         
-        This package includes all Ignition Scripting Functions. For more information,
-        see documentation here:
-        <https://docs.inductiveautomation.com/docs/8.1/appendix/scripting-functions>.
+        To contribute to Ignition, follow these steps:
         
-        ## Contributing
+        1. Fork this repository
+        2. Create a local copy on your machine
+        3. Create a branch
+        4. Make your changes and commit them
+        5. Push to the `main` branch
+        6. Create the pull request
         
-        See [CONTRIBUTING.md].
+        Alternatively see the GitHub documentation on [creating a pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).
         
         ## Discussions
         
-        Feel free to post your questions and/or ideas at [Discussions].
+        Feel free to post your questions and/or ideas at [Discussions](https://github.com/thecesrom/incendium/discussions).
         
         ## Contributors
         
         Thanks to everyone who has contributed to this project.
         
-        Up-to-date list of contributors can be found here: [CONTRIBUTORS].
+        Up-to-date list of contributors can be found [here](https://github.com/thecesrom/Ignition/graphs/contributors).
         
         ## License
         
-        See the [LICENSE].
+        See the [LICENSE](https://github.com/thecesrom/Ignition/blob/HEAD/LICENSE).
         
         ## Code of conduct
         
-        This project has adopted the [Microsoft Open Source Code of Conduct].
-        
-        <!-- Links -->
-        [CONTRIBUTING.md]: https://github.com/ignition-api/.github/blob/main/CONTRIBUTING.md#contributing-to-ignition-api
-        [CONTRIBUTORS]: https://github.com/ignition-api/8.1/graphs/contributors
-        [Discussions]: https://github.com/ignition-api/discussions
-        [Ignition System Functions]: https://docs.inductiveautomation.com/docs/8.1/appendix/scripting-functions
-        [LICENSE]: ./LICENSE
-        [Microsoft Open Source Code of Conduct]: https://opensource.microsoft.com/codeofconduct/
-        [Python 2.7.18]: https://www.python.org/downloads/release/python-2718/
-        [releases]: https://github.com/ignition-api/8.1/releases
+        This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
         
-Keywords: hmi,ignition,inductive automation,scada
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2 :: Only
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Mocking
-Requires-Python: ==2.7.18
+Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

### Comparing `ignition_api-8.1.40/src/system/sfc.py` & `ignition-api-8.1.9/src/system/sfc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """SFC Functions.
 
 The following functions give you access to interact with the SFCs in the
 Gateway.
 """
 
 from __future__ import print_function
@@ -14,162 +18,161 @@
     "redundantCheckpoint",
     "resumeChart",
     "setVariable",
     "setVariables",
     "startChart",
 ]
 
-from typing import Any, Dict, Optional
+from system.dataset import Dataset
+
+
+class PyChartScope(object):
+    """This class represents any "scope" in the SFC system, and is
+    fundamentally just an observable dictionary.
+
+    Despite its name, it is not limited to chart scope. This class
+    notifies listeners when values are changed, and wraps any
+    dictionaries assigned to it as PyChartScopes as well.
+    """
+
+    def __set__(self, instance, value):
+        pass
+
+    def __setattr__(self, key, value):
+        pass
 
-from com.inductiveautomation.ignition.common import BasicDataset
-from com.inductiveautomation.sfc.api import PyChartScope
-from dev.coatl.helper.types import AnyStr
+    def __setitem__(self, key, value):
+        pass
 
 
 def cancelChart(instanceId):
-    # type: (AnyStr) -> None
     """Cancels the execution of a running chart instance.
 
     Any running steps will be told to stop, and the chart will enter
     Canceling state.
 
     Args:
-        instanceId: The ID of the chart instance to cancel.
-
-    Raises:
-        KeyError: If the ID does not match any running chart instance.
+        instanceId (str): The ID of the chart instance to cancel.
     """
-    if not instanceId:
-        raise KeyError("Invalid UUID string: {}".format(instanceId))
+    print(instanceId)
 
 
-def getRunningCharts(chartPath=None):
-    # type: (Optional[AnyStr]) -> BasicDataset
+def getRunningCharts(charPath=None):
     """Retrieves information about running charts.
 
     Can search all running charts, or be filtered charts at a specific
     path. This function will return charts that are in a Paused state.
 
     Args:
-        chartPath: The path to a chart to filter on: i.e.,
+        charPath (str): The path to a chart to filter on: i.e.,
             "folder/chartName". If specified, only charts at the path
             will be included in the returned dataset. If omitted, the
             function will return data for all active charts.
 
     Returns:
-        A dataset with information on the active chart.
+        Dataset: A dataset with information on the active chart.
     """
-    print(chartPath)
-    return BasicDataset()
+    print(charPath)
+    return Dataset()
 
 
 def getVariables(instanceId):
-    # type: (AnyStr) -> PyChartScope
     """Get the variables in a chart instance's scope.
 
     Commonly used to check the value of a Chart Parameter, or determine
     how long the chart has been running for.
 
     Args:
-        instanceId: The instance identifier of the chart.
+        instanceId (str): The instance identifier of the chart.
 
     Returns:
-        A python dictionary of variables. Step scopes for active steps
-        are found under the "activeSteps" key.
+        PyChartScope: A python dictionary of variables. Step scopes for
+            active steps are found under the "activeSteps" key.
     """
     print(instanceId)
     return PyChartScope()
 
 
 def pauseChart(instanceId):
-    # type: (AnyStr) -> None
     """Pauses a running chart instance.
 
     Any running steps will be told to pause, and the chart will enter
     Pausing state.
 
     Args:
-        instanceId: The ID of the chart instance to pause.
-
-    Raises:
-        KeyError: If the ID does not match any running chart instance.
+        instanceId (str): The ID of the chart instance to pause.
     """
-    if not instanceId:
-        raise KeyError("Invalid UUID string: {}".format(instanceId))
+    print(instanceId)
 
 
 def redundantCheckpoint(instanceId):
-    # type: (AnyStr) -> None
     """Synchronizes chart and step variables of the specified chart
     instance across a redundant cluster, allowing the chart instance to
     continue where it left off if a redundant failover occurs.
 
     Args:
-        instanceId: The instance identifier of the chart.
+        instanceId (str): The instance identifier of the chart.
     """
     print(instanceId)
 
 
 def resumeChart(instanceId):
-    # type: (AnyStr) -> None
     """Resumes a chart that was paused.
 
     Steps which were previously paused will be resumed, and chart will
     enter Resuming state.
 
     Args:
-        instanceId: The ID of the chart instance to resume.
+        instanceId (str): The ID of the chart instance to resume.
 
     Raises:
         KeyError: If the ID does not match any running chart instance.
     """
     if not instanceId:
         raise KeyError("Invalid UUID string: {}".format(instanceId))
 
 
 def setVariable(instanceId, stepId, variableName, variableValue):
-    # type: (AnyStr, AnyStr, AnyStr, Any) -> None
     """Sets a variable inside a currently running chart.
 
     Args:
-        instanceId: The instance identifier of the chart.
-        stepId: The id for a step inside of a chart. If omitted the
-            function will target a chart scoped variable.
-        variableName: The name of the variable to set.
-        variableValue: The value for the variable to be set to.
+        instanceId (str): The instance identifier of the chart.
+        stepId (str): The id for a step inside of a chart. If omitted
+            the function will target a chart scoped variable.
+        variableName (str): The name of the variable to set.
+        variableValue (object): The value for the variable to be set to.
     """
     print(instanceId, stepId, variableName, variableValue)
 
 
 def setVariables(instanceId, stepId, variableMap):
-    # type: (AnyStr, AnyStr, Dict[AnyStr, Any]) -> None
     """Sets any number of variables inside a currently running chart.
 
     Args:
-        instanceId: The instance identifier of the chart.
-        stepId: The id for a step inside of a chart. If omitted
+        instanceId (str): The instance identifier of the chart.
+        stepId (str): The id for a step inside of a chart. If omitted
             the function will target a chart scoped variable.
-        variableMap: A dictionary containing the name:value pairs
+        variableMap (dict): A dictionary containing the name:value pairs
             of the variables to set.
     """
     print(instanceId, stepId, variableMap)
 
 
-def startChart(projectName, chartPath, arguments):
-    # type: (AnyStr, AnyStr, Dict[AnyStr, Any]) -> AnyStr
+def startChart(path, chartPath, arguments):
     """Starts a new instance of a chart.
 
     The chart must be set to "Callable" execution mode.
 
     Args:
-        projectName: The name of the project that the chart was created
-            in.
-        chartPath: The path to the chart, for example
+        path (str): The path to the chart, for example:
+            "ChartFolder/ChartName".
+        chartPath (str): The path to the chart, for example
             "ChartFolder/ChartName"
-        arguments: A dictionary containing the name:value pairs of the
-            variables to set.
+        arguments (dict): A dictionary of arguments. Each key-value pair
+            in the dictionary becomes a variable in the chart scope and
+            will override any default.
 
     Returns:
-        The unique ID of this chart.
+        str: The unique ID of this chart.
     """
-    print(projectName, chartPath, arguments)
+    print(path, chartPath, arguments)
     return "UUID"
```

### Comparing `ignition_api-8.1.40/src/system/db.py` & `ignition-api-8.1.9/src/system/db.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,20 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Database Functions.
 
 The following functions give you access to view and modify data in the
 database.
 """
 
 from __future__ import print_function
 
 __all__ = [
-    "ARRAY",
-    "BIGINT",
-    "BINARY",
-    "BIT",
-    "BLOB",
-    "BOOLEAN",
-    "CHAR",
-    "CLOB",
-    "DATALINK",
-    "DATE",
-    "DECIMAL",
-    "DISTINCT",
-    "DOUBLE",
-    "FLOAT",
-    "INTEGER",
-    "JAVA_OBJECT",
-    "LONGNVARCHAR",
-    "LONGVARBINARY",
-    "LONGVARCHAR",
-    "NCHAR",
-    "NCLOB",
-    "NULL",
-    "NUMERIC",
-    "NVARCHAR",
-    "ORACLE_CURSOR",
-    "OTHER",
-    "READ_COMMITTED",
-    "READ_UNCOMMITTED",
-    "REAL",
-    "REF",
-    "REPEATABLE_READ",
-    "ROWID",
-    "SERIALIZABLE",
-    "SMALLINT",
-    "SQLXML",
-    "STRUCT",
-    "TIME",
-    "TIMESTAMP",
-    "TINYINT",
-    "VARBINARY",
-    "VARCHAR",
     "addDatasource",
     "beginNamedQueryTransaction",
     "beginTransaction",
     "clearAllNamedQueryCaches",
     "clearNamedQueryCache",
     "closeTransaction",
     "commitTransaction",
@@ -74,24 +37,17 @@
     "runScalarQuery",
     "runUpdateQuery",
     "setDatasourceConnectURL",
     "setDatasourceEnabled",
     "setDatasourceMaxConnections",
 ]
 
-from typing import Any, List, Optional
-
-from com.inductiveautomation.ignition.common import BasicDataset
-from com.inductiveautomation.ignition.common.script.builtin import (
-    DatasetUtilities,
-    SProcCall,
-)
-from dev.coatl.helper.types import AnyStr
-from java.util import Date
+from java.lang import Object
 from javax.swing import JComponent
+from system.dataset import Dataset, PyDataSet
 
 # Type codes
 # These are codes defined by the JDBC specification.
 BIT = -7
 REAL = 7
 LONGVARCHAR = -1
 LONGVARBINARY = -4
@@ -134,58 +90,137 @@
 # Isolation levels.
 READ_COMMITTED = 2
 READ_UNCOMMITTED = 1
 REPEATABLE_READ = 4
 SERIALIZABLE = 8
 
 
+class SProcCall(Object):
+    def __init__(self):
+        pass
+
+    def getResultSet(self):
+        """Returns a dataset that is the resulting data of the stored
+        procedure, if any.
+
+        Returns:
+            Dataset: The dataset that is the resulting data of the
+                stored procedure, if any.
+        """
+        print(self)
+        return Dataset()
+
+    def getUpdateCount(self):
+        """Returns the number of rows modified by the stored procedure,
+        or -1 if not applicable.
+
+        Returns:
+             int: The number of rows modified by the stored procedure,
+                or -1 if not applicable.
+        """
+        print(self)
+        return 1
+
+    def getReturnValue(self):
+        """Returns the return value, if registerReturnParam had been
+        called.
+
+        Returns:
+             int: The return value, if registerReturnParam had been
+                called.
+        """
+        print(self)
+        return 0
+
+    def getOutParamValue(self, param):
+        """Returns the value of the previously registered out-parameter.
+
+        Args:
+            param (object): Index (int) or name (str) of the previously
+                registered out-parameter.
+
+        Returns:
+            object: The value of the previously registered
+                out-parameter.
+        """
+        print(self, param)
+        return 0
+
+    def registerInParam(self, param, typeCode, value):
+        """Registers an in parameter for the stored procedure.
+
+        Args:
+            param (object): Index (int starting at 1, not 0), or name
+                (str).
+            typeCode (int): Type code constant.
+            value (object): Value of type typeCode.
+        """
+        print(self, param, typeCode, value)
+
+    def registerOutParam(self, param, typeCode):
+        """Registers an out parameter for the stored procedure.
+
+        Args:
+            param (object): Index (int starting at 1, not 0), or name
+                (str).
+            typeCode (int): Type code constant.
+        """
+        print(self, param, typeCode)
+
+    def registerReturnParam(self, typeCode):
+        """Use this function to specify the datatype of the returned
+        value.
+
+        Args:
+            typeCode (int): Type code constant.
+        """
+        print(self, typeCode)
+
+
 def addDatasource(
-    jdbcDriver,  # type: AnyStr
-    name,  # type: AnyStr
-    description="",  # type: AnyStr
-    connectUrl=None,  # type: Optional[AnyStr]
-    username=None,  # type: Optional[AnyStr]
-    password=None,  # type: Optional[AnyStr]
-    props=None,  # type: Optional[AnyStr]
-    validationQuery=None,  # type: Optional[AnyStr]
-    maxConnections=8,  # type: int
+    jdbcDriver,
+    name,
+    description=None,
+    connectUrl=None,
+    username=None,
+    password=None,
+    props=None,
+    validationQuery=None,
+    maxConnections=8,
 ):
-    # type: (...) -> None
     """Adds a new database connection in Ignition.
 
     Args:
-        jdbcDriver: The name of the JDBC driver configuration to use.
-            Available options are based off the JDBC driver
-            configurations on the Gateway.
-        name: The datasource name.
-        description: Description of the datasource. Optional.
-        connectUrl: Default is the connect URL for JDBC driver.
+        jdbcDriver (str): The name of the JDBC driver in Ignition.
+            Required.
+        name (str): The datasource name. Required.
+        description (str): Description of the datasource. Optional.
+        connectUrl (str): Default is the connect URL for JDBC driver.
+        username (str): Username to login to the datasource with.
             Optional.
-        username: Username to login to the datasource with. Optional.
-        password: Password for the login. Optional.
-        props: The extra connection parameters. Optional.
-        validationQuery: Default is the validation query for the JDBC
-            driver. Optional.
-        maxConnections: Default is 8. Optional.
+        password (str): Password for the login. Optional.
+        props (str): The extra connection parameters. Optional.
+        validationQuery (str): Default is the validation query for the
+            JDBC driver. Optional.
+        maxConnections (int): Default is 8. Optional.
     """
     print(
         jdbcDriver,
         name,
         description,
         connectUrl,
         username,
         password,
         props,
         validationQuery,
         maxConnections,
     )
 
 
-def beginNamedQueryTransaction(*args, **kwargs):
-    # type: (*Any, **Any) -> AnyStr
+def beginNamedQueryTransaction(*args):
     """Begins a new database transaction using Named Queries.
 
     Database transactions are used to execute multiple queries in an
     atomic fashion. After executing queries, you must either commit the
     transaction to have your changes take effect, or rollback the
     transaction which will make all operations since the last commit not
     take place. The transaction is given a new unique string code, which
@@ -208,29 +243,26 @@
 
     When calling from Perspective or Gateway scope use:
     system.db.beginNamedQueryTransaction(project, database,
                                         [isolationLevel], [timeout])
 
     Args:
         *args: Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
 
     Returns:
-         The new transaction ID. You'll use this ID as the "tx" argument
-         for all other calls to have them execute against this
-         transaction.
+         str: The new transaction ID. You'll use this ID as the "tx"
+            argument for all other calls to have them execute against
+            this transaction.
     """
-    print(args, kwargs)
+    print(args)
     return "transaction_id"
 
 
-def beginTransaction(database="", isolationLevel=None, timeout=None):
-    # type: (Optional[AnyStr], Optional[int], Optional[int]) -> AnyStr
-    """Begins a new database transaction for using run* and runPrep*
-    queries.
+def beginTransaction(database=None, isolationLevel=None, timeout=None):
+    """Begins a new database transaction.
 
     Database transactions are used to execute multiple queries in an
     atomic fashion. After executing queries, you must either commit the
     transaction to have your changes take effect, or rollback the
     transaction which will make all operations since the last commit not
     take place. The transaction is given a new unique string code, which
     is then returned. You can then use this code as the tx argument for
@@ -243,296 +275,265 @@
     the transaction is used, the timeout timer is reset. For example, if
     you make a transaction with a timeout of one minute, you must use
     that transaction at least once a minute. If a transaction is
     detected to have timed out, it will be automatically closed and its
     transaction id will no longer be valid.
 
     Args:
-        database: The name of the database connection to create a
+        database (str): The name of the database connection to create a
             transaction in. Use "" for the project's default connection.
             Optional.
-        isolationLevel: The transaction isolation level to use. Use one
-            of the four constants: system.db.READ_COMMITTED,
+        isolationLevel (int): The transaction isolation level to use.
+            Use one of the four constants: system.db.READ_COMMITTED,
             system.db.READ_UNCOMMITTED, system.db.REPEATABLE_READ, or
             system.db.SERIALIZABLE. Optional.
-        timeout: The amount of time, in milliseconds, that this
+        timeout (long): The amount of time, in milliseconds, that this
             connection is allowed to remain open without being used.
             Timeout counter is reset any time a query or call is
             executed against the transaction, or when committed or
             rolled-back. Optional.
 
     Returns:
-        The new transaction ID. You'll use this ID as the "tx" argument
-        for all other calls to have them execute against this
-        transaction.
+        str: The new transaction ID. You'll use this ID as the "tx"
+            argument for all other calls to have them execute against
+            this transaction.
     """
     print(database, isolationLevel, timeout)
     return "transaction_id"
 
 
-def clearAllNamedQueryCaches(project=None):
-    # type: (Optional[AnyStr]) -> None
+def clearAllNamedQueryCaches(*args):
     """This clears the caches of all Named Queries in a project.
 
     If called from the Shared Scope (i.e., Tag Event Scripts, Alarm
     Pipelines, etc.) then the name of the project must be passed as a
     parameter.
 
+    When calling from the Project Scope use:
+    system.db.clearAllNamedQueryCaches()
+
+    When calling from the Shared Scope use:
+    system.db.clearAllNamedQueryCaches(project)
+
     Args:
-        project: The project that contains the Named Query whose cache
-            needs to be cleared. Optional.
+        *args: Variable length argument list.
     """
-    print(project)
+    print(args)
 
 
-def clearNamedQueryCache(*args, **kwargs):
-    # type: (*AnyStr, **AnyStr) -> None
+def clearNamedQueryCache(*args):
     """This clears the cache of a Named Query.
 
     If called from the Shared Scope (i.e., Tag Event Scripts, Alarm
     Pipelines, etc.) then the name of the project must be passed as a
     parameter.
 
     When calling from the Project Scope use:
     system.db.clearNamedQueryCache(path)
 
     When calling from the Shared Scope use:
     system.db.clearNamedQueryCache(project, path)
 
     Args:
         *args: Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
     """
-    print(args, kwargs)
+    print(args)
 
 
 def closeTransaction(tx):
-    # type: (AnyStr) -> None
     """Closes the transaction with the given ID.
 
-    You must commit or rollback the transaction before you close it.
-    Closing the transaction will return its database connection to the
-    pool. The transaction ID will no longer be valid.
+    Note that you must commit or rollback the transaction before you
+    close it. Closing the transaction will return its database
+    connection to the pool. The transaction ID will no longer be valid.
 
     Args:
-        tx: The transaction ID.
+        tx (str): The transaction ID.
     """
     print(tx)
 
 
 def commitTransaction(tx):
-    # type: (AnyStr) -> None
     """Performs a commit for the given transaction.
 
     This will make all statements executed against the transaction since
     its beginning or since the last commit or rollback take effect in
     the database. Until you commit a transaction, any changes that the
-    transaction makes will not be visible to other connections.
-
-    Note:
-        If you are done with the transaction, you must close it after
-        you commit it.
+    transaction makes will not be visible to other connections. Note
+    that if you are done with the transaction, you must close it after
+    you commit it.
 
     Args:
-        tx: The transaction ID.
+        tx (str): The transaction ID.
     """
     print(tx)
 
 
-def createSProcCall(
-    procedureName,  # type: AnyStr
-    database="",  # type: AnyStr
-    tx=None,  # type: Optional[AnyStr]
-    skipAudit=False,  # type: bool
-):
-    # type: (...) -> SProcCall
+def createSProcCall(procedureName, database=None, tx=None, skipAudit=None):
     """Creates an SProcCall object, which is a stored procedure call
     context.
 
     Args:
-        procedureName: The name of the stored procedure to call.
-        database: The name of the database connection to execute
+        procedureName (str): The named of the stored procedure to call.
+        database (str): The name of the database connection to execute
             against. If omitted or "", the project's default database
             connection will be used. Optional.
-        tx: A transaction identifier. If omitted, the call will be
+        tx (str): A transaction identifier. If omitted, the call will be
             executed in its own transaction. Optional.
-        skipAudit: A flag which, if set to True, will cause the
+        skipAudit (bool): A flag which, if set to True, will cause the
             procedure call to skip the audit system. Useful for some
             queries that have fields which won't fit into the audit log.
             Optional.
 
     Returns:
-        A stored procedure call context, which can be configured and
-        then used as the argument to system.db.execSProcCall.
+        SProcCall: A stored procedure call context, which can be
+            configured and then used as the argument to
+            system.db.execSProcCall.
     """
     print(procedureName, database, tx, skipAudit)
     return SProcCall()
 
 
 def dateFormat(date, formatPattern):
-    # type: (Date, AnyStr) -> AnyStr
     """This function is used to format Dates nicely as strings.
 
     It uses a format string to guide its formatting behavior.
 
     Args:
-        date: The Date object that you'd like to format.
-        formatPattern: A format pattern string to apply.
+        date (Date): The Date object that you'd like to format.
+        formatPattern (str): A format pattern string to apply.
 
     Returns:
-        The date as a string formatted according to the format pattern.
+        str: The date as a string formatted according to the format
+            pattern.
     """
     print(date, formatPattern)
     return ""
 
 
 def execSProcCall(callContext):
-    # type: (SProcCall) -> None
     """Executes a stored procedure call.
 
     The one parameter to this function is an SProcCall - a stored
     procedure call context.
 
     Args:
-        callContext: A stored procedure call context, with any input,
-            output, and/or return value parameters correctly configured.
-            Use system.db.createSProcCall to create a call context.
+        callContext (SProcCall): A stored procedure call context, with
+            any input, output, and/or return value parameters correctly
+            configured. Use system.db.createSProcCall to create a call
+            context.
     """
     print(callContext)
 
 
 def getConnectionInfo(name=""):
-    # type: (Optional[AnyStr]) -> BasicDataset
-    """Returns a dataset of information about a single database
-    connection, as specified by the name argument, or about the current
-    project's default database connection.
-
-    Note:
-        The database connection used when called from the Gateway scope
-        is the connection configured on the Gateway scripting project.
+    """Returns a dataset of information about a database connection.
 
     Args:
-        name: The name of the database connection to find information
-            about. Optional.
+        name (str): The name of the database connection to find
+            information about, or the project's default connection if
+            omitted. Optional.
 
     Returns:
-        A dataset containing information about the named database
-        connection or about the current project's default database
-        connection, or an empty dataset if the connection wasn't found.
+        Dataset: A dataset containing information about the named
+            database connection or about the current project's default
+            database connection, or an empty dataset if the connection
+            wasn't found.
     """
     print(name)
-    return BasicDataset()
+    return Dataset()
 
 
 def getConnections():
-    # type: () -> BasicDataset
     """Returns a dataset of information about each configured database
     connection.
 
     Each row represents a single connection.
 
     Returns:
-        A dataset, where each row represents a database connection.
+        Dataset: A dataset, where each row represents a database
+            connection.
     """
-    return BasicDataset()
+    return Dataset()
 
 
 def refresh(component, propertyName):
-    # type: (JComponent, AnyStr) -> bool
-    """This function will cause a Vision component binding to execute
-    immediately.
+    """This function will programmatically cause a SQL Query or DB
+    Browse property binding to execute immediately.
 
     This is most often used for bindings that are set to Polling - Off.
     In this way, you cause a binding to execute on demand, when you know
     that the results of its query will return a new result. To use it,
     you simply specify the component and name of the property on whose
     binding you'd like to refresh.
 
-    Even though the function includes "db" in the name, the function can
-    update all types of Vision component bindings, including Property
-    and Expression bindings.
-
-    Note:
-        This function will only work within the Vision module. To
-        manually execute bindings in Perspective, use the refreshBinding
-        component method.
-
     Args:
-        component: The component whose property you want to refresh.
-        propertyName: The name of the property that has a binding that
-            needs to be refreshed.
+        component (JComponent): The component whose property you want to
+            refresh.
+        propertyName (str): The name of the property that has a SQL
+            Query binding that needs to be refreshed
 
     Returns:
-        True if the property was found and refreshed successfully.
+        bool: True (1) if the property was found and refreshed
+            successfully.
     """
     print(component, propertyName)
     return True
 
 
 def removeDatasource(name):
-    # type: (AnyStr) -> None
     """Removes a database connection from Ignition.
 
     Args:
-        name: The name of the database connection in Ignition.
+        name (str): The name of the database connection in Ignition.
     """
     print(name)
 
 
 def rollbackTransaction(tx):
-    # type: (AnyStr) -> None
     """Performs a rollback on the given connection.
 
     This will make all statements executed against this transaction
     since its beginning or since the last commit or rollback undone.
-
-    Note:
-        If you are done with the transaction, you must also close it
-        after you do a rollback on it.
+    Note that if you are done with the transaction, you must also close
+    it after you do a rollback on it.
 
     Args:
-        tx: The transaction ID.
+        tx (str): The transaction ID.
     """
     print(tx)
 
 
-def runNamedQuery(*args, **kwargs):
-    # type: (*Any, **Any) -> Any
+def runNamedQuery(*args):
     """Runs a named query and returns the results.
 
     Note that the number of parameters in the function is determined by
     scope. Both versions of the function are listed below.
 
     When calling from the Project Scope use:
     system.db.runNamedQuery(path, parameters, [tx], [getKey])
 
     When calling from the Gateway Scope use:
     system.db.runNamedQuery(project, path, parameters, [tx], [getKey])
 
     Args:
         *args: Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
 
     Returns:
-        The results of the query. The exact object returned depends on
-        the Query Type property of the Named Query: typically either a
-        dataset when set to Query, an integer representing the number of
-        rows affected when set to Update Query, or an object matching
-        the datatype of the value returned by a Scalar Query.
+        object: The results of the query. The exact object returned
+            depends on the Query Type property of the Named Query:
+            typically either a dataset when set to Query, an integer
+            representing the number of rows affected when set to Update
+            Query, or an object matching the datatype of the value
+            returned by a Scalar Query.
     """
-    print(args, kwargs)
+    print(args)
 
 
-def runPrepQuery(
-    query,  # type: AnyStr
-    args,  # type: List[Any]
-    database="",  # type: AnyStr
-    tx=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> DatasetUtilities.PyDataSet
+def runPrepQuery(query, args, database="", tx=None):
     """Runs a prepared statement against the database, returning the
     results in a PyDataSet.
 
     Prepared statements differ from regular queries in that they can use
     a special placeholder, the question-mark character (?) in the query
     where any dynamic arguments would go, and then use an array of
     values to provide real information for those arguments. Make sure
@@ -542,324 +543,283 @@
     This call should be used for SELECT queries. This is a useful
     alternative to system.db.runQuery because it allows values in the
     WHERE clause, JOIN clause, and other clauses to be specified without
     having to turn those values into strings. This is safer because it
     protects against a problem known as a SQL injection attack, where a
     user can input data that affects the query's semantics.
 
-    Note:
-        The "?" placeholder refers to variables of the query statement
-        that help the statement return the correct information. The "?"
-        placeholder cannot reference column names, table names, or the
-        underlying syntax of the query. This is because the SQL standard
-        for handling the "?" placeholder excludes these items.
-
     Args:
-        query: A query (typically a SELECT) to run as a prepared
+        query (str): A query (typically a SELECT) to run as a prepared
             statement with placeholders (?) denoting where the arguments
             go.
-        args: A list of arguments. Will be used in order to match each
-            placeholder (?) found in the query.
-        database: The name of the database connection to execute
+        args (list[object]): A list of arguments. Will be used in order
+            to match each placeholder (?) found in the query.
+        database (str): The name of the database connection to execute
             against. If omitted or "", the project's default database
             connection will be used.
-        tx: A transaction identifier. If omitted, the query will be
-            executed in its own transaction. Optional.
+        tx (str): A transaction identifier. If omitted, the query will
+            be executed in its own transaction.
 
     Returns:
-        The results of the query as a PyDataSet.
+        PyDataSet: The results of the query as a PyDataSet.
     """
     print(query, args, database, tx)
-    return DatasetUtilities.PyDataSet()
+    return PyDataSet()
 
 
 def runPrepUpdate(
-    query,  # type: AnyStr
-    args,  # type: List[Any]
-    database="",  # type: AnyStr
-    tx=None,  # type: Optional[AnyStr]
-    getKey=False,  # type: bool
-    skipAudit=True,  # type: bool
+    query, args, database="", tx=None, getKey=False, skipAudit=True
 ):
-    # type: (...) -> int
     """Runs a prepared statement against the database, returning the
     number of rows that were affected.
 
     Prepared statements differ from regular queries in that they can use
     a special placeholder, the question-mark character (?) in the query
     where any dynamic arguments would go, and then use an array of
     values to provide real information for those arguments. Make sure
     that the length of your argument array matches the number of
     question-mark placeholders in your query. This call should be used
     for UPDATE, INSERT, and DELETE queries.
 
-    Note:
-        The "?" placeholder refers to variables of the query statement
-        that help the statement return the correct information. The "?"
-        placeholder cannot reference column names, table names, or the
-        underlying syntax of the query. This is because the SQL standard
-        for handling the "?" placeholder excludes these items.
-
     Args:
-        query: A query (typically an UPDATE, INSERT, or DELETE) to run
-            as a prepared statement with placeholders (?) denoting where
-            the arguments go.
-        args: A list of arguments. Will be used in order to match each
-            placeholder (?) found in the query.
-        database: The name of the database connection to execute
+        query (str): A query (typically an UPDATE, INSERT, or DELETE)
+            to run as a prepared statement with placeholders (?)
+            denoting where the arguments go.
+        args (list[object]): A list of arguments. Will be used in order
+            to match each placeholder (?) found in the query.
+        database (str): The name of the database connection to execute
             against. If omitted or "", the project's default database
             connection will be used. Optional.
-        tx: A transaction identifier. If omitted, the update will be
-            executed in its own transaction. Optional.
-        getKey: A flag indicating whether or not the result should be
-            the number of rows returned (getKey=0) or the newly
-            generated key value that was created as a result of the
-            update (getKey=1). Not all databases support automatic
+        tx (str): A transaction identifier. If omitted, the update will
+            be executed in its own transaction. Optional.
+        getKey (bool): A flag indicating whether or not the result
+            should be the number of rows returned (getKey=0) or the
+            newly generated key value that was created as a result of
+            the update (getKey=1). Not all databases support automatic
             retrieval of generated keys. Optional.
-        skipAudit: A flag which, if set to True, will cause the prep
-            update to skip the audit system. Useful for some queries
-            that have fields which won't fit into the audit log.
+        skipAudit (bool): A flag which, if set to True, will cause the
+            prep update to skip the audit system. Useful for some
+            queries that have fields which won't fit into the audit log.
             Optional.
 
     Returns:
-        The number of rows affected by the query, or the key value that
-        was generated, depending on the value of the getKey flag.
+        int: The number of rows affected by the query, or the key value
+            that was generated, depending on the value of the getKey
+            flag.
     """
     print(query, args, database, tx, getKey, skipAudit)
     return 1
 
 
-def runQuery(
-    query,  # type: AnyStr
-    database="",  # type: AnyStr
-    tx=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> DatasetUtilities.PyDataSet
+def runQuery(query, database="", tx=None):
     """Runs a SQL query, usually a SELECT query, against a database,
     returning the results as a dataset.
 
     If no database is specified, or the database is the empty-string "",
     then the current project's default database connection will be used.
     The results are returned as a PyDataSet, which is a wrapper around
     the standard dataset that is convenient for scripting.
 
     Args:
-        query: A SQL query, usually a SELECT query, to run.
-        database: The name of the database connection to execute
+        query (str): A SQL query, usually a SELECT query, to run.
+        database (str): The name of the database connection to execute
             against. If omitted or "", the project's default database
             connection will be used.
-        tx: A transaction identifier. If omitted, the query will be
-            executed in its own transaction.
+        tx (str): A transaction identifier. If omitted, the query will
+            be executed in its own transaction.
 
     Returns:
-        The results of the query as a PyDataSet.
+        PyDataSet: The results of the query as a PyDataSet.
     """
     print(query, database, tx)
-    return DatasetUtilities.PyDataSet()
+    return PyDataSet()
 
 
-def runSFNamedQuery(*args, **kwargs):
-    # type: (*Any, **Any) -> bool
+def runSFNamedQuery(*args):
     """Runs a named query that goes through the Store and Forward
     system.
 
     Note that the number of parameters in the function is determined by
     scope.
 
     When calling from the Project Scope use:
-    system.db.runSFNamedQuery(path, params)
+    system.db.runSFNamedQuery(path, parameters, [getKey])
 
     When calling from the Gateway Scope use:
-    system.db.runSFNamedQuery(project, path, params)
+    system.db.runSFNamedQuery(project, path, parameters, [getKey])
 
     Args:
         *args : Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
 
     Returns:
-        True if successfully sent to the Store and Forward system.
+        bool: Returns True if successfully sent to the Store and Forward
+            system.
     """
-    print(args, kwargs)
+    print(args)
     return True
 
 
 def runSFPrepUpdate(query, args, datasources):
-    # type: (AnyStr, List[Any], List[AnyStr]) -> bool
     """Runs a prepared statement query through the store and forward
     system and to multiple datasources at the same time.
 
     Prepared statements differ from regular queries in that they can use
     a special placeholder, the question-mark character (?) in the query
     where any dynamic arguments would go, and then use an array of
     values to provide real information for those arguments. Make sure
     that the length of your argument array matches the number of
     question-mark placeholders in your query. This call should be used
     for UPDATE, INSERT, and DELETE queries.
 
     Args:
-        query: A query (typically an UPDATE, INSERT, or DELETE) to run
-            as a prepared statement, with placeholders (?) denoting
+        query (str): A query (typically an UPDATE, INSERT, or DELETE) to
+            run as a prepared statement, with placeholders (?) denoting
             where the arguments go.
-        args: A list of arguments. Will be used in order to match each
-            placeholder (?) found in the query.
-        datasources: List of datasources to run the query through.
+        args (list[object]): A list of arguments. Will be used in order
+            to match each placeholder (?) found in the query.
+        datasources (list[str]): List of datasources to run the query
+            through.
 
     Returns:
-        True if successfully sent to Store and Forward system.
+        bool: Returns True if successfully sent to store-and-forward
+            system.
     """
     print(query, args, datasources)
     return True
 
 
 def runSFUpdateQuery(query, datasources):
-    # type: (AnyStr, List[AnyStr]) -> bool
-    """Runs a query through the store and forward system and to multiple
-    datasources at the same time.
+    """Runs an query through the store and forward system and to
+    multiple datasources at the same time.
 
     Args:
-        query: A query (typically an UPDATE, INSERT, or DELETE) to run.
-        datasources: List of datasources to run the query through.
+        query (str): A query (typically an UPDATE, INSERT, or DELETE) to
+            run.
+        datasources (list[str]): List of datasources to run the query
+            through.
 
     Returns:
-        True if successful and False if not.
+        bool: Returns True if successful and False if not.
     """
     print(query, datasources)
     return True
 
 
-def runScalarPrepQuery(
-    query,  # type: AnyStr
-    args,  # type: List[Any]
-    database="",  # type: AnyStr
-    tx=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> Any
+def runScalarPrepQuery(query, args, database="", tx=None):
     """Runs a prepared statement against a database connection just like
     the runPrepQuery function, but only returns the value from the first
     row and column.
 
     If no results are returned from the query, the special value None is
     returned.
 
     Args:
-        query: A SQL query (typically a SELECT) to run as a prepared
-            statement with placeholders (?) denoting where the arguments
-            go, that should be designed to return one row and one
-            column.
-        args: A list of arguments. Will be used in order to match each
-            placeholder (?) found in the query.
-        database: The name of the database connection to execute
+        query (str): A SQL query (typically a SELECT) to run as a
+            prepared statement with placeholders (?) denoting where the
+            arguments go, that should be designed to return one row and
+            one column.
+        args (list[object]): A list of arguments. Will be used in order
+            to match each placeholder (?) found in the query.
+        database (str): The name of the database connection to execute
             against. If omitted or "", the project's default database
             connection will be used. Optional.
-        tx: A transaction identifier. If omitted, the query will be
-            executed in its own transaction. Optional.
+        tx (str): A transaction identifier. If omitted, the query will
+            be executed in its own transaction.
 
     Returns:
-         The value from the first row and first column of the results.
-         Returns None if no rows were returned.
+         object: The value from the first row and first column of the
+            results. Returns None if no rows were returned.
     """
     print(query, args, database, tx)
 
 
 def runScalarQuery(query, database="", tx=None):
-    # type: (AnyStr, Optional[AnyStr], Optional[AnyStr]) -> Any
     """Runs a query against a database connection just like the runQuery
     function, but only returns the value from the first row and column.
 
     If no results are returned from the query, the special value None is
     returned.
 
     Args:
-        query: A SQL query that should be designed to return one row and
-            one column.
-        database: The name of the database connection to execute
+        query (str): A SQL query that should be designed to return one
+            row and one column.
+        database (str): The name of the database connection to execute
             against. If omitted or "", the project's default database
             connection will be used. Optional.
-        tx: A transaction identifier. If omitted, the query will be
-            executed in its own transaction. Optional.
+        tx (str): A transaction identifier. If omitted, the query will
+            be executed in its own transaction.
 
     Returns:
-         The value from the first row and first column of the results.
-         Returns None if no rows were returned.
+         object: The value from the first row and first column of the
+            results. Returns None if no rows were returned.
     """
     print(query, database, tx)
 
 
-def runUpdateQuery(
-    query,  # type: AnyStr
-    database="",  # type: AnyStr
-    tx=None,  # type: Optional[AnyStr]
-    getKey=False,  # type: bool
-    skipAudit=True,  # type: bool
-):
-    # type: (...) -> int
+def runUpdateQuery(query, database="", tx=None, getKey=False, skipAudit=True):
     """Runs a query against a database connection, returning the number
     of rows affected.
 
     Typically this is an UPDATE, INSERT, or DELETE query. If no database
     is specified, or the database is the empty-string "", then the
     current project's default database connection will be used.
 
-    Note:
-        You may want to use the runPrepUpdate query if your query is
-        constructed with user input (to avoid the user's input from
-        breaking your syntax) or if you need to insert binary or BLOB
-        data.
+    Note that you may want to use the runPrepUpdate query if your query
+    is constructed with user input (to avoid the user's input from
+    breaking your syntax) or if you need to insert binary or BLOB data.
 
     Args:
-        query: A SQL query, usually an INSERT, UPDATE, or DELETE query,
-            to run.
-        database: The name of the database connection to execute
+        query (str): A SQL query, usually an INSERT, UPDATE, or DELETE
+            query, to run.
+        database (str): The name of the database connection to execute
             against. If omitted or "", the project's default database
             connection will be used.
-        tx: A transaction identifier. If omitted, the update will be
-            executed in its own transaction.
-        getKey: A flag indicating whether or not the result should be
-            the number of rows returned (getKey=0) or the newly
-            generated key value that was created as a result of the
-            update (getKey=1). Not all databases support automatic
+        tx (str): A transaction identifier. If omitted, the update will
+            be executed in its own transaction.
+        getKey (bool): A flag indicating whether or not the result
+            should be the number of rows returned (getKey=0) or the
+            newly generated key value that was created as a result of
+            the update (getKey=1). Not all databases support automatic
             retrieval of generated keys.
-        skipAudit: A flag which, if set to True, will cause the update
-            query to skip the audit system. Useful for some queries that
-            have fields which won't fit into the audit log.
+        skipAudit (bool): A flag which, if set to True, will cause the
+            update query to skip the audit system. Useful for some
+            queries that have fields which won't fit into the audit log.
 
     Returns:
-        The number of rows affected by the query, or the key value that
-        was generated, depending on the value of the getKey flag.
+        int: The number of rows affected by the query, or the key value
+            that was generated, depending on the value of the getKey
+            flag.
     """
     print(query, database, tx, getKey, skipAudit)
     return 1
 
 
 def setDatasourceConnectURL(name, connectUrl):
-    # type: (AnyStr, AnyStr) -> None
     """Changes the connect URL for a given database connection.
 
     Args:
-        name: The name of the database connection in Ignition.
-        connectUrl: The new connect URL.
+        name (str): The name of the database connection in Ignition.
+        connectUrl (str): The new connect URL.
     """
     print(name, connectUrl)
 
 
 def setDatasourceEnabled(name, enabled):
-    # type: (AnyStr, bool) -> None
     """Enables/disables a given database connection.
 
     Args:
-        name: The name of the database connection in Ignition.
-        enabled: Specifies whether the database connection will be set
-            to enabled or disabled state.
+        name (str): The name of the database connection in Ignition.
+        enabled (bool): True if the connection should be enabled, False
+            otherwise.
     """
     print(name, enabled)
 
 
 def setDatasourceMaxConnections(name, maxConnections):
-    # type: (AnyStr, int) -> None
     """Sets the Max Active and Max Idle parameters of a given database
     connection.
 
     Ags:
-        name: The name of the database connection in Ignition.
-        maxConnections: The new value for Max Active and Max Idle.
+        name (str): The name of the database connection in Ignition.
+        maxConnections (int): The number of maximum connections allowed.
     """
     print(name, maxConnections)
```

### Comparing `ignition_api-8.1.40/src/system/opchda.py` & `ignition-api-8.1.9/src/system/opchda.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """OPC HDA Functions.
 
 The following functions give you access to interact with the HDA types
 of OPC servers.
 """
 
 from __future__ import print_function
@@ -16,259 +20,318 @@
     "isServerAvailable",
     "readAttributes",
     "readProcessed",
     "readRaw",
     "replace",
 ]
 
-from typing import Any, List
+from abc import ABCMeta, abstractmethod
 
-from com.inductiveautomation.ignition.common.browsing import Results
-from com.inductiveautomation.ignition.common.model.values import QualityCode
-from com.inductiveautomation.ignition.common.sqltags.history import AggregateInfo
-from com.inductiveautomation.opccom.hda import AttributeInfo, ReadResult
-from dev.coatl.helper.types import AnyStr
+from java.lang import Object
 from java.util import Date
 
 
+class Aggregate(ABCMeta):
+    """This interface defines an aggregation function used by the
+    history query system.
+
+    Different types of history providers may support different Aggregate
+    functions, and may define new types of aggregates. The name and
+    description are for informational purposes, aggregates are only
+    identified by their id (name and description should not be taken
+    into account).
+
+    The general implementation class is AggregateInfo. Common or "well
+    known" aggregates are defined in the AggregationMode enum. The
+    system works like this for historical reasons, previous to 7.7 only
+    the AggregationMode aggregates were used. After, with the
+    introduction of history providers as an extension point, new
+    providers could define any aggregation function.
+    """
+
+    def __new__(mcs, *args, **kwargs):
+        pass
+
+    @abstractmethod
+    def getDesc(cls):
+        pass
+
+    @abstractmethod
+    def getId(cls):
+        pass
+
+    @abstractmethod
+    def getName(cls):
+        pass
+
+
+class Results(Object):
+    """The results of a browse operation.
+
+    May only represent a partial result set, which can be determined by
+    comparing the Total Available Size to the Returned Size. If there is
+    a mismatch, the continuation point should be non-null and can be
+    used in constructing the subsequent BrowseFilter to continue the
+    browse.
+    """
+
+    def error(self, result):
+        pass
+
+    def getContinuationPoint(self):
+        pass
+
+    def getResultQuality(self):
+        pass
+
+    def getResults(self):
+        pass
+
+    def getReturnedSize(self):
+        pass
+
+    def getTotalAvailableSize(self):
+        pass
+
+    def of(self, arg):
+        pass
+
+    def setContinuationPoint(self, continuationPoint):
+        pass
+
+    def setResultQuality(self, value):
+        pass
+
+    def setResults(self, results):
+        pass
+
+    def setTotalAvailableResults(self, totalAvailableResults):
+        pass
+
+
 def browse(root):
-    # type: (AnyStr) -> List[Results]
     """Performs a browse at the given root.
 
     Args:
-        root: The root at which to browse. Needs to be a qualified path.
+        root (str): The root at which to browse. Needs to be a qualified
+            path.
 
     Returns:
-        The results of the browse operation from the given root.
+        list[Results]: The Browse Results that would result for the
+            operation at that root. Refer to the list of Results
+            objects.
     """
     print(root)
     return [Results()]
 
 
 def getAggregates(serverName):
-    # type: (AnyStr) -> List[AggregateInfo]
-    """Will query the Server for aggregates that it supports.
+    """Will query the server for aggregates that it supports.
 
     Args:
-        serverName: The name of the defined OPC-HDA Server to query.
+        serverName (str): The name of the defined OPC-HDA server to
+            query.
 
     Returns:
-        A list of supported Aggregate objects. Each object has 'id',
-        'name', and 'desc' properties defined.
+        list[Aggregate]: A list of supported Aggregate objects. Each
+            object has 'id', 'name', and 'desc' properties defined.
     """
     print(serverName)
-    return [AggregateInfo()]
+    return [Aggregate()]
 
 
 def getAttributes(serverName):
-    # type: (AnyStr) -> List[AttributeInfo]
-    """Queries the given Server for the item attributes that are
+    """Queries the given server for the item attributes that are
     available with system.opchda.readAttributes().
 
     Args:
-        serverName: The name of the defined OPC-HDA Server to query.
+        serverName (str): The name of the defined OPC-HDA server to
+            query.
 
     Returns:
-        A list of supported Aggregate objects. Each object has 'id',
-        'name', and 'desc' properties defined.
+        list[Aggregate]: A list of supported Aggregate objects. Each
+            object has 'id', 'name', and 'desc' properties defined.
     """
     print(serverName)
-    return [AttributeInfo()]
+    return [Aggregate()]
 
 
 def getServers():
-    # type: () -> List[AnyStr]
     """Returns a list of the OPC-HDA servers configured on the system.
 
     This call will return all configured and enabled servers, including
     those that are not currently connected.
 
     Returns:
-        A list of the string names of servers.
+        list[str]: A list of the string names of servers.
     """
     return []
 
 
 def insert(serverName, itemId, value, date, quality):
-    # type: (AnyStr, AnyStr, Any, Any, int) -> QualityCode
-    """Insert values on the OPC-HDA Server if the given item ID does not
+    """Insert values on the OPC-HDA server if the given item ID does not
     exist.
 
     Args:
-        serverName: The name of the defined OPC-HDA Server.
-        itemId: The item ID on which to perform the operation.
-        value: The value to insert.
-        date: The date to insert.
-        quality: The quality to insert.
+        serverName (str): The name of the defined OPC-HDA server.
+        itemId (str): The item ID to perform the operation on.
+        value (object): The value to insert.
+        date (object): The date to insert.
+        quality (int): The quality to insert.
 
     Returns:
-        The result of the insert.
+        int: The items quality form the operation.
     """
     print(serverName, itemId, value, date, quality)
-    return QualityCode()
+    return 192
 
 
 def insertReplace(serverName, itemId, value, date, quality):
-    # type: (AnyStr, AnyStr, Any, Date, int) -> QualityCode
-    """Will insert values on the OPC-HDA Server, or replace them if they
+    """Will insert values on the OPC-HDA server, or replace them if they
     already exist.
 
     Args:
-        serverName: The name of the defined OPC-HDA Server.
-        itemId: The item ID on which to perform the operation.
-        value: The value to insert or replace.
-        date: The date to insert or replace.
-        quality: The quality to insert or replace.
+        serverName (str): The name of the defined OPC-HDA server.
+        itemId (str): The item ID to perform the operation on.
+        value (object): The value to insert.
+        date (object): The date to insert.
+        quality (int): The quality to insert.
 
     Returns:
-        The items quality form the operation.
+        int: The items quality form the operation.
     """
     print(serverName, itemId, value, date, quality)
-    return QualityCode()
+    return 192
 
 
 def isServerAvailable(serverName):
-    # type: (AnyStr) -> bool
-    """Checks to see if the specified OPC-HDA Server is defined,
+    """Checks to see if the specified OPC-HDA server is defined,
     enabled, and connected.
 
     Args:
-        serverName: The name of the OPC-HDA Server to check.
+        serverName (str): The name of the OPC-HDA server to check.
 
     Returns:
-        True if the Server is available and can be queried, False if
-        not.
+        bool: Will be True if the server is available and can be
+            queried, False if not.
     """
     print(serverName)
     return True
 
 
-def readAttributes(
-    serverName,  # type: AnyStr
-    itemId,  # type: AnyStr
-    attributeIds,  # type: List[AnyStr]
-    startDate,  # type: Date
-    endDate,  # type: Date
-):
-    # type: (...) -> List[ReadResult]
+def readAttributes(serverName, itemId, attributeIds, startDate, endDate):
     """Reads the specified attributes for the given item over a time
     range.
 
     Attributes and their IDs are defined in the OPC-HDA specification,
     and can be discovered by calling system.opchda.getAttributes().
 
     Args:
-        serverName: The name of the defined OPC-HDA Server to read.
-        itemId: The itemID to retrieve attributes for.
-        attributeIds: The integer IDs of the attributes to read. The
-            attribute ids are defined in the OPC-HDA specification. The
-            attributes can also be obtained by calling
-            system.opchda.getAttributes(). Some servers may not support
-            all attributes.
-        startDate: The starting date/time of the query.
-        endDate: The ending date/time of the query.
-
-    Returns:
-        A list of read results which is one-to-one with the requested
-        attributes. The ReadResult object has a 'serviceResult' quality
-        property that indicates whether the call was successful, and is
-        itself a list of QualifiedValues.
+        serverName (str): The name of the defined OPC-HDA server to
+            read.
+        itemId (str): The itemID to retrieve attributes for.
+        attributeIds (list[int]): The integer IDs of the attributes to
+            read. The attribute ids are defined in the OPC-HDA
+            specification. The attributes can also be obtained by
+            calling system.opchda.getAttributes(). Some servers may not
+            support all attributes.
+        startDate (Date): The starting date/time of the query.
+        endDate (Date): The ending date/time of the query.
+
+    Returns:
+        list[ReadResult]: A list of read results which is one-to-one
+            with the requested attributes. The ReadResult object has a
+            'serviceResult' quality property that indicates whether the
+            call was successful, and is itself a list of
+            QualifiedValues.
     """
     print(serverName, itemId, attributeIds, startDate, endDate)
-    return [ReadResult() for _ in attributeIds]
+    return []
 
 
 def readProcessed(
-    serverName,  # type: AnyStr
-    itemIds,  # type: List[AnyStr]
-    startDate,  # type: Date
-    endDate,  # type: Date
-    resampleIntervalMS,  # type: int
-    aggregates,  # type: List[Any]
+    serverName, itemIds, startDate, endDate, resampleIntervalMS, aggregates
 ):
-    # type: (...) -> List[ReadResult]
-    """Reads processed values from the OPC-HDA Server.
+    """Reads processed values from the OPC-HDA server.
 
     Processed values are calculated values, based on the aggregate
     function requested for each item. The list of aggregates can be
     obtained by calling system.opchda.getAggregates().
 
     Args:
-        serverName: The name of the defined OPC-HDA Server to read.
-        itemIds: A list of item ids to read.
-        startDate: The starting date/time of the query.
-        endDate: The ending date/time of the query.
-        resampleIntervalMS: The interval, in milliseconds, that each
-            value should cover.
-        aggregates: A list which should be one-to-one with the item ids
-            requested, specifying the integer id of the aggregation
-            function to use. The aggregation ids are defined in the
-            OPC-HDA specification. The list of aggregates can also be
-            obtained by calling system.opchda.getAggregates().
-
-    Returns:
-        A list of read results which is one-to-one with the item IDs
-        passed in. The ReadResult object has a 'serviceResult' quality
-        property that indicates whether the call was successful, and is
-        itself a list of QualifiedValues.
+        serverName (str): The name of the defined OPC-HDA server to
+            read.
+        itemIds (list[str]): A list of item ids to read.
+        startDate (Date): The starting date/time of the query.
+        endDate (Date): The ending date/time of the query.
+        resampleIntervalMS (int): The interval, in milliseconds, that
+            each value should cover.
+        aggregates (list[object]): A list which should be one-to-one
+            with the item ids requested, specifying the integer id of
+            the aggregation function to use. The aggregation ids are
+            defined in the OPC-HDA specification. The list of aggregates
+            can also be obtained by calling
+            system.opchda.getAggregates().
+
+    Returns:
+        list[ReadResult]: A list of read results which is one-to-one
+            with the item IDs passed in. The ReadResult object has a
+            'serviceResult' quality property that indicates whether the
+            call was successful, and is itself a list of
+            QualifiedValues.
     """
     print(
         serverName,
         itemIds,
         startDate,
         endDate,
         resampleIntervalMS,
         aggregates,
     )
-    return [ReadResult() for _ in itemIds]
+    return []
 
 
 def readRaw(
-    serverName,  # type: AnyStr
-    itemIds,  # type: List[AnyStr]
-    startDate,  # type: Date
-    endDate,  # type: Date
-    maxValues,  # type: int
-    boundingValues,  # type: bool
+    serverName, itemIds, startDate, endDate, maxValues, boundingValues
 ):
-    # type: (...) -> List[Any]
-    """Reads raw values from the OPC-HDA Server.
+    """Reads raw values from the OPC-HDA server.
 
     Args:
-        serverName: The name of the defined OPC-HDA Server to read.
-        itemIds: A list of item ids to read.
-        startDate: The starting date/time of the query.
-        endDate: The ending date/time of the query.
-        maxValues: The maximum number of values to return. 0 or less
-            means unlimited.
-        boundingValues: A boolean indicating whether or not the
+        serverName (str): The name of the defined OPC-HDA server to
+            read.
+        itemIds (list[str]): A list of item ids to read.
+        startDate (Date): The starting date/time of the query.
+        endDate (Date): The ending date/time of the query.
+        maxValues (int): The maximum number of values to return. 0 or
+            less means unlimited.
+        boundingValues (bool): A boolean indicating whether or not the
             "bounding values" should be included in the result set. The
             bounding values provide a value exactly at the start and end
             dates, but may be resource-intensive to retrieve.
 
     Returns:
-        A list of read results which is one-to-one with the item IDs
-        passed in. The ReadResult object has a 'serviceResult' quality
-        property that indicates whether the call was successful, and is
-        itself a list of QualifiedValues.
+        list[ReadResult]: A list of read results which is one-to-one
+            with the item IDs passed in. The ReadResult object has a
+            'serviceResult' quality property that indicates whether the
+            call was successful, and is itself a list of
+            QualifiedValues.
     """
     print(serverName, itemIds, startDate, endDate, maxValues, boundingValues)
-    return [ReadResult() for _ in itemIds]
+    return []
 
 
 def replace(serverName, itemId, value, date, quality):
-    # type: (AnyStr, AnyStr, Any, Date, int) -> QualityCode
-    """Replaces values on the OPC-HDA Server if the given item ID
+    """Replaces values on the OPC-HDA server if the given item ID
     exists.
 
     Args:
-        serverName: The name of the defined OPC-HDA Server.
-        itemId: The item ID to perform the operation on.
-        value: The value to replace.
-        date: The date to replace.
-        quality: The quality to replace.
+        serverName (str): The name of the defined OPC-HDA server.
+        itemId (str): The item ID to perform the operation on.
+        value (object): The value to replace.
+        date (Date): The date to replace.
+        quality (int): The quality to replace.
 
     Returns:
-        The items quality resulting from the operation.
+        int: The item's quality resulting from the operation.
     """
     print(serverName, itemId, value, date, quality)
-    return QualityCode()
+    return 192
```

### Comparing `ignition_api-8.1.40/src/system/file.py` & `ignition-api-8.1.9/src/system/file.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """File Functions.
 
 The following functions give you access to read and write to files.
 """
 
 from __future__ import print_function
 
@@ -15,216 +19,167 @@
     "saveFile",
     "writeFile",
 ]
 
 import io
 import os.path
 import tempfile
-from typing import Any, List, Optional
-
-from dev.coatl.helper.types import AnyStr
 
 
 def fileExists(filepath):
-    # type: (AnyStr) -> bool
     """Checks to see if a file or folder at a given path exists.
 
-    Note:
-        This function is scoped for Perspective Sessions, but since all
-        scripts in Perspective run on the Gateway, the file must be
-        located on the Gateway's file system.
-
     Args:
-        filepath: The path of the file or folder to check.
+        filepath (str): The path of the file or folder to check.
 
     Returns:
-        True if the file/folder exists, False otherwise.
+        bool: True (1) if the file/folder exists, False (0) otherwise.
     """
     return os.path.isfile(filepath)
 
 
 def getTempFile(extension):
-    # type: (AnyStr) -> AnyStr
     """Creates a new temp file on the host machine with a certain
     extension, returning the path to the file.
 
     The file is marked to be removed when the Java VM exits.
 
-    Note:
-        This function is scoped for Perspective Sessions, but since all
-        scripts in Perspective run on the Gateway, the file must be
-        located on the Gateway's file system.
-
     Args:
-        extension: An extension, like ".txt", to append to the end of
-            the temporary file.
+        extension (str): An extension, like ".txt", to append to the end
+            of the temporary file.
 
     Returns:
-        The path to the newly created temp file.
+        str: The path to the newly created temp file.
     """
     suffix = ".{}".format(extension)
     with tempfile.NamedTemporaryFile(suffix=suffix) as temp:
-        return unicode(temp.name)
+        name = temp.name
+    return name
 
 
 def openFile(extension=None, defaultLocation=None):
-    # type: (Optional[AnyStr], Optional[AnyStr]) -> Optional[AnyStr]
     r"""Shows an "Open File" dialog box, prompting the user to choose a
     file to open.
 
     Returns the path to the file that the user chose, or None if the
     user canceled the dialog box. An extension can optionally be passed
     in that sets the filetype filter to that extension.
 
     Args:
-        extension: A file extension, like "pdf", to try to open.
+        extension (str): A file extension, like "pdf", to try to open.
             Optional.
-        defaultLocation: A folder location, like "C:\\MyFiles", to use
-            as the starting location for the file chooser. Optional.
+        defaultLocation (str): A folder location, like "C:\\MyFiles", to
+            use as the starting location for the file chooser. Optional.
 
     Returns:
-        The path to the selected file, or None if canceled.
+        str: The path to the selected file, or None if canceled.
     """
     print(extension, defaultLocation)
-    return ""
 
 
-def openFiles(
-    extension=None,  # type: Optional[AnyStr]
-    defaultLocation=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> Optional[List[AnyStr]]
+def openFiles(extension=None, defaultLocation=None):
     r"""Shows an "Open File" dialog box, prompting the user to choose a
     file or files to open.
 
     Returns the paths to the files that the user chooses, or None if the
     user canceled the dialog box. An extension can optionally be passed
     in that sets the filetype filter to that extension.
 
     Args:
-        extension: A file extension, like "pdf", to try to open.
+        extension (str): A file extension, like "pdf", to try to open.
             Optional.
-        defaultLocation: A folder location, like "C:\\MyFiles", to use
-            as the starting location for the file chooser. Optional.
+        defaultLocation (str): A folder location, like "C:\\MyFiles", to
+            use as the starting location for the file chooser. Optional.
 
     Returns:
-        The paths to the selected files, or None if canceled.
+        list[str]: The paths to the selected files, or None if canceled.
     """
     print(extension, defaultLocation)
-    return ["path/to/file"]
 
 
 def readFileAsBytes(filepath):
-    # type: (AnyStr) -> Any
     """Opens the file found at path filename, and reads the entire file.
 
     Returns the file as an array of bytes. Commonly this array of bytes
     is uploaded to a database table with a column of type BLOB (Binary
     Large OBject). This upload would be done through an INSERT or UPDATE
     SQL statement run through the system.db.runPrepUpdate function. You
     could also write the bytes to another file using the
     system.file.writeFile function, or send the bytes as an email
     attachment using system.net.sendEmail.
 
-    Note:
-        This function is scoped for Perspective Sessions, but since all
-        scripts in Perspective run on the Gateway, the file must be
-        located on the Gateway's file system.
-
     Args:
-        filepath: The path of the file to read.
+        filepath (str): The path of the file to read.
 
     Returns:
-        The contents of the file as an array of bytes.
+        bytearray: The contents of the file as an array of bytes.
     """
-    with io.open(filepath, "r+b") as f:
-        return f.read()
+    with open(filepath, "rb") as _file:
+        return _file.read()
 
 
 def readFileAsString(filepath, encoding="UTF-8"):
-    # type: (AnyStr, Optional[AnyStr]) -> AnyStr
     """Opens the file found at path filename, and reads the entire file.
 
     Returns the file as a string. Common things to do with this string
     would be to load it into the text property of a component, upload it
     to a database table, or save it to another file using
     system.file.writeFile function.
 
-    Note:
-        This function is scoped for Perspective Sessions, but since all
-        scripts in Perspective run on the Gateway, the file must be
-        located on the Gateway's file system.
-
     Args:
-        filepath: The path of the file to read.
-        encoding: The character encoding of the file to be read. Will
-            throw an exception if the string does not represent a
+        filepath (str): The path of the file to read.
+        encoding (str): The character encoding of the file to be read.
+            Will throw an exception if the string does not represent a
             supported encoding. Common encodings are "UTF-8",
-            "ISO-8859-1" and "US-ASCII". Default is "UTF-8". Optional.
+            "ISO-8859-1" and "US-ASCII". Optional.
 
     Returns:
-        The contents of the file as a string.
+        str: The contents of the file as a string.
     """
-    with io.open(filepath, "r", encoding=encoding) as f:
-        return unicode(f.read())
+    with io.open(filepath, "r", encoding=encoding) as _file:
+        return _file.read()
 
 
-def saveFile(
-    filename,  # type: AnyStr
-    extension=None,  # type: Optional[AnyStr]
-    typeDesc=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> Optional[AnyStr]
+def saveFile(filename, extension=None, typeDesc=None):
     """Prompts the user to save a new file named filename.
 
     The optional extension and typeDesc arguments can be added to be
     used as a type filter. If the user accepts the save, the path to
     that file will be returned. If the user cancels the save, None will
     be returned.
 
     Args:
-        filename: A file name to suggest to the user.
-        extension: The appropriate file extension, like "jpeg", for the
-            file. Optional.
-        typeDesc: A description of the extension, like "JPEG Image".
-            Optional.
+        filename (str): A file name to suggest to the user.
+        extension (str): The appropriate file extension, like "jpeg",
+            for the file. Optional.
+        typeDesc (str): A description of the extension, like "JPEG
+            Image". Optional.
 
     Returns:
-        The path to the file that the user decided to save to, or None
-        if they canceled.
+        str: The path to the file that the user decided to save to, or
+            None if they canceled.
     """
     print(filename, extension, typeDesc)
-    return ""
 
 
-def writeFile(
-    filepath,  # type: AnyStr
-    data,  # type: Any
-    append=False,  # type: bool
-    encoding="UTF-8",  # type: AnyStr
-):
-    # type: (...) -> None
+def writeFile(filepath, data, append=False, encoding="UTF-8"):
     """Writes the given data to the file at file path filename.
 
     If the file exists, the append argument determines whether or not it
     is overwritten (the default) or appended to. The data argument can
     be either a string or an array of bytes (commonly retrieved from a
     BLOB in a database or read from another file using
     system.file.readFileAsBytes).
 
-    Note:
-        This function is scoped for Perspective Sessions, but since all
-        scripts in Perspective run on the Gateway, the file must be
-        located on the Gateway's file system.
-
     Args:
-        filepath: The path of the file to write to.
-        data: The character or binary content to write to the file.
-        append: If True, the file will be appended to if it already
-            exists. If False, the file will be overwritten if it
-            exists. The default is False. Optional.
-        encoding: The character encoding of the file to write. Will
-            throw an exception if the string does not represent a
+        filepath (str): The path of the file to write to.
+        data (object): The character or binary content to write to the
+            file.
+        append (bool): If True(1), the file will be appended to if it
+            already exists. If False(0), the file will be overwritten if
+            it exists. The default is False(0). Optional.
+        encoding (str): The character encoding of the file to write.
+            Will throw an exception if the string does not represent a
             supported encoding. Common encodings are "UTF-8",
             "ISO-8859-1" and "US-ASCII". Default is "UTF-8". Optional.
     """
     print(filepath, data, append, encoding)
```

### Comparing `ignition_api-8.1.40/src/system/date.py` & `ignition-api-8.1.9/src/system/date.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Date Functions.
 
 The following functions give you access to test and modify dates.
 """
 
-from __future__ import print_function
-
 __all__ = [
     "addDays",
     "addHours",
     "addMillis",
     "addMinutes",
     "addMonths",
     "addSeconds",
@@ -47,779 +49,688 @@
     "secondsBetween",
     "setTime",
     "toMillis",
     "weeksBetween",
     "yearsBetween",
 ]
 
-from datetime import datetime
+from calendar import monthrange
+from datetime import datetime, timedelta
 from time import localtime, mktime
-from typing import Optional, Union
 
-from dev.coatl.helper.types import AnyStr
 from java.util import Date, Locale
 
 
-def _now():
-    # type: () -> datetime
-    """Get current datetime.
-
-    Returns:
-        Now.
-    """
-    return datetime.now()
-
-
 def addDays(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of days to a given date and time.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
+        Date: A new date object offset by the integer passed to the
+            function.
     """
-    print(date, value)
-    return Date()
+    return date + timedelta(days=value)
 
 
 def addHours(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of hours to a given date and time.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
+        Date: A new date object offset by the integer passed to the
+            function.
     """
-    print(date, value)
-    return Date()
+    return date + timedelta(hours=value)
 
 
 def addMillis(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of milliseconds to a given date and
     time.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
+        Date: A new date object offset by the integer passed to the
+            function.
     """
-    print(date, value)
-    return Date()
+    return date + timedelta(milliseconds=value)
 
 
 def addMinutes(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of minutes to a given date and time.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
+        Date: A new date object offset by the integer passed to the
+            function.
     """
-    print(date, value)
-    return Date()
+    return date + timedelta(minutes=value)
 
 
 def addMonths(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of months to a given date and time.
 
     This function is unique since each month can have a variable number
     of days. For example, if the date passed in is March 31st, and we
     add one month, April does not have a 31st day, so the returned date
     will be the proper number of months rounded down to the closest
     available day, in this case April 30th.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
-    """
-    print(date, value)
-    return Date()
+        Date: A new date object offset by the integer passed to the
+            function.
+    """
+    month = (date.month + value) % 12
+    year = date.year + (date.month + value - 1) // 12
+    if not month:
+        month = 12
+    day = min(date.day, monthrange(year, month)[1])
+    return date.replace(day=day, month=month, year=year)
 
 
 def addSeconds(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of seconds to a given date and time.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
+        Date: A new date object offset by the integer passed to the
+            function.
     """
-    print(date, value)
-    return Date()
+    return date + timedelta(seconds=value)
 
 
 def addWeeks(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of weeks to a given date and time.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
+        Date: A new date object offset by the integer passed to the
+            function.
     """
-    print(date, value)
-    return Date()
+    return date + timedelta(weeks=value)
 
 
 def addYears(date, value):
-    # type: (Date, int) -> Date
     """Add or subtract an amount of years to a given date and time.
 
     Args:
-        date: The starting date.
-        value: The number of units to add, or subtract if the value is
-            negative.
+        date (Date): The starting date.
+        value (int): The number of units to add, or subtract if the
+            value is negative.
 
     Returns:
-        A new date object offset by the integer passed to the function.
+        Date: A new date object offset by the integer passed to the
+            function.
     """
-    print(date, value)
-    return Date()
+    return date.replace(year=date.year + value)
 
 
 def daysBetween(date_1, date_2):
-    # type: (Date, Date) -> int
     """Calculates the number of whole days between two dates.
 
     Daylight Saving Time changes are taken into account.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
+        int: An integer that is representative of the difference between
+            two dates.
     """
-    print(date_1, date_2)
-    return 1
+    return (date_2 - date_1).days
 
 
 def format(date, format="yyyy-MM-dd HH:mm:ss"):
-    # type: (Date, AnyStr) -> unicode
     """Returns the given date as a string, formatted according to a
     pattern.
 
-    The pattern is a format that is full of various placeholders that
-    display different parts of the date. These are case-sensitive. These
-    placeholders can be repeated for a different effect. For example, M
-    will give you 1-12, MM will give you 01-12, MMM will give you
-    Jan-Dec, MMMM will give you January-December.
-
     Note:
-        The functions above are based off the Java class
-        `SimpleDateFormat` internally. The functions will accept any
-        valid format string for that class.
+        Not all symbols from system.date.format() have a counterpart
+        directive on strftime().
 
     Args:
-        date: The date to format.
-        format: A format string such as "yyyy-MM-dd HH:mm:ss". The
-            format argument is optional. The default is
-            "yyyy-MM-dd HH:mm:ss". Optional.
+        date (Date): The date to format.
+        format (str): A format string such as "yyyy-MM-dd HH:mm:ss".
+            Optional.
 
     Returns:
-        A string representing the formatted datetime.
+        str: A string representing the formatted datetime
     """
-    print(date, format)
-    _date = _now()
-    _format = format
-    _format = _format.replace("a", "%p")
-    _format = _format.replace("D", "%j")
-    _format = _format.replace("dd", "{:02}".format(_date.day))
-    _format = _format.replace("d", "{}".format(_date.day))
-    _format = _format.replace("EEEE", "%A")
-    _format = _format.replace("E", "%a")
-    _format = _format.replace("F", "{}".format(_date.isocalendar()[2]))
-    _format = _format.replace("G", "AD")
-    _format = _format.replace("hh", "%I")
-    _format = _format.replace("h", "%-I")
-    _format = _format.replace("HH", "{:02}".format(_date.hour))
-    _format = _format.replace("H", "%-H")
-    _format = _format.replace("k", "%H")
-    _format = _format.replace("K", "%-I")
+    _format = format.replace("yyyy", "%Y")
+    _format = _format.replace("yy", "%y")
     _format = _format.replace("MMMM", "%B")
     _format = _format.replace("MMM", "%b")
-    _format = _format.replace("MM", "{:02}".format(_date.month))
-    _format = _format.replace("M", "{}".format(_date.month))
+    _format = _format.replace("MM", "%m")
+    _format = _format.replace("dd", "%d")
+    _format = _format.replace("HH", "%H")
+    _format = _format.replace("hh", "%I")
     _format = _format.replace("mm", "%M")
-    _format = _format.replace("m", "%-M")
-    _millis = _date.microsecond % 1000
-    _format = _format.replace("SSS", "{:03}".format(_millis))
-    _format = _format.replace("SS", "{:02}".format(_millis))
-    _format = _format.replace("S", "{:01}".format(_millis))
+    _format = _format.replace("S", "%f")
     _format = _format.replace("ss", "%S")
-    _format = _format.replace("s", "%-S")
-    _format = _format.replace("w", "{}".format(_date.isocalendar()[1] + 1))
-    _format = _format.replace("u", "%w")
-    _format = _format.replace(
-        "W",
-        "{}".format(_date.isocalendar()[1] - _date.replace(day=1).isocalendar()[1] + 1),
-    )
-
-    _format = _format.replace("XXX", "{:03.0f}:00".format(getTimezoneOffset()))
-    _format = _format.replace("XX", "{:03.0f}00".format(getTimezoneOffset()))
-    _format = _format.replace("X", "{:03.0f}".format(getTimezoneOffset()))
-    _format = _format.replace("yyyy", "{}".format(_date.year))
-    _format = _format.replace("yy", str(_date.year)[-2:])
-    _format = _format.replace("Y", "%Y")
-    _format = _format.replace("y", "%Y")
-    _format = _format.replace("Z", "{:03.0f}00".format(getTimezoneOffset()))
-    _format = _format.replace("z", "PDT")
-    return unicode(_date.strftime(_format))
+    _format = _format.replace("z", "%Z")
+    _format = _format.replace("Z", "%z")
+    _format = _format.replace("a", "%p")
+    _format = _format.replace("w", "%U")
+    _format = _format.replace("D", "%j")
+    return date.strftime(_format)
 
 
 def fromMillis(millis):
-    # type: (int) -> Date
     """Creates a date object given a millisecond value.
 
     Args:
-        millis: The number of milliseconds elapsed since January 1,
-            1970, 00:00:00 UTC (GMT).
+        millis (long): The number of milliseconds elapsed since
+            January 1, 1970, 00:00:00 UTC (GMT).
 
     Returns:
-        A new date object.
+        Date: A new date object.
     """
-    return Date(millis)
+    seconds = millis // 1000
+    micro = (millis % 1000) * 1000
+    _date = datetime.fromtimestamp(seconds)
+    return datetime(
+        _date.year,
+        _date.month,
+        _date.day,
+        _date.hour,
+        _date.minute,
+        _date.second,
+        micro,
+    )
 
 
 def getAMorPM(date):
-    # type: (Date) -> int
     """Returns a 0 if the time is before noon, and a 1 if the time is
     after noon.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return 1 if _now().hour >= 12 else 0
+    return 1 if date.hour >= 12 else 0
 
 
 def getDate(year, month, day):
-    # type: (int, int, int) -> Date
     """Creates a new Date object given a year, month and a day.
 
     The time will be set to midnight of that day.
 
     Args:
-        year: The year for the new date.
-        month: The month of the new date. January is month 0.
-        day: The day of the month for the new date. The first day
+        year (int): The year for the new date.
+        month (int): The month of the new date. January is month 0.
+        day (int): The day of the month for the new date. The first day
             of the month is day 1.
 
     Returns:
-        A new date, set to midnight of that day.
+        Date: A new date, set to midnight of that day.
     """
-    print(year, month, day)
-    return Date()
+    _jan = datetime(year, 1, day)
+    return addMonths(_jan, month)
 
 
 def getDayOfMonth(date):
-    # type: (Date) -> int
-    """Extracts the day of the month from a date.
-
-    The first day of the month is day 1.
+    """Extracts the day of the month from a date. The first day of the
+    month is day 1.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().day
+    return date.day
 
 
 def getDayOfWeek(date):
-    # type: (Date) -> int
     """Extracts the day of the week from a date.
 
     Sunday is day 1, Saturday is day 7.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
     _dow = [2, 3, 4, 5, 6, 7, 1]
-    return _dow[_now().weekday()]
+    return _dow[date.weekday()]
 
 
 def getDayOfYear(date):
-    # type: (Date) -> int
-    """Extracts the day of the year from a date.
-
-    The first day of the year is day 1.
+    """Extracts the day of the year from a date. The first day of the
+    year is day 1.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().timetuple().tm_yday
+    return date.timetuple().tm_yday
 
 
 def getHour12(date):
-    # type: (Date) -> int
-    """Extracts the hour from a date.
-
-    Uses a 12 hour clock, so noon and midnight are returned as 0.
+    """Extracts the hour from a date. Uses a 12 hour clock, so noon and
+    midnight are returned as 0.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().hour - 12 if _now().hour >= 12 else _now().hour
+    return date.hour - 12 if date.hour >= 12 else date.hour
 
 
 def getHour24(date):
-    # type: (Date) -> int
-    """Extracts the hour from a date.
-
-    Uses a 24 hour clock, so midnight is zero.
+    """Extracts the hour from a date. Uses a 24 hour clock, so midnight
+    is zero.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().hour
+    return date.hour
 
 
 def getMillis(date):
-    # type: (Date) -> int
     """Extracts the milliseconds from a date, ranging from 0-999.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().microsecond // 1000
+    return date.microsecond // 1000
 
 
 def getMinute(date):
-    # type: (Date) -> int
     """Extracts the minutes from a date, ranging from 0-59.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().minute
+    return date.minute
 
 
 def getMonth(date):
-    # type: (Date) -> int
     """Extracts the month from a date, where January is month 0.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().month
+    return date.month - 1
 
 
 def getQuarter(date):
-    # type: (Date) -> int
     """Extracts the quarter from a date, ranging from 1-4.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return ((_now().month - 1) // 3) + 1
+    return ((date.month - 1) // 3) + 1
 
 
 def getSecond(date):
-    # type: (Date) -> int
     """Extracts the seconds from a date, ranging from 0-59.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().second
+    return date.second
 
 
 def getTimezone():
-    # type: () -> AnyStr
     """Returns the ID of the current timezone.
 
     Returns:
-        A representation of the current timezone.
+        str: A representation of the current timezone.
     """
     return "America/Tijuana"
 
 
-def getTimezoneOffset(date=None):
-    # type: (Optional[Date]) -> float
+def getTimezoneOffset(date=datetime.now()):
     """Returns the current timezone's offset versus UTC for a given
     instant, taking Daylight Saving Time into account.
 
     Args:
-        date: The instant in time for which to calculate the offset.
-            Uses now() if omitted. Optional.
+        date (Date): The instant in time for which to calculate the
+            offset. Uses now() if omitted. Optional.
 
     Returns:
-        The timezone offset compared to UTC, in hours.
+        float: The timezone offset compared to UTC, in hours.
     """
     return -7.0 if isDaylightTime(date) else -8.0
 
 
 def getTimezoneRawOffset():
-    # type: () -> float
     """Returns the current timezone offset versus UTC, not taking
     Daylight Saving Time into account.
 
     Returns:
-         The timezone offset.
+         float: The timezone offset.
     """
-    return float(0)
+    offset = -1.0 if isDaylightTime() else 0.0
+    return float(hoursBetween(datetime.utcnow(), datetime.now())) + offset
 
 
 def getYear(date):
-    # type: (Date) -> int
     """Extracts the year from a date.
 
     Args:
-        date: The date to use.
+        date (Date): The date to use.
 
     Returns:
-        An integer that is representative of the extracted value.
+        int: An integer that is representative of the extracted value.
     """
-    print(date)
-    return _now().year
+    return date.year
 
 
 def hoursBetween(date_1, date_2):
-    # type: (Date, Date) -> int
     """Calculates the number of whole hours between two dates.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
+        int: An integer that is representative of the difference between
+            two dates.
     """
-    print(date_1, date_2)
-    return 1
+    diff = date_2 - date_1
+    days, seconds, _ = diff.days, diff.seconds, diff.microseconds
+    return days * 24 + seconds // 3600
 
 
 def isAfter(date_1, date_2):
-    # type: (Date, Date) -> bool
     """Compares two dates to see if date_1 is after date_2.
 
     Args:
-        date_1: The first date.
-        date_2: The second date.
+        date_1 (Date): The first date.
+        date_2 (Date): The second date.
 
     Returns:
-        True if date_1 is after date_2, False otherwise.
+        bool: True (1) if date_1 is after date_2, False (0) otherwise.
     """
-    print(date_1, date_2)
-    return True
+    return date_1 > date_2
 
 
 def isBefore(date_1, date_2):
-    # type: (Date, Date) -> bool
     """Compares to dates to see if date_1 is before date_2.
 
     Args:
-        date_1: The first date.
-        date_2: The second date.
+        date_1 (Date): The first date.
+        date_2 (Date): The second date.
 
     Returns:
-        True if date_1 is before date_2, False otherwise.
+        bool: True (1) if date_1 is before date_2, False (0) otherwise.
     """
-    print(date_1, date_2)
-    return False
+    return date_1 < date_2
 
 
 def isBetween(target_date, start_date, end_date):
-    # type: (Date, Date, Date) -> bool
     """Compares two dates to see if a target date is between two other
     dates.
 
     Args:
-        target_date: The date to compare.
-        start_date: The start of a date range.
-        end_date: The end of a date range. This date must be after the
-            start date.
+        target_date (Date): The date to compare.
+        start_date (Date): The start of a date range.
+        end_date (Date): The end of a date range. This date must be
+            after the start date.
 
     Returns:
-        True if target_date is >= start_date and target_date <=
-        end_date, False otherwise.
+        bool: True (1) if target_date is >= start_date and
+            target_date <= end_date, False (0) otherwise.
     """
-    print(target_date, start_date, end_date)
-    return True
+    return start_date <= target_date <= end_date
 
 
-def isDaylightTime(date=None):
-    # type: (Optional[Date]) -> bool
+def isDaylightTime(date=datetime.now()):
     """Checks to see if the current timezone is using Daylight Saving
     Time during the date specified.
 
     Args:
-        date: The date you want to check if the current timezone is
-            observing Daylight Saving Time. Uses now() if omitted.
-            Optional.
+        date (Date): The date you want to check if the current
+            timezone is observing Daylight Saving Time. Uses now() if
+            omitted. Optional.
 
     Returns:
-        True if date is observing Daylight Saving Time in the
-        current timezone, False otherwise.
+        bool: True (1) if date is observing Daylight Saving Time in the
+            current timezone, False (0) otherwise.
     """
-    print(date)
-    _date = _now()
     time_tuple = (
-        _date.year,
-        _date.month,
-        _date.day,
-        _date.hour,
-        _date.minute,
-        _date.second,
-        _date.weekday(),
+        date.year,
+        date.month,
+        date.day,
+        date.hour,
+        date.minute,
+        date.second,
+        date.weekday(),
         0,
         0,
     )
     stamp = mktime(time_tuple)
     time_tuple = localtime(stamp)
     return time_tuple.tm_isdst > 0
 
 
 def midnight(date):
-    # type: (Date) -> Date
     """Returns a copy of a date with the hour, minute, second, and
     millisecond fields set to zero.
 
     Args:
-        date: The starting date.
+        date (Date): The starting date.
 
     Returns:
-        A new date, set to midnight of the day provided.
+        Date: A new date, set to midnight of the day provided.
     """
-    print(date)
-    return Date()
+    return date.replace(hour=0, minute=0, second=0, microsecond=0)
 
 
 def millisBetween(date_1, date_2):
-    # type: (Date, Date) -> long
     """Calculates the number of whole milliseconds between two dates.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
+        long: An integer that is representative of the difference
+            between two dates.
     """
-    print(date_2, date_1)
-    return long(1)
+    diff = date_2 - date_1
+    days, seconds, microseconds = diff.days, diff.seconds, diff.microseconds
+    return days * 86400 * 1000 + seconds * 1000 + microseconds // 1000
 
 
 def minutesBetween(date_1, date_2):
-    # type: (Date, Date) -> int
     """Calculates the number of whole minutes between two dates.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
+        int: An integer that is representative of the difference between
+            two dates.
     """
-    print(date_2, date_1)
-    return 1
+    diff = date_2 - date_1
+    days, seconds, _ = diff.days, diff.seconds, diff.microseconds
+    return days * 1440 + seconds // 60
 
 
 def monthsBetween(date_1, date_2):
-    # type: (Date, Date) -> int
-    """Calculates the number of whole months between two dates.
-
-    Daylight Saving Time changes are taken into account.
+    """Calculates the number of whole months between two dates. Daylight
+    Saving Time changes are taken into account.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
-    """
-    print(date_1, date_2)
-    return 0
+        int: An integer that is representative of the difference between
+            two dates.
+    """
+    delta = 0
+    while True:
+        mdays = monthrange(date_1.year, date_2.month)[1]
+        date_1 += timedelta(days=mdays)
+        if date_1 <= date_2:
+            delta += 1
+        else:
+            break
+    return delta
 
 
 def now():
-    # type: () -> Date
     """Returns a java.util.Date object that represents the current time
     according to the local system clock.
 
     Returns:
-        A new date, set to the current date and time.
+        Date: A new date, set to the current date and time.
     """
-    return Date()
-
+    return datetime.now()
 
-def parse(dateString, formatString="yyyy-MM-dd HH:mm:ss", locale=Locale.ENGLISH):
-    # type: (AnyStr, AnyStr, Union[AnyStr, Locale, None]) -> Date
-    """Attempts to parse a string and create a Date.
 
-    Causes ParseException if the date dateString parameter is in an
+def parse(
+    dateString, formatString="yyyy-MM-dd HH:mm:ss", locale=Locale.ENGLISH
+):
+    """Attempts to parse a string and create a Date. Causes
+    ParseException if the date dateString parameter is in an
     unrecognized format.
 
     Args:
-        dateString: The string to parse into a date.
-        formatString: Format string used by the parser. Default is
+        dateString (str): The string to parse into a date.
+        formatString (str): Format string used by the parser. Default is
             "yyyy-MM-dd HH:mm:ss". Optional.
-        locale: Locale used for parsing. Can be the locale name
-            such as 'fr', or the Java Locale such as 'Locale.FRENCH'.
-            Default is 'Locale.ENGLISH'. Optional.
+        locale (object): Locale used for parsing. Can be the locale name
+            such as 'fr', or the Java Locale such as 'Locale.French'.
+            Default is 'Locale.English'. Optional.
 
     Returns:
-        The parsed date.
+        Date: The parsed date.
     """
     print(dateString, formatString, locale)
-    return Date()
+    return now()
 
 
 def secondsBetween(date_1, date_2):
-    # type: (Date, Date) -> int
     """Calculates the number of whole seconds between two dates.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
+        int: An integer that is representative of the difference between
+            two dates.
     """
-    print(date_2, date_1)
-    return 0
+    diff = date_2 - date_1
+    days, seconds, _ = diff.days, diff.seconds, diff.microseconds
+    return days * 86400 + seconds
 
 
 def setTime(date, hour, minute, second):
-    # type: (Date, int, int, int) -> Date
     """Takes in a date, and returns a copy of it with the time fields
     set as specified.
 
     Args:
-        date: The starting date.
-        hour: The hours (0-23) to set.
-        minute: The minutes (0-59) to set.
-        second: The seconds (0-59) to set.
+        date (Date): The starting date.
+        hour (int): The hours (0-23) to set.
+        minute(int): The minutes (0-59) to set.
+        second (int): The seconds (0-59) to set.
 
     Returns:
-        A new date, set to the appropriate time.
+        Date: A new date, set to the appropriate time.
     """
-    print(date, hour, minute, second)
-    return Date()
+    return date.replace(hour=hour, minute=minute, second=second, microsecond=0)
 
 
 def toMillis(date):
-    # type: (Date) -> long
     """Converts a Date object to its millisecond value elapsed since
     January 1, 1970, 00:00:00 UTC (GMT).
 
     Args:
-        date: The date object to convert.
+        date (Date): The date object to convert.
 
     Returns:
-        An 8-byte integer representing the number of millisecond elapsed
-        since January 1, 1970, 00:00:00 UTC (GMT).
+        int: 8-byte integer representing the number of millisecond
+            elapsed since January 1, 1970, 00:00:00 UTC (GMT).
     """
-    print(date)
-    _date = _now()
-    millis = mktime(_date.timetuple()) * 1000 + _date.microsecond // 1000
-    return long(millis)
+    millis = mktime(date.timetuple()) * 1000 + date.microsecond // 1000
+    return int(millis)
 
 
 def weeksBetween(date_1, date_2):
-    # type: (Date, Date) -> int
     """Calculates the number of whole weeks between two dates.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
+        int: An integer that is representative of the difference between
+            two dates.
     """
-    print(date_1, date_2)
-    return 0
+    diff = date_2 - date_1
+    return diff.days // 7
 
 
 def yearsBetween(date_1, date_2):
-    # type: (Date, Date) -> int
-    """Calculates the number of whole years between two dates.
-
-    Daylight Saving Time changes are taken into account.
+    """Calculates the number of whole years between two dates. Daylight
+    Saving Time changes are taken into account.
 
     Args:
-        date_1: The first date to use.
-        date_2: The second date to use.
+        date_1 (Date): The first date to use.
+        date_2 (Date): The second date to use.
 
     Returns:
-        An integer that is representative of the difference between two
-        dates.
+        int: An integer that is representative of the difference between
+            two dates.
     """
-    print(date_1, date_2)
-    return 0
+    return monthsBetween(date_1, date_2) // 12
```

### Comparing `ignition_api-8.1.40/src/system/report.py` & `ignition-api-8.1.9/src/system/report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Report Functions.
 
 The following functions give you access to report details and the
 ability to run reports.
 """
 
 from __future__ import print_function
@@ -9,86 +13,64 @@
 __all__ = [
     "executeAndDistribute",
     "executeReport",
     "getReportNamesAsDataset",
     "getReportNamesAsList",
 ]
 
-from typing import Any, Dict, List, Optional
-
-from com.inductiveautomation.ignition.common import BasicDataset
-from dev.coatl.helper.types import AnyStr
 from java.lang import IllegalArgumentException
+from system.dataset import Dataset
 
 
 def executeAndDistribute(
-    path,  # type: AnyStr
-    project="project",  # type: AnyStr
-    parameters=None,  # type: Optional[Dict[AnyStr, int]]
-    action=None,  # type: Optional[AnyStr]
-    actionSettings=None,  # type: Optional[Dict[AnyStr, Any]]
+    path, project="project", parameters=None, action=None, actionSettings=None
 ):
-    # type: (...) -> None
     """Executes and distributes a report.
 
     Similar to scheduling a report to execute, except a schedule in not
     required to utilize this function. This is a great way to distribute
-    the report on demand from a Client.
-
-    Note:
-        The function system.report.executeAndDistribute() does not run
-        on its own thread and can get blocked. For example, if a printer
-        is backed up and it takes a while to finish the request made by
-        this function, the script will block the execution of other
-        things on that thread until it finishes. Be sure to keep this in
-        mind when using it in a script.
+    the report on demand from a client.
 
     Args:
-        path: The path to the existing report.
-        project: The name of the project where the report is located.
-            Optional in client scope.
-        parameters: An optional dictionary of parameter overrides, in
-            the form name:value.
-        action: The name of the distribution action to use.
-        actionSettings: An optional dictionary of settings particular to
-            the action. Missing values will use the default value for
-            that action.
+        path (str): The path to the existing report.
+        project (str): The name of the project where the report is
+            located. Optional in client scope.
+        parameters (dict): An optional dictionary of parameter
+            overrides, in the form name:value.
+        action (str): The name of the distribution action to use.
+        actionSettings (dict): An optional dictionary of settings
+            particular to the action. Missing values will use the
+            default value for that action.
 
     Raises:
         IllegalArgumentException: Thrown when any of the following
             occurs: If the file type is not recognized, path does not
             exist, project does not exist, or a key is not valid.
     """
-    if project is None:
+    if project is not None:
+        print(path, project, parameters, action, actionSettings)
+    else:
         raise IllegalArgumentException()
 
-    print(path, project, parameters, action, actionSettings)
 
-
-def executeReport(
-    path,  # type: AnyStr
-    project="project",  # type: AnyStr
-    parameters=None,  # type: Optional[Dict[AnyStr, int]]
-    fileType="pdf",  # type: AnyStr
-):
-    # type: (...) -> Any
+def executeReport(path, project="project", parameters=None, fileType="pdf"):
     """Immediately executes an existing report and returns a byte[] of
     the output.
 
     Args:
-        path: The path to the existing report.
-        project: The name of the project where the report is located.
-            Optional in client scope.
-        parameters: An optional dictionary of parameter overrides, in
-            the form name:value. Optional.
-        fileType: The file type the resulting byte array should
+        path (str): The path to the existing report.
+        project (str): The name of the project where the report is
+            located. Optional in client scope.
+        parameters (dict): An optional dictionary of parameter
+            overrides, in the form name:value. Optional.
+        fileType (str): The file type the resulting byte array should
             represent. Defaults to "pdf". Not case-sensitive. Optional.
 
     Returns:
-        A byte array of the resulting report.
+        object: A byte array of the resulting report.
 
     Raises:
         IllegalArgumentException: Thrown when any of the following
             occurs: If the file type is not recognized, path does not
             exist, project does not exist.
     """
     file_types = [
@@ -104,52 +86,54 @@
     ]
     if path is None or project is None or fileType not in file_types:
         raise IllegalArgumentException()
     print(path, project, parameters, fileType)
 
 
 def getReportNamesAsDataset(project="project", includeReportName=True):
-    # type: (Optional[AnyStr], bool) -> BasicDataset
     """Gets a data of all reports for a project.
 
+    This dataset is particularly suited for display in a Tree View
+    component.
+
     Args:
-        project: The name of the project where the reports are located.
-            Optional in client scope.
-        includeReportName: When set to False, the end of Path does not
-            include the report name. Default is True. Optional.
+        project (str): The name of the project where the reports are
+            located. Optional in client scope.
+        includeReportName (bool): When set to False, the end of Path
+            does not include the report name. Default is True. Optional.
 
     Returns:
-        A dataset of report paths and names for the project. Returns an
-        empty dataset if the project has no reports.
+        Dataset: A dataset of report paths and names for the project.
+            Returns an empty dataset if the project has no reports.
 
     Raises:
         IllegalArgumentException: Thrown when any of the following
             occurs: If the project name is omitted in the Gateway scope,
             project does not exist.
     """
     if project is None:
         raise IllegalArgumentException()
 
     print(project, includeReportName)
-    return BasicDataset()
+    return Dataset()
 
 
 def getReportNamesAsList(project="project"):
-    # type: (Optional[AnyStr]) -> List[AnyStr]
     """Gets a list of all reports for a project.
 
     Args:
-        project: The name of the project where the reports are located.
-            Optional in client scope.
+        project (str): The name of the project where the reports are
+            located. Optional in client scope.
 
     Returns:
-        A list of report paths for the project. Returns an empty list if
-        the project has no reports.
+        list[str]: A list of report paths for the project. Returns an
+            empty list if the project has no reports.
 
     Raises:
         IllegalArgumentException: Thrown when any of the following
             occurs: If the project name is omitted in the Gateway scope,
             project does not exist.
     """
     if project is None:
         raise IllegalArgumentException()
+
     return []
```

### Comparing `ignition_api-8.1.40/src/system/secsgem.py` & `ignition-api-8.1.9/src/system/secsgem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """SECS/GEM Functions.
 
 The following functions allow you to interact with equipment defined by
 the SECS/GEM module. Note that the SECS/GEM module must be installed
 before these functions will be accessible.
 """
 
@@ -17,69 +21,66 @@
     "sendRequest",
     "sendResponse",
     "startSimEventRun",
     "toDataSet",
     "toTreeDataSet",
 ]
 
-from typing import Any, Dict, List, Optional, Tuple
-
-from com.inductiveautomation.ignition.common import BasicDataset
-from dev.coatl.helper.types import AnyStr
-from java.util import Date
+import system.date
+from system.dataset import Dataset
 
 
 def copyEquipment(
-    equipmentSource,  # type: AnyStr
-    newEquipmentName,  # type: AnyStr
-    enabled,  # type: bool
-    activeAddress,  # type: AnyStr
-    activePort,  # type: int
-    passiveAddress,  # type: AnyStr
-    passivePort,  # type: int
-    deviceId,  # type: int
-    dbTablePrefix=None,  # type: Optional[AnyStr]
-    description=None,  # type: Optional[AnyStr]
+    equipmentSource,
+    newEquipmentName,
+    enabled,
+    activeAddress,
+    activePort,
+    passiveAddress,
+    passivePort,
+    deviceId,
+    dbTablePrefix=None,
+    description=None,
 ):
-    # type: (...) -> None
     """Creates a copy of an equipment connection.
 
     Common settings can be overridden for the new connection.
 
     An exception is thrown if the new Equipment Connection cannot be
     created.
 
     Args:
-        equipmentSource: Some new equipment settings will be retrieved
-            from this equipment connection. Specify the source equipment
-            connection name.
-        newEquipmentName: The name of the new equipment connection.
-        enabled: If set to False, the new equipment connection will be
-            disabled after it is created.
-        activeAddress: IP Address of new equipment. Must be specified if
-            the SECS/GEM module is used in Active mode. Otherwise, do
-            not use this parameter.
-        activePort: Port number of new equipment. Must be specified if
-            the SECS/GEM module is used in Active mode. Otherwise, do
-            not use this parameter.
-        passiveAddress: IP Address of new equipment. Must be specified
-            if the SECS/GEM module is used in Passive mode. Otherwise,
-            do not use this parameter.
-        passivePort: Port number of new equipment. Must be specified if
-            the SECS/GEM module is used in Passive mode. Otherwise, do
-            not use this parameter.
-        deviceId: Unique identifier of new equipment. This value must be
-            an integer, and is specified within the equipment.
-        dbTablePrefix: SECS/GEM database table names will use the
+        equipmentSource (str): Some new equipment settings will be
+            retrieved from this equipment connection. Specify the source
+            equipment connection name.
+        newEquipmentName (str): The name of the new equipment
+            connection.
+        enabled (bool): If set to False, the new equipment connection
+            will be disabled after it is created.
+        activeAddress (str): IP Address of new equipment. Must be
+            specified if the SECS/GEM module is used in Active mode.
+            Otherwise, do not use this parameter.
+        activePort (int): Port number of new equipment. Must be
+            specified if the SECS/GEM module is used in Active mode.
+            Otherwise, do not use this parameter.
+        passiveAddress (str): IP Address of new equipment. Must be
+            specified if the SECS/GEM module is used in Passive mode.
+            Otherwise, do not use this parameter.
+        passivePort (int): Port number of new equipment. Must be
+            specified if the SECS/GEM module is used in Passive mode.
+            Otherwise, do not use this parameter.
+        deviceId (int): Unique identifier of new equipment. This value
+            must be an integer, and is specified within the equipment.
+        dbTablePrefix (str): SECS/GEM database table names will use the
             specified prefix for the new equipment connection. If no
             prefix is specified, the description of the source equipment
             will be used. Optional.
-        description: The description for the new equipment connection.
-            If no description is specified, the description of the
-            source equipment will be used. Optional.
+        description (str): The description for the new equipment
+            connection. If no description is specified, the description
+            of the source equipment will be used. Optional.
     """
     print(
         equipmentSource,
         newEquipmentName,
         enabled,
         activeAddress,
         activePort,
@@ -88,216 +89,204 @@
         deviceId,
         dbTablePrefix,
         description,
     )
 
 
 def deleteToolProgram(ppid):
-    # type: (AnyStr) -> None
     """Deletes a process program from the Gateway.
 
     Args:
-        ppid: The PPID that was sent from the tool when the S7F3 message
-            was saved.
+        ppid (str): The PPID that was sent from the tool when the S7F3
+            message was saved.
     """
     print(ppid)
 
 
 def enableDisableEquipment(enable, names):
-    # type: (bool, Tuple[AnyStr, ...]) -> List[unicode]
     """Enables or disables a Tuple of equipment connections from a
     script.
 
     Args:
-        enable: Set to True to enable equipment connections, or set to
-            False to disable them.
-        names: A Tuple of Strings. Each string should match an Equipment
-            Connection configured on the Gateway. If this parameter
-            contains the name of an Equipment Connection that does not
-            exist, then a message will be included in the List returned
-            by this function.
+        enable (bool): Set to True to enable equipment connections, or
+            set to False to disable them.
+        names (tuple[str]): A Tuple of Strings. Each String should match
+            an Equipment Connection configured on the Gateway. If this
+            parameter contains the name of an Equipment Connection that
+            does not exist, then a message will be included in the List
+            returned by this function.
 
     Returns:
-         A List of unicode strings. Each string contains a message about
-         an equipment connection that could not be enabled/disabled. If
-         the list is empty, then all specified equipment connections
-         were successfully modified.
+         list[str]: A List of unicode strings. Each string contains a
+            message about an equipment connection that could not be
+            enabled/disabled. If the list is empty, then all specified
+            equipment connections were successfully modified.
     """
     print(enable)
     for name in names:
         print(name)
-    return [unicode("")]
+    return [""]
 
 
 def getResponse(transactionID, equipment, timeout=5, poll=150):
-    # type: (int, AnyStr, int, int) -> Any
     """Attempts to retrieve a response message from the Gateway.
 
     The transaction id from the sent message is used to retrieve the
     response.
 
     Args:
-        transactionID: The transactionID of the request and response.
-            The transactionID is used to retrieve the response.
-            Typically used in conjunction with
+        transactionID (int): The transactionID of the request and
+            response. The transactionID is used to retrieve the
+            response. Typically used in conjunction with
             system.secsgem.sendRequest to generate a transactionID.
-        equipment: Name of equipment connection.
-        timeout: Specifies in seconds how long to wait for a response
-            before returning None. If omitted the timeout will be 5
-            seconds. Optional.
-        poll: Specifies in milliseconds how often to poll the system for
-            a response. If omitted the poll will be 150 milliseconds.
-            Optional.
+        equipment (str): Name of equipment connection.
+        timeout (int): Specifies in seconds how long to wait for a
+            response before returning None. If omitted the timeout will
+            be 5 seconds. Optional.
+        poll (int): Specifies in milliseconds how often to poll the
+            system for a response. If omitted the poll will be 150
+            milliseconds. Optional.
 
     Returns:
-        A Python object, typically a dictionary. The actual result is a
-        JSON string that's decoded into a python object, as shown on the
-        mapping on the system.util.jsonDecode page.
+        object: A Python object, typically a dictionary. The actual
+            result is a JSON string that's decoded into a python object,
+            as shown on the mapping on the system.util.jsonDecode page.
     """
     print(transactionID, equipment, timeout, poll)
-    return ""
 
 
 def getToolProgram(ppid):
-    # type: (AnyStr) -> Dict[AnyStr, Any]
     """Returns a process program from the Gateway that was previously
     sent by a a tool in an S7F3 message.
 
     Args:
-        ppid: The PPID that was sent from the tool when the S7F3 message
-            was saved.
+        ppid (str): The PPID that was sent from the tool when the S7F3
+            message was saved.
 
     Returns:
-        A Python Dictionary containing the following keys: editDate,
-        ppbody, bodyFormat.
+        dict: A Python Dictionary containing the following keys:
+            [editDate, ppbody, bodyFormat].
     """
     print(ppid)
     return {
-        "editDate": Date(),
+        "editDate": system.date.now(),
         "ppBody": "program",
         "bodyFormat": "A",
     }
 
 
 def getToolProgramDataset():
-    # type: () -> BasicDataset
     """Returns a Dataset containing information about all stored process
     programs.
 
     Returns:
-         A Dataset containing information about all stored process
-         programs. Includes the following columns in order: ppid,
-         editDate, bodyFormat.
+         Dataset: A Dataset containing information about all stored
+            process programs. Includes the following columns in order:
+            ppid, editDate, bodyFormat.
     """
-    return BasicDataset()
+    return Dataset()
 
 
 def sendRequest(streamFunction, reply, body, equipment):
-    # type: (AnyStr, bool, Any, AnyStr) -> int
     """Sends a JSON-formatted SECS message to a tool.
 
     An equipment connection must be configured for the tool in the
     Gateway.
 
     Args:
-        streamFunction: The stream and function of the SECS message to
-            send. Example: "S1F13"
-        reply: Whether or not the SECS message expects a reply message.
-        body: This contains the body of a SECS message. The argument can
-            be a Python Object or JSON string representing the body of a
-            SECS message. If this argument is a string then it will be
-            converted to a Python Object using the
+        streamFunction (str): The stream and function of the SECS
+            message to send. Example: "S1F13"
+        reply (bool): Whether or not the SECS message expects a reply
+            message.
+        body (object): This contains the body of a SECS message. The
+            argument can be a Python Object or JSON string representing
+            the body of a SECS message. If this argument is a string
+            then it will be converted to a Python Object using the
             system.util.jsonDecode function.
-        equipment: Name of the equipment connection to use.
+        equipment (str): Name of the equipment connection to use.
 
     Returns:
-        The transactionID of the SECS message response.
+        int: The transactionID of the SECS message response.
     """
     print(streamFunction, reply, body, equipment)
     return 0
 
 
 def sendResponse(transactionID, systemBytes, streamFunction, body, equipment):
-    # type: (int, int, AnyStr, Any, AnyStr) -> None
     """Sends a JSON-formatted SECS response message to a message sent by
     a tool.
 
     An equipment connection must be configured for the tool in the
     Gateway, and this must be used within a Message Handler to create a
     Custom Message Response Handler.
 
     Args:
-        transactionID: The TxID of the response. The TxID from the
+        transactionID (int): The TxID of the response. The TxID from the
             received request in the payload of the message handler must
             be specified here.
-        systemBytes: The SystemBytes of the response. The SystemBytes
-            from the received request in the payload of the message
-            handler must be specified here.
-        streamFunction: The stream and function of the SECS message to
-            send. Example: "S1F14".
-        body: This contains the body of a SECS response. The argument
-            can be a Python Object or JSON string representing the body
-            of a SECS message. If this argument is a string then it will
-            be converted to a Python Object using the
+        systemBytes (int): The SystemBytes of the response. The
+            SystemBytes from the received request in the payload of the
+            message handler must be specified here.
+        streamFunction (str): The stream and function of the SECS
+            message to send. Example: "S1F14".
+        body (object): This contains the body of a SECS response. The
+            argument can be a Python Object or JSON string representing
+            the body of a SECS message. If this argument is a string
+            then it will be converted to a Python Object using the
             system.util.jsonDecode function.
-        equipment: Name of the equipment connection to use.
+        equipment (str): Name of the equipment connection to use.
     """
     print(transactionID, systemBytes, streamFunction, body, equipment)
 
 
 def startSimEventRun(simulatorName, eventRunName):
-    # type: (AnyStr, AnyStr) -> None
     """Starts a configured simulator event run in the Gateway.
 
     Note, that this function only works with the simulators that come
     included with the SECS/GEM module.
 
     The function will throw an exception if the specified Event Run
     cannot be started.
 
     Args:
-        simulatorName: The simulator that holds the configured event
-            run. Will throw an exception if the specified simulator
-            can't be found.
-        eventRunName: The event run to start. Will throw an exception if
-            the specified simulator can't be found.
+        simulatorName (str): The simulator that holds the configured
+            event run. Will throw an exception if the specified
+            simulator can't be found.
+        eventRunName (str): The event run to start. Will throw an
+            exception if the specified simulator can't be found.
     """
     print(simulatorName, eventRunName)
 
 
 def toDataSet(secsObject):
-    # type: (Any) -> BasicDataset
     """Converts a SECS message data structure, as returned by the
     system.secsgem.getResponse function, into a dataset and returns it.
 
     Args:
-        secsObject: A Python object, such as Sequence or a Dictionary,
-            representing a SECS message to convert to a dataset.
+        secsObject (object): A Python object, such as Sequence or a
+            Dictionary, representing a SECS message to convert to a
+            dataset.
 
     Returns:
-         A Dataset representing a SECS message.
+         Dataset: A Dataset representing a SECS message.
     """
     print(secsObject)
-    return BasicDataset()
+    return Dataset()
 
 
 def toTreeDataSet(dataset):
-    # type: (BasicDataset) -> BasicDataset
     """Changes an existing dataset, as returned by the
     system.secsgem.toDataSet function, to make it usable for the Tree
     View component.
 
     Args:
-        dataset: A dataset containing a SECS message. Note that this
-            parameter cannot take a JSON message, so the object returned
-            by system.secsgem.getResponse must first be processed by
-            system.secsgem.toDataSet.
+        dataset (Dataset): A DataSet containing a SECS message. Note
+            that this parameter cannot take a JSON message, so the
+            object returned by system.secsgem.getResponse must first be
+            processed by system.secsgem.toDataSet.
 
     Returns:
-        A dataset containing a SECS message with the following columns,
-        as suited for Vision's tree view component: "path", "text",
-        "icon", "background", "foreground", "tooltip", "border",
-        "selectedText", "selectedIcon", "selectedBackground",
-        "selectedForeground", "selectedTooltip", "selectedBorder".
+        Dataset: A Dataset containing a SECS message that can be used in
+            the Tree View component.
     """
     print(dataset)
-    return BasicDataset()
+    return Dataset()
```

### Comparing `ignition_api-8.1.40/src/system/device.py` & `ignition-api-8.1.9/src/system/device.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,113 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Device Functions.
 
 The following functions give you access to view and edit device
 connections in the Gateway.
 """
 
 from __future__ import print_function
 
 __all__ = [
     "addDevice",
     "getDeviceHostname",
     "listDevices",
     "refreshBrowse",
     "removeDevice",
-    "restart",
     "setDeviceEnabled",
     "setDeviceHostname",
 ]
 
-from typing import Any, Dict, Optional
-
-from com.inductiveautomation.ignition.common import BasicDataset
-from dev.coatl.helper.types import AnyStr
+from system.dataset import Dataset
 
 
-def addDevice(
-    deviceType,  # type: AnyStr
-    deviceName,  # type: AnyStr
-    deviceProps,  # type: Dict[AnyStr, Any]
-    description=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> None
+def addDevice(deviceType, deviceName, deviceProps):
     """Adds a new device connection in Ignition.
 
     Accepts a dictionary of parameters to configure the connection.
     Acceptable parameters differ by device type: i.e., a Modbus/TCP
     connection requires a hostname and port, but a simulator doesn't
-    require any parameters. When using this function, the arguments must
-    be passed in as keyword arguments.
+    require any parameters.
 
     Args:
-        deviceType: The device driver type.
-        deviceName: The name that will be given to the new device
-            connection.
-        deviceProps: A dictionary of device connection properties and
-            values. Each deviceType has different properties, but most
-            require at least a hostname. Keys in the dictionary are
+        deviceType (str): The device driver type. Possible values are
+            listed in the Device Types table below.
+        deviceName (str): The name that will be given to the the new
+            device connection.
+        deviceProps (dict): A dictionary of device connection properties
+            and values. Each deviceType has different properties, but
+            most require at least a hostname. Keys in the dictionary are
             case-insensitive, spaces are omitted, and the names of the
             properties that appear when manually creating a device
             connection.
-        description: The description that will be given to the new
-            device connection. Optional.
     """
-    print(deviceType, deviceName, deviceProps, description)
+    print(deviceType, deviceName, deviceProps)
 
 
 def getDeviceHostname(deviceName):
-    # type: (AnyStr) -> AnyStr
     """Gets the hostname of a device.
 
     Args:
-        deviceName: The name of the device in Ignition.
+        deviceName (str): The name of the device in Ignition.
 
     Returns:
-        The hostname of the device. Null if device doesn't have a
-        hostname.
+        str: The hostname of the device. Null if device doesn't have a
+            hostname.
     """
     print(deviceName)
-    return ""
 
 
 def listDevices():
-    # type: () -> BasicDataset
     """Returns a dataset of information about each configured device.
 
     Each row represents a single device.
 
     Returns:
-        A dataset, where each row represents a device. Contains 4
-        columns Name, Enabled, State, and Driver.
+        Dataset: A dataset, where each row represents a device. Contains
+            4 columns Name, Enabled, State, and Driver.
     """
-    return BasicDataset()
+    return Dataset()
 
 
 def refreshBrowse(deviceName):
-    # type: (AnyStr) -> None
     """Forces Ignition to browse the controller.
 
     Only works for Allen-Bradley controllers.
 
     Args:
-        deviceName: The name of the device in Ignition.
+        deviceName (str): The name of the device in Ignition.
     """
     print(deviceName)
 
 
 def removeDevice(deviceName):
-    # type: (AnyStr) -> None
     """Removes a given device from Ignition.
 
     Args:
-        deviceName: The name of the device in Ignition.
-    """
-    print(deviceName)
-
-
-def restart(deviceName):
-    # type: (AnyStr) -> None
-    """Restarts the named device connection.
-
-    Args:
-        deviceName: The name of the device connection to restart. The
-            function will throw an error if the specified deviceName
-            does not exist on the host gateway.
+        deviceName (str): The name of the device in Ignition.
     """
     print(deviceName)
 
 
 def setDeviceEnabled(deviceName, enabled):
-    # type: (AnyStr, bool) -> None
     """Enables/disables a device in Ignition.
 
     Args:
-        deviceName: The name of the device in Ignition.
-        enabled: Specifies whether the device connection will be set to
-            enabled or disabled state.
+        deviceName (str): The name of the device in Ignition.
+        enabled (bool): The enabled status of the device.
     """
     print(deviceName, enabled)
 
 
 def setDeviceHostname(deviceName, hostname):
-    # type: (AnyStr, AnyStr) -> None
     """Changes the hostname of a device.
 
-    Used for all Ethernet based drivers.
+    Used for all ethernet based drivers.
 
     Args:
-        deviceName: The name of the device in Ignition.
-        hostname: The new IP address or hostname.
+        deviceName (str): The name of the device in Ignition.
+        hostname (str): The new IP address or hostname.
     """
     print(deviceName, hostname)
```

### Comparing `ignition_api-8.1.40/src/system/twilio.py` & `ignition-api-8.1.9/src/system/twilio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Twilio Functions.
 
 The following functions give you access to read info and send SMS
 through Twilio. This requires the Twilio Module, which is not included
 in a typical install.
 """
 
@@ -11,85 +15,80 @@
     "getAccounts",
     "getAccountsDataset",
     "getPhoneNumbers",
     "getPhoneNumbersDataset",
     "sendSms",
 ]
 
-from typing import List
-
-from com.inductiveautomation.ignition.common import BasicDataset
-from dev.coatl.helper.types import AnyStr
+from system.dataset import Dataset
 
 
 def getAccounts():
-    # type: () -> List[AnyStr]
     """Return a list of Twilio accounts that have been configured in the
     Gateway.
 
     Returns:
-        A list of configured Twilio accounts.
+        list[str]: A list of configured Twilio accounts.
     """
     return ["twilio_account1", "twilio_account2"]
 
 
 def getAccountsDataset():
-    # type: () -> BasicDataset
     """Return a list of Twilio accounts that have been configured in the
     Gateway as a single-column Dataset.
 
     Returns:
-        A list of configured Twilio accounts as a single-column Dataset.
+        Dataset: A list of configured Twilio accounts as a single-column
+            Dataset.
     """
-    return BasicDataset()
+    return Dataset()
 
 
 def getPhoneNumbers(accountName):
-    # type: (AnyStr) -> List[AnyStr]
     """Returns a list of outgoing phone numbers for a Twilio account.
 
     Note that these numbers are supplied by Twilio, and are not defined
     on a user in Ignition.
 
     Args:
-        accountName: The Twilio account to retrieve phone numbers for.
+        accountName (str): The Twilio account to retrieve phone numbers
+            for.
 
     Returns:
-        A list of phone numbers for the given Twilio account.
+        list[str]: A list of phone numbers for the given Twilio account.
     """
-    phoneNumbers = []  # type: List[AnyStr]
+    phoneNumbers = []
     if accountName == "Jenny":
         phoneNumbers.append("+12058675309")
     return phoneNumbers
 
 
 def getPhoneNumbersDataset(accountName):
-    # type: (AnyStr) -> BasicDataset
     """Return a list of outgoing phone numbers for a Twilio account as a
     single-column Dataset.
 
     Note that these numbers are supplied by Twilio, and are not defined
     on a user in Ignition.
 
     Args:
-        accountName: The Twilio account to retrieve phone numbers for.
+        accountName (str): The Twilio account to retrieve phone numbers
+            for.
 
     Returns:
-        A list of phone numbers for the given Twilio account as a
-        single-column Dataset.
+        Dataset: A list of phone numbers for the given Twilio account as
+            a single-column Dataset.
     """
     print(accountName)
-    return BasicDataset()
+    return Dataset()
 
 
 def sendSms(accountName, fromNumber, toNumber, message):
-    # type: (AnyStr, AnyStr, AnyStr, AnyStr) -> None
     """Sends an SMS message.
 
     Args:
-        accountName: The Twilio account to send the SMS from.
-        fromNumber: The outbound phone number belonging to the Twilio
-            account to use.
-        toNumber: The phone number of the recipient.
-        message: The body of the SMS.
+        accountName (str): The Twilio account to send the SMS from.
+        fromNumber (str): The outbound phone number belonging to the
+            Twilio account to use.
+        toNumber (str): The phone number of the recipient.
+        message (str): The body of the SMS.
     """
     print(accountName, fromNumber, toNumber, message)
```

### Comparing `ignition_api-8.1.40/src/system/alarm.py` & `ignition-api-8.1.9/src/system/alarm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Alarm Functions.
 
 The following functions give you access to view and interact with the
 Alarm system in Ignition.
 """
 
 from __future__ import print_function
@@ -15,333 +19,374 @@
     "listPipelines",
     "queryJournal",
     "queryStatus",
     "shelve",
     "unshelve",
 ]
 
-from typing import Any, Dict, List, Optional, Tuple, Union
+from abc import ABCMeta, abstractmethod
 
-from com.inductiveautomation.ignition.common.alarming.evaluation import ShelvedPath
-from com.inductiveautomation.ignition.common.alarming.query import AlarmQueryResultImpl
-from dev.coatl.helper.types import AnyStr
+import system.date
+from java.lang import Object
 from java.util import Date
 
 
-def acknowledge(alarmIds, notes, username=None):
-    # type: (List[AnyStr], AnyStr, Optional[AnyStr]) -> List[AnyStr]
+class AlarmQueryResults(ABCMeta):
+    """This is the result of a query against the alarming system, for
+    both status and history.
+
+    It provides the results as a list, but also provides additional
+    helper functions for getting the event and associated data as a
+    dataset.
+    """
+
+    def __new__(mcs, *args, **kwargs):
+        pass
+
+    @abstractmethod
+    def getAssociatedDate(cls, uuid):
+        pass
+
+    @abstractmethod
+    def getDataSet(cls):
+        pass
+
+    @abstractmethod
+    def getEvent(cls, uuid):
+        pass
+
+
+class ShelvedPath(Object):
+    """This class provides information about a path that has been
+    "shelved", such as when it was shelved, and by whom, and the actual
+    path.
+    """
+
+    def __init__(self, path=None, user=None, expiration=None):
+        self.path = path
+        self.user = user
+        self.expiration = expiration
+
+    def getExpiration(self):
+        pass
+
+    def getHitCount(self):
+        pass
+
+    def getPath(self):
+        pass
+
+    def getShelveTime(self):
+        pass
+
+    def getUser(self):
+        pass
+
+    def incrementHitCount(self):
+        pass
+
+    def isExpired(self):
+        pass
+
+
+def acknowledge(alarmIds, notes=None, username=None):
     """Acknowledges any number of alarms, specified by their event ids.
 
     The event id is generated for an alarm when it becomes active, and
     is used to identify a particular event from other events for the
     same source. The alarms will be acknowledged by the logged in user
     making the call. Additionally, acknowledgement notes may be included
     and will be stored along with the acknowledgement.
 
-    Note:
-         The `username` parameter is only used when called from a
-         gateway scoped script. This parameter should be omitted from
-         any client-based scripts.
-
     Args:
-        alarmIds: List of alarm event ids (UUIDs) to acknowledge.
-        notes: A string that will be used as the Ack Note on each
-            acknowledged alarm event. If set to None, then an Ack Note
-            note will not be assigned to the alarm event.
-        username: The user that acknowledged the alarm.
-
-    Returns:
-        List of alarm event ids (UUIDs) that were unable to be
-        acknowledged successfully.
+        alarmIds (list[str]): List of alarm event ids (uuids) to
+            acknowledge.
+        notes (str): Notes that will be stored on the acknowledged alarm
+            events. Optional.
+        username (str): The user that acknowledged the alarm. NOTE that
+            this parameter is only used when called from a gateway
+            scoped script. This parameter should be omitted from any
+            client-based scripts. Optional.
     """
     print(alarmIds, notes, username)
-    return alarmIds
 
 
 def cancel(alarmIds):
-    # type: (List[AnyStr]) -> None
     """Cancels any number of alarms, specified by their event ids.
 
-    Event ids can be obtained from the system.alarm.queryStatus
-    function. Canceling a pipeline will not impact the alarm that
-    triggered the pipeline. The alarm will still be active, but will
-    drop out of alarm pipelines.
+    The event id is generated for an alarm when it becomes active, and
+    is used to identify a particular event from other events for the
+    same source. The alarm will still be active, but will drop out of
+    alarm pipelines.
 
     Args:
-        alarmIds: List of alarm event ids (UUIDs) to cancel.
+        alarmIds (list[str]): List of alarm event ids (uuids) to cancel.
     """
     print(alarmIds)
 
 
-def createRoster(name, description):
-    # type: (AnyStr, AnyStr) -> None
+def createRoster(name, description=""):
     """This function creates a new roster.
 
     Users may be added to the roster through the Gateway or the Roster
     Management component.
 
     Args:
-        name: The name for the new roster.
-        description: A description for the new roster. Required, but can
-            be blank.
+        name (str): The name for the new roster.
+        description (str): A description for the new roster. Required,
+            but can be blank. Optional.
     """
     print(name, description)
 
 
 def getRosters():
-    # type: () -> Dict[AnyStr, List[AnyStr]]
     """This function returns a mapping of roster names to a list of
     usernames contained in the roster.
 
     Returns:
-        A dictionary that maps roster names to a List of usernames in
-        the roster. The list of usernames may be empty if no users have
-        been added to the roster.
+         dict: A dictionary that maps roster names to a List of
+            usernames in the roster. The List of usernames may be empty
+            if no users have been added to the roster.
     """
     return {}
 
 
 def getShelvedPaths():
-    # type: () -> List[ShelvedPath]
-    """Returns a list of ShelvedPath objects, which each represent a
-    shelved alarm.
+    """A list of ShelvedPath objects.
+
+    ShelvedPath objects can be examined with getExpiration, getHitCount,
+    getPath, getShelveTime, getUser, and isExpired.
 
     Returns:
-        A list of ShelvedPath objects.
+        list[ShelvedPath]: A list of ShelvedPath objects. ShelvedPath
+            objects can be examined with getExpiration, getHitCount,
+            getPath, getShelveTime, getUser, and isExpired.
     """
     return [ShelvedPath()]
 
 
 def listPipelines(projectName="alarm-pipelines"):
-    # type: (AnyStr) -> List[AnyStr]
     """Will return a list of the available Alarm Notification Pipelines.
 
     Args:
-        projectName: The project to check alarm pipelines for. If
+        projectName (str): The project to check alarm pipelines for. If
             omitted, will look for a project named "alarm-pipelines".
             Optional.
 
     Returns:
-        A list of pipeline names. The list may be empty if no pipelines
-        exist. Unsaved name changes will not be reflected in the list.
+        list[str]: A list of pipeline names. The list may be empty if no
+            pipelines exist. Unsaved name changes will not be reflected
+            in the list.
     """
     print(projectName)
     return []
 
 
 def queryJournal(
-    startDate=None,  # type: Optional[Date]
-    endDate=None,  # type: Optional[Date]
-    journalName=None,  # type: Optional[AnyStr]
-    priority=None,  # type: Optional[List[Union[AnyStr, int]]]
-    state=None,  # type: Optional[List[Union[AnyStr, int]]]
-    path=None,  # type: Optional[List[AnyStr]]
-    source=None,  # type: Optional[List[AnyStr]]
-    displaypath=None,  # type: Optional[List[AnyStr]]
-    all_properties=None,  # type: Optional[List[Tuple[AnyStr, AnyStr, Any]]]
-    any_properties=None,  # type: Optional[List[Tuple[AnyStr, AnyStr, Any]]]
-    defined=None,  # type: Optional[List[AnyStr]]
-    includeData=None,  # type: Optional[bool]
-    includeSystem=None,  # type: Optional[bool]
-    includeShelved=None,  # type: Optional[bool]
-    isSystem=None,  # type: Optional[bool]
-    provider=None,  # type: Optional[List[AnyStr]]
+    startDate=None,
+    endDate=None,
+    journalName=None,
+    priority=None,
+    state=None,
+    path=None,
+    source=None,
+    displaypath=None,
+    all_properties=None,
+    any_properties=None,
+    defined=None,
+    includeData=None,
+    includeSystem=None,
+    isSystem=None,
 ):
-    # type: (...) -> AlarmQueryResultImpl
     """Queries the specified journal for historical alarm events.
 
     The result is a list of alarm events, which can be queried for
-    individual properties.
-
-    Note:
-        Each item in the resulting object is a separate alarm event: an
-        alarm becoming active is one item, while the same alarm becoming
-        acknowledged is a separate item. This differs from
-        `system.alarm.queryStatus()` which groups each event into a
-        single item.
+    individual properties. The result object also has a getDataset()
+    function that can be used to convert the query results into a normal
+    dataset, with the columns: EventId, Source, DisplayPath, EventTime,
+    EventState, Priority, IsSystemEvent.
 
     Args:
-        startDate: The start of the time range to query. Defaults to 8
-            hours previous to now if omitted. Time range is inclusive.
-            Optional.
-        endDate: The end of the time range to query. Defaults to "now"
-            if omitted. Optional.
-        journalName: The journal name to query. If only one journal
-            exists on the Gateway, can be omitted. Optional.
-        priority: A list of possible priorities to match. Priorities can
-            be specified by name or number, with the values:
-            Diagnostic(0), Low(1), Medium(2), High(3), Critical(4).
-            Optional.
-        state: A list of the event state types to match. Valid values
-            can either be integers or strings, representing a number of
-            states. Optional.
-        path: A list of possible source paths to search at. The wildcard
-            "*" may be used. Optional.
-        source: A list of possible source paths to search at. The
-            wildcard "*" may be used. Optional.
-        displaypath: A list of display paths to search at. Display paths
-            are separated by "/", and if a path ends in "/*", everything
-            below that path will be searched as well.
-        all_properties: A set of property conditions, all of which must
-            be met for the condition to pass. This parameter is a list
-            of tuples, in the form ("propName", "condition", value).
-            Valid condition values: "=", "!=", "<", "<=", ">", ">=".
-            String values can only be compared using "=" and "!="
-            conditions. Optional.
-        any_properties: A set of property conditions, any of which will
-            cause the overall condition to pass. This parameter is a
-            list of tuples, in the form ("propName", "condition",
-            value). Valid condition values: "=", "!=", "<", "<=", ">",
-            ">=". String values can only be compared using "=" and "!="
-            conditions. Optional.
-        defined: A list of string property names, all of which must be
-            present on an event for it to pass. Optional.
-        includeData: Whether or not event data should be included in the
-            return. If True, returns Python dictionaries (or nulls) for
-            Active Data, Clear Data, Ack Data, Runtime Data inside of
-            the AlarmQueryResult object. Optional.
-        includeSystem: Specifies whether system events are included in
-            the return. Optional.
-        includeShelved: A flag indicating whether shelved events should
-            be included in the results. Defaults to false. Optional.
-        isSystem: Specifies whether the returned event must or must not
-            be a system event. Optional.
-        provider: A list of tag providers to include in the query.
-            Omitting this parameter will query all providers. Optional.
+        startDate (Date): The start of the time range to query.
+            Defaults to 8 hours previous to now if omitted. Time range
+            is inclusive.
+        endDate (Date): The end of the time range to query. Defaults
+            to "now" if omitted.
+        journalName (str): The journal name to query.
+        priority (list[str]): A list of possible priorities to match.
+            Priorities can be specified by name or number, with the
+            values: Diagnostic(0), Low(1), Medium(2), High(3),
+            Critical(4).
+        state (list[str]): A list of the event state types to match.
+            Valid values are "ClearUnacked", "ClearAcked",
+            "ActiveUnacked", and "ActiveAcked".
+        path (list[str]): A list of possible source paths to search at.
+            The wildcard "*" may be used.
+        source (list[str]): A list of possible source paths to search
+            at. The wildcard "*" may be used.
+        displaypath (list[str]): A list of display paths to search at.
+            Display paths are separated by "/", and if a path ends in
+            "/*", everything below that path will be searched as well.
+        all_properties (list[object]): A set of property conditions, all
+            of which must be met for the condition to pass. This
+            parameter is a list of tuples, in the form ("propName",
+            "condition", value). Valid condition values: "=", "!=", "<",
+            "<=", ">", ">=". Only the first two conditions may be used
+            for string values.
+        any_properties (list[object]): A set of property conditions, any
+            of which will cause the overall the condition to pass. This
+            parameter is a list of tuples, in the form ("propName",
+            "condition", value). Valid condition values: "=", "!=", "<",
+            "<=", ">", ">=". Only the first two conditions may be used
+            for string values.
+        defined (list[str]): A list of string property names, all of
+            which must be present on an event for it to pass.
+        includeData (bool): Whether or not event data should be included
+            in the return. If this parameter is False, and if there are
+            no conditions specified on associated data, the properties
+            table will not be queried.
+        includeSystem (bool): Specifies whether system events are
+            included in the return.
+        isSystem (bool): Specifies whether the returned event must or
+            must not be a system event.
 
     Returns:
-        The AlarmQueryResult object is functionally a list of AlarmEvent
-        objects.
+        AlarmQueryResults: The AlarmQueryResults object is functionally
+            a list of AlarmEvent objects. The AlarmQueryResults object
+            has a built-in getDataset() function that will return a
+            Standard Dataset containing the Event Id (UUID of the
+            alarm), Source Path, Display Path, Event Time, State (as an
+            integer), and Priority (as an integer).
     """
+    endDate = system.date.now() if endDate is None else endDate
+    startDate = (
+        system.date.addHours(endDate, -8) if startDate is None else startDate
+    )
     print(
         startDate,
         endDate,
         journalName,
         priority,
         state,
         path,
         source,
         displaypath,
         all_properties,
         any_properties,
         defined,
         includeData,
         includeSystem,
-        includeShelved,
         isSystem,
-        provider,
     )
-    return AlarmQueryResultImpl()
+    return AlarmQueryResults()
 
 
 def queryStatus(
-    priority=None,  # type: Optional[List[Union[AnyStr, int]]]
-    state=None,  # type: Optional[List[Union[AnyStr, int]]]
-    path=None,  # type: Optional[List[AnyStr]]
-    source=None,  # type: Optional[List[AnyStr]]
-    displaypath=None,  # type: Optional[List[AnyStr]]
-    all_properties=None,  # type: Optional[List[Tuple[AnyStr, AnyStr, Any]]]
-    any_properties=None,  # type: Optional[List[Tuple[AnyStr, AnyStr, Any]]]
-    defined=None,  # type: Optional[List[AnyStr]]
-    includeShelved=False,  # type: bool
+    priority=None,
+    state=None,
+    path=None,
+    source=None,
+    displaypath=None,
+    all_properties=None,
+    any_properties=None,
+    defined=None,
+    includeShelved=False,
 ):
-    # type: (...) -> AlarmQueryResultImpl
     """Queries the current state of alarms.
 
     The result is a list of alarm events, which can be queried for
-    individual properties. The results provided by this function
-    represent the current state of alarms, in contrast to the historical
-    alarm events retrieved by the `system.alarm.queryJournal` function.
-
-    Note:
-        Depending on the number of alarm events in the system, this
-        function can be fairly intensive and take a while to finish
-        executing. This can be problematic if the application is
-        attempting to show the results on a component (such as using
-        this function to retrieve a count of alarms). In these cases
-        it's preferred to call this function in a gateway script of some
-        sort (such as a timer script), and store the results in a tag.
+    individual properties. The result object also has a getDataset()
+    function that can be used to convert the query results into a normal
+    dataset, with the columns: EventId, Source, DisplayPath, EventTime,
+    State, Priority.
 
     Args:
-        priority: A list of possible priorities to match. Priorities can
-            be specified by name or number, with the values:
-            Diagnostic(0), Low(1), Medium(2), High(3), Critical(4).
-            Optional.
-        state: A list of states to allow. Optional.
-        path: A list of possible source paths to search at. The
-            wildcard "*" may be used. Works the same as the source
+        priority (list[str]): A list of possible priorities to match.
+            Priorities can be specified by name or number, with the
+            values: Diagnostic(0), Low(1), Medium(2), High(3),
+            Critical(4). Optional.
+        state (list[str]): A list of states to allow. Valid values:
+            "ClearUnacked", "ClearAcked", "ActiveUnacked",
+            "ActiveAcked". Optional.
+        path (list[str]): A list of possible source paths to search at.
+            The wildcard "*" may be used. Works the same as the source
             argument, and either can be used. Optional.
-        source: A list of possible source paths to search at. The
-            wildcard "*" may be used. Works the same as the path
+        source (list[str]): A list of possible source paths to search
+            at. The wildcard "*" may be used. Works the same as the path
             argument, and either can be used. Optional.
-        displaypath: A list of display paths to search at. Display paths
-            are separated by "/", and if a path ends in "/*", everything
-            below that path will be searched as well. Optional.
-        all_properties: A set of property conditions, all of which must
-            be met for the condition to pass. This parameter is a list
-            of tuples, in the form ("propName", "condition", value).
-            Valid condition values: "=", "!=", "<", "<=", ">", ">=".
-            String values can only be compared using "=" and "!="
-            conditions. Optional.
-        any_properties: A set of property conditions, any of which will
-            cause the overall the condition to pass. This parameter is a
-            list of tuples, in the form ("propName", "condition",
-            value). Valid condition values: "=", "!=", "<", "<=", ">",
-            ">=". String values can only be compared using "=" and "!="
-            conditions. Optional.
-        defined: A list of string property names, all of which must be
-            present on an event for it to pass. Optional.
-        includeShelved: A flag indicating whether shelved events should
-            be included in the results. Defaults to False. Optional.
+        displaypath (list[str]): A list of display paths to search at.
+            Display paths are separated by "/", and if a path ends in
+            "/*", everything below that path will be searched as well.
+            Optional.
+        all_properties (list[object]): A set of property conditions, all
+            of which must be met for the condition to pass. This
+            parameter is a list of tuples, in the form ("propName",
+            "condition", value). Valid condition values: "=", "!=", "<",
+            "<=", ">", ">=". Only the first two conditions may be used
+            for string values. Optional.
+        any_properties (list[object]): A set of property conditions, any
+            of which will cause the overall the condition to pass. This
+            parameter is a list of tuples, in the form ("propName",
+            "condition", value). Valid condition values: "=", "!=", "<",
+            "<=", ">", ">=". Only the first two conditions may be used
+            for string values. Optional.
+        defined (list[str]): A list of string property names, all of
+            which must be present on an event for it to pass. Optional.
+        includeShelved (bool): A flag indicating whether shelved events
+            should be included in the results. Defaults to "False".
+            Optional.
 
     Returns:
-        The AlarmQueryResult object is functionally a list of AlarmEvent
-        objects with some additional helper methods.
+        AlarmQueryResults: The AlarmQueryResults object is functionally
+            a list of AlarmEvent objects. The AlarmQueryResults object
+            has a built-in getDataset() function that will return a
+            Standard Dataset containing the Event Id (UUID of the
+            alarm), Source Path, Display Path, Event Time, State (as an
+            integer), and Priority (as an integer).
     """
     print(
         priority,
         state,
         path,
         source,
         displaypath,
         all_properties,
         any_properties,
         defined,
         includeShelved,
     )
-    return AlarmQueryResultImpl()
+    return AlarmQueryResults()
 
 
-def shelve(path, timeoutSeconds=0, timeoutMinutes=15):
-    # type: (List[AnyStr], int, int) -> None
+def shelve(path, timeoutSeconds=None, timeoutMinutes=None):
     """This function shelves the specified alarms for the specified
     amount of time.
 
-    The time can be specified in minutes (timeoutMinutes) or seconds
+    The paths may be either source paths, or display paths. The time can
+    be specified in minutes (timeoutMinutes) or seconds
     (timeoutSeconds). If an alarm is already shelved, this will
-    overwrite the remaining time. If no timeout is specified, will
-    default to 15 minutes.
+    overwrite the remaining time. To unshelve alarms, this function may
+    be used with a time of "0".
 
     Args:
-        path: A list of possible source paths to search at. If a path
-            ends in "/*", the results will include anything below that
-            path.
-        timeoutSeconds: The amount of time to shelve the matching alarms
-            for, specified in seconds. Setting this to 0 will unshelve
-            the alarms. Optional.
-        timeoutMinutes: The amount of time to shelve the matching alarms
-            for, specified in minutes. Setting this to 0 will unshelve
-            the alarms. Optional.
+        path (list[str]): A list of possible source paths to search at.
+            If a path ends in "/*", the results will include anything
+            below that path.
+        timeoutSeconds (int): The amount of time to shelve the matching
+            alarms for, specified in seconds. 0 indicates that matching
+            alarm events should now be allowed to pass. Optional.
+        timeoutMinutes (int): The amount of time to shelve the matching
+            alarms for, specified in minutes. 0 indicates that matching
+            alarm events should now be allowed to pass. Optional.
     """
     print(path, timeoutSeconds, timeoutMinutes)
 
 
 def unshelve(path):
-    # type: (List[AnyStr]) -> None
-    """Unshelves a list of alarms based on the source paths provided.
+    """Unshelves alarms in accordance with the path parameter.
 
     Args:
-        path: A list of possible source paths to search at. If a path
-            ends in "/*", the results will include anything below that
-            path.
+        path (list[str]): A list of possible source paths to search at.
+            If a path ends in "/*", the results will include anything
+            below that path.
     """
     print(path)
```

### Comparing `ignition_api-8.1.40/src/system/perspective/workstation.py` & `ignition-api-8.1.9/src/system/perspective/workstation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Perspective Workstation Functions.
 
 The following functions offer various ways to interact with Perspective
 Workstation from a Python script. Note that the functions here only work
 when called from a session running in Perspective Workstation.
 """
 
 __all__ = ["exit", "toKiosk", "toWindowed"]
 
 
 def exit():
-    # type: () -> None
     """When called from a session running in Workstation, this function
     will close Workstation.
     """
     pass
 
 
 def toKiosk():
-    # type: () -> None
     """When called from a session running in Perspective Workstation,
     attempts to put Workstation into Kiosk mode.
     """
     pass
 
 
 def toWindowed():
-    # type: () -> None
     """When called from a Session running in Perspective Workstation,
     attempts to put Workstation into windowed mode.
     """
     pass
```

### Comparing `ignition_api-8.1.40/src/system/perspective/__init__.py` & `ignition-api-8.1.9/src/system/perspective/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Perspective Functions.
 
 The following functions offer various ways to interact with a
-Perspective Session from a Python script.
+Perspective session from a Python script.
 """
 
 from __future__ import print_function
 
 __all__ = [
-    "alterDock",
     "alterLogging",
-    "authenticationChallenge",
     "closeDock",
     "closePage",
     "closePopup",
     "closeSession",
     "download",
     "getProjectInfo",
     "getSessionInfo",
@@ -31,525 +33,489 @@
     "setTheme",
     "toggleDock",
     "togglePopup",
     "vibrateDevice",
 ]
 
 import __builtin__ as builtins
-from typing import Any, Dict, List, Optional, Union
 
-from com.inductiveautomation.ignition.common.gson import JsonObject
-from com.inductiveautomation.ignition.common.script.adapters import PyJsonObjectAdapter
-from dev.coatl.helper.types import AnyStr
+from java.lang import Object
 
 
-def alterDock(
-    dockId,  # type: AnyStr
-    config=None,  # type: Optional[Dict[AnyStr, Any]]
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-):
-    # type: (...) -> None
-    """Changes configuration of a specified dock on a Perspective Page.
+class PyJsonObjectAdapter(Object):
+    """Class PyJsonObjectAdapter."""
 
-    Args:
-        dockId: The ID of the dock to be altered. If no such dock exists
-            on the current page with the given ID, a warning will be
-            logged to the console.
-        config: The new configuration for the dock. All properties are
-            optional, and any properties not specified will remain
-            unchanged. Optional.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
-            current Page will be used automatically. Optional.
-    """
-    builtins.print(dockId, config, sessionId, pageId)
+    def __init__(self, obj):
+        builtins.print(self, obj)
+
+    def __delitem__(self, key):
+        pass
+
+    def __findattr_ex__(self, name):
+        pass
+
+    def __finditem__(self, key):
+        pass
+
+    def __iter__(self):
+        pass
+
+    def __len__(self):
+        pass
+
+    def __setitem__(self, key, value):
+        pass
+
+    def clear(self):
+        pass
+
+    def get(self, key, default=None):
+        pass
+
+    def has_key(self, key):
+        pass
+
+    def items(self):
+        pass
+
+    def iteritems(self):
+        pass
+
+    def iterkeys(self):
+        pass
+
+    def itervalues(self):
+        pass
+
+    def keys(self):
+        pass
+
+    def pop(self, key):
+        pass
+
+    def popitem(self):
+        pass
+
+    def setdefault(self, key, default):
+        pass
+
+    def update(self, *args, **kwargs):
+        pass
+
+    def values(self):
+        pass
 
 
 def alterLogging(
-    remoteLoggingEnabled=False,  # type: bool
-    level="info",  # type: AnyStr
-    remoteLoggingLevel="warn",  # type: AnyStr
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
+    remoteLoggingEnabled=False,
+    level="info",
+    remoteLoggingLevel="warn",
+    sessionId="current_session",
+    pageId="current_page",
 ):
-    # type: (...) -> None
     """Changes Perspective Session logging attributes and levels.
 
     All parameters are optional, with the caveat that at least one of
     them needs to be used.
 
     Args:
-        remoteLoggingEnabled: Will enable remote logging if True. Remote
-            logging will send log events from the Session to the Gateway
-            under the `perspective.client` logger if they meet the
+        remoteLoggingEnabled (bool): Will enable remote logging if True.
+            Remote logging will send log events from the Session to the
+            Gateway under the perspective.client logger if the meet the
             remoteLevel logging level requirement. Optional.
-        level: The desired Session logging level. Possible values are:
-            all, trace, debug, info, warn, error, fatal, off. The
+        level (str): The desired Session logging level. Possible values
+            are: all, trace, debug, info, warn, error, fatal, off. The
             default is info. Optional.
-        remoteLoggingLevel: The desired remote logging level. Possible
-            values are: all, trace, debug, info, warn, error, fatal,
-            off. The default is warn. Optional.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
-            current Page will be used automatically. Optional.
-    """
-    builtins.print(remoteLoggingEnabled, level, remoteLoggingLevel, sessionId, pageId)
-
-
-def authenticationChallenge(
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    idp="",  # type: AnyStr
-    forceAuth=False,  # type: bool
-    timeout=2,  # type: int
-    payload=None,  # type: Optional[Dict[AnyStr, Any]]
-    framing="self",  # type: AnyStr
-):
-    # type: (...) -> None
-    """Triggers an authentication challenge action.
-
-    Args:
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the page to target. If omitted, the
-            current page will be used. Optional.
-        idp: The name of the IdP to use for this authentication
-            challenge. If omitted, the Project default IdP will be used.
-            Optional.
-        forceAuth: True if Ignition should ask the IdP to
-            re-authenticate the user, even if the user is already signed
-            into the IdP. False if Ignition should not ask the IdP to
-            re-authenticate the user. If the IdP supports this option,
-            the IdP will ask the user to re-enter their credentials,
-            even if the user is already signed into the IdP. If omitted,
-            the default value for this argument will fall back to the
-            value in the Project Properties. Optional.
-        timeout: The number of minutes the system will wait in between
-            the authentication request and the authentication response
-            before timing out the request. If set to any number <= zero,
-            the request is rejected. If omitted, the default of two
-            minutes will be used as the timeout. Optional.
-        payload: An opaque payload object that may contain any
-            information. This object will be passed to the
-            onAuthenticationChallengeCompleted session event script. The
-            payload should be a JSON-encodable data structure.
-            Optional.
-        framing: A string representing the type of framing that should
-            be used. A value of "self" indicates that the same window
-            should be used. A value of "new" indicates that a new tab
-            should be used. A value of "embedded" indicates that an
-            embedded iframe should be used. If omitted, the default
-            value of "self" (same window) is used. Optional.
+        remoteLoggingLevel (str): The desired remote logging level.
+            Possible values are: all, trace, debug, info, warn, error,
+            fatal, off. The default is warn. Optional.
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
+            current Page will be used automatically. Optional.
     """
-    builtins.print(sessionId, pageId, idp, forceAuth, timeout, payload, framing)
+    builtins.print(
+        remoteLoggingEnabled, level, remoteLoggingLevel, sessionId, pageId
+    )
 
 
-def closeDock(id, sessionId="current_session", pageId="current_page"):
-    # type: (AnyStr, AnyStr, AnyStr) -> None
+def closeDock(id, sessionId=None, pageId=None):
     """Closes a docked view.
 
     Args:
-        id: The unique, preconfigured dock ID for the docked View. Is
-            specified when a View is assigned as docked for a particular
-            Page (in Page Configuration).
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        id (str): The unique, preconfigured 'Dock ID' for the docked
+            View. Is specified when a View is assigned as docked for a
+            particular Page (in Page Configuration).
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
     """
     builtins.print(id, sessionId, pageId)
 
 
 def closePage(
-    message=None,  # type: Optional[AnyStr]
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
+    message=None, sessionId="current_session", pageID="current_page"
 ):
-    # type: (...) -> None
     """Closes the page with the given page id or the current page if no
     page id is provided.
 
     If a message is provided, it is displayed on the page when the page
-    closes. Otherwise, the default message (set in the Project
+    closes. Otherwise the default message (set in the Project
     Properties) is displayed.
 
     Args:
-        message: The message to display when the page closes. If
+        message (str): The message to display when the page closes. If
             omitted, the default message (set in the Project Properties)
             is shown. Optional.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the page to be closed. If omitted, the
-            current pageId is used. Optional.
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageID (str): Identifier of the page to be closed. If omitted,
+            the current pageId is used. Optional.
     """
-    builtins.print(message, sessionId, pageId)
+    builtins.print(message, sessionId, pageID)
 
 
 def closePopup(id, sessionId="current_session", pageId="current_page"):
-    # type: (AnyStr, AnyStr, AnyStr) -> None
     """Closes a popup View.
 
     Args:
-        id: The unique identifier for the popup, given to the popup when
-            first opened. If given an empty string, then the most
-            recently focused popup will be closed.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        id (str): The unique identifier for the the popup, given to the
+            popup when first opened. If given an empty string, then the
+            most recently focused popup will be closed.
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
     """
     builtins.print(id, sessionId, pageId)
 
 
 def closeSession(message=None, sessionId="current_session"):
-    # type: (Optional[AnyStr], AnyStr) -> None
-    """Closes the Perspective Session with the given Session ID or the
-    current Session if no ID is provided.
+    """Closes the Perspective Session with the given session ID or the
+    current session if no ID is provided.
 
     If a message is provided, it is displayed on the page when the
-    Session closes. Otherwise, the default message (set in the Project
+    session closes. Otherwise the default message (set in the Project
     Properties) is displayed.
 
     Args:
-        message: The message to display when the Session closes. If
-            omitted, the default message (set in the Project Properties)
-            is shown. Optional.
-        sessionId: Identifier of the Session to be closed. If omitted,
-            the current sessionId is used. Optional.
+        message (str): The message to display when the session closes.
+            If omitted, the default message (set in the Project
+            Properties) is shown. Optional.
+        sessionId (str): Identifier of the session to be closed. If
+            omitted, the current sessionId is used. Optional.
     """
     builtins.print(message, sessionId)
 
 
 def download(
-    filename,  # type: AnyStr
-    data,  # type: Any
-    contentType=None,  # type: Optional[AnyStr]
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-):
-    # type: (...) -> None
-    """Downloads data from the gateway to a device running a Session.
+    filename,
+    data,
+    contentType=None,
+    sessionId="current_session",
+    pageId="current_page",
+):
+    """Downloads data from the gateway to a device running a session.
 
     Args:
-        filename: Suggested name for the downloaded file.
-        data: The data to be downloaded. It may be a string, a byte[],
-            or an InputStream. Strings will be written with in "utf-8"
-            encoding.
-        contentType: Value for the "Content-Type" header. Example:
+        filename (str): Suggested name for the downloaded file.
+        data (object): The data to be downloaded. May be a String, a
+            byte[], or an InputStream. Strings will be written with in
+            "utf-8" encoding.
+        contentType (str): Value for the "Content-Type" header. Example:
             "text/plain; charset=utf-8". Optional.
-        sessionId: Identifier of the Session to target. If omitted the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        sessionId (str): Identifier of the Session to target. If omitted
+            the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
     """
     builtins.print(filename, data, contentType, sessionId, pageId)
 
 
-def getProjectInfo():
-    # type: () -> Dict[AnyStr, Any]
+def getProjectInfo(projectName):
     """Returns a dictionary of meta data from a Perspective Project.
 
+    Args:
+        projectName (str): The name of the project.
+
     Returns:
-        A dictionary of project meta data.
+        dict: A dictionary of project meta data.
     """
+    builtins.print(projectName)
     return {
         "name": "Project",
         "title": "Project",
         "description": "Project's description",
-        "lastModified": "2021-11-22T20:46:00.000Z",
+        "lastModified": "2021-04-01T13:37:00.000Z",
         "lastModifiedBy": "thecesrom",
         "views": [{"path": "Page/Home"}],
-        "pageConfigs": [{"url": "", "primaryView": ""}],
     }
 
 
-def getSessionInfo(
-    usernameFilter=None,  # type: Optional[AnyStr]
-    projectFilter=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> List[PyJsonObjectAdapter]
-    """Returns information about one or more Perspective Sessions.
+def getSessionInfo(usernameFilter=None, projectFilter=None):
+    """Returns information about one or more Perspective sessions.
 
     The information returned by this function is a combination of
-    information available on the perspective Sessions status page on the
-    Gateway, and some Session props (id and userAgent).
+    information available on the perspective sessions status page on the
+    Gateway, and some session props (id and userAgent).
 
     Args:
-        usernameFilter: A filter based on logged-in user. Optional.
-        projectFilter: A filter based on the project name. Optional.
+        usernameFilter (str): A filter based on logged in user.
+            Optional.
+        projectFilter (str): A filter based on the project name.
+            Optional.
 
     Returns:
-        A list of objects (PyJsonObjectAdapter).
+        list[PyJsonObjectAdapter]: A list of objects
+            (PyJsonObjectAdapter).
     """
     builtins.print(usernameFilter, projectFilter)
-    return [PyJsonObjectAdapter(JsonObject())]
+    return [PyJsonObjectAdapter(None)]
 
 
 def isAuthorized(isAllOf, securityLevels, sessionId="current_session"):
-    # type: (bool, List[AnyStr], AnyStr) -> bool
-    """Checks if the user in the current Session is authorized against a
+    """Checks if the user in the current session is authorized against a
     target collection of security levels.
 
     Args:
-        isAllOf: True if the current user must have all of the given
-            security levels to be authorized. False if the current user
-            must have at least one of the given security levels to be
-            authorized.
-        securityLevels: An array of string paths to a security level
-            node in the form of "Path/To/Node". Each level in the tree
-            is delimited by a forward slash character. The public node
-            is never a part of the path.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. Optional.
+        isAllOf (bool): True if the current user must have all of the
+            given security levels to be authorized. False if the current
+            user must have at least one of the given security levels to
+            be authorized.
+        securityLevels (list[str]): An array of string paths to a
+            security level node in the form of "Path/To/Node". Each
+            level in the tree is delimited by a forward slash character.
+            The public node is never a part of the path.
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            Optional.
 
     Returns:
-        True if the user in the current Session is authorized, False
-        otherwise.
+        bool: True if the user in the current session is authorized,
+            False otherwise.
     """
     builtins.print(isAllOf, securityLevels, sessionId)
     return True
 
 
 def login(sessionId="current_session", pageId="current_page", forceAuth=False):
-    # type: (AnyStr, AnyStr, bool) -> None
     """Triggers a login event that will allow the user to login with the
     project's configured Identity Provider (IdP).
 
     For this function to work, an Identity Provider must be set in
     Perspective project properties. This is particularly useful when you
-    want it to be possible to start a Session without authentication and
+    want it to be possible to start a session without authentication and
     sign in to access certain restricted features.
 
     Args:
-        sessionId: Identifier of the Session to target. If omitted the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        sessionId (str): Identifier of the Session to target. If omitted
+            the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
-        forceAuth: Determines if Ignition should ask the Identity
+        forceAuth (bool): Determines if Ignition should ask the Identity
             Provider to re-authenticate the user, even if the user is
             already signed into the Identity Provider. If set to True,
             then the Identity Provider will ask the user to re-enter
             their credentials. If set to False, then the Gateway will
             request that the Identity Provider use the last provided
-            credentials for the Session, potentially allowing
+            credentials for the session, potentially allowing
             re-authentication without requiring the user to re-type
             their credentials. Note that support for this argument is
             determined by the Identity Provider; the IdP may choose to
             ignore this request. If this parameter is omitted, then the
             function will use the re-authentication setting defined
             under Project Properties. Optional.
     """
     builtins.print(sessionId, pageId, forceAuth)
 
 
-def logout(
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    message="default message",  # type: AnyStr
-):
-    # type: (...) -> None
+def logout(sessionId="current_session", pageId="current_page"):
     """Triggers a logout event, which will log the user out.
 
     For this function to work, an Identity Provider must be set in the
     Perspective project properties.
 
     Args:
-        sessionId: Identifier of the Session to target. If omitted the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
-            current Page will be used automatically. Optional.
-        message: The message to display when the user logs out of their
-            session. This message is only shown when the project
-            requires authentication. If omitted, the default message
-            (set in Project Properties) is shown. Optional.
+        sessionId (str): Identifier of the Session to target. If omitted
+            the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
+            current Page will be used automatically. Optional.
     """
-    builtins.print(sessionId, pageId, message)
+    builtins.print(sessionId, pageId)
 
 
 def navigate(
-    page,  # type: AnyStr
-    url=None,  # type: Optional[AnyStr]
-    view=None,  # type: Optional[AnyStr]
-    params=None,  # type: Optional[Dict[AnyStr, AnyStr]]
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    newTab=False,  # type: bool
+    page,
+    url=None,
+    view=None,
+    params=None,
+    sessionId="current_session",
+    pageId="current_page",
+    newTab=False,
 ):
-    # type: (...) -> None
-    """Navigate the Session to a specified view or mounted page.
+    """Navigate the session to a specified view or mounted page.
 
     The function can be used in three different ways, depending on which
     parameter is specified:
         page: navigates to a perspective-page
-        url: navigates to a Web address, so the function can be used to
-            navigate the user to a Web portal, search engine, or other
-            Website. This parameter is specified via keyword argument
+        url: navigates to a web address, so the function can be used to
+            navigate the user to a web portal, search engine, or other
+            website. This parameter is specified via keyword argument
         view: navigates to a view. Note that using this parameter does
-            not modify the Web browser's address bar, so the browser's
+            not modify the web browser's address bar, so the browser's
             history will not contain a listing for the new view. This
             parameter is specified via keyword argument
 
     Args:
-        page: The URL of a Perspective page to navigate to.
-        url: The URL of a Web address to navigate to. If the page or
-            view parameters are specified, then this parameter is
-            ignored. Optional.
-        view: If specified, will navigate to a specific view. Navigating
-            to a view via this parameter does not change the address in
-            the Web browser. Thus the Web browser's back button will not
-            be able to return the user to the previous view. If the page
-            parameter is specified, then this parameter is ignored.
-            Optional.
-        params: Used only in conjunction with the view parameter,
+        page (str): The URL of a Perspective page to navigate to.
+        url (str): The URL of a web address to navigate to. If the page
+            or view parameters are specified, then this parameter is
+            ignored.
+        view (str): If specified, will navigate to a specific view.
+            Navigating to a view via this parameter does not change the
+            address in the web browser. Thus the web browser's back
+            button will not be able to return the user to the previous
+            view. If the page parameter is specified, then this
+            parameter is ignored. Optional.
+        params (dict): Used only in conjunction with the view parameter,
             Dictionary of values to pass to any parameters on the view.
             Optional.
-        sessionId: Identifier of the Session to target. If omitted
+        sessionId (str): Identifier of the Session to target. If omitted
             the current Session will be used automatically. When
-            targeting a different Session, then the pageId parameter
+            targeting a different session, then the pageId parameter
             must be included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
-        newTab: If True, opens the contents in a new tab.
+        newTab (bool): If True, opens the contents in a new tab.
             Optional.
     """
     builtins.print(page, url, view, params, sessionId, pageId, newTab)
 
 
-def navigateBack(sessionId="current_session", pageId="current_page"):
-    # type: (AnyStr, AnyStr) -> None
-    """Navigate the Session to a specified view or mounted page.
+def navigateBack(sessionId=None, pageId=None):
+    """Navigate the session to a specified view or mounted page.
 
     This is similar to a browser's "back" function.
 
     Args:
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. Optional.
-        pageId: Identifier of the page to target. If omitted, the
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            Optional.
+        pageId (str): Identifier of the page to target. If omitted, the
             current page will be used automatically. Optional.
     """
     builtins.print(sessionId, pageId)
 
 
-def navigateForward(sessionId="current_session", pageId="current_page"):
-    # type: (AnyStr, AnyStr) -> None
-    """Navigate the Session to a specified view or mounted page.
+def navigateForward(sessionId=None, pageId=None):
+    """Navigate the session to a specified view or mounted page.
 
     This is similar to a browser's "forward" function.
 
     Args:
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the page to target. If omitted, the
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the page to target. If omitted, the
             current page will be used automatically. Optional.
     """
     builtins.print(sessionId, pageId)
 
 
 def openDock(
-    id,  # type: AnyStr
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    params=None,  # type: Optional[Dict[AnyStr, AnyStr]]
+    id, sessionId="current_session", pageId="current_page", params=None
 ):
-    # type: (...) -> None
     """Opens a docked View.
 
     Requires the preconfigured dock ID for the view.
 
     Args:
-        id: The unique, preconfigured 'Dock ID' for the docked View. Is
-            specified when a View is assigned as docked for a particular
-            Page (in Page Configuration).
-        sessionId: Identifier of the Session to target. If omitted the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        id (str): The unique, preconfigured 'Dock ID' for the docked
+            View. Is specified when a View is assigned as docked for a
+            particular Page (in Page Configuration).
+        sessionId (str): Identifier of the Session to target. If omitted
+            the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
-        params: Parameters that can be passed into the docked view. Must
-            match the docked views View Parameters. Optional.
+        params (dict): Parameters that can be passed into the docked
+            view. Must match the docked views View Parameters. Optional.
     """
     builtins.print(id, sessionId, pageId, params)
 
 
 def openPopup(
-    id,  # type: AnyStr
-    view,  # type: AnyStr
-    params=None,  # type: Optional[Dict[AnyStr, Any]]
-    title="",  # type: AnyStr
-    position=None,  # type: Optional[Dict[AnyStr, Union[int, AnyStr]]]
-    showCloseIcon=True,  # type: bool
-    draggable=True,  # type: bool
-    resizable=False,  # type: bool
-    modal=False,  # type: bool
-    overlayDismiss=False,  # type: bool
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    viewPortBound=False,  # type: bool
+    id,
+    view,
+    params=None,
+    title="",
+    position=None,
+    showCloseIcon=True,
+    draggable=True,
+    resizable=False,
+    modal=False,
+    overlayDismiss=False,
+    sessionId="current_session",
+    pageId="current_page",
+    viewPortBound=False,
 ):
-    # type: (...) -> None
     """Open a popup view over the given page.
 
     Args:
-        id: A unique popup string. Will be used to close the popup from
-            other popup or script actions.
-        view: The path to the View to use in the popup.
-        params: Dictionary of key-value pairs to us as input parameters
-            to the View. Optional.
-        title: Text to display in the title bar. If no value or an empty
-            string are given, the title bar will not be displayed.
+        id (str): A unique popup string. Will be used to close the popup
+            from other popup or script actions.
+        view (str): The path to the View to use in the popup.
+        params (dict): Dictionary of key-value pairs to us as input
+            parameters to the View. Optional.
+        title (str): Text to display in the title bar. If no value or an
+            empty string are given, the title bar will not be displayed.
             Defaults to an empty string. Optional.
-        position: Dictionary of key-value pairs to use for position.
-            Possible position keys are: left, top, right, bottom, width,
-            height. Defaults to the center of the window. Optional.
-        showCloseIcon: Will show the close icon if True. Defaults to
-            True. Optional.
-        draggable: Will allow the popup to be dragged if True. Defaults
-            to True. Optional.
-        resizable: Will allow the popup to be resized if True. Defaults
-            to False. Optional.
-        modal: Will make the popup modal if True. A modal popup is the
-            only view the user can interact with. Defaults to False.
+        position (dict): Dictionary of key-value pairs to use for
+            position. Possible position keys are: left, top, right,
+            bottom, width, height. Defaults to the center of the window.
             Optional.
-        overlayDismiss: Will allow the user to dismiss and close a modal
-            popup by clicking outside of it if True. Defaults to False.
-            Optional.
-        sessionId: Identifier of the Session to target. If omitted the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
-            current Page will be used automatically. Optional.
-        viewPortBound: If True, popups will be "shifted" to open within
-            the bounds of the viewport. If the popup would be larger
-            than the viewport, then it will be resized to fit within the
-            bounds. Default is False. Optional.
+        showCloseIcon (bool): Will show the close icon if True. Defaults
+            to True. Optional.
+        draggable (bool): Will allow the popup to be dragged if True.
+            Defaults to True. Optional.
+        resizable (bool): Will allow the popup to be resized if True.
+            Defaults to False. Optional.
+        modal (bool): Will make the popup modal if True. A modal popup
+            is the only view the user can interact with. Defaults to
+            False. Optional.
+        overlayDismiss (bool): Will allow the user to dismiss and close
+            a modal popup by clicking outside of it if True. Defaults to
+            False. Optional.
+        sessionId (str): Identifier of the Session to target. If omitted
+            the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
+            current Page will be used automatically. Optional.
+        viewPortBound (bool): If True, popups will be "shifted" to open
+            within the bounds of the viewport. If the popup would be
+            larger than the viewport, then it will be resized to fit
+            within the bounds. Default is False. Optional.
     """
     builtins.print(
         id,
         view,
         params,
         title,
         position,
@@ -561,192 +527,179 @@
         sessionId,
         pageId,
         viewPortBound,
     )
 
 
 def print(
-    message,  # type: AnyStr
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    destination="client",  # type: AnyStr
+    message,
+    sessionId="current_session",
+    pageId="current_page",
+    destination="client",
 ):
-    # type: (...) -> None
     """Sends print statements to the scripting console when in the
     Designer.
 
     When in a Session, sends print statements to the output console.
     This function makes scripting diagnostics easier.
 
     Args:
-        message: The print statement that will be displayed on the
+        message (str): The print statement that will be displayed on the
             console.
-        sessionId: Identifier of the Session to target. If omitted the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        sessionId (str): Identifier of the Session to target. If omitted
+            the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
-        destination: Where the message should be printed. If specified,
-            must be "client", "gateway", or "all". Default is "client".
-            Optional.
+        destination (str): Where the message should be printed. If
+            specified, must be "client", "gateway", or "all". Default is
+            "client". Optional.
     """
     builtins.print(message, sessionId, pageId, destination)
 
 
 def refresh(sessionId="current_session", pageId="current_page"):
-    # type: (AnyStr, AnyStr) -> None
     """Triggers a refresh of the page.
 
-    Note:
-        This method should not be confused with the refreshBinding
-        component method, which automatically fires a binding on a
-        Perspective component property.
-
     Args:
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
     """
     builtins.print(sessionId, pageId)
 
 
 def sendMessage(
-    messageType,  # type: AnyStr
-    payload,  # type: Dict[AnyStr, AnyStr]
-    scope="page",  # type: AnyStr
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-):
-    # type: (...) -> None
-    """Send a message to a message handler within the same Session.
-
-    Args:
-        messageType: The message type that will be invoked. Message
-            handlers configured within the project are listening for
-            messages of a specific messageType.
-        payload: A python dictionary representing any parameters that
-            will be passed to the message handler.
-        scope: The scope that the message should be delivered to. Valid
-            values are "Session", "page", or "view". If omitted, "page"
-            will be used. Optional.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
-            current Page will be used. Optional.
+    messageType,
+    payload,
+    scope="page",
+    sessionId="current_session",
+    pageId="current_page",
+):
+    """Send a message to a message handler within the same session.
+
+    Args:
+        messageType (str): The message type that will be invoked.
+            Message handlers configured within the project are listening
+            for messages of a specific messageType.
+        payload (dict): A python dictionary representing any parameters
+            that will be passed to the message handler.
+        scope (str): The scope that the message should be delivered to.
+            Valid values are "session", "page", or "view". If omitted,
+            "page" will be used. Optional.
+        sessionId (str): Identifier of the Session to target. If
+            omitted, the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
+            current Page will be used automatically. Optional.
     """
     builtins.print(messageType, payload, scope, sessionId, pageId)
 
 
 def setTheme(name, sessionId="current_session", pageId="current_page"):
-    # type: (AnyStr, AnyStr, AnyStr) -> None
     """Changes the theme in a page to the specified theme.
 
     Note that this function only changes the theme for a single page,
     not the entire session. To change the theme for a session, write
     directly to the session.theme property instead.
 
     Args:
-        name: The theme name to switch to. Possible values are "dark" or
-            "light".
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        name (str): The theme name to switch to. Possible values are
+            "dark" or "light".
+        sessionId (str): Identifier of the Session to target. If
+            omitted the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
     """
     builtins.print(name, sessionId, pageId)
 
 
 def toggleDock(
-    id,  # type: AnyStr
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    params=None,  # type: Optional[Dict[AnyStr, AnyStr]]
+    id, sessionId="current_session", pageId="current_page", params=None
 ):
-    # type: (...) -> None
     """Toggles a docked View.
 
     Args:
-        id: The unique, preconfigured 'Dock ID' for the docked View. Is
-            specified when a View is assigned as docked for a particular
-            Page (in Page Configuration).
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
+        id (str): The unique, preconfigured 'Dock ID' for the docked
+            View. Is specified when a View is assigned as docked for a
+            particular Page (in Page Configuration).
+        sessionId (str): Identifier of the Session to target. If
+            omitted the current Session will be used automatically.
+            When targeting a different session, then the pageId
+            parameter must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
             current Page will be used automatically. Optional.
-        params: Parameters that can be passed into the docked view. Must
-            match the docked views View Parameters. Optional.
+        params (dict): Parameters that can be passed into the docked
+            view. Must match the docked views View Parameters. Optional.
     """
     builtins.print(id, sessionId, pageId, params)
 
 
 def togglePopup(
-    id,  # type: AnyStr
-    view,  # type: AnyStr
-    params,  # type: Optional[Dict[AnyStr, Any]]
-    title="",  # type: AnyStr
-    position=None,  # type: Optional[Dict[AnyStr, Union[int, AnyStr]]]
-    showCloseIcon=True,  # type: bool
-    draggable=True,  # type: bool
-    resizable=False,  # type: bool
-    modal=False,  # type: bool
-    overlayDismiss=False,  # type: bool
-    sessionId="current_session",  # type: AnyStr
-    pageId="current_page",  # type: AnyStr
-    viewPortBound=False,  # type: bool
+    id,
+    view,
+    params,
+    title="",
+    position=None,
+    showCloseIcon=True,
+    draggable=True,
+    resizable=False,
+    modal=False,
+    overlayDismiss=False,
+    sessionId="current_session",
+    pageId="current_page",
+    viewPortBound=False,
 ):
-    # type: (...) -> None
-    """Toggles a popup view.
+    """Toggles a popup.
 
     Will open up the popup if it has not been opened yet. Otherwise, it
     will close the currently opened popup.
 
     Args:
-        id: A unique popup string. Will be used to close the popup from
-            other popup or script actions.
-        view: The path to the View to use in the popup.
-        params: Dictionary of key-value pairs to us as input parameters
-            to the View. Optional.
-        title: Text to display in the title bar. If no value or an empty
-            string are given, the title bar will not be displayed.
+        id (str): A unique popup string. Will be used to close the popup
+            from other popup or script actions.
+        view (str): The path to the View to use in the popup.
+        params (dict): Dictionary of key-value pairs to us as input
+            parameters to the View. Optional.
+        title (str): Text to display in the title bar. If no value or an
+            empty string are given, the title bar will not be displayed.
             Defaults to an empty string. Optional.
-        position: Dictionary of key-value pairs to use for position.
-            Possible position keys are: left, top, right, bottom, width,
-            height. Defaults to the center of the window. Optional.
-        showCloseIcon: Will show the close icon if True. Defaults to
-            True. Optional.
-        draggable: Will allow the popup to be dragged if True. Defaults
-            to True. Optional.
-        resizable: Will allow the popup to be resized if True. Defaults
-            to False. Optional.
-        modal: Will make the popup modal if True. A modal popup is the
-            only view the user can interact with. Defaults to False.
+        position (dict): Dictionary of key-value pairs to use for
+            position. Possible position keys are: left, top, right,
+            bottom, width, height. Defaults to the center of the window.
             Optional.
-        overlayDismiss: Will allow the user to dismiss and close a modal
-            popup by clicking outside of it if True. Defaults to False.
-            Optional.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. When targeting a
-            different Session, then the pageId parameter must be
-            included in the call. Optional.
-        pageId: Identifier of the Page to target. If omitted, the
-            current Page will be used automatically. Optional.
-        viewPortBound: If True, popups will be "shifted" to open within
-            the bounds of the viewport. If the popup would be larger
-            than the viewport, then it will be resized to fit within the
-            bounds. Default is False. Optional.
+        showCloseIcon (bool): Will show the close icon if True. Defaults
+            to True. Optional.
+        draggable (bool): Will allow the popup to be dragged if True.
+            Defaults to True. Optional.
+        resizable (bool): Will allow the popup to be resized if True.
+            Defaults to False. Optional.
+        modal (bool): Will make the popup modal if True. A modal popup
+            is the only view the user can interact with. Defaults to
+            False. Optional.
+        overlayDismiss (bool): Will allow the user to dismiss and close
+            a modal popup by clicking outside of it if True. Defaults to
+            False. Optional.
+        sessionId (str): Identifier of the Session to target. If omitted
+            the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
+        pageId (str): Identifier of the Page to target. If omitted, the
+            current Page will be used automatically. Optional.
+        viewPortBound (bool): If True, popups will be "shifted" to open
+            within the bounds of the viewport. If the popup would be
+            larger than the viewport, then it will be resized to fit
+            within the bounds. Default is False. Optional.
     """
     builtins.print(
         id,
         view,
         params,
         title,
         position,
@@ -758,22 +711,19 @@
         sessionId,
         pageId,
         viewPortBound,
     )
 
 
 def vibrateDevice(duration, sessionId="current_session"):
-    # type: (int, AnyStr) -> None
-    """When called from the Perspective App, will cause the device to
-    vibrate for the specified number of milliseconds.
-
-    Note:
-        iOS vibration duration is fixed. This function will cause an iOS
-        device to vibrate for its default duration, 0.4 seconds
-        (400 milliseconds).
+    """When called from the Perspective mobile app, will cause the
+    device to vibrate for the specified number of milliseconds.
 
     Args:
-        duration: The duration in milliseconds to vibrate the device.
-        sessionId: Identifier of the Session to target. If omitted, the
-            current Session will be used automatically. Optional.
+        duration (int): The duration in milliseconds to vibrate the
+            device.
+        sessionId (str): Identifier of the Session to target. If
+            omitted the current Session will be used automatically. When
+            targeting a different session, then the pageId parameter
+            must be included in the call. Optional.
     """
     builtins.print(duration, sessionId)
```

### Comparing `ignition_api-8.1.40/src/system/nav.py` & `ignition-api-8.1.9/src/system/nav.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Navigation Functions.
 
 The following functions allow you to open and close windows in the
 client.
 """
 
 from __future__ import print_function
@@ -17,225 +21,298 @@
     "goHome",
     "openWindow",
     "openWindowInstance",
     "swapTo",
     "swapWindow",
 ]
 
-from typing import Any, Dict, Optional, Union
+from abc import ABCMeta, abstractmethod
 
-from com.inductiveautomation.factorypmi.application import FPMIWindow
-from com.inductiveautomation.factorypmi.application.script.builtin import NavUtilities
-from dev.coatl.helper.types import AnyStr
 from java.util import EventObject
+from javax.swing import JInternalFrame
+
+
+class FPMIWindow(JInternalFrame):
+    """FPMIWindow object."""
+
+    # Fields.
+    CACHE_ALWAYS = 2
+    CACHE_AUTO = 0
+    CACHE_NEVER = 1
+    DOCK_EAST = 2
+    DOCK_FLOAT = 0
+    DOCK_NORTH = 2
+    DOCK_SOUTH = 4
+    DOCK_WEST = 3
+    PARENT_WINDOW_NAME = "_parent"
+    SHOW_ALWAYS = 0
+    SHOW_NEVER = 1
+    SHOW_MAXIMIZED = 2
+
+    _path = "Path/To/Window"
+
+    def __init__(self, name):
+        self.name = name
+
+    def getPath(self):
+        return self._path
+
+    def getRootContainer(self):
+        print(self)
+
+
+class INavUtilities(ABCMeta):
+    """Parent interface to coordinate the functions between NavUtilities
+    and NavUtilitiesDispatcher.
+    """
+
+    def __new__(mcs, *args, **kwargs):
+        pass
+
+    @abstractmethod
+    def centerWindow(cls, arg):
+        pass
+
+    @abstractmethod
+    def closeParentWindow(cls, event):
+        pass
+
+    @abstractmethod
+    def closeWindow(cls, arg):
+        pass
+
+    @abstractmethod
+    def getCurrentWindow(cls):
+        pass
+
+    @abstractmethod
+    def goBack(cls):
+        pass
+
+    @abstractmethod
+    def goForward(cls):
+        pass
+
+    @abstractmethod
+    def goHome(cls):
+        pass
+
+    @abstractmethod
+    def openWindow(cls, *args):
+        pass
+
+    @abstractmethod
+    def openWindowImpl(cls, path, params, openAdditional):
+        pass
+
+    @abstractmethod
+    def openWindowInstance(cls, *args):
+        pass
+
+    @abstractmethod
+    def swapTo(cls, *args):
+        pass
+
+    @abstractmethod
+    def swapWindow(cls, *args):
+        pass
 
 
 def centerWindow(arg):
-    # type: (Union[AnyStr, FPMIWindow]) -> None
     """Given a window path, or a reference to a window itself, it will
     center the window.
 
     The window should be floating and non-maximized. If the window can't
     be found, this function will do nothing.
 
     Args:
-        arg: The path of the window or a reference to the window to
-            center.
+        arg (object): The path of the window (str) or a reference to the
+            window (FPMIWindow) to center.
     """
     print(arg)
 
 
 def closeParentWindow(event):
-    # type: (EventObject) -> None
     """Closes the parent window given a component event object.
 
     Args:
-        event: A component event object. The enclosing window for the
-            component will be closed.
+        event (EventObject): A component event object. The enclosing
+            window for the component will be closed.
     """
     print(event)
 
 
 def closeWindow(arg):
-    # type: (Union[AnyStr, FPMIWindow]) -> None
     """Given a window path, or a reference to a window itself, it will
     close the window.
 
     If the window can't be found, this function will do nothing.
 
     Args:
-        arg: The path of the window or a reference to the window to
-            center.
+        arg (object): A reference to the window to close as an
+            FPMIWindow instance or the path of the window to close as a
+            String.
     """
     print(arg)
 
 
 def desktop(handle="primary"):
-    # type: (Optional[AnyStr]) -> NavUtilities
     """Allows for invoking system.nav functions on a specific desktop.
 
     Args:
-        handle: The handle for the desktop to use. May be omitted for
-            the primary desktop. Optional.
+        handle (str): The handle for the desktop to use. The screen
+            index casted as a string may be used instead of the handle.
+            If omitted, this will default to the Primary Desktop.
+            Alternatively, the handle "primary" can be used to refer to
+            the Primary Desktop.
 
     Returns:
-        A copy of system.nav that will alter the desktop named by the
-        given handle.
+        INavUtilities: A copy of system.nav that will alter the desktop
+            named by the given handle.
     """
     print(handle)
-    return NavUtilities()
+    return INavUtilities()
 
 
 def getCurrentWindow():
-    # type: () -> AnyStr
     """Returns the path of the current "main screen" window, which is
     defined as the maximized window.
 
-    With the typical navigation, there is only ever one maximized window
-    at a time.
+    With the Typical Navigation Strategy, there is only ever one
+    maximized window at a time.
 
     Returns:
-        The path of the current "main screen" window - the maximized
-        window.
+        str: The path of the current "main screen" window - the
+            maximized window.
     """
     return "Path/To/Maximized Window"
 
 
 def goBack():
-    # type: () -> FPMIWindow
-    """When using the typical navigation strategy, this function will
+    """When using the Typical Navigation Strategy, this function will
     navigate back to the previous main screen window.
 
     Returns:
-        A reference to window that was navigated to.
+        FPMIWindow: The window that was returned to.
     """
     return FPMIWindow("Back")
 
 
 def goForward():
-    # type: () -> FPMIWindow
-    """When using the typical navigation strategy, this function will
-    navigate "forward" to the last main screen window the user was on
+    """When using the Typical Navigation Strategy, this function will
+    navigate "forward" to the last main-screen window the user was on
     when they executed a system.nav.goBack().
 
     Returns:
-        A reference to window that was navigated to.
+        FPMIWindow: The window that was returned to.
     """
     return FPMIWindow("Forward")
 
 
 def goHome():
-    # type: () -> FPMIWindow
-    """When using the typical navigation strategy, this function will
+    """When using the Typical Navigation Strategy, this function will
     navigate to the "home" window.
 
     This is automatically detected as the first main-screen window shown
     in a project.
 
     Returns:
-        A reference to window that was navigated to.
+        FPMIWindow: The window that was returned to.
     """
     return FPMIWindow("Home")
 
 
 def openWindow(path, params=None):
-    # type: (AnyStr, Optional[Dict[AnyStr, Any]]) -> FPMIWindow
     """Opens the window with the given path.
 
     If the window is already open, brings it to the front. The optional
     params dictionary contains key:value pairs which will be used to set
     the target window's root container's dynamic variables.
 
     Args:
-        path: The path to the window to open.
-        params: A dictionary of parameters to pass into the window. The
-            keys in the dictionary must match dynamic property names on
-            the target window's root container. The values for each key
-            will be used to set those properties. Optional.
+        path (str): The path to the window to open.
+        params (dict): A dictionary of parameters to pass into the
+            window. The keys in the dictionary must match dynamic
+            property names on the target window's root container. The
+            values for each key will be used to set those properties.
+            Optional.
 
     Returns:
-        A reference to the opened window.
+        FPMIWindow: A reference to the opened window.
     """
     print(path, params)
     return FPMIWindow("Opened Window")
 
 
 def openWindowInstance(path, params=None):
-    # type: (AnyStr, Optional[Dict[AnyStr, Any]]) -> FPMIWindow
     """Operates exactly like system.nav.openWindow, except that if the
     named window is already open, then an additional instance of the
     window will be opened.
 
     There is no limit to the number of additional instances of a window
     that you can open.
 
     Args:
-        path: The path to the window to open.
-        params: A dictionary of parameters to pass into the window. The
-            keys in the dictionary must match dynamic property names on
-            the target window's root container. The values for each key
-            will be used to set those properties. Optional.
+        path (str): The path to the window to open.
+        params (dict): A dictionary of parameters to pass into the
+            window. The keys in the dictionary must match dynamic
+            property names on the target window's root container. The
+            values for each key will be used to set those properties.
+            Optional.
 
     Returns:
-        A reference to the opened window.
+        FPMIWindow: A reference to the opened window.
     """
     print(path, params)
     return FPMIWindow("Window Instance")
 
 
 def swapTo(path, params=None):
-    # type: (AnyStr, Optional[Dict[AnyStr, Any]]) -> FPMIWindow
     """Performs a window swap from the current main screen window to the
     window specified.
 
     Swapping means that the opened window will take the place of the
     closing window - in this case it will be maximized.
 
     This function works like system.nav.swapWindow except that you
     cannot specify the source for the swap.
 
     Args:
-        path: The path to the window to open.
-        params: A dictionary of parameters to pass into the window. The
-            keys in the dictionary must match dynamic property names on
-            the target window's root container. The values for each key
-            will be used to set those properties. Optional.
+        path (str): The path to the window to open.
+        params (dict): A dictionary of parameters to pass into the
+            window. The keys in the dictionary must match dynamic
+            property names on the target window's root container. The
+            values for each key will be used to set those properties.
+            Optional.
 
     Returns:
-        A reference to the swapped-to window.
+        FPMIWindow: A reference to the swapped-to window.
     """
     print(path, params)
     return FPMIWindow("Swapped To")
 
 
-def swapWindow(
-    arg,  # type: Union[AnyStr, EventObject]
-    swapToPath,  # type: AnyStr
-    params=None,  # type: Optional[Dict[AnyStr, Any]]
-):
-    # type: (...) -> FPMIWindow
+def swapWindow(arg, swapToPath, params=None):
     """Performs a window swap.
 
     This means that one window is closed, and another is opened and
     takes its place - assuming its size, floating state, and
     maximization state. This gives a seamless transition; one window
     seems to simply turn into another.
 
-    This function works like system.nav.swapTo except that you can
-    specify the source and destination for the swap.
-
     Args:
-        arg: The path of the window to swap from. Must be a currently
-            open window, otherwise this will act like an openWindow, or
-            a component event (EventObject) whose enclosing window will
-            be used as the "swap-from" window.
-        swapToPath: The name of the window to swap to.
-        params: A dictionary of parameters to pass into the window. The
-            keys in the dictionary must match dynamic property names on
-            the target window's root container. The values for each key
-            will be used to set those properties. Optional.
+        arg (object): The path of the window (str) to swap from. Must be
+            a currently open window, or this will act like an
+            openWindow, or a component event (EventObject) whose
+            enclosing window will be used as the "swap-from" window.
+        swapToPath (str): The name of the window to swap to.
+        params (dict): A dictionary of parameters to pass into the
+            window. The keys in the dictionary must match dynamic
+            property names on the target window's root container. The
+            values for each key will be used to set those properties.
+            Optional.
 
     Returns:
-        A reference to the swapped-to window.
+        FPMIWindow: A reference to the swapped-to window.
     """
     print(arg, swapToPath, params)
     return FPMIWindow("Swapped To")
```

### Comparing `ignition_api-8.1.40/src/system/eam.py` & `ignition-api-8.1.9/src/system/eam.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,134 +1,135 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """EAM Functions.
 
 The following functions give you access to view EAM information from the
 Gateway.
 """
 
 from __future__ import print_function
 
 __all__ = ["getGroups", "queryAgentHistory", "queryAgentStatus", "runTask"]
 
-from typing import List, Optional
-
-from com.inductiveautomation.ignition.common import BasicDataset
-from com.inductiveautomation.ignition.common.messages import UIResponse
-from dev.coatl.helper.types import AnyStr
+import system.date
+from java.lang import Object
 from java.util import Date, Locale
+from system.dataset import Dataset
+
+
+class UIResponse(Object):
+    def __init__(self, locale):
+        self.locale = locale
+
+    def attempt(self, method):
+        pass
+
+    def error(self, message, args):
+        pass
+
+    def getErrors(self):
+        pass
+
+    def getInfos(self):
+        pass
+
+    def getLocale(self):
+        pass
+
+    def getWarns(self):
+        pass
+
+    def info(self, message, args):
+        pass
+
+    def warn(self, message, args):
+        pass
+
+    def wrap(self, locale, fx):
+        pass
 
 
 def getGroups():
-    # type: () -> List[AnyStr]
     """Returns the names of the defined agent organizational groups in
     the Gateway.
 
-    This function should only be called from the Controller.
-
-    Note:
-        If called from an Agent on 8.1.11+, this function will return an
-        exception.
-
     Returns:
-        A string list of group names.
+        list[str]: A string list of group names.
     """
     return [""]
 
 
 def queryAgentHistory(
-    groupIds=None,  # type: Optional[List[AnyStr]]
-    agentIds=None,  # type: Optional[List[AnyStr]]
-    startDate=None,  # type: Optional[Date]
-    endDate=None,  # type: Optional[Date]
-    limit=100,  # type: int
+    groupIds=None, agentIds=None, startDate=None, endDate=None, limit=100
 ):
-    # type: (...) -> BasicDataset
     """Returns a list of the most recent agent events.
 
-    This function should only be called from the Controller.
-
-    Note:
-        If called from an Agent on 8.1.11+, this function will return an
-        exception.
-
     Args:
-        groupIds: A list of groups to restrict the results to. If not
-            specified, all groups will be included. Optional.
-        agentIds: A list of agent names to restrict the results to. If
-            not specified, all agents will be allowed. Optional.
-        startDate: The starting time for history events. If null,
-            defaults to 8 hours previous to now. Optional.
-        endDate: The ending time for the query range. If null, defaults
-            to "now". Optional.
-        limit: The limit of results to return. Defaults to 100. A value
-            of 0 means "no limit". Optional.
+        groupIds (list[str]): A list of groups to restrict the results
+            to. If not specified, all groups will be included. Optional.
+        agentIds (list[str]): A list of agent names to restrict the
+            results to. If not specified, all agents will be allowed.
+            Optional.
+        startDate (Date): The starting time for history events. If
+            null, defaults to 8 hours previous to now. Optional.
+        endDate (Date): The ending time for the query range. If
+            null, defaults to "now". Optional.
+        limit (int): The limit of results to return. Defaults to 100. A
+            value of 0 means "no limit". Optional.
 
     Returns:
-        A dataset with columns id, agent_name, agent_role, event_time,
-        event_category, event_type, event_source, event_level,
-        event_level_int, and message, where each row is a new agent
-        event.
+        Dataset: A dataset with columns id, agent_name, agent_role,
+            event_time, event_category, event_type, event_source,
+            event_level, event_level_int, and message, where each row is
+            a new agent event.
     """
+    endDate = system.date.now() if endDate is None else endDate
+    startDate = (
+        system.date.addHours(endDate, -8) if startDate is None else startDate
+    )
     print(groupIds, agentIds, startDate, endDate, limit)
-    return BasicDataset()
+    return Dataset()
 
 
-def queryAgentStatus(
-    groupIds=None,  # type: Optional[List[AnyStr]]
-    agentIds=None,  # type: Optional[List[AnyStr]]
-    isConnected=True,  # type: bool
-):
-    # type: (...) -> BasicDataset
+def queryAgentStatus(groupIds=None, agentIds=None, isConnected=True):
     """Returns the current state of the matching agents.
 
-    This function should only be called from the Controller.
-
-    Note:
-        If called from an Agent on 8.1.11+, this function will return an
-        exception.
-
     Args:
-        groupIds: A list of groups to restrict the results to. If not
-            specified, all groups will be included. Optional.
-        agentIds: A list of agent names to restrict the results to. If
-            not specified, all agents will be allowed. Optional.
-        isConnected: If True, only returns agents that are currently
-            connected. If False, only agents that are considered down
-            will be returned, and if not specified, all agents will be
-            returned. Optional.
+        groupIds (list[str]): A list of groups to restrict the results
+            to. If not specified, all groups will be included.
+        agentIds (list[str]): A list of agent names to restrict the
+            results to. If not specified, all agents will be allowed.
+        isConnected (bool): If True, only returns agents that are
+            currently connected. If False, only agents that are
+            considered down will be returned, and if not specified, all
+            agents will be returned.
 
     Returns:
-        A dataset with columns AgentName, NodeRole, AgentGroup,
-        LastCommunication, IsConnected, IsRunning, RunningState,
-        RunningStateInt, LicenseKey, and Version, where each row is a
-        new agent.
-
-        Possible values for RunningState and RunningStateInt are:
-        0 = Disconnected, 1 = Running, 2 = Warned, 3 = Errored.
+        Dataset: A dataset with columns AgentName, NodeRole, AgentGroup,
+            LastCommunication, IsConnected, IsRunning, RunningState,
+            RunningStateInt, LicenseKey, and Version, where each row is
+            a new agent.
     """
     print(groupIds, agentIds, isConnected)
-    return BasicDataset()
+    return Dataset()
 
 
 def runTask(taskname):
-    # type: (AnyStr) -> UIResponse
     """Takes the name of a task as an argument as a string (must be
     configured on the Controller before hand), attempts to execute the
     task.
 
-    This function should only be called from the Controller.
-
     To run in the client, the user needs a role-based permission. This
     permission is disabled by default.
 
-    Note:
-        If called from an Agent on 8.1.11+, this function will return an
-        exception.
-
     Args:
-        taskname: Name of the task to run. If more than one task has
-            this name, an error will be returned.
+        taskname (str): Name of the task to run. If more than one task
+            has this name, an error will be returned.
 
     Returns:
-        A UIResponse with a list of infos, errors, and warnings.
+        UIResponse: A UIResponse with a list of infos, errors, and
+            warnings.
     """
     print(taskname)
     return UIResponse(Locale.ENGLISH)
```

### Comparing `ignition_api-8.1.40/src/system/net.py` & `ignition-api-8.1.9/src/system/net.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Net Functions.
 
 The following functions give you access to interact with http services.
 """
 
 from __future__ import print_function
 
@@ -16,254 +20,319 @@
     "httpPost",
     "httpPut",
     "openURL",
     "sendEmail",
 ]
 
 import socket
-from typing import Any, Callable, Dict, List, Optional
 
-from com.inductiveautomation.ignition.common.script.builtin.http import JythonHttpClient
-from dev.coatl.helper.types import AnyStr
-from java.lang import IllegalArgumentException
+from java.lang import Object
+
+
+class JythonHttpClient(Object):
+    """A Jython-optimized wrapper around the base HttpClient available
+    in Java 11+.
+
+    Mostly, through convenience functions that make things easier to use
+    from Jython.
+    """
+
+    def delete(self, *args, **kwargs):
+        pass
+
+    def deleteAsync(self, *args, **kwargs):
+        pass
+
+    def get(self, *args, **kwargs):
+        pass
+
+    def getAsync(self, *args, **kwargs):
+        pass
+
+    def getConnectTimeout(self):
+        pass
+
+    def getCookieManager(self):
+        pass
+
+    def getJavaClient(self):
+        pass
+
+    def getRedirectPolicy(self):
+        pass
+
+    def head(self, *args, **kwargs):
+        pass
+
+    def headAsync(self, *args, **kwargs):
+        pass
+
+    def options(self, *args, **kwargs):
+        pass
+
+    def parseChart(self, contentType):
+        pass
+
+    def patch(self, *args, **kwargs):
+        pass
+
+    def patchAsync(self, *args, **kwargs):
+        pass
+
+    def post(self, *args, **kwargs):
+        pass
+
+    def postAsync(self, *args, **kwargs):
+        pass
+
+    def put(self, *args, **kwargs):
+        pass
+
+    def putAsync(self, *args, **kwargs):
+        pass
+
+    def request(self, *args, **kwargs):
+        pass
+
+    def requestAsync(self, *args, **kwargs):
+        pass
+
+    def trace(self, *args, **kwargs):
+        pass
+
+    def traceAsync(self, *args, **kwargs):
+        pass
 
 
 def getExternalIpAddress():
-    # type: () -> AnyStr
     """Returns the client's IP address, as it is detected by the
     Gateway.
 
     This means that this call will communicate with the Gateway, and the
     Gateway will tell the client what IP address its incoming traffic is
-    coming from. If you have a client behind a Network Address
-    Translation (NAT) router, then this address will be the Wide Area
-    Network (WAN) address of the router instead of the Local Area
-    Network (LAN) address of the client, which is what you'd get with
+    coming from. If you have a client behind a NAT router, then this
+    address will be the WAN address of the router instead of the LAN
+    address of the client, which is what you'd get with
     system.net.getIpAddress.
 
     Returns:
-        A text representation of the Client's IP address, as detected by
-        the Gateway.
+        str: A text representation of the client's IP address, as
+            detected by the Gateway.
     """
     return "52.52.32.221"
 
 
 def getHostName():
-    # type: () -> AnyStr
     """Returns the host name of the computer that the script was ran on.
 
     When run in the Gateway scope, returns the Gateway hostname. When
     run in the Client scope, returns the Client hostname. On Windows,
     this is typically the "computer name". For example, might return
     EAST_WING_WORKSTATION or bobs-laptop.
 
     Returns:
-        The hostname of the local machine.
+        str: The hostname of the local machine.
     """
     return socket.gethostname()
 
 
 def getIpAddress():
-    # type: () -> AnyStr
-    """Returns the IP address of the computer that the script was ran
-    on.
+    """Returns the IP address of the computer the client is running on,
+    as it appears to the client.
+
+    See also: system.net.getExternalIpAddress().
 
     Returns:
-        Returns the IP address of the local machine, as it sees it.
+        str: Returns the IP address of the local machine, as it sees it.
     """
-    return socket.gethostbyname(str(getHostName()))
+    return "127.0.0.1"
 
 
 def getRemoteServers(runningOnly=True):
-    # type: (Optional[bool]) -> List[AnyStr]
     """This function returns a List of Gateway Network servers that are
     visible from the local Gateway.
 
     Args:
-        runningOnly: If set to True, only servers on the Gateway Network
-            that are running will be returned. Servers that have lost
-            contact with the Gateway Network will be filtered out.
+        runningOnly (bool): If set to True, only servers on the Gateway
+            Network that are running will be returned. Servers that have
+            lost contact with the Gateway Network will be filtered out.
             Optional.
 
     Returns:
-        A List of strings representing Gateway Network Server IDs.
+        list[str]: A List of Strings representing Gateway Network server
+            ids.
     """
     print(runningOnly)
     return []
 
 
 def httpClient(
-    timeout=60000,  # type: int
-    bypass_cert_validation=False,  # type: bool
-    username=None,  # type: Optional[AnyStr]
-    password=None,  # type: Optional[AnyStr]
-    proxy=None,  # type: Optional[AnyStr]
-    cookie_policy="ACCEPT_ORIGINAL_SERVER",  # type: AnyStr
-    redirect_policy="NORMAL",  # type: AnyStr
-    version="HTTP_2",  # type: AnyStr
-    customizer=None,  # type: Optional[Callable[..., Any]]
+    timeout=60000,
+    bypass_cert_validation=True,
+    username=None,
+    password=None,
+    proxy=None,
+    cookie_policy="ACCEPT_ORIGINAL_SERVER",
+    redirect_policy="NORMAL",
+    customizer=None,
 ):
-    # type: (...) -> JythonHttpClient
     """Provides a general use object that can be used to send and
     receive HTTP requests.
 
     The object created by this function is a wrapper around Java's
     HttpClient class. Usage requires creating a JythonHttpClient object
     with a call to system.net.httpClient, then calling a method (such as
     get(), post()) on the JythonHttpClient to actually issue a request.
 
     Args:
-        timeout: A value, in milliseconds, to set the client's connect
-            timeout setting to. Defaults to 60000. Optional.
-        bypass_cert_validation: A boolean indicating whether the client
-            should attempt to validate the certificates of remote
-            servers, if connecting via HTTPS/SSL. Defaults to False.
+        timeout (int): A value, in milliseconds, to set the client's
+            connect timeout setting to. Defaults to 60000. Optional.
+        bypass_cert_validation (bool): A boolean indicating whether the
+            client should attempt to validate the certificates of remote
+            servers, if connecting via HTTPS/SSL. Defaults to True.
             Optional.
-        username: A string indicating the username to use for
+        username (str): A string indicating the username to use for
             authentication if the remote server requests authentication;
             specifically, by responding with a WWW-Authenticate or
             Proxy-Authenticate header. Only supports Basic
             authentication. If username is specified but not password,
             an empty string will be used for the password in the Basic
             Authentication response. Defaults to None. Optional.
-        password: A string indicating the password to use for
+        password (str): A string indicating the password to use for
             authentication. Defaults to None. Optional.
-        proxy: The address of a proxy server, which will be used for
-            HTTP and HTTPS traffic. If a port is not specified as part
-            of that address, it will be assumed from the protocol in the
-            URL, i.e. 80/443. Defaults to None. Optional.
-        cookie_policy: A string representing this client's cookie
+        proxy (str): The address of a proxy server, which will be used
+            for HTTP and HTTPS traffic. If a port is not specified as
+            part of that address, it will be assumed from the protocol
+            in the URL, i.e. 80/443. Defaults to None. Optional.
+        cookie_policy (str): A string representing this client's cookie
             policy. Accepts values "ACCEPT_ALL", "ACCEPT_NONE", and
             "ACCEPT_ORIGINAL_SERVER". Defaults to
             "ACCEPT_ORIGINAL_SERVER". Optional.
-        redirect_policy: A string representing this client's redirect
-            policy. Acceptable values are listed below. Defaults to
-            "Normal". Optional.
-        version: A string specifying either HTTP_2 or HTTP_1_1 for the
-            HTTP protocol. When omitted, the previous default of HTTP_2
-            is implied. Optional.
-        customizer: A reference to a function. This function will be
-            called with one argument (an instance of
+        redirect_policy (str): A string representing this client's
+            redirect policy. Acceptable values are listed below.
+            Defaults to "Normal". Optional.
+        customizer (object): A reference to a function. This function
+            will be called with one argument (an instance of
             HttpClient.Builder). The function should operate on that
             builder instance, which allows for customization of the
             created HTTP client. Defaults to None. Optional.
 
     Returns:
-        An object wrapped around an instance of Java's HttpClient class.
-        The httpClient object has methods that can be called to execute
-        HTTP requests against a server.
+        JythonHttpClient: An object wrapped around an instance of Java's
+            HttpClient class. The httpClient object has methods that can
+            be called to execute HTTP requests against a server.
     """
     print(
         timeout,
         bypass_cert_validation,
         username,
         password,
         proxy,
         cookie_policy,
         redirect_policy,
-        version,
         customizer,
     )
     return JythonHttpClient()
 
 
 def httpDelete(
-    url,  # type: AnyStr
-    contentType=None,  # type: Optional[AnyStr]
-    connectTimeout=10000,  # type: int
-    readTimeout=60000,  # type: int
-    username=None,  # type: Optional[AnyStr]
-    password=None,  # type: Optional[AnyStr]
-    headerValues=None,  # type: Optional[Dict[AnyStr, AnyStr]]
-    bypassCertValidation=True,  # type: bool
+    url,
+    contentType=None,
+    connectTimeout=10000,
+    readTimeout=60000,
+    username=None,
+    password=None,
+    headerValues=None,
+    bypassCertValidation=True,
 ):
-    # type: (...) -> AnyStr
     """Performs an HTTP DELETE to the given URL.
 
     Args:
-        url: The URL to send the request to.
-        contentType: The MIME type used in the HTTP 'Content-type'
+        url (str): The URL to send the request to.
+        contentType (str): The MIME type used in the HTTP 'Content-type'
             header. Optional.
-        connectTimeout: The timeout for connecting to the URL in
+        connectTimeout (int): The timeout for connecting to the URL in
             milliseconds. Default is 10,000. Optional.
-        readTimeout: The read timeout for the operation in
+        readTimeout (int): The read timeout for the operation in
             milliseconds. Default is 60,000. Optional.
-        username: If specified, the call will attempt to authenticate
-            with basic HTTP authentication. Optional.
-        password: The password used for basic HTTP authentication, if
-            the username parameter is also present. Optional.
-        headerValues: A dictionary of name/value pairs that will be set
-            in the HTTP header. Optional.
-        bypassCertValidation: If the target address in an HTTPS address,
-            and this parameter is TRUE, the system will bypass all SSL
-            certificate validation. This is not recommended, though is
-            sometimes necessary for self-signed certificates. Optional.
+        username (str): If specified, the call will attempt to
+            authenticate with basic HTTP authentication. Optional.
+        password (str): The password used for basic HTTP authentication,
+            if the username parameter is also present. Optional.
+        headerValues (dict): A dictionary of name/value pairs that will
+            be set in the HTTP header. Optional.
+        bypassCertValidation (bool): If the target address in an HTTPS
+            address, and this parameter is TRUE, the system will bypass
+            all SSL certificate validation. This is not recommended,
+            though is sometimes necessary for self-signed certificates.
+            Optional.
 
     Returns:
-        The content returned for the DELETE operation.
+        object: The content returned for the DELETE operation.
     """
     print(
         url,
         contentType,
         connectTimeout,
         readTimeout,
         username,
         password,
         headerValues,
         bypassCertValidation,
     )
-    return "DELETE"
+    return object
 
 
 def httpGet(
-    url,  # type: AnyStr
-    connectTimeout=10000,  # type: int
-    readTimeout=60000,  # type: int
-    username=None,  # type: Optional[AnyStr]
-    password=None,  # type: Optional[AnyStr]
-    headerValues=None,  # type: Optional[Dict[AnyStr, AnyStr]]
-    bypassCertValidation=None,  # type: Optional[bool]
-    useCaches=True,  # type: bool
-    throwOnError=True,  # type: bool
+    url,
+    connectTimeout=10000,
+    readTimeout=60000,
+    username=None,
+    password=None,
+    headerValues=None,
+    bypassCertValidation=None,
+    useCaches=True,
+    throwOnError=True,
 ):
-    # type: (...) -> AnyStr
     """Retrieves the document at the given URL using the HTTP GET
     protocol.
 
     The document is returned as a string. For example, if you use the
     URL of a website, you'll get the same thing you'd get by going to
     that website in a browser and using the browser's "View Source"
     function.
 
     Args:
-        url: The URL to retrieve.
-        connectTimeout: The timeout for connecting to the URL. In
+        url (str): The URL to retrieve.
+        connectTimeout (int): The timeout for connecting to the URL. In
             milliseconds. Default is 10,000. Optional.
-        readTimeout: The read timeout for the get operation. In
+        readTimeout (int): The read timeout for the get operation. In
             milliseconds. Default is 60,000. Optional.
-        username: If specified, the call will attempt to authenticate
-            with basic HTTP authentication. Optional.
-        password: The password used for basic HTTP authentication, if
-            the username parameter is also present. Optional.
-        headerValues: A dictionary of name/value pairs that will be set
-            in the HTTP header. Optional.
-        bypassCertValidation: If the target address is an HTTPS address,
-            and this parameter is True, the system will bypass all SSL
-            certificate validation. This is not recommended, though is
-            sometimes necessary for self-signed certificates. Optional.
-        useCaches: Will cache the information returned by the httpGet
-            call. If using this for something that constantly updates
-            like an rss feed, it would be better to set this to False.
-            Default is True. Optional.
-        throwOnError: Set to False if you wish to get the error body
-            rather than a Python exception if the GET request returns an
-            error code (non-200 responsive). Default is True. Optional.
+        username (str): If specified, the call will attempt to
+            authenticate with basic HTTP authentication. Optional.
+        password (str): The password used for basic HTTP authentication,
+            if the username parameter is also present. Optional.
+        headerValues (dict): A dictionary of name/value pairs that will
+            be set in the HTTP header. Optional.
+        bypassCertValidation (bool): If the target address is an HTTPS
+            address, and this parameter is True, the system will bypass
+            all SSL certificate validation. This is not recommended,
+            though is sometimes necessary for self-signed certificates.
+            Optional.
+        useCaches (bool): Will cache the information returned by the
+            httpGet call. If using this for something that constantly
+            updates like an rss feed, it would be better to set this to
+            False. Default is True. Optional.
+        throwOnError (bool): Set to False if you wish to get the error
+            body rather than a Python exception if the GET request
+            returns an error code (non-200 responsive). Default is True.
+            Optional.
 
     Returns:
-        The content found at the given URL.
+        str: The content found at the given URL.
     """
     print(
         url,
         connectTimeout,
         readTimeout,
         username,
         password,
@@ -271,210 +340,143 @@
         bypassCertValidation,
         useCaches,
         throwOnError,
     )
     return ""
 
 
-def httpPost(url, *args, **kwargs):
-    # type: (AnyStr, *Any, **Any) -> AnyStr
+def httpPost(url, *args):
     """Retrieves the document at the given URL using the HTTP POST
     protocol.
 
     If a parameter dictionary argument is specified, the entries in the
     dictionary will encoded in "application/x-www-form-urlencoded"
     format, and then posted. You can post arbitrary data as well, but
     you'll need to specify the MIME type. The document is then returned
     as a string.
 
     Args:
-        url: The URL to post to.
+        url (str): The URL to post to.
         *args: Variable length argument list.
-        **kwargs: Arbitrary keyword arguments.
 
     Returns:
-        The content returned for the POST operation.
+        str: The content returned for the POST operation.
     """
-    print(url, args, kwargs)
+    print(url, args)
     return ""
 
 
 def httpPut(url, *args, **kwargs):
-    # type: (AnyStr, *Any, **Any) -> AnyStr
     """Performs an HTTP PUT to the given URL.
 
     Encodes the given dictionary of parameters using
     "applications/x-www-form-urlencoded" format.
 
     Args:
-        url: The URL to put to.
+        url (str): The URL to send the request to.
         *args: Variable length argument list.
         **kwargs: Arbitrary keyword arguments.
 
     Returns:
-        The content returned by the PUT operation.
+        str: The content returned by the PUT operation.
     """
     print(url, args, kwargs)
     return ""
 
 
 def openURL(url, useApplet=False):
-    # type: (AnyStr, Optional[bool]) -> None
     """Opens the given URL or URI scheme outside of the currently
     running Client in whatever application the host operating system
     deems appropriate.
 
     Args:
-        url: The URL to open in a web browser.
-        useApplet: If set to True, and the client is running as an
-            Applet, then the browser instance that launched the applet
-            will be used to open the URL. Optional.
+        url (str): The URL to open in a web browser.
+        useApplet (bool): If set to True (1), and the client is running
+            as an Applet, then the browser instance that launched the
+            applet will be used to open the URL. Optional.
     """
     print(url, useApplet)
 
 
-def _sendEmail(
-    smtpSettings,  # type: Optional[AnyStr]
-    fromAddr,  # type: AnyStr
-    subject=None,  # type: Optional[AnyStr]
-    body=None,  # type: Optional[AnyStr]
-    html=False,  # type: bool
-    to=None,  # type: Optional[List[AnyStr]]
-    attachmentNames=None,  # type: Optional[List[object]]
-    attachmentData=None,  # type: Optional[List[object]]
-    timeout=300000,  # type: int
-    username=None,  # type: Optional[AnyStr]
-    password=None,  # type: Optional[AnyStr]
-    priority="3",  # type: AnyStr
-    cc=None,  # type: Optional[List[AnyStr]]
-    bcc=None,  # type: Optional[List[AnyStr]]
-    retries=0,  # type: int
-    replyTo=None,  # type: Optional[List[AnyStr]]
-):
-    # type: (...) -> None
-    _to = [] if to is None else to
-    _cc = [] if cc is None else cc
-    _bcc = [] if bcc is None else bcc
-    recipients = _to + _cc + _bcc
-    if smtpSettings and fromAddr and len(recipients) > 0:
-        print(
-            smtpSettings,
-            fromAddr,
-            subject,
-            body,
-            html,
-            to,
-            attachmentNames,
-            attachmentData,
-            timeout,
-            username,
-            password,
-            priority,
-            cc,
-            bcc,
-            retries,
-            replyTo,
-        )
-    else:
-        raise IllegalArgumentException(
-            "Cannot send email without SMTP host, from address and recipient list."
-        )
-
-
 def sendEmail(
-    smtp=None,  # type: Optional[AnyStr]
-    fromAddr="",  # type: AnyStr
-    subject=None,  # type: Optional[AnyStr]
-    body=None,  # type: Optional[AnyStr]
-    html=False,  # type: bool
-    to=None,  # type: Optional[List[AnyStr]]
-    attachmentNames=None,  # type: Optional[List[object]]
-    attachmentData=None,  # type: Optional[List[object]]
-    timeout=300000,  # type: int
-    username=None,  # type: Optional[AnyStr]
-    password=None,  # type: Optional[AnyStr]
-    priority="3",  # type: AnyStr
-    smtpProfile=None,  # type: Optional[AnyStr]
-    cc=None,  # type: Optional[List[AnyStr]]
-    bcc=None,  # type: Optional[List[AnyStr]]
-    retries=0,  # type: int
-    replyTo=None,  # type: Optional[List[AnyStr]]
+    smtp,
+    fromAddr,
+    subject,
+    body,
+    html,
+    to,
+    attachmentNames=None,
+    attachmentData=None,
+    timeout=300000,
+    username=None,
+    password=None,
+    priority="3",
+    smtpProfile=None,
+    cc=None,
+    bcc=None,
+    retries=0,
+    replyTo=None,
 ):
-    # type: (...) -> None
     """Sends an email through the given SMTP server.
 
     Note that this email is relayed first through the Gateway - the
     client host machine doesn't need network access to the SMTP server.
 
     Args:
-        smtp: The address of an SMTP server to send the email through,
-            like "mail.example.com". A port can be specified, like
-            "mail.example.com:25". SSL can also be forced, like
+        smtp (str): The address of an SMTP server to send the email
+            through, like "mail.example.com". A port can be specified,
+            like "mail.example.com:25". SSL can also be forced, like
             "mail.example.com:25:tls".
-        fromAddr: An email address to have the email come from.
-        subject: The subject line for the email. Optional.
-        body: The body text of the email. Optional.
-        html: A flag indicating whether or not to send the email as an
-            HTML email. Will auto-detect if omitted. Optional.
-        to: A list of email addresses to send to.
-        attachmentNames: A list of attachment names. Attachment names
-            must have the correct extension for the file type or an
-            error will occur. Optional.
-        attachmentData: A list of attachment data, in binary format.
-        timeout: A timeout for the email, specified in milliseconds.
-            Defaults to 5 minutes (60,000*5). Optional.
-        username: If specified, will be used to authenticate with the
-            SMTP host. Optional.
-        password: If specified, will be used to authenticate with the
-            SMTP host. Optional.
-        priority: Priority for the message, from "1" to "5", with "1"
-            being highest priority. Defaults to "3" (normal) priority.
-            Optional.
-        smtpProfile: If specified, the named SMTP profile defined
+        fromAddr (str): An email address to have the email come from.
+        subject (str): The subject line for the email.
+        body (str): The body text of the email.
+        html (bool): A flag indicating whether or not to send the email
+            as an HTML email. Will auto-detect if omitted.
+        to (list[str]): A list of email addresses to send to.
+        attachmentNames (list[str]): A list of attachment names.
+            Attachment names must have the correct extension for the
+            file type or an error will occur.
+        attachmentData (list[object]): A list of attachment data, in
+            binary format.
+        timeout (int): A timeout for the email, specified in
+            milliseconds. Defaults to 5 minutes (60,000*5). Optional.
+        username (str): If specified, will be used to authenticate with
+            the SMTP host. Optional.
+        password (str): If specified, will be used to authenticate with
+            the SMTP host. Optional.
+        priority (str): Priority for the message, from "1" to "5", with
+            "1" being highest priority. Defaults to "3" (normal)
+            priority. Optional.
+        smtpProfile (str): If specified, the named SMTP profile defined
             in the Gateway will be used. If this keyword is present, the
             smtp, username, and password keywords will be ignored.
             Optional.
-        cc: A list of email addresses to carbon copy. Only available if
-            a smtpProfile is used. Optional.
-        bcc: A list of email addresses to blind carbon copy. Only
+        cc (list[str]): A list of email addresses to carbon copy. Only
             available if a smtpProfile is used. Optional.
-        retries: The number of additional times to retry sending on
-            failure. Defaults to 0. Only available if a smtpProfile is
-            used. Optional.
-        replyTo: An optional list of addresses to have the recipients
-            reply to. If omitted, this defaults to the from address.
-            Optional.
+        bcc (list[str]): A list of email addresses to blind carbon copy.
+            Only available if a smtpProfile is used. Optional.
+        retries (int): The number of additional times to retry sending
+            on failure. Defaults to 0. Only available if a smtpProfile
+            is used. Optional.
+        replyTo (list[str]): An optional list of addresses to have the
+            recipients reply to. If omitted, this defaults to the from
+            address. Optional.
     """
-    if not smtpProfile:
-        _sendEmail(
-            smtp,
-            fromAddr,
-            subject,
-            body,
-            html,
-            to,
-            attachmentNames,
-            attachmentData,
-            timeout,
-            username,
-            password,
-            priority,
-            retries=retries,
-            replyTo=replyTo,
-        )
-    else:
-        _sendEmail(
-            smtpProfile,
-            fromAddr,
-            subject,
-            body,
-            html,
-            to,
-            attachmentNames,
-            attachmentData,
-            timeout,
-            priority=priority,
-            cc=cc,
-            bcc=bcc,
-            retries=retries,
-            replyTo=replyTo,
-        )
+    print(
+        smtp,
+        fromAddr,
+        subject,
+        body,
+        html,
+        to,
+        attachmentNames,
+        attachmentData,
+        timeout,
+        username,
+        password,
+        priority,
+        smtpProfile,
+        cc,
+        bcc,
+        retries,
+        replyTo,
+    )
```

### Comparing `ignition_api-8.1.40/src/system/gui.py` & `ignition-api-8.1.9/src/system/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """GUI Functions.
 
 The following functions allow you to control windows and create popup
 interfaces.
 """
 
 from __future__ import print_function
 
 __all__ = [
-    "ACCL_CONSTANT",
-    "ACCL_EASE",
-    "ACCL_FAST_TO_SLOW",
-    "ACCL_NONE",
-    "ACCL_SLOW_TO_FAST",
-    "COORD_DESIGNER",
-    "COORD_SCREEN",
     "chooseColor",
     "closeDesktop",
     "color",
     "confirm",
     "convertPointToScreen",
     "createPopupMenu",
     "desktop",
@@ -44,105 +41,151 @@
     "setTouchscreenModeEnabled",
     "showNumericKeypad",
     "showTouchscreenKeyboard",
     "transform",
     "warningBox",
 ]
 
-from typing import Any, Callable, List, Optional, Tuple
-
-from com.inductiveautomation.factorypmi.application import FPMIWindow
-from com.inductiveautomation.factorypmi.application.script.builtin import (
-    WindowUtilities,
-)
-from dev.coatl.helper.types import AnyNum, AnyStr
 from java.awt import Color
-from java.org.jdesktop.core.animation.timing import Animator
+from java.lang import Object
 from java.util import EventObject
 from javax.swing import (
     JComponent,
     JFrame,
+    JInternalFrame,
     JLabel,
     JOptionPane,
     JPanel,
     JPopupMenu,
     JTextField,
 )
 
 # Constants
 ACCL_NONE = 0
 ACCL_CONSTANT = 1
 ACCL_FAST_TO_SLOW = 2
 ACCL_SLOW_TO_FAST = 3
 ACCL_EASE = 4
-COORD_DESIGNER = 1
 COORD_SCREEN = 0
+COORD_DESIGNER = 1
+
+
+class FPMIWindow(JInternalFrame):
+    """FPMIWindow object."""
+
+    # Fields.
+    CACHE_ALWAYS = 2
+    CACHE_AUTO = 0
+    CACHE_NEVER = 1
+    DOCK_EAST = 2
+    DOCK_FLOAT = 0
+    DOCK_NORTH = 2
+    DOCK_SOUTH = 4
+    DOCK_WEST = 3
+    PARENT_WINDOW_NAME = "_parent"
+    SHOW_ALWAYS = 0
+    SHOW_NEVER = 1
+    SHOW_MAXIMIZED = 2
+
+    _path = "Path/To/Window"
+
+    def __init__(self, name):
+        self.name = name
+
+    def getPath(self):
+        return self._path
+
+    def getRootContainer(self):
+        print(self)
+
+
+class WindowUtilities(Object):
+    """WindowUtilities object."""
+
+    def confirm(self, *args):
+        pass
+
+    def errorBox(self, *args):
+        pass
+
+    def inputBox(self, *args):
+        pass
+
+    def messageBox(self, *args):
+        pass
+
+    def passwordBox(self, *args):
+        pass
+
+    def warningBox(self, *args):
+        pass
+
+
+def _dummy(message, title):
+    print(message, title)
 
 
 def chooseColor(initialColor, dialogTitle="Choose Color"):
-    # type: (Color, AnyStr) -> Color
     """Prompts the user to pick a color using the default color-chooser
     dialog box.
 
     Args:
-        initialColor: A color to use as a starting point in the color
-            choosing popup.
-        dialogTitle: The title for the color choosing popup. Defaults to
-            "Choose Color". Optional.
+        initialColor (Color): A color to use as a starting point in the
+            color choosing popup.
+        dialogTitle (str): The title for the color choosing popup.
+            Defaults to "Choose Color". Optional.
 
     Returns:
-        The new color chosen by the user.
+        Color: The new color chosen by the user.
     """
     print(initialColor, dialogTitle)
     return Color()
 
 
-def closeDesktop(handle):
-    # type: (AnyStr) -> None
+def closeDesktop(handle="primary"):
     """Allows you to close any of the open desktops associated with the
     current client.
 
     Args:
-        handle: The handle for the desktop to close. The screen index
-            cast as a string may be used instead of the handle. If
+        handle (str): The handle for the desktop to close. The screen
+            index cast as a string may be used instead of the handle. If
             omitted, this will default to the Primary Desktop.
             Alternatively, the handle "primary" can be used to refer to
             the Primary Desktop.
     """
     print(handle)
 
 
 def color(*args):
-    # type: (*Any) -> Color
     """Creates a new color object, either by parsing a string or by
-    having the RGB[A] channels specified explicitly.
+    having the RGB[A] channels specified explicitly. See toColor to see
+    a list of available color names.
 
     Args:
         args: Variable-length argument list.
 
     Returns:
-        The newly created color.
+        Color: The newly created color.
     """
     print(args)
-    return Color(*args)
 
 
 def confirm(message, title="Confirm", allowCancel=False):
-    # type: (AnyStr, AnyStr, bool) -> Optional[bool]
     """Displays a confirmation dialog box to the user with "Yes", "No"
-    options, and a custom message.
+    and "Cancel" options, and a custom message.
 
     Args:
-        message: The message to show in the confirmation dialog.
-        title: The title for the confirmation dialog. Optional.
-        allowCancel: Show a cancel button in the dialog. Optional.
+        message (str): The message to show in the confirmation dialog.
+        title (str): The title for the confirmation dialog. Optional.
+        allowCancel (bool): Show a cancel button in the dialog.
+            Optional.
 
     Returns:
-        True if the user selected "Yes", False if the user
-        selected "No", None if the user selected "Cancel".
+        bool: True (1) if the user selected "Yes", False (0) if the user
+            selected "No", None if the user selected "Cancel".
     """
     options = ["Yes", "No"]
 
     if allowCancel:
         options.append("Cancel")
 
     choice = JOptionPane.showOptionDialog(
@@ -160,279 +203,271 @@
         not bool(choice)
         if choice in [JOptionPane.YES_OPTION, JOptionPane.NO_OPTION]
         else None
     )
 
 
 def convertPointToScreen(x, y, event):
-    # type: (int, int, EventObject) -> Tuple[int, int]
-    """Converts a pair of coordinates that are relative to the upper-
-    left corner of some component to be relative to the upper-left
+    """Converts a pair of coordinates that are relative to the
+    upper-left corner of some component to be relative to the upper-left
     corner of the entire screen.
 
     Args:
-        x: The X-coordinate, relative to the component that fired the
-            event.
-        y: The Y-coordinate, relative to the component that fired the
-            event.
-        event: An event object for a component event.
+        x (int): The X-coordinate, relative to the component that fired
+            the event.
+        y (int): The Y-coordinate, relative to the component that fired
+            the event.
+        event (EventObject): An event object for a component event.
 
     Returns:
-        A tuple of (x,y) in screen coordinates.
+        tuple: A tuple of (x,y) in screen coordinates.
     """
     print(x, y, event)
     return x, y
 
 
 def createPopupMenu(itemNames, itemFunctions):
-    # type: (List[AnyStr], List[Callable[..., Any]]) -> JPopupMenu
     """Creates a new popup menu, which can then be shown over a
     component on a mouse event.
 
     Args:
-        itemNames: A list of names to create popup menu items with.
-        itemFunctions: A list of functions to match up with the names.
+        itemNames (list[str]): A list of names to create popup menu
+            items with.
+        itemFunctions (list[object]): A list of functions to match up
+            with the names.
 
     Returns:
-        The javax.swing.JPopupMenu that was created.
+        JPopupMenu: The javax.swing.JPopupMenu that was created.
     """
     print(itemNames, itemFunctions)
     return JPopupMenu()
 
 
-def desktop(handle):
-    # type: (AnyStr) -> WindowUtilities
+def desktop(handle="primary"):
     """Allows for invoking system.gui functions on a specific desktop.
 
     Args:
-        handle: The handle for the desktop to use. The screen index cast
-            as a string may be used instead of the handle. If omitted,
-            this will default to the Primary Desktop. Alternatively, the
-            handle "primary" can be used to refer to the primary
-            desktop.
+        handle (str): The handle for the desktop to use. The screen
+            index cast as a string may be used instead of the handle. If
+            omitted, this will default to the Primary Desktop.
+            Alternatively, the handle "primary" can be used to refer to
+            the Primary Desktop.
 
     Returns:
-        A copy of system.gui that will be relative to the desktop named
-        by the given handle.
+        WindowUtilities: A copy of system.gui that will be relative to
+            the desktop named by the given handle.
     """
     print(handle)
     return WindowUtilities()
 
 
 def errorBox(message, title="Error"):
-    # type: (AnyStr, AnyStr) -> None
     """Displays an error-style message box to the user.
 
     Args:
-        message: The message to display in an error box.
-        title: The title for the error box. Optional.
+        message (str): The message to display in an error box.
+        title (str): The title for the error box. Optional.
     """
-    JOptionPane.showMessageDialog(None, message, title, JOptionPane.ERROR_MESSAGE)
+    JOptionPane.showMessageDialog(
+        None, message, title, JOptionPane.ERROR_MESSAGE
+    )
 
 
 def findWindow(path):
-    # type: (AnyStr) -> List[FPMIWindow]
     """Finds and returns a list of windows with the given path.
 
     If the window is not open, an empty list will be returned. Useful
     for finding all instances of an open window that were opened with
     system.gui.openWindowInstance.
 
     Args:
-        path: The path of the window to search for.
+        path (str): The path of the window to search for.
 
     Returns:
-        A list of window objects. May be empty if window is not open, or
-        have more than one entry if multiple windows are open.
+        list[object]: A list of window objects. May be empty if window
+            is not open, or have more than one entry if multiple windows
+            are open.
     """
     print(path)
-    return [FPMIWindow("Window")]
+    return []
 
 
 def getCurrentDesktop():
-    # type: () -> AnyStr
     """Returns the handle of the desktop this function was called from.
 
     Commonly used with the system.gui.desktop and system.nav.desktop
     functions.
 
     Returns:
-        The handle of the current desktop.
+        str: The handle of the current desktop.
     """
     return "primary"
 
 
 def getDesktopHandles():
-    # type: () -> List[AnyStr]
     """Gets a list of all secondary handles of the open desktops
     associated with the current client.
 
     In this case, secondary means any desktop frame opened by the
     original client frame.
 
     Example:
         If the original client opened 2 new frames ('left client' and
         'right client'), then this function would return ['left client',
         'right client'].
 
     Returns:
-        A list of window handles of all secondary Desktop frames.
+        list[str]: A list of window handles of all secondary Desktop
+            frames.
     """
     return ["left client", "right client"]
 
 
 def getOpenedWindowNames():
-    # type: () -> Tuple[AnyStr, ...]
-    """Finds all of the currently open windows and returns a tuple of
+    """Finds all of the currently open windows, returning a tuple of
     their paths.
 
     Returns:
-        A tuple of strings, representing the path of each window that is
-        open.
+        tuple: A tuple of strings, representing the path of each window
+            that is open.
     """
     return "window_1", "window_2", "window_n"
 
 
 def getOpenedWindows():
-    # type: () -> Tuple[FPMIWindow, ...]
     """Finds all of the currently open windows, returning a tuple of
     references to them.
 
     Returns:
-         A tuple of the opened windows. Not their names, but the actual
-         window objects themselves.
+         tuple: A tuple of the opened windows. Not their names, but the
+            actual window objects themselves.
     """
-    return FPMIWindow("Main Window"), FPMIWindow("Other Window")
+    return [FPMIWindow("Main Window")]
 
 
 def getParentWindow(event):
-    # type: (EventObject) -> FPMIWindow
     """Finds the parent (enclosing) window for the component that fired
     an event, returning a reference to it.
 
     Args:
-        A component event object.
+        event (EventObject): A component event object.
 
     Returns:
-        The window that contains the component that fired the event.
+        object: The window that contains the component that fired the
+            event.
     """
     print(event)
-    return FPMIWindow("Parent Window")
+    return object
 
 
 def getQuality(component, propertyName):
-    # type: (JComponent, AnyStr) -> int
     """Returns the data quality for the property of the given component
     as an integer.
 
     This function can be used to check the quality of a Tag binding on a
     component in the middle of the script so that alternative actions
     can be taken in the event of device disconnections.
 
     Args:
-        component: The component whose property is being checked.
-        propertyName: The name of the property as a string value.
+        component (JComponent): The component whose property is being
+            checked.
+        propertyName (str): The name of the property as a string value.
 
     Returns:
-        The data quality of the given property as an integer.
+        int: The data quality of the given property as an integer.
     """
     print(component, propertyName)
     return 192
 
 
 def getScreenIndex():
-    # type: () -> int
     """Returns the returns an integer value representing the current
-    screen index based on the screen from which this function was
-    called.
+    screen index based on the screen this function was called from.
 
     Returns:
-        The screen from which the function was called.
+        int: The screen that the function was called from.
     """
     return 0
 
 
 def getScreens():
-    # type: () -> List[Tuple[AnyStr, int, int]]
     """Get a list of all the monitors on the computer this client is
     open on.
 
     Use with system.gui.setScreenIndex() to move the client.
 
     Returns:
-        A sequence of tuples of the form (index, width, height) for each
-        screen device (monitor) available.
+        list[tuple]: A sequence of tuples of the form (index, width,
+            height) for each screen device (monitor) available.
     """
-    return [("primary", 1440, 900), ("secondary", 1920, 1080)]
+    return [(0, 1024, 768), (1, 3840, 2160)]
 
 
 def getSibling(event, name):
-    # type: (EventObject, AnyStr) -> FPMIWindow
     """Given a component event object, looks up a sibling component.
 
     Shortcut for event.source.parent.getComponent("siblingName"). If no
     such sibling is found, the special value None is returned.
 
     Args:
-        event: A component event object.
-        name: The name of the sibling component.
+        event (EventObject): A component event object.
+        name (str): The name of the sibling component.
 
     Returns:
-        The sibling component itself.
+        object: The sibling component itself.
     """
     print(event, name)
     return FPMIWindow("Sibling")
 
 
 def getWindow(name):
-    # type: (AnyStr) -> FPMIWindow
     """Finds a reference to an open window with the given name.
 
     Throws a ValueError if the named window is not open or not found.
 
     Args:
-        name: The path to the window to field.
+        name (str): The path to the window to field.
 
     Returns:
-        A reference to the window, if it was open.
+        FPMIWindow: A reference to the window, if it was open. Use
+            .getRootContainer() to grab the root container of the
+            window.
     """
     print(name)
     return FPMIWindow("Main Window")
 
 
 def getWindowNames():
-    # type: () -> Tuple[AnyStr, ...]
     """Returns a list of the paths of all windows in the current
     project, sorted alphabetically.
 
     Returns:
-        A tuple of strings, representing the path of each window defined
-        in the current project.
+        tuple[str]: A tuple of strings, representing the path of each
+            window defined in the current project.
     """
     return "Main Window", "Main Window 1", "Main Window 2"
 
 
-def inputBox(message, defaultText=""):
-    # type: (AnyStr, AnyStr) -> Optional[AnyStr]
+def inputBox(message, defaultText=None):
     """Opens up a popup input dialog box.
 
     This dialog box will show a prompt message, and allow the user to
     type in a string. When the user is done, they can press "OK" or
     "Cancel". If OK is pressed, this function will return with the value
     that they typed in. If Cancel is pressed, this function will return
     the value None.
 
     Args:
-        message: The message to display for the input box. Will accept
-            HTML formatting.
-        defaultText: The default text to initialize the input box with.
-            Optional.
+        message (str): The message to display for the input box. Will
+            accept html formatting.
+        defaultText (str): The default text to initialize the input box
+            with. Optional.
 
     Returns:
-        The string value that was entered in the input box.
+        str: The string value that was entered in the input box.
     """
     options = ["OK", "Cancel"]
 
     panel = JPanel()
     label = JLabel("{}: ".format(message))
     panel.add(label)
     text_field = JTextField(25)
@@ -450,254 +485,246 @@
         options[0],
     )
 
     return text_field.getText() if choice == JOptionPane.OK_OPTION else None
 
 
 def isTouchscreenModeEnabled():
-    # type: () -> bool
     """Checks whether or not the running client's touchscreen mode is
     currently enabled.
 
     Returns:
-         True if the Client currently has Touch Screen mode activated.
+         bool: True(1) if the client currently has touchscreen mode
+            activated.
     """
     return False
 
 
 def messageBox(message, title="Information"):
-    # type: (AnyStr, AnyStr) -> None
     """Displays an informational-style message popup box to the user.
 
     Args:
-        message: The message to display. Will accept HTML formatting.
-        title: The title for the message box. Optional.
+        message (str): The message to display. Will accept html
+            formatting.
+        title (str): The title for the message box. Optional.
     """
-    JOptionPane.showMessageDialog(None, message, title, JOptionPane.INFORMATION_MESSAGE)
+    JOptionPane.showMessageDialog(
+        None, message, title, JOptionPane.INFORMATION_MESSAGE
+    )
 
 
 def openDesktop(
-    screen=0,  # type: int
-    handle=None,  # type: Optional[AnyStr]
-    title=None,  # type: Optional[AnyStr]
-    width=None,  # type: Optional[int]
-    height=None,  # type: Optional[int]
-    x=0,  # type: int
-    y=0,  # type: int
-    windows=None,  # type: Optional[List[AnyStr]]
+    screen=0,
+    handle=None,
+    title=None,
+    width=None,
+    height=None,
+    x=0,
+    y=0,
+    windows=None,
 ):
-    # type: (...) -> JFrame
     """Creates an additional Desktop in a new frame.
 
     Args:
-        screen: The screen index of which screen to place the new frame
-            on. If omitted, screen 0 will be used. Optional.
-        handle: A name for the desktop. If omitted, the screen index
-            will be used. Optional.
-        title: The title for the new frame. If omitted, the index handle
-            will be used. If the handle and title are omitted, the
-            screen index will be used. Optional.
-        width: The width for the new Desktop's frame. If omitted, frame
-            will become maximized on the specified monitor. Optional.
-        height: The width for the new desktop's frame. If omitted, frame
-            will become maximized on the specified monitor. Optional.
-        x: The X coordinate for the new desktop's frame. Only used if
-            both width and height are specified. If omitted, defaults to
-            0. Optional.
-        y: The Y coordinate for the new desktop's frame. Only used if
-            both width and height are specified. If omitted, defaults to
-            0. Optional.
-        windows: A list of window paths to open in the new Desktop
-            frame. If omitted, the desktop will open without any opened
-            windows. Optional.
+        screen (int): The screen index of which screen to place the new
+            frame on. If omitted, screen 0 will be used.
+        handle (str): A name for the desktop. If omitted, the screen
+            index will be used.
+        title (str): The title for the new frame. If omitted, the index
+            handle will be used. If the handle and title are omitted,
+            the screen index will be used.
+        width (int): The width for the new Desktop's frame. If omitted,
+            frame will become maximized on the specified monitor.
+        height (int): The width for the new desktop's frame. If omitted,
+            frame will become maximized on the specified monitor.
+        x (int): The X coordinate for the new desktop's frame. Only used
+            if both width and height are specified. If omitted, defaults
+            to 0.
+        y (int): The Y coordinate for the new desktop's frame. Only used
+            if both width and height are specified. If omitted, defaults
+            to 0.
+        windows (list[str]): A list of window paths to open in the new
+            Desktop frame.
 
     Returns:
-        A reference to the new Desktop frame object.
+        JFrame: A reference to the new Desktop frame.
     """
     print(screen, handle, title, width, height, x, y, windows)
     return JFrame()
 
 
 def openDiagnostics():
-    # type: () -> None
     """Opens the client runtime diagnostics window, which provides
     information regarding performance, logging, active threads,
     connection status, and the console.
 
     This provides an opportunity to open the diagnostics window in
     situations where the menu bar in the client is hidden, and the
     keyboard shortcut can not be used.
     """
     pass
 
 
-def passwordBox(
-    message,  # type:AnyStr
-    title="Password",  # type: AnyStr
-    echoChar="*",  # type: AnyStr
-):
-    # type: (...) -> Optional[AnyStr]
+def passwordBox(message, title="Password", echoChar="*"):
     """Pops up a special input box that uses a password field, so the
     text isn't echoed back in clear-text to the user.
 
     Returns the text they entered, or None if they canceled the dialog
     box.
 
     Args:
-        message: The message for the password prompt. Will accept HTML
-            formatting.
-        title: A title for the password prompt. Optional.
-        echoChar: A custom echo character. Defaults to: *. Optional.
+        message (str): The message for the password prompt. Will accept
+            html formatting.
+        title (str): A title for the password prompt. Optional.
+        echoChar (str): A custom echo character. Defaults to: *.
+            Optional.
 
     Returns:
-        The password that was entered, or None if the prompt was
-        canceled.
+        str: The password that was entered, or None if the prompt was
+            canceled.
     """
     print(message, title, echoChar)
     return "password"
 
 
 def setScreenIndex(index):
-    # type: (int) -> None
     """Moves an open client to a specific monitor.
 
     Use with system.gui.getScreens() to identify monitors before moving.
 
     Args:
-        index: The new monitor index for this client to move to. 0
+        index (int): The new monitor index for this client to move to. 0
             based.
     """
     print(index)
 
 
 def setTouchscreenModeEnabled(enabled):
-    # type: (bool) -> None
-    """Alters a running Client's Touch Screen mode on the fly.
+    """Alters a running client's touchscreen mode on the fly.
 
     Args:
-        enabled: The new value for Touch Screen mode being enabled.
+        enabled (bool): The new value for touchscreen mode being
+            enabled.
     """
     print(enabled)
 
 
-def showNumericKeypad(
-    initialValue,  # type: AnyNum
-    fontSize=None,  # type: Optional[int]
-    usePasswordMode=False,  # type: bool
-):
-    # type: (...) -> AnyNum
+def showNumericKeypad(initialValue=None, fontSize=None, usePasswordMode=False):
     """Displays a modal on-screen numeric keypad, allowing for arbitrary
     numeric entry using the mouse, or a finger on a touchscreen monitor.
 
     Returns the number that the user entered.
 
     Args:
-        initialValue: The value to start the on-screen keypad with.
-        fontSize: The font size to display in the keypad. Optional.
-        usePasswordMode: If True, display a * for each digit. Optional.
+        initialValue (object): The value to start the on-screen keypad
+            with.
+        fontSize (int): The font size to display in the keypad.
+            Optional.
+        usePasswordMode (bool): If True, display a * for each digit.
+            Optional.
 
     Returns:
-        The value that was entered in the keypad.
+        object: The value that was entered in the keypad.
     """
     print(initialValue, fontSize, usePasswordMode)
     return 43
 
 
-def showTouchscreenKeyboard(initialText, fontSize=None, passwordMode=False):
-    # type: (AnyStr, Optional[int], Optional[bool]) -> AnyStr
+def showTouchscreenKeyboard(
+    initialText=None, fontSize=None, passwordMode=False
+):
     """Displays a modal on-screen keyboard, allowing for arbitrary text
     entry using the mouse, or a finger on a touchscreen monitor.
 
-    Returns the text that the user entered.
+    Returns the text that the user "typed".
 
     Args:
         initialText: The text to start the on-screen keyboard with.
-        fontSize: The font size to display in the keypad. Optional.
-        passwordMode: True to activate password mode, where the text
-            entered isn't echoed back clear-text. Optional.
+        fontSize (int): The font size to display in the keypad.
+            Optional.
+        passwordMode (bool): True (1) to activate password mode, where
+            the text entered isn't echoed back clear-text. Optional.
 
     Returns:
-        The text that was entered in the on-screen keyboard.
+        str: The text that was "typed" in the on-screen keyboard.
     """
     print(initialText, fontSize, passwordMode)
     return ""
 
 
 def transform(
-    component,  # type: JComponent
-    newX=None,  # type: Optional[int]
-    newY=None,  # type: Optional[int]
-    newWidth=None,  # type: Optional[int]
-    newHeight=None,  # type: Optional[int]
-    duration=0,  # type: int
-    callback=None,  # type: Optional[Callable[..., Any]]
-    framesPerSecond=60,  # type: int
-    acceleration=None,  # type: Optional[int]
-    coordSpace=None,  # type: Optional[int]
+    component,
+    newX=None,
+    newY=None,
+    newWidth=None,
+    newHeight=None,
+    duration=0,
+    callback=None,
+    framesPerSecond=60,
+    acceleration=None,
+    coordSpace=None,
 ):
-    # type: (...) -> Animator
     """Sets a component's position and size at runtime.
 
     Additional arguments for the duration, framesPerSecond, and
     acceleration of the operation exist for animation. An optional
     callback argument will be executed when the transformation is
     complete.
 
-    Note:
-        The transformation is performed in Designer coordinate space on
-        components which are centered or have more than two anchors.
+    Note: The transformation is performed in Designer coordinate space
+    on components which are centered or have more than 2 anchors.
 
     Args:
-        component: The component to move or resize.
-        newX: An optional x-coordinate to move to, relative to the
+        component (JComponent): The component to move or resize.
+        newX (int): An optional x-coordinate to move to, relative to the
             upper-left corner of the component's parent container.
-        newY: An optional y-coordinate to move to, relative to the
+        newY (int): An optional y-coordinate to move to, relative to the
             upper-left corner of the component's parent container.
-        newWidth: An optional width for the component.
-        newHeight: An optional height for the component.
-        duration: An optional duration over which the transformation
-            will take place. If omitted or 0, the transform will take
-            place immediately.
-        callback: An optional function to be called when the
+        newWidth (int): An optional width for the component.
+        newHeight (int):An optional height for the component.
+        duration (int): An optional duration over which the
+            transformation will take place. If omitted or 0, the
+            transform will take place immediately.
+        callback (object): An optional function to be called when the
             transformation is complete.
-        framesPerSecond: An optional frame rate argument which dictates
-            how often the transformation updates over the given
+        framesPerSecond (int): An optional frame rate argument which
+            dictates how often the transformation updates over the given
             duration. The default is 60 frames per second.
-        acceleration: An optional modifier to the acceleration of the
-            transformation over the given duration. See system.gui
+        acceleration (int): An optional modifier to the acceleration of
+            the transformation over the given duration. See system.gui
             constants for valid arguments.
-        coordSpace: The coordinate space to use. When the default Screen
-            Coordinates are used, the given size and position are
+        coordSpace (int): The coordinate space to use. When the default
+            Screen Coordinates are used, the given size and position are
             absolute, as they appear in the client at runtime. When
             Designer Coordinates are used, the given size and position
             are pre-runtime adjusted values, as they would appear in the
             Designer. See system.gui constants for valid arguments.
 
     Returns:
-        An object that contains pause(), resume(), and cancel() methods,
-        allowing for a script to interrupt the animation.
+        object: An animation object that the script can use to pause(),
+            resume(), or cancel() the transformation.
     """
     print(
         component,
         newX,
         newY,
         newWidth,
         newHeight,
         duration,
         callback,
         framesPerSecond,
         acceleration,
         coordSpace,
     )
-    return Animator()
 
 
 def warningBox(message, title="Warning"):
-    # type: (AnyStr, AnyStr) -> None
-    """Displays a message to the user in a warning style popup dialog.
+    """Displays a message to the user in a warning style pop-up dialog.
 
     Args:
-        message: The message to display in the warning box. Will accept
-            HTML formatting.
-        title: The title for the warning box. Optional.
+        message (str): The message to display in the warning box. Will
+            accept html formatting.
+        title (str): The title for the warning box. Optional.
     """
-    JOptionPane.showMessageDialog(None, message, title, JOptionPane.WARNING_MESSAGE)
+    JOptionPane.showMessageDialog(
+        None, message, title, JOptionPane.WARNING_MESSAGE
+    )
```

### Comparing `ignition_api-8.1.40/src/system/dnp3.py` & `ignition-api-8.1.9/src/system/dnp3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,190 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """DNP3 Functions.
 
 The following functions give you access to interact with the DNP3
 devices.
 """
 
-from __future__ import print_function
-
 __all__ = [
-    "CLOSE",
-    "LATCH_OFF",
-    "LATCH_ON",
-    "NUL",
-    "PULSE_OFF",
-    "PULSE_ON",
-    "TRIP",
     "directOperateAnalog",
     "directOperateBinary",
     "freezeAnalogs",
     "freezeAnalogsAtTime",
     "freezeCounters",
     "freezeCountersAtTime",
     "selectOperateAnalog",
     "selectOperateBinary",
 ]
 
-from typing import List, Optional
-
-from dev.coatl.helper.types import AnyNum, AnyStr
-
 # Constants
 NUL = 0
 PULSE_ON = 1
 PULSE_OFF = 2
 LATCH_ON = 3
 LATCH_OFF = 4
 CLOSE = 1
 TRIP = 2
 
 
-def directOperateAnalog(
-    deviceName,  # type: AnyStr
-    index,  # type: int
-    value,  # type: AnyNum
-    variation=None,  # type: Optional[int]
-):
-    # type: (...) -> int
+def directOperateAnalog(deviceName, index, value, variation=None):
     """Issues a Select-And-Operate command to set an analog value in an
     analog output point.
 
     Args:
-        deviceName: The name of the DNP3 device driver.
-        index: The index of the object to be modified in the outstation.
-        value: The analog value that is requested (of type int, short,
-            float, or double).
-        variation: The DNP3 object variation to use in the request.
-            Optional.
+        deviceName (str): The name of the DNP3 device driver.
+        index (int): The index of the object to be modified in the
+            outstation.
+        value (object): The analog value that is requested (of type int,
+            short, float, or double).
+        variation (int): The DNP3 object variation to use in the
+            request. Optional.
 
     Returns:
-        The DNP3 status code of the response, as an integer.
+        int: The DNP3 status code of the response, as an integer.
     """
     print(deviceName, index, value, variation)
     return 0
 
 
 def directOperateBinary(
-    deviceName,  # type: AnyStr
-    indexes,  # type: List[int]
-    opType,  # type: int
-    tcCode=None,  # type: Optional[int]
-    count=None,  # type: Optional[int]
-    onTime=None,  # type: Optional[int]
-    offTime=None,  # type: Optional[int]
+    deviceName,
+    indexes,
+    opType,
+    tcCode=None,
+    count=None,
+    onTime=None,
+    offTime=None,
 ):
-    # type: (...) -> int
     """Issues a Direct-Operate command for digital control operations at
     binary output points (CROB).
 
     Args:
-        deviceName: The name of the DNP3 device driver.
-        indexes: A list of indexes of the objects to be modified in the
-            outstation.
-        opType: The type of the operation. 0=NUL, 1=PULSE_ON,
+        deviceName (str): The name of the DNP3 device driver.
+        indexes (list[object]): A list of indexes of the objects to be
+            modified in the outstation.
+        opType (int): The type of the operation. 0=NUL, 1=PULSE_ON,
             2=PULSE_OFF, 3=LATCH_ON, 4=LATCH_OFF.
-        tcCode: The Trip-Close code, used in conjunction with the
+        tcCode (int): The Trip-Close code, used in conjunction with the
             opType. 0=NUL, 1=CLOSE, 2=TRIP. Optional.
-        count: The number of times the outstation shall execute the
-            operation. Optional.
-        onTime: The duration that the output drive remains active, in
-            millis. Optional.
-        offTime: The duration that the output drive remains non-active,
-            in millis. Optional.
+        count (int): The number of times the outstation shall execute
+            the operation. Optional.
+        onTime (long): The duration that the output drive remains
+            active, in millis. Optional.
+        offTime (long): The duration that the output drive remains
+            non-active, in millis. Optional.
 
     Returns:
-        The DNP3 status code of the response, as an integer.
+        int: The DNP3 status code of the response, as an integer.
     """
     print(deviceName, indexes, opType, tcCode, count, onTime, offTime)
     return 0
 
 
-def freezeAnalogs(deviceName, indexes):
-    # type: (AnyStr, List[int]) -> None
+def freezeAnalogs(deviceName, indexes=None):
     """Issues a freeze command on the given analog outputs.
 
     Args:
-        deviceName: The name of the DNP3 device driver.
-        indexes: An optional list of specific indexes on which to issue
-            the freeze command. An empty list can be passed to freeze
-            all analogs.
+        deviceName (str): The name of the DNP3 device driver.
+        indexes (list[object]): An optional list of specific indexes on
+            which to issue the freeze command.
     """
     print(deviceName, indexes)
 
 
-def freezeAnalogsAtTime(deviceName, absoluteTime, intervalTime, indexes):
-    # type: (AnyStr, int, int, List[int]) -> None
+def freezeAnalogsAtTime(deviceName, absoluteTime, intervalTime, indexes=None):
     """Issues a freeze command on the given analog outputs at the given
     time for the specified duration.
 
     Args:
-        deviceName: The name of the DNP3 device driver.
-        absoluteTime: The absolute time at which to freeze, in millis.
-        intervalTime: The interval at which to periodically freeze, in
+        deviceName (str): The name of the DNP3 device driver.
+        absoluteTime (int): The absolute time at which to freeze, in
             millis.
-        indexes: An optional list of specific indexes on which to issue
-            the freeze command. An empty list will freeze all points.
+        intervalTime (int): The interval at which to periodically
+            freeze, in millis.
+        indexes (list[object]): An optional list of specific indexes on
+            which to issue the freeze command. Optional.
     """
     print(deviceName, absoluteTime, intervalTime, indexes)
 
 
-def freezeCounters(deviceName, indexes):
-    # type: (AnyStr, List[int]) -> None
+def freezeCounters(deviceName, indexes=None):
     """Issues a freeze command on the given counters.
 
     Args:
-        deviceName: The name of the DNP3 device driver.
-        indexes: An optional list of specific indexes on which to issue
-            the freeze command. An empty list can be passed to freeze
-            all counters.
+        deviceName (str): The name of the DNP3 device driver.
+        indexes (list[object]): An optional list of specific indexes on
+            which to issue the freeze command. Optional.
     """
     print(deviceName, indexes)
 
 
-def freezeCountersAtTime(deviceName, absoluteTime, intervalTime, indexes):
-    # type: (AnyStr, int, int, List[int]) -> None
+def freezeCountersAtTime(deviceName, absoluteTime, intervalTime, indexes=None):
     """Issues a freeze command on the given counters at the given time
     for the specified duration.
 
     Args:
-        deviceName: The name of the DNP3 device driver.
-        absoluteTime: The absolute time at which to freeze, in millis.
-        intervalTime: The interval at which to periodically freeze, in
+        deviceName (str): The name of the DNP3 device driver.
+        absoluteTime (int): The absolute time at which to freeze, in
             millis.
-        indexes: An optional list of specific indexes on which to issue
-            the freeze command. An empty list will freeze all counters.
+        intervalTime (int): The interval at which to periodically
+            freeze, in millis.
+        indexes (list[object]): An optional list of specific indexes on
+            which to issue the freeze command. Optional.
     """
     print(deviceName, absoluteTime, intervalTime, indexes)
 
 
-def selectOperateAnalog(
-    deviceName,  # type: AnyStr
-    index,  # type: int
-    value,  # type: AnyNum
-    variation=None,  # type: Optional[int]
-):
-    # type: (...) -> int
+def selectOperateAnalog(deviceName, index, value, variation=None):
     """Issues a Select-And-Operate command to set an analog value in an
     analog output point.
 
     Args:
-        deviceName: The name of the DNP3 device driver.
-        index: The index of the object to be modified in the outstation.
-        value: The analog value that is requested (of type int, short,
-            float, or double).
-        variation: The DNP3 object variation to use in the request.
-            Optional.
+        deviceName (str): The name of the DNP3 device driver.
+        index (int): The index of the object to be modified in the
+            outstation.
+        value (object): The analog value that is requested (of type int,
+            short, float, or double).
+        variation (int): The DNP3 object variation to use in the
+            request. Optional.
 
     Returns:
-        The DNP3 status code of the response, as an integer.
+        int: The DNP3 status code of the response, as an integer.
     """
     print(deviceName, index, value, variation)
-    return 0
 
 
 def selectOperateBinary(
-    deviceName,  # type: AnyStr
-    indexes,  # type: List[int]
-    opType,  # type: int
-    tcCode=None,  # type: Optional[int]
-    count=None,  # type: Optional[int]
-    onTime=None,  # type: Optional[int]
-    offTime=None,  # type: Optional[int]
+    deviceName,
+    indexes,
+    opType,
+    tcCode=None,
+    count=None,
+    onTime=None,
+    offTime=None,
 ):
-    # type: (...) -> int
     """Issues a Select-And-Operate command for digital control
     operations at binary output points (CROB).
 
     Args:
         deviceName: The name of the DNP3 device driver.
-        indexes: A list of indexes of the objects to be modified in the
-            outstation.
-        opType: The type of operation. 0=NUL, 1=PULSE_ON, 2=PULSE_OFF,
-            3=LATCH_ON, 4=LATCH_OFF.
-        tcCode: The Trip-Close code, used in conjunction with the
+        indexes (list[object]): A list of indexes of the objects to be
+            modified in the outstation.
+        opType (int): The type of operation. 0=NUL, 1=PULSE_ON,
+            2=PULSE_OFF, 3=LATCH_ON, 4=LATCH_OFF
+        tcCode (int): The Trip-Close code, used in conjunction with the
             opType. 0=NUL, 1=CLOSE, 2=TRIP. Optional.
-        count: The number of times the outstation shall execute the
-            operation. Optional.
-        onTime: The duration that the output drive remains active, in
-            millis. Optional.
-        offTime: The duration that the output drive remains non-active,
+        count (int): The number of times the outstation shall execute
+            the operation. Optional.
+        onTime (int): The duration that the output drive remains active,
             in millis. Optional.
+        offTime (int): The duration that the output drive remains
+            non-active, in millis. Optional.
 
     Returns:
-        The DNP3 status code of the response, as an integer.
+        int: The DNP3 status code of the response, as an integer.
     """
     print(deviceName, indexes, opType, tcCode, count, onTime, offTime)
     return 0
```

### Comparing `ignition_api-8.1.40/src/system/groups.py` & `ignition-api-8.1.9/src/system/groups.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,42 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Transaction Group Functions.
 
 The following functions give you access to import and remove Transaction
 Groups.
 """
 
 from __future__ import print_function
 
 __all__ = ["loadFromFile", "removeGroups"]
 
-from typing import List
-
-from dev.coatl.helper.types import AnyStr
-
 
 def loadFromFile(filePath, projectName, mode):
-    # type: (AnyStr, AnyStr, int) -> None
     """Loads a transaction group configuration from an xml export, into
-    the specified project (creating the project if necessary).
-
-    The mode parameter dictates how overwrites occur.
-
-    Note:
-        This function is scoped for Perspective Sessions, but since all
-        scripts in Perspective run on the Gateway, the file must be
-        located on the Gateway's file system.
+    the specified project (creating the project if necessary). The mode
+    parameter dictates how overwrites occur.
 
     Args:
-        filePath: The path to a valid transaction group xml or csv file.
-        projectName: The name of the project to load into.
-        mode: How duplicates will be handled. 0 = Overwrite, 1 = Ignore,
-            2 = Replace the existing project with this one.
+        filePath (str): The path to a valid transaction group xml or csv
+            file.
+        projectName (str): The name of the project to load into.
+        mode (int): How duplicates will be handled. 0 = Overwrite,
+            1 = Ignore, 2 = Replace the existing project with this one.
     """
     print(filePath, projectName, mode)
 
 
 def removeGroups(projectName, paths):
-    # type: (AnyStr, List[AnyStr]) -> None
-    """Removes the specified groups from the project.
-
-    The group paths are "Folder/Path/To/GroupName", separated by forward
-    slashes.
+    """Removes the specified groups from the project. The group paths
+    are "Folder/Path/To/GroupName", separated by forward slashes.
 
     Args:
-        projectName: The project to remove from. If the project does not
-            exist, throws an IllegalArgumentException.
-        paths: A collection of paths to remove. The group paths are
-            "Folder/Path/To/GroupName", separated by forward slashes.
+        projectName (str): The project to remove from. If the project
+            does not exist, throws an IllegalArgumentException.
+        paths (list[str]): A collection of paths to remove. The group
+            paths are "Folder/Path/To/GroupName", separated by forward
+            slashes.
     """
     print(projectName, paths)
```

### Comparing `ignition_api-8.1.40/src/system/tag.py` & `ignition-api-8.1.9/src/system/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,929 +1,1169 @@
-"""Tag Functions.
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
 
-The following functions give you access to interact with Ignition Tags.
+"""Utility Functions.
+
+The following functions give you access to view various Gateway and
+Client data, as well as interact with other various systems.
 """
 
 from __future__ import print_function
 
 __all__ = [
-    "DEFAULT_TIMEOUT_MILLIS",
-    "LEGACY_DEFAULT_TIMEOUT_MILLIS",
-    "TAG_PATH",
-    "browse",
-    "browseHistoricalTags",
-    "configure",
-    "copy",
-    "deleteAnnotations",
-    "deleteTags",
-    "exists",
-    "exportTags",
-    "getConfiguration",
-    "importTags",
-    "isOverlaysEnabled",
-    "move",
-    "query",
-    "queryAnnotations",
-    "queryTagCalculations",
-    "queryTagDensity",
-    "queryTagHistory",
-    "readAsync",
-    "readBlocking",
-    "rename",
-    "requestGroupExecution",
-    "setOverlaysEnabled",
-    "storeAnnotations",
-    "storeTagHistory",
-    "writeAsync",
-    "writeBlocking",
+    "audit",
+    "beep",
+    "execute",
+    "exit",
+    "getAvailableLocales",
+    "getAvailableTerms",
+    "getClientId",
+    "getConnectTimeout",
+    "getConnectionMode",
+    "getEdition",
+    "getGatewayAddress",
+    "getGatewayStatus",
+    "getGlobals",
+    "getInactivitySeconds",
+    "getLocale",
+    "getLogger",
+    "getProjectName",
+    "getProperty",
+    "getReadTimeout",
+    "getSessionInfo",
+    "getSystemFlags",
+    "getVersion",
+    "invokeAsynchronous",
+    "invokeLater",
+    "jsonDecode",
+    "jsonEncode",
+    "modifyTranslation",
+    "playSoundClip",
+    "queryAuditLog",
+    "retarget",
+    "sendMessage",
+    "sendRequest",
+    "sendRequestAsync",
+    "setConnectTimeout",
+    "setConnectionMode",
+    "setLocale",
+    "setLoggingLevel",
+    "setReadTimeout",
+    "threadDump",
+    "translate",
 ]
 
-from typing import Any, Callable, Dict, List, Optional
-
-from com.inductiveautomation.ignition.common import BasicDataset
-from com.inductiveautomation.ignition.common.browsing import Results
-from com.inductiveautomation.ignition.common.model.values import (
-    BasicQualifiedValue,
-    QualityCode,
-)
-from com.inductiveautomation.ignition.common.sqltags.history.annotations import (
-    Annotation,
-)
-from dev.coatl.helper.types import AnyStr
+import getpass
+import json
+import os
+import platform
+import re
+import sys
+
+import system.__version__ as version
+import system.date
+import system.security
+from java.awt import Toolkit
+from java.lang import Object, Thread
 from java.util import Date
+from system.dataset import Dataset, PyDataSet
+
+
+class LoggerEx(Object):
+    """This class is a wrapper around a logger which provides additional
+    useful tools.
+
+    To create one, use the newBuilder() function and configure the
+    builder.
+    """
+
+    def getLogger(self):
+        pass
+
+    def getName(self):
+        pass
+
+    @staticmethod
+    def log(*args):
+        pass
+
+
+class Request(Object):
+    def block(self):
+        pass
+
+    def cancel(self):
+        pass
+
+    def checkTimeout(self):
+        pass
+
+    def compose(self, requestWatchers):
+        pass
+
+    def dispatchFunc(self):
+        pass
+
+    def finishExceptionally(self, e):
+        pass
+
+    def finishSuccessfully(self, value):
+        pass
+
+    def get(self):
+        pass
+
+    def getError(self):
+        pass
+
+    def getLongId(self):
+        pass
+
+    def internalOperationCompleted(self):
+        pass
+
+    def internalWait(self):
+        pass
+
+    def onError(self, func):
+        pass
+
+    def onSuccess(self, func):
+        pass
+
+    def startTime(self):
+        pass
+
+
+class Version(Object):
+    """Version object."""
+
+    dev = True
+    snapshot = False
+
+    def __init__(self, major=0, minor=0, rev=0, build=0, beta=0, rc=0):
+        """Version initializer.
+
+        Args:
+            major (int): Major number.
+            minor (int): Minor number.
+            rev (int): Revision number.
+            build (int): Build number.
+            beta (int): Beta number.
+            rc (int): Release Candidate number.
+        """
+        self.major = major
+        self.minor = minor
+        self.rev = rev
+        self.build = build
+        self.beta = beta
+        self.rc = rc
+
+    def __eq__(self, other, strict=False):
+        ret = 0
+        version_1 = [self.major, self.minor, self.rev]
+        version_2 = [other.major, other.minor, other.rev]
+
+        if strict:
+            version_1.append(self.build)
+            version_1.append(self.beta)
+            version_1.append(self.rc)
+            version_2.append(other.build)
+            version_2.append(other.beta)
+            version_2.append(other.rc)
+
+        for i in range(max(len(version_1), len(version_2))):
+            v_1 = version_1[i] if i < len(version_1) else 0
+            v_2 = version_2[i] if i < len(version_2) else 0
+            if v_1 > v_2:
+                ret = 1
+            elif v_1 < v_2:
+                ret = -1
+        return ret
+
+    def __str__(self):
+        return self.toString()
+
+    def compareTo(self, that):
+        """Compares two Versions.
+
+        Note that this comparison is stricter than we want for Gateway
+        restores or project imports. For those, isFutureVersion().
+
+        Args:
+            that (Version): The version to compare.
+
+        Returns:
+             int: 0 if self and that are equal, -1 if that is greater
+                than self, or 1 if self is greater than that.
+        """
+        return self.__eq__(that, True)
+
+    def exists(self):
+        pass
+
+    @staticmethod
+    def fromXML(inputStream):
+        pass
+
+    def getBasicString(self):
+        if self.rc > 0:
+            ret = "{}.{}.{}-rc{}".format(
+                self.major, self.minor, self.rev, self.rc
+            )
+        else:
+            ret = "{}.{}.{}".format(self.major, self.minor, self.rev)
+        return ret
+
+    def getBeta(self):
+        return self.beta
+
+    def getBuildNumber(self):
+        return self.build
+
+    def getMajor(self):
+        return self.major
+
+    def getMinor(self):
+        return self.minor
+
+    def getRc(self):
+        return self.rc
+
+    def getRevision(self):
+        return self.rev
+
+    def getXML(self):
+        pass
+
+    def isDev(self):
+        return self.dev
+
+    def isFutureVersion(self, arg):
+        other = self.parse(arg)
+        return self.__eq__(other) == -1
+
+    def isSnapshot(self):
+        return self.snapshot
+
+    @staticmethod
+    def parse(s):
+        sem_ver = [int(i) for i in re.findall(r"-?\d+", s)]
+        return Version(sem_ver[0], sem_ver[1], sem_ver[2])
+
+    def toParseableString(self):
+        """Returns the version as a compact, parseable (non-XML) string
+        that can be parsed with the 1-string constructor of this class.
+
+        Returns:
+            string: Compact, parseable (non-XML) string.
+        """
+        return "{}.{}.{}.{}".format(
+            self.major, self.minor, self.rev, self.build
+        )
+
+    def toString(self):
+        if self.rc > 0:
+            version = "{}.{}.{}-rc{} (b{})".format(
+                self.major, self.minor, self.rev, self.rc, self.build
+            )
+        elif self.isSnapshot():
+            version = "{}.{}.{}-SNAPSHOT (b{})".format(
+                self.major, self.minor, self.rev, self.build
+            )
+        elif self.build is not None:
+            version = "{}.{}.{} (b{})".format(
+                self.major, self.minor, self.rev, self.build
+            )
+        else:
+            version = "{}.{}.{}".format(self.major, self.minor, self.rev)
+        return version
+
+
+def audit(
+    action=None,
+    actionValue=None,
+    auditProfile="",
+    actor=None,
+    actorHost="localhost",
+    originatingSystem=None,
+    eventTimestamp=None,
+    originatingContext=4,
+    statusCode=0,
+):
+    """Inserts a record into an audit profile.
+
+    Args:
+        action (str): What happened. Default is null. Optional.
+        actionValue (str): What the action happened to. Default is null.
+            Optional.
+        auditProfile (str): Where the audit record should be stored.
+            Defaults to the project's audit profile (if specified), or
+            the gateway audit profile if calling in the gateway or
+            perspective scope. Optional.
+        actor (str): Who made the change. Will be populated
+            automatically if omitted, assuming there is a known user.
+            Optional.
+        actorHost (str): The hostname of whoever made the change. Will
+            be populated automatically if omitted.
+        originatingSystem (object): An even-length list providing
+            additional context to the audit event. Optional.
+        eventTimestamp (Date): When the event happened. Will be set
+            to the current time if omitted. Optional.
+        originatingContext (int): What scope the event originated from:
+            1 means Gateway, 2 means Designer, 4 means Client. Will be
+            set automatically if omitted. Optional.
+        statusCode (int): A quality code to attach to the object.
+            Defaults to 0, indicating no special meaning. Optional.
+    """
+    actor = system.security.getUsername() if actor is None else actor
+    eventTimestamp = (
+        system.date.now() if eventTimestamp is None else eventTimestamp
+    )
+    print(
+        action,
+        actionValue,
+        auditProfile,
+        actor,
+        actorHost,
+        originatingSystem,
+        eventTimestamp,
+        originatingContext,
+        statusCode,
+    )
+
+
+def beep():
+    """Tells the computer to make a "beep" sound."""
+    platforms = {
+        "linux1": "Linux",
+        "linux2": "Linux",
+        "darwin": "macOS",
+        "win32": "Windows",
+    }
+
+    if "java" in sys.platform:
+        Toolkit.getDefaultToolkit().beep()
+    elif sys.platform in platforms:
+        if platforms[sys.platform] == "Windows":
+            try:
+                import winsound
+
+                winsound.MessageBeep(winsound.MB_ICONEXCLAMATION)
+            except ImportError:
+                print("Beep!")
+        elif platforms[sys.platform] == "macOS":
+            os.system('say "beep"')
+        elif platforms[sys.platform] == "Linux":
+            print("\a")
+    else:
+        print("Beep!")
+
+
+def execute(commands):
+    """Executes the given commands via the operating system, in a
+    separate process.
+
+    The commands argument is an array of strings. The first string is
+    the program to execute, with subsequent strings being the arguments
+    to that command.
 
-DEFAULT_TIMEOUT_MILLIS = 45000
-LEGACY_DEFAULT_TIMEOUT_MILLIS = 45000
-TAG_PATH = None  # type: Any
+    Args:
+        commands (list[str]): A list containing the command (1st entry)
+            and associated arguments (remaining entries) to execute.
+    """
+    print(commands)
 
 
-def browse(path, filter=None):
-    # type: (AnyStr, Optional[Dict[AnyStr, Any]]) -> Results
-    """Returns a list of tags found at the specified Tag path.
+def exit(force=False):
+    """Exits the running client, as long as the shutdown intercept
+    script doesn't cancel the shutdown event.
 
-    The list objects are returned as dictionaries with some basic
-    information about each Tag.
+    Set force to True to not give the shutdown intercept script a chance
+    to cancel the exit. Note that this will quit the Client completely.
+    You can use system.security.logout() to return to the login screen.
 
     Args:
-        path: The path that will be browsed, typically to a folder or
-            UDT instance.
-        filter: A dictionary of browse filter keys.
+        force (bool): If True (1), the shutdown-intercept script will be
+            skipped. Default is False (0). Optional.
+    """
+    print(force)
+
+
+def getAvailableLocales():
+    """Returns a collection of strings representing the Locales added to
+    the Translation Manager, such as 'en' for English.
 
     Returns:
-        A Results object which contains a list of Tag dictionaries, one
-        for each Tag found during the browse.
+        list[str]: A collection of strings representing the Locales
+            added to the Translation Manager.
     """
-    print(path, filter)
-    return Results()
+    return ["en"]
 
 
-def browseHistoricalTags(
-    path,  # type: AnyStr
-    nameFilters=None,  # type: Optional[List[AnyStr]]
-    maxSize=None,  # type: Optional[int]
-    continuationPoint=None,  # type: Optional[Any]
-):
-    # type: (...) -> Results
-    """Will browse for any historical Tags at the provided historical
-    path.
+def getAvailableTerms():
+    """Returns a collection of available terms defined in the
+    translation system.
 
-    It will only browse for Tags at the path, and will not go down
-    through any children. Will return with a BrowseResults object.
+    Returns:
+         list[str]: A collection of all of the terms available from the
+            Translation Manager.
+    """
+    return ["term1", "term2"]
 
-    Args:
-        path: The Historical Tag Path to browse.
-        nameFilters: A list of name filters to be applied to the result
-            set. Optional.
-        maxSize: The maximum size of the result set. Optional.
-        continuationPoint: Sets the continuation point in order to
-            continue a browse that was previously started and then
-            limited. Use getContinuationPoint() on the Results object to
-            get the continuation point. Optional.
+
+def getClientId():
+    """Returns a hex-string that represents a number unique to the
+    running client's session.
+
+    You are guaranteed that this number is unique between all running
+    clients.
 
     Returns:
-        A Results object which contains a list of Tag dictionaries, one
-        for each Tag found during the browse.
+        str: A special code representing the client's session in a
+            unique way.
     """
-    print(path, nameFilters, maxSize, continuationPoint)
-    return Results()
+    return "92247003"
 
 
-def configure(
-    basePath,  # type: AnyStr
-    tags,  # type: List[Dict[AnyStr, Any]]
-    collisionPolicy="o",  # type: AnyStr
-):
-    # type: (...) -> List[QualityCode]
-    """Creates Tags from a given list of Python dictionaries or from a
-    JSON source string.
-
-    Can be used to overwrite a current Tag's configuration.
-
-    When utilizing this function, the Tag definitions must specify the
-    names of properties with their scripting/JSON name.
-
-    Args:
-        basePath: The starting point where the new Tags will be created.
-            When making changes to existing tags with this function,
-            you want to set the path to the parent folder of the
-            existing Tag(s), not the Tag(s) themselves.
-        tags: A list of Tag definitions, where each Tag definition is a
-            Python dictionary. Alternately, a JSON source string may be
-            passed to this parameter. When editing existing tags, it is
-            generally easier to retrieve the Tag configurations with
-            system.Tag.getConfiguration, modify the results of the
-            getConfiguration call, and then write the new configuration
-            to the parent folder of the existing Tag(s).
-        collisionPolicy: The action to take when a Tag or folder with
-            the same path and name is encountered. Possible values
-            include:
-
-            a - Abort and throw an exception
-            o - Overwrite and replace existing Tag's configuration
-            i - Ignore that item in the list
-            m - Merge, modifying values that are specified in the
-                definition, without impacting values that aren't defined
-                in the definition. Use this when you want to apply a
-                slight change to tags, without having to build a
-                complete configuration object.
-
-            Defaults to Overwrite. Optional.
-
-    Returns:
-        A List of QualityCode objects, one for each Tag in the list,
-        that is representative of the result of the operation.
-    """
-    print(basePath, tags, collisionPolicy)
-    return [QualityCode() for _ in tags]
-
-
-def copy(
-    tags,  # type: List[AnyStr]
-    destination,  # type: AnyStr
-    collisionPolicy="o",  # type: AnyStr
+def getConnectTimeout():
+    """Returns the connect timeout in milliseconds for all
+    client-to-gateway communication.
+
+    This is the maximum amount of time that communication operations to
+    the Gateway will be given to connect. The default is 10,000ms (10
+    seconds).
+
+    Returns:
+        int: The current connect timeout, in milliseconds. Default is
+            10,000 (ten seconds).
+    """
+    return 10000
+
+
+def getConnectionMode():
+    """Retrieves this client session's current connection mode.
+
+    3 is read/write, 2 is read-only, and 1 is disconnected.
+
+    Returns:
+        int: The current connection mode for the client.
+    """
+    return 3
+
+
+def getEdition():
+    """Returns the "edition" of the Vision client - "standard",
+    "limited", or "panel".
+
+    Returns:
+        str: The edition of the Vision module that is running the
+            client.
+    """
+    return "standard"
+
+
+def getGatewayAddress():
+    """Returns the address of the gateway that the client is currently
+    communicating with.
+
+    Returns:
+        str: The address of the Gateway that the client is communicating
+            with.
+    """
+    return "http://localhost:8088/"
+
+
+def getGatewayStatus(
+    gatewayAddress, connectTimeoutMillis=None, socketTimeoutMillis=None
 ):
-    # type: (...) -> List[QualityCode]
-    """Copies tags from one folder to another.
+    """Returns a string that indicates the status of the Gateway.
 
-    Multiple Tag and folder paths may be passed to a single call of this
-    function. The new destination can be a separate Tag provider.
+    A status of RUNNING means that the Gateway is fully functional.
+    Thrown exceptions return "ERROR" with the error message appended to
+    the string.
 
     Args:
-        tags: A List of Tag paths to move.
-        destination: The destination to copy the Tags to. All specified
-            tags will be copied to the same destination. The destination
-            Tag provider must be specified.
-        collisionPolicy: The action to take when a Tag or folder with
-            the same path and name is encountered. Possible values
-            include: "a" Abort and throw an exception, "o" Overwrite and
-            replace existing Tag's configuration, "i" Ignore that item
-            in the list. Defaults to Overwrite. Optional.
+        gatewayAddress (str): The gateway address to ping, in the form
+            of ADDR:PORT/main.
+        connectTimeoutMillis (int): The maximum time in milliseconds to
+            attempt to initially contact a Gateway. Optional.
+        socketTimeoutMillis (int): The maximum time in milliseconds to
+            wait for a response from a Gateway after initial connection
+            has been established. Optional.
 
     Returns:
-        A List of QualityCode objects, one for each Tag in the list,
-        that is representative of the result of the operation.
+        str: A string that indicates the status of the Gateway. A status
+            of RUNNING means that the Gateway is fully functional.
     """
-    print(tags, destination, collisionPolicy)
-    return [QualityCode() for _ in tags]
+    print(gatewayAddress, connectTimeoutMillis, socketTimeoutMillis)
+    return "RUNNING"
 
 
-def deleteAnnotations(paths, storageIds):
-    # type: (List[AnyStr], List[AnyStr]) -> List[BasicQualifiedValue]
-    """Removes stored annotations from the sqlth_annotations table.
+def getGlobals():
+    """This method returns a dictionary that provides access to the
+    legacy global namespace.
 
-    Requires the full Tag path (including history provider) for each
-    annotation, as well as each annotation's storage ID.
+    As of version 7.7.0, most new scripts use the modern style of
+    scoping, which makes the 'global' keyword act very differently. Most
+    importantly, the modern scoping rules mean that variables declared
+    as 'global' are only global within that one module. The
+    system.util.getGlobals() method can be used to interact with older
+    scripts that used the old meaning of the 'global' keyword.
 
-    The function expects two lists (PySequences) of equal length. The
-    items in each list is 1-to-1, meaning the first item in the "paths"
-    list relates to the first item in the "storageIds" list, the second
-    item in "paths" relates to the second item in "storageIds", etc.
+    Returns:
+        dict: The global namespace, as a dictionary.
+    """
+    return {}
 
-    Args:
-        paths: A list of Tag paths with existing annotations. The paths
-            are equivalent to what would be used for a Tag history
-            query, and should specify the source provider as well. For
-            example, "[HistoryProvider/Gateway:Provider]Path/To/Tag".
-        storageIds: A sequence of storage identifiers that will be
-            deleted. Storage ID values can be retrieved with
-            system.tag.queryAnnotations.
+
+def getInactivitySeconds():
+    """Returns the number of seconds since any keyboard or mouse
+    activity.
 
     Returns:
-        A list of qualified values. The quality code will indicate
-        success or failure, and if successful, the storage id of the
-        annotation will have been deleted.
+        long: The number of seconds the mouse and keyboard have been
+            inactive for this client.
     """
-    print(paths, storageIds)
-    return [BasicQualifiedValue() for _ in paths]
+    return long(0)
 
 
-def deleteTags(tagPaths):
-    # type: (List[AnyStr]) -> List[QualityCode]
-    """Deletes multiple Tags or Tag Folders.
+def getLocale():
+    """Returns the current string representing the user's Locale, such
+    as 'en' for English.
+
+    Returns:
+        str: The current Locale.
+    """
+    return "en"
 
-    When deleting a Tag Folder, all Tags under the folder are also
-    deleted.
+
+def getLogger(name):
+    """Returns a Logger object that can be used to log messages to the
+    console.
 
     Args:
-        tagPaths: A List of the paths to the Tags or Tag Folders that
-            are to be removed.
+        name (str): The name of a logger to create.
+
+    Returns:
+        LoggerEx: A new Logger object used to log informational and
+            error messages.
+    """
+    print(name)
+    return LoggerEx()
+
+
+def getProjectName():
+    """Returns the name of the project that is currently being run.
 
     Returns:
-         A List of QualityCode objects, one for each Tag in the list,
-         that is representative of the result of the operation.
+        str: The name of the currently running project.
     """
-    print(tagPaths)
-    return [QualityCode() for _ in tagPaths]
+    return "MyProject"
 
 
-def exists(tagPath):
-    # type: (AnyStr) -> bool
-    """Checks whether or not a Tag with a given path exists.
+def getProperty(propertyName):
+    r"""Retrieves the value of a named system property.
+
+    Some of the available properties are:
+
+        file.separator. The system file separator character. (for
+            example, "/" (unix) or "\" (windows))
+        line.separator. The system line separator string. (for example,
+            "\r\n" (carriage return, newline))
+        os.arch. Operating system architecture. (for example, "x86")
+        os.name. Operating system name. (for example, "Windows XP")
+        os.version. Operating system version. (for example, "5.1")
+        user.home. User's home directory.
+        user.name. User's account name.
 
     Args:
-        tagPath: The path of the Tag to look up.
+        propertyName (str): The name of the system property to get.
 
     Returns:
-        True if a Tag exists for the given path, False otherwise.
+        str: The value for the named property.
     """
-    print(tagPath)
-    return True
+    # Initialize variables.
+    ret = None
 
+    if propertyName == "file.separator":
+        ret = os.sep
+    elif propertyName == "line.separator":
+        ret = os.linesep
+    elif propertyName == "os.arch":
+        ret = platform.machine()
+    elif propertyName == "os.name":
+        ret = platform.system()
+    elif propertyName == "os.version":
+        ret = platform.release()
+    elif propertyName == "user.home":
+        ret = os.path.expanduser("~")
+    elif propertyName == "user.name":
+        ret = getpass.getuser()
 
-def exportTags(
-    filePath=None,  # type: Optional[AnyStr]
-    tagPaths=None,  # type: Optional[List[AnyStr]]
-    recursive=True,  # type: bool
-    exportType="json",  # type: AnyStr
-):
-    # type: (...) -> Optional[AnyStr]
-    """Exports Tags to a file on a local file system.
+    return ret
 
-    The term "local file system" refers to the scope in which the script
-    was running; for example, running this script in a Gateway Timer
-    script will export the file to the Gateway file system.
-
-    Args:
-        filePath: The file path that the Tags will be exported to. If
-            the file does not already exist, this function will attempt
-            to create it.
-        tagPaths: A List of Tag paths to export. All Tag paths in the
-            list must be from the same parent folder.
-        recursive: Set to True to export all Tags under each Tag path,
-            including Tags in child folders. Defaults to True. Optional.
-        exportType: The type of file that will be exported. Set to
-            "json" or "xml". Defaults to "json". Optional.
-
-    Returns:
-        None or if ``filePath`` is omitted, the tag export as a string.
-    """
-    print(filePath, tagPaths, recursive, exportType)
-    return None if filePath is None else ""
-
-
-def getConfiguration(basePath, recursive=False):
-    # type: (AnyStr, bool) -> List[Dict[AnyStr, Any]]
-    """Retrieves Tags from the Gateway as Python dictionaries.
-
-    These can be edited and then saved back using system.tag.configure.
-
-    Args:
-        basePath: The starting point where the Tags will be retrieved.
-            This can be a folder containing, and if recursive is True,
-            then the function will attempt to retrieve all of the tags
-            in the folder.
-        recursive: If True, the entire Tag Tree under the specified path
-            will be retrieved. Note that this will only check one level
-            under the base path. True recursion would require multiple
-            uses of this function at different paths. Optional.
-
-    Returns:
-         A List of Tag dictionaries. Nested Tags are placed in a list
-         marked as "tags" in the dictionary.
-    """
-    return (
-        [
-            {
-                "tags": [
-                    {
-                        "path": "New Tag",
-                        "tagType": "AtomicTag",
-                        "name": "New Tag",
-                        "valueSource": "memory",
-                    }
-                ],
-                "path": basePath,
-                "tagType": "Folder",
-                "name": "Test",
-            }
-        ]
-        if recursive
-        else [{"path": basePath, "tagType": "Folder", "name": "Test"}]
-    )
+
+def getReadTimeout():
+    """Returns the read timeout in milliseconds for all
+    client-to-gateway communication.
+
+    This is the maximum amount of time allowed for a communication
+    operation to complete. The default is 60,000 ms (1 minute).
+
+    Returns:
+         int: The current read timeout, in milliseconds. Default is
+            60,000 ms (one minute).
+    """
+    return 60000
 
 
-def importTags(filePath, basePath, collisionPolicy="o"):
-    # type: (AnyStr, AnyStr, AnyStr) -> List[QualityCode]
-    """Imports a JSON Tag file at the provided path.
+def getSessionInfo(usernameFilter=None, projectFilter=None):
+    """Returns a PyDataSet holding information about all of the sessions
+    (logged-in users) on the Gateway.
 
-    Also supports XML and CSV Tag file exports from legacy systems.
+    Optional regular-expression based filters can be provided to filter
+    the username or the username and the project returned.
 
     Args:
-        filePath: The file path of the Tag export to import.
-        basePath: The Tag path that will serve as the root node for the
-            imported Tags.
-        collisionPolicy: The action to take when a Tag or folder with
-            the same path and name is encountered. Possible values
-            include: "a" Abort and throw an exception, "o" Overwrite and
-            replace existing Tag's configuration, "i" Ignore that item
-            in the list. Defaults to Overwrite. Optional.
+        usernameFilter (str): A regular-expression based filter string
+            to restrict the list by username. Optional.
+        projectFilter (str): A regular-expression based filter string to
+            restrict the list by project. Optional.
 
     Returns:
-        A List of QualityCode objects, one for each Tag in the list,
-        that is representative of the result of the operation.
+        PyDataSet: A dataset representing the Gateway's current
+            sessions.
     """
-    print(filePath, basePath, collisionPolicy)
-    return [QualityCode()]
+    print(usernameFilter, projectFilter)
+    return PyDataSet()
 
 
-def isOverlaysEnabled():
-    # type: () -> bool
-    """Returns whether or not the current client's quality overlay
-    system is currently enabled.
+def getSystemFlags():
+    """Returns an integer that represents a bit field containing
+    information about the currently running system.
+
+    Each bit corresponds to a specific flag as defined in the bitmask
+    below. The integer return will be a total of all of the bits that
+    are currently active.
+
+    Returns:
+        int: A total of all the bits that are currently active. A full
+            screen client launched from the gateway webpage with no SSL
+            will have a value of 44 (Fullscreen flag + Webstart Flag +
+            Client Flag).
+    """
+    return 1
+
+
+def getVersion():
+    """Returns the Ignition version number that is currently being run.
 
     Returns:
-         True if overlays are currently enabled.
+        Version: The currently running Ignition version number. as a
+            Version object.
     """
-    return False
+    major, minor, rev = [int(i) for i in version.__version__.split(".")]
+    build = int(version.__build__)
+    return Version(major=major, minor=minor, rev=rev, build=build)
 
 
-def move(tags, destination, collisionPolicy="o"):
-    # type: (List[AnyStr], AnyStr, AnyStr) -> List[QualityCode]
-    """Moves Tags or Folders to a new destination.
+def invokeAsynchronous(function, args=None, kwargs=None, description=None):
+    """Invokes (calls) the given Python function on a different thread.
 
-    The new destination can be a separate Tag provider. If interested in
-    copying the tags to a new destination, instead of moving them,
-    please see the system.tag.copy page.
+    This means that calls to invokeAsynchronous will return immediately,
+    and then the given function will start executing asynchronously on a
+    different thread. This is useful for long-running data intensive
+    functions, where running them synchronously (in the GUI thread)
+    would make the GUI non-responsive for an unacceptable amount of
+    time.
 
     Args:
-        tags: A List of Tag paths to move.
-        destination: The destination to move the Tags to. The
-            destination Tag provider must be specified: i.e.,
-            ``[default]Folder/myTag``.
-        collisionPolicy: The action to take when a Tag or folder with
-            the same path and name is encountered. Possible values
-            include: "a" Abort and throw an exception, "o" Overwrite and
-            replace existing Tag's configuration, "i" Ignore that item
-            in the list. Defaults to Overwrite. Optional.
+        function (object): A Python function object that will get
+            invoked with no arguments in a separate thread.
+        args: A list or tuple of Python objects that will be provided to
+            the called function as arguments. Equivalent to the *
+            operator. Optional.
+        kwargs: A dictionary of keyword argument names to Python object
+            values that will be provided to the called function as
+            keyword arguments. Equivalent to the ** operator. Optional.
+        description (str): A description to use for the asynchronous
+            thread. Will be displayed on the current scope's diagnostic
+            view for scripts. For Vision and the Designer, this would be
+            the "Scripts" tab of the Diagnostics popup. For Perspective
+            and the Gateway scope, this would be the Gateway's Running
+            Scripts status page. Optional.
 
     Returns:
-        A List of QualityCode objects, one for each Tag in the list,
-        that is representative of the result of the operation.
+        Thread: The executing thread.
     """
-    print(tags, destination, collisionPolicy)
-    return [QualityCode() for _ in tags]
+    print(function, args, kwargs, description)
+    return Thread()
 
 
-def query(
-    provider=None,  # type: Optional[AnyStr]
-    query=None,  # type: Optional[Dict[AnyStr, Any]]
-    limit=None,  # type: Optional[int]
-    continuation=None,  # type: Optional[AnyStr]
-):
-    # type: (...) -> Results
-    """Queries a Tag Provider to produce a list of tags that meet the
-    specified criteria.
+def invokeLater(function, delay=0):
+    """Invokes (calls) the given Python function object after all of the
+    currently processing and pending events are done being processed, or
+    after a specified delay.
+
+    The function will be executed on the GUI, or event dispatch, thread.
+    This is useful for events like propertyChange events, where the
+    script is called before any bindings are evaluated.
+
+    If you specify an optional time argument (number of milliseconds),
+    the function will be invoked after all currently processing and
+    pending events are processed plus the duration of that time.
 
     Args:
-        provider: The Tag Provider to query. Optional.
-        query: A JSON document that specifies the query conditions.
+        function (object): A Python function object that will be invoked
+            later, on the GUI, or event-dispatch, thread with no
+            arguments.
+        delay (int): A delay, in milliseconds, to wait before the
+            function is invoked. The default is 0, which means it will
+            be invoked after all currently pending events are processed.
             Optional.
-        limit: Maximum results to return. If more results are possible,
-            the result will have a continuation point set. Optional.
-        continuation: The Tag ID of a previously returned
-            continuation point, to continue the associated query from
-            that point. Optional.
+    """
+    print(function, delay)
+
+
+def jsonDecode(jsonString):
+    """Takes a json String and converts it into a Python object such as
+    a list or a dict.
+
+    If the input is not valid json, a string is returned.
+
+    Args:
+        jsonString (str): The JSON string to decode into a Python
+            object.
 
     Returns:
-        A dataset representing the results of the query.
+        dict: The decoded Python object.
     """
-    print(provider, query, limit, continuation)
-    return Results()
+    return json.loads(jsonString)
 
 
-def queryAnnotations(
-    paths,  # type: List[AnyStr]
-    startTime=None,  # type: Optional[Date]
-    endTime=None,  # type: Optional[Date]
-    types=None,  # type: Optional[List[AnyStr]]
-):
-    # type: (...) -> List[Annotation]
-    """Queries user stored annotations from the Tag history system for a
-    set of paths, for a given time range.
-
-    Args:
-        paths: A list of Tag paths to query. The paths are equivalent to
-            what would be used ofr a Tag history query, and should
-            specify the source provider as well. For example,
-            ``"[HistoryProvider/Gateway:Provider]Path/To/Tag"``.
-        startTime: The start of the time range. If not defined, defaults
-            to 12 hours ago. Optional.
-        endTime: The end of time range. If not defined, defaults to
-            "now". Optional.
-        types: A list of string "types" to filter on. Types are defined
-            by the annotations and various subsystems, and may vary with
-            different providers. Possible annotation types are listed on
-            the system.Tag.storeAnnotations page. Optional.
-
-    Returns:
-        A list of Annotation objects that match the query criteria.
-    """
-    print(paths, startTime, endTime, types)
-    return [Annotation() for _ in paths]
-
-
-def queryTagCalculations(
-    paths,  # type: List[AnyStr]
-    calculations,  # type: List[AnyStr]
-    startDate=None,  # type: Optional[Date]
-    endDate=None,  # type: Optional[Date]
-    rangeHours=None,  # type: Optional[int]
-    rangeMinutes=None,  # type: Optional[int]
-    aliases=None,  # type: Optional[List[AnyStr]]
-    includeBoundingValues=True,  # type: bool
-    validatesSCExec=True,  # type: bool
-    noInterpolation=False,  # type: bool
-    ignoreBadQuality=False,  # type: bool
+def jsonEncode(pyObj, indentFactor=4):
+    """Takes a Python object such as a list or dict and converts into a
+    json string.
+
+    Args:
+        pyObj (object): The Python object to encode into JSON such as a
+            Python list or dictionary.
+        indentFactor (int): The number of spaces to add to each level of
+            indentation for prettyprinting. Optional.
+
+    Returns:
+        str: The encoded JSON string.
+    """
+    return json.dumps(pyObj, indent=indentFactor)
+
+
+def modifyTranslation(term, translation, locale="en"):
+    """This function allows you to add or modify a global translation.
+
+    Args:
+        term (str): The key term to translate.
+        translation (str): The translated value to store.
+        locale (str): If specified, the locale code (such as "es")
+            identifying the language of the translation. Otherwise, the
+            currently set language is used. Optional.
+    """
+    print(term, translation, locale)
+
+
+def playSoundClip(wav, volume=1.0, wait=False):
+    """Plays a sound clip from a wav file to the system's default audio
+    device.
+
+    The wav file can be specified as a filepath, a URL, or directly as a
+    raw byte[].
+
+    Args:
+        wav (object): A byte list of a wav file or filepath or URL that
+            represents a wav file.
+        volume (float): The clip's volume, represented as a floating
+            point number between 0.0 and 1.0. Optional.
+        wait (bool): A boolean flag indicating whether or not the call
+            to playSoundClip should wait for the clip to finish before
+            it returns. Optional.
+    """
+    print(wav, volume, wait)
+
+
+def queryAuditLog(
+    auditProfileName,
+    startDate=None,
+    endDate=None,
+    actorFilter=None,
+    actionFilter=None,
+    targetFilter=None,
+    valueFilter=None,
+    systemFilter=None,
+    contextFilter=None,
 ):
-    # type: (...) -> BasicDataset
-    """Queries various calculations (aggregations) for a set of tags
-    over a specified range.
-
-    Returns a dataset with a row per Tag, and a column per calculation.
-
-    This is useful when you wish to aggregate Tag history collected over
-    a period of time into a single value per aggregate. If you want
-    multiple values aggregated to a single time slice (i.e., hourly
-    aggregates for the same Tag over an 8 hour period) consider using
-    system.Tag.queryTagHistory
-
-    Args:
-        paths: An array of Tag paths (strings) to query calculations
-            for. The resulting dataset will have a row for each Tag, and
-            a column for each calculation.
-        calculations: An array of calculations (aggregation functions)
-            to execute for each Tag. Valid values are: "Average"
-            (time-weighted), "MinMax", "LastValue", "SimpleAverage",
-            "Sum", "Minimum", "Maximum", "DurationOn", "DurationOff",
-            "CountOn", "CountOff", "Count", "Range", "Variance",
-            "StdDev", "PctGood", and "PctBad".
-        startDate: The starting point for the calculation window. If
-            omitted, and range is not used, 8 hours before the current
-            time is used. Optional.
-        endDate: The end of the calculation window. If omitted, and
-            range is not used, uses the current time. Optional.
-        rangeHours: Allows you to specify the query range in hours,
-            instead of using start and end date. Can be positive or
-            negative, and can be used in conjunction with startDate or
-            endDate. Optional.
-        rangeMinutes: Same as rangeHours, but in minutes. Optional.
-        aliases: Aliases that will be used to override the Tag path
-            names in the result dataset. Must be 1-to-1 with the Tag
-            paths. If not specified, the Tag paths themselves will be
-            used. Optional.
-        includeBoundingValues: A boolean flag indicating that the system
-            should attempt to load values before and after the query
-            bounds for the purpose of interpolation. The effect depends
-            on the aggregates used. The default is True. Optional.
-        validatesSCExec: A boolean flag indicating whether or not data
-            should be validated against the scan class execution
-            records. If False, calculations may include data that is
-            assumed to be good, even though the system may not have been
-            running. Default is True. Optional.
-        noInterpolation: A boolean flag indicating that the system
-            should not attempt to interpolate values in situations where
-            it normally would, such as for analog tags. Default is
-            False. Optional.
-        ignoreBadQuality: A boolean flag indicating that bad quality
-            values should not be used in the query process. If set, any
-            value with a "bad" quality will be completely ignored in
-            calculations. Default is False. Optional.
+    """Queries an audit profile for audit history.
+
+    Returns the results as a dataset.
+
+    Args:
+        auditProfileName (str): The name of the audit profile to pull
+            the history from.
+        startDate (Date): The earliest audit event to return. If
+            omitted, the current time - 8 hours will be used. Optional.
+        endDate (Date): The latest audit event to return. If
+            omitted, the current time will be used. Optional.
+        actorFilter (str): A filter string used to restrict the results
+            by actor. Optional.
+        actionFilter (str): A filter string used to restrict the results
+            by action. Optional.
+        targetFilter (str): A filter string used to restrict the results
+            by target. Optional.
+        valueFilter (str): A filter string used to restrict the results
+            by value. Optional.
+        systemFilter (str): A filter string used to restrict the results
+            by system. Optional.
+        contextFilter (int): A bitmask used to restrict the results by
+            context. 0x01 = Gateway, 0x02 = Designer, 0x04 = Client.
+            Optional.
 
     Returns:
-        A dataset representing the calculations over the specified
-        range.
+        Dataset: A dataset with the audit events from the specified
+            profile that match the filter arguments.
     """
+    endDate = system.date.now() if endDate is None else endDate
+    startDate = (
+        system.date.addHours(endDate, -8) if startDate is None else startDate
+    )
     print(
-        paths,
-        calculations,
+        auditProfileName,
         startDate,
         endDate,
-        rangeHours,
-        rangeMinutes,
-        aliases,
-        includeBoundingValues,
-        validatesSCExec,
-        noInterpolation,
-        ignoreBadQuality,
+        actorFilter,
+        actionFilter,
+        targetFilter,
+        valueFilter,
+        systemFilter,
+        contextFilter,
     )
-    return BasicDataset()
+    return Dataset()
 
 
-def queryTagDensity(paths, startDate, endDate):
-    # type: (List[AnyStr], Date, Date) -> BasicDataset
-    """Queries the Tag history system for information about the density
-    of data.
-
-    In other words, how much data is available for a given time
-    span.
-
-    This function is called with a list of Tag paths, and a start and
-    end date. The result set is a two column dataset specifying the
-    timestamp, and a relative weight. Each row is valid from the given
-    time until the next row. Tags are assigned a 1 or a 0 if they are
-    present or not. All values are then multiplied together to get a
-    decimal based percentage for the density. Thus, for four Tag paths
-    passed in, if three Tags were present during the span, the result
-    would be 0.75.
-
-    Note:
-        This function relies on being able to validate the data against
-        tag group execution. This function will be unable to return
-        density information for tags that were stored by an Internal
-        Historian Provider, as well as cases where tag group validation
-        is disabled (such as by disabling Enable State Data Detection).
-
-    Args:
-        paths: An array of Tag paths (strings) to query.
-        startDate: The start of the range to query.
-        endDate: The end of the range to query.
-
-    Returns:
-        A two-column dataset consisting of a timestamp and a weight.
-        Each row is valid until the next row.
-    """
-    print(paths, startDate, endDate)
-    return BasicDataset()
-
-
-def queryTagHistory(
-    paths,  # type: List[AnyStr]
-    startDate=None,  # type: Optional[Date]
-    endDate=None,  # type: Optional[Date]
-    returnSize=-1,  # type: int
-    aggregationMode="Average",  # type: AnyStr
-    returnFormat="Wide",  # type: AnyStr
-    columnNames=None,  # type: Optional[List[AnyStr]]
-    intervalHours=None,  # type: Optional[int]
-    intervalMinutes=None,  # type: Optional[int]
-    rangeHours=None,  # type: Optional[int]
-    rangeMinutes=None,  # type: Optional[int]
-    aggregationModes=None,  # type: Optional[List[AnyStr]]
-    includeBoundingValues=None,  # type: Optional[bool]
-    validateSCExec=None,  # type: Optional[bool]
-    noInterpolation=None,  # type: Optional[bool]
-    ignoreBadQuality=None,  # type: Optional[bool]
-    timeout=None,  # type: Optional[int]
-    intervalSeconds=None,  # type: Optional[int]
-    rangeSeconds=None,  # type: Optional[int]
+def retarget(project, addresses=None, params=None, windows=None):
+    """This function allows you to programmatically 'retarget' the
+    Client to a different project and/or different Gateway.
+
+    You can have it switch to another project on the same Gateway, or
+    another gateway entirely, even across a WAN. This feature makes the
+    vision of a seamless, enterprise-wide SCADA application a reality.
+
+    The retarget feature will attempt to transfer the current user
+    credentials over to the new project / Gateway. If the credentials
+    fail on that project, the user will be prompted for a valid username
+    and password. Once valid authentication has been achieved, the
+    currently running project is shut down, and the new project is
+    loaded.
+
+    You can pass any information to the other project through the
+    parameters dictionary. All entries in this dictionary will be set in
+    the global scripting namespace in the other project. Even if you
+    don't specify any parameters, the system will set the variable
+    _RETARGET_FROM_PROJECT to the name of the current project and
+    _RETARGET_FROM_GATEWAY to the address of the current Gateway.
+
+    Args:
+        project (str): The name of the project to retarget to.
+        addresses (object): The address of the Gateway that the project
+            resides on. If omitted, the current Gateway will be used.
+            Format is: host:port. Optional.
+            As of 8.0.8 this can be a list of strings. When using a
+            list, the function will try each address in order, waiting
+            for the timeout period between each address attempt.
+        params (dict): A dictionary of parameters that will be passed to
+            the new project. They will be set as global variables in the
+            new project's Python scripting environment. Optional.
+        windows (list[str]): A list of window paths to use as the
+            startup windows. If omitted, the project's normal startup
+            windows will be opened. If specified, the project's normal
+            startup windows will be ignored, and this list will be used
+            instead. Optional.
+    """
+    print(project, addresses, params, windows)
+
+
+def sendMessage(
+    project,
+    messageHandler,
+    payload=None,
+    scope=None,
+    clientSessionId=None,
+    user=None,
+    hasRole=None,
+    hostName=None,
+    remoteServers=None,
 ):
-    # type: (...) -> BasicDataset
-    """Issues a query to the Tag Historian.
+    """This function sends a message to clients running under the
+    Gateway, or to a project within the Gateway itself.
 
-    Querying Tag history involves specifying the tags and the date
-    range, as well as a few optional parameters. The Tag historian will
-    find the relevant history and then interpolate and aggregate it
-    together into a coherent, tabular result set.
-
-    Args:
-        paths: An array of Tag paths (strings) to query. Each Tag path
-            specified will be a column in the result dataset.
-        startDate: The earliest value to retrieve. If omitted, 8 hours
-            before current time is used. Optional.
-        endDate: The latest value to retrieve. If omitted, current time
-            is used. Optional.
-        returnSize: The number of samples to return. -1 will return
-            values as they changed, and 0 will return the "natural"
-            number of values based on the logging rates of the scan
-            class(es) involved. -1 is the default. Optional.
-        aggregationMode: The mode to use when aggregating multiple
-            samples into one time slice. Valid values are: "Average"
-            (time-weighted), "MinMax", "LastValue", "SimpleAverage",
-            "Sum", "Minimum", "Maximum", "DurationOn", "DurationOff",
-            "CountOn", "CountOff", "Count", "Range", "Variance",
-            "StdDev", "PctGood", and "PctBad". Optional.
-        returnFormat: Use "Wide" to have a column per Tag queried, or
-            "Tall" to have a fixed-column format. Default is "Wide".
-            Optional.
-        columnNames: Aliases that will be used to override the column
-            names in the result dataset. Must be 1-to-1 with the Tag
-            paths. If not specified, the Tag paths themselves will be
-            used as column titles. Optional.
-        intervalHours: Allows you to specify the window interval in
-            terms of hours, as opposed to using a specific return size.
-            Optional.
-        intervalMinutes: Same as intervalHours, but in minutes. Can be
-            used on its own, or in conjunction with intervalHours.
-            Optional.
-        rangeHours: Allows you to specify the query range in hours,
-            instead of using start and end date. Can be positive or
-            negative, and can be used in conjunction with startDate or
-            endDate. Optional.
-        rangeMinutes: Same as rangeHours, but in minutes. Optional.
-        aggregationModes: A one-to-one list with paths specifying an
-            aggregation mode per column. Optional.
-        includeBoundingValues: A boolean flag indicating that the system
-            should attempt to include values for the query bound times
-            if possible. The default for this property depends on the
-            query mode, so unless a specific behavior is desired, it is
-            best to not include this parameter. Optional.
-        validateSCExec: A boolean flag indicating whether or not data
-            should be validated against the scan class execution
-            records. If False, data will appear flat (but good quality)
-            for periods of time in which the system wasn't running. If
-            True, the same data would be bad quality during downtime
-            periods. Optional.
-        noInterpolation: A boolean flag indicating that the system
-            should not attempt to interpolate values in situations where
-            it normally would. This will also prevent the return of rows
-            that are purely interpolated. Optional.
-        ignoreBadQuality: A boolean flag indicating that bad quality
-            values should not be used in the query process. If set, any
-            value with a "bad" quality will be completely ignored in
-            calculations and in the result set. Optional.
-        timeout: Timeout in milliseconds for Client Scope. This property
-            is ignored in the Gateway Scope. Optional.
-        intervalSeconds: Same as intervalHours and interval Minutes, but
-            in seconds. Can be used on its own, or in conjunction with
-            intervalHours and intervalMinutes. Optional.
-        rangeSeconds: Allows you to specify the query range in seconds,
-            instead of using start and end date. Can be positive or
-            negative, and can be used in conjunction with startDate or
-            endDate. Optional.
-
-    Returns:
-        A dataset representing the historian values for the specified
-        Tag paths. The first column will be the timestamp, and each
-        column after that represents a Tag.
+    To handle received messages, you must set up event script message
+    handlers within a project. These message handlers run Jython code
+    when a message is received. You can add message handlers under the
+    "Message" section of the client/Gateway event script configuration
+    dialogs.
+
+    Args:
+        project (str): The name of the project containing the message
+            handler.
+        messageHandler (str): The name of the message handler that will
+            fire upon receiving a message.
+        payload (dict): A PyDictionary which will get passed to the
+            message handler. Use "payload" in the message handler to
+            access dictionary variables. Optional.
+        scope (str): Limits the scope of the message delivery to "C"
+            (clients), "G" (Gateway), or "CG" for clients and the
+            Gateway. Defaults to "C" if the user name, role or host name
+            parameters are set, and to "CG" if none of these parameters
+            are set. Optional.
+        clientSessionId (str): Limits the message delivery to a client
+            with the specified session ID. Optional.
+        user (str): Limits the message delivery to clients where the
+            specified user has logged in. Optional.
+        hasRole (str): Limits the message delivery to any client where
+            the logged in user has the specified user role. Optional.
+        hostName (str): Limits the message delivery to the client that
+            has the specified network host name. Optional.
+        remoteServers (list[str]): A list of Strings representing
+            Gateway Server names. The message will be delivered to each
+            server in the list. Upon delivery, the message is
+            distributed to the local Gateway and clients as per the
+            other parameters. Optional.
+
+    Returns:
+        list[str]: A List of Strings containing information about each
+            system that was selected for delivery, where each List item
+            is comma-delimited.
     """
     print(
-        paths,
-        startDate,
-        endDate,
-        returnSize,
-        aggregationMode,
-        returnFormat,
-        columnNames,
-        intervalHours,
-        intervalMinutes,
-        rangeHours,
-        rangeMinutes,
-        aggregationModes,
-        includeBoundingValues,
-        validateSCExec,
-        noInterpolation,
-        ignoreBadQuality,
-        timeout,
-        intervalSeconds,
-        rangeSeconds,
+        project,
+        messageHandler,
+        payload,
+        scope,
+        clientSessionId,
+        user,
+        hasRole,
+        hostName,
+        remoteServers,
     )
-    return BasicDataset()
-
 
-def readAsync(tagPaths, callback):
-    # type: (List[AnyStr], Callable[..., Any]) -> None
-    """Asynchronously reads the value of the Tags at the given paths.
 
-    You must provide a python callback function that can process the
-    read results.
+def sendRequest(
+    project,
+    messageHandler,
+    payload=None,
+    hostName=None,
+    remoteServer=None,
+    timeoutSec=None,
+):
+    """This function sends a message to the Gateway, working in a
+    similar manner to the sendMessage function, except sendRequest
+    expects a response to the message.
+
+    To handle received messages, you must set up Gateway Event Script
+    message handlers within a project. These message handlers run Jython
+    code when a message is received. You can then place a return at the
+    end of the code to return something to where the sendRequest was
+    originally called from. You can add message handlers under the
+    "Message" section of the Gateway Event Script configuration dialog.
+
+    Args:
+        project (str): The name of the project containing the message
+            handler.
+        messageHandler (str): The name of the message handler that will
+            fire upon receiving a message.
+        payload (dict): A PyDictionary which will get passed to the
+            message handler. Use "payload" in the message handler to
+            access dictionary variables. Optional.
+        hostName (str): Limits the message delivery to the client that
+            has the specified network host name. Optional.
+        remoteServer (str): A string representing a target Gateway
+            Server name. The message will be delivered to the remote
+            Gateway over the Gateway Network. Upon delivery, the message
+            is distributed to the local Gateway and clients as per the
+            other parameters. Optional.
+        timeoutSec (str): The number of seconds before the sendRequest
+            call times out. Optional.
 
-    Args:
-        tagPaths: A List of Tag paths to read from. If no property is
-            specified in the path, the Value property is assumed.
-        callback: A Python callback function to process the read
-            results. The function definition must provide a single
-            argument, which will hold a List of qualified values when
-            the callback function is invoked. The qualified values will
-            have three sub members: value, quality, and timestamp.
+    Returns:
+        object: The return from the message handler.
     """
-    print(tagPaths, callback)
-
+    print(
+        project,
+        messageHandler,
+        payload,
+        hostName,
+        remoteServer,
+        timeoutSec,
+    )
 
-def readBlocking(tagPaths, timeout=45000):
-    # type: (List[AnyStr], int) -> List[BasicQualifiedValue]
-    """Reads the value of the Tags at the given paths.
 
-    Will block until the read operation is complete or times out.
+def sendRequestAsync(
+    project,
+    messageHandler,
+    payload=None,
+    hostName=None,
+    remoteServer=None,
+    timeoutSec=None,
+    onSuccess=None,
+    onError=None,
+):
+    """This function sends a message to the Gateway and expects a
+    response.
 
-    Args:
-        tagPaths: A List of Tag paths to read from. If no property is
-            specified in a path, the Value property is assumed.
-        timeout: How long to wait in milliseconds before the read
-            operation times out. This parameter is optional, and
-            defaults to 45000 milliseconds if not specified. Optional.
+    Works in a similar manner to the sendRequest function, except
+    sendRequestAsync will send the request and then immediately return a
+    handle for it.
+
+    Args:
+        project (str): The name of the project containing the message
+            handler.
+        messageHandler (str): The name of the message handler that will
+            fire upon receiving a message.
+        payload (dict): A PyDictionary which will get passed to the
+            message handler. Use "payload" in the message handler to
+            access dictionary variables. Optional.
+        hostName (str): Limits the message delivery to the client that
+            has the specified network host name. Optional.
+        remoteServer (str): A string representing the target Gateway
+            Server name. The message will be delivered to the remote
+            Gateway over the Gateway Network. Upon delivery, the message
+            is distributed to the local Gateway and clients as per the
+            other parameters. Optional.
+        timeoutSec (int): The number of seconds before the sendRequest
+            call times out. Optional.
+        onSuccess (object): Should take one argument, which will be the
+            result from the message handler. Callback functions will be
+            executed on the GUI thread, similar to
+            system.util.invokeLater. Optional.
+        onError (object): Should take one argument, which will be the
+            exception encountered. Callback functions will be executed
+            on the GUI thread, similar to system.util.invokeLater.
+            Optional.
 
     Returns:
-        A list of QualifiedValue objects corresponding to the Tag paths.
+        Request: The Request object that can be used while waiting for
+            the message handler callback.
     """
-    print(tagPaths, timeout)
-    return [BasicQualifiedValue() for _ in tagPaths]
+    print(
+        project,
+        messageHandler,
+        payload,
+        hostName,
+        remoteServer,
+        timeoutSec,
+        onSuccess,
+        onError,
+    )
+    return Request()
 
 
-def rename(tag, newName, collisionPollicy="a"):
-    # type: (AnyStr, AnyStr, AnyStr) -> QualityCode
-    """Renames a single Tag or folder.
+def setConnectTimeout(connectTimeout):
+    """Sets the connect timeout for client-to-gateway communication.
 
-    Args:
-        tag: A path to the Tag or folder to rename.
-        newName: The new name for the tag or folder.
-        collisionPollicy: The action to take when a Tag or folder with
-            the same path and names is encountered. Possible values
-            include "a" (Abort, throws an exception), "o" (Overwrite,
-            completely replaces a Tag's configuration), and "i"
-            (Ignore). Defaults to Abort if not specified. Optional.
+    Specified in milliseconds.
 
-    Returns:
-        A QualityCode object that contains the result of the rename
-        operation.
+    Args:
+        connectTimeout (int): The new connect timeout, specified in
+            milliseconds.
     """
-    print(tag, newName, collisionPollicy)
-    return QualityCode()
+    print(connectTimeout)
+
 
+def setConnectionMode(mode):
+    """Sets the connection mode for the client session.
 
-def requestGroupExecution(provider, tagGroup):
-    # type: (AnyStr, AnyStr) -> None
-    """Sends a request to the specified Tag Group to execute now.
+    Normally a client runs in mode 3, which is read-write. You may wish
+    to change this to mode 2, which is read-only, which will only allow
+    reading and subscribing to tags, and running SELECT queries. Tag
+    writes and INSERT / UPDATE / DELETE queries will not function. You
+    can also set the connection mode to mode 1, which is disconnected,
+    all tag and query features will not work.
 
     Args:
-        provider: Name of the Tag Provider that the Tag Group is in.
-        tagGroup: The name of the Tag Group to execute.
+        mode (int): The new connection mode. 1 = Disconnected,
+            2 = Read-only, 3 = Read/Write.
     """
-    print(provider, tagGroup)
+    print(mode)
 
 
-def setOverlaysEnabled(enabled):
-    # type: (bool) -> None
-    """Enables or disables the component quality overlay system.
+def setLocale(locale):
+    """Sets the user's current Locale.
+
+    Any valid Java locale code (case-insensitive) can be used as a
+    parameter, including ones that have not yet been added to the
+    Translation Manager. An invalid locale code will cause an Illegal
+    Argument Exception.
 
     Args:
-        enabled: True to turn on Tag overlays, False to turn
-            them off.
+        locale (str): A locale code, such as 'en_US' for US English.
     """
-    print(enabled)
+    print(locale)
 
 
-def storeAnnotations(
-    paths,  # type: List[AnyStr]
-    startTimes=None,  # type: Optional[List[Date]]
-    endTimes=None,  # type: Optional[List[Date]]
-    types=None,  # type: Optional[List[Annotation]]
-    data=None,  # type: Optional[List[AnyStr]]
-    storageIds=None,  # type: Optional[List[int]]
-    deleted=None,  # type: Optional[List[bool]]
-):
-    # type: (...) -> List[BasicQualifiedValue]
-    """Stores annotations into the Tag history system.
+def setLoggingLevel(loggerName, loggerLevel):
+    """Sets the logging level on the given logger.
 
-    Annotations are stored by the underlying historian implementations,
-    so different providers may store in different ways, and some
-    providers may not support annotation storage. All parameters are
-    1-to-1, so all provided lists should be of the same length. If a
-    particular annotation doesn't need a parameter, that element can be
-    None in the list.
-
-    Args:
-        paths: A list of Tag paths to store for. The paths are
-            equivalent to what would be used for a Tag history query,
-            and should specify the source provider as well. For example,
-            ``"[HistoryProvider/Gateway:Provider]Path/To/Tag"``. This
-            parameter is required, even if storage ids are included,
-            because it is used to identify the underlying storage
-            provider.
-        startTimes: The start times of the events. If omitted, defaults
-            to the current time. Optional.
-        endTimes: The end times of the event, if applicable. If omitted,
-            does not store an end time for the annotation. Optional.
-        types: The type id for the annotation. If not defined, "marker"
-            will be used. See the Annotation Types for more details.
-            Optional.
-        data: Data for the annotation, such as text describing the
-            meaning of the annotation. Optional.
-        storageIds: If defined, the function will instead update the
-            existing annotation instead of adding new ones, overriding
-            existing values for the annotation with those provided by
-            this function (if the corresponding delete parameter is
-            True). Storage id is available on the Annotation object, and
-            is returned as the result value from the storeAnnotations
-            call. Optional.
-        deleted: A list of booleans indicating that the individual
-            annotation should be deleted. Requires storage id to be set
-            as well. Optional.
-
-    Returns:
-        A list of QualifiedValues. The quality code will indicate
-        success or failure. If successful,  the storage id of the
-        annotation will be returned in the value.
-    """
-    print(paths, startTimes, endTimes, types, data, storageIds, deleted)
-    return [BasicQualifiedValue() for _ in paths]
-
-
-def storeTagHistory(
-    historyprovider,  # type: AnyStr
-    tagprovider,  # type: AnyStr
-    paths,  # type: List[AnyStr]
-    values,  # type: List[Any]
-    qualities=None,  # type: Optional[List[int]]
-    timestamps=None,  # type: Optional[List[Date]]
-):
-    # type: (...) -> None
-    """Inserts data into the Tag history system, allowing Tag history to
-    be recorded via scripting.
-
-    The Tag paths are associated with a historical and realtime
-    provider, but they do not necessarily need to exist in the realtime
-    provider. This means records from non-existent (virtual) Tags can be
-    stored in the Tag History system. Because of this, it is imperative
-    that Tag paths passed to the function are typed precisely, otherwise
-    the history will be stored at an incorrect path.
-
-    Note that the Tag History system does cache Tag data. Thus, if this
-    function is called, the Tag path and Tag id are cached until the
-    history provider or gateway are restarted. This means manually
-    removing the Tag from the sqlth_te table, and then calling this
-    function again with the same path will not re-populate the Tag
-    execution table (especially so when working purely with virtual Tag
-    paths). Instead, the cache must first be cleared, and then a new
-    entry will be added the next time this function is called.
-
-    If a Tag's datatype changes after recording Tag history, this
-    function will create a new entry in the sqlth_te table to reflect
-    the change.
-
-    Args:
-        historyprovider: The historical provider to store to.
-        tagprovider: The name of the realtime Tag provider to associate
-            these tags with. The Tag provider does not need to exist,
-            and the Tag paths do not need to exist in it.
-        paths: A list of paths to store. The values, qualities, and
-            timestamps are one-to-one with the paths. A single path may
-            be present multiple times in order to store multiple values.
-        values: A list of values to store.
-        qualities: A list of integer quality codes corresponding to the
-            values. Quality codes can be found on the Tag Quality and
-            Overlays page. If omitted, GOOD quality will be used.
-            Optional.
-        timestamps: A list of Date timestamps corresponding to the
-            values. If omitted, the current time will be used. A
-            java.util.date object may be passed, so the system.date
-            functions can be used to return a timestamp. Optional.
-    """
-    print(historyprovider, tagprovider, paths, values, qualities, timestamps)
+    This can be a logger you create, or a logger already defined in the
+    system.
+
+    Args:
+        loggerName (str): The unique name of the logger to change the
+            logging level on, for example "Tags.Client".
+        loggerLevel (str): The level you want to change to logger to:
+            "trace", "debug", "info", "warn" or "error".
+    """
+    print(loggerName, loggerLevel)
 
 
-def writeAsync(
-    tagPaths,  # type: List[AnyStr]
-    values,  # type: List[Any]
-    callback=None,  # type: Optional[Callable[..., Any]]
-):
-    # type: (...) -> None
-    """Asynchronously writes values to Tags a the given paths.
+def setReadTimeout(readTimeout):
+    """Sets the read timeout for client-to-gateway communication.
 
-    You must provide a Python callback function that can process the
-    write results.
+    Specified in milliseconds.
 
     Args:
-        tagPaths: A List of Tag paths to write to. If no property is
-            specified in a Tag path, the Value property is assumed.
-        values: The values to write to the specified paths.
-        callback: A Python callback function to process the write
-            results. The function definition must provide a single
-            argument: a List of QualityCode objects corresponding to the
-            results of the write operation. Optional.
+        readTimeout (int): The new read timeout, specified in
+            milliseconds.
     """
-    print(tagPaths, values, callback)
+    print(readTimeout)
 
 
-def writeBlocking(
-    tagPaths,  # type: List[AnyStr]
-    values,  # type: List[Any]
-    timeout=45000,  # type: int
-):
-    # type: (...) -> List[QualityCode]
-    """Writes values to Tags at the given paths.
+def threadDump():
+    """Creates a thread dump of the current running JVM.
+
+    Returns:
+        str: The dump of the current running JVM.
+    """
+    return "Ignition version: {}...".format(getVersion())
 
-    This function will block until the write operation is complete or
-    times out.
+
+def translate(term, locale=None, strict=False):
+    """This function allows you to retrieve the global translation of a
+    term from the translation database using the current locale.
 
     Args:
-        tagPaths: A List of Tag paths to write to. If no property is
-            specified in a Tag path, the Value property is assumed.
-        values: The values to write to the specified paths.
-        timeout: How long to wait in milliseconds before the write
-            operation times out. This parameter is optional, and
-            defaults to 45,000 milliseconds if not specified. Optional.
+        term (str): The term to look up.
+        locale (str): Which locale to translate against. Useful when
+            there are multiple locales defined for a single term. If
+            omitted, the function attempts to use the current locale (as
+            defined by the client, session, or Designer). Optional.
+        strict (bool): If False, the function will return the passed
+            term (param 1) if it could not find a defined translation
+            for the locale: meaning, if you pass a term that hasn't been
+            configured, the function will just send the term back to
+            you. If True, then the function will return a None when it
+            fails to find a defined translation. Default is False.
+            Optional.
 
     Returns:
-        A List of QualityCode objects, one for each Tag path.
+        str: The translated term.
     """
-    print(tagPaths, values, timeout)
-    return [QualityCode() for _ in tagPaths]
+    print(term, locale, strict)
+    return term
```

### Comparing `ignition_api-8.1.40/src/system/project.py` & `ignition-api-8.1.9/src/system/project.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Project Functions.
 
 The following functions allow you to list projects on the Gateway
 through scripting.
 """
 
 from __future__ import print_function
 
-__all__ = ["getProjectName", "getProjectNames", "requestScan"]
-
-from typing import List
-
-from dev.coatl.helper.types import AnyStr
+__all__ = ["getProjectName", "getProjectNames"]
 
 
 def getProjectName():
-    # type: () -> AnyStr
     """Returns the name of the project where the function was called
     from.
 
     When called from the Gateway scope from a resource that originates
     from a singular project (reports, SFCs, etc.), will return that
     resources project.
 
@@ -27,43 +26,27 @@
 
     When called from a scope that does not have an associated project
     (a Tag Event Script), the function will return the name of the
     Gateway scripting project. If a Gateway scripting project has not
     been configured, then returns an empty string.
 
     Returns:
-         The name of the currently running project.
+         str: The name of the currently running project.
     """
     return "MyProject"
 
 
 def getProjectNames():
-    # type: () -> List[AnyStr]
     """Returns an unsorted collection of strings, where each string
     represents the name of a project on the Gateway.
 
     If no projects exist, returns an empty list.
 
     This function only ever returns project names, ignoring project
     titles. The function also ignores the "enabled" property, including
     disabled projects in the results.
 
     Returns:
-         A list containing string representations of project names on
-         the Gateway.
+         list[str]: A list containing string representations of project
+            names on the Gateway.
     """
     return ["MyProject", "DisabledProject"]
-
-
-def requestScan(timeout=10):
-    # type: (int) -> None
-    """Requests a manual scan of the projects directory in order to
-    refresh projects and their resources. If a scan is currently
-    running, this method has no effect and will return when the in-
-    progress scan has finished. This function blocks the current thread
-    until a scan has completed.
-
-    Args:
-        timeout: The amount of time, in seconds, to block the current
-            thread before timing out. Default is 10 seconds. Optional.
-    """
-    print(timeout)
```

### Comparing `ignition_api-8.1.40/src/system/dataset.py` & `ignition-api-8.1.9/src/system/dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Dataset Functions.
 
 The following functions give you access to view and interact with
 datasets.
 """
 
 from __future__ import print_function
 
 __all__ = [
+    "Dataset",
+    "PyDataSet",
     "addColumn",
     "addRow",
     "addRows",
     "appendDataset",
     "clearDataset",
     "dataSetToHTML",
     "deleteRow",
@@ -27,615 +33,642 @@
     "toCSV",
     "toDataSet",
     "toExcel",
     "toPyDataSet",
     "updateRow",
 ]
 
-import os.path
-from typing import Any, Dict, List, Optional, Type, Union
+import os
+from collections import Iterable
+
+from java.util import Locale
+
+
+class Dataset(Iterable):
+    """A dataset is a collection of values arranged in a structured
+    format.
+
+    Most datasets are two dimensional -- they can be viewed as a table
+    with rows and columns being the two dimensions. Values in a dataset
+    are usually accessed by specifying one index for each dimension of
+    data (row and column for tables).
+    """
+
+    def __iter__(self):
+        """Return the iterator object itself."""
+        pass
+
+    def getColumnCount(self):
+        """Returns the number of columns in the dataset.
+
+        Returns:
+            int: The number of columns in the dataset.
+        """
+        print(self)
+        return 4
+
+    def getColumnIndex(self, colName):
+        """Returns the index of the column with the name colName.
+
+        Args:
+            colName (str): The name of the column
+
+        Returns:
+            int: The index of the column with the name colName.
+        """
+        print(self, colName)
+        return 2
+
+    def getColumnName(self, colIndex):
+        """Returns the name of the column at the index colIndex.
+
+        Args:
+            colIndex (str): The index of the column.
+
+        Returns:
+            str: The name of the column at the index colIndex.
+        """
+        print(self, colIndex)
+        return "Population"
+
+    def getColumnNames(self):
+        """Returns a list with the names of all the columns.
+
+        Returns:
+            list[str]: A list with the names of all the columns.
+        """
+        print(self)
+        return ["City", "Population", "Timezone", "GMTOffset"]
+
+    def getColumnType(self, colIndex):
+        """Returns the type of the column at the index colIndex.
+
+        Args:
+            colIndex (int): The index of the column.
+
+        Returns:
+            object: The type of the column at the index colIndex.
+        """
+        print(self, colIndex)
+        return type(0)
+
+    def getColumnTypes(self):
+        """Returns a list with the types of all the columns.
+
+        Returns:
+             list[object]: A list with the types of all the columns.
+        """
+        print(self)
+        return [type(""), type(0), type(""), type(0)]
+
+    def getRowCount(self):
+        """Returns the number of rows in the dataset.
+
+        Returns:
+            int: The number of rows in the dataset.
+        """
+        print(self)
+        return 5
+
+    def getValueAt(self, *args):
+        """Returns the value at the specified row index and column name.
 
-from com.inductiveautomation.ignition.common import Dataset
-from com.inductiveautomation.ignition.common.script.builtin import DatasetUtilities
-from dev.coatl.helper.types import AnyNum, AnyStr
-from java.util import Date, Locale
-
-ColType = Union[AnyNum, AnyStr, Date]
-
-
-def addColumn(
-    dataset,  # type: Dataset
-    colIndex,  # type: int
-    col,  # type: List[Any]
-    colName,  # type: AnyStr
-    colType,  # type: Type[ColType]
-):
-    # type: (...) -> Dataset
+        Args:
+            args (object): args[0] = rowIndex, args[1] colIndex or
+                colName.
+
+        Returns:
+            object: The value at the specified row index and column
+                name.
+        """
+        ret = None
+        if isinstance(args[1], int):
+            print(self, "colIndex")
+            ret = "PST"
+        elif isinstance(args[1], str):
+            print(self, "colName")
+            ret = 2853114
+        return ret
+
+
+class PyDataSet(Iterable):
+    """PyDatasets are special, in that they can be handled similarly to
+    other Python sequences.
+    """
+
+    def __add__(self, other):
+        """Add a new element."""
+        pass
+
+    def __iter__(self):
+        """Return the iterator object itself."""
+        pass
+
+    def __len__(self):
+        """Return the number of elements."""
+        pass
+
+
+def addColumn(dataset, colIndex, col, colName, colType):
     """Takes a dataset and returns a new dataset with a new column added
     or inserted into it.
 
-    If the `colIndex` argument is omitted, the column will be appended
-    to the end of the dataset.
+    Datasets are immutable, so it is important to realize that this
+    function does not actually add a column to a dataset. You'll need to
+    do something with the new dataset that this function creates to
+    achieve something useful. If the columnIndex argument is omitted,
+    the column will be appended to the end of the dataset.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
-
-    Args:
-        dataset: The starting dataset. Please be aware that this dataset
-            will not actually be modified (datasets are immutable), but
-            rather will be the starting point for creating a new
-            dataset.
-        colIndex: The index (starting at 0) at which to insert the new
-            column. Will throw an IndexError if less than zero or
+    Args:
+        dataset (Dataset): The starting dataset. Please be aware that
+            this dataset will not actually be modified (datasets are
+            immutable), but rather will be the starting point for
+            creating a new dataset.
+        colIndex (int): The index (starting at 0) at which to insert the
+            new column. Will throw an IndexError if less than zero or
             greater than the length of the dataset. If omitted, the new
             column will be appended to the end. Optional.
-        col: A Python sequence representing the data for the new column.
-            Its length must equal the number of rows in the dataset.
-        colName: The name of the column.
-        colType: The type of the column. The type can be a Python
-            builtin type, such as str, int, float, or a Java class, such
-            as java.util.Date.
+        col (list[object]): A Python sequence representing the data for
+            the new column. Its length must equal the number of rows in
+            the dataset.
+        colName (str): The name of the column.
+        colType (type): The type of the of the column. The type can be
+            the Python equivalent of String, Long, Double, Short,
+            Integer, Float, Boolean, null, or java.util.Date if they
+            exist.
 
     Returns:
-        A new dataset with the new column inserted or appended.
+        Dataset: A new dataset with the new column inserted or appended.
     """
     print(dataset, colIndex, col, colName, colType)
     return Dataset()
 
 
 def addRow(dataset, rowIndex, row):
-    # type: (Dataset, int, List[Any]) -> Dataset
     """Takes a dataset and returns a new dataset with a new row added or
     inserted into it.
 
-    If the `rowIndex` argument is omitted, the column will be appended
-    to the end of the dataset.
+    Datasets are immutable, so it is important to realize that this
+    function does not actually add a row to a dataset. You'll need to do
+    something with the new dataset that this function creates to achieve
+    something useful. If the rowIndex argument is omitted, the row will
+    be appended to the end of the dataset.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
-
-    Args:
-        dataset: The starting dataset. Please be aware that this dataset
-            will not actually be modified (datasets are immutable), but
-            rather will be the starting point for creating a new
-            dataset.
-        rowIndex: The index (starting at 0) at which to insert the new
-            row. Will throw an IndexError if less than zero or greater
-            than the length of the dataset. If omitted, the new row will
-            be appended to the end. Optional.
-        row: A Python sequence representing the data for the new row.
-            Its length must equal the number of columns in the dataset.
+    Args:
+        dataset (Dataset): The starting dataset. Please be aware that
+            this dataset will not actually be modified (datasets are
+            immutable), but rather will be the starting point for
+            creating a new dataset.
+        rowIndex (int): The index (starting at 0) at which to insert the
+            new row. Will throw an IndexError if less than zero or
+            greater than the length of the dataset. If omitted, the new
+            row will be appended to the end. Optional.
+        row (list[object]): A Python sequence representing the data for
+            the new row. Its length must equal the number of columns in
+            the dataset.
 
     Returns:
-        A new dataset with the new row inserted or appended.
+        Dataset: A new dataset with the new row inserted or appended.
     """
     print(dataset, rowIndex, row)
     return Dataset()
 
 
 def addRows(dataset, rowIndex, rows):
-    # type: (Dataset, int, List[List[Any]]) -> Dataset
     """Takes a dataset and returns a new dataset with a new row added or
     inserted into it.
 
-    If the `rowIndex` argument is omitted, the column will be appended
-    to the end of the dataset.
+    Datasets are immutable, so it is important to realize that this
+    function does not actually add a row to a dataset. You'll need to do
+    something with the new dataset that this function creates to achieve
+    something useful. If the rowIndex argument is omitted, the row will
+    be appended to the end of the dataset.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
-
-    Args:
-        dataset: The starting dataset. Please be aware that this dataset
-            will not actually be modified (datasets are immutable), but
-            rather will be the starting point for creating a new
-            dataset.
-        rowIndex: The index (starting at 0) at which to insert the new
-            row. Will throw an IndexError if less than zero or greater
-            than the length of the dataset. If omitted, the new row will
-            be appended to the end. Optional.
-        rows: A Python sequence of sequences representing the data for
+    Args:
+        dataset (Dataset): The starting dataset. Please be aware that
+            this dataset will not actually be modified (datasets are
+            immutable), but rather will be the starting point for
+            creating a new dataset.
+        rowIndex (int): The index (starting at 0) at which to insert the
+            new row. Will throw an IndexError if less than zero or
+            greater than the length of the dataset. If omitted, the new
+            row will be appended to the end. Optional.
+        rows (list[object]): A Python sequence representing the data for
             the new rows. The length of each sequence must equal the
             number of columns in the dataset.
 
     Returns:
-        A new dataset with the new row inserted or appended.
+        Dataset: A new dataset with the new row inserted or appended.
     """
     print(dataset, rowIndex, rows)
     return Dataset()
 
 
 def appendDataset(dataset1, dataset2):
-    # type: (Dataset, Dataset) -> Dataset
     """Takes two different datasets and returns a new dataset with the
     second dataset appended to the first.
 
     Will throw an error if the number and types of columns do not match.
 
     Args:
-        dataset1: The dataset that will come first in the returned
-            dataset.
-        dataset2: The second dataset that will be appended to the end in
-            the returned dataset.
+        dataset1 (Dataset): The dataset that will come first in the
+            returned dataset.
+        dataset2 (Dataset): The second dataset that will be appended to
+            the end in the returned dataset.
 
     Returns:
-        A new dataset that is a combination of the original two
-        datasets.
+        Dataset: A new dataset that is a combination of the original two
+            datasets.
     """
     print(dataset1, dataset2)
     return Dataset()
 
 
 def clearDataset(dataset):
-    # type: (Dataset) -> Dataset
     """Takes a dataset and returns a new dataset with all of the same
     column names, but all of the rows deleted.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
-
     Args:
-        dataset: The starting dataset.
+        dataset (Dataset): The starting dataset. If NULL, a NULL dataset
+            will be returned.
 
     Returns:
-        A new dataset with no data.
+        Dataset: A new dataset with no data.
     """
     print(dataset)
     return Dataset()
 
 
 def dataSetToHTML(showHeaders, dataset, title):
-    # type: (bool, Dataset, AnyStr) -> AnyStr
     """Formats the contents of a dataset as an HTML page, returning the
     results as a string.
 
     Uses the <table> element to create a data table page.
 
     Args:
-        showHeaders: If True, the HTML table will include a header
-            row.
-        dataset: The dataset to export.
-        title: The title for the HTML page.
+        showHeaders (bool): If True(1), the HTML table will include a
+            header row.
+        dataset (Dataset): The dataset to export.
+        title (str): The title for the HTML page.
 
     Returns:
-        The HTML page as a string.
+        str: The HTML page as a string.
     """
     print(showHeaders, dataset, title)
     return "<html><head>{}</head><body>data</body></html>".format(title)
 
 
 def deleteRow(dataset, rowIndex):
-    # type: (Dataset, int) -> Dataset
     """Takes a dataset and returns a new dataset with a row removed.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
+    Datasets are immutable, so it is important to realize that this
+    function does not actually remove the row from the argument dataset.
+    You'll need to do something with the new dataset that this function
+    creates to achieve something useful.
 
     Args:
-        dataset: The starting dataset. Please be aware that this dataset
-            will not actually be modified (datasets are immutable), but
-            rather will be the starting point for creating a new
-            dataset.
-        rowIndex: The index (starting at 0) of the row to delete.
+        dataset (Dataset): The starting dataset. Please be aware that
+            this dataset will not actually be modified (datasets are
+            immutable), but rather will be the starting point for
+            creating a new dataset.
+        rowIndex (int): The index (starting at 0) of the row to delete.
 
     Returns:
-        A new dataset with the specified row removed.
+        Dataset: A new dataset with the specified row removed.
 
     Raises:
         IndexError: If rowIndex is less than zero or greater than the
             row count of the dataset -1.
     """
     print(dataset, rowIndex)
     if rowIndex < 0:
         raise IndexError("Error")
 
     return Dataset()
 
 
 def deleteRows(dataset, rowIndices):
-    # type: (Dataset, List[int]) -> Dataset
     """Takes a dataset and returns a new dataset with one or more rows
     removed.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
+    Datasets are immutable, so it is important to realize that this
+    function does not actually remove the rows from the argument
+    dataset. You'll need to do something with the new dataset that this
+    function creates to achieve something useful.
 
     Args:
-        dataset: The starting dataset. Please be aware that this dataset
-            will not actually be modified (datasets are immutable), but
-            rather will be the starting point for creating a new
-            dataset.
-        rowIndices: The indices (starting at 0) of the rows to delete.
+        dataset (Dataset): The starting dataset. Please be aware that
+            this dataset will not actually be modified (datasets are
+            immutable), but rather will be the starting point for
+            creating a new dataset.
+        rowIndices (list[int]): The indices (starting at 0) of the rows
+            to delete.
 
     Returns:
-        A new dataset with the specified row removed.
+        Dataset: A new dataset with the specified row removed.
 
     Raises:
         IndexError: If any element is less than zero or greater than the
             number of rows in the dataset - 1.
     """
     print(dataset, rowIndices)
     if -1 in rowIndices:
         raise IndexError("Error")
 
     return Dataset()
 
 
 def exportCSV(filename, showHeaders, dataset):
-    # type: (AnyStr, bool, Dataset) -> AnyStr
     """Exports the contents of a dataset as a CSV file, prompting the
     user to save the file to disk.
 
-    To write silently to a file, you cannot use the `dataset.export*`
-    functions. Instead, use the `toCSV()` function.
-
     Args:
-        filename: A suggested filename to save as.
-        showHeaders: If True, the CSV file will include a header
-            row.
-        dataset: The dataset to export.
+        filename (str): A suggested filename to save as.
+        showHeaders (bool): If True (1), the CSV file will include a
+            header row.
+        dataset (Dataset): The dataset to export.
 
     Returns:
-        The path to the saved file, or None if the action was canceled
-        by the user.
+        str: The path to the saved file, or None if the action was
+            canceled by the user.
     """
     print(filename, showHeaders, dataset)
     return os.path.expanduser("~")
 
 
-def exportExcel(
-    filename,  # type: AnyStr
-    showHeaders,  # type: bool
-    dataset,  # type: Union[Dataset, List[Dataset]]
-    nullsEmpty=False,  # type: bool
-):
-    # type: (...) -> AnyStr
+def exportExcel(filename, showHeaders, dataset, nullsEmpty=False):
     """Exports the contents of a dataset as an Excel spreadsheet,
-    prompting the user to save the file to disk.
-
-    Uses the same format as the dataSetToExcel function.
-
-    To write silently to a file, you cannot use the `dataset.export*`
-    functions. Instead, use the `toExcel()` function.
+    prompting the user to save the file to disk. Uses the same format as
+    the toExcel function.
 
     Args:
-        filename: A suggested filename to save as.
-        showHeaders: If True, the spreadsheet will include a header
-            row.
-        dataset: Either a single dataset, or a list of datasets. When
-            passing a list, each element represents a single sheet in
-            the resulting workbook.
-        nullsEmpty: If True, the spreadsheet will leave cells with NULL
-            values empty, instead of allowing Excel to provide a default
-            value like 0. Defaults to False. Optional.
+        filename (str): A suggested filename to save as.
+        showHeaders (bool): If True (1), the spreadsheet will include a
+            header row.
+        dataset (list[Dataset]): A sequence of datasets, one for each
+            sheet in the resulting workbook.
+        nullsEmpty (bool): If True (1), the spreadsheet will leave cells
+            with NULL values empty, instead of allowing Excel to provide
+            a default value like 0. Defaults to False. Optional.
 
     Returns:
-        The path to the saved file, or None if the action was canceled
-        by the user.
+        str: The path to the saved file, or None if the action was
+            canceled by the user.
     """
     print(filename, showHeaders, dataset, nullsEmpty)
     return os.path.expanduser("~")
 
 
 def exportHTML(filename, showHeaders, dataset, title):
-    # type: (AnyStr, bool, Dataset, AnyStr) -> AnyStr
     """Exports the contents of a dataset to an HTML page.
 
     Prompts the user to save the file to disk.
 
     Args:
-        filename: A suggested filename to save as.
-        showHeaders: If True, the HTML table will include a header
-            row.
-        dataset: The dataset to export.
-        title: The title for the HTML page.
+        filename (str): A suggested filename to save as.
+        showHeaders (bool): If True (1), the HTML table will include a
+            header row.
+        dataset (Dataset): The dataset to export.
+        title (str): The title for the HTML page.
 
     Returns:
-        The path to the saved file, or None if the action was canceled
-        by the user.
+        str: The path to the saved file, or None if the action was
+            canceled by the user.
     """
     print(filename, showHeaders, dataset, title)
     return os.path.expanduser("~")
 
 
-def filterColumns(
-    dataset,  # type: Dataset
-    columns,  # type: Union[List[AnyStr], List[int]]
-):
-    # type: (...) -> Dataset
+def filterColumns(dataset, columns):
     """Takes a dataset and returns a view of the dataset containing only
     the columns found within the given list of columns.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
-
     Args:
-        dataset: The starting dataset.
-        columns: A list of columns to keep in the returned dataset. The
-            columns may be in integer index form (starting at 0), or the
-            name of the columns as Strings.
+        dataset (Dataset): The starting dataset.
+        columns (list[object]): A list of columns to keep in the
+            returned dataset. The columns may be in integer index form
+            (starting at 0), or the name of the columns as Strings.
 
     Returns:
-        A new dataset containing the filtered columns.
+        Dataset: A new dataset containing the filtered columns.
     """
     print(dataset, columns)
     return Dataset()
 
 
 def formatDates(dataset, dateFormat, locale=Locale.ENGLISH):
-    # type: (Dataset, AnyStr, Optional[Locale]) -> Dataset
     """Returns a new dataset with Date columns as strings formatted
     according to the dateFormat specified.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
-
     Args:
-        dataset: The starting dataset to format.
-        dateFormat: A valid Java DateFormat string such as
+        dataset (Dataset): The starting dataset to format.
+        dateFormat (str): A valid Java DateFormat string such as
             "yyyy-MM-dd HH:mm:ss". See system.date.format for more
             information on the valid characters.
-        locale: The Locale to use for formatting. If no Locale is
-            specified, the default Locale will be used. Optional.
+        locale (Locale): The Locale to use for formatting. If no Locale
+            is specified, the default Locale will be used. Optional.
 
     Returns:
-        A new dataset, containing the formatted dates.
+        Dataset: A new dataset, containing the formatted dates.
     """
     print(dataset, dateFormat, locale)
     return Dataset()
 
 
 def fromCSV(csv):
-    # type: (AnyStr) -> Dataset
     """Converts a dataset stored in a CSV formatted string to a dataset
     that can be immediately assignable to a dataset property in your
     project.
 
-    Usually this is used in conjunction with `readFileAsString` when
-    reading in a CSV file that was exported using `toCSV`. The CSV
-    string must be formatted in a specific way.
+    Usually this is used in conjunction with
+    system.file.readFileAsString when reading in a CSV file that was
+    exported using system.dataset.toCSV. The CSV string must be
+    formatted in a specific way.
 
     Args:
-        csv: A string holding a CSV dataset.
+        csv (str): A string holding a CSV dataset.
 
     Returns:
-        A new dataset.
+        Dataset: A new dataset.
     """
     print(csv)
     return Dataset()
 
 
 def getColumnHeaders(dataset):
-    # type: (Dataset) -> List[AnyStr]
     """Takes in a dataset and returns the headers as a python list.
 
     Args:
-        dataset: The input dataset.
+        dataset (Dataset): The input dataset.
 
     Returns:
-        A list of column header strings.
+        list[str]: A list of column header strings.
     """
     print(dataset)
-    return ["column1", "column2"]
+    return []
 
 
-def setValue(dataset, rowIndex, columnNameOrIndex, value):
-    # type: (Dataset, int, Union[AnyStr, int], Any) -> Dataset
+def setValue(dataset, rowIndex, columnName, value):
     """Takes a dataset and returns a new dataset with a one value
     altered.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
+    Datasets are immutable, so it is important to realize that this
+    function does not actually set a value in the argument dataset.
+    You'll need to do something with the new dataset that this function
+    creates to achieve something useful.
 
     Args:
-        dataset: The starting dataset. Will not be modified (datasets
-            are immutable), but acts as the basis for the returned
-            dataset.
-        rowIndex: The index of the row to set the value at (starting at
-            0).
-        columnNameOrIndex: The name of the column to set the value at,
-            or the index of the column to set the value at (starting at
-            0).
-        value: The new value for the specified row/column.
+        dataset (Dataset): The starting dataset. Will not be modified
+            (datasets are immutable), but acts as the basis for the
+            returned dataset.
+        rowIndex (int): The index of the row to set the value at
+            (starting at 0).
+        columnName (str): The name of the column to set the value at.
+            Case insensitive.
+        value (object): The new value for the specified row/column.
 
     Returns:
-         A new dataset, with the new value set at the given location.
+         Dataset: A new dataset, with the new value set at the given
+            location.
     """
-    print(dataset, rowIndex, columnNameOrIndex, value)
+    print(dataset, rowIndex, columnName, value)
     return Dataset()
 
 
-def sort(
-    dataset,  # type: Dataset
-    keyColumn,  # type: Union[AnyStr, int]
-    ascending=True,  # type: bool
-    naturalOrdering=True,  # type: bool
-):
-    # type: (...) -> Dataset
-    """Takes a dataset and returns a sorted version of dataset.
-
-    The sort order is determined by a single column. This works on
-    numeric, as well as alphanumeric columns.
+def sort(dataset, keyColumn, ascending=True):
+    """Sorts a dataset and returns the sorted dataset.
 
-    When sorting alphanumerically, contiguous numbers are treated as a
-    single number: you may recognize this as a "natural sort".
-
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
+    This works on numeric, as well as alphanumeric columns. It will go
+    character by character, going from 0-9, A-Z, a-z.
 
     Args:
-        dataset: The dataset to sort.
-        keyColumn: The index or column name to sort on.
-        ascending: True for ascending order, False for descending order.
-            If omitted, ascending order will be used. Optional.
-        naturalOrdering: True for natural ordering, False for
-            alphabetical ordering. Ignored if the sort column is a
-            directly sortable data type. If omitted, defaults to True
-            (natural ordering). Optional.
+        dataset (Dataset): The dataset to sort.
+        keyColumn (object): The index or column name of the column to
+            sort on.
+        ascending (bool): True for ascending order, False for descending
+            order. If omitted, ascending order will be used. Optional.
 
     Returns:
-        A new sorted dataset.
+        Dataset: A new sorted dataset.
     """
-    print(dataset, keyColumn, ascending, naturalOrdering)
+    print(dataset, keyColumn, ascending)
     return Dataset()
 
 
-def toCSV(
-    dataset,  # type: Dataset
-    showHeaders=True,  # type: bool
-    forExport=False,  # type: bool
-    localized=False,  # type: bool
-):
-    # type: (...) -> AnyStr
+def toCSV(dataset, showHeaders=True, forExport=False, localized=False):
     """Formats the contents of a dataset as CSV (comma separated
     values), returning the resulting CSV as a string.
 
     If the "forExport" flag is set, then the format will be appropriate
-    for parsing using the `fromCSV` function.
+    for parsing using the system.dataset.fromCSV function.
 
     Args:
-        dataset: The dataset to export to CSV.
-        showHeaders: If set to True, a header row will be present in
-            the CSV. Default is True. Optional.
-        forExport: If set to True, extra header information will be
-            present in the CSV data which is necessary for the CSV to be
-            compatible with the fromCSV method. Overrides showHeaders.
-            Default is False. Optional.
-        localized: If set to True, the string representations of the
-            values in the CSV data will be localized. Default is
-            False. Optional.
+        dataset (Dataset): The dataset to export to CSV.
+        showHeaders (bool): If set to True(1), a header row will be
+            present in the CSV. Default is True(1). Optional.
+        forExport (bool): If set to True(1), extra header information
+            will be present in the CSV data which is necessary for the
+            CSV to be compatible with the fromCSV method. Overrides
+            showHeaders. Default is False(0). Optional.
+        localized (bool): If set to True(1), the string representations
+            of the values in the CSV data will be localized. Default is
+            False(0). Optional.
 
     Returns:
-        The CSV data as a string.
+        str: The CSV data as a string.
     """
     print(dataset, showHeaders, forExport, localized)
     return ""
 
 
 def toDataSet(*args):
-    # type: (*Any) -> Dataset
     """This function is used to convert PyDataSets to DataSets, and to
     create new datasets from raw Python lists.
 
     When creating a new dataset, headers should have unique names.
 
     1) system.dataset.toDataSet(dataset)
     2) system.dataset.toDataSet(headers, data)
 
     Args:
         args: A variable-length argument list.
 
     Returns:
-        The newly created dataset.
+        Dataset: The newly created dataset.
     """
-    print(args)
+    for arg in args:
+        print(arg)
     return Dataset()
 
 
-def toExcel(
-    showHeaders,  # type: bool
-    dataset,  # type: List[Dataset]
-    nullsEmpty=False,  # type: bool
-    sheetNames=None,  # type: Optional[List[AnyStr]]
-):
-    # type: (...) -> Any
-    """Formats the contents of one or more datasets as an Excel
-    spreadsheet, returning the results as a byte array.
+def toExcel(showHeaders, dataset, nullsEmpty=False, sheetNames=None):
+    """Formats the contents of one or more datasets as an excel
+    spreadsheet, returning the results as a string.
 
     Each dataset specified will be added as a worksheet in the Excel
-    workbook.
+    workbook. This function uses an xml-format for Excel spreadsheets,
+    not the native Excel file format.
 
     Args:
-        showHeaders: If True, the spreadsheet will include a header row.
-            If False, the header row will be omitted.
-        dataset: A sequence of one or more datasets, one for each sheet
-            in the resulting workbook.
-        nullsEmpty: If True, the spreadsheet will leave cells with
-            NULL values empty, instead of allowing Excel to provide a
-            default value like 0. Defaults to False. Optional.
-        sheetNames: Expects a list of strings, where each string is a
-            name for one of the datasets. When used, there must be an
-            equal number of string names in sheetName as there are
-            datasets in the dataset parameter. Names provided in this
-            parameter may be sanitized into acceptable Excel sheet
-            names. Optional.
+        showHeaders (bool): If True, the spreadsheet will include a
+            header row. If False, the header row will be omitted.
+        dataset (list[Dataset]): A sequence of one or more datasets,
+            one for each sheet in the resulting workbook.
+        nullsEmpty (bool): If True (1), the spreadsheet will leave cells
+            with NULL values empty, instead of allowing Excel to provide
+            a default value like 0. Defaults to False. Optional.
+        sheetNames (list[str]): Expects a list of strings, where each
+            string is a name for one of the datasets. When used, there
+            must be an equal number of string names in sheetName as
+            there are datasets in the dataset parameter. Names provided
+            in this parameter may be sanitized into acceptable Excel
+            sheet names. Optional.
 
     Returns:
-        A byte array representing an Excel workbook.
+        str: An Excel-compatible XML-based workbook, with one worksheet
+            per dataset.
     """
     print(showHeaders, dataset, nullsEmpty, sheetNames)
 
 
 def toPyDataSet(dataset):
-    # type: (Dataset) -> DatasetUtilities.PyDataSet
     """This function converts from a normal DataSet to a PyDataSet,
     which is a wrapper class which makes working with datasets more
     Python-esque.
 
     Args:
-        dataset: A Dataset object to convert into a PyDataSet.
+        dataset (Dataset): A DataSet object to convert into a PyDataSet.
 
     Returns:
-        The newly created PyDataSet.
+        PyDataSet: The newly created PyDataSet.
     """
     print(dataset)
-    return DatasetUtilities.PyDataSet()
+    return PyDataSet()
 
 
 def updateRow(dataset, rowIndex, changes):
-    # type: (Dataset, int, Dict[AnyStr, Any]) -> Dataset
     """Takes a dataset and returns a new dataset with a one row altered.
 
+    Datasets are immutable, so it is important to realize that this
+    function does not actually change the row in the argument dataset.
+    You'll need to do something with the new dataset that this function
+    creates to achieve something useful.
+
     To alter the row, this function takes a Python dictionary to
     represent the changes to make to the specified row. The keys in the
     dictionary are used to find the columns to alter.
 
-    Note:
-        Datasets are immutable, which means they cannot be directly
-        modified once created. Instead, this scripting function returns
-        a new dataset with some modification applied, which must be
-        assigned to a variable to be used.
-
     Args:
-        dataset: The starting dataset. Will not be modified (datasets
-            are immutable), but acts as the basis for the returned
-            dataset.
-        rowIndex: The index of the row to update (starting at 0).
-        changes: A Dictionary of changes to make. They keys in the
-            dictionary should match column names in the dataset, and
+        dataset (Dataset): The starting dataset. Will not be modified
+            (datasets are immutable), but acts as the basis for the
+            returned dataset.
+        rowIndex (int): The index of the row to update (starting at 0).
+        changes (dict): A Dictionary of changes to make. They keys in
+            the dictionary should match column names in the dataset, and
             their values will be used to update the row.
 
     Returns:
-         A new dataset with the values at the specified row updated
-         according to the values in the dictionary.
+         Dataset: A new dataset with the values at the specified row
+            updated according to the values in the dictionary.
     """
     print(dataset, rowIndex, changes)
     return Dataset()
```

### Comparing `ignition_api-8.1.40/src/system/serial.py` & `ignition-api-8.1.9/src/system/serial.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,33 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Serial Functions.
 
 The following functions give you access to read and write through serial
 ports.
 """
 
 from __future__ import print_function
 
 __all__ = [
-    "BIT_RATE_110",
-    "BIT_RATE_115200",
-    "BIT_RATE_1200",
-    "BIT_RATE_150",
-    "BIT_RATE_19200",
-    "BIT_RATE_230400",
-    "BIT_RATE_2400",
-    "BIT_RATE_300",
-    "BIT_RATE_38400",
-    "BIT_RATE_460800",
-    "BIT_RATE_4800",
-    "BIT_RATE_57600",
-    "BIT_RATE_600",
-    "BIT_RATE_921600",
-    "BIT_RATE_9600",
-    "DATA_BITS_5",
-    "DATA_BITS_6",
-    "DATA_BITS_7",
-    "DATA_BITS_8",
-    "HANDSHAKE_CTS_DTR",
-    "HANDSHAKE_CTS_RTS",
-    "HANDSHAKE_DSR_DTR",
-    "HANDSHAKE_HARD_IN",
-    "HANDSHAKE_HARD_OUT",
-    "HANDSHAKE_NONE",
-    "HANDSHAKE_SOFT_IN",
-    "HANDSHAKE_SOFT_OUT",
-    "HANDSHAKE_SPLIT_MASK",
-    "HANDSHAKE_XON_XOFF",
-    "PARITY_EVEN",
-    "PARITY_MARK",
-    "PARITY_NONE",
-    "PARITY_ODD",
-    "PARITY_SPACE",
-    "STOP_BITS_1",
-    "STOP_BITS_2",
     "closeSerialPort",
     "configureSerialPort",
     "openSerialPort",
     "port",
     "readBytes",
     "readBytesAsString",
     "readLine",
     "readUntil",
     "sendBreak",
     "write",
     "writeBytes",
 ]
 
-from typing import Any, List, Optional
-
-from com.inductiveautomation.ignition.modules.serial.scripting import SerialScriptModule
-from dev.coatl.helper.types import AnyStr
-
 # Bit rate constants.
 BIT_RATE_110 = 110
 BIT_RATE_150 = 150
 BIT_RATE_300 = 300
 BIT_RATE_600 = 600
 BIT_RATE_1200 = 1200
 BIT_RATE_2400 = 2400
@@ -104,108 +67,137 @@
 PARITY_NONE = 0
 
 # Stop bits constants.
 STOP_BITS_1 = 1
 STOP_BITS_2 = 3
 
 
+class PortManager(object):
+    def __init__(self):
+        pass
+
+    def __enter__(self):
+        print("Enter")
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        print("Exit")
+
+
+class SerialConfigurator(object):
+    """Serial Configurator class."""
+
+    def setBitRate(self, value):
+        pass
+
+    def setDataBits(self, value):
+        pass
+
+    def setFlowControl(self, value):
+        pass
+
+    def setHandshake(self, value):
+        pass
+
+    def setHardwareFlowControl(self, value):
+        pass
+
+    def setParity(self, value):
+        pass
+
+    def setStopBits(self, value):
+        pass
+
+
 def closeSerialPort(port):
-    # type: (AnyStr) -> None
     """Closes a previously opened serial port.
 
     Returns without doing anything if the named serial port is not
     currently open. Will throw an exception if the port is open and
     cannot be closed.
 
     Args:
-        port: The name of the serial port, e.g., "COM1" or "dev/ttyS0".
+        port (str): The name of the serial port, e.g., "COM1" or
+            "dev/ttyS0".
     """
     print(port)
 
 
 def configureSerialPort(
-    port,  # type: AnyStr
-    bitRate=None,  # type: Optional[int]
-    dataBits=None,  # type: Optional[int]
-    handshake=None,  # type: Optional[int]
-    hardwareFlowControl=None,  # type: Optional[bool]
-    parity=None,  # type: Optional[int]
-    stopBits=None,  # type: Optional[int]
+    port, bitRate, dataBits, handshake, hardwareFlowControl, parity, stopBits
 ):
-    # type: (...) -> SerialScriptModule.SerialConfigurator
     """Configure a serial port for use in a later call.
 
     This only needs to be done once unless the configuration has changed
     after the initial call. All access to constants must be prefixed by
     "system.serial.".
 
     Args:
-        port: The name of the serial port, e.g., "COM1" or "/dev/ttyS0".
-            This parameter is required.
-        bitRate: Configure the bit rate. Valid values are defined by the
-            following constants: BIT_RATE_110, BIT_RATE_150,
+        port (str): The name of the serial port, e.g., "COM1" or
+            "/dev/ttyS0". This parameter is required.
+        bitRate (int): Configure the bit rate. Valid values are defined
+            by the following constants: BIT_RATE_110, BIT_RATE_150,
             BIT_RATE_300, BIT_RATE_600, BIT_RATE_1200, BIT_RATE_2400,
             BIT_RATE_4800, BIT_RATE_9600, BIT_RATE_19200,
             BIT_RATE_38400, BIT_RATE_57600, BIT_RATE_115200,
-            BIT_RATE_230400, BIT_RATE_460800, BIT_RATE_921600. Optional.
-        dataBits: Configure the data bits. Valid values are defined by
-            the following constants: DATA_BITS_5, DATA_BITS_6,
-            DATA_BITS_7, DATA_BITS_8. Optional.
-        handshake: Configure the handshake. Valid values are defined by
-            the following constants: HANDSHAKE_CTS_DTR,
+            BIT_RATE_230400, BIT_RATE_460800, BIT_RATE_921600.
+        dataBits (int): Configure the data bits. Valid values are
+            defined by the following constants: DATA_BITS_5,
+            DATA_BITS_6, DATA_BITS_7, DATA_BITS_8.
+        handshake (int): Configure the handshake. Valid values are
+            defined by the following constants: HANDSHAKE_CTS_DTR,
             HANDSHAKE_CTS_RTS, HANDSHAKE_DSR_DTR, HANDSHAKE_HARD_IN,
             HANDSHAKE_HARD_OUT, HANDSHAKE_NONE, HANDSHAKE_SOFT_IN,
             HANDSHAKE_SOFT_OUT, HANDSHAKE_SPLIT_MASK,
-            HANDSHAKE_XON_XOFF. Optional.
-        hardwareFlowControl: Configure hardware flow control. On or off.
-        parity: Configure parity. Valid values are defined by the
+            HANDSHAKE_XON_XOFF.
+        hardwareFlowControl (bool): Configure hardware flow control. On
+            or off.
+        parity (int): Configure parity. Valid values are defined by the
             following constants: PARITY_EVEN, PARITY_ODD, PARITY_MARK,
-            PARITY_SPACE, PARITY_NONE. Optional.
-        stopBits: Configure stop bits. Valid values are defined by the
-            following constants: STOP_BITS_1, STOP_BITS_2. Optional.
+            PARITY_SPACE, PARITY_NONE.
+        stopBits (int): Configure stop bits. Valid values are defined by
+            the following constants: STOP_BITS_1, STOP_BITS_2.
 
     Returns:
-        A SerialConfigurator object with exposed functions that can be
-        used to configure the serial port instead of, or in addition to,
-        the arguments passed to configureSerialPort.
+        SerialConfigurator: A SerialConfigurator that can be used to
+            configure the serial port instead of or in addition to the
+            given keyword arguments.
     """
     print(
         port,
         bitRate,
         dataBits,
         handshake,
         hardwareFlowControl,
         parity,
         stopBits,
     )
-    return SerialScriptModule.SerialConfigurator()
+    return SerialConfigurator()
 
 
 def openSerialPort(port):
-    # type: (AnyStr) -> None
     """Opens a previously configured serial port for use.
 
     Will throw an exception if the serial port cannot be opened.
 
     Args:
-        port: The name of the serial port, e.g., "COM1" or "dev/ttyS0".
+        port (str): The name of the serial port, e.g., "COM1" or
+            "dev/ttyS0".
     """
     print(port)
 
 
 def port(
-    port,  # type: AnyStr
-    bitRate=None,  # type: Optional[int]
-    dataBits=None,  # type: Optional[int]
-    handshake=None,  # type: Optional[int]
-    hardwareFlowControl=None,  # type: Optional[bool]
-    parity=None,  # type: Optional[int]
-    stopBits=None,  # type: Optional[int]
+    port,
+    bitRate=None,
+    dataBits=None,
+    handshake=None,
+    hardwareFlowControl=None,
+    parity=None,
+    stopBits=None,
 ):
-    # type: (...) -> SerialScriptModule.PortManager
     """Returns a context manager wrapping a serial port, allowing the
     rest of the system to interact with that port.
 
     This function effectively combines the
     system.serial.configureSerialPort, system.serial.openSerialPort,
     and system.serial.closeSerialPort functions into a single call.
 
@@ -217,189 +209,175 @@
     ends.
 
     Accepts the same arguments as configureSerialPort, and access to
     constants must be prefixed by "system.serial." As shown in the
     parameter descriptions.
 
     Args:
-        port: The name of the serial port, e.g., "COM1" or "dev/ttyS0".
-        bitRate: Configure the bit rate. Valid values are defined by the
-            following constants: BIT_RATE_110, BIT_RATE_150,
+        port (str): The name of the serial port, e.g., "COM1" or
+            "dev/ttyS0".
+        bitRate (int): Configure the bit rate. Valid values are defined
+            by the following constants: BIT_RATE_110, BIT_RATE_150,
             BIT_RATE_300, BIT_RATE_600, BIT_RATE_1200, BIT_RATE_2400,
             BIT_RATE_4800, BIT_RATE_9600, BIT_RATE_19200,
             BIT_RATE_38400, BIT_RATE_57600, BIT_RATE_115200,
             BIT_RATE_230400, BIT_RATE_460800, BIT_RATE_921600. Optional.
-        dataBits: Configure the data bits. Valid values are defined by
-            the following constants: DATA_BITS_5, DATA_BITS_6,
-            DATA_BITS_7, DATA_BITS_8. Optional.
-        handshake: Configure the handshake. Valid values are defined by
-            the following constants: HANDSHAKE_CTS_DTR,
+        dataBits (int): Configure the data bits. Valid values are
+            defined by the following constants: DATA_BITS_5,
+            DATA_BITS_6, DATA_BITS_7, DATA_BITS_8. Optional.
+        handshake (int): Configure the handshake. Valid values are
+            defined by the following constants: HANDSHAKE_CTS_DTR,
             HANDSHAKE_CTS_RTS, HANDSHAKE_DSR_DTR, HANDSHAKE_HARD_IN,
             HANDSHAKE_HARD_OUT, HANDSHAKE_NONE, HANDSHAKE_SOFT_IN,
             HANDSHAKE_SOFT_OUT, HANDSHAKE_SPLIT_MASK,
             HANDSHAKE_XON_XOFF. Optional.
-        hardwareFlowControl: Configure hardware flow control. On or off.
-            Optional.
-        parity: Configure parity. Valid values are defined by the
+        hardwareFlowControl (bool): Configure hardware flow control. On
+            or off. Optional.
+        parity (int): Configure parity. Valid values are defined by the
             following constants: PARITY_EVEN, PARITY_ODD, PARITY_MARK,
             PARITY_SPACE, PARITY_NONE. Optional.
-        stopBits: Configure stop bits. Valid values are defined by the
-            following constants: STOP_BITS_1, STOP_BITS_2. Optional.
+        stopBits (int): Configure stop bits. Valid values are defined by
+            the following constants: STOP_BITS_1, STOP_BITS_2. Optional.
 
     Returns:
-        A wrapper around the configured port, that can be entered by
-        using a 'with' statement. The port will automatically close on
-        exiting the 'with' statement scope.
+        PortManager: A wrapper around the configured port, that can be
+            entered by using a 'with' statement. The port will
+            automatically close on exiting the 'with' statement scope.
     """
     print(
         port,
         bitRate,
         dataBits,
         handshake,
         hardwareFlowControl,
         parity,
         stopBits,
     )
-    return SerialScriptModule.PortManager()
+    return PortManager()
 
 
 def readBytes(port, numberOfBytes, timeout=5000):
-    # type: (AnyStr, int, Optional[int]) -> List[Any]
     """Read numberOfBytes bytes from a serial port.
 
     Args:
-        port: The previously configured serial port to use.
-        numberOfBytes: The number of bytes to read.
-        timeout: Maximum amount of time, in milliseconds, to block
-            before returning. Default is 5,000. Optional.
+        port (str): The previously configured serial port to use.
+        numberOfBytes (int): The number of bytes to read.
+        timeout (int): Maximum amount of time, in milliseconds, to block
+            before returning. Default is 5000. Optional.
 
     Returns:
-        A list containing bytes read from the serial port.
+        object: A byte[] containing bytes read from the serial port.
     """
     print(port, numberOfBytes, timeout)
-    return []
 
 
-def readBytesAsString(
-    port,  # type: AnyStr
-    numberOfBytes,  # type: int
-    timeout=5000,  # type: int
-    encoding="utf-8",  # type: AnyStr
-):
-    # type: (...) -> AnyStr
+def readBytesAsString(port, numberOfBytes, timeout=5000, encoding="utf-8"):
     """Read numberOfBytes bytes from a serial port and convert them to a
     String.
 
     If a specific encoding is needed to match the source of the data,
     use system.serial.readBytes and use the desired encoding to decode
     the byte array returned.
 
     Args:
-        port: The previously configured serial port to use.
-        numberOfBytes: The number of bytes to read.
-        timeout: Maximum amount of time, in milliseconds, to block
-            before returning. Default is 5,000. Optional.
-        encoding: Encoding to use when constructing the string. Defaults
-            to the platform's default character set. Optional.
+        port (str): The previously configured serial port to use.
+        numberOfBytes (int): The number of bytes to read.
+        timeout (int): Maximum amount of time, in milliseconds, to block
+            before returning. Default is 5000. Optional.
+        encoding (str): Encoding to use when constructing the string.
+            Defaults to the platform's default character set. Optional.
 
     Returns:
-        A String created from the bytes read.
+        str: A String created from the bytes read.
     """
     print(port, numberOfBytes, timeout, encoding)
     return ""
 
 
-def readLine(
-    port,  # type: AnyStr
-    timeout=5000,  # type: int
-    encoding="utf-8",  # type: AnyStr
-    crlfRequired=False,  # type: bool
-):
-    # type: (...) -> AnyStr
+def readLine(port, timeout=5000, encoding="utf-8", crlfRequired=False):
     r"""Attempts to read a line from a serial port.
 
     A "line" is considered to be terminated by either a line feed
     ('\n'), a carriage return ('\r'), or a carriage return followed
     immediately by a line feed.
 
     The function will wait until the timeout period for a terminator. If
     the timeout is reached before the line is properly terminated, then
     the buffer will be dumped, possibly resulting in data loss.
 
     Args:
-        port: The previously configured serial port to use.
-        timeout: Maximum amount of time, in milliseconds, to block
+        port (str): The previously configured serial port to use.
+        timeout (int): Maximum amount of time, in milliseconds, to block
             before returning. Default is 5000. Optional.
-        encoding: The String encoding to use. Default is UTF8. Optional.
-        crlfRequired: True if both CR and LF are required to delimit a
-            line. Optional.
+        encoding (str): The String encoding to use. Default is UTF8.
+            Optional.
+        crlfRequired (bool): True if both CR and LF are required to
+            delimit a line. Optional.
 
     Returns:
-        A line of text.
+        str: A line of text.
     """
     print(port, timeout, encoding, crlfRequired)
     return ""
 
 
 def readUntil(port, delimiter, includeDelimiter, timeout=5000):
-    # type: (AnyStr, AnyStr, bool, Optional[int]) -> AnyStr
     """Reads a byte at a time from a serial port until a delimiter
     character is encountered.
 
     The read will block for up to timeout milliseconds before returning.
 
     If the delimiter is not found before the timeout period, then the
     buffer will dump, potentially resulting in data loss.
 
     Args:
-        port: The previously configured serial port to use.
-        delimiter: The delimiter to read until.
-        includeDelimiter: If True, the delimiter will be included in the
-            return value.
-        timeout: Timeout in milliseconds. Default is 5,000. Optional.
+        port (str): The previously configured serial port to use.
+        delimiter (str): The delimiter to read until.
+        includeDelimiter (bool): If True, the delimiter will be included
+            in the return value.
+        timeout (int): Optional timeout in milliseconds. Default is
+            5000.
 
     Returns:
-        A string containing all 8-bit ASCII characters read until the
-        delimiter was reached, and including the delimiter if the
-        "includeDelimiter" parameter was True.
+        str: Returns a String containing all 8-bit ASCII characters read
+            until the delimiter was reached, and including the delimiter
+            if the "includeDelimiter" parameter was True.
     """
     print(port, delimiter, includeDelimiter, timeout)
     return ""
 
 
 def sendBreak(port, millis):
-    # type: (AnyStr, int) -> None
     """Sends a break signal for approximately millis milliseconds.
 
     Args:
-        port: The name of the serial port, e.g., "COM1" or "dev/ttyS0".
-        millis: Approximate length of break signal, in milliseconds.
+        port (str): The name of the serial port, e.g., "COM1" or
+            "dev/ttyS0".
+        millis (int): Approximate length of break signal, in
+            milliseconds.
     """
     print(port, millis)
 
 
-def write(port, toWrite, timeout=5000, encoding="utf-8"):
-    # type: (AnyStr, AnyStr, int, Optional[AnyStr]) -> None
-    """Write a string to a serial port using the platforms default
+def write(port, toWrite, encoding="utf-8"):
+    """Write a String to a serial port using the platforms default
     character encoding.
 
     Args:
-        port: The previously configured serial port to use.
-        toWrite: The string to write.
-        timeout: Timeout in milliseconds. Default is 5,000. Optional.
-        encoding: Encoding to use when constructing the string. Defaults
-            to the platform's default character set. Optional.
+        port (str): The previously configured serial port to use.
+        toWrite (str): The String to write.
+        encoding (str): Encoding to use when constructing the string.
+            Defaults to the platform's default character set. Optional.
     """
     print(port, toWrite, encoding)
 
 
 def writeBytes(port, toWrite, timeout=5000):
-    # type: (AnyStr, Any, Optional[int]) -> None
-    """Write a byte array to a serial port.
+    """Write a byte[] to a serial port.
 
     Args:
-        port: The previously configured serial port to use.
-        toWrite: The byte array to write.
-        timeout: Optional timeout in milliseconds. Default is 5,000.
-            Optional.
+        port (str): The previously configured serial port to use.
+        toWrite (object): The byte[] to write.
+        timeout (int): Optional timeout in milliseconds. Default is
+            5000. Optional.
     """
     print(port, toWrite, timeout)
```

### Comparing `ignition_api-8.1.40/src/system/math.py` & `ignition-api-8.1.9/src/system/math.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Math Functions.
 
 The following functions assist with running statistical analysis.
 """
 
 from __future__ import print_function
 
@@ -24,465 +28,436 @@
     "sumDifference",
     "sumLog",
     "sumSquares",
     "variance",
 ]
 
 import __builtin__ as builtins
-from typing import List
 
-from dev.coatl.helper.types import AnyNum
-from org.apache.commons.math3.exception import DimensionMismatchException
+from java.lang import Exception as JException
+
+
+class DimensionMismatchException(JException):
+    pass
 
 
 def geometricMean(values):
-    # type: (List[AnyNum]) -> float
     """Calculates the geometric mean.
 
     Geometric Mean is a type of average which indicates a typical value
     in a set of numbers by using the product of values in the set.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The geometric mean, or NaN if the input was empty or null.
-        Because this uses logs to compute the geometric mean, will
-        return NaN if any entries are negative.
+        float: The geometric mean, or nan if the input was empty or
+            null. Because this uses logs to compute the geometric mean,
+            will return nan if any entries are negative.
     """
     print(values)
     return float(43)
 
 
 def kurtosis(values):
-    # type: (List[AnyNum]) -> float
     """Calculates the kurtosis of a sequence of values.
 
     Kurtosis measures if data is peaked or flat relative to normal
     distribution. A set of data with high kurtosis will have distinct
     peaks near the mean, while a set of data with low kurtosis will have
     a flat top near the mean. Uniform distribution is typically a flat
     line.
 
     Returns NaN (Not a Number) if passed an empty sequence measure of
     whether the data are heavy-tailed or light-tailed of a given
     distribution.
 
     Args:
-        values: A sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The kurtosis, or NaN if the input was empty or null.
-        Additionally, returns NaN if the values returned fewer than 4
-        values.
+        float: The kurtosis, or nan if the input was empty or null.
+            Additionally, returns nan if the values returned fewer than
+            4 values.
     """
     print(values)
-    return float(43)
 
 
 def max(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, returns the greatest value in the
     sequence, also known as the "max" value.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The maximum value contained in the values parameter, or NaN if
-        the input was empty or null.
+        float: The maximum value contained in the 'values' parameter, or
+            nan if the input was empty or null.
     """
     return builtins.max(values)
 
 
 def mean(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, calculates the arithmetic mean
     (average).
 
-    Returns NaN (Not a Number) if passed an empty sequence, a null.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The arithmetic mean, or NaN if the input was empty or None.
+        float: The maximum value contained in the 'values' parameter, or
+            nan if the input was empty or null.
     """
     print(values)
-    return float(43)
 
 
 def meanDifference(values1, values2):
-    # type: (List[AnyNum], List[AnyNum]) -> float
     """Given two sequences of values, calculates the mean of the signed
     difference between both sequences.
 
     In other words, returns the absolute difference between the mean
     values of two different sets of data.
 
     Args:
-        values1: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
-        values2: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values1 (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
+        values2 (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The mean difference, or NaN if one of the parameters was empty
-        or null.
+        float: The mean difference, or nan if one of the parameters was
+            empty or null.
 
     Raises:
         DimensionMismatchException: If the two sequences have different
             lengths.
     """
     if len(values1) != len(values2):
         raise DimensionMismatchException()
-    return float(43)
 
 
 def median(values):
-    # type: (List[AnyNum]) -> float
     """Takes a sequence of values, and returns the median.
 
     The Median represents the middle value in a set of data.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The median, or NaN if the input was empty or null.
+        float: The median, or nan if the input was empty or null.
     """
     print(values)
-    return float(43)
 
 
 def min(values):
-    # type: (List[AnyNum]) -> float
     """Given a Sequence of numerical values, returns the minimum value,
     also known as the "min" value.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The minimum value contained within the values parameter, or NaN
-        if the input was empty or null.
+        float: The minimum value contained within the 'values'
+            parameter, or nan if the input was empty or null.
     """
     return builtins.min(values)
 
 
 def mode(values):
-    # type: (List[AnyNum]) -> List[float]
     """Given a sequence of values, returns the 'mode', or most frequent
     values.
 
     Returns an empty list if the sequence was empty or None.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values.
 
     Returns:
-        A Java Array (functionally similar to a Python List) of floats
-        representing the most frequent values in the values parameter.
-        If the values parameter was empty, then an empty list will be
-        returned instead.
+        list[float]: A Java Array (functionally similar to a Python
+            List) of floats representing the most frequent values in the
+            'values' parameter. If the values parameter was empty, then
+            an empty list will be returned instead.
     """
     print(values)
-    return [float(43)]
 
 
 def normalize(values):
-    # type: (List[AnyNum]) -> List[float]
     """Given a sequence of values, normalizes the values.
 
     Normalizing data refers to adjusting values measured on different
     scales and brings them into alignment to allow the comparison of
     corresponding normalized values. This creates uniformity of values
     by eliminating the different units of measurement, and to more
     easily compare data from different places
 
     Returns an empty list if the sequence was empty or None.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values.
 
     Returns:
-        A Java Array (functionally similar to a Python List) of floats
-        representing normalized input, with a mean of 0 and a standard
-        deviation of 1. Returns an empty array if the input was empty or
-        None. If the standard deviation is 0, will return an array of
-        float NaN (Not a Number).
+        list[float]: A Java Array (functionally similar to a Python
+            List) of floats representing normalized input, with a mean
+            of 0 and a standard deviation of 1. Returns an empty array
+            if the input was empty or None. If the standard deviation is
+            0, will return an array of float nan (Not a Number).
     """
     print(values)
-    return [float(43)]
 
 
 def percentile(values, percentile):
-    # type: (List[AnyNum], float) -> float
     """Given a sequence of numerical values, estimates the percentile of
     input.
 
     The percentile is a value on a scale that represents a percentage
     position in a list of data that can be equal to or below that value:
     i.e., the 25th percentile is a value below which 25% of observable
     data points may be found.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
-        percentile: The percentile to compute. A float greater than 0
-            and less than or equal to 100. Will throw an exception if
-            the percentile is out of bounds.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
+        percentile (float): The percentile to compute. A float greater
+            than 0 and less than or equal to 100. Will throw an
+            exception if the percentile is out of bounds.
 
     Returns:
-        An estimate of the requested percentile of the input, or NaN if
-        the input was empty or null.
+        float: An estimate of the requested percentile of the input, or
+            nan if the input was empty or null.
     """
     print(values, percentile)
-    if 0 > percentile > 100:
-        raise ValueError("percentile out of bounds.")
-    return float(43)
 
 
 def populationVariance(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, returns the Population Variance.
 
     Population variance calculates how values in a dataset are spread
     out from their average value.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The population variance, or NaN if the input was empty or null.
+        float: The population variance, or nan if the input was empty or
+            null.
     """
     print(values)
-    return float(43)
 
 
 def product(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, calculates the product of the
     sequence: the result of multiplying of all values in the sequence
     together.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The product of all values in the values parameter, or NaN if the
-        input was empty or null.
+        float: The product of all values in the 'values' parameter, or
+            nan if the input was empty or null.
     """
     print(values)
-    return float(43)
 
 
 def skewness(values):
-    # type: (List[AnyNum]) -> float
     """Calculates the skewness given a sequence of values.
 
     Skewness is a measure of the degree of asymmetry of a distribution
     of the mean. If skewed to the left, the distribution has a long tail
     in the negative direction. If skewed to the right, the tail will be
     skewed in the positive direction.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The skewness of the values parameter, or NaN if values was empty
-        or null.
+        float: The skewness of the 'values' parameter, or nan if values
+            was empty or null.
     """
     print(values)
-    return float(43)
 
 
 def standardDeviation(values):
-    # type: (List[AnyNum]) -> float
     """Given a Sequence of numerical values, calculates the standard
     deviation.
 
     Standard deviation is a calculated number for how close, or how far
     the values of that dataset are in relation to the mean.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The standard deviation of the values parameter, or NaN if the
-        values was empty or null.
+        float: The standard deviation of the 'values' parameter, or nan
+            if the values was empty or null.
     """
     print(values)
-    return float(43)
 
 
 def sum(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, calculates the sum of all values.
 
     The sum is the number returned by addition.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The sum of all values in the values parameter, or NaN if values
-        was empty or null.
+        float: The sum of all values in the 'values' parameter, or nan
+            if values was empty or null.
     """
     return builtins.sum(values)
 
 
 def sumDifference(values1, values2):
-    # type: (List[AnyNum], List[AnyNum]) -> float
     """Given two sequences of values, calculates the sum of the signed
     difference between both sequences.
 
     In other words, the sum and difference between two sets of numbers.
 
     Args:
-        values1: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
-        values2: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values1 (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
+        values2 (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The sum difference, or NaN if one of the parameters was empty or
-        null.
+        float: The sum difference, or nan if one of the parameters was
+            empty or null.
 
     Raises:
         DimensionMismatchException: If the two sequences have different
             lengths.
     """
     if len(values1) != len(values2):
         raise DimensionMismatchException()
-    return float(43)
 
 
 def sumLog(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, calculates the sum of the natural
     logs.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The sum of the natural logs of the input values, or NaN if the
-        input was empty, None, or contains negative numbers.
+        float: The sum of the natural logs of the input values, or nan
+            if the input was empty, None, or contains negative numbers.
     """
     print(values)
-    return float(43)
 
 
 def sumSquares(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, calculates the sum of the squares of
     all values.
 
     Sum squares measures how far individual values are from the mean by
     calculating how much variation there is in a set of values.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The sum of all squares of the values parameter, or NaN if the
-        input was empty or null.
+        float: The sum of all squares of the 'values' parameter, or nan
+            if the input was empty or null.
     """
-    return builtins.sum(value**2 for value in values)
+    return builtins.sum(value ** 2 for value in values)
 
 
 def variance(values):
-    # type: (List[AnyNum]) -> float
     """Given a sequence of values, calculates the variance of all
     values.
 
     Variance measures how far values in a set are spread out from their
     mean value.
 
-    Returns NaN (Not a Number) if passed an empty sequence.
+    Returns NaN (Not A Number) if passed an empty sequence.
 
     Args:
-        values: A Sequence of numerical values. Accepts both Integers
-            and Floats. The sequence may not contain None type values.
-            However, passing a None type object instead of a Sequence of
-            numerical values will return NaN.
+        values (list[float]): A Sequence of numerical values. Accepts
+            both Integers and Floats. The sequence may not contain None
+            type values. However, passing a None type object instead of
+            a Sequence of numerical values will return nan.
 
     Returns:
-        The variance of all values in the values parameter, or NaN if
-        the input was empty or null.
+        float: The sum of all values in the 'values' parameter, or nan
+            if the input was empty or null.
     """
     print(values)
-    return float(43)
```

### Comparing `ignition_api-8.1.40/src/system/roster.py` & `ignition-api-8.1.9/src/system/roster.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,125 +1,92 @@
+# Copyright (C) 2018-2021
+# Author: Cesar Roman
+# Contact: cesar@thecesrom.dev
+
 """Roster Functions.
 
 Functions that provide roster manipulation, including adding and remove
 users from a roster.
 """
 
 from __future__ import print_function
 
 __all__ = [
     "addUsers",
     "createRoster",
     "deleteRoster",
-    "getRoster",
-    "getRosterNames",
     "getRosters",
     "removeUsers",
 ]
 
-from typing import Dict, List, Union
-
-from com.inductiveautomation.ignition.alarming.common.rosters import RosterModel
-from com.inductiveautomation.ignition.common.user import PyUser
-from dev.coatl.helper.types import AnyStr
+from system.user import PyUser
 
 
 def addUsers(rosterName, users):
-    # type: (AnyStr, List[PyUser]) -> None
     """Adds a list of users to an existing roster.
 
     Users are always appended to the end of the roster.
 
     Args:
-        rosterName: The name of the roster to modify.
-        users: A list of User objects that will be added to the end of
-            the roster. User objects can be created with the
-            system.user.getUser and system.user.addUser functions. These
-            users must exist before being added to the roster.
+        rosterName (str): The name of the roster to modify.
+        users (list[PyUser]): A list of User objects that will be added
+            to the end of the roster. User objects can be created with
+            the system.user.getUser and system.user.addUser functions.
+            These users must exist before being added to the roster.
     """
     print(rosterName)
     for user in users:
         print(user.Username)
 
 
 def createRoster(name, description):
-    # type: (AnyStr, Union[AnyStr, None]) -> None
     """Creates a roster with the given name and description, if it does
     not already exist.
 
     This function was designed to run in the Gateway and in Perspective
     sessions. If creating rosters from Vision clients, use
     system.alarm.createRoster instead.
 
     Args:
-        name: The name of the roster to create.
-        description: The description for the roster. May be None, but
-            the parameter is mandatory.
+        name (str): The name of the roster to create.
+        description (str): The description for the roster. May be None,
+            but the parameter is mandatory.
     """
     print(name, description)
 
 
 def deleteRoster(rosterName):
-    # type: (AnyStr) -> None
     """Deletes a roster with the given name.
 
     Args:
-        rosterName: The name of the roster to delete.
+        rosterName (str): The name of the roster to delete.
     """
     print(rosterName)
 
 
-def getRoster(name):
-    # type: (AnyStr) -> RosterModel
-    """Returns the roster corresponding to the given name.
-
-    Args:
-        name: The name of the roster to get the RosterModel object from.
-
-    Returns:
-        A RosterModel Object. Call getUsers() to access a list of User
-        objects in the RosterModel.
-    """
-    print(name)
-    return RosterModel()
-
-
-def getRosterNames():
-    # type: () -> List[AnyStr]
-    """Returns a list of roster names.
-
-    Returns:
-        A list of Strings representing the roster names
-    """
-    return ["On-Call"]
-
-
 def getRosters():
-    # type: () -> Dict[AnyStr, List[AnyStr]]
     """Returns a dictionary of rosters, where the key is the name of the
     roster, and the value is an array list of string user names.
 
     This function was designed to run in the Gateway and in Perspective
     sessions. If creating rosters from Vision clients, use
     system.alarm.getRosters instead.
 
     Returns:
-        A dictionary that maps roster names to a list of usernames in
-        the roster. The list of usernames may be empty if no users have
-        been added to the roster.
+        dict: A python dictionary of rosters. Refer to the list of User
+            objects.
     """
     return {}
 
 
 def removeUsers(rosterName, users):
-    # type: (AnyStr, List[PyUser]) -> None
     """Removes one or more users from an existing roster.
 
     Args:
-        rosterName: The name of the roster to modify.
-        users: A list of user objects that will be added to the end of
-            the roster. User objects can be created with the
-            system.user.getUser and system.user.addUser functions.
+        rosterName (str): The name of the roster to modify.
+        users (list[PyUser]): A list of user objects that will be added
+            to the end of the roster. User objects can be created with
+            the system.user.getUser and system.user.addUser functions.
     """
     print(rosterName)
     for user in users:
         print(user.Username)
```

### Comparing `ignition_api-8.1.40/src/ignition_api.egg-info/PKG-INFO` & `ignition-api-8.1.9/src/ignition_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,207 +1,191 @@
 Metadata-Version: 2.1
 Name: ignition-api
-Version: 8.1.40
-Summary: Ignition Scripting API
-Home-page: https://ignition-api.github.io/8.1
+Version: 8.1.9
+Summary: Ignition Scripting API.
+Home-page: https://github.com/thecesrom/Ignition
 Author: César Román
-Author-email: cesar@coatl.dev
+Author-email: cesar@thecesrom.dev
 License: MIT
-Project-URL: Source, https://github.com/ignition-api/8.1
-Project-URL: Documentation, https://docs.inductiveautomation.com/display/DOC81/System+Functions
-Project-URL: Funding, https://github.com/sponsors/thecesrom
-Project-URL: Tracker, https://github.com/ignition-api/8.1/issues
-Description: # ignition-api 8.1
+Description: # Ignition
         
         <!--- Badges --->
-        ![GitHub last commit (8.1)](https://img.shields.io/github/last-commit/ignition-api/8.1/main)
-        [![GitHub contributors](https://img.shields.io/github/contributors/ignition-api/8.1)](https://github.com/ignition-api/8.1/graphs/contributors)
-        [![Downloads](https://static.pepy.tech/badge/ignition-api)](https://pepy.tech/project/ignition-api)
+        ![GitHub last commit (main)](https://img.shields.io/github/last-commit/thecesrom/Ignition/main)
+        [![GitHub contributors](https://img.shields.io/github/contributors/thecesrom/Ignition)](https://github.com/thecesrom/Ignition/graphs/contributors)
+        [![GitHub downloads](https://img.shields.io/github/downloads/thecesrom/Ignition/total)](https://github.com/thecesrom/Ignition/releases)
+        [![time tracker](https://wakatime.com/badge/github/thecesrom/Ignition.svg)](https://wakatime.com/badge/github/thecesrom/Ignition)
+        [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Join us on GitHub discussions](https://img.shields.io/badge/github-discussions-informational)](https://github.com/ignition-api/8.1/discussions)
-        
-        ignition-api is a Python package that allows developers to get code completion
-        for Ignition Scripting API scripting functions in their IDE of choice.
-        
-        ## Table of contents
-        
+        [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+        [![Imports: flake8](https://img.shields.io/badge/%20imports-flake8-%231674b1?style=flat&labelColor=ef8336)](https://flake8.pycqa.org/en/latest/)
+        [![Imports: pydocstyle](https://img.shields.io/badge/%20imports-pydocstyle-%231674b1?style=flat&labelColor=ef8336)](https://www.pydocstyle.org/en/stable/)
+        [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/thecesrom/Ignition/main.svg)](https://results.pre-commit.ci/latest/github/thecesrom/Ignition/main)
+        
+        Ignition is a set of packages and modules that allows developers to get code completion for Ignition Scripting API scripting functions in their IDE of choice.
+        
+        # Table of contents
+        
+        - [Releases](#releases)
+        - [Branches](#branches)
+          - [Cloning a single branch](#cloning-a-single-branch)
         - [Prerequisites](#prerequisites)
+        - [Packages](#packages)
         - [Installation and usage](#installation-and-usage)
+          - [PyCharm installation](#pycharm-installation)
           - [Installing with pip](#installing-with-pip)
-          - [Downloading from releases](#downloading-from-releases)
-            - [Using as a dependency in PyCharm](#using-as-a-dependency-in-pycharm)
-        - [Project structure](#project-structure)
-          - [Packages](#packages)
-        - [Contributing](#contributing)
+        - [Contributing to Ignition](#contributing-to-ignition)
         - [Discussions](#discussions)
         - [Contributors](#contributors)
         - [License](#license)
         - [Code of conduct](#code-of-conduct)
         
-        ## Prerequisites
+        # Releases
         
-        Before you begin, ensure you have met the following requirements:
+        Check the [releases page](https://github.com/thecesrom/Ignition/releases) and download the one for your current version.
         
-        - You have installed [Python 2.7.18]
-        - You are familiar with [Ignition System Functions]
+        If you can't find it, feel free to submit your request on our [Discussions](https://github.com/thecesrom/Ignition/discussions).
         
-        ## Installation and usage
+        ## Branches
         
-        To use ignition-api, you may install it by doing any of the following.
+        This repository consists of the following branches:
         
-        ### Installing with `pip`
+        ### [main](https://github.com/thecesrom/Ignition/tree/main)
         
-        The preferred method is to install it by running `pip`. It requires Python
-        2.7.18.
+        This branch will contain all Scripting Functions from the latest Ignition Release requiring only Python
         
-        ```bash
-        python2 -m pip install ignition-api
-        ```
+        ### [7.9](https://github.com/thecesrom/Ignition/tree/7.9)
         
-        This will install it as package to your Python installation, which will allow
-        you to call Ignition Scripting functions from Python's REPL, and get code
-        completion using an IDE such as PyCharm and Visual Studio Code.
+        This branch will contain all Scripting Functions from the latest Ignition Release for the 7.9 version requiring only Python
         
-        ```bash
-        $ python2
-        Python 2.7.18 (default, Nov  9 2020, 16:23:15)
-        [GCC Apple LLVM 12.0.0 (clang-1200.0.32.21)] on darwin
-        Type "help", "copyright", "credits" or "license" for more information.
-        >>> from __future__ import print_function
-        >>> import system.util
-        >>> print(system.util.__doc__)
-        Utility Functions.
+        ### [8.0](https://github.com/thecesrom/Ignition/tree/8.0)
         
-        The following functions give you access to view various Gateway and
-        Client data, as well as interact with other various systems.
+        This branch will contain all Scripting Functions from the latest Ignition Release for the 8.0 version requiring only Python
         
-        >>> system.util.beep()
-        >>> quit()
-        ```
+        ### [jython](https://github.com/thecesrom/Ignition/tree/jython)
         
-        And to uninstall:
+        This branch will contain all Scripting Functions from the latest Ignition Release requiring Jython (see [jython prerequisites](https://github.com/thecesrom/Ignition/tree/jython#prerequisites))
         
-        ```bash
-        python2 -m pip uninstall ignition-api
-        ```
+        ### Cloning a single branch
         
-        ### Downloading from releases
+        If you wish to clone just one branch in particular, use any of the following commands:
         
-        You may also download the code targeted to your desired version from [releases]
-        and add it as a dependency to your scripting project.
+        - HTTPS
+            ```bash
+            git clone --single-branch --branch <name> https://github.com/thecesrom/Ignition.git [<directory>]
+            ```
+        - SSH
+            ```bash
+            git clone --single-branch --branch <name> git@github.com:thecesrom/Ignition.git [<directory>]
+            ```
+        - GitHub CLI
+            ```bash
+            gh repo clone thecesrom/Ignition [<directory>] -- --single-branch --branch <name>
+            ```
         
-        #### Using as a dependency in PyCharm
+        ## Prerequisites
+        
+        Before you begin, ensure you have met the following requirements:
         
-        To include ignition-api as a dependency in PyCharm, you will need to attach it
-        to your project.
+        * You have installed Python 2.7.18 ([download here](https://www.python.org/downloads/release/python-2718/))
+        * You are familiar with [Ignition 8.1 System Functions](https://docs.inductiveautomation.com/display/DOC81/System+Functions)
         
-        1. Clone the repo or download from [releases]
-        1. With your project open where you want to include `ignition-api`, navigate to
-           `File > Open` and select the `ignition-api` project folder
-        1. Choose `Attach` when prompted
-        1. Under the `ignitition-api` project folder, right-click on the `src/` folder
-           and choose `Mark Directory as > Sources Root`
         
-        ## Project structure
+        ## Packages
         
-        ### Packages
+        Ignition consists of the following packages:
         
-        This project consists of the following packages:
+        * java/javax
+        * system
         
-        - com.inductiveautomation
-        - java
-        - javax
-        - org
-        - system
+        ### java/javax
         
-        #### com.inductiveautomation
+        These are libraries for some Java packages and functions that are imported in `system` packages meant to be used on development environments where no JDK can be installed, and the project interpreter is Python 2.7.
         
-        This package includes supporting Inductive Automation's classes and interfaces.
-        For more information, see documentation here:
-        <https://files.inductiveautomation.com/sdk/javadoc/ignition81/8.1.39/index.html>.
+        ### system
         
-        #### java/javax
+        Is a package that includes all Ignition Scripting Functions.
         
-        These packages include supporting Java classes and interfaces. For more
-        information, see documentation here:
-        <https://docs.oracle.com/en/java/javase/17/docs/api/index.html>.
+        ## Installation and usage
+        
+        To use Ignition, download the code targeted to your desired version from the [releases page](https://github.com/thecesrom/Ignition/releases) and add it as a dependency to your scripting project.
         
-        #### org.apache
+        ### PyCharm Installation
+        To use Ignition in PyCharm, you will need to attach it to your project.
+        1. With your project open that you want to use with Ignition, navigate to `File > Open` and select the `Ignition` project folder.
+        2. Choose `Attach` when you're prompted on how to open the project.
+        3. Under the new `Ignition` project folder, right-click on the `src/` folder and choose `Mark Directory as > Sources Root`.
         
-        This package includes supporting classes and interfaces from Apache Commons Math
-        API. For more information, see documentation here:
-        <https://commons.apache.org/proper/commons-math/javadocs/api-3.6.1/index.html>
+        ### Installing with `pip`
+        Also, it can be installed by running `pip`. It requires Python 2.7 (we recommend version 2.7.18).
         
-        #### org.json
+        ```bash
+        $ python2 -m pip install ignition-api
+        ```
         
-        This package includes supporting classes and interfaces from the Inductive
-        Automation's `org.json` package, see documentation here:
-        <https://files.inductiveautomation.com/sdk/javadoc/ignition81/8.1.39/org/json/package-summary.html>
+        This will install it as package to your Python installation, which will allow you to call Ignition Scripting functions from Python's REPL, and get code completion using and IDE (we recommend PyCharm).
         
-        #### org.python
+        ```bash
+        Python 2.7.18 (default, Nov  9 2020, 16:23:15) 
+        [GCC Apple LLVM 12.0.0 (clang-1200.0.32.21)] on darwin
+        Type "help", "copyright", "credits" or "license" for more information.
+        >>> from __future__ import print_function
+        >>> import system.util
+        >>> print(system.util.__doc__)
+        Utility Functions.
         
-        This package includes supporting Jython classes and interfaces. For more
-        information, see documentation here:
-        <https://www.javadoc.io/doc/org.python/jython-standalone/2.7.3/index.html>.
+        The following functions give you access to view various Gateway and
+        Client data, as well as interact with other various systems.
         
-        #### org.slf4j
+        >>> system.util.beep()
+        >>> quit()
+        ```
         
-        This package includes supporting classes and interfaces from SLF4J API Module.
-        For more information, see documentation here:
-        <https://www.javadoc.io/doc/org.slf4j/slf4j-api/1.7.26/overview-summary.html>.
+        And to uninstall:
+        ```bash
+        $ python2 -m pip uninstall ignition-api
+        ```
         
-        #### system
+        ## Contributing to Ignition
         
-        This package includes all Ignition Scripting Functions. For more information,
-        see documentation here:
-        <https://docs.inductiveautomation.com/docs/8.1/appendix/scripting-functions>.
+        To contribute to Ignition, follow these steps:
         
-        ## Contributing
+        1. Fork this repository
+        2. Create a local copy on your machine
+        3. Create a branch
+        4. Make your changes and commit them
+        5. Push to the `main` branch
+        6. Create the pull request
         
-        See [CONTRIBUTING.md].
+        Alternatively see the GitHub documentation on [creating a pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).
         
         ## Discussions
         
-        Feel free to post your questions and/or ideas at [Discussions].
+        Feel free to post your questions and/or ideas at [Discussions](https://github.com/thecesrom/incendium/discussions).
         
         ## Contributors
         
         Thanks to everyone who has contributed to this project.
         
-        Up-to-date list of contributors can be found here: [CONTRIBUTORS].
+        Up-to-date list of contributors can be found [here](https://github.com/thecesrom/Ignition/graphs/contributors).
         
         ## License
         
-        See the [LICENSE].
+        See the [LICENSE](https://github.com/thecesrom/Ignition/blob/HEAD/LICENSE).
         
         ## Code of conduct
         
-        This project has adopted the [Microsoft Open Source Code of Conduct].
-        
-        <!-- Links -->
-        [CONTRIBUTING.md]: https://github.com/ignition-api/.github/blob/main/CONTRIBUTING.md#contributing-to-ignition-api
-        [CONTRIBUTORS]: https://github.com/ignition-api/8.1/graphs/contributors
-        [Discussions]: https://github.com/ignition-api/discussions
-        [Ignition System Functions]: https://docs.inductiveautomation.com/docs/8.1/appendix/scripting-functions
-        [LICENSE]: ./LICENSE
-        [Microsoft Open Source Code of Conduct]: https://opensource.microsoft.com/codeofconduct/
-        [Python 2.7.18]: https://www.python.org/downloads/release/python-2718/
-        [releases]: https://github.com/ignition-api/8.1/releases
+        This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
         
-Keywords: hmi,ignition,inductive automation,scada
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2 :: Only
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Mocking
-Requires-Python: ==2.7.18
+Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

