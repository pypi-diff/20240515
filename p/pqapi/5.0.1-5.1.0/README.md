# Comparing `tmp/pqapi-5.0.1.tar.gz` & `tmp/pqapi-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqapi-5.0.1.tar", last modified: Thu May  2 20:00:52 2024, max compression
+gzip compressed data, was "pqapi-5.1.0.tar", last modified: Wed May 15 20:13:16 2024, max compression
```

## Comparing `pqapi-5.0.1.tar` & `pqapi-5.1.0.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.542230 pqapi-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 20:00:30.000000 pqapi-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-02 20:00:52.542230 pqapi-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-02 20:00:30.000000 pqapi-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.538231 pqapi-5.0.1/pqapi/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 20:00:30.000000 pqapi-5.0.1/pqapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.542230 pqapi-5.0.1/pqapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 20:00:52.000000 pqapi-5.0.1/pqapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-02 20:00:30.000000 pqapi-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:00:52.542230 pqapi-5.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:00:52.542230 pqapi-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-02 20:00:30.000000 pqapi-5.0.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:13:16.287449 pqapi-5.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:13:16.279449 pqapi-5.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:13:16.279449 pqapi-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-15 20:12:37.000000 pqapi-5.1.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-15 20:12:37.000000 pqapi-5.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-15 20:12:37.000000 pqapi-5.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-15 20:12:37.000000 pqapi-5.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 20:12:37.000000 pqapi-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-15 20:13:16.287449 pqapi-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-15 20:12:37.000000 pqapi-5.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 20:12:37.000000 pqapi-5.1.0/example.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:13:16.283449 pqapi-5.1.0/pqapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-15 20:12:37.000000 pqapi-5.1.0/pqapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-15 20:12:37.000000 pqapi-5.1.0/pqapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-15 20:12:37.000000 pqapi-5.1.0/pqapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:12:37.000000 pqapi-5.1.0/pqapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 20:12:37.000000 pqapi-5.1.0/pqapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 20:13:16.000000 pqapi-5.1.0/pqapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:13:16.287449 pqapi-5.1.0/pqapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-15 20:13:16.000000 pqapi-5.1.0/pqapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-15 20:13:16.000000 pqapi-5.1.0/pqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:13:16.000000 pqapi-5.1.0/pqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 20:13:16.000000 pqapi-5.1.0/pqapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 20:13:16.000000 pqapi-5.1.0/pqapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-15 20:12:37.000000 pqapi-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:13:16.287449 pqapi-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:13:16.287449 pqapi-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)  1620022 2024-05-15 20:12:37.000000 pqapi-5.1.0/tests/paper.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-15 20:12:37.000000 pqapi-5.1.0/tests/test_api.py
```

### Comparing `pqapi-5.0.1/LICENSE` & `pqapi-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqapi-5.0.1/PKG-INFO` & `pqapi-5.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqapi
-Version: 5.0.1
+Version: 5.1.0
 Summary: API for interacting with paperqa.app
 Author-email: Andrew White <andrew@futurehouse.org>
 Maintainer-email: Andrew White <andrew@futurehouse.org>, James Braza <james@futurehouse.org>, Michael Skarlinski <mskarlinski@futurehouse.org>
 License: MIT License
         
         Copyright (c) 2023 Future House
         
@@ -46,16 +46,18 @@
 Requires-Dist: click; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-sugar; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
+Provides-Extra: publish
+Requires-Dist: build; extra == "publish"
 
-# peperqa-api
+# paperqa-api
 
 Python client for interacting with paperqa app
 
 # Usage
 
 Make sure to set the environment variable `PQA_API_TOKEN` or `PQA_API_KEY` to your API token.
```

### Comparing `pqapi-5.0.1/README.md` & `pqapi-5.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# peperqa-api
+# paperqa-api
 
 Python client for interacting with paperqa app
 
 # Usage
 
 Make sure to set the environment variable `PQA_API_TOKEN` or `PQA_API_KEY` to your API token.
```

### Comparing `pqapi-5.0.1/pqapi/__init__.py` & `pqapi-5.1.0/pqapi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from .api import (
     agent_query,
     async_agent_query,
     async_delete_bibliography,
     async_get_bibliography,
     async_get_feedback,
     async_query,
+    async_scrape,
     async_send_feedback,
     check_dois,
     delete_bibliography,
     get_bibliography,
     upload_file,
     upload_paper,
 )
-from .models import AnswerResponse, QueryRequest, UploadMetadata, get_prompts
+from .models import (
+    AnswerResponse,
+    QueryRequest,
+    ScrapeRequest,
+    UploadMetadata,
+    get_prompts,
+)
 from .version import __version__
 
 __all__ = [
-    "__version__",
-    "upload_file",
-    "upload_paper",
-    "agent_query",
-    "get_bibliography",
-    "delete_bibliography",
+    "AnswerResponse",
     "QueryRequest",
+    "ScrapeRequest",
     "UploadMetadata",
-    "AnswerResponse",
+    "__version__",
+    "agent_query",
+    "async_agent_query",
     "async_delete_bibliography",
     "async_get_bibliography",
-    "async_agent_query",
+    "async_get_feedback",
     "async_query",
-    "get_prompts",
+    "async_scrape",
     "async_send_feedback",
-    "async_get_feedback",
     "check_dois",
+    "delete_bibliography",
+    "get_bibliography",
+    "get_prompts",
+    "upload_file",
+    "upload_paper",
 ]
```

### Comparing `pqapi-5.0.1/pqapi/api.py` & `pqapi-5.1.0/pqapi/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-import json
 import logging
 from typing import Any, BinaryIO
 from uuid import UUID
 
 import aiohttp
 import requests
 import tenacity
 
-from .models import AnswerResponse, DocsStatus, QueryRequest, UploadMetadata
+from .models import (
+    AnswerResponse,
+    DocsStatus,
+    QueryRequest,
+    ScrapeRequest,
+    UploadMetadata,
+)
 from .utils import get_pqa_key, get_pqa_url
 
 logger = logging.getLogger(__name__)
 PQA_URL = get_pqa_url()
 
 
 def coerce_request(query: str | QueryRequest) -> QueryRequest:
@@ -128,15 +133,15 @@
 )
 def agent_query(query: QueryRequest | str, bibliography: str = "tmp") -> AnswerResponse:
     query_request = coerce_request(query)
     url = f"{PQA_URL}/api/agent/{bibliography if bibliography else 'tmp'}"
     with requests.Session() as session:
         response = session.post(
             url,
-            json={"query": query_request.model_dump()},
+            json={"query": query_request.model_dump_json()},
             headers={
                 "Authorization": f"Bearer {get_pqa_key()}",
                 "Content-Type": "application/json; charset=utf-8",
             },
         )
         response.raise_for_status()
         return parse_response(response.json())
@@ -147,29 +152,30 @@
     stop=tenacity.stop_after_attempt(2),
 )
 async def async_agent_query(
     query: QueryRequest | str,
     bibliography: str = "tmp",
 ) -> AnswerResponse:
     query_request = coerce_request(query)
-    qd = query_request.model_dump()
     async with (
         aiohttp.ClientSession() as session,
         session.post(
             f"{PQA_URL}/api/agent/{bibliography if bibliography else 'tmp'}",
-            json={"query": qd},
+            json={"query": query_request.model_dump_json()},
             timeout=1200,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         ) as response,
     ):
         try:
             data = await response.json()
         except Exception:
             text = await response.text()
-            logger.warning(f"Failed Request: \n{json.dumps(qd, indent=2)}")
+            logger.warning(
+                f"Failed Request: \n{query_request.model_dump_json(indent=2)}"
+            )
             logger.warning(f"\n\nResponse:\n\n{text}")
         response.raise_for_status()
         return parse_response(data)
 
 
 @tenacity.retry(
     wait=tenacity.wait_random_exponential(multiplier=1, max=10),
@@ -235,7 +241,32 @@
             json=body,
             timeout=600,
             headers={"Authorization": f"Bearer {get_pqa_key()}"},
         ) as response,
     ):
         response.raise_for_status()
         return await response.json()
+
+
+async def async_scrape(
+    scrape_request: ScrapeRequest, docs_name: str = "tmp"
+) -> list[dict]:
+    """
+    Call /api/scrape/{docs_name}.
+
+    Args:
+        scrape_request: ScrapeRequest to send.
+        docs_name: Stored Docs object's name, or 'tmp' to use a temporary Docs object.
+
+    Returns:
+        Websocket logs from the scrape.
+    """
+    async with (
+        aiohttp.ClientSession() as session,
+        session.post(
+            f"{PQA_URL}/api/scrape/{docs_name}",
+            json=scrape_request.model_dump(exclude={"use_internal_scrapers"}),
+            headers={"Authorization": f"Bearer {get_pqa_key()}"},
+        ) as response,
+    ):
+        response.raise_for_status()
+        return await response.json()
```

### Comparing `pqapi-5.0.1/pqapi/models.py` & `pqapi-5.1.0/pqapi/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import re
 from functools import lru_cache
 
 import paperqa
 import requests
 from paperqa.types import Answer, PromptCollection
-from pydantic import BaseModel, Field, ValidationInfo, field_validator, validator
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    Field,
+    ValidationInfo,
+    computed_field,
+    field_validator,
+    validator,
+)
 
 from .utils import get_pqa_key, get_pqa_url
 
 
 class AgentPromptCollection(BaseModel):
     agent_prompt: str = ""
     agent_search_tool: str = ""
@@ -129,7 +137,29 @@
 class AnswerResponse(BaseModel):
     answer: Answer
     usage: dict[str, list[int]]
     bibtex: dict[str, str]
     status: str
     timing_info: dict[str, dict[str, float]] | None = None
     duration: float = 0
+
+
+class ScrapeRequest(BaseModel):
+    """This was copied from paperqa-server as of shortened commit 452c6fc."""
+
+    model_config = ConfigDict(frozen=True, extra="forbid")
+    question: str = ""
+    limit: int = Field(
+        default=5,
+        description=(
+            "Target minimum number of papers to scrape. Note that we may not pull this"
+            " many in some scenarios (e.g. if scraper fails on many papers)."
+        ),
+    )
+    query: str | None = None
+    year: str | None = None
+    search_type: str = "default"
+    offset: int = 0
+
+    @computed_field  # type: ignore[misc]
+    @property
+    def use_internal_scrapers(self) -> bool: ...  # type: ignore[empty-body]
```

### Comparing `pqapi-5.0.1/pqapi.egg-info/PKG-INFO` & `pqapi-5.1.0/pqapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqapi
-Version: 5.0.1
+Version: 5.1.0
 Summary: API for interacting with paperqa.app
 Author-email: Andrew White <andrew@futurehouse.org>
 Maintainer-email: Andrew White <andrew@futurehouse.org>, James Braza <james@futurehouse.org>, Michael Skarlinski <mskarlinski@futurehouse.org>
 License: MIT License
         
         Copyright (c) 2023 Future House
         
@@ -46,16 +46,18 @@
 Requires-Dist: click; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-sugar; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
+Provides-Extra: publish
+Requires-Dist: build; extra == "publish"
 
-# peperqa-api
+# paperqa-api
 
 Python client for interacting with paperqa app
 
 # Usage
 
 Make sure to set the environment variable `PQA_API_TOKEN` or `PQA_API_KEY` to your API token.
```

### Comparing `pqapi-5.0.1/pyproject.toml` & `pqapi-5.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools >= 61.0"]
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 
 [project]
 authors = [
     {email = "andrew@futurehouse.org", name = "Andrew White"},
 ]
 # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
 classifiers = [
@@ -19,35 +19,38 @@
     "aiohttp",
     "paper-qa>=4.1.1",
     "pydantic~=2.0",
     "requests",
     "tenacity",
 ]
 description = "API for interacting with paperqa.app"
+dynamic = ["version"]
 license = {file = "LICENSE"}
 maintainers = [
     {email = "andrew@futurehouse.org", name = "Andrew White"},
     {email = "james@futurehouse.org", name = "James Braza"},
     {email = "mskarlinski@futurehouse.org", name = "Michael Skarlinski"},
 ]
 name = "pqapi"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "5.0.1"
 
 [project.optional-dependencies]
 dev = [
     "click",
     "pre-commit",
     "pytest",
     "pytest-asyncio",
     "pytest-sugar",
     "pytest-xdist",
     "types-requests",
 ]
+publish = [
+    "build",
+]
 
 [project.urls]
 issues = "https://github.com/Future-House/paperqa-api/issues"
 repository = "https://github.com/Future-House/paperqa-api"
 
 [tool.black]
 preview = true
@@ -110,21 +113,14 @@
 warn_unreachable = true
 # Warns about per-module sections in the config file that do not match any
 # files processed when invoking mypy.
 warn_unused_configs = true
 # Warns about unneeded `# type: ignore` comments.
 warn_unused_ignores = true
 
-[[tool.mypy.overrides]]
-# Suppresses error messages about imports that cannot be resolved.
-ignore_missing_imports = true
-# Per-module configuration options
-module = [
-]
-
 [tool.pytest.ini_options]
 # List of directories that should be searched for tests when no specific directories,
 # files or test ids are given in the command line when executing pytest from the rootdir
 # directory. File system paths may use shell-style wildcards, including the recursive **
 # pattern.
 testpaths = ["tests"]
 
@@ -222,13 +218,16 @@
 # Whether to use Google-style or NumPy-style conventions or the PEP257
 # defaults when analyzing docstring sections.
 convention = "google"
 
 [tool.setuptools.packages.find]
 include = ["pqapi*"]
 
+[tool.setuptools_scm]
+version_file = "pqapi/version.py"
+
 [tool.tomlsort]
 all = true
 in_place = true
 spaces_before_inline_comment = 2  # Match Python PEP 8
 spaces_indent_inline_array = 4  # Match Python PEP 8
 trailing_comma_inline_array = true
```

### Comparing `pqapi-5.0.1/tests/test_api.py` & `pqapi-5.1.0/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import paperqa
 import pytest
 import requests
 
 from pqapi import (
     AnswerResponse,
     QueryRequest,
+    ScrapeRequest,
     UploadMetadata,
     agent_query,
     async_agent_query,
     async_query,
+    async_scrape,
     async_send_feedback,
     check_dois,
     delete_bibliography,
     get_bibliography,
     get_prompts,
     upload_file,
     upload_paper,
@@ -23,15 +25,15 @@
 
 
 def test_get_prompts() -> None:
     prompts, agent_prompts = get_prompts()
     some_prompt = prompts["default"]
     assert isinstance(some_prompt, paperqa.PromptCollection)
     assert agent_prompts.timeout > 0
-    assert len(agent_prompts.agent_search_tool) > 25
+    assert len(agent_prompts.agent_prompt) > 25
 
 
 def test_bad_bibliography():
     with pytest.raises(requests.exceptions.HTTPError):
         get_bibliography("bad-bibliography")
 
 
@@ -140,14 +142,24 @@
 
 @pytest.mark.asyncio()
 async def test_async_query_noagent():
     response = await async_query("Why is KRAS studied?", "public:pqa-bench")
     assert isinstance(response, AnswerResponse)
 
 
+@pytest.mark.asyncio()
+async def test_async_scrape() -> None:
+    response = await async_scrape(
+        ScrapeRequest(query="10.1021/acs.jctc.2c01235", search_type="doi", limit="1")
+    )
+    assert response[-1]["c"].startswith(
+        "scrape"
+    ), "Expected scrape websocket trace to end with something like 'scrape-complete'."
+
+
 def test_check_dois() -> None:
     response = check_dois(
         dois=[
             "10.1126/science.1240517",
             "10.1126/science.1240517",  # NOTE: duplicate input DOI
             "10.1016/j.febslet.2014.11.036",
         ]
```

