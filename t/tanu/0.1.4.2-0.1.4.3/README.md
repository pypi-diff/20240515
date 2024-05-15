# Comparing `tmp/tanu-0.1.4.2.tar.gz` & `tmp/tanu-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanu-0.1.4.2.tar", last modified: Mon May 13 10:37:33 2024, max compression
+gzip compressed data, was "tanu-0.1.4.3.tar", last modified: Wed May 15 06:13:27 2024, max compression
```

## Comparing `tanu-0.1.4.2.tar` & `tanu-0.1.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:37:33.045909 tanu-0.1.4.2/
--rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.4.2/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.4.2/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-13 10:37:33.045842 tanu-0.1.4.2/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.4.2/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.4.2/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      720 2024-05-13 10:37:33.046177 tanu-0.1.4.2/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.4.2/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:37:33.041418 tanu-0.1.4.2/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:37:33.043314 tanu-0.1.4.2/src/tanu/
--rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.4.2/src/tanu/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    17941 2024-05-13 10:37:21.000000 tanu-0.1.4.2/src/tanu/tanu.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:37:33.045312 tanu-0.1.4.2/src/tanu/utils/
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.4.2/src/tanu/utils/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.4.2/src/tanu/utils/object_encoder_decoder.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:37:33.045616 tanu-0.1.4.2/src/tanu.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-13 10:37:33.000000 tanu-0.1.4.2/src/tanu.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-13 10:37:33.000000 tanu-0.1.4.2/src/tanu.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-13 10:37:33.000000 tanu-0.1.4.2/src/tanu.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       47 2024-05-13 10:37:33.000000 tanu-0.1.4.2/src/tanu.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-13 10:37:33.000000 tanu-0.1.4.2/src/tanu.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 06:13:27.608486 tanu-0.1.4.3/
+-rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.4.3/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.4.3/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-15 06:13:27.608422 tanu-0.1.4.3/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.4.3/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.4.3/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      720 2024-05-15 06:13:27.608782 tanu-0.1.4.3/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.4.3/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 06:13:27.604791 tanu-0.1.4.3/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 06:13:27.606708 tanu-0.1.4.3/src/tanu/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.4.3/src/tanu/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    18425 2024-05-15 06:09:24.000000 tanu-0.1.4.3/src/tanu/tanu.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 06:13:27.607764 tanu-0.1.4.3/src/tanu/utils/
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.4.3/src/tanu/utils/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.4.3/src/tanu/utils/object_encoder_decoder.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-15 06:13:27.608187 tanu-0.1.4.3/src/tanu.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-15 06:13:27.000000 tanu-0.1.4.3/src/tanu.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-15 06:13:27.000000 tanu-0.1.4.3/src/tanu.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-15 06:13:27.000000 tanu-0.1.4.3/src/tanu.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       47 2024-05-15 06:13:27.000000 tanu-0.1.4.3/src/tanu.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-15 06:13:27.000000 tanu-0.1.4.3/src/tanu.egg-info/top_level.txt
```

### Comparing `tanu-0.1.4.2/LICENSE.txt` & `tanu-0.1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tanu-0.1.4.2/PKG-INFO` & `tanu-0.1.4.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.4.2
+Version: 0.1.4.3
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tanu-0.1.4.2/setup.cfg` & `tanu-0.1.4.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tanu
-version = 0.1.4.2
+version = 0.1.4.3
 author = chocolate-icecream
 description = Message passing between Python programs via RabbitMQ.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `tanu-0.1.4.2/src/tanu/tanu.py` & `tanu-0.1.4.3/src/tanu/tanu.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,21 @@
 
     def start_consumer(self):
         """Continuously consume results from the result queue."""
         connection = pika.BlockingConnection(pika.ConnectionParameters(host=self.host, port=self.port))
         channel = connection.channel()
         channel.queue_declare(queue=self.result_queue_name)
         channel.basic_consume(queue=self.result_queue_name, auto_ack=True, on_message_callback=self.on_result_received)
-        channel.start_consuming()
+        try:
+            channel.start_consuming()
+        except pika.exceptions.StreamLossError:
+            t = threading.Thread(target=self.start_consumer)
+            t.daemon = True
+            t.start()
+
 
     def on_result_received(self, ch, method, properties, body):
         """Handle received results and trigger callback if set."""
         try:
             response = ResponseLetter.parse_raw(body)
             apply_decoder(response)
             if response.job_id in self.result_queues:
@@ -325,22 +331,30 @@
 
         self.command_dict = {}
         self.units = {}
     
     def run(self):
         """Start consuming tasks from the queue."""
         queue_name = f"task_{self.name}"
-        self.connection_for_task_queue = pika.BlockingConnection(pika.ConnectionParameters(host=self.host, port=self.port))
-        self.base_response_connection = TanukiResponseConnection(self, units=self.units)
-        channel = self.connection_for_task_queue.channel()
-        channel.queue_declare(queue=queue_name, durable=True)
-        channel.basic_qos(prefetch_count=1)
-        channel.basic_consume(queue=queue_name, on_message_callback=self._call_command)
-        logger.info(f"{self.name} starts running...")
-        channel.start_consuming()
+        while True:
+            self.connection_for_task_queue = pika.BlockingConnection(pika.ConnectionParameters(host=self.host, port=self.port))
+            self.base_response_connection = TanukiResponseConnection(self, units=self.units)
+            channel = self.connection_for_task_queue.channel()
+            channel.queue_declare(queue=queue_name, durable=True)
+            channel.basic_qos(prefetch_count=1)
+            channel.basic_consume(queue=queue_name, on_message_callback=self._call_command)
+            logger.info(f"{self.name} starts running...")
+            try:
+                channel.start_consuming()
+            except KeyboardInterrupt:
+                break
+            except pika.exceptions.StreamLostError:
+                logger.warning(f"Stream Lost Error while consuming queue {queue_name}")
+                pass
+            
 
     def _call_command(self, ch_req, method, properties, body):
         """Process incoming command requests."""
         try:
             request = RequestLetter.parse_raw(body)
             if request.command not in self.command_dict:
                 TanukiResponseConnection.send_error(self, request, f"Tanuki Worker {self.name} cannot recognize '{request.command}'.")
```

### Comparing `tanu-0.1.4.2/src/tanu/utils/object_encoder_decoder.py` & `tanu-0.1.4.3/src/tanu/utils/object_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `tanu-0.1.4.2/src/tanu.egg-info/PKG-INFO` & `tanu-0.1.4.3/src/tanu.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.4.2
+Version: 0.1.4.3
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

