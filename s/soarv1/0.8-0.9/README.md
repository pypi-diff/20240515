# Comparing `tmp/soarv1-0.8.tar.gz` & `tmp/soarv1-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soarv1-0.8.tar", last modified: Tue May 14 11:19:01 2024, max compression
+gzip compressed data, was "soarv1-0.9.tar", last modified: Wed May 15 01:19:40 2024, max compression
```

## Comparing `soarv1-0.8.tar` & `soarv1-0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.150057 soarv1-0.8/
--rw-rw-rw-   0        0        0      634 2024-05-14 11:19:01.150057 soarv1-0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-14 11:19:01.150057 soarv1-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.130056 soarv1-0.8/soar/
--rw-rw-rw-   0        0        0      126 2024-05-14 11:18:42.000000 soarv1-0.8/soar/__init__.py
--rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.8/soar/config.py
--rw-rw-rw-   0        0        0     8044 2024-05-14 11:18:33.000000 soarv1-0.8/soar/context.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.133055 soarv1-0.8/soar/datasets/
--rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.8/soar/datasets/__init__.py
--rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.8/soar/datasets/augment.py
--rw-rw-rw-   0        0        0     1402 2024-05-10 06:09:42.000000 soarv1-0.8/soar/datasets/dataloader.py
--rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.8/soar/datasets/dataset.py
--rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.8/soar/datasets/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.136054 soarv1-0.8/soar/engine/
--rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.8/soar/engine/__init__.py
--rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.8/soar/engine/exporter.py
--rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.8/soar/engine/predictor.py
--rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.8/soar/engine/trainer.py
--rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.8/soar/engine/validator.py
--rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.8/soar/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.139056 soarv1-0.8/soar/models/
--rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.8/soar/models/__init__.py
--rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.8/soar/models/botnet.py
--rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.8/soar/models/model.py
--rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.8/soar/models/resnet.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.145055 soarv1-0.8/soar/utils/
--rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.8/soar/utils/__init__.py
--rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.8/soar/utils/crypt.py
--rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.8/soar/utils/ema.py
--rw-rw-rw-   0        0        0     3534 2024-05-14 09:45:06.000000 soarv1-0.8/soar/utils/event.py
--rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.8/soar/utils/logger.py
--rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.8/soar/utils/loss.py
--rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.8/soar/utils/metric.py
--rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.8/soar/utils/optimizer.py
--rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.8/soar/utils/parallel.py
--rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.8/soar/utils/scheduler.py
--rw-rw-rw-   0        0        0     1443 2024-05-14 07:57:35.000000 soarv1-0.8/soar/utils/storager.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.146057 soarv1-0.8/soar/weights/
--rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.8/soar/weights/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:19:01.149055 soarv1-0.8/soarv1.egg-info/
--rw-rw-rw-   0        0        0      634 2024-05-14 11:19:01.000000 soarv1-0.8/soarv1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      820 2024-05-14 11:19:01.000000 soarv1-0.8/soarv1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:19:01.000000 soarv1-0.8/soarv1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2024-05-14 11:19:01.000000 soarv1-0.8/soarv1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-14 11:19:01.000000 soarv1-0.8/soarv1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.675597 soarv1-0.9/
+-rw-rw-rw-   0        0        0      634 2024-05-15 01:19:40.674595 soarv1-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-15 01:19:40.675597 soarv1-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-10 04:20:32.000000 soarv1-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.653595 soarv1-0.9/soar/
+-rw-rw-rw-   0        0        0      126 2024-05-15 01:19:29.000000 soarv1-0.9/soar/__init__.py
+-rw-rw-rw-   0        0        0      807 2024-04-24 09:55:36.000000 soarv1-0.9/soar/config.py
+-rw-rw-rw-   0        0        0     8044 2024-05-14 11:18:33.000000 soarv1-0.9/soar/context.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.657596 soarv1-0.9/soar/datasets/
+-rw-rw-rw-   0        0        0      168 2024-04-19 03:51:36.000000 soarv1-0.9/soar/datasets/__init__.py
+-rw-rw-rw-   0        0        0    11892 2024-04-11 07:34:48.000000 soarv1-0.9/soar/datasets/augment.py
+-rw-rw-rw-   0        0        0     1402 2024-05-10 06:09:42.000000 soarv1-0.9/soar/datasets/dataloader.py
+-rw-rw-rw-   0        0        0     2156 2024-04-24 14:49:32.000000 soarv1-0.9/soar/datasets/dataset.py
+-rw-rw-rw-   0        0        0      624 2024-04-07 10:23:04.000000 soarv1-0.9/soar/datasets/transform.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.660595 soarv1-0.9/soar/engine/
+-rw-rw-rw-   0        0        0      118 2024-03-24 08:54:17.000000 soarv1-0.9/soar/engine/__init__.py
+-rw-rw-rw-   0        0        0     1153 2024-04-05 12:04:11.000000 soarv1-0.9/soar/engine/exporter.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 06:35:27.000000 soarv1-0.9/soar/engine/predictor.py
+-rw-rw-rw-   0        0        0     1805 2024-04-24 06:44:01.000000 soarv1-0.9/soar/engine/trainer.py
+-rw-rw-rw-   0        0        0     1479 2024-04-24 06:53:00.000000 soarv1-0.9/soar/engine/validator.py
+-rw-rw-rw-   0        0        0      467 2024-04-19 09:07:29.000000 soarv1-0.9/soar/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.663596 soarv1-0.9/soar/models/
+-rw-rw-rw-   0        0        0      129 2024-04-19 09:19:16.000000 soarv1-0.9/soar/models/__init__.py
+-rw-rw-rw-   0        0        0     6852 2024-04-05 09:10:11.000000 soarv1-0.9/soar/models/botnet.py
+-rw-rw-rw-   0        0        0      617 2024-04-19 09:16:23.000000 soarv1-0.9/soar/models/model.py
+-rw-rw-rw-   0        0        0     3284 2024-04-07 14:39:57.000000 soarv1-0.9/soar/models/resnet.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.670596 soarv1-0.9/soar/utils/
+-rw-rw-rw-   0        0        0      451 2024-04-24 14:48:31.000000 soarv1-0.9/soar/utils/__init__.py
+-rw-rw-rw-   0        0        0      570 2024-04-24 14:56:14.000000 soarv1-0.9/soar/utils/crypt.py
+-rw-rw-rw-   0        0        0     1361 2024-04-25 01:47:53.000000 soarv1-0.9/soar/utils/ema.py
+-rw-rw-rw-   0        0        0     3573 2024-05-14 11:39:20.000000 soarv1-0.9/soar/utils/event.py
+-rw-rw-rw-   0        0        0     1233 2024-04-19 08:01:57.000000 soarv1-0.9/soar/utils/logger.py
+-rw-rw-rw-   0        0        0      592 2024-03-27 07:30:41.000000 soarv1-0.9/soar/utils/loss.py
+-rw-rw-rw-   0        0        0     1419 2024-04-23 04:19:41.000000 soarv1-0.9/soar/utils/metric.py
+-rw-rw-rw-   0        0        0      685 2024-04-18 04:25:37.000000 soarv1-0.9/soar/utils/optimizer.py
+-rw-rw-rw-   0        0        0      897 2024-04-23 06:13:49.000000 soarv1-0.9/soar/utils/parallel.py
+-rw-rw-rw-   0        0        0      734 2024-04-06 13:49:57.000000 soarv1-0.9/soar/utils/scheduler.py
+-rw-rw-rw-   0        0        0     1443 2024-05-14 07:57:35.000000 soarv1-0.9/soar/utils/storager.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.671595 soarv1-0.9/soar/weights/
+-rw-rw-rw-   0        0        0        0 2024-05-10 05:22:40.000000 soarv1-0.9/soar/weights/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:19:40.674595 soarv1-0.9/soarv1.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-05-15 01:19:40.000000 soarv1-0.9/soarv1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2024-05-15 01:19:40.000000 soarv1-0.9/soarv1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 01:19:40.000000 soarv1-0.9/soarv1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2024-05-15 01:19:40.000000 soarv1-0.9/soarv1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 01:19:40.000000 soarv1-0.9/soarv1.egg-info/top_level.txt
```

### Comparing `soarv1-0.8/PKG-INFO` & `soarv1-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.8
+Version: 0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.8/setup.py` & `soarv1-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/config.py` & `soarv1-0.9/soar/config.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/context.py` & `soarv1-0.9/soar/context.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/datasets/augment.py` & `soarv1-0.9/soar/datasets/augment.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/datasets/dataloader.py` & `soarv1-0.9/soar/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/datasets/dataset.py` & `soarv1-0.9/soar/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/datasets/transform.py` & `soarv1-0.9/soar/datasets/transform.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/engine/exporter.py` & `soarv1-0.9/soar/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/engine/trainer.py` & `soarv1-0.9/soar/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/engine/validator.py` & `soarv1-0.9/soar/engine/validator.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/models/botnet.py` & `soarv1-0.9/soar/models/botnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/models/model.py` & `soarv1-0.9/soar/models/model.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/models/resnet.py` & `soarv1-0.9/soar/models/resnet.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/crypt.py` & `soarv1-0.9/soar/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/ema.py` & `soarv1-0.9/soar/utils/ema.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/event.py` & `soarv1-0.9/soar/utils/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
         process = Popen(cmd)
         time.sleep(5)
         return process
 
     def reload(self, result):
         metrics = result.to_dict()
         for key, value in metrics.items():
-            self.metrics[key] = list(value.values())
-
-        epochs = self.metrics["epoch"]
+            metrics[key] = list(value.values())
+        self.metrics = copy.deepcopy(metrics)
+        epochs = metrics.pop("epoch")
         for epoch in epochs:
             for name, metric in metrics.items():
                 self.writer.add_scalar(name, metric[epoch-1], epoch)
 
         # concat tensorboard output
         # event_list = []
         # for event_name in os.listdir(self.storager.save_path):
```

### Comparing `soarv1-0.8/soar/utils/logger.py` & `soarv1-0.9/soar/utils/logger.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/loss.py` & `soarv1-0.9/soar/utils/loss.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/metric.py` & `soarv1-0.9/soar/utils/metric.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/optimizer.py` & `soarv1-0.9/soar/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/parallel.py` & `soarv1-0.9/soar/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/scheduler.py` & `soarv1-0.9/soar/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soar/utils/storager.py` & `soarv1-0.9/soar/utils/storager.py`

 * *Files identical despite different names*

### Comparing `soarv1-0.8/soarv1.egg-info/PKG-INFO` & `soarv1-0.9/soarv1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soarv1
-Version: 0.8
+Version: 0.9
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `soarv1-0.8/soarv1.egg-info/SOURCES.txt` & `soarv1-0.9/soarv1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

