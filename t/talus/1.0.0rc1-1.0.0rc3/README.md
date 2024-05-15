# Comparing `tmp/talus-1.0.0rc1.tar.gz` & `tmp/talus-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-1.0.0rc1.tar", last modified: Tue May 14 21:46:30 2024, max compression
+gzip compressed data, was "talus-1.0.0rc3.tar", last modified: Wed May 15 21:08:19 2024, max compression
```

## Comparing `talus-1.0.0rc1.tar` & `talus-1.0.0rc3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.158894 talus-1.0.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-14 21:46:18.000000 talus-1.0.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-14 21:46:18.000000 talus-1.0.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-14 21:46:18.000000 talus-1.0.0rc1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-14 21:46:18.000000 talus-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-14 21:46:30.158894 talus-1.0.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-14 21:46:18.000000 talus-1.0.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-14 21:46:18.000000 talus-1.0.0rc1/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-14 21:46:18.000000 talus-1.0.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-14 21:46:30.158894 talus-1.0.0rc1/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.154894 talus-1.0.0rc1/talus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/consumer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.154894 talus-1.0.0rc1/talus/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/binding.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3969 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/models/retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.154894 talus-1.0.0rc1/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.158894 talus-1.0.0rc1/talus/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_binding.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3949 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_processor.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/models/test_retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-14 21:46:18.000000 talus-1.0.0rc1/talus/tests/test_producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-14 21:46:30.158894 talus-1.0.0rc1/talus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-14 21:46:29.000000 talus-1.0.0rc1/talus.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-14 21:46:30.000000 talus-1.0.0rc1/talus.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-14 21:46:18.000000 talus-1.0.0rc1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:08:19.632459 talus-1.0.0rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-15 21:08:04.000000 talus-1.0.0rc3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-15 21:08:04.000000 talus-1.0.0rc3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-15 21:08:04.000000 talus-1.0.0rc3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-15 21:08:04.000000 talus-1.0.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-15 21:08:19.632459 talus-1.0.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-15 21:08:04.000000 talus-1.0.0rc3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-15 21:08:04.000000 talus-1.0.0rc3/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-15 21:08:04.000000 talus-1.0.0rc3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-15 21:08:19.632459 talus-1.0.0rc3/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:08:19.628459 talus-1.0.0rc3/talus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-15 21:08:19.000000 talus-1.0.0rc3/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:08:19.628459 talus-1.0.0rc3/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:08:19.632459 talus-1.0.0rc3/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:08:19.632459 talus-1.0.0rc3/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-15 21:08:04.000000 talus-1.0.0rc3/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:08:19.632459 talus-1.0.0rc3/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-15 21:08:19.000000 talus-1.0.0rc3/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-15 21:08:19.000000 talus-1.0.0rc3/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-15 21:08:19.000000 talus-1.0.0rc3/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-15 21:08:19.000000 talus-1.0.0rc3/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-15 21:08:19.000000 talus-1.0.0rc3/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-15 21:08:19.000000 talus-1.0.0rc3/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-15 21:08:04.000000 talus-1.0.0rc3/tox.ini
```

### Comparing `talus-1.0.0rc1/.gitignore` & `talus-1.0.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/.pre-commit-config.yaml` & `talus-1.0.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/LICENSE` & `talus-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/PKG-INFO` & `talus-1.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc1
+Version: 1.0.0rc3
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc1/README.rst` & `talus-1.0.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/bitbucket-pipelines.yml` & `talus-1.0.0rc3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/pyproject.toml` & `talus-1.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/base.py` & `talus-1.0.0rc3/talus/base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/consumer.py` & `talus-1.0.0rc3/talus/consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/models/binding.py` & `talus-1.0.0rc3/talus/models/binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/models/connection_parameters.py` & `talus-1.0.0rc3/talus/models/connection_parameters.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/models/message.py` & `talus-1.0.0rc3/talus/models/message.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,50 +6,52 @@
 
 import pika.spec
 from pydantic import BaseModel
 from pydantic import ConfigDict
 from pydantic import Field
 
 
-class MessageSchemaBase(BaseModel):
+class MessageBodySchemaBase(BaseModel):
     """
     Base class for message schemas which can be used to validate message bodies.
     """
 
     model_config = ConfigDict(extra="allow")
 
     conversation_id: str = Field(default_factory=lambda: uuid.uuid4().hex, alias="conversationId")
 
 
 class MessageBase:
     """
     Base class for messages establishing a common interface for use by DurableConnections
     """
 
-    message_schema_cls: Type[MessageSchemaBase] = MessageSchemaBase
+    message_body_schema_cls: Type[MessageBodySchemaBase] = MessageBodySchemaBase
 
-    def __init__(self, routing_key: str, body: bytes | dict | str | MessageSchemaBase):
+    def __init__(self, routing_key: str, body: bytes | dict | str | MessageBodySchemaBase):
         self.routing_key = routing_key
         if isinstance(body, dict | BaseModel):
-            self.body: MessageSchemaBase = self.message_schema_cls.model_validate(body)
+            self.body: MessageBodySchemaBase = self.message_body_schema_cls.model_validate(body)
         else:  # str | bytes
-            self.body: MessageSchemaBase = self.message_schema_cls.model_validate_json(body)
+            self.body: MessageBodySchemaBase = self.message_body_schema_cls.model_validate_json(
+                body
+            )
 
 
 class ConsumeMessageBase(MessageBase):
     """
     Base class for messages consumed from a DurableConsumer MessageProcessor.
     TODO example of how to use this class
     """
 
     def __init__(
         self,
         method: pika.spec.Basic.Deliver,
         properties: pika.spec.BasicProperties,
-        body: bytes | dict | str | MessageSchemaBase,
+        body: bytes | dict | str | MessageBodySchemaBase,
     ):
         super().__init__(method.routing_key, body)
         self.method = method
         self.properties = properties
 
     @property
     def delivery_tag(self):
@@ -66,15 +68,15 @@
     """
 
     routing_key: str = "default.m"
     headers: dict[str, str] | None = (None,)
 
     def __init__(
         self,
-        body: bytes | dict | str | MessageSchemaBase,
+        body: bytes | dict | str | MessageBodySchemaBase,
     ):
         super().__init__(self.routing_key, body)
 
     @property
     def properties(self) -> pika.spec.BasicProperties:
         return pika.BasicProperties(
             content_type="text/plain",
```

### Comparing `talus-1.0.0rc1/talus/models/processor.py` & `talus-1.0.0rc3/talus/models/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def dlq_message(
         cls,
         channel: pika.adapters.blocking_connection.BlockingChannel,
         method: pika.spec.Basic.Deliver,
         properties: pika.spec.BasicProperties,
         exception: Exception | None = None,
     ) -> None:
-        logger.error(f"Dead lettering message:{method=}, {properties=}, {exception=}")
+        logger.warning(f"Dead lettering message:{method=}, {properties=}, {exception=}")
         channel.basic_nack(delivery_tag=method.delivery_tag, requeue=False)
 
     @classmethod
     def acknowledge_message(
         cls, channel: pika.adapters.blocking_connection.BlockingChannel, message: ConsumeMessageBase
     ) -> None:
         logger.debug(
```

### Comparing `talus-1.0.0rc1/talus/models/retryer.py` & `talus-1.0.0rc3/talus/models/retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/producer.py` & `talus-1.0.0rc3/talus/producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/tests/conftest.py` & `talus-1.0.0rc3/talus/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 from talus.consumer import DurableConsumer
 from talus.models.binding import Binding
 from talus.models.connection_parameters import ConsumerConnectionParameterFactory
 from talus.models.connection_parameters import ProducerConnectionParameterFactory
 from talus.models.exchange import Exchange
 from talus.models.message import ConsumeMessageBase
-from talus.models.message import MessageSchemaBase
+from talus.models.message import MessageBodySchemaBase
 from talus.models.message import PublishMessageBase
 from talus.models.queue import Queue
 from talus.models.retryer import ConnectionRetryerFactory
 from talus.models.retryer import RetryerFactory
 from talus.producer import DurableProducer
 
 
 @pytest.fixture()
-def message_data_schema_cls() -> Type[MessageSchemaBase]:
-    class MessageDataSchema(MessageSchemaBase):
+def message_data_schema_cls() -> Type[MessageBodySchemaBase]:
+    class MessageDataBodySchema(MessageBodySchemaBase):
         key: str = Field(default="value")
 
-    return MessageDataSchema
+    return MessageDataBodySchema
 
 
 @pytest.fixture(params=["no-conversation-id", "conversation-id"])
 def message_data(request, message_data_schema_cls) -> dict[str, str]:
     result = message_data_schema_cls(key=uuid4().hex).model_dump()
     match request.param:
         case "no-conversation-id":
@@ -100,15 +100,15 @@
 
 
 @pytest.fixture()
 def consume_message_cls(message_data_schema_cls) -> Type[ConsumeMessageBase]:
     """A test consume message class."""
 
     class ConsumeMessage(ConsumeMessageBase):
-        message_schema_cls = message_data_schema_cls
+        message_body_schema_cls = message_data_schema_cls
 
     return ConsumeMessage
 
 
 @pytest.fixture
 def publish_message_cls(routing_key, headers) -> Type[PublishMessageBase]:
     """A test publish message class."""
```

### Comparing `talus-1.0.0rc1/talus/tests/models/test_binding.py` & `talus-1.0.0rc3/talus/tests/models/test_binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/tests/models/test_message.py` & `talus-1.0.0rc3/talus/tests/models/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 import pika
 import pydantic_core
 import pytest
 
 from talus.models.message import ConsumeMessageBase
-from talus.models.message import MessageSchemaBase
+from talus.models.message import MessageBodySchemaBase
 from talus.models.message import PublishMessageBase
 
 
 def test_consume_message_model_valid(
     method, properties, body, routing_key, headers, delivery_tag, message_data
 ):
     """
@@ -35,21 +35,21 @@
     serialized_message_dict = json.loads(message.body.model_dump_json(by_alias=True))
     assert serialized_message_dict["conversationId"] == message.body.conversation_id
     assert (
         serialized_message_dict == {"conversationId": message.body.conversation_id} | message_data
     )
 
 
-class ExampleMessageSchema(MessageSchemaBase):
+class ExampleMessageBodySchema(MessageBodySchemaBase):
     required_str: str
     required_int: int
 
 
 class ConsumableMessage(ConsumeMessageBase):
-    message_schema_cls = ExampleMessageSchema
+    message_body_schema_cls = ExampleMessageBodySchema
 
 
 @pytest.mark.parametrize(
     "invalid_body",
     [
         pytest.param(
             json.dumps({"required_str": 1, "required_int": "zz"}).encode("utf-8"),
@@ -90,15 +90,15 @@
     assert serialized_message_dict["conversationId"] == message.body.conversation_id
     assert (
         serialized_message_dict == {"conversationId": message.body.conversation_id} | message_data
     )
 
 
 class PublishMessage(PublishMessageBase):
-    message_schema_cls = ExampleMessageSchema
+    message_body_schema_cls = ExampleMessageBodySchema
     routing_key = "test.m"
 
 
 @pytest.mark.parametrize(
     "invalid_body",
     [
         pytest.param(
```

### Comparing `talus-1.0.0rc1/talus/tests/models/test_processor.py` & `talus-1.0.0rc3/talus/tests/models/test_processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/tests/models/test_queue.py` & `talus-1.0.0rc3/talus/tests/models/test_queue.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/tests/models/test_retryer.py` & `talus-1.0.0rc3/talus/tests/models/test_retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/tests/test_base.py` & `talus-1.0.0rc3/talus/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/tests/test_consumer.py` & `talus-1.0.0rc3/talus/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus/tests/test_producer.py` & `talus-1.0.0rc3/talus/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/talus.egg-info/PKG-INFO` & `talus-1.0.0rc3/talus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc1
+Version: 1.0.0rc3
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc1/talus.egg-info/SOURCES.txt` & `talus-1.0.0rc3/talus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc1/tox.ini` & `talus-1.0.0rc3/tox.ini`

 * *Files identical despite different names*

