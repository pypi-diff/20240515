# Comparing `tmp/astra_haystack-0.6.0.tar.gz` & `tmp/astra_haystack-0.7.0.tar.gz`

## Comparing `astra_haystack-0.6.0.tar` & `astra_haystack-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/__init__.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/example.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/pipeline_example.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/requirements.txt
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/examples/data/usr_01.txt
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/pydoc/config.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/components/retrievers/astra/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/components/retrievers/astra/retriever.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/__init__.py
--rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/astra_client.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/document_store.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/errors.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/filters.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0    11745 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/tests/test_document_store.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/LICENSE
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/README.md
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 astra_haystack-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/__init__.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/example.py
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/pipeline_example.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/requirements.txt
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/examples/data/usr_01.txt
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/pydoc/config.yml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/components/retrievers/astra/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/components/retrievers/astra/retriever.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/__init__.py
+-rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/astra_client.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/document_store.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/errors.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/filters.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/README.md
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 astra_haystack-0.7.0/PKG-INFO
```

### Comparing `astra_haystack-0.6.0/examples/example.py` & `astra_haystack-0.7.0/examples/example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/examples/pipeline_example.py` & `astra_haystack-0.7.0/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/examples/data/usr_01.txt` & `astra_haystack-0.7.0/examples/data/usr_01.txt`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/pydoc/config.yml` & `astra_haystack-0.7.0/pydoc/config.yml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Astra integration for Haystack
   category_slug: integrations-api
   title: Astra
   slug: integrations-astra
   order: 30
   markdown:
     descriptive_class_title: false
```

### Comparing `astra_haystack-0.6.0/src/haystack_integrations/components/retrievers/astra/retriever.py` & `astra_haystack-0.7.0/src/haystack_integrations/components/retrievers/astra/retriever.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/astra_client.py` & `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/astra_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
         :param find_query: a dictionary with the query options
         :returns: the documents found in the index
         """
         response_dict = self._astra_db_collection.find(
             filter=find_query.get("filter"),
             sort=find_query.get("sort"),
             options=find_query.get("options"),
+            projection={"*": 1},
         )
 
         if "data" in response_dict and "documents" in response_dict["data"]:
             return response_dict["data"]["documents"]
         else:
             logger.warning(f"No documents found: {response_dict}")
 
@@ -269,14 +270,15 @@
         """
         document_id = document.pop(id_key)
 
         response_dict = self._astra_db_collection.find_one_and_update(
             filter={id_key: document_id},
             update={"$set": document},
             options={"returnDocument": "after"},
+            projection={"*": 1},
         )
 
         document[id_key] = document_id
 
         if "status" in response_dict and "errors" not in response_dict:
             if "matchedCount" in response_dict["status"] and "modifiedCount" in response_dict["status"]:
                 if response_dict["status"]["matchedCount"] == 1 and response_dict["status"]["modifiedCount"] == 1:
```

### Comparing `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/document_store.py` & `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/document_store.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/errors.py` & `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/errors.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/src/haystack_integrations/document_stores/astra/filters.py` & `astra_haystack-0.7.0/src/haystack_integrations/document_stores/astra/filters.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/tests/test_document_store.py` & `astra_haystack-0.7.0/tests/test_document_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,32 @@
 from haystack.document_stores.errors import MissingDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
 
 from haystack_integrations.document_stores.astra import AstraDocumentStore
 
 
-def test_namespace_init():
+@pytest.fixture
+def mock_auth(monkeypatch):
+    monkeypatch.setenv("ASTRA_DB_API_ENDPOINT", "http://example.com")
+    monkeypatch.setenv("ASTRA_DB_APPLICATION_TOKEN", "test_token")
+
+
+def test_namespace_init(mock_auth):  # noqa
     with mock.patch("haystack_integrations.document_stores.astra.astra_client.AstraDB") as client:
         AstraDocumentStore()
         assert "namespace" in client.call_args.kwargs
         assert client.call_args.kwargs["namespace"] is None
 
         AstraDocumentStore(namespace="foo")
         assert "namespace" in client.call_args.kwargs
         assert client.call_args.kwargs["namespace"] == "foo"
 
 
-def test_to_dict():
+def test_to_dict(mock_auth):  # noqa
     with mock.patch("haystack_integrations.document_stores.astra.astra_client.AstraDB"):
         ds = AstraDocumentStore()
         result = ds.to_dict()
         assert result["type"] == "haystack_integrations.document_stores.astra.document_store.AstraDocumentStore"
         assert set(result["init_parameters"]) == {
             "api_endpoint",
             "token",
```

### Comparing `astra_haystack-0.6.0/tests/test_retriever.py` & `astra_haystack-0.7.0/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/.gitignore` & `astra_haystack-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/LICENSE` & `astra_haystack-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/README.md` & `astra_haystack-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `astra_haystack-0.6.0/pyproject.toml` & `astra_haystack-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -76,20 +76,20 @@
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive --explicit-package-bases {args:src/ tests}"
 style = [
-  "ruff {args:.}",
+  "ruff check {args:.}",
   "black --check --diff {args:.}",
 ]
 fmt = [
   "black {args:.}",
-  "ruff --fix {args:.}",
+  "ruff check --fix {args:.}",
   "style",
 ]
 all = [
   "style",
   "typing",
 ]
 
@@ -100,15 +100,15 @@
 target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py38"
 line-length = 120
-select = [
+lint.select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
   "EM",
@@ -127,37 +127,37 @@
   "S",
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
-ignore = [
+lint.ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
-unfixable = [
+lint.unfixable = [
   # Don't touch unused imports
   "F401",
 ]
-exclude = ["example"]
+lint.exclude = ["example"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["haystack_integrations"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "parents"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source = ["haystack_integrations"]
 branch = true
 parallel = false
```

### Comparing `astra_haystack-0.6.0/PKG-INFO` & `astra_haystack-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astra-haystack
-Version: 0.6.0
+Version: 0.7.0
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/astra
 Author-email: Anant Corporation <support@anant.us>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

