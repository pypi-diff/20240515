# Comparing `tmp/santa_iw-0.6.1.tar.gz` & `tmp/santa_iw-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "santa_iw-0.6.1.tar", max compression
+gzip compressed data, was "santa_iw-0.7.4.tar", max compression
```

## Comparing `santa_iw-0.6.1.tar` & `santa_iw-0.7.4.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     1075 2024-05-06 17:51:08.585069 santa_iw-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     3477 2024-05-08 23:48:25.731558 santa_iw-0.6.1/README.md
--rw-r--r--   0        0        0     1265 2024-04-28 22:46:34.773374 santa_iw-0.6.1/Santa_IW/DBConnection.py
--rw-r--r--   0        0        0     9533 2024-05-08 19:29:42.033557 santa_iw-0.6.1/Santa_IW/DataRecording.py
--rw-r--r--   0        0        0     1651 2024-05-08 19:29:41.995557 santa_iw-0.6.1/Santa_IW/DiscoveryHelper.py
--rw-r--r--   0        0        0    12568 2024-05-08 19:29:41.854556 santa_iw-0.6.1/Santa_IW/Flask/WebGUI.py
--rw-r--r--   0        0        0        0 2024-04-28 22:46:34.774374 santa_iw-0.6.1/Santa_IW/Flask/__init__.py
--rw-r--r--   0        0        0    20496 2024-04-28 22:46:34.774374 santa_iw-0.6.1/Santa_IW/Flask/static/images/santa.jpg
--rw-r--r--   0        0        0     9523 2024-04-28 22:46:34.774374 santa_iw-0.6.1/Santa_IW/Flask/static/images/santa_button.jpg
--rw-r--r--   0        0        0      834 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/BoostrapBase.html.jinja
--rw-r--r--   0        0        0     3510 2024-05-04 19:52:31.553762 santa_iw-0.6.1/Santa_IW/Flask/templates/NavigationBar.html.jinja
--rw-r--r--   0        0        0      894 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja
--rw-r--r--   0        0        0      996 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/control_page.html.jinja
--rw-r--r--   0        0        0     2161 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/focus_page.html.jinja
--rw-r--r--   0        0        0     1639 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/table_analog_stats.html.jinja
--rw-r--r--   0        0        0      842 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/table_config.html.jinja
--rw-r--r--   0        0        0      895 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/table_discrete_stats.html.jinja
--rw-r--r--   0        0        0      946 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/table_internal_status.html.jinja
--rw-r--r--   0        0        0     1341 2024-04-28 22:46:34.775375 santa_iw-0.6.1/Santa_IW/Flask/templates/table_subsystems.html.jinja
--rw-r--r--   0        0        0       59 2024-04-28 22:46:34.776374 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/PLUGIN_CONFIG/Hue.json_disabled
--rwxr-xr-x   0        0        0     4898 2024-05-08 19:29:41.930557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/PLUGIN_MODULES/AttachHue.py
--rw-r--r--   0        0        0        0 2024-05-04 15:36:27.847610 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/PLUGIN_MODULES/__init__.py
--rw-r--r--   0        0        0      142 2024-05-08 01:42:01.224301 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TEMPLATES/Cockpit.json
--rw-r--r--   0        0        0      129 2024-05-01 14:00:42.726357 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingIntranet.json
--rw-r--r--   0        0        0      121 2024-05-08 01:42:01.230301 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingSloppy.json
--rwxr-xr-x   0        0        0     2658 2024-05-08 19:29:41.848556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/ApcAccess.py
--rwxr-xr-x   0        0        0     2570 2024-05-08 19:29:41.876556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/DiskFree.py
--rw-r--r--   0        0        0     4916 2024-05-08 19:29:41.924557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/HTTPTest.py
--rwxr-xr-x   0        0        0     2649 2024-05-08 19:29:41.890556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/IPVx_Address.py
--rwxr-xr-x   0        0        0     3259 2024-05-08 19:29:42.041557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/PendingUpdates.py
--rw-r--r--   0        0        0     7525 2024-05-08 19:29:41.865556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/PingTest.py
--rwxr-xr-x   0        0        0     1462 2024-05-08 19:29:41.935557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/RemoteProcess.py
--rwxr-xr-x   0        0        0     1216 2024-05-08 19:29:41.921557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SE_Status.py
--rwxr-xr-x   0        0        0     1722 2024-05-08 19:29:41.857556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SNMP_id.py
--rwxr-xr-x   0        0        0     7873 2024-05-08 19:29:41.913556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Sensors.py
--rwxr-xr-x   0        0        0     1231 2024-05-08 19:29:42.038557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Shares_NFS.py
--rwxr-xr-x   0        0        0     1983 2024-05-08 19:29:42.035557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Shares_SMB.py
--rwxr-xr-x   0        0        0     4656 2024-05-08 19:29:41.918557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SmartCtl.py
--rwxr-xr-x   0        0        0     5921 2024-05-08 19:29:42.006557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SystemctlFailed.py
--rwxr-xr-x   0        0        0     3583 2024-05-08 19:29:42.027557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/TimeMachine.py
--rwxr-xr-x   0        0        0     1433 2024-05-08 19:29:41.873556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Uname.py
--rwxr-xr-x   0        0        0     3653 2024-05-08 19:29:42.012557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Uptime.py
--rwxr-xr-x   0        0        0     4267 2024-05-08 19:29:41.906556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/ZFS_Snapshots.py
--rwxr-xr-x   0        0        0      998 2024-05-08 19:29:41.842556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/ZFS_Version.py
--rwxr-xr-x   0        0        0     2560 2024-05-08 19:29:41.851556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Zpool_Free.py
--rwxr-xr-x   0        0        0     2837 2024-05-08 19:29:41.893556 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Zpool_Status.py
--rw-r--r--   0        0        0        0 2024-05-04 15:36:27.847610 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 15:36:27.847610 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/__init__.py
--rw-r--r--   0        0        0      355 2024-04-28 22:46:34.780375 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/minimal_makelist.json
--rw-r--r--   0        0        0       74 2024-04-28 22:46:34.780375 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/santa_config.json
--rw-r--r--   0        0        0     1096 2024-05-08 19:29:42.021557 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/santa_defaults.json
--rw-r--r--   0        0        0     1542 2024-05-01 19:56:57.611167 santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/santa_makelist.json
--rw-r--r--   0        0        0     5778 2024-05-08 19:29:42.030557 santa_iw-0.6.1/Santa_IW/Main.py
--rw-r--r--   0        0        0    33341 2024-05-08 19:42:50.503362 santa_iw-0.6.1/Santa_IW/MakeList.py
--rw-r--r--   0        0        0     2362 2024-05-08 19:29:41.927557 santa_iw-0.6.1/Santa_IW/Naughty.py
--rw-r--r--   0        0        0     3297 2024-05-08 19:29:41.879556 santa_iw-0.6.1/Santa_IW/Node.py
--rw-r--r--   0        0        0     4817 2024-05-08 19:29:42.003557 santa_iw-0.6.1/Santa_IW/NodeFactory.py
--rw-r--r--   0        0        0      520 2024-05-08 19:29:41.845556 santa_iw-0.6.1/Santa_IW/PluginBase.py
--rw-r--r--   0        0        0     6323 2024-05-08 19:29:42.000557 santa_iw-0.6.1/Santa_IW/PluginFactory.py
--rw-r--r--   0        0        0      687 2024-05-08 19:29:41.885556 santa_iw-0.6.1/Santa_IW/PluginType.py
--rw-r--r--   0        0        0     4087 2024-04-28 22:46:34.782374 santa_iw-0.6.1/Santa_IW/Status.py
--rw-r--r--   0        0        0    20717 2024-05-08 19:29:41.897556 santa_iw-0.6.1/Santa_IW/Subassembly.py
--rw-r--r--   0        0        0     4765 2024-05-08 19:29:41.992557 santa_iw-0.6.1/Santa_IW/TemplateFactory.py
--rw-r--r--   0        0        0     6954 2024-05-08 19:29:41.882556 santa_iw-0.6.1/Santa_IW/TestBase.py
--rw-r--r--   0        0        0     7516 2024-05-08 19:29:41.888556 santa_iw-0.6.1/Santa_IW/TestFactory.py
--rw-r--r--   0        0        0      666 2024-05-08 19:29:41.932556 santa_iw-0.6.1/Santa_IW/TestType.py
--rw-r--r--   0        0        0     4651 2024-05-08 19:29:42.015557 santa_iw-0.6.1/Santa_IW/TreeRoot.py
--rw-r--r--   0        0        0     2241 2024-05-08 19:29:41.839556 santa_iw-0.6.1/Santa_IW/UnitTests/DBConnection_test.py
--rw-r--r--   0        0        0      624 2024-05-08 19:29:41.870556 santa_iw-0.6.1/Santa_IW/UnitTests/Status_test.py
--rw-r--r--   0        0        0     1947 2024-05-08 19:29:41.867556 santa_iw-0.6.1/Santa_IW/UnitTests/Subassembly_test.py
--rw-r--r--   0        0        0        0 2024-04-28 22:46:34.783375 santa_iw-0.6.1/Santa_IW/UnitTests/__init__.py
--rw-r--r--   0        0        0     3123 2024-04-28 22:46:34.783375 santa_iw-0.6.1/Santa_IW/Utils.py
--rw-r--r--   0        0        0        0 2024-04-28 22:46:34.783375 santa_iw-0.6.1/Santa_IW/__init__.py
--rw-r--r--   0        0        0     1654 2024-05-09 00:20:33.499767 santa_iw-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4994 1970-01-01 00:00:00.000000 santa_iw-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-09 20:26:26.420102 santa_iw-0.7.4/LICENSE.txt
+-rw-r--r--   0        0        0     3351 2024-05-15 16:43:51.996453 santa_iw-0.7.4/README.md
+-rw-r--r--   0        0        0     1265 2024-05-09 20:26:26.421102 santa_iw-0.7.4/Santa_IW/DBConnection.py
+-rw-r--r--   0        0        0     8718 2024-05-14 18:25:52.223959 santa_iw-0.7.4/Santa_IW/DataRecording.py
+-rw-r--r--   0        0        0    31302 2024-05-15 15:50:54.252006 santa_iw-0.7.4/Santa_IW/Discovery.py
+-rw-r--r--   0        0        0     1651 2024-05-09 20:26:26.421102 santa_iw-0.7.4/Santa_IW/DiscoveryHelper.py
+-rw-r--r--   0        0        0    12745 2024-05-14 18:21:25.055379 santa_iw-0.7.4/Santa_IW/Flask/WebGUI.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:26:26.421102 santa_iw-0.7.4/Santa_IW/Flask/__init__.py
+-rw-r--r--   0        0        0    20496 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/static/images/santa.jpg
+-rw-r--r--   0        0        0     9523 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/static/images/santa_button.jpg
+-rw-r--r--   0        0        0      834 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/BoostrapBase.html.jinja
+-rw-r--r--   0        0        0     3524 2024-05-10 14:34:18.046847 santa_iw-0.7.4/Santa_IW/Flask/templates/NavigationBar.html.jinja
+-rw-r--r--   0        0        0      894 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja
+-rw-r--r--   0        0        0      976 2024-05-10 14:45:23.384624 santa_iw-0.7.4/Santa_IW/Flask/templates/control_page.html.jinja
+-rw-r--r--   0        0        0     2112 2024-05-10 14:45:23.388624 santa_iw-0.7.4/Santa_IW/Flask/templates/focus_page.html.jinja
+-rw-r--r--   0        0        0      550 2024-05-10 15:39:25.758191 santa_iw-0.7.4/Santa_IW/Flask/templates/page_footer.html.jinja
+-rw-r--r--   0        0        0     1639 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_analog_stats.html.jinja
+-rw-r--r--   0        0        0      842 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_config.html.jinja
+-rw-r--r--   0        0        0      895 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_discrete_stats.html.jinja
+-rw-r--r--   0        0        0      946 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_internal_status.html.jinja
+-rw-r--r--   0        0        0     1341 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_subsystems.html.jinja
+-rw-r--r--   0        0        0       59 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/PLUGIN_CONFIG/Hue.json_disabled
+-rw-r--r--   0        0        0      142 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/TEMPLATES/Cockpit.json
+-rw-r--r--   0        0        0      129 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingIntranet.json
+-rw-r--r--   0        0        0      121 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingSloppy.json
+-rw-r--r--   0        0        0      343 2024-05-10 20:34:57.538717 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_discovery.json
+-rw-r--r--   0        0        0     1607 2024-05-10 14:05:28.346026 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_gnas_discovery.json
+-rw-r--r--   0        0        0      626 2024-05-15 14:21:44.851032 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_runtime.json
+-rw-r--r--   0        0        0      750 2024-05-14 18:21:25.062379 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/runtime_defaults.json
+-rw-r--r--   0        0        0     4546 2024-05-14 19:15:37.776775 santa_iw-0.7.4/Santa_IW/Main.py
+-rw-r--r--   0        0        0     2493 2024-05-12 19:23:55.646340 santa_iw-0.7.4/Santa_IW/Naughty.py
+-rw-r--r--   0        0        0     3297 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/Node.py
+-rw-r--r--   0        0        0     4975 2024-05-15 16:19:57.978116 santa_iw-0.7.4/Santa_IW/NodeFactory.py
+-rw-r--r--   0        0        0     8131 2024-05-15 16:30:30.912789 santa_iw-0.7.4/Santa_IW/NorthPole.py
+-rwxr-xr-x   0        0        0     4898 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/PLUGIN_MODULES/AttachHue.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/PLUGIN_MODULES/__init__.py
+-rw-r--r--   0        0        0      520 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/PluginBase.py
+-rw-r--r--   0        0        0     6756 2024-05-15 16:19:57.966116 santa_iw-0.7.4/Santa_IW/PluginFactory.py
+-rw-r--r--   0        0        0      687 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/PluginType.py
+-rw-r--r--   0        0        0     4087 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/Status.py
+-rw-r--r--   0        0        0    20717 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/Subassembly.py
+-rwxr-xr-x   0        0        0     2658 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/ApcAccess.py
+-rwxr-xr-x   0        0        0     2570 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/DiskFree.py
+-rw-r--r--   0        0        0     5053 2024-05-11 13:20:54.909267 santa_iw-0.7.4/Santa_IW/TEST_MODULES/HTTPTest.py
+-rwxr-xr-x   0        0        0     2677 2024-05-14 18:25:52.193959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/IPVx_Address.py
+-rwxr-xr-x   0        0        0     3259 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/PendingUpdates.py
+-rw-r--r--   0        0        0     7525 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/PingTest.py
+-rwxr-xr-x   0        0        0     1462 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/RemoteProcess.py
+-rwxr-xr-x   0        0        0     1244 2024-05-14 18:25:52.203959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SE_Status.py
+-rwxr-xr-x   0        0        0     1722 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SNMP_id.py
+-rwxr-xr-x   0        0        0     7903 2024-05-14 18:25:52.231959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Sensors.py
+-rwxr-xr-x   0        0        0     1259 2024-05-14 18:25:52.218959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Shares_NFS.py
+-rwxr-xr-x   0        0        0     1983 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Shares_SMB.py
+-rwxr-xr-x   0        0        0     4656 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SmartCtl.py
+-rwxr-xr-x   0        0        0     5921 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SystemctlFailed.py
+-rwxr-xr-x   0        0        0     3583 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/TimeMachine.py
+-rwxr-xr-x   0        0        0     1433 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Uname.py
+-rwxr-xr-x   0        0        0     3653 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Uptime.py
+-rwxr-xr-x   0        0        0     4296 2024-05-14 18:25:52.212959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/ZFS_Snapshots.py
+-rwxr-xr-x   0        0        0     1026 2024-05-14 18:25:52.227959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/ZFS_Version.py
+-rwxr-xr-x   0        0        0     2588 2024-05-14 18:25:52.237959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Zpool_Free.py
+-rwxr-xr-x   0        0        0     2865 2024-05-14 18:25:52.234959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Zpool_Status.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:26:26.426102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/__init__.py
+-rw-r--r--   0        0        0     5020 2024-05-15 16:09:51.907602 santa_iw-0.7.4/Santa_IW/TemplateFactory.py
+-rw-r--r--   0        0        0     6954 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/TestBase.py
+-rw-r--r--   0        0        0     8204 2024-05-15 16:17:51.191380 santa_iw-0.7.4/Santa_IW/TestFactory.py
+-rw-r--r--   0        0        0      666 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/TestType.py
+-rw-r--r--   0        0        0     5150 2024-05-15 14:13:07.826048 santa_iw-0.7.4/Santa_IW/TreeRoot.py
+-rw-r--r--   0        0        0     2284 2024-05-14 18:25:52.184959 santa_iw-0.7.4/Santa_IW/UnitTests/DBConnection_test.py
+-rw-r--r--   0        0        0      624 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/UnitTests/Status_test.py
+-rw-r--r--   0        0        0     1947 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/UnitTests/Subassembly_test.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/UnitTests/__init__.py
+-rw-r--r--   0        0        0     3123 2024-05-09 20:26:26.429102 santa_iw-0.7.4/Santa_IW/Utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:26:26.429102 santa_iw-0.7.4/Santa_IW/__init__.py
+-rw-r--r--   0        0        0     1793 2024-05-15 16:43:55.992477 santa_iw-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     4868 1970-01-01 00:00:00.000000 santa_iw-0.7.4/PKG-INFO
```

### Comparing `santa_iw-0.6.1/LICENSE.txt` & `santa_iw-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/README.md` & `santa_iw-0.7.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,44 @@
-"Santa Is Watching" (Santa_IW) is a network monitoring tool intended for homelab use. Based upon configuration files
-describing your system, Santa_IW periodically cycles through a suite of tests on your computers, disks, and network
-hardware.
-Santa_IW runs on a
-single Linux computer which needs ssh keys to run diagnostic commands on other computers in your system. Simple ping
-only testing is available for nodes without ssh access. Santa_IW is not forked from or modeled after Nagios, but it
-addresses a
-similar problem space.
-
-Santa_IW includes a network discovery tool called MakeList. MakeList takes a list of start and stop network addresses to
-scan
-and tries to determine what tests are appropriate for each node it finds. Any computer which responds to a network ping
-becomes a candidate for ping testing. If Santa_IW can make an ssh connection to the node, it will:
+["Santa Is Watching" (aka Santa_IW)](https://gitlab.com/SRG_gitlab/santa-is-watching) is a network monitoring tool with an 
+emphasis on ZFS and network attached storage in a homelab environment. Based upon configuration files describing your 
+system, Santa_IW periodically cycles through a suite of
+tests on your computers, disks, and network hardware. Santa_IW runs on a single Linux computer which needs ssh keys
+to run diagnostic commands on other computers in your system. Santa_IW includes a network discovery tool which takes a
+list of start and stop network addresses to scan and tries to determine what tests are appropriate for each node it
+finds. Any computer which responds to a network ping becomes a candidate for ping testing. If Santa_IW can make an 
+ssh connection to the node, it will:
 
 * look at temperature and other data reported by lm-sensors
-* look for drives listed in /etc/fstab and check each for disk free space
+* look for drives listed in /etc/fstab and monitor each for disk free space
 * look for drives supported by smartctl and report SMART status on them
 * look for zfs pools and check each for status and free space
 * look for zfs volumes which seem to be getting frequent snapshots (or are listed in pyznap's config file) and monitor
   the age of the last snapshot
 * look for failed services reported by systemctl --failed
 
-Santa_IW is written in Python and its configuration files are all editable json. It ships with 20+ built in test types
-and
-can load additional user written tests or plugins from user directories. An example plugin is provided to use a Phillips
-Hue color changing light bulb to provide a GREEN/YELLOW/RED status light.
+Santa_IW is written entirely in Python (3.11 or later) and its configuration files are all editable json. It ships with 20+ built in test types
+and can load additional user written tests or plugins from user directories. An example plugin is provided to use a
+Philips Hue color changing light bulb to provide a GREEN/YELLOW/RED status light.
 
 A web based interface lets the user navigate up and down the hierarchy of node groups, nodes and tests to see various
 levels of detail. Tests can record numeric data where appropriate. Running averages are displayed and values over time
 can be graphed or extracted for offline processing.
 
 ----
 
-Santa_IW has been developed and tested on a Linux platform. It has been run on RHEL, Fedora, Ubuntu and Debian
-platforms (including Raspberry Pi 3). It is written in pure Python, but calls out to many Linux/Posix command line
-utilities. It is plausible
-that it might someday work on other Posix compliant platforms (MacOS or BSD), but that is out of scope for the current
-effort. Santa_IW will probably never run natively on Windows, and there are not presently any tests designed to exercise
-Windows nodes beyond a simple ping.
+Santa_IW is hosted on [GitLab](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home) and has been developed and tested on a Linux platform. It has been run installed and run on RHEL, Fedora, Ubuntu
+and Debian platforms (including Raspberry Pi 3). It is written in pure Python, but calls out to many Linux/Posix
+command line utilities. It is plausible that it might someday work on other Posix compliant platforms (macOS or BSD),
+but that is out of scope for the current effort. [For windows support...](https://en.wikipedia.org/wiki/Somebody_else%27s_problem)
 
 Santa_IW is intended for homelab use on an internal network. It does not yet have any robust authentication system and
-should not be exposed on the internet.
+should not be exposed on the open internet.
 
-The code for Santa_IW is pretty much ready for an initial release, but documentation is still being cleaned up.
-If you are reading this, you are a little bit early to the party, but feel free to look around. Installation
-instructions are on the wiki if you are interested in a test drive. I think I have a week or two of documentation tasks
-to complete before I feel comfortable posting to social media in search of beta testers.
+# 🚧 PRE-BETA RELEASE 🚧
 
-----
-Key links:
-
-* [Santa_IW Homepage](https://gitlab.com/SRG_gitlab/santa-is-watching)
-* [Santa_IW Wiki](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home)
-* [Santa_IW API](https://srg_gitlab.gitlab.io/santa-is-watching/index.html)
-* [Santa_IW Issues](https://gitlab.com/SRG_gitlab/santa-is-watching/-/issues)
-* [Libsrg Wiki](https://gitlab.com/SRG_gitlab/libsrg/-/wikis/home)
+If you are reading this, you are a little bit early to the party, but feel free to look
+around. Installation and operating instructions are on the [wiki](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home)
+if you are interested in a test drive. The [Roadmap page]
+(https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/Roadmap) describes some of the work pending before I start 
+inviting people to beta test. The code as-is works well, but many of the pending changes planned will invalidate the 
+documentation. Expecting new users to read the manual once is a big ask these days, so asking them to do it all 
+again after major changes would be too much.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `santa_iw-0.6.1/Santa_IW/DBConnection.py` & `santa_iw-0.7.4/Santa_IW/DBConnection.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/DataRecording.py` & `santa_iw-0.7.4/Santa_IW/DataRecording.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-import os
 from dataclasses import dataclass
 from io import BytesIO
 from threading import Thread
 from time import sleep, time
 from typing import Optional, NamedTuple
 
 import pandas as pd
-
-try:
-    import psutil
-except ImportError:
-    psutil = None
-
 from libsrg.Config import Config
 from libsrg.ElapsedTime import ElapsedTime
 from libsrg.Statistics.ADStatsBase import ADStatsBase
 from libsrg.Statistics.AnalogStatsBase import AnalogStatsBase, AStatsRecord
 from libsrg.Statistics.AnalogStatsSlidingWindow import AnalogStatsSlidingWindow
 from libsrg.Statistics.DiscreteStatsBase import DiscreteStatsBase, DStatsRecord
 from pandas import DataFrame
@@ -47,16 +40,14 @@
         self.db_thread: Optional[Thread] = None
         self._connection: Optional[DBConnection] = None
         self.db_pending: list[str] = []
         self.db_per_sec = AnalogStatsSlidingWindow(self.prefix_name("Mean db writes/s"), window=3600)
         self.data_recording_interval_sec = self.config().get_item("data_recording_interval_sec")
         self.data_recording_keep_days = float(self.config().get_item("data_recording_keep_days"))
         self.statistics_dict: [str, ADStatsBase] = {}
-        if psutil is None:
-            self.log_internal_status(Status.NODATA, "No psutil installed")
 
     def get_dbconnection(self) -> DBConnection:
         if self._connection is None:
             try:
                 self._connection = DBConnection(self.db_filename)
                 self.create_tables()
             except Exception as e:
@@ -155,18 +146,17 @@
 
     def run_in_db_thread(self):
         threshold = self.config().get_item("data_recording_purge_interval")
         purge_timer = ElapsedTime("purge_timer")
         interval_timer = ElapsedTime("actual_interval")
         purge_timer.start()
         while self.subsystem_is_enabled():
-            self.update_psutil_stats()
             len0 = len(self.db_pending)
             # time since last sample (prevent divide by zero on first pass)
-            delta_t=max(interval_timer.current(),0.1)
+            delta_t = max(interval_timer.current(), 0.1)
             interval_timer.start()
             self.db_per_sec.sample(len0 / delta_t)
             if purge_timer.current() >= threshold:
                 purge_timer.start()
                 self.logger.info(f"Purge database")
                 retention_threshold = time() - self.sc.day * self.data_recording_keep_days
                 self.db_pending.append(f"DELETE FROM asamples WHERE time<{retention_threshold}")
@@ -174,19 +164,19 @@
                 self.db_pending.append(f"DELETE FROM ssamples WHERE time<{retention_threshold}")
             if len0 > 0:
                 self.logger.info(f"{len0} database actions to process")
                 with self.get_db_connect() as cur:
                     while len(self.db_pending) > 0:
                         cmd = self.db_pending.pop(0)
                         # self.logger.info(f"Processing {cmd}")
-                        curresult:CursorResult=cur.execute(text(cmd))
-                        #self.logger.info(f"Processing {cmd} {curresult.rowcount=} {curresult!r}")
+                        # noinspection PyUnusedLocal
+                        curresult: CursorResult = cur.execute(text(cmd))
+                        # self.logger.info(f"Processing {cmd} {curresult.rowcount=} {curresult!r}")
                     cur.commit()
 
-
             sleep(self.data_recording_interval_sec)
 
         self._connection.close()
 
     def get_astat_image(self, sensor: str):
         cmd = f"SELECT time,value FROM asamples WHERE name='{sensor}'"
         df: DataFrame = pd.read_sql_query(cmd, self.get_db_engine())
@@ -205,32 +195,12 @@
         if name in self.statistics_dict:
             stat = self.statistics_dict[name]
         else:
             stat = AnalogStatsSlidingWindow(name=name, window=100)
             self.statistics_dict[name] = stat
         return stat
 
-    def update_psutil_stats(self):
-        if psutil == None:
-            return
-        try:
-            data = psutil.cpu_times()
-            self.update_named_tuple(data,"cpu_times")
-
-            data = psutil.cpu_freq()
-            self.update_named_tuple(data,"cpu_freq")
-
-            data = psutil.virtual_memory()
-            self.update_named_tuple(data,"virtual_memory")
-
-            process = psutil.Process(os.getpid())
-            data = process.memory_info()
-            self.update_named_tuple(data,"proc_mem_info")
-
-        except Exception as e:
-            self.logger.error(f"Failed to update psutil stats: {e}", exc_info=True, stack_info=True)
-
-    def update_named_tuple(self,tup:NamedTuple,tup_name):
+    def update_named_tuple(self, tup: NamedTuple, tup_name):
         # noinspection PyProtectedMember
         for key, val in tup._asdict().items():
             stat = self.get_sensor_stats(tup_name, key)
-            stat.sample(val)
+            stat.sample(val)
```

### Comparing `santa_iw-0.6.1/Santa_IW/DiscoveryHelper.py` & `santa_iw-0.7.4/Santa_IW/DiscoveryHelper.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/WebGUI.py` & `santa_iw-0.7.4/Santa_IW/Flask/WebGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import html
 import os
 import signal
+import sys
 import threading
 from pathlib import Path
 from time import sleep
 from typing import Optional, Any
 
 from flask import Flask, render_template, redirect, url_for, request, send_file
 from libsrg.Config import Config
@@ -130,14 +131,15 @@
             self.focus = self.tree_root_subassembly
         self.logger.info(f"Focus set to {self.focus.name():<}")
         return self.focus
 
     def log(self, message: str) -> None:
         self.logger.info(message)
 
+    # noinspection PyMethodMayBeStatic
     def sort_config_list(self,sub: Subassembly):
         lst=sub.config().to_list()
         lst.sort(key=lambda x: f"{x[2]:02n}{x[0]}")
         return lst
 
     def prepare_focus_page(self, name: str, **extras) -> Config:
         """
@@ -154,28 +156,30 @@
         :return:
         """
         now = datetime.datetime.now()
         current_time_txt = now.strftime("%Y-%m-%d %H:%M:%S")
         self.runtime.stop()
         elapsed_time_txt = self.runtime.elapsed_asc()
         focus: Subassembly = self.find_subsystem(name) if not self.shutting_down else self.tree_root_subassembly
-        version = self.config().get_item("SANTA_VERSION")
+        version = self.config().get_item("SANTA_IW_VERSION")
+        branch = self.config().get_item("branch", default="local")
         flask_config = Config({
             "title": f"SHUTDOWN",
             "root_tint": self.tree_root_subassembly.latest_status().tint(),
             "focus_tint": focus.latest_status().tint(),
             "focus": focus,
             "root": self.tree_root_subassembly,
             "parent": focus.parent(),
             "stepparent": focus.stepparent(),
             "trail": [focus],
             "child_nodes": None,
             "child_tests": None,
             "suspects": None,
-            "version": version,
+            "version": f"{version}/{branch}",
+            "python_version": sys.version,
             "body": focus.report(),
             "current_time_txt": current_time_txt,
             "elapsed_time_txt": elapsed_time_txt,
             "astats": None,
             "dstats": None,
             "istats": None,
             "cstats": None,
```

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/static/images/santa.jpg` & `santa_iw-0.7.4/Santa_IW/Flask/static/images/santa.jpg`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/static/images/santa_button.jpg` & `santa_iw-0.7.4/Santa_IW/Flask/static/images/santa_button.jpg`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/BoostrapBase.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/BoostrapBase.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/NavigationBar.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/NavigationBar.html.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,17 @@
                 </li>
                 {#  <li>{{ current_time_txt }}<br/>on {{ localhost }} for {{ elapsed_time_txt }}</li>  #}
             </ul>
             <ul class="nav">
                 <li>
                     <pre>   {{ current_time_txt }}  </pre>
                 </li>
-                <li></li>
+                <li><pre> {{ version }} </pre></li>
                 <li>
-                    <pre>  Santa {{ version }} on {{ localhost }} for {{ elapsed_time_txt }}  </pre>
+                    <pre>  Running on {{ localhost }} for {{ elapsed_time_txt }}  </pre>
                 </li>
                 <li class="nav-item">
                 </li>
             </ul>
 
         </div>
     </div>
```

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/control_page.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/control_page.html.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -40,11 +40,10 @@
     </tr>
 </table>
 
 {% set table_subs = focus_config_list %}
 {% set table_cap = "Configuration Data for  " + focus.name() %}
 {% include "table_config.html.jinja" %}
 
-{% if timeslug %}
-    <pre>{{ timeslug }}</pre>
-{% endif %}
+{% include "page_footer.html.jinja" %}
+
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,9 @@
 {% extends'BoostrapBase.html.jinja' %} {% block header_insert %}
 {% endblock %} {% block body_insert %}
 ************ SSaannttaa CCoonnttrrooll PPaaggee ************
 {% include "NavigationBar.html.jinja" %}
                 CCoonnttrroollss
 ************ {{{{ llooccaallhhoosstt }}}} ************ [SHUTDOWN]
 {% set table_subs = focus_config_list %} {% set table_cap = "Configuration Data
-for " + focus.name() %} {% include "table_config.html.jinja" %} {% if timeslug
-%}
-{{ timeslug }}
-{% endif %} {% endblock %}
+for " + focus.name() %} {% include "table_config.html.jinja" %} {% include
+"page_footer.html.jinja" %} {% endblock %}
```

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/focus_page.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/focus_page.html.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -65,11 +65,9 @@
 
 
     {% if body %}
         <pre>{{ body }}</pre>
         <br/>
     {% endif %}
 
-    {% if current_time_txt %}
-        <pre>{{ current_time_txt }}</pre>
-    {% endif %}
+{% include "page_footer.html.jinja" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -20,10 +20,8 @@
 "table_analog_stats.html.jinja" %} {% if image %}
 ************ IImmaaggee:: {{{{ iimmaaggee }}}} ************
 [data plot]{% endif %} {% set table_subs = focus_config_list %} {% set
 table_cap = "Configuration Data for " + focus.name() %} {% include
 "table_config.html.jinja" %} {% if body %}
 {{ body }}
 
-{% endif %} {% if current_time_txt %}
-{{ current_time_txt }}
-{% endif %} {% endblock %}
+{% endif %} {% include "page_footer.html.jinja" %} {% endblock %}
```

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/table_analog_stats.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/table_analog_stats.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/table_config.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/table_config.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/table_discrete_stats.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/table_discrete_stats.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/table_internal_status.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/table_internal_status.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Flask/templates/table_subsystems.html.jinja` & `santa_iw-0.7.4/Santa_IW/Flask/templates/table_subsystems.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/PLUGIN_MODULES/AttachHue.py` & `santa_iw-0.7.4/Santa_IW/PLUGIN_MODULES/AttachHue.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/ApcAccess.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/ApcAccess.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/DiskFree.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/DiskFree.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/HTTPTest.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/HTTPTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from typing import Optional
 
 import requests
 from libsrg.Config import Config
 from libsrg.ElapsedTime import ElapsedTime
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 from libsrg.Statistics.DiscreteStatsCumulative import DiscreteStatsCumulative
 from requests import Response, get
@@ -25,32 +26,34 @@
 
     def run_test_once(self) -> Status:
         # url can use {{fqdn}} for portable defaults
         # see helper.alias lines at EOF
         url_ = self.config().get_item("url", jinja=True)
         ok_stats = self.config().get_item("allowed_status_codes")
         msg = "bad response"
+        response_: Optional[Response]=None
         try:
             # self.page = requests.get(self.url, auth=HTTPBasicAuth(self.args.user, self.args.password), verify=self.v)
             for try_ in range(0, 2):
                 et = ElapsedTime()
-                response: Response = get(url_, stream=True)
+                response_: Response = get(url_, stream=True)
                 reply_time = et.current()
                 self.reply_stats.sample(reply_time)
-                msg = f"{response.status_code=} {reply_time=} {url_}"
+                msg = f"{response_.status_code=} {reply_time=} {url_}"
                 if url_.startswith("https:"):
-                    connection = response.raw.connection
+                    connection = response_.raw.connection
                     if connection is not None and connection.sock is not None:
-                        certificate_info = connection.sock.getpeercert()
-                        if certificate_info is not None:
-                            for k, v in certificate_info.items():
+                        certificate_info_ = connection.sock.getpeercert()
+                        if certificate_info_ is not None:
+                            for k, v in certificate_info_.items():
                                 self.log_test_status(Status.OK, f"{k}: {v}")
                             # subject = dict(x[0] for x in certificate_info['subject'])
                             # issuer = dict(x[0] for x in certificate_info['issuer'])
-                            notAfter = certificate_info['notAfter']
+                            # noinspection PyPep8Naming
+                            notAfter = certificate_info_['notAfter']
                             # notAfter: Jun 4 22:57:04 2024 GMT
                             fmt = "%b %d %H:%M:%S %Y %Z"
                             cert_dt = datetime.strptime(notAfter, fmt)
                             now_dt = datetime.utcnow()
                             ttl = cert_dt - now_dt
                             seconds_to_live = ttl.total_seconds()
                             days_to_live = seconds_to_live / self.sc.day
@@ -59,18 +62,18 @@
                             if days_to_live < 7:
                                 self.log_test_status(Status.WARNING, msg)
                             elif days_to_live < 21:
                                 self.log_test_status(Status.MAINT, msg)
                             else:
                                 self.log_test_status(Status.OK, msg)
 
-                self.code_stats.sample(response.status_code)
-                if response.status_code in ok_stats:
+                self.code_stats.sample(response_.status_code)
+                if response_.status_code in ok_stats:
                     break
-            if response.status_code not in ok_stats:
+            if response_.status_code not in ok_stats:
                 self.log_test_status(Status.CRITICAL, message=msg)
                 return Status.CRITICAL
             self.log_test_status(Status.OK, message=msg)
             return Status.OK
         except Exception as e:
             self.logger.exception(e, stack_info=True, exc_info=True)
             self.log_test_status(Status.CRITICAL, message=f"Exception: {type(e)} {str(e)}")
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/IPVx_Address.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/IPVx_Address.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 
 from libsrg.Runner import Runner
 
 from Santa_IW.TestBase import Status, TestBase
 
 
+# noinspection PyPep8Naming
 class IPVx_Address(TestBase):
 
     # def extendParser(self):
     #     # can set thresholds to allow known count of uncorrectable errors if needed
     #     self.parser.add_argument("-g", "--global", action="store_const", dest="scope",
     #     const="global", default="global",
     #                              help="scope: global")
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/PendingUpdates.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/PendingUpdates.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/PingTest.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/PingTest.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/RemoteProcess.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/RemoteProcess.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SE_Status.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/SE_Status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env  python3
 
 from libsrg.Runner import Runner
 
 from Santa_IW.TestBase import Status, TestBase
 
 
+# noinspection PyPep8Naming
 class SE_Status(TestBase):
 
     def run_test_once(self):
         cmd = ["sestatus"]
         self.logger.info(cmd)
         r = Runner(cmd, userat=self.userat)
         ret = r.ret
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SNMP_id.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/SNMP_id.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Sensors.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
          "power1_cap": 272.000
       }
    }
 }
 """
 
 
+# noinspection DuplicatedCode
 class Sensors(TestBase):
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly, stepparent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent, stepparent=stepparent,
                          short_name=short_name)  # super defines self.logger
         self.statistics_dict: [str, ADStatsBase] = {}
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Shares_NFS.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Shares_NFS.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env  python3
 
 from libsrg.Runner import Runner
 
 from Santa_IW.TestBase import Status, TestBase
 
 
+# noinspection PyPep8Naming
 class Shares_NFS(TestBase):
 
     def run_test_once(self):
         shares = self.config().get_item("shares")
         expect_set = set(shares)
         self.log_test_status(Status.OK, message=f"Expected {expect_set!r}")
         cmd = ["exportfs", "-s"]
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Shares_SMB.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Shares_SMB.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SmartCtl.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/SmartCtl.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/SystemctlFailed.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/SystemctlFailed.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/TimeMachine.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/TimeMachine.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Uname.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Uname.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Uptime.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Uptime.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/ZFS_Snapshots.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/ZFS_Snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import Status, TestBase
 
 
+# noinspection PyPep8Naming
 class ZFS_Snapshots(TestBase):
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly, stepparent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent, stepparent=stepparent,
                          short_name=short_name)  # super defines self.logger
         self.vol: str = self.config().get_item("vol", "pool", "dev", "par_0")
         self.warnS = self.config().get_item("warnS", default=45)
@@ -81,9 +82,9 @@
                 res_str = f"CRITICAL - No snapshots for {self.vol}"
                 self.log_test_status(Status.CRITICAL, message=res_str)
 
 
 from Santa_IW.DiscoveryHelper import DiscoveryHelper
 
 helper: DiscoveryHelper = DiscoveryHelper(ZFS_Snapshots)
-helper.alias("ZFS_Snapshots_Master", {"warnS": 15, "critS": 30, "period": 10 * TestBase.sc.minute})
+helper.alias("ZFS_Snapshots_Primary", {"warnS": 15, "critS": 30, "period": 10 * TestBase.sc.minute})
 helper.alias("ZFS_Snapshots_Copy", {"warnS": 45, "critS": 90, "period": 10 * TestBase.sc.minute})
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/ZFS_Version.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/ZFS_Version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env  python3
 
 from libsrg.Runner import Runner
 
 from Santa_IW.TestBase import Status, TestBase
 
 
+# noinspection PyPep8Naming
 class ZFS_Version(TestBase):
 
     # def extendParser(self):
     #     pass
     #     # can set thresholds to allow known count of uncorrectable errors if needed
 
     def run_test_once(self):
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Zpool_Free.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Zpool_Free.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import Status, TestBase
 
 
+# noinspection PyPep8Naming
 class Zpool_Free(TestBase):
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly, stepparent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent, stepparent=stepparent,
                          short_name=short_name)  # super defines self.logger
         self.percent_used = AnalogStatsFading(self.prefix_name("percent_used"))
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/TESTS/Zpool_Status.py` & `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Zpool_Status.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import Status, TestBase
 
 
+# noinspection PyPep8Naming
 class Zpool_Status(TestBase):
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly, stepparent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent, stepparent=stepparent,
                          short_name=short_name)  # super defines self.logger
         self.run_hours = AnalogStatsFading(self.prefix_name("PowerOnHours"))
         self.pool: str = self.config().get_item("pool", "dev", "par_0")
```

### Comparing `santa_iw-0.6.1/Santa_IW/INSTALL_CONFIG/santa_makelist.json` & `santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_gnas_discovery.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'additional_per_node'": "OrderedDict([('nas0', OrderedDict([('tests', []), ('templates', "*

 * *                          '[])]))])',*

 * * "'additional_santa_config'": "OrderedDict([('additional_item', 42)])",*

 * * 'delete': "['additional_tests']"}*

```diff
@@ -1,14 +1,17 @@
 {
-    "additional_tests": {
+    "additional_per_node": {
         "nas0": {
             "templates": [],
             "tests": []
         }
     },
+    "additional_santa_config": {
+        "additional_item": 42
+    },
     "explicit_group_assignments": {
         "38:F7:3D": "!drop amazon",
         "68:37:E9": "!drop amazon",
         "E2:13:B7": "!randomized mac?",
         "iphone-5": "MOBILE",
         "mbp13": "MOBILE",
         "mbp14": "MOBILE",
```

### Comparing `santa_iw-0.6.1/Santa_IW/Main.py` & `santa_iw-0.7.4/Santa_IW/Main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import argparse
 import atexit
 import logging
 import logging.config
 import os
-from pathlib import Path
+import pprint
 
 try:
     import tomllib
 except ImportError:
     tomllib = None
 
-
 import libsrg.LoggingCounter
 from libsrg.Config import Config
 from libsrg.Info import Info
 from libsrg.LoggingCounter import LoggingCounter
 
 from Santa_IW.TreeRoot import TreeRoot
+from Santa_IW.NorthPole import NorthPole
 
 
 class Main:
     """
     Main starts up the application by:
     - Initializing the logger
     - Parsing the command line
@@ -31,27 +31,19 @@
     It is a singleton and all application objects will be discoverable from there.
 
     """
 
     def __init__(self):
 
         """ Initializing the santa application """
-        my_file = __file__
-        santa_module_dir = Path(my_file).parent
-        santa_clone_dir = santa_module_dir.parent
-        santa_opt_dir = santa_clone_dir.parent
-        santa_log_dir = santa_opt_dir / "LOGS"
-        santa_db_dir = santa_opt_dir / "DB"
-        santa_secrets_dir = santa_opt_dir / "SECRETS"
-        santa_user_config_dir = santa_opt_dir / "CONFIG"
-        install_dir_path = santa_module_dir / "INSTALL_CONFIG"
+        self.np = NorthPole()
+        np = self.np
 
         parser_args = {}
         self.parser = argparse.ArgumentParser(**parser_args)
-        self.parser.add_argument('--config', help="path to configuation file", dest='config_file')
         self.parser.add_argument("--level", help="Logging level at santa.log", action='store',
                                  choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], default="INFO")
         self.parser.add_argument("--console", help="Logging level at console (stderr)", action='store',
                                  choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], default="ERROR")
 
         self.args = self.parser.parse_args()
 
@@ -76,15 +68,15 @@
                     "formatter": "detailed",
                     "stream": "ext://sys.stderr"
                 },
                 "file": {
                     "class": "logging.handlers.RotatingFileHandler",
                     "level": self.args.level.upper(),
                     "formatter": "detailed",
-                    "filename": santa_log_dir / "santa.log",
+                    "filename": np.santa_logs_dir / "santa.log",
                     "maxBytes": 100_000_000,
                     "backupCount": 5,
                     "mode": "a"
                 }
             },
             "root": {
                 "level": "DEBUG",
@@ -99,61 +91,46 @@
         self.logger = logging.getLogger(self.__class__.__name__)
         atexit.register(libsrg.LoggingCounter.LoggingCounter.log_counters)
 
         # any major issues here are assumed fatal
         # no heroics, but I do want to log what happens (as soon as logging is running).
         self.exit_counter = 0
         try:
-
-
-
-            # figure out where the defaults file lives
-            defaults_file_path = install_dir_path / "santa_defaults.json"
-
-            startup_config=Config()
-            # remember where install files are
-            startup_config["__INSTALL__"] = str(install_dir_path)
-            startup_config["__CONFIG__"] = str(santa_user_config_dir)
-            startup_config["__SANTA_MODULE_DIR__"] = str(santa_module_dir)
-            startup_config["__SANTA_CLONE_DIR__"] = str(santa_clone_dir)
-            startup_config["__SANTA_OPT_DIR__"] = str(santa_opt_dir)
-            startup_config["__SANTA_LOG_DIR__"] = str(santa_log_dir)
-            startup_config["__SANTA_DB_DIR__"] = str(santa_db_dir)
-            startup_config["__SANTA_SECRETS_DIR__"] = str(santa_secrets_dir)
+            self.logger.info(pprint.pformat(self.np.as_dict()))
+            startup_config = Config(np.setup_defaults_file, np.as_dict())
 
             if tomllib:
-                with open(santa_clone_dir / "pyproject.toml", 'rb') as fp:
+                with open(np.pyproject_toml_file, 'rb') as fp:
                     toml_dict = tomllib.load(fp)
                 version = toml_dict["tool"]["poetry"]["version"]
             else:
                 version = "0.0.0"
-            startup_config["SANTA_VERSION"] = version
-
+            startup_config["SANTA_IW_VERSION"] = version
 
             # Get localhost info
             localhost_info = Info()
-            localhost_config= localhost_info.to_config("localhost_")
+            localhost_config = localhost_info.to_config("localhost_")
             localhost_config.set_item("localhost_is_root", os.geteuid() == 0)
             localhost_config.set_item("fqdn", localhost_info.fqdn)
 
             # load the defaults file
-            defaults_config = Config(defaults_file_path,localhost_config,startup_config)
-
-            config_file_path = Path(self.args.config_file) if self.args.config_file is not None \
-                else santa_user_config_dir / "santa_config.json"
+            defaults_config = Config(np.default_runtime_file, localhost_config, startup_config)
 
             # noinspection PyUnboundLocalVariable
-            primary_config = Config(config_file_path, defaults_config)
-
+            primary_config = Config(np.user_runtime_file, defaults_config)
 
-            self.treeroot = TreeRoot(primary_config)
-            self.treeroot.start()
+            self.tree_root = TreeRoot(primary_config)
+            self.tree_root.start()
             LoggingCounter.rotate_files()
             exit(0)
 
         except Exception as e:
             self.logger.exception(f"Fatal: {type(e)} {e}", stack_info=True, exc_info=True)
             exit(1)
 
 
-if __name__ == '__main__':
+def main():
     _ = Main()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `santa_iw-0.6.1/Santa_IW/MakeList.py` & `santa_iw-0.7.4/Santa_IW/Discovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,120 @@
 import logging
 import os
 import socket
+from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from ipaddress import IPv4Address, IPv4Network  # IPv4Network
 from pathlib import Path
 from typing import Any, Optional
 
 from libsrg.Config import Config
 from libsrg.ElapsedTime import ElapsedTime
 from libsrg.Info import Info
-from libsrg.LoggingAppBase import LoggingAppBase
 from libsrg.Runner import Runner
 from requests import Response, get
 
-"""
-This module is a sample application template for libsrg application logging
-"""
+from Santa_IW.NorthPole import NorthPole
+from Santa_IW.PluginBase import PluginBase
+from Santa_IW.PluginType import PluginType
+from Santa_IW.Status import Status
+from Santa_IW.Subassembly import Subassembly
+
+
+class TestDiscoveryBase(ABC):
+    def __init__(self, host_creator: "HostCreator"):
+        self.host_creator = host_creator
+        self.config = self.host_creator.config
+        self.logger = self.host_creator.logger
+        self.fqdn = self.host_creator.fqdn
+        self.can_ping = self.host_creator.can_ping
+        self.can_ssh = self.host_creator.can_ssh
+        self.can_name = self.host_creator.can_name
+        self.userat = self.host_creator.userat
+        self.can_snmp = self.host_creator.can_snmp
+
+    def add_test(self, d: dict[str, Any]):
+        self.host_creator.add_test(d)
+
+    def add_template(self, d: str):
+        self.host_creator.add_template(d)
+
+    @abstractmethod
+    def discover(self):
+        pass
+
+
+class PingDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ping and not self.can_ssh:
+            self.add_test(
+                {
+                    "test_type": "PingTest_D"
+                })
+        else:
+            self.add_test(
+                {
+                    "test_type": "PingTest_A"
+                })
+
+
+class LinuxCommonDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh:
+            self.add_test(
+                {
+                    "test_type": "Uname"
+                })
+            self.add_test(
+                {
+                    "test_type": "Uptime"
+                })
+            self.add_test(
+                {
+                    "test_type": "SystemctlFailed"
+                })
+            self.add_test(
+                {
+                    "test_type": "PendingUpdates"
+                })
+            self.add_test(
+                {
+                    "test_type": "IPV4_Address"
+                })
+            self.add_test(
+                {
+                    "test_type": "IPV6_Address"
+                })
+
+
+class SNMPDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if not self.can_snmp:
+            return
+        self.add_test(
+            {
+                "test_type": "SNMP_id",
+                "community": "{{__SNMP_COMMUNITY__}}",
+            })
+
+
+class SensorsDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh:
+            r = Runner("sensors -j", userat=self.userat, timeout=5)
+            if r.success:
+                self.add_test(
+                    {
+                        "test_type": "Sensors"
+                    })
 
 
 class HostCreator:
 
     def __init__(self, address: IPv4Address, config: Config, group_paths: dict[str, Path], host_template_dir: Path):
         self.hostname_info = None
         self.is_localhost = None
@@ -44,16 +138,16 @@
         self.can_ping = False
         self.can_ssh = False
         self.can_name = False
         self.can_snmp = False
         self.overwrite = self.config.get_item("overwrite")
         self.userat = None
         self.short = None
-        self.ipaddrlist = None
-        self.aliaslist = None
+        self.ip_addr_list = None
+        self.alias_list = None
         self.fqdn = None
         # self.logger.info(f"Starting {address}")
 
     def identify(self):
         et = ElapsedTime("identify " + str(self.address))
         self.identify_inner()
         self.logger.debug(f"ElapsedTime {et}")
@@ -62,15 +156,15 @@
         r = Runner(f"ping -q -c 4 -w 4 -i .25 -W .25 {self.address}", timeout=5, silent=True)
         self.can_ping = r.success
         if not self.can_ping:
             self.logger.debug(f"Can't ping {self.address}")
             return
         self.logger.info(f"Pinged {self.address}")
         try:
-            self.fqdn, self.aliaslist, self.ipaddrlist = socket.gethostbyaddr(str(self.address))
+            self.fqdn, self.alias_list, self.ip_addr_list = socket.gethostbyaddr(str(self.address))
             self.logger.info(f"Reverse DNS for Address: {self.address} Hostname: {self.fqdn}")
             self.can_name = True
         except socket.herror as e:
             self.logger.error(f"Reverse address lookup failed for {self.address} {e}", stack_info=True, exc_info=True)
         r2 = Runner(f"uname -n", timeout=5, userat=f"root@{self.address}", silent=True)
         self.can_ssh = r2.success
         if r2.success:
@@ -171,145 +265,105 @@
             self.group_name = self.config.get_item(self.kernel_name)
         else:
             self.logger.error(f"Can't find group for {self.kernel_name}, dropping {self.address} {self.fqdn}")
             return False
 
         self.logger.info(f"{self.address} {self.short} assigned group {self.group_name}")
         explicit_group_assignments = Config(self.config.get_item("explicit_group_assignments", default={}))
-        g0 = self.group_name
+        group_name_init = self.group_name
         self.logger.info(f"searching {str(self.address)=}, {self.short=}, {self.mac_address=}, {self.oui=}")
-        gnew = explicit_group_assignments.get_item(str(self.address), self.short, self.mac_address, self.oui,
-                                                   default=g0)
-        if g0 != gnew:
-            self.group_name = gnew
-            self.logger.info(f"{self.address} {self.short} group reassigned {g0} -> {self.group_name}")
+        group_name_new = explicit_group_assignments.get_item(str(self.address), self.short, self.mac_address, self.oui,
+                                                             default=group_name_init)
+        if group_name_init != group_name_new:
+            self.group_name = group_name_new
+            self.logger.info(f"{self.address} {self.short} group reassigned {group_name_init} -> {self.group_name}")
 
         if self.group_name in self.group_paths:
             self.group_path = self.group_paths[self.group_name]
         else:
             if self.group_name.lower().startswith(("drop", "!")):
                 self.logger.warning(f"Group {self.group_name}, dropping {self.address} {self.short}")
                 return False
             self.logger.error(f"Group {self.group_name} does not exist, dropping {self.address} {self.short}")
             return False
         return True
 
     def write_host_file(self):
-        fname: Path = self.group_path / f"{self.fqdn}.json"
-        if fname.exists() and not self.overwrite:
-            self.logger.warning(f"Host file {fname} is already exists -- not overwriting")
+        host_file_path: Path = self.group_path / f"{self.fqdn}.json"
+        if host_file_path.exists() and not self.overwrite:
+            self.logger.warning(f"Host file {host_file_path} is already exists -- not overwriting")
             return
-        additional_tests = Config(self.config.get_item("additional_tests", default={}))
+        additional_tests = Config(self.config.get_item("additional_per_node", "additional_tests", default={}))
         data = additional_tests.get_item(str(self.address), self.short, self.mac_address, self.oui, default={})
 
         ncon = Config(data)
         ncon.set_item("fqdn", self.fqdn)
         ncon.set_item("discovered_ipv4", str(self.address))
         ncon.set_item("discovered_mac", str(self.mac_address))
         ncon.set_item("discovered_oui", str(self.oui))
 
         ncon.set_item("short_name", self.short)
         templates = ncon.get_item("templates", default=[])
         templates.append(f"auto_{self.fqdn}")
         ncon.set_item("templates", templates)
-        ncon.to_json_file(fname, indent=4)
-        self.logger.info(f"Host config for {self.fqdn} added at {fname}")
+        ncon.to_json_file(host_file_path, indent=4)
+        self.logger.info(f"Host config for {self.fqdn} added at {host_file_path}")
 
     def add_test(self, d: dict[str, Any]):
         self.auto_tests.append(d)
         self.logger.info(f"{self.short} Adding test {len(self.auto_tests)} {d} ")
 
     def add_template(self, d: str):
         self.auto_templates.append(d)
         self.logger.info(f"{self.short} Adding template {len(self.auto_templates)} {d} ")
 
     def write_host_template(self):
-        fname: Path = self.host_template_dir / f"auto_{self.fqdn}.json"
-        if fname.exists() and not self.overwrite:
-            self.logger.warning(f"Host file {fname} is already exists -- not overwriting")
+        auto_file_path: Path = self.host_template_dir / f"auto_{self.fqdn}.json"
+        if auto_file_path.exists() and not self.overwrite:
+            self.logger.warning(f"Host file {auto_file_path} is already exists -- not overwriting")
             return
         ncon = Config()
 
         self.add_ping_intranet()
-        self.add_df()
         self.add_linux_common()
+        self.add_snmp()
+        self.add_sensors()
+
+        self.add_df()
         self.add_smart()
         self.add_zfs_stuff()
         self.add_cockpit()
         self.add_sestatus()
-        self.add_sensors()
-        self.add_snmp()
         self.add_apcaccess()
         self.add_nfs()
         self.add_smb()
         self.add_http()
         self.add_time_machine()
 
         ncon.set_item("intended_for", self.fqdn)
         ncon.set_item("tests", self.auto_tests)
         ncon.set_item("templates", self.auto_templates)
-        ncon.to_json_file(fname, indent=4)
-        self.logger.info(f"Host template for {self.fqdn} added at {fname}")
+        ncon.to_json_file(auto_file_path, indent=4)
+        self.logger.info(f"Host template for {self.fqdn} added at {auto_file_path}")
 
     def add_ping_intranet(self):
-        if self.can_ping and not self.can_ssh:
-            self.add_test(
-                {
-                    "test_type": "PingTest_D"
-                })
-        else:
-            self.add_test(
-                {
-                    "test_type": "PingTest_A"
-                })
+        d = PingDiscovery(self)
+        d.discover()
 
     def add_linux_common(self):
-        if self.can_ssh:
-            self.add_test(
-                {
-                    "test_type": "Uname"
-                })
-            self.add_test(
-                {
-                    "test_type": "Uptime"
-                })
-            self.add_test(
-                {
-                    "test_type": "SystemctlFailed"
-                })
-            self.add_test(
-                {
-                    "test_type": "PendingUpdates"
-                })
-            self.add_test(
-                {
-                    "test_type": "IPV4_Address"
-                })
-            self.add_test(
-                {
-                    "test_type": "IPV6_Address"
-                })
+        d = LinuxCommonDiscovery(self)
+        d.discover()
 
     def add_snmp(self):
-        if not self.can_snmp:
-            return
-        self.add_test(
-            {
-                "test_type": "SNMP_id",
-                "community": "{{__SNMP_COMMUNITY__}}",
-            })
+        d = SNMPDiscovery(self)
+        d.discover()
 
     def add_sensors(self):
-        if self.can_ssh:
-            r = Runner("sensors -j", userat=self.userat, timeout=5)
-            if r.success:
-                self.add_test(
-                    {
-                        "test_type": "Sensors"
-                    })
+        d = SensorsDiscovery(self)
+        d.discover()
 
     def add_cockpit(self):
         if self.can_ssh:
             r = Runner(f"systemctl is-enabled cockpit", userat=self.userat, timeout=5)
             if r.success:
                 self.add_template("Cockpit")
 
@@ -481,278 +535,163 @@
         if not r.success:
             return
         cmd = {
             "test_type": "ZFS_Version",
             "period": 900
         }
         self.add_test(cmd)
-        for poolname in r.so_lines:
+        for pool_name in r.so_lines:
             cmd = {
                 "test_type": "Zpool_Status",
-                "instance_name": poolname,
+                "instance_name": pool_name,
                 "period": 300,
-                "pool": poolname
+                "pool": pool_name
             }
             self.add_test(cmd)
             cmd = {
                 "test_type": "Zpool_Free",
-                "instance_name": poolname,
+                "instance_name": pool_name,
                 "period": 300,
-                "pool": poolname
+                "pool": pool_name
             }
             self.add_test(cmd)
-        zvols_processed = []
+        zfs_volumes_processed = []
         r = Runner("cat /etc/pyznap/pyznap.conf", userat=self.userat, timeout=4)
         if r.success:
             data = Config(Config.text_to_dict('\n'.join(r.so_lines)))
             for vol_name in data.keys():
                 sdata = data[vol_name]
                 if sdata.get("snap", "no") == "yes":
                     cmd = {
                         "par_0": vol_name,
-                        "test_type": "ZFS_Snapshots_Master"
+                        "test_type": "ZFS_Snapshots_Primary"
                     }
                     self.add_test(cmd)
-                    zvols_processed.append(vol_name)
+                    zfs_volumes_processed.append(vol_name)
         r = Runner("zfs list -H -o name", userat=self.userat, timeout=10)
-        zvols = r.so_lines
-        for vol_name in zvols:
+        zfs_volumes = r.so_lines
+        for vol_name in zfs_volumes:
             # Looking for vols with no child vols
             matched = False
-            for vol_name2 in zvols:
+            for vol_name2 in zfs_volumes:
                 if vol_name == vol_name2:
                     continue
                 if vol_name2.startswith(vol_name):
                     matched = True
                     break
             if matched:
                 continue
-            if vol_name in zvols_processed:
+            if vol_name in zfs_volumes_processed:
                 continue
             if not self.check_age_of_snapshots(vol_name):
                 continue
             cmd = {
                 "par_0": vol_name,
                 "test_type": "ZFS_Snapshots_Copy"
             }
             self.add_test(cmd)
-            zvols_processed.append(vol_name)
+            zfs_volumes_processed.append(vol_name)
 
     def check_age_of_snapshots(self, vol) -> bool:
-        zargs = ["/sbin/zfs", "list", "-H", "-t",
-                 "snapshot", "-r",
-                 "-d1", "-o", "name,creation", "-S", "creation", vol]
-        r = Runner(zargs, userat=self.userat, timeout=15)
+        zfs_commands = ["/sbin/zfs", "list", "-H", "-t",
+                        "snapshot", "-r",
+                        "-d1", "-o", "name,creation", "-S", "creation", vol]
+        r = Runner(zfs_commands, userat=self.userat, timeout=15)
         lines = r.so_lines
         ret = r.ret
         if ret != 0:
             res_str = f"UNKNOWN - Command Error 0x{ret:04x} {vol}"
             self.logger.warning(res_str)
             return False
         else:
             minutes = 60
             crit_t = timedelta(0, minutes * 60)
 
-            # reg=re.compile(r'auto-([-0-9:_.]*)')
-            # regp=re.compile(r'[-:_.]+')
-            dtnow = datetime.now()
+            datetime_now = datetime.now()
             if lines:
                 for line in lines:
                     parts = line.split('\t')
                     self.logger.info(parts)
                     # name = parts[0]
                     if len(parts) > 1:
                         dat_a = parts[1]
                         dt = datetime.strptime(dat_a, '%a %b %d %H:%M %Y')
-                        age = dtnow - dt
+                        age = datetime_now - dt
                         self.logger.info(f"Snapshot {vol} age {age} minutes")
                         return age <= crit_t
         return False
 
 
-class MakeLists(LoggingAppBase):
+class MakeListsEmbedded:
+
+    def __init__(self, santa_config: Config, np: NorthPole):
+        self.logger = logging.getLogger(self.__class__.__name__)
+        self.np = np
+        self.santa_config = santa_config
 
-    def __init__(self):
-        super().__init__()  # super defines self.logger
-        self.local_plugins_config_dir = None
-        self.local_plugin_modules_dir = None
         self.candidate_hosts: list[HostCreator] = []
-        self.network_dir = None
-        self.mobile_dir = None
-        self.iot_dir = None
-        self.hosts_dir = None
-        self.secrets_path = None
-        self.local_tests_dir = None
-        self.local_template_dir = None
-        self.host_template_dir = None
-        self.host_nodes_dir = None
-        self.santa_config_dir = None
-        self.user_config = Config()
+
         self.group_path_dict: dict[str, Path] = dict()
 
         self.is_root = os.getuid() == 0
-        if self.is_root:
-            assumed_dir = Path("/opt/Santa_IW/CONFIG")
-        else:
-            assumed_dir = Path.home() / "Santa_IW" / "CONFIG"
+
         # local_info = Info("localhost")
         # local_info.dump()
 
         # setup any program specific command line arguments
-        self.parser.add_argument('--dir', help="Dir to generate files into", dest='santa_config_dir',
-                                 default=str(assumed_dir))
-        self.parser.add_argument('--config', help="Configuration File", dest='config', default=None)
-        self.parser.add_argument('--threads', help="Number of threads in pool", dest='num_threads', type=int,
-                                 default=32)
-
-        # invoke the parser
-        self.perform_parse()
+        # self.parser.add_argument('--dir', help="Dir to generate files into", dest='santa_config_dir',
+        #                          default=str(assumed_dir))
+        # self.parser.add_argument('--config', help="Configuration File", dest='config', default=None)
+        # self.parser.add_argument('--threads', help="Number of threads in pool", dest='num_threads', type=int,
+        #                          default=32)
 
         # create output dir if missing
-        self.santa_config_dir = Path(self.args.santa_config_dir)
-        if not self.santa_config_dir.exists():
-            self.santa_config_dir.mkdir()
-        self.logger.info(f"Santa_IW config output to {self.santa_config_dir}")
-
-        # form path to where makelist config will reside in output dir
-        self.makelist_path_perm = self.santa_config_dir / "santa_makelist.json"
-
-        # figure out where the defaults files live
-        my_file = __file__
-        self.module_dir = Path(my_file).parent
-        self.install_parent_dir = self.module_dir.parent.parent
-        self.logger.info(f"Install parent dir {self.install_parent_dir}")
-        self.install_dir_path = self.module_dir / "INSTALL_CONFIG"
-        self.minimal_makelist_path = self.install_dir_path / "minimal_makelist.json"
-
-        # use command line config path if given
-        if self.args.config is not None:
-            self.makelist_path = Path(self.args.config)
-        else:
-            # else use file in output dir if it exists
-            self.makelist_path = self.santa_config_dir / "santa_makelist.json"
-            if not self.makelist_path.exists():
-                # finally, use file from install dir as fallback
-                self.makelist_path = self.minimal_makelist_path
 
-        self.logger.info(f"Santa_IW makelist input config is {self.makelist_path}")
+        if not self.np.santa_discovery_config_dir.exists():
+            self.np.create_discovery_dirs()
+
+        self.logger.info(f"Santa_IW config output to {self.np.santa_discovery_config_dir}")
+
+        self.logger.info(f"Santa_IW discovery input config is {self.np.user_discovery_file}")
         self.info = Info()
         self.localhost_config = self.info.to_config("localhost.")
-        self.config = Config(self.makelist_path, self.localhost_config)
+        self.discovery_config = Config(self.np.user_discovery_file, self.localhost_config)
 
-        if self.makelist_path_perm != self.makelist_path:
-            self.config.to_json_file(self.makelist_path_perm, indent=4)
-            self.logger.info(f"Santa_IW makelist input config saved to  {self.makelist_path_perm}")
-
-        self.worker_pool = ThreadPoolExecutor(max_workers=self.args.num_threads)
-        self.logger.info(f"Started pool with {self.args.num_threads} threads")
+        self.worker_pool = ThreadPoolExecutor(max_workers=32)  # fixme config
 
         self.create_dirs()
         self.loop_over_scans()
-        # self.scan_network(self.args.network)
-        self.write_config()
         #
 
     def create_dirs(self) -> None:
-        self.logger.info(f"Santa_IW dir: {self.santa_config_dir}")
-
-        nuke_old_hosts = self.config.get_item("nuke_old_hosts", default=False)
-
-        # top directory for node definitions
-        self.host_nodes_dir = self.santa_config_dir / 'HOST_NODES'
-        if nuke_old_hosts and self.host_nodes_dir.exists():
-            _ = Runner(f"rm -rf {self.host_nodes_dir}")
-
-        self.host_nodes_dir.mkdir(parents=True, exist_ok=True)
-        self.user_config.set_item("nodedirs", [
-            "{{__CONFIG__}}/HOST_NODES",
-        ])
-
-        # this dir holds automatically generated templates for each host
-        self.host_template_dir = self.santa_config_dir / 'AUTO_HOST_TEMPLATES'
-        self.host_template_dir.mkdir(parents=True, exist_ok=True)
-
-        # this is where a user can add their own templates
-        self.local_template_dir = self.santa_config_dir / 'LOCAL_TEMPLATES'
-        self.local_template_dir.mkdir(parents=True, exist_ok=True)
-        self.user_config.set_item("templatedirs", [
-            "{{__CONFIG__}}/LOCAL_TEMPLATES",
-            "{{__CONFIG__}}/AUTO_HOST_TEMPLATES",
-            "{{__INSTALL__}}/TEMPLATES",
-        ])
-
-        # this is where a user can add their own plugins
-        self.local_plugin_modules_dir = self.santa_config_dir / 'LOCAL_PLUGIN_MODULES'
-        self.local_plugin_modules_dir.mkdir(parents=True, exist_ok=True)
-        self.user_config.set_item("plugin_modules_dirs", [
-            "{{__CONFIG__}}/LOCAL_PLUGIN_MODULES",
-            "{{__INSTALL__}}/PLUGIN_MODULES",
-        ])
-
-        # this is where a user can add their own plugin configurations
-        self.local_plugins_config_dir = self.santa_config_dir / 'LOCAL_PLUGIN_CONFIG'
-        self.local_plugins_config_dir.mkdir(parents=True, exist_ok=True)
-        self.user_config.set_item("plugin_config_dirs", [
-            "{{__CONFIG__}}/LOCAL_PLUGIN_CONFIG",
-            "{{__INSTALL__}}/PLUGIN_CONFIG",
-        ])
-
-        # this is where a user can add their own tests
-        self.local_tests_dir = self.santa_config_dir / 'LOCAL_TESTS'
-        self.local_tests_dir.mkdir(parents=True, exist_ok=True)
-        self.user_config.set_item("testdirs", [
-            "{{__CONFIG__}}/LOCAL_TESTS",
-            "{{__INSTALL__}}/TESTS",
-        ])
-
         # create group subdirectories below HOST_NODES
-        groups: dict[str, Any] = self.config.get_item("groups")
-        for group, gconfig in groups.items():
+        groups: dict[str, Any] = self.discovery_config.get_item("groups")
+        for group, group_config in groups.items():
             # if the given group name contains a slash "HOSTS/RPI"
             # this will magically create nested groups
-            # groupz is just the last part of this name
-            groupz = group.split('/')[-1]
-            path = self.host_nodes_dir / group
+            # group_short is just the last part of this name
+            group_short = group.split('/')[-1]
+            path = self.np.santa_discovery_nodes_dir / group
             path.mkdir(parents=True, exist_ok=True)
             self.group_path_dict[group] = path
             # data in config should just reflect th last part of this name
             con = Config(dict({
-                "short_name": groupz,
+                "short_name": group_short,
                 "tests": [],
                 "templates": []
-            }), gconfig)
+            }), group_config)
 
-            con.to_json_file(path / f'__{groupz}.json', indent=4)
+            con.to_json_file(path / f'__{group_short}.json', indent=4)
             self.logger.info(f"Santa_IW group path {group} at {path}")
 
-        self.secrets_path = self.santa_config_dir.parent / "SECRETS" / "santa_secrets.json"
-        if not self.secrets_path.exists():
-            placeholder = Config()
-            placeholder.set_item("__SECRETS_HELP__", "https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/Secrets")
-            placeholder.to_json_file(self.secrets_path, indent=4)
-
-        Config.set_secrets(self.secrets_path)
-
-    @classmethod
-    def demo(cls):
-        _ = MakeLists()
-
-    def write_config(self):
-        pout = self.santa_config_dir / 'santa_config.json'
-        nuke_user_config = bool(self.config.get_item("nuke_user_config", default=False))
-        if pout.exists() and not nuke_user_config:
-            self.logger.warning(f"Santa_IW config file {pout} already exists -- not overwritten")
-        else:
-            self.user_config.to_json_file(pout, indent=4)
-
     def loop_over_scans(self):
-        scan_defaults = self.config.get_item("scan_defaults")
-        scans = self.config.get_item("scans")
+        scan_defaults = self.discovery_config.get_item("scan_defaults")
+        scans = self.discovery_config.get_item("scans")
         for scan in scans:
-            scan_config = Config(scan, scan_defaults, self.config)
+            scan_config = Config(scan, scan_defaults, self.discovery_config)
             self.perform_one_scan(scan_config)
 
         self.logger.info(f"Phase one, identify hosts")
         futures = [self.worker_pool.submit(candidate.identify) for candidate in self.candidate_hosts]
         for future in futures:
             future.result()
         self.logger.info(f"Phase two, process hosts")
@@ -773,42 +712,69 @@
                     parts = line.split()
                     cidr_range = parts[3]
                     break
             else:
                 self.logger.error(f"Could not find ip address {local_info.ip} in {r.so_lines}")
                 exit(1)
             network = IPv4Network(cidr_range, strict=False)
-            net0 = network.network_address
-            netz = network.broadcast_address
-            inet0 = self.ipv4_to_int(net0) + 1
-            inetz = self.ipv4_to_int(netz) - 1
-            inetz = min(inetz, inet0 + 512 - 3)
-            first_address = IPv4Address(inet0)
-            last_address = IPv4Address(inetz)
+            net_addr_start = network.network_address
+            net_addr_end = network.broadcast_address
+            int_net_addr_start = self.ipv4_to_int(net_addr_start) + 1
+            int_net_addr_end = self.ipv4_to_int(net_addr_end) - 1
+            # given huge range, limit to x.y.0.1 through x.y.4.254
+            int_net_addr_end = min(int_net_addr_end, int_net_addr_start + (5 * 256) - 3)
+            first_address = IPv4Address(int_net_addr_start)
+            last_address = IPv4Address(int_net_addr_end)
             self.logger.info(f"Santa_IW auto will scan {first_address} -> {last_address}")
         else:
             first_address = IPv4Address(first_ip)
             last_address = IPv4Address(last_ip)
         self.logger.info(
             f"{first_address=} {first_address.packed=} {first_address.compressed=} {last_address.exploded=} {last_address.version=}")
         first_int = self.ipv4_to_int(first_address)
         last_int = self.ipv4_to_int(last_address)
         num = last_int - first_int
         self.logger.info(f"Scanning {num=} addresses {first_address=} {last_address=}")
-        for iaddr in range(first_int, last_int + 1):
-            ip = IPv4Address(iaddr)
-            self.logger.info(f"Scanning {ip=} {iaddr=:x}")
-            x = HostCreator(address=ip, config=scan_config, host_template_dir=self.host_template_dir,
+        for int_addr in range(first_int, last_int + 1):
+            ip = IPv4Address(int_addr)
+            self.logger.info(f"Scanning {ip=} {int_addr=:x}")
+            x = HostCreator(address=ip, config=scan_config, host_template_dir=self.np.santa_discovery_templates_dir,
                             group_paths=self.group_path_dict)
             self.candidate_hosts.append(x)
 
     # noinspection PyMethodMayBeStatic
     def ipv4_to_int(self, ipv4: IPv4Address) -> int:
         byts = ipv4.packed
         v: int = 0
         for byte in byts:
             v = v * 256 + byte
         return v
 
 
-if __name__ == '__main__':
-    MakeLists.demo()
+# noinspection DuplicatedCode
+class Discovery(Subassembly):
+
+    def __init__(self, instance_config: Config, short_name: str, parent: Subassembly):
+        super().__init__(instance_config=instance_config, parent=parent,
+                         short_name=short_name)  # super defines self.logger
+        self.plugin_type_map: dict[str, PluginType] = {}
+        self.plugin_instance_map: dict[str, PluginBase] = {}
+        self.plugin_names_not_found: set[str] = set()
+        # failure within a test type does not imply factory failure
+        self._propagate_child_stats_in_overall = False
+        self.np = NorthPole()
+
+    def start(self) -> None:
+        # fixme add rotation later
+        if self.np.santa_discovery_config_dir.is_dir():
+            self.log_internal_status(Status.OK, message=f"Keeping Previous Network Discovery at {self.np.santa_discovery_config_dir}")
+        else:
+            et=ElapsedTime("discovery")
+            self.log_internal_status(Status.MAINT,message="Performing network discovery")
+            _ = MakeListsEmbedded(self.config(), self.np)
+            et.stop()
+            self.log_internal_status(Status.OK,message=f"Net discovery completed {et}")
+
+    def report(self) -> str:
+        out = super().report()
+        out += "\n"
+        return out
```

### Comparing `santa_iw-0.6.1/Santa_IW/Naughty.py` & `santa_iw-0.7.4/Santa_IW/Naughty.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from libsrg.Config import Config
 
+from Santa_IW.Node import Node
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
+from Santa_IW.TestBase import TestBase
 
 
 class Naughty(Subassembly):
     """
     Data Recording subassembly
 
     """
@@ -24,15 +26,15 @@
         Subassembly.register_global_status_observer(self.observe_subsystem_status)
 
         self.log_internal_status(Status.OK, "Running...", assess=True)
         # self.logger.info("Finished")
 
     # noinspection PyUnusedLocal
     def observe_subsystem_status(self, child: Subassembly, status: Status, attention: bool, assess=True) -> None:
-        if status.value > Status.OK.value or attention:
+        if status.value > Status.OK.value or attention and (isinstance(child, TestBase) or isinstance(child, Node)):
             self._suspects |= {child}
             msg = f"Add Suspect {child.short_name()} {status=} {attention=}"
         else:
             self._suspects -= {child}
             msg = f"Clear Suspect {child.short_name()} {status=} {attention=}"
         self.logger.info(msg)
         self.set_annotation(msg)
```

### Comparing `santa_iw-0.6.1/Santa_IW/Node.py` & `santa_iw-0.7.4/Santa_IW/Node.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/NodeFactory.py` & `santa_iw-0.7.4/Santa_IW/NodeFactory.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,85 +19,86 @@
 
     """
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent,
                          short_name=short_name)  # super defines self.logger
         # self.logger.info(map_chain_as_str(self.args))
-        self.nodemap: dict[str, Any] = {}
+        self.node_dict: dict[str, Any] = {}
 
     def start(self) -> None:
         self.set_annotation("Loading Nodes...")
         self.log_internal_status(Status.OK, "Started", assess=True)
         # self.logger.info("Started")
         # self.logger.info(map_chain_as_str(self.args))
         tf: TestFactory = self.config().get_item("test_factory")
         tpf: TemplateFactory = self.config().get_item("template_factory")
-        nodedirs: list[str] = self.config().get_item("nodedirs")
-        for nodedir in nodedirs:
-            dpath = Path(nodedir).resolve()
+        node_dirs: list[str] = self.config().get_item("node_dirs")
+        for node_dir in node_dirs:
+            dpath = Path(node_dir).resolve()
             self.process_node_subdir(dpath, group_below=self.tree_root_subassembly, tf=tf, tpf=tpf)
 
         self.set_annotation("Done")
-        self.log_internal_status(Status.OK, "Done", assess=True)
+        self.log_internal_status(Status.OK, message=f"Loaded {len(self.node_dict)} nodes", assess=True)
         # self.logger.info("Finished")
 
     def process_node_subdir(self, dpath, group_below: Subassembly, tf: TestFactory, tpf: TemplateFactory):
-        self.logger.info(f"Looking in {dpath} for group below {group_below.name()}")
-        if dpath.is_dir():
+        if not dpath.is_dir():
+            self.log_internal_status(Status.OK, f"Not a directory: {dpath} for group below {group_below.name()}", assess=True)
+        else:
+            self.log_internal_status(Status.OK, f"Looking in {dpath} for group below {group_below.name()}", assess=True)
             # first pass (group_pass=True) we are looking for special __file
             for group_pass in [True, False]:
                 count_in_pass = 0
-                for nodefile in dpath.glob("*.json"):
-                    special = nodefile.stem.startswith("__")
+                for node_file in dpath.glob("*.json"):
+                    special = node_file.stem.startswith("__")
                     if group_pass != special:
                         continue
-                    self.logger.info(f"loading {nodefile}")
+                    self.logger.info(f"loading {node_file}")
                     # noinspection PyBroadException
                     try:
-                        data = Config(nodefile)
-                        data["__LOADED_FROM__"] = str(nodefile)
+                        data = Config(node_file)
+                        data["__LOADED_FROM__"] = str(node_file)
                     except Exception as e:
-                        msg = f"Error parsing {nodefile} {e}"
+                        msg = f"Error parsing {node_file} {e}"
                         self.log_internal_status(Status.CRITICAL, msg)
                         self.logger.exception(msg, stack_info=True, exc_info=True)
                         continue
                     if int(data.get_item("register", default=1)) == 0:
-                        self.logger.info(f"node not registered {nodefile} to {data}")
+                        self.logger.info(f"node not registered {node_file} to {data}")
                         continue
                     if group_pass:
                         count_in_pass += 1
                         if count_in_pass > 1:
-                            msg = f"More than one special node file in directory {nodefile}"
+                            msg = f"More than one special node file in directory {node_file}"
                             self.logger.info(msg)
                             self.log_internal_status(Status.CRITICAL, msg, assess=True)
                             raise Exception(msg)
                         if "group_below" in data:
                             group_below = data["group_below"]
-                    self.logger.info(f"parsed {nodefile} to {data} below {group_below.name()}")
+                    self.logger.info(f"parsed {node_file} to {data} below {group_below.name()}")
                     tpf.apply_templates(data)
                     short_name = data.get_item("short_name")
                     self.log_internal_status(Status.OK, f"Creating node {short_name} below {group_below.name()}")
                     node = Node(instance_config=data, short_name=short_name, parent=group_below)
-                    self.nodemap[short_name] = node
+                    self.node_dict[short_name] = node
                     if group_pass:
                         group_below = node
                     tf.create_tests_for_node(node, data)
-            # all files in this directory processed, examine subdirs
+            # all files in this directory processed, examine sub_dirs
             for subdir in dpath.iterdir():
                 if not subdir.is_dir():
                     continue
                 self.process_node_subdir(subdir, group_below, tf=tf, tpf=tpf)
 
     def start_nodes(self):
-        self.logger.info(self.nodemap)
-        for node in self.nodemap.values():
+        self.logger.info(self.node_dict)
+        for node in self.node_dict.values():
             self.logger.info(f"Starting {node}")
             node.start()
 
     @log_entry_and_exit
     def create(self, node_args: ChainMap[str, Any], test_args: dict[str, Any]) -> TestBase:
         name = test_args["test_type"]
-        # self.logger.info(f"Creating {name} from\n {map_chain_as_str(self.nodemap)}")
-        test_class = self.nodemap[name]
+        test_class = self.node_dict[name]
         test = test_class(node_args, test_args)
         return test
```

### Comparing `santa_iw-0.6.1/Santa_IW/PluginBase.py` & `santa_iw-0.7.4/Santa_IW/PluginBase.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/PluginFactory.py` & `santa_iw-0.7.4/Santa_IW/PluginFactory.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,42 +8,47 @@
 
 from Santa_IW.PluginBase import PluginBase
 from Santa_IW.PluginType import PluginType
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
 
 
+# noinspection DuplicatedCode
 class PluginFactory(Subassembly):
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent,
                          short_name=short_name)  # super defines self.logger
         self.plugin_type_map: dict[str, PluginType] = {}
         self.plugin_instance_map: dict[str, PluginBase] = {}
         self.plugin_names_not_found: set[str] = set()
         # failure within a test type does not imply factory failure
         self._propagate_child_stats_in_overall = False
 
     def start(self) -> None:
         self.scan_plugin_classes()
         self.scan_plugin_configs()
-        self.log_internal_status(Status.OK, message="Loading Complete", assess=True)
+        self.log_internal_status(Status.OK,
+                                 message=f"Loaded {len(self.plugin_type_map)} Plugin Types and {len(self.plugin_instance_map)} Plugin Instances",
+                                 assess=True)
 
     def scan_plugin_classes(self):
         self.set_annotation("Loading Plugin Classes...")
         self.log_internal_status(Status.OK, "Started", assess=True)
         module_dirs = self.config().get_item("plugin_modules_dirs")
         for module_dir in module_dirs:
             dpath = Path(module_dir).resolve()
-            self.logger.info(f"Looking in {dpath}")
-            if dpath.is_dir():
+            if not dpath.is_dir():
+                self.log_internal_status(Status.WARNING, f"{dpath} is not a directory", assess=True)
+            else:
+                self.log_internal_status(Status.OK, f"Looking in {dpath}", assess=True)
                 for module_file in dpath.glob("*.py"):
-                    fname = module_file.stem
+                    file_name = module_file.stem
                     # problem with __init__.py
-                    if fname.startswith("_"):
+                    if file_name.startswith("_"):
                         continue
                     # noinspection PyBroadException
                     try:
                         self.load_module_file(module_file)
                     except Exception as e:
                         self.logger.exception(e, stack_info=True, exc_info=True)
                         self.log_internal_status(Status.CRITICAL, f"Failed to load test file {module_file} {e}",
@@ -66,35 +71,34 @@
         for alias, config in all_configs.items():
             plugin_type: PluginType = PluginType(instance_config=config, parent=module_types_parent, short_name=alias,
                                                  plugin_class=plugin_class)
             self.plugin_type_map[alias] = plugin_type
 
     def create_plugin_instance(self, plugin_args: Config) -> None:
         name = plugin_args.get_item("plugin_type")
-        short= plugin_args.get_item("short_name")
+        short = plugin_args.get_item("short_name")
         if name in self.plugin_type_map:
             plugin_type: PluginType = self.plugin_type_map[name]
             plugin_class: Type[PluginBase] = plugin_type.get_plugin_class()
 
             try:
                 self.logger.info("About to create plugin instance {name}")
                 plugin: PluginBase = plugin_class(instance_config=plugin_args, short_name=short, parent=plugin_type)
                 self.logger.info("About to save plugin type {name}")
                 self.plugin_instance_map[plugin.name()] = plugin
                 # self.log_internal_status(Status.OK, f"created {test.name()}", assess=True)
             except Exception as e:
-                self.logger.exception(f"constructor {name} failed for {plugin_args}\n{e}", stack_info=True, exc_info=True)
+                self.logger.exception(f"constructor {name} failed for {plugin_args}\n{e}", stack_info=True,
+                                      exc_info=True)
                 plugin_type.log_internal_status(Status.CRITICAL, f"constructor failed {name} {short}", assess=True)
         else:
             self.logger.error(f"plugin {name} not found")
             self.plugin_names_not_found |= {name}
             self.log_internal_status(Status.WARNING, f"no plugin class {name}", assess=True)
 
-
-
     def get_all_plugins(self) -> List[PluginBase]:
         return sorted(list(self.plugin_instance_map.values()))
 
     def report_all_plugins(self) -> str:
         return self.report()
 
     def report(self) -> str:
@@ -114,15 +118,14 @@
 
         # out += "\n\nTest Statistics"
         # for test in all_tests:
         #     out += test.report()
         #     out += "------\n"
         return out
 
-
     def scan_plugin_configs(self):
         self.set_annotation("Loading Plugin Configs...")
         self.log_internal_status(Status.OK, "Started Plugin Configs", assess=True)
         config_dirs = self.config().get_item("plugin_config_dirs")
         for config_dir in config_dirs:
             dpath = Path(config_dir).resolve()
             self.logger.info(f"Looking in {dpath}")
@@ -130,9 +133,10 @@
                 for config_file in dpath.glob("*.json"):
                     # noinspection PyBroadException
                     try:
                         mod_config = Config(config_file)
                         self.create_plugin_instance(plugin_args=mod_config)
                     except Exception as e:
                         self.logger.exception(e, stack_info=True, exc_info=True)
-                        self.log_internal_status(Status.CRITICAL, f"Failed to load plugin config file {config_file} {e}",
+                        self.log_internal_status(Status.CRITICAL,
+                                                 f"Failed to load plugin config file {config_file} {e}",
                                                  assess=True)
```

### Comparing `santa_iw-0.6.1/Santa_IW/PluginType.py` & `santa_iw-0.7.4/Santa_IW/PluginType.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Status.py` & `santa_iw-0.7.4/Santa_IW/Status.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Subassembly.py` & `santa_iw-0.7.4/Santa_IW/Subassembly.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/TemplateFactory.py` & `santa_iw-0.7.4/Santa_IW/TemplateFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,48 +14,51 @@
 
     """
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent,
                          short_name=short_name)  # super defines self.logger
         # self.logger.info(map_chain_as_str(self.args))
-        self.templatemap: dict[str, Any] = {}
+        self.template_dict: dict[str, Any] = {}
         self.template_names_not_found: set[str] = set()
         self.template_used_by: dict[str, set[str]] = {}
 
     def start(self) -> None:
         self.set_annotation("Loading Templates...")
         self.log_internal_status(Status.OK, "Started", assess=True)
         # self.logger.info("Started")
         # self.logger.info(map_chain_as_str(self.args))
-        templatedirs = self.config().get_item("templatedirs")
-        for templatedir in templatedirs:
-            dpath = Path(templatedir).resolve()
-            self.logger.info(f"Looking in {dpath}")
-            if dpath.is_dir():
-                for templatefile in dpath.glob("*.json"):
+        template_dirs = self.config().get_item("template_dirs")
+        for template_dir in template_dirs:
+            dpath = Path(template_dir).resolve()
+            if not dpath.is_dir():
+                self.log_internal_status(Status.WARNING, f"Not a directory: {str(dpath)!r}", assess=True)
+            else:
+                self.log_internal_status(Status.OK, f"Loading {dpath}", assess=True)
+                for template_file in dpath.glob("*.json"):
                     try:
-                        self.logger.info(f"loading {templatefile}")
-                        with open(templatefile, "r") as f:
+                        self.logger.info(f"loading {template_file}")
+                        with open(template_file, "r") as f:
                             data = json.load(f)
-                        self.logger.info(f"parsed {templatefile} to {data}")
-                        templatename = templatefile.stem
-                        if templatename in self.templatemap:
+                        self.logger.info(f"parsed {template_file} to {data}")
+                        template_name = template_file.stem
+                        if template_name in self.template_dict:
                             self.log_internal_status(Status.WARNING,
-                                                     f"Template {templatename} already loaded, ignoring {templatefile}")
+                                                     f"Template {template_name} already loaded, ignoring {template_file}")
                         else:
-                            self.templatemap[templatename] = data
-                            self.template_used_by[templatename] = set()
+                            self.template_dict[template_name] = data
+                            self.template_used_by[template_name] = set()
                     except Exception as e:
                         self.logger.exception(e, stack_info=True, exc_info=True)
-                        self.log_internal_status(Status.WARNING, f"Template did not load {templatefile} {e}")
-        self.log_internal_status(Status.OK, "Done", assess=True)
-        self.set_annotation("Done")
+                        self.log_internal_status(Status.WARNING, f"Template did not load {template_file} {e}")
+        self.log_internal_status(Status.OK, message=f"Loaded {len(self.template_dict)} Templates, {len(self.template_names_not_found)} names not found", assess=True)
         # self.logger.info("Finished")
 
+
+
     def apply_templates(self, data: Config) -> Config:
         pending = data.get("templates", []).copy()
         applied = []
         if "tests" not in data:
             data["tests"] = []
         while len(pending) > 0:
             template_name = pending.pop(0)
@@ -66,21 +69,21 @@
             if template_name in applied:
                 msg = f"template {template_name} reload ignored"
                 self.logger.warning(msg)
                 self.log_internal_status(Status.WARNING, msg, assess=True)
 
                 continue
             applied.append(template_name)
-            if template_name not in self.templatemap:
+            if template_name not in self.template_dict:
                 msg = f"template {template_name} requested but not found"
                 self.logger.warning(msg)
                 self.log_internal_status(Status.WARNING, msg, assess=True)
                 self.template_names_not_found |= {template_name}
                 continue
-            template = self.templatemap[template_name]
+            template = self.template_dict[template_name]
             self.template_used_by[template_name] |= {data.get_item("short_name")}
             for test_x in template.get("tests", []):
                 data["tests"].append(test_x)
             for template_x in template.get("templates", []):
                 pending.append(template_x)
         data["templates_applied"] = applied
```

### Comparing `santa_iw-0.6.1/Santa_IW/TestBase.py` & `santa_iw-0.7.4/Santa_IW/TestBase.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/TestFactory.py` & `santa_iw-0.7.4/Santa_IW/TestFactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 import importlib
 import importlib.util
 import sys
 from collections import Counter
 from pathlib import Path
-from typing import List, Type
+from typing import List, Type, Any
 
 from libsrg.Config import Config
 
 from Santa_IW.Node import Node
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import TestBase
 from Santa_IW.TestType import TestType
 
 
+# noinspection DuplicatedCode
 class TestFactory(Subassembly):
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent,
                          short_name=short_name)  # super defines self.logger
+        self.test_class_map: dict[str, Any] = {}
         self.test_type_map: dict[str, TestType] = {}
         self.test_instance_map: dict[str, TestBase] = {}
         self.tests_names_not_found: set[str] = set()
         # failure within a test type does not imply factory failure
         self._propagate_child_stats_in_overall = False
         self.test_used_by: dict[str, set[str]] = {}
 
     def start(self) -> None:
         self.set_annotation("Loading Test Classes...")
         self.log_internal_status(Status.OK, "Started", assess=True)
-        testdirs = self.config().get_item("testdirs")
-        for test_dir in testdirs:
+        test_dirs = self.config().get_item("test_modules_dirs")
+        for test_dir in test_dirs:
             dpath = Path(test_dir).resolve()
-            self.logger.info(f"Looking in {dpath}")
-            if dpath.is_dir():
+            if not dpath.is_dir():
+                self.log_internal_status(Status.WARNING, f"{dpath} is not a directory", assess=True)
+            else:
+                self.log_internal_status(Status.OK,f"Loading tests from {dpath}...", assess=True)
                 for testfile in dpath.glob("*.py"):
-                    fname = testfile.stem
+                    file_name = testfile.stem
                     # problem with __init__.py
-                    if fname.startswith("_"):
+                    if file_name.startswith("_"):
                         continue
                     # noinspection PyBroadException
                     try:
                         self.load_testfile(testfile)
                     except Exception as e:
                         self.logger.exception(e, stack_info=True, exc_info=True)
                         self.log_internal_status(Status.CRITICAL, f"Failed to load test file {testfile} {e}",
                                                  assess=True)
 
         self.set_annotation("Done")
-        self.log_internal_status(Status.OK, "Loading Complete", assess=True)
+        self.log_internal_status(Status.OK, message=f"Loaded {len(self.test_type_map)} test types and {len(self.test_instance_map)} test instances", assess=True)
         self.logger.info("Finished")
 
+    def spawn(self):
+        # no new thread, but update status
+        self.log_internal_status(Status.OK, message=f"Loaded {len(self.test_class_map)} Test Classes, {len(self.test_type_map)} Test Types, and {len(self.test_instance_map)} Test Instances", assess=True)
+
+
     def load_testfile(self, testfile):
         self.logger.info(f"Loading {testfile!s}")
         module_name = testfile.stem
         file_path = str(testfile)
         spec = importlib.util.spec_from_file_location(module_name, file_path)
         module = importlib.util.module_from_spec(spec)
         sys.modules[module_name] = module
         spec.loader.exec_module(module)
 
         helper = module.helper
-        testclass = helper.get_loaded_class()
+        test_class = helper.get_loaded_class()
         all_configs = helper.get_all_configs()
         self.logger.info(f"{file_path} supports DiscoveryHelper")
-
+        self.test_class_map[module_name]= file_path
         test_types = self.config().get_item("test_types")
         for alias, config in all_configs.items():
             test_type: TestType = TestType(instance_config=config, parent=test_types, short_name=alias,
-                                           test_class=testclass)
+                                           test_class=test_class)
             self.test_used_by[alias] = set()
             self.test_type_map[alias] = test_type
 
     def create_one_test(self, node: Node, test_args: Config, short: str) -> None:
         name = test_args["test_type"]
         if name in self.test_type_map:
             test_type: TestType = self.test_type_map[name]
@@ -82,19 +91,20 @@
             try:
                 self.logger.info("About to create test type {name} for {node.name()}")
                 test: TestBase = test_class(instance_config=test_args, short_name=short, parent=node,
                                             stepparent=stepparent)
                 self.logger.info("About to save test type {name} for {node.name()}")
                 self.test_instance_map[test.name()] = test
                 # self.log_internal_status(Status.OK, f"created {test.name()}", assess=True)
+
             except Exception as e:
                 self.logger.exception(f"constructor {name} failed for {test_args}\n{e}", stack_info=True, exc_info=True)
                 test_type.log_internal_status(Status.CRITICAL, f"constructor failed {name} {short}", assess=True)
         else:
-            self.logger.error(f"testclass {name} not found")
+            self.logger.error(f"test_class {name} not found")
             self.tests_names_not_found |= {name}
             self.log_internal_status(Status.WARNING, f"no test class {name}", assess=True)
 
     def get_test(self, name: str) -> TestBase:
         return self.test_instance_map[name]
 
     def get_all_tests(self) -> List[TestBase]:
@@ -110,18 +120,18 @@
         all_tests = self.get_all_tests()
         out += f"There are {len(all_tests)} instances of {len(self.test_type_map)} test types\n"
         if self.tests_names_not_found:
             out += f"\nThere are {len(self.tests_names_not_found)} test class names not found:\n"
             for test in self.tests_names_not_found:
                 out += f"  {test}\n"
 
-        out += f"\n\nTest Alias -> Classes @ Module :\n"
+        out += f"\n\nTest Alias -> Module.Class :\n"
         for k, v in self.test_type_map.items():
             tc:Type[TestBase] = v.get_test_class()
-            out += f"\t{k:<30} -> {tc.__name__:<30} @ {tc.__module__:<30}\n"
+            out += f"\t{k:<30} -> {tc.__module__}.{tc.__name__}\n"
 
         out += "\nTest Alias Usage:\n"
         names: list[str] = list(self.test_used_by.keys())
         names.sort()
         for name in names:
             val = self.test_used_by[name]
             if len(val) != 0:
@@ -130,38 +140,38 @@
         for name in names:
             val = self.test_used_by[name]
             if len(val) == 0:
                 out += f"\t{name}\n"
         return out
 
     def create_tests_for_node(self, node: Node, data: Config) -> None:
-        testargs: list[Config] = [Config(ti) for ti in data["tests"]]
+        test_args: list[Config] = [Config(ti) for ti in data["tests"]]
         dup_counter = Counter()
         test_sep = self.config().get_item("tree_test_separator")
         # first pass determines short name and counts duplicate names within same node
 
-        for testinfo in testargs:
-            if int(testinfo.get_item("register", default=1)) > 0:
-                testclass = testinfo["test_type"]
-                name = testinfo.get_item("instance_name", "name", "copy", default="")
-                short: str = testclass + test_sep + name
+        for test_info in test_args:
+            if int(test_info.get_item("register", default=1)) > 0:
+                test_class = test_info["test_type"]
+                name = test_info.get_item("instance_name", "name", "copy", default="")
+                short: str = test_class + test_sep + name
                 if short.startswith("Check"):
                     short = short.replace("Check", "", 1)
-                testinfo["short_name"] = short
+                test_info["short_name"] = short
                 dup_counter[short] += 1
         instance_counter = Counter()
-        # second pass adds numeric suffix where first pass found dups
+        # second pass adds numeric suffix where first pass found duplicates
         # then constructs test
-        for testinfo in testargs:
-            reg = int(testinfo.get_item("register", default=1)) > 0
+        for test_info in test_args:
+            reg = int(test_info.get_item("register", default=1)) > 0
             if reg:
-                short = testinfo["short_name"]
+                short = test_info["short_name"]
                 if dup_counter[short] > 1:
                     n = instance_counter[short]
                     instance_counter[short] += 1
                     if not short.endswith(test_sep):
                         short += "_"
                     short += f"{n:02d}"
-                self.create_one_test(node=node, test_args=testinfo, short=short)
+                self.create_one_test(node=node, test_args=test_info, short=short)
         if self.tests_names_not_found:
             msg = f"{len(self.tests_names_not_found)} Test Classes not found "
             self.log_internal_status(Status.WARNING, msg)
```

### Comparing `santa_iw-0.6.1/Santa_IW/TestType.py` & `santa_iw-0.7.4/Santa_IW/TestType.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/TreeRoot.py` & `santa_iw-0.7.4/Santa_IW/TreeRoot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from threading import Thread
 
 from libsrg.Config import Config
 
 from Santa_IW.DataRecording import DataRecording
+from Santa_IW.Discovery import Discovery
 from Santa_IW.Flask.WebGUI import WebGUI
 from Santa_IW.Naughty import Naughty
 from Santa_IW.Node import Node
 from Santa_IW.NodeFactory import NodeFactory
 from Santa_IW.PluginFactory import PluginFactory
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
@@ -44,24 +45,27 @@
 
         self.node_factory = NodeFactory(parent=self.sw_subsystems, short_name="NodeFactory", instance_config=sw_args)
         self.naughty = Naughty(parent=self.sw_subsystems, short_name="Naughty", instance_config=sw_args)
         self.test_types = Node(parent=self.sw_subsystems, short_name="TestTypes", instance_config=sw_args)
 
         self.plugin_factory = PluginFactory(parent=self.sw_subsystems, short_name="PluginFactory",
                                             instance_config=sw_args)
+        self.discovery = Discovery(parent=self.sw_subsystems, short_name="Discovery",
+                                   instance_config=sw_args)
 
         # These callback arguments will become visible in the children before start,
         # but are not valid within constructors
         self.sw_subsystems.config().set_item("node_factory", self.node_factory)
         self.sw_subsystems.config().set_item("test_factory", self.test_factory)
         self.sw_subsystems.config().set_item("template_factory", self.template_factory)
         self.sw_subsystems.config().set_item("data_recording", self.data_recording)
         self.sw_subsystems.config().set_item("naughty", self.naughty)
         self.sw_subsystems.config().set_item("test_types", self.test_types)
         self.sw_subsystems.config().set_item("plugin_factory", self.test_factory)
+        self.sw_subsystems.config().set_item("discovery", self.discovery)
 
         secrets_file = self.config().get_item("secrets_file")
         Config.set_secrets(secrets_file, dict(os.environ))
 
     def start(self) -> None:
         self.mark_subsystem_enabled()
         self.log_internal_status(Status.OK, "Creating new thread for treeroot")
@@ -71,28 +75,35 @@
         self.log_internal_status(Status.OK, "Letting GUI takeover main thread")
         self.webgui.takeover_main_thread()
 
     def _run_in_thread(self):
         self.logger.info("TreeRoot Started")
         self.set_annotation("Startup...")
 
-        self.plugin_factory.start()
-
+        self.set_annotation("Loading Data Recording...")
         self.data_recording.start()
-        self.naughty.start()
 
         self.set_annotation("Loading Test Classes...")
         self.test_factory.start()
 
+        self.set_annotation("Network Discovery...")
+        self.discovery.start()
+
+        self.set_annotation("Plugin Factory...")
+        self.plugin_factory.start()
+
         self.set_annotation("Loading Templates...")
         self.template_factory.start()
 
         self.set_annotation("Loading Nodes...")
         self.node_factory.start()
 
+        self.set_annotation("Naughty List...")
+        self.naughty.start()
+
         self.set_annotation("Spawning tests...")
         self.spawn()
         self.set_annotation("Running tests...")
 
     def shutdown_instance(self):
         super().shutdown_instance()
         self.logger.info("===================================================================================")
```

### Comparing `santa_iw-0.6.1/Santa_IW/UnitTests/DBConnection_test.py` & `santa_iw-0.7.4/Santa_IW/UnitTests/DBConnection_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import math
 import os
 import unittest
 from pathlib import Path
-from time import time
 
 from Santa_IW.DBConnection import DBConnection
 
 dbpath = Path("/tmp/test_SQLite.db")
 
 
 class MyTestCase(unittest.TestCase):
+    # noinspection PyUnreachableCode
     def test_SQLite_clean(self):
         if dbpath.exists():
             os.remove(dbpath)
         db = DBConnection(dbpath)
         self.assertIsNotNone(db)
-        return # FIXME
+        return  # FIXME #169
         with db as cur:
             res = cur.execute("SELECT name FROM sqlite_master")
             a = res.fetchone()
             print(a)
             self.assertIsNone(a)
 
             cur.execute("""CREATE TABLE asamples (
@@ -29,21 +29,21 @@
                  value float
                  )        """)
             tables = db.all_tables()
             print(tables)
             self.assertEqual(('asamples',), tables)  # add assertion here
         db.close()
 
+    # noinspection PyUnreachableCode
     def test_repopen(self):
         if dbpath.exists():
             os.remove(dbpath)
         db = DBConnection(dbpath)
-        now = time()
         self.assertIsNotNone(db)
-        return # FIXME
+        return  # FIXME #169
         with db as cur:
             cur.execute("""CREATE TABLE asamples (
                 name text,
                  count integer,
                  time float,
                  value float
                  )        """)
```

### Comparing `santa_iw-0.6.1/Santa_IW/UnitTests/Status_test.py` & `santa_iw-0.7.4/Santa_IW/UnitTests/Status_test.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/UnitTests/Subassembly_test.py` & `santa_iw-0.7.4/Santa_IW/UnitTests/Subassembly_test.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/Santa_IW/Utils.py` & `santa_iw-0.7.4/Santa_IW/Utils.py`

 * *Files identical despite different names*

### Comparing `santa_iw-0.6.1/pyproject.toml` & `santa_iw-0.7.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Santa_IW"
-version = "0.6.1"
+version = "0.7.4"
 description = "Santa Is Watching: ZFS Aware Network Monitor"
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -17,15 +17,15 @@
 ]
 packages= [{include='Santa_IW'}]
 # package-mode = false
 
 [tool.poetry.dependencies]
 python = "^3.11"
 jinja2 = ">=3.1.3,<3.2.0"
-libsrg = ">=5.0.0"
+libsrg = ">=5.1.1"
 sphinx = {version = "^7.3.7", optional = true, extras = ["doc"]}
 sphinx-rtd-theme = {version = "^2.0.0", optional = true, extras = ["doc"]}
 sphinxcontrib-napoleon = {version = "^0.7", optional = true, extras = ["doc"]}
 nltk = ">=3.8.1,<3.9.0"
 flask = ">=3.0.2,<3.1.0"
 requests = ">=2.31.0,<2.32.0"
 aiohue = "^4.7.1"
@@ -45,8 +45,13 @@
 [project.urls]
 Homepage = "https://gitlab.com/SRG_gitlab/santa-is-watching"
 Issues = "https://gitlab.com/SRG_gitlab/santa-is-watching/-/issues"
 API = "https://srg_gitlab.gitlab.io/santa-is-watching/index.html"
 Wiki = "https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home"
 
 [tool.poetry.extras]
-doc = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon"]
+doc = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon"]
+
+[tool.poetry.scripts]
+Santa_IW_service_run = "Santa_IW.Main:main"
+SantaSetup = "SantaSetup:main"
+SantaSetupInner = "SantaSetupInner:main"
```

### Comparing `santa_iw-0.6.1/PKG-INFO` & `santa_iw-0.7.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Santa_IW
-Version: 0.6.1
+Version: 0.7.4
 Summary: Santa Is Watching: ZFS Aware Network Monitor
 Author: Steve Goncalo
 Author-email: steven@goncalo.us
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,78 +16,66 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring :: Hardware Watchdog
 Provides-Extra: doc
 Requires-Dist: aiohue (>=4.7.1,<5.0.0)
 Requires-Dist: flask (>=3.0.2,<3.1.0)
 Requires-Dist: jinja2 (>=3.1.3,<3.2.0)
-Requires-Dist: libsrg (>=5.0.0)
+Requires-Dist: libsrg (>=5.1.1)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<3.9.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pathvalidate (>=3.2.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: sphinx-rtd-theme[doc] (>=2.0.0,<3.0.0) ; extra == "doc"
 Requires-Dist: sphinx[doc] (>=7.3.7,<8.0.0) ; extra == "doc"
 Requires-Dist: sphinxcontrib-napoleon[doc] (>=0.7,<0.8) ; extra == "doc"
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sympy (>=1.12,<2.0)
 Description-Content-Type: text/markdown
 
-"Santa Is Watching" (Santa_IW) is a network monitoring tool intended for homelab use. Based upon configuration files
-describing your system, Santa_IW periodically cycles through a suite of tests on your computers, disks, and network
-hardware.
-Santa_IW runs on a
-single Linux computer which needs ssh keys to run diagnostic commands on other computers in your system. Simple ping
-only testing is available for nodes without ssh access. Santa_IW is not forked from or modeled after Nagios, but it
-addresses a
-similar problem space.
-
-Santa_IW includes a network discovery tool called MakeList. MakeList takes a list of start and stop network addresses to
-scan
-and tries to determine what tests are appropriate for each node it finds. Any computer which responds to a network ping
-becomes a candidate for ping testing. If Santa_IW can make an ssh connection to the node, it will:
+["Santa Is Watching" (aka Santa_IW)](https://gitlab.com/SRG_gitlab/santa-is-watching) is a network monitoring tool with an 
+emphasis on ZFS and network attached storage in a homelab environment. Based upon configuration files describing your 
+system, Santa_IW periodically cycles through a suite of
+tests on your computers, disks, and network hardware. Santa_IW runs on a single Linux computer which needs ssh keys
+to run diagnostic commands on other computers in your system. Santa_IW includes a network discovery tool which takes a
+list of start and stop network addresses to scan and tries to determine what tests are appropriate for each node it
+finds. Any computer which responds to a network ping becomes a candidate for ping testing. If Santa_IW can make an 
+ssh connection to the node, it will:
 
 * look at temperature and other data reported by lm-sensors
-* look for drives listed in /etc/fstab and check each for disk free space
+* look for drives listed in /etc/fstab and monitor each for disk free space
 * look for drives supported by smartctl and report SMART status on them
 * look for zfs pools and check each for status and free space
 * look for zfs volumes which seem to be getting frequent snapshots (or are listed in pyznap's config file) and monitor
   the age of the last snapshot
 * look for failed services reported by systemctl --failed
 
-Santa_IW is written in Python and its configuration files are all editable json. It ships with 20+ built in test types
-and
-can load additional user written tests or plugins from user directories. An example plugin is provided to use a Phillips
-Hue color changing light bulb to provide a GREEN/YELLOW/RED status light.
+Santa_IW is written entirely in Python (3.11 or later) and its configuration files are all editable json. It ships with 20+ built in test types
+and can load additional user written tests or plugins from user directories. An example plugin is provided to use a
+Philips Hue color changing light bulb to provide a GREEN/YELLOW/RED status light.
 
 A web based interface lets the user navigate up and down the hierarchy of node groups, nodes and tests to see various
 levels of detail. Tests can record numeric data where appropriate. Running averages are displayed and values over time
 can be graphed or extracted for offline processing.
 
 ----
 
-Santa_IW has been developed and tested on a Linux platform. It has been run on RHEL, Fedora, Ubuntu and Debian
-platforms (including Raspberry Pi 3). It is written in pure Python, but calls out to many Linux/Posix command line
-utilities. It is plausible
-that it might someday work on other Posix compliant platforms (MacOS or BSD), but that is out of scope for the current
-effort. Santa_IW will probably never run natively on Windows, and there are not presently any tests designed to exercise
-Windows nodes beyond a simple ping.
+Santa_IW is hosted on [GitLab](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home) and has been developed and tested on a Linux platform. It has been run installed and run on RHEL, Fedora, Ubuntu
+and Debian platforms (including Raspberry Pi 3). It is written in pure Python, but calls out to many Linux/Posix
+command line utilities. It is plausible that it might someday work on other Posix compliant platforms (macOS or BSD),
+but that is out of scope for the current effort. [For windows support...](https://en.wikipedia.org/wiki/Somebody_else%27s_problem)
 
 Santa_IW is intended for homelab use on an internal network. It does not yet have any robust authentication system and
-should not be exposed on the internet.
+should not be exposed on the open internet.
 
-The code for Santa_IW is pretty much ready for an initial release, but documentation is still being cleaned up.
-If you are reading this, you are a little bit early to the party, but feel free to look around. Installation
-instructions are on the wiki if you are interested in a test drive. I think I have a week or two of documentation tasks
-to complete before I feel comfortable posting to social media in search of beta testers.
+# 🚧 PRE-BETA RELEASE 🚧
 
-----
-Key links:
-
-* [Santa_IW Homepage](https://gitlab.com/SRG_gitlab/santa-is-watching)
-* [Santa_IW Wiki](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home)
-* [Santa_IW API](https://srg_gitlab.gitlab.io/santa-is-watching/index.html)
-* [Santa_IW Issues](https://gitlab.com/SRG_gitlab/santa-is-watching/-/issues)
-* [Libsrg Wiki](https://gitlab.com/SRG_gitlab/libsrg/-/wikis/home)
+If you are reading this, you are a little bit early to the party, but feel free to look
+around. Installation and operating instructions are on the [wiki](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home)
+if you are interested in a test drive. The [Roadmap page]
+(https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/Roadmap) describes some of the work pending before I start 
+inviting people to beta test. The code as-is works well, but many of the pending changes planned will invalidate the 
+documentation. Expecting new users to read the manual once is a big ask these days, so asking them to do it all 
+again after major changes would be too much.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

