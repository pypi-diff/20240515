# Comparing `tmp/ebb_events-0.3.1.tar.gz` & `tmp/ebb_events-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_events-0.3.1.tar", max compression
+gzip compressed data, was "ebb_events-0.3.2.tar", max compression
```

## Comparing `ebb_events-0.3.1.tar` & `ebb_events-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.1/LICENSE
--rw-r--r--   0        0        0     8842 2024-05-14 16:56:47.897263 ebb_events-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.1/ebb_events/__init__.py
--rw-r--r--   0        0        0     8308 2024-05-14 16:56:47.897743 ebb_events-0.3.1/ebb_events/builders/event_builder.py
--rw-r--r--   0        0        0     9364 2024-05-14 17:13:18.576368 ebb_events-0.3.1/ebb_events/consumers/event_consumer.py
--rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.1/ebb_events/enums.py
--rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.3.1/ebb_events/event_payload_utils.py
--rw-r--r--   0        0        0     2668 2024-05-13 20:48:51.509330 ebb_events-0.3.1/ebb_events/event_schema.py
--rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.1/ebb_events/exceptions.py
--rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.1/ebb_events/field_constants.py
--rw-r--r--   0        0        0      571 2024-05-14 17:13:18.576796 ebb_events-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 ebb_events-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8842 2024-05-14 16:56:47.897263 ebb_events-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.2/ebb_events/__init__.py
+-rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.2/ebb_events/builders/event_builder.py
+-rw-r--r--   0        0        0    10366 2024-05-15 20:31:26.931154 ebb_events-0.3.2/ebb_events/consumers/event_consumer.py
+-rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.2/ebb_events/enums.py
+-rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.3.2/ebb_events/event_payload_utils.py
+-rw-r--r--   0        0        0     2668 2024-05-13 20:48:51.509330 ebb_events-0.3.2/ebb_events/event_schema.py
+-rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.2/ebb_events/exceptions.py
+-rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.2/ebb_events/field_constants.py
+-rw-r--r--   0        0        0      571 2024-05-15 20:31:26.931473 ebb_events-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 ebb_events-0.3.2/PKG-INFO
```

### Comparing `ebb_events-0.3.1/LICENSE` & `ebb_events-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.1/README.md` & `ebb_events-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.1/ebb_events/builders/event_builder.py` & `ebb_events-0.3.2/ebb_events/builders/event_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from datetime import datetime, timezone
 import json
+import logging
+
+from datetime import datetime, timezone
+from marshmallow import ValidationError
 from typing import Optional
 from uuid import uuid4
 
-from marshmallow import ValidationError
 from ebb_events.field_constants import (
     DATA,
     ID,
     METADATA,
     SOURCE,
     TIME,
     TYPE,
@@ -58,14 +60,15 @@
         Return: None if valid fields
         Raises: TopicFormatException for invalid fields
         """
         envelope_schema = EventEnvelopeSchema()
         errors = envelope_schema.validate(envelope_schema.dump(self))
         if errors:
             # errors will be a dictionary of validation errors
+            logging.error("Invalid EventEnvelope", extra={"errors": errors})
             raise TopicFormatException(errors)
 
     def _format_time(self, datetime_raw: Optional[datetime] = None) -> str:
         """
         Helper takes in datetime object or None and returns the string datetime in RFC3339 format UTC.
         If None - timestamp is datetime.now().
 
@@ -87,14 +90,15 @@
         Note: Fields are validated in __init__ so no need to re-validate here.
         Returns:
             str: _description_
         """
         topic = f"{self.organization}/{self.system_id}/{self.event_type}/{self.subsystem_id}/{self.device_id}"
         # This should be enforced by the ._validate() call and the EventEnvelopeSchema too
         if len(topic) > 256:
+            logging.error(f"Invalid Topic. Topic too long: {topic}.")
             raise TopicFormatException("Topic length cannot exceed 256 characters.")
         return topic
 
     def build_event_payload_dict(
         self,
         message: dict,
         serial_number: str = None,
@@ -124,14 +128,17 @@
         Exceptions:
             Raises 'PayloadFormatException' if the topic or message does not meet the expected format.
         """
         if serial_number is not None:
             metadata[SERIAL_NUMBER] = str(serial_number)
         payload_schema = EventPayloadSchema(context={"remove_nones": remove_nones})
         if datetime_obj is not None and type(datetime_obj) is not datetime:
+            logging.error(
+                f"Invalid datetime_obj: {datetime_obj} must be of type datetime."
+            )
             raise PayloadFormatException(
                 "datetime_obj must be a valid datetime object."
             )
         try:
             event_payload = {
                 ID: uuid4(),
                 TIME: self._format_time(datetime_raw=datetime_obj),
@@ -143,24 +150,29 @@
             json.dumps(message)
             json.dumps(metadata)
             deserialized_payload = payload_schema.load(
                 data=event_payload
             )  # validates event_payload against schema
         except TopicFormatException:
             # Exception raised by build_event_topic() if too long
+            # logging.error called at source of the TopicFormatException raised
             raise PayloadFormatException(
                 "Source and topic must be less than 256 characters."
             )
         except ValidationError as error:
-            # Exception raised by json.dumps() if not valid json serializable object
+            # Exception raised by schema.load() if not valid marshmallow schema
+            logging.error(
+                f"Invalid payload. Does not match marshmallow schema: {str(error)}"
+            )
             raise PayloadFormatException(
                 f"Payload does not match required format: {str(error)}"
             )
-        except TypeError:
+        except TypeError as error:
             # Exception raised by json.dumps() if not valid json serializable object
+            logging.error(f"Invalid payload, not JSON serializable: {str(error)}")
             raise PayloadFormatException(
                 "Payload message and metadata must be JSON serializable dictionaries."
             )
         return payload_schema.dump(deserialized_payload)
 
     def build_event_payload_json(
         self,
```

### Comparing `ebb_events-0.3.1/ebb_events/consumers/event_consumer.py` & `ebb_events-0.3.2/ebb_events/consumers/event_consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import logging
 from datetime import datetime
 from marshmallow import ValidationError
 from ebb_events.field_constants import (
     DATA,
     ID,
     METADATA,
     SERIAL_NUMBER,
@@ -20,14 +21,17 @@
     Class to consume and parse events that follow the ebb_event structure
     """
 
     def __init__(self, payload: dict = {}) -> None:
         """
         Initializes an EventConsumer object with payload data
         """
+        self.error_log_message = (
+            "Error fetching %s. Invalid payload, not an ebb-event structure."
+        )
         self.raw_payload: dict = payload
         self.is_ebb_event_structure: bool = self.check_is_ebb_event_structure(
             payload=self.raw_payload
         )
 
     def check_is_ebb_event_structure(self, payload: dict) -> bool:
         """
@@ -48,56 +52,60 @@
             PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
             str: event's string id.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(ID))
+        logging.error(self.error_log_message % "event_id")
         raise PayloadFormatException()
 
     def get_event_time_str(self) -> str:
         """
         Helper to fetch event's time field in RFC3339 format: YYYY-MM-DDThh:mm:ss.ssssss+/-hh:mm
 
         Raises:
             PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
             str: event's time field.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(TIME))
+        logging.error(self.error_log_message % "event_time_str")
         raise PayloadFormatException()
 
     def get_event_time(self) -> datetime:
         """
         Helper to fetch event's time field as python datetime object.
 
         Raises:
             PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
             datetime: event's time field.
         """
         if self.is_ebb_event_structure:
             return datetime.fromisoformat(self.raw_payload.get(TIME))
+        logging.error(self.error_log_message % "event_time")
         raise PayloadFormatException()
 
     def get_event_source(self) -> str:
         """
         Helper to fetch event's source as string. For ebb_events, the `source` field matches the MQTT `topic`.
 
         Raises:
             PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
             str: event's source field.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(SOURCE))
+        logging.error(self.error_log_message % "event_source/event_topic")
         raise PayloadFormatException()
 
     def get_event_topic(self) -> str:
         """
         Helper to fetch event's topic string. For ebb_events, the MQTT `topic` field matches the event's source.
 
         Raises:
@@ -116,14 +124,15 @@
             PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
             str: event's type field.
         """
         if self.is_ebb_event_structure:
             return str(self.raw_payload.get(TYPE))
+        logging.error(self.error_log_message % "event_type")
         raise PayloadFormatException()
 
     def get_event_organization(self) -> str:
         """
         Helper to fetch event's organization portion of topic hierarchy as string.
         This is the top level of the topic hierarchy.
 
@@ -133,14 +142,15 @@
         Returns:
             str: event's organization portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[0]
+        logging.error(self.error_log_message % "event_organization")
         raise PayloadFormatException()
 
     def get_event_system_id(self) -> str:
         """
         Helper to fetch event's system_id portion of topic hierarchy as string.
         This is the second level of the topic hierarchy.
 
@@ -150,14 +160,15 @@
         Returns:
             str: event's system_id portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[1]
+        logging.error(self.error_log_message % "event_system_id")
         raise PayloadFormatException()
 
     def get_event_subsystem_id(self) -> str:
         """
         Helper to fetch event's subsystem_id portion of topic hierarchy as string.
         This is the fourth level of the topic hierarchy.
 
@@ -167,14 +178,15 @@
         Returns:
             str: event's subsystem_id portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[3]
+        logging.error(self.error_log_message % "event_subsystem_id")
         raise PayloadFormatException()
 
     def get_event_device_id(self) -> str:
         """
         Helper to fetch event's device_id portion of topic hierarchy as string.
         This is the fourth level of the topic hierarchy.
 
@@ -184,14 +196,15 @@
         Returns:
             str: event's device_id portion of the topic hierarchy.
         """
         # This ensures that the `source` field matches the expected topic structure
         if self.is_ebb_event_structure:
             topic_list = self.raw_payload.get(SOURCE).split("/")
             return topic_list[4]
+        logging.error(self.error_log_message % "event_device_id")
         raise PayloadFormatException()
 
     def get_event_envelope(self) -> EventEnvelope:
         """
         Helper to build and return EventEnvelope from payload.
 
         Raises:
@@ -204,14 +217,15 @@
             return EventEnvelope(
                 organization=self.get_event_organization(),
                 system_id=self.get_event_system_id(),
                 event_type=self.get_event_type(),
                 subsystem_id=self.get_event_subsystem_id(),
                 device_id=self.get_event_device_id(),
             )
+        logging.error(self.error_log_message % "event_envelope")
         raise PayloadFormatException()
 
     def get_event_message(self, metadata_included=True) -> dict:
         """
         Helper fetches and returns message dict from payload.
         Metadata field in the message dict is included by default but can be parsed out.
 
@@ -227,28 +241,30 @@
         """
         if self.is_ebb_event_structure:
             # Copy of message so that we don't actually alter the raw_payload itself
             message: dict = copy.deepcopy(self.raw_payload.get(DATA))
             if not metadata_included:
                 message.pop(METADATA, {})
             return message
+        logging.error(self.error_log_message % "event_message")
         raise PayloadFormatException()
 
     def get_event_message_metadata(self) -> dict:
         """
         Helper to fetch and return the metadata dictionary within the payload's event message.
 
         Raises:
             PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
             dict: Metadata included in event message.
         """
         if self.is_ebb_event_structure:
             return self.raw_payload.get(DATA, {}).get(METADATA, {})
+        logging.error(self.error_log_message % "event_message_metadata")
         raise PayloadFormatException()
 
     def get_device_serial_number(self) -> str:
         """
         Helper to fetch and return the serial number of the publishing device as a string.
         Pulls this information from the metadata of the event message.
 
@@ -262,8 +278,9 @@
             if (
                 ser_num := self.raw_payload.get(DATA, {})
                 .get(METADATA, {})
                 .get(SERIAL_NUMBER, None)
             ):
                 return str(ser_num)
             return None
+        logging.error(self.error_log_message % "device_serial_number")
         raise PayloadFormatException()
```

### Comparing `ebb_events-0.3.1/ebb_events/event_schema.py` & `ebb_events-0.3.2/ebb_events/event_schema.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.1/pyproject.toml` & `ebb_events-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-events"
-version = "0.3.1"
+version = "0.3.2"
 description = "Package for building and standardizing MQTT event messages."
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 marshmallow = "^3.21.1"
```

### Comparing `ebb_events-0.3.1/PKG-INFO` & `ebb_events-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-events
-Version: 0.3.1
+Version: 0.3.2
 Summary: Package for building and standardizing MQTT event messages.
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

