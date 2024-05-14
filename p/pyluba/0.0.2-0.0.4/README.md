# Comparing `tmp/pyluba-0.0.2.tar.gz` & `tmp/pyluba-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyluba-0.0.2.tar", max compression
+gzip compressed data, was "pyluba-0.0.4.tar", max compression
```

## Comparing `pyluba-0.0.2.tar` & `pyluba-0.0.4.tar`

### file list

```diff
@@ -1,55 +1,67 @@
--rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.2/LICENSE
--rw-r--r--   0        0        0      660 2024-02-24 00:10:17.430127 pyluba-0.0.2/README.md
--rw-r--r--   0        0        0      744 2024-02-24 08:02:07.442793 pyluba-0.0.2/pyluba/__init__.py
--rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.2/pyluba/aliyun/cloud_gateway.py
--rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.2/pyluba/aliyun/cloud_service.py
--rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.2/pyluba/aliyun/test_alicloud_api_gateway.py
--rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/aliyun/tmp_constant.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/__init__.py
--rw-r--r--   0        0        0     2918 2024-04-23 05:49:02.984986 pyluba-0.0.2/pyluba/bluetooth/ble.py
--rw-r--r--   0        0        0    34772 2024-04-24 23:43:48.736942 pyluba-0.0.2/pyluba/bluetooth/ble_message.py
--rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/const.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/__init__.py
--rw-r--r--   0        0        0     4166 2024-04-24 21:43:54.006537 pyluba-0.0.2/pyluba/bluetooth/data/convert.py
--rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/framectrldata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/model/__init__.py
--rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/bluetooth/data/notifydata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/__init__.py
--rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/__init__.py
--rw-r--r--   0        0        0     1349 2024-04-23 05:07:53.289798 pyluba-0.0.2/pyluba/data/model/excute_boarder_params.py
--rw-r--r--   0        0        0     1075 2024-04-23 05:07:10.891334 pyluba-0.0.2/pyluba/data/model/execute_boarder.py
--rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/generate_route_information.py
--rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/hash_list.py
--rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/mowing_modes.py
--rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/plan.py
--rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/rapid_state.py
--rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/model/region_data.py
--rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.2/pyluba/data/mqtt/__init__.py
--rw-r--r--   0        0        0     1669 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/data/mqtt/event.py
--rw-r--r--   0        0        0     2343 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/data/mqtt/properties.py
--rw-r--r--   0        0        0      924 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/data/mqtt/status.py
--rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/event/__init__.py
--rw-r--r--   0        0        0     1440 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/event/event.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/http/_init_.py
--rw-r--r--   0        0        0     1832 2024-02-24 11:05:42.835293 pyluba-0.0.2/pyluba/http/http.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/luba/_init_.py
--rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/luba/base.py
--rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.2/pyluba/mqtt/mqtt.py
--rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/common.proto
--rw-r--r--   0        0        0     1022 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/common_pb2.py
--rw-r--r--   0        0        0     2699 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/esp_driver.proto
--rw-r--r--   0        0        0     6770 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/esp_driver_pb2.py
--rw-r--r--   0        0        0     1161 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/luba_msg.proto
--rw-r--r--   0        0        0     3365 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/luba_msg_pb2.py
--rw-r--r--   0        0        0      587 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_driver.proto
--rw-r--r--   0        0        0     2124 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_driver_pb2.py
--rw-r--r--   0        0        0     8806 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_nav.proto
--rw-r--r--   0        0        0    18010 2024-02-24 00:10:17.432128 pyluba-0.0.2/pyluba/proto/mctrl_nav_pb2.py
--rw-r--r--   0        0        0     4643 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/proto/mctrl_sys.proto
--rw-r--r--   0        0        0    11241 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/proto/mctrl_sys_pb2.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/py.typed
--rw-r--r--   0        0        0     2134 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/utility/constant/device_constant.py
--rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/utility/periodic.py
--rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.2/pyluba/utility/rocker_util.py
--rw-r--r--   0        0        0     1293 2024-04-24 23:46:30.703512 pyluba-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 pyluba-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.4/LICENSE
+-rw-r--r--   0        0        0      742 2024-05-08 21:27:25.359942 pyluba-0.0.4/README.md
+-rw-r--r--   0        0        0      903 2024-05-14 09:31:14.376882 pyluba-0.0.4/pyluba/__init__.py
+-rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.4/pyluba/aliyun/cloud_gateway.py
+-rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.4/pyluba/aliyun/cloud_service.py
+-rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.4/pyluba/aliyun/test_alicloud_api_gateway.py
+-rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/aliyun/tmp_constant.py
+-rw-r--r--   0        0        0       43 2024-05-08 22:13:38.998098 pyluba-0.0.4/pyluba/bluetooth/__init__.py
+-rw-r--r--   0        0        0     2495 2024-05-08 22:35:28.441708 pyluba-0.0.4/pyluba/bluetooth/ble.py
+-rw-r--r--   0        0        0    40449 2024-05-14 09:30:20.272669 pyluba-0.0.4/pyluba/bluetooth/ble_message.py
+-rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/bluetooth/const.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/bluetooth/data/__init__.py
+-rw-r--r--   0        0        0     4455 2024-05-14 09:19:33.644102 pyluba-0.0.4/pyluba/bluetooth/data/convert.py
+-rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/bluetooth/data/framectrldata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/bluetooth/data/model/__init__.py
+-rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/bluetooth/data/notifydata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/__init__.py
+-rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/model/__init__.py
+-rw-r--r--   0        0        0     1349 2024-04-23 05:07:53.289798 pyluba-0.0.4/pyluba/data/model/excute_boarder_params.py
+-rw-r--r--   0        0        0     1075 2024-04-23 05:07:10.891334 pyluba-0.0.4/pyluba/data/model/execute_boarder.py
+-rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/model/generate_route_information.py
+-rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/model/hash_list.py
+-rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/model/mowing_modes.py
+-rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/model/plan.py
+-rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/model/rapid_state.py
+-rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/model/region_data.py
+-rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.4/pyluba/data/mqtt/__init__.py
+-rw-r--r--   0        0        0     1669 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/data/mqtt/event.py
+-rw-r--r--   0        0        0     2343 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/data/mqtt/properties.py
+-rw-r--r--   0        0        0      924 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/data/mqtt/status.py
+-rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/event/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-29 23:01:28.524663 pyluba-0.0.4/pyluba/event/event.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/http/_init_.py
+-rw-r--r--   0        0        0     1832 2024-02-24 11:05:42.835293 pyluba-0.0.4/pyluba/http/http.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/luba/_init_.py
+-rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/luba/base.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:38.823703 pyluba-0.0.4/pyluba/mammotion/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:22.155845 pyluba-0.0.4/pyluba/mammotion/commands/proto.py
+-rw-r--r--   0        0        0       47 2024-05-14 09:11:29.107222 pyluba-0.0.4/pyluba/mammotion/devices/__init__.py
+-rw-r--r--   0        0        0    14989 2024-05-14 08:49:20.985172 pyluba-0.0.4/pyluba/mammotion/devices/luba.py
+-rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.4/pyluba/mqtt/mqtt.py
+-rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.4/pyluba/proto/common.proto
+-rw-r--r--   0        0        0      428 2024-05-08 21:10:33.874300 pyluba-0.0.4/pyluba/proto/common_p2p.py
+-rw-r--r--   0        0        0     1015 2024-04-25 20:48:27.244814 pyluba-0.0.4/pyluba/proto/common_pb2.py
+-rw-r--r--   0        0        0     3330 2024-05-13 07:27:07.774053 pyluba-0.0.4/pyluba/proto/dev_net.proto
+-rw-r--r--   0        0        0     5090 2024-05-13 20:01:44.718647 pyluba-0.0.4/pyluba/proto/dev_net_p2p.py
+-rw-r--r--   0        0        0     6968 2024-05-13 07:28:18.216030 pyluba-0.0.4/pyluba/proto/dev_net_pb2.py
+-rw-r--r--   0        0        0     1271 2024-05-12 22:00:22.601976 pyluba-0.0.4/pyluba/proto/luba_msg.proto
+-rw-r--r--   0        0        0     1984 2024-05-08 21:10:25.440293 pyluba-0.0.4/pyluba/proto/luba_msg_p2p.py
+-rw-r--r--   0        0        0     3575 2024-05-12 22:27:40.502487 pyluba-0.0.4/pyluba/proto/luba_msg_pb2.py
+-rw-r--r--   0        0        0      589 2024-05-08 21:08:24.231673 pyluba-0.0.4/pyluba/proto/mctrl_driver.proto
+-rw-r--r--   0        0        0     1347 2024-05-08 21:10:04.558292 pyluba-0.0.4/pyluba/proto/mctrl_driver_p2p.py
+-rw-r--r--   0        0        0     2024 2024-05-06 21:49:09.712665 pyluba-0.0.4/pyluba/proto/mctrl_driver_pb2.py
+-rw-r--r--   0        0        0     9943 2024-05-12 21:44:30.955843 pyluba-0.0.4/pyluba/proto/mctrl_nav.proto
+-rw-r--r--   0        0        0    15703 2024-05-13 20:02:00.650601 pyluba-0.0.4/pyluba/proto/mctrl_nav_p2p.py
+-rw-r--r--   0        0        0    19003 2024-05-12 22:27:53.181170 pyluba-0.0.4/pyluba/proto/mctrl_nav_pb2.py
+-rw-r--r--   0        0        0      682 2024-05-13 20:58:20.824741 pyluba-0.0.4/pyluba/proto/mctrl_ota.proto
+-rw-r--r--   0        0        0     2370 2024-05-13 20:59:13.504552 pyluba-0.0.4/pyluba/proto/mctrl_ota_pb2.py
+-rw-r--r--   0        0        0     8857 2024-05-13 21:29:49.796694 pyluba-0.0.4/pyluba/proto/mctrl_sys.proto
+-rw-r--r--   0        0        0    13657 2024-05-08 21:10:56.506338 pyluba-0.0.4/pyluba/proto/mctrl_sys_p2p.py
+-rw-r--r--   0        0        0    18942 2024-05-13 21:30:02.817702 pyluba-0.0.4/pyluba/proto/mctrl_sys_pb2.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.4/pyluba/py.typed
+-rw-r--r--   0        0        0     5306 2024-05-13 23:09:11.573598 pyluba-0.0.4/pyluba/utility/constant/device_constant.py
+-rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.4/pyluba/utility/periodic.py
+-rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.4/pyluba/utility/rocker_util.py
+-rw-r--r--   0        0        0     1473 2024-05-14 09:31:01.350074 pyluba-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 pyluba-0.0.4/PKG-INFO
```

### Comparing `pyluba-0.0.2/LICENSE` & `pyluba-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/README.md` & `pyluba-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 [url_pyversions]: https://pypi.python.org/pypi/pyluba
 
 # PyLuba API
 
 API to control Luba via MQTT, Cloud and bluetooth.
 
 See wiki for progress and issues for ways you can help in the effort.
+
+protobuf and protobuf models are generated using protobuf_to_pydantic and protoc
```

### Comparing `pyluba-0.0.2/pyluba/__init__.py` & `pyluba-0.0.4/pyluba/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # __init__.py
 
 # version of Luba API
 # TODO export the three interface types
-__version__ = "0.0.1"
+__version__ = "0.0.4"
 
+# works outside HA on its own
 from pyluba.bluetooth.ble import (
     LubaBLE
 )
 
+# TODO make a working device that will work outside HA too.
+from pyluba.mammotion.devices import (
+    MammotionBaseBLEDevice
+)
+
 from pyluba.mqtt.mqtt import (
     LubaMQTT
 )
 
 from pyluba.http.http import (
     LubaHTTP,
     connect_http
```

### Comparing `pyluba-0.0.2/pyluba/aliyun/cloud_gateway.py` & `pyluba-0.0.4/pyluba/aliyun/cloud_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/aliyun/cloud_service.py` & `pyluba-0.0.4/pyluba/aliyun/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/aliyun/test_alicloud_api_gateway.py` & `pyluba-0.0.4/pyluba/aliyun/test_alicloud_api_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/aliyun/tmp_constant.py` & `pyluba-0.0.4/pyluba/aliyun/tmp_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/bluetooth/ble_message.py` & `pyluba-0.0.4/pyluba/bluetooth/ble_message.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import queue
 import sys
 import time
 from typing import Dict
 
 from bleak import BleakClient
 from jsonic import serialize
-from pyluba.bluetooth.data.convert import parseCustomData
+from pyluba.bluetooth.data.convert import parse_custom_data
 
 from pyluba.bluetooth.data.framectrldata import FrameCtrlData
-from pyluba.proto import mctrl_driver_pb2, luba_msg_pb2, esp_driver_pb2, mctrl_nav_pb2, mctrl_sys_pb2
+from pyluba.proto import mctrl_driver_pb2, luba_msg_pb2, dev_net_pb2, mctrl_nav_pb2, mctrl_sys_pb2, mctrl_ota_pb2
 from pyluba.utility.constant.device_constant import bleOrderCmd
 from pyluba.aliyun.tmp_constant import tmp_constant
 
 from pyluba.data.model.execute_boarder import ExecuteBorder
 from pyluba.bluetooth.data.notifydata import BlufiNotifyData
 from pyluba.utility.rocker_util import RockerControlUtil
 from pyluba.bluetooth.const import UUID_WRITE_CHARACTERISTIC
@@ -29,22 +29,14 @@
     DEFAULT_PACKAGE_LENGTH = 20
     DH_G = "2"
     DH_P = "cf5cf5c38419a724957ff5dd323b9c45c3cdd261eb740f69aa94b8bb1a5c96409153bd76b24222d03274e4725a5406092e9e82e9135c643cae98132b0d95f7d65347c68afc1e677da90e51bbab5f5cf429c291b4ba39c6b2dc5e8c7231e46aa7728e87664532cdf547be20c9a3fa8342be6e34371a27c06f7dc0edddd2f86373"
     MIN_PACKAGE_LENGTH = 20
     NEG_SECURITY_SET_ALL_DATA = 1
     NEG_SECURITY_SET_TOTAL_LENGTH = 0
     PACKAGE_HEADER_LENGTH = 4
-    # TAG = "BlufiClientImpl"
-    # BluetoothDevice mDevice
-    # BluetoothGatt mGatt
-    # BluetoothGattCharacteristic mNotifyChar
-    # BlufiNotifyData mNotifyData
-    # BlufiCallback mUserBlufiCallback
-    # BluetoothGattCallback mUserGattCallback
-    # BluetoothGattCharacteristic mWriteChar
     mPrintDebug = False
     mWriteTimeout = -1
     mPackageLengthLimit = -1
     mBlufiMTU = -1
     mEncrypted = False
     mChecksum = False
     mRequireAck = False
@@ -53,67 +45,208 @@
     mReadSequence = itertools.count()
     mAck = queue.Queue()
     notification = BlufiNotifyData()
 
     def __init__(self, client: BleakClient):
         self.client = client
 
-    async def all_powerful_RW(self, i: int, i2: int, i3: int):
-        mctrl_sys = mctrl_sys_pb2.MctlSys()
+    async def all_powerful_RW(self, id: int, context: int, rw: int):
+        mctrl_sys = mctrl_sys_pb2.MctlSys(
+            bidire_comm_cmd=mctrl_sys_pb2.SysCommCmd(
+                rw=rw,
+                id=id,
+                context=context,
+            )
+        )
 
-        reqIdReq = mctrl_sys_pb2.SysCommCmd()
-        reqIdReq.id = i
-        reqIdReq.context = i2
-        reqIdReq.rw = i3
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_EMBED_SYS
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
         lubaMsg.rcver = luba_msg_pb2.DEV_MAINCTL
         lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
         lubaMsg.seqs = 1
         lubaMsg.version = 1
         lubaMsg.subtype = 1
         lubaMsg.sys.CopyFrom(mctrl_sys)
         byte_arr = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
+
+    async def send_order_msg_ota(self, type: int):
+        mctrl_ota = mctrl_ota_pb2.MctrlOta(
+            to_dev_get_info_req=mctrl_ota_pb2.ToDevGetInfoReq(
+                type=type
+            )
+        )
+
+        lubaMsg = luba_msg_pb2.LubaMsg()
+        lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_EMBED_OTA
+        lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
+        lubaMsg.rcver = luba_msg_pb2.DEV_MAINCTL
+        lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
+        lubaMsg.seqs = 1
+        lubaMsg.version = 1
+        lubaMsg.subtype = 1
+        lubaMsg.ota.CopyFrom(mctrl_ota)
+        byte_arr = lubaMsg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
+
+    async def get_report_cfg(self, timeout: int, period: int, no_change_period: int):
+
+
+        mctlsys = mctrl_sys_pb2.MctlSys(
+            todev_report_cfg=mctrl_sys_pb2.ReportInfoCfg(
+                timeout=timeout,
+                period=period,
+                no_change_period=no_change_period,
+                count=1
+            )
+        )
+
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_CONNECT
+        )
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_RTK
+        )
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_DEV_LOCAL
+        )
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_WORK
+        )
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_DEV_STA
+        )
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_VISION_POINT
+        )
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_VIO
+        )
+        mctlsys.todev_report_cfg.sub.append(
+            mctrl_sys_pb2.RptInfoType.RIT_VISION_STATISTIC
+        )
+
+        lubaMsg = luba_msg_pb2.LubaMsg()
+        lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_EMBED_SYS
+        lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
+        lubaMsg.rcver = luba_msg_pb2.DEV_MAINCTL
+        lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
+        lubaMsg.seqs = 1
+        lubaMsg.version = 1
+        lubaMsg.subtype = 1
+        lubaMsg.sys.CopyFrom(mctlsys)
+        byte_arr = lubaMsg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
+    async def get_device_base_info(self):
+        commEsp = dev_net_pb2.DevNet(
+            todev_devinfo_req=dev_net_pb2.DrvDevInfoReq()
+        )
+
+        commEsp.todev_devinfo_req.req_ids.add(
+            id=1,
+            type=6
+        )
+
+        lubaMsg = luba_msg_pb2.LubaMsg()
+        lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_ESP
+        lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
+        lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
+        lubaMsg.seqs = 1
+        lubaMsg.version = 1
+        lubaMsg.subtype = 1
+        lubaMsg.net.CopyFrom(commEsp)
+        byte_arr = lubaMsg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
     async def get_device_version_main(self):
-        commEsp = esp_driver_pb2.CommEsp(
-            todev_devinfo_req=esp_driver_pb2.DrvDevInfoReq()
+        commEsp = dev_net_pb2.DevNet(
+            todev_devinfo_req=dev_net_pb2.DrvDevInfoReq()
         )
 
+        for i in range(1, 8):
+            if (i == 1):
+                commEsp.todev_devinfo_req.req_ids.add(
+                    id=i,
+                    type=6
+                )
+            commEsp.todev_devinfo_req.req_ids.add(
+            id=i,
+            type=3
+            )
+
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_ESP
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
-        lubaMsg.rcver = luba_msg_pb2.DEV_COMM_ESP
         lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
         lubaMsg.seqs = 1
         lubaMsg.version = 1
         lubaMsg.subtype = 1
-        lubaMsg.esp.CopyFrom(commEsp)
+        lubaMsg.net.CopyFrom(commEsp)
         byte_arr = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def send_todev_ble_sync(self, sync_type: int):
-        commEsp = esp_driver_pb2.CommEsp(
-            todev_ble_sync=1
+        commEsp = dev_net_pb2.DevNet(
+            todev_ble_sync=sync_type
         )
 
-        commEsp.todev_ble_sync = sync_type
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_ESP
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
-        lubaMsg.rcver = luba_msg_pb2.DEV_COMM_ESP
+        lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
         lubaMsg.seqs = 1
         lubaMsg.version = 1
         lubaMsg.subtype = 1
-        lubaMsg.esp.CopyFrom(commEsp)
+        lubaMsg.net.CopyFrom(commEsp)
         byte_arr = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
+    async def set_data_synchronization(self, type: int):
+        mctrl_nav = mctrl_nav_pb2.MctlNav(
+                todev_get_commondata=mctrl_nav_pb2.NavGetCommData(
+                    pver=1,
+                    action=12,
+                    type=type
+                )
+        )
+
+        lubaMsg = luba_msg_pb2.LubaMsg()
+        lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_NAV
+        lubaMsg.sender = luba_msg_pb2.DEV_MAINCTL
+        lubaMsg.rcver = luba_msg_pb2.MSG_ATTR_REQ
+        lubaMsg.seqs = 1
+        lubaMsg.version = 1
+        lubaMsg.subtype = 1
+        lubaMsg.nav.CopyFrom(mctrl_nav)
+        byte_arr = lubaMsg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
+    async def get_hash(self):
+        luba_msg = luba_msg_pb2.LubaMsg(
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_NONE,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_gethash=mctrl_nav_pb2.NavGetHashList(
+                    pver=1,
+                )
+            )
+        )
+
+        byte_arr = luba_msg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
     async def get_all_boundary_hash_list(self, i: int):
         """.getAllBoundaryHashList(3); 0"""
         luba_msg = luba_msg_pb2.LubaMsg(
             msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
             sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
             rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
             msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_NONE,
@@ -160,38 +293,65 @@
             seqs=1,
             version=1,
             subtype=1,
             nav=mctrl_nav_pb2.MctlNav(
                 todev_gethash=mctrl_nav_pb2.NavGetHashList(
                     pver=1,
                     subCmd=2,
+                    action=8,
+                    type=3,
                     currentFrame=currentFrame,
                     totalFrame=totalFrame
                 )
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-    async def synchronize_hash_data(self, l: int):
+    async def get_area_tobe_transferred(self):
+        commondata = mctrl_nav_pb2.NavGetCommData(
+            pver=1,
+            subCmd=1,
+            action=8,
+            type=3
+        )
+
         luba_msg = luba_msg_pb2.LubaMsg(
             msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
             sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
             rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
             msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
             seqs=1,
             version=1,
             subtype=1,
             nav=mctrl_nav_pb2.MctlNav(
-                todev_get_commondata=mctrl_nav_pb2.NavGetCommData(
+                todev_get_commondata=commondata
+            )
+        )
+        byte_arr = luba_msg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
+    async def synchronize_hash_data(self, hash_int: int):
+        commondata = mctrl_nav_pb2.NavGetCommData(
                     pver=1,
+                    subCmd=1,
                     action=8,
-                    Hash=l,
-                    subCmd=1
+                    Hash=hash_int
                 )
+
+        luba_msg = luba_msg_pb2.LubaMsg(
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_get_commondata=commondata
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def get_task(self):
         hash_map = {"pver": 1, "subCmd": 2, "result": 0}
@@ -238,14 +398,32 @@
                 )
             )
         )
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
+    async def read_plan(self, i: int):
+        luba_msg = luba_msg_pb2.LubaMsg(
+            msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
+            sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
+            rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
+            seqs=1,
+            version=1,
+            subtype=1,
+            nav=mctrl_nav_pb2.MctlNav(
+                todev_planjob_set=mctrl_nav_pb2.NavPlanJobSet(
+                    subCmd=i,
+                )
+            )
+        )
+        byte_arr = luba_msg.SerializeToString()
+        await self.postCustomDataBytes(byte_arr)
+
     # (2, 0);
     async def read_plan(self, i: int, i2: int):
         luba_msg = luba_msg_pb2.LubaMsg(
             msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_NAV,
             sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
             rcver=luba_msg_pb2.MsgDevice.DEV_MAINCTL,
             msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
@@ -275,15 +453,15 @@
         luba_msg.version = 1
         luba_msg.subtype = 1
         luba_msg.nav.todev_unable_time_set.CopyFrom(build)
 
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
-    async def sendPlan2(self, plan: Plan):
+    async def send_plan2(self, plan: Plan):
         navPlanJobSet = luba_msg_pb2.NavPlanJobSet()
         navPlanJobSet.pver = plan.pver
         navPlanJobSet.subCmd = plan.subCmd
         navPlanJobSet.area = plan.area
         navPlanJobSet.deviceId = plan.deviceId
         navPlanJobSet.workTime = plan.workTime
         navPlanJobSet.version = plan.version
@@ -431,29 +609,30 @@
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     def clearNotification(self):
         self.notification = None
         self.notification = BlufiNotifyData()
 
-    async def get_device_info(self):
-        await self.postCustomData(self.getJsonString(bleOrderCmd.getDeviceInfo))
+    # async def get_device_info(self):
+    #     await self.postCustomData(self.getJsonString(bleOrderCmd.getDeviceInfo))
 
     async def send_device_info(self):
         """currently not called"""
         luba_msg = luba_msg_pb2.LubaMsg(
             msgtype=luba_msg_pb2.MsgCmdType.MSG_CMD_TYPE_ESP,
             sender=luba_msg_pb2.MsgDevice.DEV_MOBILEAPP,
             rcver=luba_msg_pb2.MsgDevice.DEV_COMM_ESP,
+            msgattr=luba_msg_pb2.MsgAttr.MSG_ATTR_REQ,
             seqs=1,
             version=1,
             subtype=1,
-            esp=esp_driver_pb2.CommEsp(
+            net=dev_net_pb2.DevNet(
                 todev_ble_sync=1,
-                todev_devinfo_req=esp_driver_pb2.DrvDevInfoReq()
+                todev_devinfo_req=dev_net_pb2.DrvDevInfoReq()
             )
         )
         byte_arr = luba_msg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
     async def requestDeviceStatus(self):
         request = False
@@ -515,15 +694,15 @@
         bytes = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(bytes)
 
     async def setbladeHeight(self, height: int):
         mctrlDriver = mctrl_driver_pb2.MctrlDriver()
         drvKnifeHeight = mctrl_driver_pb2.DrvKnifeHeight()
         drvKnifeHeight.knifeHeight = height
-        mctrlDriver.todev_knife_hight_set.CopyFrom(drvKnifeHeight)
+        mctrlDriver.todev_knife_height_set.CopyFrom(drvKnifeHeight)
 
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_EMBED_DRIVER
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
         lubaMsg.rcver = luba_msg_pb2.DEV_MAINCTL
         lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
         lubaMsg.seqs = 1
@@ -614,29 +793,26 @@
         if (data == None):
             return
         type_val = self.getTypeValue(1, 19)
         try:
             suc = await self.post(self.mEncrypted, self.mChecksum, self.mRequireAck, type_val, data)
             # int status = suc ? 0 : BlufiCallback.CODE_WRITE_DATA_FAILED
             # onPostCustomDataResult(status, data)
-            print(suc)
         except Exception as err:
             print(err)
 
     async def postCustomData(self, dataStr: str):
         data = dataStr.encode()
         if (data == None):
             return
         type_val = self.getTypeValue(1, 19)
         try:
             suc = await self.post(self.mEncrypted, self.mChecksum, self.mRequireAck, type_val, data)
             # int status = suc ? 0 : BlufiCallback.CODE_WRITE_DATA_FAILED
             # onPostCustomDataResult(status, data)
-            print(suc)
-            print(data)
         except Exception as err:
             print(err)
 
     def getTypeValue(self, type: int, subtype: int):
         return (subtype << 2) | type
 
     async def post(self, encrypt: bool, checksum: bool, require_ack: bool, type_of: int, data: bytearray) -> bool:
@@ -652,42 +828,39 @@
         sequence = self.generateSendSequence()
         postBytes = self.getPostBytes(type_of, encrypt, checksum, require_ack, False, sequence, None)
         posted = await self.gattWrite(postBytes)
         return posted and (not require_ack or self.receiveAck(sequence))
 
     async def postContainsData(self, encrypt: bool, checksum: bool, require_ack: bool, type_of: int,
                                data: bytearray) -> bool:
-        print("post contains data")
-        print(data)
-        chunk_size = 200  # self.client.mtu_size - 3
+        chunk_size = 517  # self.client.mtu_size - 3
 
         chunks = list()
         for i in range(0, len(data), chunk_size):
             if (i + chunk_size > len(data)):
                 chunks.append(data[i: len(data)])
             else:
                 chunks.append(data[i: i + chunk_size])
         for index, chunk in enumerate(chunks):
-            print("entered for loop")
             # frag = i < len(data)
             frag = index != len(chunks) - 1
             sequence = self.generateSendSequence()
             postBytes = self.getPostBytes(type_of, encrypt, checksum, require_ack, frag, sequence, chunk)
 
             posted = await self.gattWrite(postBytes)
             if (posted != None):
                 return False
 
             if (not frag):
-                print("not frag")
                 return not require_ack or self.receiveAck(sequence)
 
             if (require_ack and not self.receiveAck(sequence)):
                 return False
             else:
+                print("sleeping 0.01")
                 await sleep(0.01)
 
     def getPostBytes(self, type: int, encrypt: bool, checksum: bool, require_ack: bool, hasFrag: bool, sequence: int,
                      data: bytearray) -> bytearray:
 
         byteOS = BytesIO()
         dataLength = (0 if data == None else len(data))
@@ -727,28 +900,28 @@
             pkt_type = int(response[0])  # toInt
             pkgType = self._getPackageType(pkt_type)
             subType = self._getSubType(pkt_type)
             self.notification.setType(pkt_type)
             self.notification.setPkgType(pkgType)
             self.notification.setSubType(subType)
             frameCtrl = int(response[1])  # toInt
-            print("frame ctrl")
-            print(frameCtrl)
-            print(response)
-            print(f"pktType {pkt_type} pkgType {pkgType} subType {subType}")
+            # print("frame ctrl")
+            # print(frameCtrl)
+            # print(response)
+            # print(f"pktType {pkt_type} pkgType {pkgType} subType {subType}")
             self.notification.setFrameCtrl(frameCtrl)
             frameCtrlData = FrameCtrlData(frameCtrl)
             dataLen = int(response[3])  # toInt specifies length of data
             dataBytes = None
 
             try:
 
                 dataBytes = response[4: 4 + dataLen]
                 if (frameCtrlData.isEncrypted()):
-                    print("is encypted")
+                    print("is encrypted")
                 #     BlufiAES aes = new BlufiAES(self.mAESKey, AES_TRANSFORMATION, generateAESIV(sequence));
                 #     dataBytes = aes.decrypt(dataBytes);
                 # }
                 if (frameCtrlData.isChecksum()):
                     print("checksum")
                 #     int respChecksum1 = toInt(response[response.length - 1]);
                 #     int respChecksum2 = toInt(response[response.length - 2]);
@@ -775,41 +948,35 @@
             except Exception as e:
                 print(e)
                 return -100
 
         # Log.w(TAG, "parseNotification data length less than 4");
         return -2
 
-    def parseBlufiNotifyData(self):
+    async def parseBlufiNotifyData(self):
         pkgType = self.notification.getPkgType()
         subType = self.notification.getSubType()
         dataBytes = self.notification.getDataArray()
-        print("parseBlufi")
-        # print(dataBytes)
-        # if (self.mUserBlufiCallback is not None):
-        #     complete = self.mUserBlufiCallback.onGattNotification(self.mClient, pkgType, subType, dataBytes)
-        #     if (complete):
-        #         return
-
         if (pkgType == 0):
+            # never seem to get these..
+            print("control data")
             self._parseCtrlData(subType, dataBytes)
         if (pkgType == 1):
-            self._parseDataData(subType, dataBytes)
+            return await self._parseDataData(subType, dataBytes)
 
     def _parseCtrlData(self, subType: int, data: bytearray):
         pass
         # self._parseAck(data)
 
-    def _parseDataData(self, subType: int, data: bytearray):
+    async def _parseDataData(self, subType: int, data: bytearray):
         #     if (subType == 0) {
         #         this.mSecurityCallback.onReceiveDevicePublicKey(data);
         #         return;
         #     }
         print(subType)
-        print(bytearray)
         match subType:
             #         case 15:
             #             parseWifiState(data);
             #             return;
             #         case 16:
             #             parseVersion(data);
             #             return;
@@ -818,22 +985,21 @@
             #             return;
             #         case 18:
             #             int errCode = data.length > 0 ? 255 & data[0] : 255;
             #             onError(errCode);
             #             return;
             case 19:
                 #             # com/agilexrobotics/utils/EspBleUtil$BlufiCallbackMain.smali
-                parseCustomData(data)  # parse to protobuf message
-
-    # onReceiveCustomData
-    #             return;
-    #         default:
-    #             return;
-    #     }
-    # }
+                luba_msg = parse_custom_data(data)  # parse to protobuf message
+                # really need some sort of callback
+                if luba_msg.HasField('net'):
+                    if luba_msg.net.HasField('toapp_wifi_iot_status'):
+                        # await sleep(1.5)
+                        await self.send_todev_ble_sync(2)
+                return luba_msg
 
     # private void parseCtrlData(int i, byte[] bArr) {
     #     if (i == 0) {
     #         parseAck(bArr);
     #     }
     # }
 
@@ -882,8 +1048,8 @@
     def _getTypeValue(self, type: int, subtype: int):
         return (subtype << 2) | type
 
     def _getPackageType(self, typeValue: int):
         return typeValue & 3
 
     def _getSubType(self, typeValue: int):
-        return (typeValue & 252) >> 2
+        return (typeValue & 252) >> 2
```

### Comparing `pyluba-0.0.2/pyluba/bluetooth/const.py` & `pyluba-0.0.4/pyluba/bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/bluetooth/data/convert.py` & `pyluba-0.0.4/pyluba/bluetooth/data/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import asyncio
 from typing import Dict
 
 from google.protobuf.message import DecodeError
-from pyluba.proto import mctrl_driver_pb2, luba_msg_pb2, esp_driver_pb2, mctrl_nav_pb2, mctrl_sys_pb2
+
+from pyluba.proto import mctrl_driver_pb2, luba_msg_pb2, dev_net_pb2, mctrl_nav_pb2, mctrl_sys_pb2
+from pyluba.proto import luba_msg_p2p
 from pyluba.data.model import HashList, RegionData
 
 # until we have a proper store or send messages somewhere
 device_charge_map: Dict[str, int] = {}
 deviceRtkStatusMap: Dict[str, int] = {}
 deviceSelfCheckFlagMap: Dict[str, bool] = {}
 devicePileMap: Dict[str, int] = {}
@@ -16,39 +19,44 @@
 
 
 '''Parse data packets back into their protobuf types.
 
 TODO allow for registering events to individual messages
 as trying to register for all would be a mess
 '''
-def parseCustomData(data: bytearray):
-    # pass
-    # print(data)
-    # setReceiveDeviceData
-    
-    
-    
+def parse_custom_data(data: bytearray):
     luba_msg = luba_msg_pb2.LubaMsg()
     try:
         luba_msg.ParseFromString(data)
-        print(luba_msg)
+        # print(luba_msg)
+        # luba_message = luba_msg_p2p.LubaMsg(net=luba_msg.net)
+
+        # print(luba_message)
         
         # toappGetHashAck = luba_msg.nav.toapp_get_commondata_ack
         # print(toappGetHashAck.Hash)
         
-        if(luba_msg.HasField('sys')):
+        if luba_msg.HasField('sys'):
             store_sys_data(luba_msg.sys)
-        elif(luba_msg.HasField('esp')):
-            store_esp_data(luba_msg.esp)
-        elif(luba_msg.HasField('nav')):
+        elif luba_msg.HasField('net'):
+            if luba_msg.net.HasField('todev_ble_sync'):
+                pass
+                # await asyncio.sleep(1.5)
+                # await bleClient.send_todev_ble_sync(1)
+
+
+            store_net_data(luba_msg.net)
+        elif luba_msg.HasField('nav'):
             store_nav_data(luba_msg.nav)
-        elif(luba_msg.HasField('driver')):
+        elif luba_msg.HasField('driver'):
             pass
         else:
             pass
+
+        return luba_msg
         
     except DecodeError as err:
         print(err)
         
         
 def store_sys_data(sys):
     if(sys.HasField("system_tard_state_tunnel")):
@@ -89,24 +97,26 @@
         region_data.dataLen = toapp_get_commondata_ack.dataLen
         region_data.pver = toapp_get_commondata_ack.pver
         print(region_data)
 
     
     if(nav.HasField('toapp_gethash_ack')):
         toapp_gethash_ack = nav.toapp_gethash_ack
-        # luba.nav.toapp_get_commondata_ack.DESCRIPTOR.fields_by_name
         hash_list = HashList()
 
         data_couple_list = toapp_gethash_ack.dataCouple
         hash_list.pver = toapp_gethash_ack.pver
         hash_list.subCmd = toapp_gethash_ack.subCmd
         hash_list.currentFrame = toapp_gethash_ack.currentFrame
         hash_list.totalFrame = toapp_gethash_ack.totalFrame
         hash_list.dataHash = int(toapp_gethash_ack.dataHash)
         hash_list.path = data_couple_list
         print(hash_list)
         # use callback to provide hash list
     
-def store_esp_data(esp):
-    if esp.toapp_wifi_iot_status:
-        iot_status = esp.toapp_wifi_iot_status
+def store_net_data(net):
+    if net.toapp_wifi_iot_status:
+        iot_status = net.toapp_wifi_iot_status
         print(iot_status.devicename)
+    if net.todev_ble_sync:
+        pass
+        # send event to reply with sync
```

### Comparing `pyluba-0.0.2/pyluba/bluetooth/data/framectrldata.py` & `pyluba-0.0.4/pyluba/bluetooth/data/framectrldata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/bluetooth/data/notifydata.py` & `pyluba-0.0.4/pyluba/bluetooth/data/notifydata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/model/excute_boarder_params.py` & `pyluba-0.0.4/pyluba/data/model/excute_boarder_params.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/model/execute_boarder.py` & `pyluba-0.0.4/pyluba/data/model/execute_boarder.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/model/generate_route_information.py` & `pyluba-0.0.4/pyluba/data/model/generate_route_information.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/model/plan.py` & `pyluba-0.0.4/pyluba/data/model/plan.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/model/rapid_state.py` & `pyluba-0.0.4/pyluba/data/model/rapid_state.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/model/region_data.py` & `pyluba-0.0.4/pyluba/data/model/region_data.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/mqtt/event.py` & `pyluba-0.0.4/pyluba/data/mqtt/event.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/mqtt/properties.py` & `pyluba-0.0.4/pyluba/data/mqtt/properties.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/data/mqtt/status.py` & `pyluba-0.0.4/pyluba/data/mqtt/status.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/event/event.py` & `pyluba-0.0.4/pyluba/event/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,51 @@
+import asyncio
+
+
 class Event(object):
  
     def __init__(self):
         self.__eventhandlers = []
  
     def __iadd__(self, handler):
         self.__eventhandlers.append(handler)
         return self
  
     def __isub__(self, handler):
         self.__eventhandlers.remove(handler)
         return self
  
-    def __call__(self, *args, **keywargs):
-        for eventhandler in self.__eventhandlers:
-            eventhandler(*args, **keywargs)
+    async def __call__(self, *args, **kwargs):
+        await asyncio.gather(*[handler(*args, **kwargs) for handler in self.__eventhandlers])
 
 
 class MoveEvent(object):
          
     def __init__(self):
         self.OnMoveFinished = Event()
          
-    def MoveFinished(self):
+    async def MoveFinished(self):
         # This function will be executed once blufi finishes after a movement command and will
         # raise an event
-        self.OnMoveFinished()
+        await self.OnMoveFinished()
          
     def AddSubscribersForMoveFinishedEvent(self,objMethod):
         self.OnMoveFinished += objMethod
          
     def RemoveSubscribersForMoveFinishedEvent(self,objMethod):
         self.OnMoveFinished -= objMethod
 
 
 class BleNotificationEvent(object):
          
     def __init__(self):
         self.OnBleNotification = Event()
          
-    def BleNotification(self, data: bytearray):
+    async def BleNotification(self, data: bytearray):
         # This function will be executed when data is received.
-        self.OnBleNotification(data)
+        await self.OnBleNotification(data)
          
     def AddSubscribersForBleNotificationEvent(self,objMethod):
         self.OnBleNotification += objMethod
          
     def RemoveSubscribersForBleNotificationEvent(self,objMethod):
         self.OnBleNotification -= objMethod
```

### Comparing `pyluba-0.0.2/pyluba/http/http.py` & `pyluba-0.0.4/pyluba/http/http.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/luba/base.py` & `pyluba-0.0.4/pyluba/luba/base.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/mqtt/mqtt.py` & `pyluba-0.0.4/pyluba/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/proto/common_pb2.py` & `pyluba-0.0.4/pyluba/proto/common_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: common.proto
+# source: pyluba/proto/common.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\"&\n\x0e\x43ommDataCouple\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19pyluba/proto/common.proto\"&\n\x0e\x43ommDataCouple\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _globals['_COMMDATACOUPLE']._serialized_start=16
-  _globals['_COMMDATACOUPLE']._serialized_end=54
+  _COMMDATACOUPLE._serialized_start=29
+  _COMMDATACOUPLE._serialized_end=67
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.2/pyluba/proto/esp_driver.proto` & `pyluba-0.0.4/pyluba/proto/dev_net.proto`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,44 @@
 enum DrvDevInfoResult {
   DRV_RESULT_FAIL = 0;
   DRV_RESULT_SUC = 1;
   DRV_RESULT_NOTSUP = 2;
 }
 
 
-message CommEsp {
-    oneof EspSubType {
+message DevNet {
+    oneof NetSubType {
         int32 todev_ble_sync = 1;
         int32 todev_ConfType = 2;
         DrvWifiUpload todev_wifimsgupload = 3;
-        DrvWifiSet todev_wifi_configuration = 4;
-        DrvWifiSet todev_wifilistupload = 5;
-        int32 todev_req_log_info = 6;
-        DrvUploadFileCancel todev_log_data_cancel = 7;
-        DrvDevInfoReq todev_devinfo_req = 8;
-        DrvDevInfoResp toapp_devinfo_resp = 9;
-        int32 toapp_upgrade_report = 10;
-        int32 todev_uploadfile_req = 11;
-        DrvListUpload toapp_ListUpload = 12;
-        DrvWifiConf toapp_WifiConf = 13;
-        DrvWifiMsg toapp_wifimsg = 14;
-        int32 toapp_uploadfile_rsp = 15;
-        GetNetworkInfoReq todev_networkinfo_req = 16;
-        GetNetworkInfoRsp toapp_networkinfo_rsp = 17;
-        WifiIotStatusReport toapp_wifi_iot_status = 18;
+        DrvWifiSet todev_wifilistupload = 4;
+        DrvWifiSet todev_wifi_configuration = 5;
+        DrvWifiMsg toapp_wifimsg = 6;
+        DrvWifiConf toapp_WifiConf = 7;
+        DrvListUpload toapp_ListUpload = 8;
+        int32 todev_req_log_info = 9; // DrvUploadFileReq
+        DrvUploadFileCancel todev_log_data_cancel = 10;
+        DrvDevInfoReq todev_devinfo_req = 11;
+        DrvDevInfoResp toapp_devinfo_resp = 12;
+        int32 toapp_upgrade_report = 13; // DrvUpgradeReport
+        WifiIotStatusReport toapp_wifi_iot_status = 14;
+        int32 todev_uploadfile_req = 15; //DrvUploadFileToAppReq
+        int32 toapp_uploadfile_rsp = 16; //DrvUploadFileToAppRsp
+        GetNetworkInfoReq todev_networkinfo_req = 17;
+        GetNetworkInfoRsp toapp_networkinfo_rsp = 18;
+        // 19 BleTestBytes
+        // 20 GetMnetInfoReq
+        // 21 GetMnetInfoRsp
+        // 22 GetMnetCfgReq
+        // 23 GetMnetCfgRsp
+        // 24 SetMnetCfgReq
+        // 25 SetMnetCfgRsp
+        // 26 DrvDebugDdsZmq
+        // 27 SetDrvBleMTU
+
     }
 }
 
 message DrvListUpload {
     int32 current = 2;
     int32 sum = 1;
     int32 rssi = 5;
@@ -79,16 +89,16 @@
         int32 id = 1;
         int32 type = 2;
 }
 
 message DrvDevInfoRespId {
     int32 id = 1;
     int32 type = 2;
-    string info = 3;
-    int32 res = 4;
+    int32 res = 3;
+    string info = 4;
 }
 
 message DrvDevInfoReq {
     repeated DrvDevInfoReqId req_ids = 1;
 }
 
 message DrvDevInfoResp {
@@ -124,7 +134,25 @@
     int32 mask = 6;
     int32 gateway = 7;
 }
 
 message DrvUploadFileCancel {
     int32 bizId = 1;
 }
+
+message MnetInetStatus {
+  bool connect = 1;
+  int32 ip = 2;
+  int32 mask = 3;
+  int32 gateway = 4;
+}
+
+message MnetInfo {
+  string model = 1;
+  string revision = 2;
+  string imei = 3;
+  int32 sim = 4;
+  string imsi = 5;
+  int32 link_type = 6;
+  int32 rssi = 7;
+  MnetInetStatus inet = 8;
+}
```

### Comparing `pyluba-0.0.2/pyluba/proto/luba_msg.proto` & `pyluba-0.0.4/pyluba/proto/luba_msg.proto`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 syntax = "proto3";
 
 
-import "mctrl_driver.proto";
-import "mctrl_nav.proto";
-import "mctrl_sys.proto";
-import "esp_driver.proto";
+import "pyluba/proto/mctrl_driver.proto";
+import "pyluba/proto/mctrl_nav.proto";
+import "pyluba/proto/mctrl_sys.proto";
+import "pyluba/proto/dev_net.proto";
+import "pyluba/proto/mctrl_ota.proto";
 
 
 message MsgNull {
 } 
 
 message LubaMsg {
 
@@ -19,18 +20,19 @@
   int32 seqs = 5;
   int32 version = 6;
   int32 subtype = 7;
   int64 timestamp = 15;
   
   
   oneof LubaSubMsg {
-    CommEsp esp = 8;
+    DevNet net = 8;
     MctlSys sys = 10;
     MctlNav nav = 11;
     MctrlDriver driver = 12;
+    MctrlOta ota = 13;
     MsgNull null = 14;
   }
 
 }
 
 enum MsgCmdType {
   MSG_CMD_TYPE_START = 0;
```

### Comparing `pyluba-0.0.2/pyluba/proto/luba_msg_pb2.py` & `pyluba-0.0.4/pyluba/proto/luba_msg_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: luba_msg.proto
+# source: pyluba/proto/luba_msg.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import pyluba.proto.mctrl_driver_pb2 as mctrl__driver__pb2
-import pyluba.proto.mctrl_nav_pb2 as mctrl__nav__pb2
-import pyluba.proto.mctrl_sys_pb2 as mctrl__sys__pb2
-import pyluba.proto.esp_driver_pb2 as esp__driver__pb2
+from pyluba.proto import mctrl_driver_pb2 as pyluba_dot_proto_dot_mctrl__driver__pb2
+from pyluba.proto import mctrl_nav_pb2 as pyluba_dot_proto_dot_mctrl__nav__pb2
+from pyluba.proto import mctrl_sys_pb2 as pyluba_dot_proto_dot_mctrl__sys__pb2
+from pyluba.proto import dev_net_pb2 as pyluba_dot_proto_dot_dev__net__pb2
+from pyluba.proto import mctrl_ota_pb2 as pyluba_dot_proto_dot_mctrl__ota__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eluba_msg.proto\x1a\x12mctrl_driver.proto\x1a\x0fmctrl_nav.proto\x1a\x0fmctrl_sys.proto\x1a\x10\x65sp_driver.proto\"\t\n\x07MsgNull\"\xcf\x02\n\x07LubaMsg\x12\x1c\n\x07msgtype\x18\x01 \x01(\x0e\x32\x0b.MsgCmdType\x12\x1a\n\x06sender\x18\x02 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x05rcver\x18\x03 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x07msgattr\x18\x04 \x01(\x0e\x32\x08.MsgAttr\x12\x0c\n\x04seqs\x18\x05 \x01(\x05\x12\x0f\n\x07version\x18\x06 \x01(\x05\x12\x0f\n\x07subtype\x18\x07 \x01(\x05\x12\x11\n\ttimestamp\x18\x0f \x01(\x03\x12\x17\n\x03\x65sp\x18\x08 \x01(\x0b\x32\x08.CommEspH\x00\x12\x17\n\x03sys\x18\n \x01(\x0b\x32\x08.MctlSysH\x00\x12\x17\n\x03nav\x18\x0b \x01(\x0b\x32\x08.MctlNavH\x00\x12\x1e\n\x06\x64river\x18\x0c \x01(\x0b\x32\x0c.MctrlDriverH\x00\x12\x18\n\x04null\x18\x0e \x01(\x0b\x32\x08.MsgNullH\x00\x42\x0c\n\nLubaSubMsg*\xa8\x02\n\nMsgCmdType\x12\x16\n\x12MSG_CMD_TYPE_START\x10\x00\x12\x15\n\x10MSG_CMD_TYPE_NAV\x10\xf0\x01\x12\x1e\n\x19MSG_CMD_TYPE_LOCALIZATION\x10\xf1\x01\x12\x1a\n\x15MSG_CMD_TYPE_PLANNING\x10\xf2\x01\x12\x1e\n\x19MSG_CMD_TYPE_EMBED_DRIVER\x10\xf3\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_SYS\x10\xf4\x01\x12\x1f\n\x1aMSG_CMD_TYPE_EMBED_MIDWARE\x10\xf5\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_OTA\x10\xf6\x01\x12\x1d\n\x18MSG_CMD_TYPE_APPLICATION\x10\xf7\x01\x12\x15\n\x10MSG_CMD_TYPE_ESP\x10\xf8\x01*V\n\x07MsgAttr\x12\x11\n\rMSG_ATTR_NONE\x10\x00\x12\x13\n\x0fMSG_ATTR_REPORT\x10\x03\x12\x10\n\x0cMSG_ATTR_REQ\x10\x01\x12\x11\n\rMSG_ATTR_RESP\x10\x02*\xbe\x01\n\tMsgDevice\x12\x10\n\x0c\x44\x45V_COMM_ESP\x10\x00\x12\x13\n\x0f\x44\x45V_BASESTATION\x10\x04\x12\x0b\n\x07\x44\x45V_BMS\x10\t\x12\x11\n\rDEV_IOTSERVER\x10\x08\x12\x11\n\rDEV_LEFTMOTOR\x10\x02\x12\x0f\n\x0b\x44\x45V_MAINCTL\x10\x01\x12\x11\n\rDEV_MOBILEAPP\x10\x07\x12\x12\n\x0e\x44\x45V_RIGHTMOTOR\x10\x03\x12\x0e\n\nDEV_RTKCLI\x10\x05\x12\x0f\n\x0b\x44\x45V_USBHOST\x10\x06\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bpyluba/proto/luba_msg.proto\x1a\x1fpyluba/proto/mctrl_driver.proto\x1a\x1cpyluba/proto/mctrl_nav.proto\x1a\x1cpyluba/proto/mctrl_sys.proto\x1a\x1apyluba/proto/dev_net.proto\x1a\x1cpyluba/proto/mctrl_ota.proto\"\t\n\x07MsgNull\"\xe8\x02\n\x07LubaMsg\x12\x1c\n\x07msgtype\x18\x01 \x01(\x0e\x32\x0b.MsgCmdType\x12\x1a\n\x06sender\x18\x02 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x05rcver\x18\x03 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x07msgattr\x18\x04 \x01(\x0e\x32\x08.MsgAttr\x12\x0c\n\x04seqs\x18\x05 \x01(\x05\x12\x0f\n\x07version\x18\x06 \x01(\x05\x12\x0f\n\x07subtype\x18\x07 \x01(\x05\x12\x11\n\ttimestamp\x18\x0f \x01(\x03\x12\x16\n\x03net\x18\x08 \x01(\x0b\x32\x07.DevNetH\x00\x12\x17\n\x03sys\x18\n \x01(\x0b\x32\x08.MctlSysH\x00\x12\x17\n\x03nav\x18\x0b \x01(\x0b\x32\x08.MctlNavH\x00\x12\x1e\n\x06\x64river\x18\x0c \x01(\x0b\x32\x0c.MctrlDriverH\x00\x12\x18\n\x03ota\x18\r \x01(\x0b\x32\t.MctrlOtaH\x00\x12\x18\n\x04null\x18\x0e \x01(\x0b\x32\x08.MsgNullH\x00\x42\x0c\n\nLubaSubMsg*\xa8\x02\n\nMsgCmdType\x12\x16\n\x12MSG_CMD_TYPE_START\x10\x00\x12\x15\n\x10MSG_CMD_TYPE_NAV\x10\xf0\x01\x12\x1e\n\x19MSG_CMD_TYPE_LOCALIZATION\x10\xf1\x01\x12\x1a\n\x15MSG_CMD_TYPE_PLANNING\x10\xf2\x01\x12\x1e\n\x19MSG_CMD_TYPE_EMBED_DRIVER\x10\xf3\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_SYS\x10\xf4\x01\x12\x1f\n\x1aMSG_CMD_TYPE_EMBED_MIDWARE\x10\xf5\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_OTA\x10\xf6\x01\x12\x1d\n\x18MSG_CMD_TYPE_APPLICATION\x10\xf7\x01\x12\x15\n\x10MSG_CMD_TYPE_ESP\x10\xf8\x01*V\n\x07MsgAttr\x12\x11\n\rMSG_ATTR_NONE\x10\x00\x12\x13\n\x0fMSG_ATTR_REPORT\x10\x03\x12\x10\n\x0cMSG_ATTR_REQ\x10\x01\x12\x11\n\rMSG_ATTR_RESP\x10\x02*\xbe\x01\n\tMsgDevice\x12\x10\n\x0c\x44\x45V_COMM_ESP\x10\x00\x12\x13\n\x0f\x44\x45V_BASESTATION\x10\x04\x12\x0b\n\x07\x44\x45V_BMS\x10\t\x12\x11\n\rDEV_IOTSERVER\x10\x08\x12\x11\n\rDEV_LEFTMOTOR\x10\x02\x12\x0f\n\x0b\x44\x45V_MAINCTL\x10\x01\x12\x11\n\rDEV_MOBILEAPP\x10\x07\x12\x12\n\x0e\x44\x45V_RIGHTMOTOR\x10\x03\x12\x0e\n\nDEV_RTKCLI\x10\x05\x12\x0f\n\x0b\x44\x45V_USBHOST\x10\x06\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'luba_msg_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.luba_msg_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _globals['_MSGCMDTYPE']._serialized_start=440
-  _globals['_MSGCMDTYPE']._serialized_end=736
-  _globals['_MSGATTR']._serialized_start=738
-  _globals['_MSGATTR']._serialized_end=824
-  _globals['_MSGDEVICE']._serialized_start=827
-  _globals['_MSGDEVICE']._serialized_end=1017
-  _globals['_MSGNULL']._serialized_start=90
-  _globals['_MSGNULL']._serialized_end=99
-  _globals['_LUBAMSG']._serialized_start=102
-  _globals['_LUBAMSG']._serialized_end=437
+  _MSGCMDTYPE._serialized_start=557
+  _MSGCMDTYPE._serialized_end=853
+  _MSGATTR._serialized_start=855
+  _MSGATTR._serialized_end=941
+  _MSGDEVICE._serialized_start=944
+  _MSGDEVICE._serialized_end=1134
+  _MSGNULL._serialized_start=182
+  _MSGNULL._serialized_end=191
+  _LUBAMSG._serialized_start=194
+  _LUBAMSG._serialized_end=554
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.2/pyluba/proto/mctrl_driver.proto` & `pyluba-0.0.4/pyluba/proto/mctrl_driver.proto`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 message MctrlDriver {
 
 
     oneof SubDrvMsg {
 
         DrvMotionCtrl todev_devmotion_ctrl = 1;
-        DrvKnifeHeight todev_knife_hight_set = 2;
+        DrvKnifeHeight todev_knife_height_set = 2;
         DrvSrSpeed bidire_speed_read_set = 3;
-        DrvKnifeHeight bidire_knife_hight_report = 4;
+        DrvKnifeHeight bidire_knife_height_report = 4;
         DrvKnifeStatus toapp_knife_status = 5;
     }
 
 }
 
 
 message DrvMotionCtrl {
```

### Comparing `pyluba-0.0.2/pyluba/proto/mctrl_driver_pb2.py` & `pyluba-0.0.4/pyluba/proto/mctrl_driver_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: mctrl_driver.proto
+# source: pyluba/proto/mctrl_driver.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12mctrl_driver.proto\"\x8f\x02\n\x0bMctrlDriver\x12.\n\x14todev_devmotion_ctrl\x18\x01 \x01(\x0b\x32\x0e.DrvMotionCtrlH\x00\x12\x30\n\x15todev_knife_hight_set\x18\x02 \x01(\x0b\x32\x0f.DrvKnifeHeightH\x00\x12,\n\x15\x62idire_speed_read_set\x18\x03 \x01(\x0b\x32\x0b.DrvSrSpeedH\x00\x12\x34\n\x19\x62idire_knife_hight_report\x18\x04 \x01(\x0b\x32\x0f.DrvKnifeHeightH\x00\x12-\n\x12toapp_knife_status\x18\x05 \x01(\x0b\x32\x0f.DrvKnifeStatusH\x00\x42\x0b\n\tSubDrvMsg\"@\n\rDrvMotionCtrl\x12\x17\n\x0fsetAngularSpeed\x18\x02 \x01(\x05\x12\x16\n\x0esetLinearSpeed\x18\x01 \x01(\x05\"%\n\x0e\x44rvKnifeHeight\x12\x13\n\x0bknifeHeight\x18\x01 \x01(\x05\"\'\n\nDrvSrSpeed\x12\n\n\x02rw\x18\x01 \x01(\x05\x12\r\n\x05speed\x18\x02 \x01(\x02\"&\n\x0e\x44rvKnifeStatus\x12\x14\n\x0cknife_status\x18\x01 \x01(\x05\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fpyluba/proto/mctrl_driver.proto\"\x8f\x02\n\x0bMctrlDriver\x12.\n\x14todev_devmotion_ctrl\x18\x01 \x01(\x0b\x32\x0e.DrvMotionCtrlH\x00\x12\x30\n\x15todev_knife_hight_set\x18\x02 \x01(\x0b\x32\x0f.DrvKnifeHeightH\x00\x12,\n\x15\x62idire_speed_read_set\x18\x03 \x01(\x0b\x32\x0b.DrvSrSpeedH\x00\x12\x34\n\x19\x62idire_knife_hight_report\x18\x04 \x01(\x0b\x32\x0f.DrvKnifeHeightH\x00\x12-\n\x12toapp_knife_status\x18\x05 \x01(\x0b\x32\x0f.DrvKnifeStatusH\x00\x42\x0b\n\tSubDrvMsg\"@\n\rDrvMotionCtrl\x12\x17\n\x0fsetAngularSpeed\x18\x02 \x01(\x05\x12\x16\n\x0esetLinearSpeed\x18\x01 \x01(\x05\"%\n\x0e\x44rvKnifeHeight\x12\x13\n\x0bknifeHeight\x18\x01 \x01(\x05\"\'\n\nDrvSrSpeed\x12\n\n\x02rw\x18\x01 \x01(\x05\x12\r\n\x05speed\x18\x02 \x01(\x02\"&\n\x0e\x44rvKnifeStatus\x12\x14\n\x0cknife_status\x18\x01 \x01(\x05\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mctrl_driver_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.mctrl_driver_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _globals['_MCTRLDRIVER']._serialized_start=23
-  _globals['_MCTRLDRIVER']._serialized_end=294
-  _globals['_DRVMOTIONCTRL']._serialized_start=296
-  _globals['_DRVMOTIONCTRL']._serialized_end=360
-  _globals['_DRVKNIFEHEIGHT']._serialized_start=362
-  _globals['_DRVKNIFEHEIGHT']._serialized_end=399
-  _globals['_DRVSRSPEED']._serialized_start=401
-  _globals['_DRVSRSPEED']._serialized_end=440
-  _globals['_DRVKNIFESTATUS']._serialized_start=442
-  _globals['_DRVKNIFESTATUS']._serialized_end=480
+  _MCTRLDRIVER._serialized_start=36
+  _MCTRLDRIVER._serialized_end=307
+  _DRVMOTIONCTRL._serialized_start=309
+  _DRVMOTIONCTRL._serialized_end=373
+  _DRVKNIFEHEIGHT._serialized_start=375
+  _DRVKNIFEHEIGHT._serialized_end=412
+  _DRVSRSPEED._serialized_start=414
+  _DRVSRSPEED._serialized_end=453
+  _DRVKNIFESTATUS._serialized_start=455
+  _DRVKNIFESTATUS._serialized_end=493
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.2/pyluba/proto/mctrl_nav.proto` & `pyluba-0.0.4/pyluba/proto/mctrl_nav.proto`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 syntax = "proto3";
 
-import "common.proto";
+import "pyluba/proto/common.proto";
 
 message NavLatLonUp {
     double lat = 1;
     double lon = 2;
 }
 
 message NavBorderState {
@@ -332,14 +332,53 @@
 
 message chargePileType {
   int32 toward = 1;
   float x = 2;
   float y = 3;
 }
 
+message AppRequestCoverPaths {
+  int32 pver = 1;
+  int32 subCmd = 2;
+  int32 totalFrame = 3;
+  int32 currentFrame = 4;
+  fixed64 dataHash = 5;
+  int64 transactionId = 6;
+  repeated int64 reserved = 7;
+  repeated int64 hashList = 8;
+}
+
+message CoverPathPacket {
+  fixed64 pathHash = 1;
+  int32 pathType = 2;
+  int32 pathTotal = 3;
+  int32 pathCur = 4;
+  fixed64 zoneHash = 5;
+  repeated CommDataCouple dataCouple = 6;
+}
+
+message CoverPathUpload {
+  int32 pver = 1;
+  int32 result = 2;
+  int32 subCmd = 3;
+  int32 area = 4;
+  int32 time = 5;
+  int32 totalFrame = 6;
+  int32 currentFrame = 7;
+  int32 totalPathNum = 8;
+  int32 validPathNum = 9;
+  fixed64 dataHash = 10;
+  int64 transactionId = 11;
+  repeated int64 reserved = 12;
+  int32 dataLen = 13;
+  repeated CoverPathPacket pathPackets = 14;
+}
+
+
+
 
 message MctlNav {
     oneof SubNavMsg {
         NavLatLonUp toapp_lat_up = 1;
         NavPosUp toapp_pos_up = 2;
         NavCHlLineData todev_chl_line_data = 3;
         NavTaskInfo toapp_task_info = 4;
@@ -381,9 +420,17 @@
         NavPlanJobSet todev_planjob_set = 40;
         NavUnableTimeSet todev_unable_time_set = 41;
         SimulationCmdData simulation_cmd = 42;
         WorkReportUpdateCmd todev_work_report_update_cmd = 43;
         WorkReportUpdateAck toapp_work_report_update_ack = 44;
         WorkReportCmdData todev_work_report_cmd = 45;
         WorkReportInfoAck toapp_work_report_ack = 46;
+        WorkReportInfoAck toapp_work_report_upload = 47;
+        AppRequestCoverPaths app_request_cover_paths_t = 48;
+        CoverPathUpload cover_path_upload_t = 49;
+        // 50 zone_start_precent_t
+        // 51 vision_ctrl_msg
+        // 52 nav_sys_param_msg
+        // 53 nav_plan_task_execute
+        // 54 costmap_t
     }
 }
```

### Comparing `pyluba-0.0.2/pyluba/proto/mctrl_nav_pb2.py` & `pyluba-0.0.4/pyluba/proto/mctrl_sys_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,134 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: mctrl_nav.proto
+# source: pyluba/proto/mctrl_sys.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import pyluba.proto.common_pb2 as common__pb2
+from pyluba.proto import dev_net_pb2 as pyluba_dot_proto_dot_dev__net__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fmctrl_nav.proto\x1a\x0c\x63ommon.proto\"\'\n\x0bNavLatLonUp\x12\x0b\n\x03lat\x18\x01 \x01(\x01\x12\x0b\n\x03lon\x18\x02 \x01(\x01\"!\n\x0eNavBorderState\x12\x0f\n\x07\x62\x64state\x18\x01 \x01(\x05\"\xc9\x01\n\x08NavPosUp\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\x0e\n\x06status\x18\x03 \x01(\x05\x12\x0e\n\x06toward\x18\x04 \x01(\x05\x12\r\n\x05stars\x18\x05 \x01(\x05\x12\x0b\n\x03\x61ge\x18\x06 \x01(\x02\x12\x11\n\tlatStddev\x18\x07 \x01(\x02\x12\x11\n\tlonStddev\x18\x08 \x01(\x02\x12\x11\n\tl2dfStars\x18\t \x01(\x05\x12\x0f\n\x07posType\x18\n \x01(\x05\x12\x0f\n\x07\x63HashId\x18\x0b \x01(\x03\x12\x10\n\x08posLevel\x18\x0c \x01(\x05\":\n\x13NavBorderDataGetAck\x12\r\n\x05jobId\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\"Z\n\x15NavObstiBorderDataGet\x12\x15\n\robstacleIndex\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x14\n\x0cobstaclesLen\x18\x03 \x01(\x05\"G\n\x18NavObstiBorderDataGetAck\x12\x15\n\robstacleIndex\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\"d\n\x0eNavCHlLineData\x12\x16\n\x0e\x63hannelLineLen\x18\x04 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\"O\n\x11NavCHlLineDataAck\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\"J\n\x10NavBorderDataGet\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x11\n\tborderLen\x18\x03 \x01(\x05\x12\r\n\x05jobId\x18\x01 \x01(\x05\"\x7f\n\x0bNavTaskInfo\x12\x10\n\x08\x61llFrame\x18\x03 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x01 \x01(\x05\x12\x0c\n\x04time\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x0f\n\x07pathlen\x18\x05 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"\x91\x01\n\x0cNavOptLineUp\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x16\n\x0e\x63hannelDataLen\x18\x05 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"~\n\x11NavOptiBorderInfo\x12\r\n\x05jobId\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x15\n\rborderDataLen\x18\x04 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x05 \x03(\x0b\x32\x0f.CommDataCouple\"\x81\x01\n\rNavOptObsInfo\x12\x12\n\nobstacleId\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x17\n\x0fobstacleDataLen\x18\x04 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x05 \x03(\x0b\x32\x0f.CommDataCouple\"\xb4\x01\n\x0bNavStartJob\x12\r\n\x05jobId\x18\x01 \x01(\x03\x12\x0e\n\x06jobVer\x18\x02 \x01(\x05\x12\x0f\n\x07jobMode\x18\x03 \x01(\x05\x12\x13\n\x0brainTactics\x18\x04 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x05 \x01(\x05\x12\r\n\x05speed\x18\x06 \x01(\x02\x12\x14\n\x0c\x63hannelWidth\x18\x07 \x01(\x05\x12\x11\n\tultraWave\x18\x08 \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\t \x01(\x05\"|\n\x0eNavGetHashList\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x03\x12\x10\n\x08reserved\x18\x06 \x01(\t\"\xa4\x01\n\x11NavGetHashListAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x03\x12\x0f\n\x07hashLen\x18\x06 \x01(\x05\x12\x10\n\x08reserved\x18\x07 \x01(\t\x12\x12\n\ndataCouple\x18\r \x03(\x03\"\xd6\x01\n\x0eNavGetCommData\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\x05\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\x0c\n\x04Hash\x18\x05 \x01(\x03\x12\x15\n\rpaternalHashA\x18\x06 \x01(\x06\x12\x15\n\rpaternalHashB\x18\x07 \x01(\x06\x12\x12\n\ntotalFrame\x18\x08 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\t \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\n \x01(\x06\x12\x10\n\x08reserved\x18\x0b \x01(\t\"\x9f\x02\n\x11NavGetCommDataAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\x05\x12\x0c\n\x04type\x18\x05 \x01(\x05\x12\x0c\n\x04Hash\x18\x06 \x01(\x06\x12\x15\n\rpaternalHashA\x18\x07 \x01(\x06\x12\x15\n\rpaternalHashB\x18\x08 \x01(\x06\x12\x12\n\ntotalFrame\x18\t \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\n \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x0b \x01(\x03\x12\x0f\n\x07\x64\x61taLen\x18\x0c \x01(\x05\x12#\n\ndataCouple\x18\r \x03(\x0b\x32\x0f.CommDataCouple\x12\x10\n\x08reserved\x18\x0e \x01(\t\"\xaa\x02\n\x0fNavReqCoverPath\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\r\n\x05jobId\x18\x02 \x01(\x03\x12\x0e\n\x06jobVer\x18\x03 \x01(\x05\x12\x0f\n\x07jobMode\x18\x04 \x01(\x05\x12\x0e\n\x06subCmd\x18\x05 \x01(\x05\x12\x10\n\x08\x65\x64geMode\x18\x06 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x07 \x01(\x05\x12\x14\n\x0c\x63hannelWidth\x18\x08 \x01(\x05\x12\x11\n\tultraWave\x18\t \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\n \x01(\x05\x12\x0e\n\x06toward\x18\x0b \x01(\x05\x12\r\n\x05speed\x18\x0c \x01(\x02\x12\x11\n\tzoneHashs\x18\r \x03(\x03\x12\x10\n\x08pathHash\x18\x0e \x01(\x03\x12\x10\n\x08reserved\x18\x0f \x01(\t\x12\x0e\n\x06result\x18\x10 \x01(\x05\"\xa7\x03\n\x15NavUploadZigZagResult\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\r\n\x05jobId\x18\x02 \x01(\x03\x12\x0e\n\x06jobVer\x18\x03 \x01(\x05\x12\x0e\n\x06result\x18\x04 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x05 \x01(\x05\x12\x0c\n\x04time\x18\x06 \x01(\x05\x12\x14\n\x0ctotalZoneNum\x18\x07 \x01(\x05\x12\x1a\n\x12\x63urrentZonePathNum\x18\x08 \x01(\x05\x12\x19\n\x11\x63urrentZonePathId\x18\t \x01(\x05\x12\x13\n\x0b\x63urrentZone\x18\n \x01(\x05\x12\x13\n\x0b\x63urrentHash\x18\x0b \x01(\x03\x12\x12\n\ntotalFrame\x18\x0c \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\r \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\x0e \x01(\x05\x12\x15\n\rchannelModeId\x18\x0f \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x10 \x01(\x03\x12\x0f\n\x07\x64\x61taLen\x18\x11 \x01(\x05\x12\x10\n\x08reserved\x18\x12 \x01(\t\x12#\n\ndataCouple\x18\x13 \x03(\x0b\x32\x0f.CommDataCouple\x12\x0e\n\x06subCmd\x18\x14 \x01(\x05\"\xb0\x01\n\x18NavUploadZigZagResultAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x13\n\x0b\x63urrentZone\x18\x02 \x01(\x05\x12\x13\n\x0b\x63urrentHash\x18\x03 \x01(\x03\x12\x12\n\ntotalFrame\x18\x04 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x05 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x06 \x01(\x03\x12\x10\n\x08reserved\x18\x07 \x01(\t\x12\x0e\n\x06subCmd\x18\x08 \x01(\x05\"M\n\x0bNavTaskCtrl\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x10\n\x08reserved\x18\x04 \x01(\x05\"o\n\x0bNavTaskIdRw\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x10\n\x08taskName\x18\x03 \x01(\t\x12\x0e\n\x06taskId\x18\x04 \x01(\t\x12\x0e\n\x06result\x18\x05 \x01(\x05\x12\x10\n\x08reserved\x18\x06 \x01(\t\"J\n\x12NavSysHashOverview\x12\x1a\n\x12\x63ommonhashOverview\x18\x01 \x01(\x03\x12\x18\n\x10pathHashOverview\x18\x02 \x01(\x03\"i\n\x11NavTaskBreakPoint\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\x0e\n\x06toward\x18\x03 \x01(\x05\x12\x0c\n\x04\x66lag\x18\x04 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\x05\x12\x10\n\x08zoneHash\x18\x06 \x01(\x03\"\xa2\x04\n\rNavPlanJobSet\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x03 \x01(\x05\x12\x10\n\x08workTime\x18\x04 \x01(\x05\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\n\n\x02id\x18\x06 \x01(\t\x12\x0e\n\x06userId\x18\x07 \x01(\t\x12\x10\n\x08\x64\x65viceId\x18\x08 \x01(\t\x12\x0e\n\x06planId\x18\t \x01(\t\x12\x0e\n\x06taskId\x18\n \x01(\t\x12\r\n\x05jobId\x18\x0b \x01(\t\x12\x11\n\tstartTime\x18\x0c \x01(\t\x12\x0f\n\x07\x65ndTime\x18\r \x01(\t\x12\x0c\n\x04week\x18\x0e \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x0f \x01(\x05\x12\r\n\x05model\x18\x10 \x01(\x05\x12\x10\n\x08\x65\x64geMode\x18\x11 \x01(\x05\x12\x14\n\x0crequiredTime\x18\x12 \x01(\x05\x12\x12\n\nrouteAngle\x18\x13 \x01(\x05\x12\x12\n\nrouteModel\x18\x14 \x01(\x05\x12\x14\n\x0crouteSpacing\x18\x15 \x01(\x05\x12\x19\n\x11ultrasonicBarrier\x18\x16 \x01(\x05\x12\x14\n\x0ctotalPlanNum\x18\x17 \x01(\x05\x12\x11\n\tplanIndex\x18\x18 \x01(\x05\x12\x0e\n\x06result\x18\x19 \x01(\x05\x12\r\n\x05speed\x18\x1a \x01(\x02\x12\x10\n\x08taskName\x18\x1b \x01(\t\x12\x0f\n\x07jobName\x18\x1c \x01(\t\x12\x11\n\tzoneHashs\x18\x1d \x03(\x03\x12\x10\n\x08reserved\x18\x1e \x01(\t\"\x1e\n\x0bNavResFrame\x12\x0f\n\x07\x66rameid\x18\x01 \x01(\x05\"\'\n\x0fNavTaskProgress\x12\x14\n\x0ctaskProgress\x18\x01 \x01(\x05\"\x86\x01\n\x10NavUnableTimeSet\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x10\n\x08\x64\x65viceId\x18\x02 \x01(\t\x12\x17\n\x0funableStartTime\x18\x03 \x01(\t\x12\x15\n\runableEndTime\x18\x04 \x01(\t\x12\x0e\n\x06result\x18\x05 \x01(\x05\x12\x10\n\x08reserved\x18\x06 \x01(\t\"H\n\x11SimulationCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x0f\n\x07paramId\x18\x02 \x01(\x05\x12\x12\n\nparamValue\x18\x03 \x03(\x05\"7\n\x11WorkReportCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x12\n\ngetInfoNum\x18\x02 \x01(\x05\"\xfd\x01\n\x11WorkReportInfoAck\x12\x15\n\rcurrentAckNum\x18\x01 \x01(\x05\x12\x13\n\x0b\x65ndWorkTime\x18\x02 \x01(\x03\x12\x15\n\rheightOfKnife\x18\x03 \x01(\x05\x12\x15\n\rinterruptFlag\x18\x04 \x01(\x08\x12\x15\n\rstartWorkTime\x18\x05 \x01(\x03\x12\x13\n\x0btotalAckNum\x18\x06 \x01(\x05\x12\x10\n\x08workAres\x18\x07 \x01(\x01\x12\x14\n\x0cworkProgress\x18\x08 \x01(\x05\x12\x12\n\nworkResult\x18\t \x01(\x05\x12\x14\n\x0cworkTimeUsed\x18\n \x01(\x05\x12\x10\n\x08workType\x18\x0b \x01(\x05\":\n\x13WorkReportUpdateAck\x12\x0f\n\x07infoNum\x18\x02 \x01(\x05\x12\x12\n\nupdateFlag\x18\x01 \x01(\x08\"%\n\x13WorkReportUpdateCmd\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\"6\n\x0e\x63hargePileType\x12\x0e\n\x06toward\x18\x01 \x01(\x05\x12\t\n\x01x\x18\x02 \x01(\x02\x12\t\n\x01y\x18\x03 \x01(\x02\"\x84\x0f\n\x07MctlNav\x12$\n\x0ctoapp_lat_up\x18\x01 \x01(\x0b\x32\x0c.NavLatLonUpH\x00\x12!\n\x0ctoapp_pos_up\x18\x02 \x01(\x0b\x32\t.NavPosUpH\x00\x12.\n\x13todev_chl_line_data\x18\x03 \x01(\x0b\x32\x0f.NavCHlLineDataH\x00\x12\'\n\x0ftoapp_task_info\x18\x04 \x01(\x0b\x32\x0c.NavTaskInfoH\x00\x12*\n\x11toapp_opt_line_up\x18\x05 \x01(\x0b\x32\r.NavOptLineUpH\x00\x12\x33\n\x15toapp_opt_border_info\x18\x06 \x01(\x0b\x32\x12.NavOptiBorderInfoH\x00\x12,\n\x12toapp_opt_obs_info\x18\x07 \x01(\x0b\x32\x0e.NavOptObsInfoH\x00\x12+\n\x13todev_task_info_ack\x18\x08 \x01(\x0b\x32\x0c.NavResFrameH\x00\x12\x31\n\x19todev_opt_border_info_ack\x18\t \x01(\x0b\x32\x0c.NavResFrameH\x00\x12.\n\x16todev_opt_obs_info_ack\x18\n \x01(\x0b\x32\x0c.NavResFrameH\x00\x12-\n\x15todev_opt_line_up_ack\x18\x0b \x01(\x0b\x32\x0c.NavResFrameH\x00\x12*\n\x0ftoapp_chgpileto\x18\x0c \x01(\x0b\x32\x0f.chargePileTypeH\x00\x12\x17\n\rtodev_sustask\x18\r \x01(\x05H\x00\x12\x18\n\x0etodev_rechgcmd\x18\x0e \x01(\x05H\x00\x12\x17\n\rtodev_edgecmd\x18\x0f \x01(\x05H\x00\x12\x1b\n\x11todev_draw_border\x18\x10 \x01(\x05H\x00\x12\x1f\n\x15todev_draw_border_end\x18\x11 \x01(\x05H\x00\x12\x18\n\x0etodev_draw_obs\x18\x12 \x01(\x05H\x00\x12\x1c\n\x12todev_draw_obs_end\x18\x13 \x01(\x05H\x00\x12\x18\n\x0etodev_chl_line\x18\x14 \x01(\x05H\x00\x12\x1c\n\x12todev_chl_line_end\x18\x15 \x01(\x05H\x00\x12\x19\n\x0ftodev_save_task\x18\x16 \x01(\x05H\x00\x12\x1d\n\x13todev_cancel_suscmd\x18\x17 \x01(\x05H\x00\x12\x1e\n\x14todev_reset_chg_pile\x18\x18 \x01(\x05H\x00\x12\x1f\n\x15todev_cancel_draw_cmd\x18\x19 \x01(\x05H\x00\x12$\n\x1atodev_one_touch_leave_pile\x18\x1a \x01(\x05H\x00\x12&\n\x0etodev_mow_task\x18\x1b \x01(\x0b\x32\x0c.NavStartJobH\x00\x12\'\n\x0ctoapp_bstate\x18\x1c \x01(\x0b\x32\x0f.NavBorderStateH\x00\x12\x1a\n\x10todev_lat_up_ack\x18\x1d \x01(\x05H\x00\x12(\n\rtodev_gethash\x18\x1e \x01(\x0b\x32\x0f.NavGetHashListH\x00\x12/\n\x11toapp_gethash_ack\x18\x1f \x01(\x0b\x32\x12.NavGetHashListAckH\x00\x12/\n\x14todev_get_commondata\x18  \x01(\x0b\x32\x0f.NavGetCommDataH\x00\x12\x36\n\x18toapp_get_commondata_ack\x18! \x01(\x0b\x32\x12.NavGetCommDataAckH\x00\x12\x31\n\x15\x62idire_reqconver_path\x18\" \x01(\x0b\x32\x10.NavReqCoverPathH\x00\x12.\n\x0ctoapp_zigzag\x18# \x01(\x0b\x32\x16.NavUploadZigZagResultH\x00\x12\x35\n\x10todev_zigzag_ack\x18$ \x01(\x0b\x32\x19.NavUploadZigZagResultAckH\x00\x12&\n\x0etodev_taskctrl\x18% \x01(\x0b\x32\x0c.NavTaskCtrlH\x00\x12%\n\rbidire_taskid\x18& \x01(\x0b\x32\x0c.NavTaskIdRwH\x00\x12&\n\x08toapp_bp\x18\' \x01(\x0b\x32\x12.NavTaskBreakPointH\x00\x12+\n\x11todev_planjob_set\x18( \x01(\x0b\x32\x0e.NavPlanJobSetH\x00\x12\x32\n\x15todev_unable_time_set\x18) \x01(\x0b\x32\x11.NavUnableTimeSetH\x00\x12,\n\x0esimulation_cmd\x18* \x01(\x0b\x32\x12.SimulationCmdDataH\x00\x12<\n\x1ctodev_work_report_update_cmd\x18+ \x01(\x0b\x32\x14.WorkReportUpdateCmdH\x00\x12<\n\x1ctoapp_work_report_update_ack\x18, \x01(\x0b\x32\x14.WorkReportUpdateAckH\x00\x12\x33\n\x15todev_work_report_cmd\x18- \x01(\x0b\x32\x12.WorkReportCmdDataH\x00\x12\x33\n\x15toapp_work_report_ack\x18. \x01(\x0b\x32\x12.WorkReportInfoAckH\x00\x42\x0b\n\tSubNavMsgb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cpyluba/proto/mctrl_sys.proto\x1a\x1apyluba/proto/dev_net.proto\"\x98\x0c\n\x07MctlSys\x12\"\n\rtoapp_batinfo\x18\x01 \x01(\x0b\x32\t.SysBatUpH\x00\x12)\n\x10toapp_work_state\x18\x02 \x01(\x0b\x32\r.SysWorkStateH\x00\x12*\n\x0ftodev_time_zone\x18\x03 \x01(\x0b\x32\x0f.SysSetTimeZoneH\x00\x12*\n\x0ftodev_data_time\x18\x04 \x01(\x0b\x32\x0f.SysSetDateTimeH\x00\x12\x1f\n\x08job_plan\x18\x06 \x01(\x0b\x32\x0b.SysJobPlanH\x00\x12(\n\x0etoapp_err_code\x18\x07 \x01(\x0b\x32\x0e.SysDevErrCodeH\x00\x12.\n\x13todev_job_plan_time\x18\n \x01(\x0b\x32\x0f.SysJobPlanTimeH\x00\x12%\n\x0etoapp_mow_info\x18\x0b \x01(\x0b\x32\x0b.SysMowInfoH\x00\x12&\n\x0f\x62idire_comm_cmd\x18\x0c \x01(\x0b\x32\x0b.SysCommCmdH\x00\x12\x16\n\x0cplan_job_del\x18\x0e \x01(\x03H\x00\x12\x1c\n\x06\x62order\x18\x0f \x01(\x0b\x32\n.SysBorderH\x00\x12.\n\x11toapp_plan_status\x18\x12 \x01(\x0b\x32\x11.SysPlanJobStatusH\x00\x12\x34\n\x12toapp_ul_fprogress\x18\x13 \x01(\x0b\x32\x16.SysUploadFileProgressH\x00\x12*\n\x10todev_deljobplan\x18\x14 \x01(\x0b\x32\x0e.SysDelJobPlanH\x00\x12\x1b\n\x11todev_mow_info_up\x18\x15 \x01(\x05H\x00\x12,\n\x10todev_knife_ctrl\x18\x16 \x01(\x0b\x32\x10.SysKnifeControlH\x00\x12\x1c\n\x12todev_reset_system\x18\x17 \x01(\x05H\x00\x12:\n\x19todev_reset_system_status\x18\x18 \x01(\x0b\x32\x15.SysResetSystemStatusH\x00\x12@\n\x19system_rapid_state_tunnel\x18\x19 \x01(\x0b\x32\x1b.systemRapidStateTunnel_msgH\x00\x12>\n\x18system_tard_state_tunnel\x18\x1a \x01(\x0b\x32\x1a.systemTardStateTunnel_msgH\x00\x12\x31\n\x11system_update_buf\x18\x1b \x01(\x0b\x32\x14.systemUpdateBuf_msgH\x00\x12/\n\x15todev_time_ctrl_light\x18\x1c \x01(\x0b\x32\x0e.TimeCtrlLightH\x00\x12\x34\n\x13system_tmp_cycle_tx\x18\x1d \x01(\x0b\x32\x15.systemTmpCycleTx_msgH\x00\x12\x30\n\x14todev_off_chip_flash\x18\x1e \x01(\x0b\x32\x10.SysOffChipFlashH\x00\x12\x1f\n\x15todev_get_dev_fw_info\x18\x1f \x01(\x05H\x00\x12,\n\x11toapp_dev_fw_info\x18  \x01(\x0b\x32\x0f.device_fw_infoH\x00\x12)\n\x12todev_lora_cfg_req\x18! \x01(\x0b\x32\x0b.LoraCfgReqH\x00\x12)\n\x12toapp_lora_cfg_rsp\x18\" \x01(\x0b\x32\x0b.LoraCfgRspH\x00\x12-\n\x0fmow_to_app_info\x18# \x01(\x0b\x32\x12.mow_to_app_info_tH\x00\x12:\n\x18\x64\x65vice_product_type_info\x18$ \x01(\x0b\x32\x16.DeviceProductTypeInfoH\x00\x12\x37\n\x17mow_to_app_qctools_info\x18% \x01(\x0b\x32\x14.MowToAppQCToolsInfoH\x00\x12*\n\x10todev_report_cfg\x18& \x01(\x0b\x32\x0e.ReportInfoCfgH\x00\x12,\n\x11toapp_report_data\x18\' \x01(\x0b\x32\x0f.ReportInfoDataH\x00\x12\x31\n\x0esimulation_cmd\x18* \x01(\x0b\x32\x17.MCtrlSimulationCmdDataH\x00\x42\x0b\n\tsubSysMsg\"M\n\x16MCtrlSimulationCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x0f\n\x07paramId\x18\x02 \x01(\x05\x12\x12\n\nparamValue\x18\x03 \x03(\x05\";\n\x0fSysKnifeControl\x12\x13\n\x0bknifeStatus\x18\x01 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x02 \x01(\x05\"\x1a\n\x08SysBatUp\x12\x0e\n\x06\x62\x61tVal\x18\x01 \x01(\x05\"Z\n\x0cSysWorkState\x12\x13\n\x0b\x64\x65viceState\x18\x01 \x01(\x05\x12\x13\n\x0b\x63hargeState\x18\x02 \x01(\x05\x12\x0e\n\x06\x63mHash\x18\x03 \x01(\x03\x12\x10\n\x08pathHash\x18\x04 \x01(\x03\"5\n\x0eSysSetTimeZone\x12\x11\n\ttimeStamp\x18\x01 \x01(\x05\x12\x10\n\x08timeArea\x18\x02 \x01(\x05\"\x9e\x01\n\x0eSysSetDateTime\x12\x0c\n\x04year\x18\x01 \x01(\x05\x12\r\n\x05month\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61te\x18\x03 \x01(\x05\x12\x0c\n\x04week\x18\x04 \x01(\x05\x12\r\n\x05hours\x18\x05 \x01(\x05\x12\x0f\n\x07minutes\x18\x06 \x01(\x05\x12\x0f\n\x07seconds\x18\x07 \x01(\x05\x12\x10\n\x08timezone\x18\x08 \x01(\x05\x12\x10\n\x08\x64\x61ylight\x18\t \x01(\x05\"V\n\nSysJobPlan\x12\r\n\x05jobId\x18\x01 \x01(\x03\x12\x0f\n\x07jobMode\x18\x02 \x01(\x05\x12\x13\n\x0brainTactics\x18\x03 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x04 \x01(\x05\"\"\n\rSysDevErrCode\x12\x11\n\terrorCode\x18\x01 \x01(\x05\"!\n\x0cSysBoardType\x12\x11\n\tboardType\x18\x01 \x01(\x05\"5\n\x0cSysSwVersion\x12\x11\n\tboardType\x18\x01 \x01(\x05\x12\x12\n\nversionLen\x18\x02 \x01(\x05\"1\n\rSysDelJobPlan\x12\x10\n\x08\x64\x65viceId\x18\x01 \x01(\t\x12\x0e\n\x06planId\x18\x02 \x01(\t\"\xe1\x01\n\x0eSysJobPlanTime\x12\x0e\n\x06planId\x18\x01 \x01(\x03\x12\x14\n\x0cstartJobTime\x18\x02 \x01(\x05\x12\x12\n\nendJobTime\x18\x03 \x01(\x05\x12\x11\n\ttimeInDay\x18\x04 \x01(\x05\x12\x13\n\x0bjobPlanMode\x18\x05 \x01(\x05\x12\x15\n\rjobPlanEnable\x18\x06 \x01(\x05\x12\x1c\n\x07jobPlan\x18\n \x01(\x0b\x32\x0b.SysJobPlan\x12\x0f\n\x07weekDay\x18\x07 \x03(\x05\x12\x15\n\rtimeInWeekDay\x18\x08 \x01(\x05\x12\x10\n\x08\x65veryday\x18\t \x01(\x05\"k\n\nSysMowInfo\x12\x13\n\x0b\x64\x65viceState\x18\x01 \x01(\x05\x12\x0e\n\x06\x62\x61tVal\x18\x02 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x03 \x01(\x05\x12\x11\n\trTKstatus\x18\x04 \x01(\x05\x12\x10\n\x08rTKstars\x18\x05 \x01(\x05\";\n\x0eSysOptiLineAck\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x13\n\x0bresponesCmd\x18\x01 \x01(\x05\"5\n\nSysCommCmd\x12\n\n\x02rw\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\x05\"H\n\x15SysUploadFileProgress\x12\r\n\x05\x62izId\x18\x01 \x01(\t\x12\x0e\n\x06result\x18\x02 \x01(\x05\x12\x10\n\x08progress\x18\x03 \x01(\x05\"\x1e\n\x0cSysErrorCode\x12\x0e\n\x06\x63odeNo\x18\x01 \x01(\x05\"\x1e\n\tSysBorder\x12\x11\n\tborderval\x18\x01 \x01(\x05\")\n\x10SysPlanJobStatus\x12\x15\n\rplanjobStatus\x18\x01 \x01(\x05\"*\n\x14SysResetSystemStatus\x12\x12\n\nresetStaus\x18\x01 \x01(\x05\"\x8a\x01\n\rTimeCtrlLight\x12\x0f\n\x07operate\x18\x01 \x01(\x05\x12\x0e\n\x06\x65nable\x18\x02 \x01(\x05\x12\x12\n\nstart_hour\x18\x03 \x01(\x05\x12\x10\n\x08\x65nd_hour\x18\x05 \x01(\x05\x12\x11\n\tstart_min\x18\x04 \x01(\x05\x12\x0f\n\x07\x65nd_min\x18\x06 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x07 \x01(\x05\"6\n\x1asystemRapidStateTunnel_msg\x12\x18\n\x10rapid_state_data\x18\x01 \x03(\x03\"4\n\x19systemTardStateTunnel_msg\x12\x17\n\x0ftard_state_data\x18\x01 \x03(\x03\".\n\x13systemUpdateBuf_msg\x12\x17\n\x0fupdate_buf_data\x18\x01 \x03(\x03\"\x86\x01\n\x0fSysOffChipFlash\x12\n\n\x02op\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x12\n\nstart_addr\x18\x03 \x01(\x05\x12\x0e\n\x06offset\x18\x04 \x01(\x05\x12\x0e\n\x06length\x18\x05 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x0c\n\x04\x63ode\x18\x07 \x01(\x05\x12\x0b\n\x03msg\x18\x08 \x01(\t\"-\n\x14systemTmpCycleTx_msg\x12\x15\n\rcycle_tx_data\x18\x01 \x03(\x03\"&\n\nLoraCfgReq\x12\x0b\n\x03op_\x18\x01 \x01(\x05\x12\x0b\n\x03\x63\x66g\x18\x02 \x01(\t\"F\n\nLoraCfgRsp\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\n\n\x02op\x18\x02 \x01(\x05\x12\x0b\n\x03\x63\x66g\x18\x03 \x01(\t\x12\x0f\n\x07\x66\x61\x63_cfg\x18\x04 \x01(\t\">\n\x0bmod_fw_info\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x10\n\x08identify\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"L\n\x0e\x64\x65vice_fw_info\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x03mod\x18\x03 \x03(\x0b\x32\x0c.mod_fw_info\"@\n\x11mow_to_app_info_t\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0b\n\x03\x63md\x18\x02 \x01(\x05\x12\x10\n\x08mow_data\x18\x03 \x03(\x05\"\x98\x01\n\x10RptConnectStatus\x12\x14\n\x0c\x63onnect_type\x18\x01 \x01(\x05\x12\x10\n\x08\x62le_rssi\x18\x02 \x01(\x05\x12\x11\n\twifi_rssi\x18\x03 \x01(\x05\x12\x11\n\tlink_type\x18\x04 \x01(\x05\x12\x11\n\tmnet_rssi\x18\x05 \x01(\x05\x12\x11\n\tmnet_inet\x18\x06 \x01(\x05\x12\x10\n\x08used_net\x18\x07 \x01(\x05\"\x9f\x03\n\x07RptWork\x12\x0c\n\x04plan\x18\x01 \x01(\x05\x12\x11\n\tpath_hash\x18\x02 \x01(\x03\x12\x10\n\x08progress\x18\x03 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x04 \x01(\x05\x12\x0f\n\x07\x62p_info\x18\x05 \x01(\x05\x12\x0f\n\x07\x62p_hash\x18\x06 \x01(\x03\x12\x10\n\x08\x62p_pos_x\x18\x07 \x01(\x05\x12\x10\n\x08\x62p_pos_y\x18\x08 \x01(\x05\x12\x15\n\rreal_path_num\x18\t \x01(\x03\x12\x12\n\npath_pos_x\x18\n \x01(\x05\x12\x12\n\npath_pos_y\x18\x0b \x01(\x05\x12\x14\n\x0cub_zone_hash\x18\x0c \x01(\x03\x12\x14\n\x0cub_path_hash\x18\r \x01(\x03\x12\x15\n\rinit_cfg_hash\x18\x0e \x01(\x03\x12\x15\n\rub_ecode_hash\x18\x0f \x01(\x03\x12\x14\n\x0cnav_run_mode\x18\x10 \x01(\x05\x12\x18\n\x10test_mode_status\x18\x11 \x01(\x03\x12\x15\n\rman_run_speed\x18\x12 \x01(\x05\x12\x17\n\x0fnav_edit_status\x18\x13 \x01(\x05\x12\x14\n\x0cknife_height\x18\x14 \x01(\x05\"E\n\x0bRptMaintain\x12\x0f\n\x07mileage\x18\x01 \x01(\x03\x12\x11\n\twork_time\x18\x02 \x01(\x05\x12\x12\n\nbat_cycles\x18\x03 \x01(\x05\"\x84\x01\n\x0eRptDevLocation\x12\x12\n\nreal_pos_x\x18\x01 \x01(\x03\x12\x12\n\nreal_pos_y\x18\x02 \x01(\x03\x12\x13\n\x0breal_toward\x18\x03 \x01(\x05\x12\x10\n\x08pos_type\x18\x04 \x01(\x05\x12\x11\n\tzone_hash\x18\x05 \x01(\x03\x12\x10\n\x08\x62ol_hash\x18\x06 \x01(\x03\"8\n\x0f\x43ollectorStatus\x12%\n\x1d\x63ollector_installation_status\x18\x01 \x01(\x05\"0\n\x0fVioSurvivalInfo\x12\x1d\n\x15vio_survival_distance\x18\x01 \x01(\x02\"\x9e\x02\n\x0cRptDevStatus\x12\x12\n\nsys_status\x18\x01 \x01(\x05\x12\x14\n\x0c\x63harge_state\x18\x02 \x01(\x05\x12\x13\n\x0b\x62\x61ttery_val\x18\x03 \x01(\x05\x12\x15\n\rsensor_status\x18\x04 \x01(\x05\x12\x13\n\x0blast_status\x18\x05 \x01(\x05\x12\x16\n\x0esys_time_stamp\x18\x06 \x01(\x03\x12\x14\n\x0cvslam_status\x18\x07 \x01(\x05\x12\x1c\n\tmnet_info\x18\x08 \x01(\x0b\x32\t.MnetInfo\x12*\n\x10\x63ollector_status\x18\n \x01(\x0b\x32\x10.CollectorStatus\x12+\n\x11vio_survival_info\x18\t \x01(\x0b\x32\x10.VioSurvivalInfo\"\x8e\x01\n\x07RptLora\x12\x16\n\x0epair_code_scan\x18\x01 \x01(\x05\x12\x19\n\x11pair_code_channel\x18\x02 \x01(\x05\x12\x17\n\x0fpair_code_locid\x18\x03 \x01(\x05\x12\x17\n\x0fpair_code_netid\x18\x04 \x01(\x05\x12\x1e\n\x16lora_connection_status\x18\x05 \x01(\x05\"\xef\x01\n\x06RptRtk\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x11\n\tpos_level\x18\x02 \x01(\x05\x12\x11\n\tgps_stars\x18\x03 \x01(\x05\x12\x0b\n\x03\x61ge\x18\x04 \x01(\x05\x12\x0f\n\x07lat_std\x18\x05 \x01(\x05\x12\x0f\n\x07lon_std\x18\x06 \x01(\x05\x12\x10\n\x08l2_stars\x18\x07 \x01(\x05\x12\x12\n\ndis_status\x18\x08 \x01(\x03\x12\x17\n\x0ftop4_total_mean\x18\t \x01(\x05\x12\x15\n\rco_view_stars\x18\n \x01(\x05\x12\r\n\x05reset\x18\x0b \x01(\x05\x12\x1b\n\tlora_info\x18\x0c \x01(\x0b\x32\x08.RptLora\"\x96\x01\n\x0fVioToAppInfoMsg\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\x12\x0f\n\x07heading\x18\x03 \x01(\x01\x12\x11\n\tvio_state\x18\x04 \x01(\x05\x12\x12\n\nbrightness\x18\x05 \x01(\x05\x12\x1a\n\x12\x64\x65tect_feature_num\x18\x06 \x01(\x05\x12\x19\n\x11track_feature_num\x18\x07 \x01(\x05\"1\n\x0eVisionPointMsg\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"W\n\x12VisionPointInfoMsg\x12\r\n\x05label\x18\x01 \x01(\x05\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12%\n\x0cvision_point\x18\x03 \x03(\x0b\x32\x0f.VisionPointMsg\"/\n\x12VisionStatisticMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x02\x12\x0b\n\x03var\x18\x02 \x01(\x02\"h\n\x16VisionStatisticInfoMsg\x12\x11\n\ttimestamp\x18\x01 \x01(\x01\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12.\n\x11vision_statistics\x18\x03 \x03(\x0b\x32\x13.VisionStatisticMsg\"\xf7\x02\n\x0eReportInfoData\x12\"\n\x07\x63onnect\x18\x01 \x01(\x0b\x32\x11.RptConnectStatus\x12\x1a\n\x03\x64\x65v\x18\x02 \x01(\x0b\x32\r.RptDevStatus\x12 \n\x07\x66w_info\x18\x06 \x01(\x0b\x32\x0f.device_fw_info\x12\"\n\tlocations\x18\x04 \x03(\x0b\x32\x0f.RptDevLocation\x12\x1e\n\x08maintain\x18\x07 \x01(\x0b\x32\x0c.RptMaintain\x12\x14\n\x03rtk\x18\x03 \x01(\x0b\x32\x07.RptRtk\x12)\n\x0fvio_to_app_info\x18\t \x01(\x0b\x32\x10.VioToAppInfoMsg\x12.\n\x11vision_point_info\x18\x08 \x03(\x0b\x32\x13.VisionPointInfoMsg\x12\x36\n\x15vision_statistic_info\x18\n \x01(\x0b\x32\x17.VisionStatisticInfoMsg\x12\x16\n\x04work\x18\x05 \x01(\x0b\x32\x08.RptWork\"\\\n\x15\x44\x65viceProductTypeInfo\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\x19\n\x11main_product_type\x18\x02 \x01(\t\x12\x18\n\x10sub_product_type\x18\x03 \x01(\t\"\x81\x01\n\rReportInfoCfg\x12\x0b\n\x03\x61\x63t\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\x12\x0e\n\x06period\x18\x03 \x01(\x05\x12\x18\n\x10no_change_period\x18\x04 \x01(\x05\x12\r\n\x05\x63ount\x18\x05 \x01(\x05\x12\x19\n\x03sub\x18\x06 \x03(\x0e\x32\x0c.RptInfoType\"\x87\x01\n\x13MowToAppQCToolsInfo\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x18\n\x10time_of_duration\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x16\n\x0eresult_details\x18\x04 \x01(\t\x12 \n\x06\x65xcept\x18\x05 \x03(\x0b\x32\x10.QCAppTestExcept\"P\n\x0fQCAppTestExcept\x12\x13\n\x0b\x65xcept_type\x18\x01 \x01(\t\x12(\n\nconditions\x18\x02 \x03(\x0b\x32\x14.QCAppTestConditions\"t\n\x13QCAppTestConditions\x12\x11\n\tcond_type\x18\x01 \x01(\t\x12\x0f\n\x07int_val\x18\x02 \x01(\x05\x12\x11\n\tfloat_val\x18\x03 \x01(\x02\x12\x12\n\ndouble_val\x18\x04 \x01(\x01\x12\x12\n\nstring_val\x18\x05 \x01(\t*+\n\tOperation\x12\t\n\x05WRITE\x10\x00\x12\x08\n\x04READ\x10\x01\x12\t\n\x05\x45RASE\x10\x02*\x8d\x02\n\tOffPartId\x12\x13\n\x0fOFF_PART_DL_IMG\x10\x00\x12\x19\n\x15OFF_PART_UPDINFO_BACK\x10\x01\x12\x14\n\x10OFF_PART_UPDINFO\x10\x02\x12\x13\n\x0fOFF_PART_NAKEDB\x10\x03\x12\x14\n\x10OFF_PART_FLASHDB\x10\x04\x12\x18\n\x14OFF_PART_UPD_APP_IMG\x10\x05\x12\x18\n\x14OFF_PART_UPD_BMS_IMG\x10\x06\x12\x18\n\x14OFF_PART_UPD_TMP_IMG\x10\x07\x12\x15\n\x11OFF_PART_DEV_INFO\x10\x08\x12\x18\n\x14OFF_PART_NAKEDB_BACK\x10\t\x12\x10\n\x0cOFF_PART_MAX\x10\n*\xbd\x01\n\x0bRptInfoType\x12\x0f\n\x0bRIT_CONNECT\x10\x00\x12\x0f\n\x0bRIT_DEV_STA\x10\x01\x12\x0b\n\x07RIT_RTK\x10\x02\x12\x11\n\rRIT_DEV_LOCAL\x10\x03\x12\x0c\n\x08RIT_WORK\x10\x04\x12\x0f\n\x0bRIT_FW_INFO\x10\x05\x12\x10\n\x0cRIT_MAINTAIN\x10\x06\x12\x14\n\x10RIT_VISION_POINT\x10\x07\x12\x0b\n\x07RIT_VIO\x10\x08\x12\x18\n\x14RIT_VISION_STATISTIC\x10\tb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mctrl_nav_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.mctrl_sys_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _globals['_NAVLATLONUP']._serialized_start=33
-  _globals['_NAVLATLONUP']._serialized_end=72
-  _globals['_NAVBORDERSTATE']._serialized_start=74
-  _globals['_NAVBORDERSTATE']._serialized_end=107
-  _globals['_NAVPOSUP']._serialized_start=110
-  _globals['_NAVPOSUP']._serialized_end=311
-  _globals['_NAVBORDERDATAGETACK']._serialized_start=313
-  _globals['_NAVBORDERDATAGETACK']._serialized_end=371
-  _globals['_NAVOBSTIBORDERDATAGET']._serialized_start=373
-  _globals['_NAVOBSTIBORDERDATAGET']._serialized_end=463
-  _globals['_NAVOBSTIBORDERDATAGETACK']._serialized_start=465
-  _globals['_NAVOBSTIBORDERDATAGETACK']._serialized_end=536
-  _globals['_NAVCHLLINEDATA']._serialized_start=538
-  _globals['_NAVCHLLINEDATA']._serialized_end=638
-  _globals['_NAVCHLLINEDATAACK']._serialized_start=640
-  _globals['_NAVCHLLINEDATAACK']._serialized_end=719
-  _globals['_NAVBORDERDATAGET']._serialized_start=721
-  _globals['_NAVBORDERDATAGET']._serialized_end=795
-  _globals['_NAVTASKINFO']._serialized_start=797
-  _globals['_NAVTASKINFO']._serialized_end=924
-  _globals['_NAVOPTLINEUP']._serialized_start=927
-  _globals['_NAVOPTLINEUP']._serialized_end=1072
-  _globals['_NAVOPTIBORDERINFO']._serialized_start=1074
-  _globals['_NAVOPTIBORDERINFO']._serialized_end=1200
-  _globals['_NAVOPTOBSINFO']._serialized_start=1203
-  _globals['_NAVOPTOBSINFO']._serialized_end=1332
-  _globals['_NAVSTARTJOB']._serialized_start=1335
-  _globals['_NAVSTARTJOB']._serialized_end=1515
-  _globals['_NAVGETHASHLIST']._serialized_start=1517
-  _globals['_NAVGETHASHLIST']._serialized_end=1641
-  _globals['_NAVGETHASHLISTACK']._serialized_start=1644
-  _globals['_NAVGETHASHLISTACK']._serialized_end=1808
-  _globals['_NAVGETCOMMDATA']._serialized_start=1811
-  _globals['_NAVGETCOMMDATA']._serialized_end=2025
-  _globals['_NAVGETCOMMDATAACK']._serialized_start=2028
-  _globals['_NAVGETCOMMDATAACK']._serialized_end=2315
-  _globals['_NAVREQCOVERPATH']._serialized_start=2318
-  _globals['_NAVREQCOVERPATH']._serialized_end=2616
-  _globals['_NAVUPLOADZIGZAGRESULT']._serialized_start=2619
-  _globals['_NAVUPLOADZIGZAGRESULT']._serialized_end=3042
-  _globals['_NAVUPLOADZIGZAGRESULTACK']._serialized_start=3045
-  _globals['_NAVUPLOADZIGZAGRESULTACK']._serialized_end=3221
-  _globals['_NAVTASKCTRL']._serialized_start=3223
-  _globals['_NAVTASKCTRL']._serialized_end=3300
-  _globals['_NAVTASKIDRW']._serialized_start=3302
-  _globals['_NAVTASKIDRW']._serialized_end=3413
-  _globals['_NAVSYSHASHOVERVIEW']._serialized_start=3415
-  _globals['_NAVSYSHASHOVERVIEW']._serialized_end=3489
-  _globals['_NAVTASKBREAKPOINT']._serialized_start=3491
-  _globals['_NAVTASKBREAKPOINT']._serialized_end=3596
-  _globals['_NAVPLANJOBSET']._serialized_start=3599
-  _globals['_NAVPLANJOBSET']._serialized_end=4145
-  _globals['_NAVRESFRAME']._serialized_start=4147
-  _globals['_NAVRESFRAME']._serialized_end=4177
-  _globals['_NAVTASKPROGRESS']._serialized_start=4179
-  _globals['_NAVTASKPROGRESS']._serialized_end=4218
-  _globals['_NAVUNABLETIMESET']._serialized_start=4221
-  _globals['_NAVUNABLETIMESET']._serialized_end=4355
-  _globals['_SIMULATIONCMDDATA']._serialized_start=4357
-  _globals['_SIMULATIONCMDDATA']._serialized_end=4429
-  _globals['_WORKREPORTCMDDATA']._serialized_start=4431
-  _globals['_WORKREPORTCMDDATA']._serialized_end=4486
-  _globals['_WORKREPORTINFOACK']._serialized_start=4489
-  _globals['_WORKREPORTINFOACK']._serialized_end=4742
-  _globals['_WORKREPORTUPDATEACK']._serialized_start=4744
-  _globals['_WORKREPORTUPDATEACK']._serialized_end=4802
-  _globals['_WORKREPORTUPDATECMD']._serialized_start=4804
-  _globals['_WORKREPORTUPDATECMD']._serialized_end=4841
-  _globals['_CHARGEPILETYPE']._serialized_start=4843
-  _globals['_CHARGEPILETYPE']._serialized_end=4897
-  _globals['_MCTLNAV']._serialized_start=4900
-  _globals['_MCTLNAV']._serialized_end=6824
+  _OPERATION._serialized_start=6798
+  _OPERATION._serialized_end=6841
+  _OFFPARTID._serialized_start=6844
+  _OFFPARTID._serialized_end=7113
+  _RPTINFOTYPE._serialized_start=7116
+  _RPTINFOTYPE._serialized_end=7305
+  _MCTLSYS._serialized_start=61
+  _MCTLSYS._serialized_end=1621
+  _MCTRLSIMULATIONCMDDATA._serialized_start=1623
+  _MCTRLSIMULATIONCMDDATA._serialized_end=1700
+  _SYSKNIFECONTROL._serialized_start=1702
+  _SYSKNIFECONTROL._serialized_end=1761
+  _SYSBATUP._serialized_start=1763
+  _SYSBATUP._serialized_end=1789
+  _SYSWORKSTATE._serialized_start=1791
+  _SYSWORKSTATE._serialized_end=1881
+  _SYSSETTIMEZONE._serialized_start=1883
+  _SYSSETTIMEZONE._serialized_end=1936
+  _SYSSETDATETIME._serialized_start=1939
+  _SYSSETDATETIME._serialized_end=2097
+  _SYSJOBPLAN._serialized_start=2099
+  _SYSJOBPLAN._serialized_end=2185
+  _SYSDEVERRCODE._serialized_start=2187
+  _SYSDEVERRCODE._serialized_end=2221
+  _SYSBOARDTYPE._serialized_start=2223
+  _SYSBOARDTYPE._serialized_end=2256
+  _SYSSWVERSION._serialized_start=2258
+  _SYSSWVERSION._serialized_end=2311
+  _SYSDELJOBPLAN._serialized_start=2313
+  _SYSDELJOBPLAN._serialized_end=2362
+  _SYSJOBPLANTIME._serialized_start=2365
+  _SYSJOBPLANTIME._serialized_end=2590
+  _SYSMOWINFO._serialized_start=2592
+  _SYSMOWINFO._serialized_end=2699
+  _SYSOPTILINEACK._serialized_start=2701
+  _SYSOPTILINEACK._serialized_end=2760
+  _SYSCOMMCMD._serialized_start=2762
+  _SYSCOMMCMD._serialized_end=2815
+  _SYSUPLOADFILEPROGRESS._serialized_start=2817
+  _SYSUPLOADFILEPROGRESS._serialized_end=2889
+  _SYSERRORCODE._serialized_start=2891
+  _SYSERRORCODE._serialized_end=2921
+  _SYSBORDER._serialized_start=2923
+  _SYSBORDER._serialized_end=2953
+  _SYSPLANJOBSTATUS._serialized_start=2955
+  _SYSPLANJOBSTATUS._serialized_end=2996
+  _SYSRESETSYSTEMSTATUS._serialized_start=2998
+  _SYSRESETSYSTEMSTATUS._serialized_end=3040
+  _TIMECTRLLIGHT._serialized_start=3043
+  _TIMECTRLLIGHT._serialized_end=3181
+  _SYSTEMRAPIDSTATETUNNEL_MSG._serialized_start=3183
+  _SYSTEMRAPIDSTATETUNNEL_MSG._serialized_end=3237
+  _SYSTEMTARDSTATETUNNEL_MSG._serialized_start=3239
+  _SYSTEMTARDSTATETUNNEL_MSG._serialized_end=3291
+  _SYSTEMUPDATEBUF_MSG._serialized_start=3293
+  _SYSTEMUPDATEBUF_MSG._serialized_end=3339
+  _SYSOFFCHIPFLASH._serialized_start=3342
+  _SYSOFFCHIPFLASH._serialized_end=3476
+  _SYSTEMTMPCYCLETX_MSG._serialized_start=3478
+  _SYSTEMTMPCYCLETX_MSG._serialized_end=3523
+  _LORACFGREQ._serialized_start=3525
+  _LORACFGREQ._serialized_end=3563
+  _LORACFGRSP._serialized_start=3565
+  _LORACFGRSP._serialized_end=3635
+  _MOD_FW_INFO._serialized_start=3637
+  _MOD_FW_INFO._serialized_end=3699
+  _DEVICE_FW_INFO._serialized_start=3701
+  _DEVICE_FW_INFO._serialized_end=3777
+  _MOW_TO_APP_INFO_T._serialized_start=3779
+  _MOW_TO_APP_INFO_T._serialized_end=3843
+  _RPTCONNECTSTATUS._serialized_start=3846
+  _RPTCONNECTSTATUS._serialized_end=3998
+  _RPTWORK._serialized_start=4001
+  _RPTWORK._serialized_end=4416
+  _RPTMAINTAIN._serialized_start=4418
+  _RPTMAINTAIN._serialized_end=4487
+  _RPTDEVLOCATION._serialized_start=4490
+  _RPTDEVLOCATION._serialized_end=4622
+  _COLLECTORSTATUS._serialized_start=4624
+  _COLLECTORSTATUS._serialized_end=4680
+  _VIOSURVIVALINFO._serialized_start=4682
+  _VIOSURVIVALINFO._serialized_end=4730
+  _RPTDEVSTATUS._serialized_start=4733
+  _RPTDEVSTATUS._serialized_end=5019
+  _RPTLORA._serialized_start=5022
+  _RPTLORA._serialized_end=5164
+  _RPTRTK._serialized_start=5167
+  _RPTRTK._serialized_end=5406
+  _VIOTOAPPINFOMSG._serialized_start=5409
+  _VIOTOAPPINFOMSG._serialized_end=5559
+  _VISIONPOINTMSG._serialized_start=5561
+  _VISIONPOINTMSG._serialized_end=5610
+  _VISIONPOINTINFOMSG._serialized_start=5612
+  _VISIONPOINTINFOMSG._serialized_end=5699
+  _VISIONSTATISTICMSG._serialized_start=5701
+  _VISIONSTATISTICMSG._serialized_end=5748
+  _VISIONSTATISTICINFOMSG._serialized_start=5750
+  _VISIONSTATISTICINFOMSG._serialized_end=5854
+  _REPORTINFODATA._serialized_start=5857
+  _REPORTINFODATA._serialized_end=6232
+  _DEVICEPRODUCTTYPEINFO._serialized_start=6234
+  _DEVICEPRODUCTTYPEINFO._serialized_end=6326
+  _REPORTINFOCFG._serialized_start=6329
+  _REPORTINFOCFG._serialized_end=6458
+  _MOWTOAPPQCTOOLSINFO._serialized_start=6461
+  _MOWTOAPPQCTOOLSINFO._serialized_end=6596
+  _QCAPPTESTEXCEPT._serialized_start=6598
+  _QCAPPTESTEXCEPT._serialized_end=6678
+  _QCAPPTESTCONDITIONS._serialized_start=6680
+  _QCAPPTESTCONDITIONS._serialized_end=6796
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.2/pyluba/utility/periodic.py` & `pyluba-0.0.4/pyluba/utility/periodic.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyluba/utility/rocker_util.py` & `pyluba-0.0.4/pyluba/utility/rocker_util.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.2/pyproject.toml` & `pyluba-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 [tool.poetry]
 name        = "pyluba"
-version     = "0.0.2"
+version     = "0.0.4"
 license     = "GNU-3.0"
 description = ""
 readme      = "README.md"
 authors     = [
     "Michael Arthur <michael@jumblesoft.co.nz>",
     "Jan Dalheimer <jan@dalheimer.de>"
 ]
 packages = [{include = "pyluba"}]
 
 
 [tool.poetry.dependencies]
-python = ">=3.11"
+python = ">=3.11,<3.13"
 bleak = "^0.21.1"
-protobuf = "^4.25.1"
+protobuf = "^5.26.1"
 py-jsonic = "^0.0.2"
 pydantic = "^2.5.3"
 aliyun-python-sdk-iot = "^8.57.0"
 aliyun-iot-linkkit = "^1.2.12"
 aiohttp = "^3.9.1"
 paho-mqtt = "^1.6.1"
 alicloud-gateway-iot = "^1.0.0"
 alibabacloud-apigateway-util = "^0.0.2"
 alibabacloud-iot-api-gateway = "^0.0.4"
 twine = "^5.0.0"
+frida-tools = "^12.3.0"
+protobuf-to-pydantic = {version = "^0.2.6.2", extras = ["mypy-protobuf"]}
+grpcio-tools = "^1.63.0"
+bleak-retry-connector = "^3.5.0"
+jsonic = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 types-protobuf = "^4.23.0.1"
 mypy-protobuf = "^3.4.0"
 
 
 [tool.bumpver]
```

### Comparing `pyluba-0.0.2/PKG-INFO` & `pyluba-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: pyluba
-Version: 0.0.2
+Version: 0.0.4
 Summary: 
 License: GNU-3.0
 Author: Michael Arthur
 Author-email: michael@jumblesoft.co.nz
-Requires-Python: >=3.11
+Requires-Python: >=3.11,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: alibabacloud-apigateway-util (>=0.0.2,<0.0.3)
 Requires-Dist: alibabacloud-iot-api-gateway (>=0.0.4,<0.0.5)
 Requires-Dist: alicloud-gateway-iot (>=1.0.0,<2.0.0)
 Requires-Dist: aliyun-iot-linkkit (>=1.2.12,<2.0.0)
 Requires-Dist: aliyun-python-sdk-iot (>=8.57.0,<9.0.0)
 Requires-Dist: bleak (>=0.21.1,<0.22.0)
+Requires-Dist: bleak-retry-connector (>=3.5.0,<4.0.0)
+Requires-Dist: frida-tools (>=12.3.0,<13.0.0)
+Requires-Dist: grpcio-tools (>=1.63.0,<2.0.0)
+Requires-Dist: jsonic (>=1.0.0,<2.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: protobuf (>=4.25.1,<5.0.0)
+Requires-Dist: protobuf (>=5.26.1,<6.0.0)
+Requires-Dist: protobuf-to-pydantic[mypy-protobuf] (>=0.2.6.2,<0.3.0.0)
 Requires-Dist: py-jsonic (>=0.0.2,<0.0.3)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: twine (>=5.0.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 [![SemVer 0.8.5][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
@@ -39,7 +44,9 @@
 
 # PyLuba API
 
 API to control Luba via MQTT, Cloud and bluetooth.
 
 See wiki for progress and issues for ways you can help in the effort.
 
+protobuf and protobuf models are generated using protobuf_to_pydantic and protoc
+
```

