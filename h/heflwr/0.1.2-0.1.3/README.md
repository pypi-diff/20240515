# Comparing `tmp/heflwr-0.1.2.tar.gz` & `tmp/heflwr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heflwr-0.1.2.tar", last modified: Mon May 13 09:50:43 2024, max compression
+gzip compressed data, was "heflwr-0.1.3.tar", last modified: Wed May 15 12:54:57 2024, max compression
```

## Comparing `heflwr-0.1.2.tar` & `heflwr-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.390899 heflwr-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-03-07 16:35:19.000000 heflwr-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       15 2024-05-13 08:46:58.000000 heflwr-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      552 2024-05-13 09:50:43.390899 heflwr-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-12 17:35:02.000000 heflwr-0.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-13 09:50:43.390899 heflwr-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-05-13 09:50:22.000000 heflwr-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.357892 heflwr-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.362876 heflwr-0.1.2/src/heflwr/
--rw-rw-rw-   0        0        0       79 2024-05-12 16:35:15.000000 heflwr-0.1.2/src/heflwr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.375832 heflwr-0.1.2/src/heflwr/fed/
--rw-rw-rw-   0        0        0       87 2024-05-12 16:19:55.000000 heflwr-0.1.2/src/heflwr/fed/__init__.py
--rw-rw-rw-   0        0        0     6687 2024-05-13 08:14:45.000000 heflwr-0.1.2/src/heflwr/fed/aggregate.py
--rw-rw-rw-   0        0        0        0 2024-05-12 14:56:04.000000 heflwr-0.1.2/src/heflwr/fed/he_client_manager.py
--rw-rw-rw-   0        0        0     4745 2024-05-13 09:50:22.000000 heflwr-0.1.2/src/heflwr/fed/hetero_aggregate.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.377699 heflwr-0.1.2/src/heflwr/log/
--rw-rw-rw-   0        0        0       22 2024-05-12 16:35:15.000000 heflwr-0.1.2/src/heflwr/log/__init__.py
--rw-rw-rw-   0        0        0     3463 2024-04-27 12:54:05.000000 heflwr-0.1.2/src/heflwr/log/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.378698 heflwr-0.1.2/src/heflwr/monitor/
--rw-rw-rw-   0        0        0       61 2024-05-12 16:24:06.000000 heflwr-0.1.2/src/heflwr/monitor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.381688 heflwr-0.1.2/src/heflwr/monitor/process_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-12 16:31:05.000000 heflwr-0.1.2/src/heflwr/monitor/process_monitor/__init__.py
--rw-rw-rw-   0        0        0     5522 2024-05-13 08:32:46.000000 heflwr-0.1.2/src/heflwr/monitor/process_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5541 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/monitor/process_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5356 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/monitor/process_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.384678 heflwr-0.1.2/src/heflwr/monitor/thread_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-12 16:31:05.000000 heflwr-0.1.2/src/heflwr/monitor/thread_monitor/__init__.py
--rw-rw-rw-   0        0        0     4938 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/monitor/thread_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5299 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5025 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/monitor/thread_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.386671 heflwr-0.1.2/src/heflwr/monitor/utils/
--rw-rw-rw-   0        0        0        0 2024-04-27 15:24:20.000000 heflwr-0.1.2/src/heflwr/monitor/utils/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/monitor/utils/network.py
--rw-rw-rw-   0        0        0     4500 2024-05-13 08:10:14.000000 heflwr-0.1.2/src/heflwr/monitor/utils/power.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.388664 heflwr-0.1.2/src/heflwr/nn/
--rw-rw-rw-   0        0        0      153 2024-05-13 07:44:10.000000 heflwr-0.1.2/src/heflwr/nn/__init__.py
--rw-rw-rw-   0        0        0      351 2024-05-13 07:27:27.000000 heflwr-0.1.2/src/heflwr/nn/scaler.py
--rw-rw-rw-   0        0        0     9696 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/nn/ssconv2d.py
--rw-rw-rw-   0        0        0     9284 2024-05-13 07:35:10.000000 heflwr-0.1.2/src/heflwr/nn/sslinear.py
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.373844 heflwr-0.1.2/src/heflwr.egg-info/
--rw-rw-rw-   0        0        0      552 2024-05-13 09:50:43.000000 heflwr-0.1.2/src/heflwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2024-05-13 09:50:43.000000 heflwr-0.1.2/src/heflwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 09:50:43.000000 heflwr-0.1.2/src/heflwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 09:50:43.000000 heflwr-0.1.2/src/heflwr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 09:50:43.389661 heflwr-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-05-12 18:35:12.000000 heflwr-0.1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.479993 heflwr-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:05:22.000000 heflwr-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       15 2024-05-14 16:05:22.000000 heflwr-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      552 2024-05-15 12:54:57.478993 heflwr-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-14 16:05:22.000000 heflwr-0.1.3/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-15 12:54:57.479993 heflwr-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-05-15 12:54:23.000000 heflwr-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.424346 heflwr-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.439346 heflwr-0.1.3/src/heflwr/
+-rw-rw-rw-   0        0        0      104 2024-05-15 12:54:23.000000 heflwr-0.1.3/src/heflwr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.456993 heflwr-0.1.3/src/heflwr/fed/
+-rw-rw-rw-   0        0        0       87 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/__init__.py
+-rw-rw-rw-   0        0        0     6687 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/aggregate.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/he_client_manager.py
+-rw-rw-rw-   0        0        0     4746 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/hetero_aggregate.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.457993 heflwr-0.1.3/src/heflwr/log/
+-rw-rw-rw-   0        0        0       22 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/log/__init__.py
+-rw-rw-rw-   0        0        0     3458 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/log/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.458994 heflwr-0.1.3/src/heflwr/monitor/
+-rw-rw-rw-   0        0        0       61 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.463993 heflwr-0.1.3/src/heflwr/monitor/process_monitor/
+-rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/__init__.py
+-rw-rw-rw-   0        0        0     5522 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5541 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5356 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.468993 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/
+-rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/__init__.py
+-rw-rw-rw-   0        0        0     4938 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5299 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5025 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.471993 heflwr-0.1.3/src/heflwr/monitor/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/utils/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/utils/network.py
+-rw-rw-rw-   0        0        0     4500 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/utils/power.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.475993 heflwr-0.1.3/src/heflwr/nn/
+-rw-rw-rw-   0        0        0      153 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/scaler.py
+-rw-rw-rw-   0        0        0     9696 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/ssconv2d.py
+-rw-rw-rw-   0        0        0     9284 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/sslinear.py
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.452993 heflwr-0.1.3/src/heflwr.egg-info/
+-rw-rw-rw-   0        0        0      552 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.476993 heflwr-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.3/tests/test.py
```

### Comparing `heflwr-0.1.2/LICENSE` & `heflwr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/PKG-INFO` & `heflwr-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflwr
-Version: 0.1.2
+Version: 0.1.3
 Summary: 「HeFlwr」is a federated learning package for heterogeneous devices.
 Home-page: https://github.com/QVQZZZ/HeFlwr
 Author: Zhu Yaolin
 Author-email: zhuyaolinluck@qq.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `heflwr-0.1.2/setup.py` & `heflwr-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.rst", encoding="UTF-8") as f:
         return f.read()
 
 
 setup(
     name="heflwr",
-    version="0.1.2",
+    version="0.1.3",
     description="「HeFlwr」is a federated learning package for heterogeneous devices.",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     author="Zhu Yaolin",
     author_email="zhuyaolinluck@qq.com",
     long_description=readme(),
     long_description_content_type='text/x-rst',
```

### Comparing `heflwr-0.1.2/src/heflwr/fed/aggregate.py` & `heflwr-0.1.3/src/heflwr/fed/aggregate.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/fed/hetero_aggregate.py` & `heflwr-0.1.3/src/heflwr/fed/hetero_aggregate.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,12 +76,12 @@
             client_net.load_state_dict(client_dict)
 
         for layer_name, layer in dict(server_net.named_modules()).items():
             if isinstance(layer, Union[SSConv2d, SSLinear]):
                 client_layers = [dict(client_net.named_modules())[layer_name] for client_net in client_nets]
                 aggregate_layer(layer, client_layers, num_examples_list)
             else:
-                logger.warn(f"Can't merge {layer}, ignore it.")
+                logger.debug(f"Can't merge {layer}, ignore it.")
 
         array_list: List[np.ndarray] = [_.numpy() for _ in list(server_net.parameters())]
         parameters = ndarrays_to_parameters(array_list)
     return parameters
```

### Comparing `heflwr-0.1.2/src/heflwr/log/logger.py` & `heflwr-0.1.3/src/heflwr/log/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from logging.handlers import HTTPHandler
 from logging import LogRecord
 from typing import Any, Dict, Optional, Tuple, Union
 from ssl import SSLContext
 import warnings
 
 # Create logger
-LOGGER_NAME = "hetero-flwr"
+LOGGER_NAME = "HeFlwr"
 HETERO_FLOWER_LOGGER = logging.getLogger(LOGGER_NAME)
 HETERO_FLOWER_LOGGER.setLevel(logging.DEBUG)
 
 # Console default formatter
 COMMON_LOG_FORMAT = "%(levelname)s %(name)s %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
 DEFAULT_FORMATTER = logging.Formatter(COMMON_LOG_FORMAT)
```

### Comparing `heflwr-0.1.2/src/heflwr/monitor/process_monitor/file_monitor.py` & `heflwr-0.1.3/src/heflwr/monitor/process_monitor/file_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/monitor/process_monitor/prometheus_monitor.py` & `heflwr-0.1.3/src/heflwr/monitor/process_monitor/prometheus_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/monitor/process_monitor/remote_monitor.py` & `heflwr-0.1.3/src/heflwr/monitor/process_monitor/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/monitor/thread_monitor/file_monitor.py` & `heflwr-0.1.3/src/heflwr/monitor/thread_monitor/file_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/monitor/thread_monitor/prometheus_monitor.py` & `heflwr-0.1.3/src/heflwr/monitor/thread_monitor/prometheus_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/monitor/thread_monitor/remote_monitor.py` & `heflwr-0.1.3/src/heflwr/monitor/thread_monitor/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/monitor/utils/network.py` & `heflwr-0.1.3/src/heflwr/monitor/utils/network.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/monitor/utils/power.py` & `heflwr-0.1.3/src/heflwr/monitor/utils/power.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/nn/ssconv2d.py` & `heflwr-0.1.3/src/heflwr/nn/ssconv2d.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr/nn/sslinear.py` & `heflwr-0.1.3/src/heflwr/nn/sslinear.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.2/src/heflwr.egg-info/PKG-INFO` & `heflwr-0.1.3/src/heflwr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflwr
-Version: 0.1.2
+Version: 0.1.3
 Summary: 「HeFlwr」is a federated learning package for heterogeneous devices.
 Home-page: https://github.com/QVQZZZ/HeFlwr
 Author: Zhu Yaolin
 Author-email: zhuyaolinluck@qq.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `heflwr-0.1.2/src/heflwr.egg-info/SOURCES.txt` & `heflwr-0.1.3/src/heflwr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

