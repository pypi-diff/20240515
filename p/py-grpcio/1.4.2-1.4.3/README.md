# Comparing `tmp/py_grpcio-1.4.2.tar.gz` & `tmp/py_grpcio-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.4.2.tar", max compression
+gzip compressed data, was "py_grpcio-1.4.3.tar", max compression
```

## Comparing `py_grpcio-1.4.2.tar` & `py_grpcio-1.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1076 2024-05-13 20:40:40.706689 py_grpcio-1.4.2/LICENSE
--rw-r--r--   0        0        0     4581 2024-05-13 20:40:40.706689 py_grpcio-1.4.2/README.md
--rw-r--r--   0        0        0      167 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/__init__.py
--rw-r--r--   0        0        0      796 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1961 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     5102 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/method.py
--rw-r--r--   0        0        0     1148 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/middleware.py
--rw-r--r--   0        0        0     4810 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3818 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      687 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     1921 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/service.py
--rw-r--r--   0        0        0     2727 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-13 20:40:40.710689 py_grpcio-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-15 21:28:04.496798 py_grpcio-1.4.3/LICENSE
+-rw-r--r--   0        0        0     4581 2024-05-15 21:28:04.496798 py_grpcio-1.4.3/README.md
+-rw-r--r--   0        0        0      167 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/__init__.py
+-rw-r--r--   0        0        0      796 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1961 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     5102 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/method.py
+-rw-r--r--   0        0        0     1148 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/middleware.py
+-rw-r--r--   0        0        0     5421 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3882 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      686 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     1921 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/server.py
+-rw-r--r--   0        0        0      924 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/service.py
+-rw-r--r--   0        0        0     2727 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-15 21:28:04.500798 py_grpcio-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.4.3/PKG-INFO
```

### Comparing `py_grpcio-1.4.2/LICENSE` & `py_grpcio-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/README.md` & `py_grpcio-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/exceptions.py` & `py_grpcio-1.4.3/py_grpcio/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/interceptor.py` & `py_grpcio-1.4.3/py_grpcio/interceptor.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/method.py` & `py_grpcio-1.4.3/py_grpcio/method.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/middleware.py` & `py_grpcio-1.4.3/py_grpcio/middleware.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/models.py` & `py_grpcio-1.4.3/py_grpcio/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from inspect import isclass
 from functools import partial
-from typing import Type, Any, TypeVar
 from typing_extensions import Annotated
-from types import FunctionType, ModuleType
+from types import FunctionType, ModuleType, GenericAlias
+from typing import Type, Any, TypeVar, Iterable, get_origin
 
 from pydantic import BaseModel, ConfigDict, Field as PyField
 from pydantic.fields import FieldInfo  # noqa: FieldInfo
 from pydantic_core.core_schema import CoreSchema, no_info_wrap_validator_function, str_schema, to_string_ser_schema
 
 from google.protobuf.message import Message as ProtoMessage
 
@@ -34,24 +34,32 @@
     def fields(cls: Type['Message']) -> list[Field]:
         return [
             Field.from_field_info(field_name=field_name, field_info=field_info)
             for field_name, field_info in cls.model_fields.items()
         ]
 
     @classmethod
-    def get_additional_messages_from_fields(
-            cls, model_fields: dict[str, FieldInfo] | None = None
+    def get_additional_messages(
+        cls, model_fields: dict[str, FieldInfo] | None = None
     ) -> dict[str, Type['Message']]:
         messages: dict[str, Type[Message]] = {}
         for field_name, field_info in (model_fields and model_fields.items()) or cls.model_fields.items():
             field_type: type | None = field_info.annotation
             if isclass(field_type) and issubclass(field_type, Message):
                 messages[field_type.__name__]: Type[Message] = field_type
-                if additional_messages := cls.get_additional_messages_from_fields(model_fields=field_type.model_fields):
+                if additional_messages := cls.get_additional_messages(model_fields=field_type.model_fields):
                     messages.update(**additional_messages)
+            elif isinstance(field_type, GenericAlias) and (origin := get_origin(tp=field_type)) is not None:
+                if issubclass(origin, Iterable):
+                    if len(args := field_type.__args__) != 1:
+                        raise
+                    if isclass(sub_field_type := args[0]) and issubclass(sub_field_type, Message):
+                        messages[sub_field_type.__name__]: Type[Message] = sub_field_type
+                        if additional_messages := cls.get_additional_messages(model_fields=sub_field_type.model_fields):
+                            messages.update(**additional_messages)
         return messages
 
 
 class ModuleTypePydanticAnnotation:
     @classmethod
     def validate_object_id(cls: Type['ModuleTypePydanticAnnotation'], value: Any, _) -> ModuleType:
         if isinstance(value, ModuleType):
@@ -88,16 +96,16 @@
             raise MethodSignatureException(
                 text=f'The `{target.__qualname__}` method should return an object of type subclass `Message`'
             )
         return cls(target=partial(target, self=target.__class__), request=requst_message, response=response_message)
 
     @property
     def messages(self: 'Method') -> dict[str, Type[Message]]:
-        self.additional_messages.update(self.request.get_additional_messages_from_fields())
-        self.additional_messages.update(self.response.get_additional_messages_from_fields())
+        self.additional_messages.update(self.request.get_additional_messages())
+        self.additional_messages.update(self.response.get_additional_messages())
         return {
             **self.additional_messages,
             self.request.__name__: self.request,
             self.response.__name__: self.response,
         }
 
     @property
```

### Comparing `py_grpcio-1.4.2/py_grpcio/proto/parser.py` & `py_grpcio-1.4.3/py_grpcio/proto/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from uuid import UUID
 from enum import Enum
 from inspect import isclass
 from datetime import datetime
 
 from pydantic import BaseModel
 
-from types import UnionType, NoneType
+from types import UnionType, NoneType, GenericAlias
 from typing import Any, Annotated, Union, Iterable, get_origin
 
 from py_grpcio.proto import ProtoBufTypes
 
 TYPE_MAPPING: dict[type, ProtoBufTypes] = {
     int: ProtoBufTypes.INT64,
     float: ProtoBufTypes.DOUBLE,
@@ -33,57 +33,57 @@
             args=list(python_value.__args__)
         )['type']
     elif allow_model and isclass(python_value) and issubclass(python_value, BaseModel):
         return python_value.__name__
     raise TypeError(f'Field `{field_name}`: unsupported type `{python_value}` in type `{field_type}`.')
 
 
-def parse_type_union(field_name: str, field_type: type | None, args: list) -> dict[str, Any]:
+def parse_type_union(field_name: str, field_type: type | None | GenericAlias, args: list) -> dict[str, Any]:
     if NoneType in args:
         args.remove(NoneType)
     if len(args) != 1:
         raise TypeError(
             f'Field `{field_name}`: type `{field_type}` must have only one subtype, not {len(args)}. '
             'Tip: None/Optional type ignoring.'
         )
     return {'name': field_name, 'type': parse_type(field_name=field_name, python_value=args[0], field_type=field_type)}
 
 
-def parse_type_sequence(field_name: str, field_type: type | None, args: list) -> dict[str, Any]:
+def parse_type_sequence(field_name: str, field_type: type | None | GenericAlias, args: list) -> dict[str, Any]:
     if len(args) != 1:
         raise TypeError(f'Field `{field_name}`: type `{field_type}` must have only one subtype, not {len(args)}.')
     return {
         'name': field_name,
         'type': parse_type(field_name=field_name, python_value=args[0], field_type=field_type),
         'repeated': True
     }
 
 
-def parse_type_mapping(field_name: str, field_type: type | None, args: list) -> dict[str, Any]:
+def parse_type_mapping(field_name: str, field_type: type | None | GenericAlias, args: list) -> dict[str, Any]:
     if len(args) != 2:
         raise TypeError(f'Field `{field_name}`: type `{field_type}` must have two subtypes, not {len(args)}')
     return {
         'name': field_name,
         'type': ProtoBufTypes.MAP,
         'map_key': parse_type(field_name=field_name, python_value=args[0], field_type=field_type, allow_model=False),
         'map_value': parse_type(field_name=field_name, python_value=args[1], field_type=field_type)
     }
 
 
 def parse_field_type(field_name: str, field_type: type) -> dict[str, Any]:
     if proto_buf_type := TYPE_MAPPING.get(field_type):
         return {'name': field_name, 'type': proto_buf_type}
-    elif (origin := get_origin(tp=field_type)) is not None:
-        args: list = list(field_type.__args__)  # noqa: __args__
+    elif isinstance(field_type, GenericAlias) and (origin := get_origin(tp=field_type)) is not None:
+        args: list = list(field_type.__args__)
         if origin in (Union, UnionType):
             return parse_type_union(field_name=field_name, field_type=field_type, args=args)
         if issubclass(origin, dict):
             return parse_type_mapping(field_name=field_name, field_type=field_type, args=args)
-        if issubclass(origin, Iterable):  # noqa: origin
+        if issubclass(origin, Iterable):
             return parse_type_sequence(field_name=field_name, field_type=field_type, args=args)
         raise TypeError(f'Field unsupported type `{field_type}`')
     elif isclass(field_type):
         if issubclass(field_type, BaseModel):
             return {'name': field_name, 'type': field_type.__name__}
-        elif issubclass(field_type, Enum):
+        if issubclass(field_type, Enum):
             return {'name': field_name, 'type': ProtoBufTypes.STRING}
     raise TypeError(f'Field unsupported type `{field_type}`')
```

### Comparing `py_grpcio-1.4.2/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.4.3/py_grpcio/proto/templates/service.proto.template`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 {% for field in message.fields() %}
     {% if field.repeated %}repeated {% endif -%}
     {% if field.type == "map" %}map<{{ field.map_key }}, {{ field.map_value }}> {% else %}{{ field.type }} {% endif -%}
     {{ field.name }} = {{ loop.index0 + 1 }};
 {% endfor %}
 }
 
-{% endfor %}
+{% endfor %}
```

### Comparing `py_grpcio-1.4.2/py_grpcio/server.py` & `py_grpcio-1.4.3/py_grpcio/server.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/service.py` & `py_grpcio-1.4.3/py_grpcio/service.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/service_meta.py` & `py_grpcio-1.4.3/py_grpcio/service_meta.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/py_grpcio/utils.py` & `py_grpcio-1.4.3/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.4.2/pyproject.toml` & `py_grpcio-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.4.2"
+version = "1.4.3"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.4.2/PKG-INFO` & `py_grpcio-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.4.2
+Version: 1.4.3
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

