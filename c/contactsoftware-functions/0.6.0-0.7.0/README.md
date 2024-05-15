# Comparing `tmp/contactsoftware_functions-0.6.0.tar.gz` & `tmp/contactsoftware_functions-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contactsoftware_functions-0.6.0.tar", max compression
+gzip compressed data, was "contactsoftware_functions-0.7.0.tar", max compression
```

## Comparing `contactsoftware_functions-0.6.0.tar` & `contactsoftware_functions-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1078 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/LICENSE
--rw-r--r--   0        0        0     2617 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/README.md
--rw-r--r--   0        0        0      193 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/__init__.py
--rw-r--r--   0        0        0      248 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/actions/__init__.py
--rw-r--r--   0        0        0      835 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/actions/abort_and_show_error.py
--rw-r--r--   0        0        0      295 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/actions/base.py
--rw-r--r--   0        0        0      350 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/actions/dummy.py
--rw-r--r--   0        0        0      200 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/config.py
--rw-r--r--   0        0        0     1008 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/__init__.py
--rw-r--r--   0        0        0      495 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/base.py
--rw-r--r--   0        0        0     1099 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/document_release.py
--rw-r--r--   0        0        0      542 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/dummy.py
--rw-r--r--   0        0        0      843 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/engineering_change_release.py
--rw-r--r--   0        0        0      391 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/field_value_calculation.py
--rw-r--r--   0        0        0     1019 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/part_release.py
--rw-r--r--   0        0        0     1083 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/events/workflow_task_trigger.py
--rw-r--r--   0        0        0     4561 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/handler.py
--rw-r--r--   0        0        0     3260 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/logging.py
--rw-r--r--   0        0        0     1660 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/metadata.py
--rw-r--r--   0        0        0      612 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/__init__.py
--rw-r--r--   0        0        0     1498 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/base.py
--rw-r--r--   0        0        0     2529 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/briefcase.py
--rw-r--r--   0        0        0     1272 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/classification.py
--rw-r--r--   0        0        0     4829 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/document.py
--rw-r--r--   0        0        0     4746 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/engineering_change.py
--rw-r--r--   0        0        0      921 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/file.py
--rw-r--r--   0        0        0     6555 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/part.py
--rw-r--r--   0        0        0     2142 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/objects/workflow.py
--rw-r--r--   0        0        0      235 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/request.py
--rw-r--r--   0        0        0     2457 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/response.py
--rw-r--r--   0        0        0     2622 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/service.py
--rw-r--r--   0        0        0        0 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/tools/__init__.py
--rw-r--r--   0        0        0      836 2024-03-01 12:05:05.778794 contactsoftware_functions-0.6.0/csfunctions/tools/write_schema.py
--rw-r--r--   0        0        0      630 2024-03-01 12:05:05.782794 contactsoftware_functions-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3445 1970-01-01 00:00:00.000000 contactsoftware_functions-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2674 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/README.md
+-rw-r--r--   0        0        0      193 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/actions/__init__.py
+-rw-r--r--   0        0        0      835 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/actions/abort_and_show_error.py
+-rw-r--r--   0        0        0      295 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/actions/base.py
+-rw-r--r--   0        0        0      350 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/actions/dummy.py
+-rw-r--r--   0        0        0      200 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/config.py
+-rw-r--r--   0        0        0     1008 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/base.py
+-rw-r--r--   0        0        0     1099 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/document_release.py
+-rw-r--r--   0        0        0      542 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/dummy.py
+-rw-r--r--   0        0        0      843 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/engineering_change_release.py
+-rw-r--r--   0        0        0      391 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/field_value_calculation.py
+-rw-r--r--   0        0        0     1019 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/part_release.py
+-rw-r--r--   0        0        0     1083 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/events/workflow_task_trigger.py
+-rw-r--r--   0        0        0     4739 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/handler.py
+-rw-r--r--   0        0        0     3260 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/logging.py
+-rw-r--r--   0        0        0     1660 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/metadata.py
+-rw-r--r--   0        0        0      612 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/objects/__init__.py
+-rw-r--r--   0        0        0     1498 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/objects/base.py
+-rw-r--r--   0        0        0     2529 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/objects/briefcase.py
+-rw-r--r--   0        0        0     1272 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/objects/classification.py
+-rw-r--r--   0        0        0     4829 2024-05-15 13:10:11.453295 contactsoftware_functions-0.7.0/csfunctions/objects/document.py
+-rw-r--r--   0        0        0     4746 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/objects/engineering_change.py
+-rw-r--r--   0        0        0      921 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/objects/file.py
+-rw-r--r--   0        0        0     6555 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/objects/part.py
+-rw-r--r--   0        0        0     2142 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/objects/workflow.py
+-rw-r--r--   0        0        0      235 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/request.py
+-rw-r--r--   0        0        0     2477 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/response.py
+-rw-r--r--   0        0        0     2622 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/service.py
+-rw-r--r--   0        0        0        0 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/tools/__init__.py
+-rw-r--r--   0        0        0      836 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/csfunctions/tools/write_schema.py
+-rw-r--r--   0        0        0      755 2024-05-15 13:10:11.457295 contactsoftware_functions-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 contactsoftware_functions-0.7.0/PKG-INFO
```

### Comparing `contactsoftware_functions-0.6.0/LICENSE` & `contactsoftware_functions-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/README.md` & `contactsoftware_functions-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
  <h1><a href="https://github.com/cslab/functions-sdk"><img src="https://www.contact-software.com/design/img/logo-icon.svg" width="50" alt="CONTACT Logo"></a> Functions-SDK for Python</h1>
 
 This SDK provides the **csfunctions** library for developing Functions with Python.
 
 Functions are deeply integrated in the CIM Database Cloud Webhooks technology. They are designed to work seamlessly together. The goal is to allow implementing custom business logic in a CIM Database Cloud SaaS application without leaving the CONTACT Cloud and without the need to create and maintain a separate infrastructure.
 
-**Documentation:** https://jens-kuerten.github.io/functions-sdk-python/
+**Documentation:** https://cslab.github.io/functions-sdk-python/
+
+**Source code:** https://github.com/cslab/functions-sdk-python
 
 ## Requirements
 
 Python 3.10+
 
 csfunctions is build with [Pydantic 2](https://docs.pydantic.dev/latest/)
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
 ************ _[[_CC_OO_NN_TT_AA_CC_TT_ _LL_oo_gg_oo_]]FFuunnccttiioonnss--SSDDKK ffoorr PPyytthhoonn ************
 This SDK provides the **csfunctions** library for developing Functions with
 Python. Functions are deeply integrated in the CIM Database Cloud Webhooks
 technology. They are designed to work seamlessly together. The goal is to allow
 implementing custom business logic in a CIM Database Cloud SaaS application
 without leaving the CONTACT Cloud and without the need to create and maintain a
-separate infrastructure. **Documentation:** https://jens-kuerten.github.io/
-functions-sdk-python/ ## Requirements Python 3.10+ csfunctions is build with
-[Pydantic 2](https://docs.pydantic.dev/latest/) ## Installation Install using
-pip: ``` sh pip install contactsoftware-functions ``` ## Usage ### Build the
-Function Folder content of a minimal example for a Function implementation: ```
-bash my_example_functions/ âââ environment.yaml âââ mymodule.py
+separate infrastructure. **Documentation:** https://cslab.github.io/functions-
+sdk-python/ **Source code:** https://github.com/cslab/functions-sdk-python ##
+Requirements Python 3.10+ csfunctions is build with [Pydantic 2](https://
+docs.pydantic.dev/latest/) ## Installation Install using pip: ``` sh pip
+install contactsoftware-functions ``` ## Usage ### Build the Function Folder
+content of a minimal example for a Function implementation: ``` bash
+my_example_functions/ âââ environment.yaml âââ mymodule.py
 âââ requirements.txt ``` Code for a Function: ``` python
 title="mymodule.py" import requests import json from csfunctions import
 MetaData, Service from csfunctions.events import DocumentReleaseEvent def
 send_doc_to_erp(metadata: MetaData, event: DocumentReleaseEvent, service:
 Service): # iterate over the documents contained in the event for document in
 event.data.documents: # create the payload for our (fictional ERP system)
 payload = json.dumps({ "document_number": document.z_nummer, "document_index":
```

### Comparing `contactsoftware_functions-0.6.0/csfunctions/actions/abort_and_show_error.py` & `contactsoftware_functions-0.7.0/csfunctions/actions/abort_and_show_error.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/events/__init__.py` & `contactsoftware_functions-0.7.0/csfunctions/events/__init__.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/events/document_release.py` & `contactsoftware_functions-0.7.0/csfunctions/events/document_release.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/events/dummy.py` & `contactsoftware_functions-0.7.0/csfunctions/events/dummy.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/events/engineering_change_release.py` & `contactsoftware_functions-0.7.0/csfunctions/events/engineering_change_release.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/events/part_release.py` & `contactsoftware_functions-0.7.0/csfunctions/events/part_release.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/events/workflow_task_trigger.py` & `contactsoftware_functions-0.7.0/csfunctions/events/workflow_task_trigger.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/handler.py` & `contactsoftware_functions-0.7.0/csfunctions/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,24 @@
     try:
         request = Request(**json.loads(request_body))
         link_objects(request.event)
         function_callback = get_function_callable(function_name, function_dir)
         service = Service(str(request.metadata.service_url), request.metadata.service_token)
 
         with RedirectToLoki(_log_stream, request.event.event_id):
-            result = function_callback(request.metadata, request.event, service)
+            response = function_callback(request.metadata, request.event, service)
+
+        if response is None:
+            return ""
 
         if not isinstance(
-            result, ResponseUnion
+            response, ResponseUnion
         ):  # need to check for ResponseUnion instead of Response, because isinstance doesn't work with annotated unions
-            raise ValueError("Function needs to return a Response object.")
+            raise ValueError("Function needs to return a Response object or None.")
+
+        # make sure the event_id is filled out correctly
+        response.event_id = request.event.event_id
+
     except Exception as e:  # pylint: disable=broad-except
-        result = ErrorResponse(message=str(e), error_type=type(e).__name__, trace=traceback.format_exc(), id="")
+        response = ErrorResponse(message=str(e), error_type=type(e).__name__, trace=traceback.format_exc(), id="")
 
-    return result.model_dump_json()
+    return response.model_dump_json()
```

### Comparing `contactsoftware_functions-0.6.0/csfunctions/logging.py` & `contactsoftware_functions-0.7.0/csfunctions/logging.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/metadata.py` & `contactsoftware_functions-0.7.0/csfunctions/metadata.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/__init__.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/base.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/base.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/briefcase.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/briefcase.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/classification.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/classification.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/document.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/document.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/engineering_change.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/engineering_change.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/file.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/file.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/part.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/part.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/objects/workflow.py` & `contactsoftware_functions-0.7.0/csfunctions/objects/workflow.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/response.py` & `contactsoftware_functions-0.7.0/csfunctions/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from csfunctions.actions import Action
 
 
 class ResponseType(str, Enum):
     WORKLOAD = "workload"
     DATA = "data"
     ERROR = "error"
+    EMPTY = "empty"
 
 
 class WorkloadResponse(BaseModel):
     def __init__(
         self,
         actions: list[Action],
         event_id: str | None = None,
```

### Comparing `contactsoftware_functions-0.6.0/csfunctions/service.py` & `contactsoftware_functions-0.7.0/csfunctions/service.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/csfunctions/tools/write_schema.py` & `contactsoftware_functions-0.7.0/csfunctions/tools/write_schema.py`

 * *Files identical despite different names*

### Comparing `contactsoftware_functions-0.6.0/pyproject.toml` & `contactsoftware_functions-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [tool.poetry]
 name = "contactsoftware-functions"
-version = "0.6.0"
+version = "0.7.0"
 readme = "README.md"
 
 license = "MIT"
 authors = [
     "Julian Alberts <jal@contact.de>",
     "Jens Kürten <jku@contact.de>"
 ]
 description = "Library for creating Functions for CIM Database Cloud."
+repository = "https://github.com/cslab/functions-sdk-python"
+documentation = "https://cslab.github.io/functions-sdk-python/"
 
 packages = [
     { include = "csfunctions"}
    ]
 
 
 [tool.poetry.dependencies]
```

### Comparing `contactsoftware_functions-0.6.0/PKG-INFO` & `contactsoftware_functions-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: contactsoftware-functions
-Version: 0.6.0
+Version: 0.7.0
 Summary: Library for creating Functions for CIM Database Cloud.
+Home-page: https://github.com/cslab/functions-sdk-python
 License: MIT
 Author: Julian Alberts
 Author-email: jal@contact.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,23 +16,27 @@
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: pydantic (>=2.3)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-mock (>=1.9.0,<2.0.0)
 Requires-Dist: rich (>=12.0.1,<13.0.0)
 Requires-Dist: urllib3 (==1.26.18)
+Project-URL: Documentation, https://cslab.github.io/functions-sdk-python/
+Project-URL: Repository, https://github.com/cslab/functions-sdk-python
 Description-Content-Type: text/markdown
 
  <h1><a href="https://github.com/cslab/functions-sdk"><img src="https://www.contact-software.com/design/img/logo-icon.svg" width="50" alt="CONTACT Logo"></a> Functions-SDK for Python</h1>
 
 This SDK provides the **csfunctions** library for developing Functions with Python.
 
 Functions are deeply integrated in the CIM Database Cloud Webhooks technology. They are designed to work seamlessly together. The goal is to allow implementing custom business logic in a CIM Database Cloud SaaS application without leaving the CONTACT Cloud and without the need to create and maintain a separate infrastructure.
 
-**Documentation:** https://jens-kuerten.github.io/functions-sdk-python/
+**Documentation:** https://cslab.github.io/functions-sdk-python/
+
+**Source code:** https://github.com/cslab/functions-sdk-python
 
 ## Requirements
 
 Python 3.10+
 
 csfunctions is build with [Pydantic 2](https://docs.pydantic.dev/latest/)
```

#### html2text {}

```diff
@@ -1,30 +1,34 @@
-Metadata-Version: 2.1 Name: contactsoftware-functions Version: 0.6.0 Summary:
-Library for creating Functions for CIM Database Cloud. License: MIT Author:
-Julian Alberts Author-email: jal@contact.de Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist:
-appdirs (>=1.4.4,<2.0.0) Requires-Dist: click (>=8.0.4,<9.0.0) Requires-Dist:
-pydantic (>=2.3) Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist:
-requests-mock (>=1.9.0,<2.0.0) Requires-Dist: rich (>=12.0.1,<13.0.0) Requires-
-Dist: urllib3 (==1.26.18) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: contactsoftware-functions Version: 0.7.0 Summary:
+Library for creating Functions for CIM Database Cloud. Home-page: https://
+github.com/cslab/functions-sdk-python License: MIT Author: Julian Alberts
+Author-email: jal@contact.de Requires-Python: >=3.10,<4.0 Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: click (>=8.0.4,<9.0.0) Requires-Dist: pydantic (>=2.3) Requires-
+Dist: requests (>=2.27.1,<3.0.0) Requires-Dist: requests-mock (>=1.9.0,<2.0.0)
+Requires-Dist: rich (>=12.0.1,<13.0.0) Requires-Dist: urllib3 (==1.26.18)
+Project-URL: Documentation, https://cslab.github.io/functions-sdk-python/
+Project-URL: Repository, https://github.com/cslab/functions-sdk-python
+Description-Content-Type: text/markdown
 ************ _[[_CC_OO_NN_TT_AA_CC_TT_ _LL_oo_gg_oo_]]FFuunnccttiioonnss--SSDDKK ffoorr PPyytthhoonn ************
 This SDK provides the **csfunctions** library for developing Functions with
 Python. Functions are deeply integrated in the CIM Database Cloud Webhooks
 technology. They are designed to work seamlessly together. The goal is to allow
 implementing custom business logic in a CIM Database Cloud SaaS application
 without leaving the CONTACT Cloud and without the need to create and maintain a
-separate infrastructure. **Documentation:** https://jens-kuerten.github.io/
-functions-sdk-python/ ## Requirements Python 3.10+ csfunctions is build with
-[Pydantic 2](https://docs.pydantic.dev/latest/) ## Installation Install using
-pip: ``` sh pip install contactsoftware-functions ``` ## Usage ### Build the
-Function Folder content of a minimal example for a Function implementation: ```
-bash my_example_functions/ âââ environment.yaml âââ mymodule.py
+separate infrastructure. **Documentation:** https://cslab.github.io/functions-
+sdk-python/ **Source code:** https://github.com/cslab/functions-sdk-python ##
+Requirements Python 3.10+ csfunctions is build with [Pydantic 2](https://
+docs.pydantic.dev/latest/) ## Installation Install using pip: ``` sh pip
+install contactsoftware-functions ``` ## Usage ### Build the Function Folder
+content of a minimal example for a Function implementation: ``` bash
+my_example_functions/ âââ environment.yaml âââ mymodule.py
 âââ requirements.txt ``` Code for a Function: ``` python
 title="mymodule.py" import requests import json from csfunctions import
 MetaData, Service from csfunctions.events import DocumentReleaseEvent def
 send_doc_to_erp(metadata: MetaData, event: DocumentReleaseEvent, service:
 Service): # iterate over the documents contained in the event for document in
 event.data.documents: # create the payload for our (fictional ERP system)
 payload = json.dumps({ "document_number": document.z_nummer, "document_index":
```

