# Comparing `tmp/marqo-3.3.0.tar.gz` & `tmp/marqo-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-3.3.0.tar", last modified: Wed Apr 24 06:45:45 2024, max compression
+gzip compressed data, was "marqo-3.4.0.tar", last modified: Wed May 15 03:45:37 2024, max compression
```

## Comparing `marqo-3.3.0.tar` & `marqo-3.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.858079 marqo-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-04-24 06:45:38.000000 marqo-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-24 06:45:45.858079 marqo-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-24 06:45:38.000000 marqo-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 06:45:38.000000 marqo-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 06:45:45.858079 marqo-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-24 06:45:38.000000 marqo-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.850079 marqo-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.854079 marqo-3.3.0/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/cloud_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/default_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    42344 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/marqo_cloud_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/marqo_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.854079 marqo-3.3.0/src/marqo/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/create_index_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/marqo_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/marqo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/marqo_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/models/search_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 06:45:38.000000 marqo-3.3.0/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:45:45.858079 marqo-3.3.0/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 06:45:45.000000 marqo-3.3.0/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.433856 marqo-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-15 03:45:31.000000 marqo-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-05-15 03:45:37.433856 marqo-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-05-15 03:45:31.000000 marqo-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 03:45:31.000000 marqo-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:45:37.433856 marqo-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 03:45:31.000000 marqo-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.425856 marqo-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.429856 marqo-3.4.0/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/cloud_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/default_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43308 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/marqo_cloud_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/marqo_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.433856 marqo-3.4.0/src/marqo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/create_index_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/marqo_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/marqo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/marqo_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/search_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.433856 marqo-3.4.0/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-3.3.0/LICENSE` & `marqo-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/PKG-INFO` & `marqo-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.3.0
+Version: 3.4.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.3.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.4.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
 Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
```

### Comparing `marqo-3.3.0/README.md` & `marqo-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/setup.py` & `marqo-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="3.3.0",
+    version="3.4.0",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-3.3.0/src/marqo/_httprequests.py` & `marqo-3.4.0/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/client.py` & `marqo-3.4.0/src/marqo/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,16 @@
         ann_parameters: Optional[marqo_index.AnnParameters] = None,
         wait_for_readiness: bool = True,
         inference_type: Optional[str] = None,
         storage_class: Optional[str] = None,
         number_of_shards: Optional[int] = None,
         number_of_replicas: Optional[int] = None,
         number_of_inferences: Optional[int] = None,
+        text_query_prefix: Optional[str] = None,
+        text_chunk_prefix: Optional[str] = None,
     ) -> Dict[str, Any]:
         """Create the index. Please refer to the marqo cloud to see options for inference and storage node types.
         Calls Index.create() with the same parameters.
         All parameters are optional, and will be set to None if not specified.
         We leave the default values to be set by Marqo.
 
         Args:
@@ -140,14 +142,16 @@
             ann_parameters=ann_parameters,
             wait_for_readiness=wait_for_readiness,
             inference_type=inference_type,
             storage_class=storage_class,
             number_of_shards=number_of_shards,
             number_of_replicas=number_of_replicas,
             number_of_inferences=number_of_inferences,
+            text_query_prefix=text_query_prefix,
+            text_chunk_prefix=text_chunk_prefix,
         )
 
     def delete_index(self, index_name: str, wait_for_readiness=True) -> Dict[str, Any]:
         """Deletes an index
 
         Args:
             index_name: name of the index
```

### Comparing `marqo-3.3.0/src/marqo/cloud_helpers.py` & `marqo-3.4.0/src/marqo/cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/config.py` & `marqo-3.4.0/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/default_instance_mappings.py` & `marqo-3.4.0/src/marqo/default_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/errors.py` & `marqo-3.4.0/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/index.py` & `marqo-3.4.0/src/marqo/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from packaging import version as versioning_helpers
 from requests import RequestException
 
 from marqo import errors, utils
 from marqo._httprequests import HttpRequests
 from marqo.cloud_helpers import cloud_wait_for_index_status
 from marqo.config import Config
-from marqo.enums import IndexStatus, InterpolationMethod
+from marqo.enums import IndexStatus, InterpolationMethod, EmbedContentType
 from marqo.enums import SearchMethods
 from marqo.errors import MarqoWebError, UnsupportedOperationError, MarqoCloudIndexNotFoundError
 from marqo.marqo_logging import mq_logger
 from marqo.models import marqo_index
 from marqo.models.create_index_settings import IndexSettings
 from marqo.models.marqo_cloud import CloudIndexSettings
 from marqo.version import minimum_supported_marqo_version
@@ -92,14 +92,16 @@
                ann_parameters: Optional[marqo_index.AnnParameters] = None,
                inference_type: Optional[str] = None,
                storage_class: Optional[str] = None,
                number_of_shards: Optional[int] = None,
                number_of_replicas: Optional[int] = None,
                number_of_inferences: Optional[int] = None,
                wait_for_readiness: bool = True,
+               text_chunk_prefix: Optional[str] = None,
+               text_query_prefix: Optional[str] = None,
                ) -> Dict[str, Any]:
         """Create the index. Please refer to the marqo cloud to see options for inference and storage node types.
         Creates CreateIndexSettings object and then uses it to create the index.
         CreateIndexSettings object sets all parameters to their default values if not specified.
 
         All parameters are optional, and will be set to their default values if not specified.
         Default values can be found in models/create_index_settings.py CreateIndexSettings class.
@@ -150,15 +152,17 @@
                 tensorFields=tensor_fields,
                 model=model,
                 modelProperties=model_properties,
                 normalizeEmbeddings=normalize_embeddings,
                 textPreprocessing=text_preprocessing,
                 imagePreprocessing=image_preprocessing,
                 vectorNumericType=vector_numeric_type,
-                annParameters=ann_parameters
+                annParameters=ann_parameters,
+                textChunkPrefix=text_chunk_prefix,
+                textQueryPrefix=text_query_prefix,
             )
 
             return req.post(f"indexes/{index_name}", body=local_create_index_settings.generate_request_body())
 
         # py-marqo against Marqo Cloud
         else:
             cloud_index_settings: CloudIndexSettings = CloudIndexSettings(
@@ -176,14 +180,16 @@
                 vectorNumericType=vector_numeric_type,
                 annParameters=ann_parameters,
                 numberOfInferences=number_of_inferences,
                 inferenceType=inference_type,
                 numberOfShards=number_of_shards,
                 numberOfReplicas=number_of_replicas,
                 storageClass=storage_class,
+                textChunkPrefix=text_chunk_prefix,
+                textQueryPrefix=text_query_prefix,
             )
 
             response = req.post(f"indexes/{index_name}", body=cloud_index_settings.generate_request_body())
             if wait_for_readiness:
                 cloud_wait_for_index_status(req, index_name, IndexStatus.READY)
             return response
 
@@ -198,15 +204,16 @@
                limit: int = 10, offset: int = 0, search_method: Union[SearchMethods.TENSOR, str] = SearchMethods.TENSOR,
                highlights=None, device: Optional[str] = None, filter_string: str = None,
                show_highlights=True, reranker=None, image_download_headers: Optional[Dict] = None,
                attributes_to_retrieve: Optional[List[str]] = None,
                boost: Optional[Dict[str, List[Union[float, int]]]] = None,
                context: Optional[dict] = None, score_modifiers: Optional[dict] = None,
                model_auth: Optional[dict] = None,
-               ef_search: Optional[int] = None, approximate: Optional[bool] = None
+               ef_search: Optional[int] = None, approximate: Optional[bool] = None,
+               text_query_prefix: Optional[str] = None,
                ) -> Dict[str, Any]:
         """Search the index.
 
         Args:
             q: String to search, or a dictionary of weighted strings to search
                 (with the structure <search string>:<weight float>). Strings
                 to search are text or a pointer/url to an image if the index
@@ -261,14 +268,15 @@
             "searchableAttributes": searchable_attributes,
             "limit": limit,
             "offset": offset,
             "searchMethod": search_method,
             "showHighlights": show_highlights,
             "reRanker": reranker,
             "boost": boost,
+            "textQueryPrefix": text_query_prefix,
         }
 
         body = {k: v for k, v in body.items() if v is not None}
 
         res = self.http.post(
             path=path_with_query_str,
             body=body,
@@ -372,15 +380,15 @@
                                   f"generate recommendations."
 
         mq_logger.debug(recommend_time_log)
         return res
 
     def embed(self, content: Union[Union[str, Dict[str, float]], List[Union[str, Dict[str, float]]]],
               device: Optional[str] = None, image_download_headers: Optional[Dict] = None,
-              model_auth: Optional[dict] = None):
+              model_auth: Optional[dict] = None, content_type: Optional[EmbedContentType] = EmbedContentType.Query):
         """Retrieve embeddings for content or list of content.
         Args:
             content: string, dictionary of weighted strings, or list of either. Strings
                 to search are text or a pointer/url to an image if the index
                 has treat_urls_and_pointers_as_images set to True.
 
                 If queries are weighted, each weight act as a (possibly negative)
@@ -388,32 +396,35 @@
 
             device: the device used to index the data. Examples include "cpu",
                 "cuda" and "cuda:2".
 
             image_download_headers: a dictionary of headers to be passed while downloading images,
                 for URLs found in documents
             model_auth: authorisation that lets Marqo download a private model, if required
+            content_type: the type of prefix the user wants. "query", "document", or None.
         Returns:
             Dictionary of content, embeddings, and processingTimeMs.
         """
 
         start_time_client_request = timer()
 
         path_with_query_str = (
             f"indexes/{self.index_name}/embed"
             f"{f'?&device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
         )
         body = {
             "content": content,
+            "content_type": content_type,
         }
 
         if image_download_headers is not None:
             body["image_download_headers"] = image_download_headers
         if model_auth is not None:
             body["modelAuth"] = model_auth
+        
 
         res = self.http.post(
             path=path_with_query_str,
             body=body,
             index_name=self.index_name,
         )
 
@@ -472,15 +483,16 @@
             documents: List[Dict[str, Any]],
             client_batch_size: int = None,
             device: str = None,
             tensor_fields: List[str] = None,
             use_existing_tensors: bool = False,
             image_download_headers: dict = None,
             mappings: dict = None,
-            model_auth: dict = None
+            model_auth: dict = None,
+            text_chunk_prefix: str = None,
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """Add documents to this index. Does a partial update on existing documents,
         based on their ID. Adds unseen documents to the index.
 
         Args:
             documents: List of documents. Each document should be a dictionary.
             client_batch_size: if it is set, documents will be indexed into batches
@@ -490,37 +502,40 @@
                 "cuda" and "cuda:2"
             tensor_fields: fields within documents to create and store tensors against.
             use_existing_tensors: use vectors that already exist in the docs.
             image_download_headers: a dictionary of headers to be passed while downloading images,
                 for URLs found in documents
             mappings: a dictionary to help handle the object fields. e.g., multimodal_combination field
             model_auth: used to authorise a private model
+            text_chunk_prefix: the request level prefix for adding docs
         Returns:
             Response body outlining indexing result
         """
 
         if image_download_headers is None:
             image_download_headers = dict()
         return self._add_docs_organiser(
             documents=documents,
             client_batch_size=client_batch_size, device=device, tensor_fields=tensor_fields,
             use_existing_tensors=use_existing_tensors,
-            image_download_headers=image_download_headers, mappings=mappings, model_auth=model_auth
+            image_download_headers=image_download_headers, mappings=mappings, model_auth=model_auth,
+            text_chunk_prefix=text_chunk_prefix
         )
 
     def _add_docs_organiser(
             self,
             documents: List[Dict[str, Any]],
             client_batch_size: int = None,
             device: str = None,
             tensor_fields: List = None,
             use_existing_tensors: bool = False,
             image_download_headers: dict = None,
             mappings: dict = None,
-            model_auth: dict = None
+            model_auth: dict = None,
+            text_chunk_prefix: str = None,
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         error_detected_message = ('Errors detected in add documents call. '
                                   'Please examine the returned result object for more information.')
 
         num_docs = len(documents)
 
         # ADD DOCS TIMER-LOGGER (1)
@@ -539,14 +554,17 @@
             "mappings": mappings,
             "modelAuth": model_auth,
         }
 
         if tensor_fields is not None:
             base_body['tensorFields'] = tensor_fields
 
+        if text_chunk_prefix is not None:
+            base_body['textChunkPrefix'] = text_chunk_prefix
+
         end_time_client_process = timer()
         total_client_process_time = end_time_client_process - start_time_client_process
         mq_logger.debug(f"add_documents pre-processing: took {(total_client_process_time):.3f}s for {num_docs} docs.")
 
         if client_batch_size is not None:
             if client_batch_size <= 0:
                 raise errors.InvalidArgError("Batch size can't be less than 1!")
```

### Comparing `marqo-3.3.0/src/marqo/instance_mappings.py` & `marqo-3.4.0/src/marqo/instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/marqo_cloud_instance_mappings.py` & `marqo-3.4.0/src/marqo/marqo_cloud_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/models/create_index_settings.py` & `marqo-3.4.0/src/marqo/models/create_index_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     model: Optional[str] = None
     modelProperties: Optional[Dict[str, Any]] = None
     normalizeEmbeddings: Optional[bool] = None
     textPreprocessing: Optional[marqo_index.TextPreProcessing] = None
     imagePreprocessing: Optional[marqo_index.ImagePreProcessing] = None
     vectorNumericType: Optional[marqo_index.VectorNumericType] = None
     annParameters: Optional[marqo_index.AnnParameters] = None
+    textQueryPrefix: Optional[str] = None
+    textChunkPrefix: Optional[str] = None
 
     def generate_request_body(self) -> dict:
         """A json encoded string of the request body"""
         # We return settingsDict if it is not None, otherwise we return the dict
         if self.settingsDict is not None:
             return self.settingsDict
         else:
```

### Comparing `marqo-3.3.0/src/marqo/models/marqo_cloud.py` & `marqo-3.4.0/src/marqo/models/marqo_cloud.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/models/marqo_index.py` & `marqo-3.4.0/src/marqo/models/marqo_index.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/models/marqo_models.py` & `marqo-3.4.0/src/marqo/models/marqo_models.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/models/search_models.py` & `marqo-3.4.0/src/marqo/models/search_models.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/utils.py` & `marqo-3.4.0/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-3.3.0/src/marqo/version.py` & `marqo-3.4.0/src/marqo/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__marqo_version__ = "2.5.0"
+__marqo_version__ = "2.6.0"
 __marqo_release_page__ = f"https://github.com/marqo-ai/marqo/releases/tag/{__marqo_version__}"
 
 __minimum_supported_marqo_version__ = "2.0"
 
 
 def supported_marqo_version() -> str:
     return f"This Marqo Python client is built for Marqo release ({__marqo_version__}) \n" \
```

### Comparing `marqo-3.3.0/src/marqo.egg-info/PKG-INFO` & `marqo-3.4.0/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.3.0
+Version: 3.4.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.3.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.4.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
 Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
```

### Comparing `marqo-3.3.0/src/marqo.egg-info/SOURCES.txt` & `marqo-3.4.0/src/marqo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

