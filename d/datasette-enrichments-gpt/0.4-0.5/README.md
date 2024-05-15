# Comparing `tmp/datasette-enrichments-gpt-0.4.tar.gz` & `tmp/datasette_enrichments_gpt-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-enrichments-gpt-0.4.tar", last modified: Wed Apr 10 03:28:44 2024, max compression
+gzip compressed data, was "datasette_enrichments_gpt-0.5.tar", last modified: Wed May 15 21:49:43 2024, max compression
```

## Comparing `datasette-enrichments-gpt-0.4.tar` & `datasette_enrichments_gpt-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.741850 datasette-enrichments-gpt-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 03:28:44.741850 datasette-enrichments-gpt-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/templates/enrichment-gpt.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 03:28:44.000000 datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:28:44.741850 datasette-enrichments-gpt-0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:28:44.737850 datasette-enrichments-gpt-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 03:28:34.000000 datasette-enrichments-gpt-0.4/tests/test_enrichments_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:49:43.874145 datasette_enrichments_gpt-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 21:49:31.000000 datasette_enrichments_gpt-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-15 21:49:43.874145 datasette_enrichments_gpt-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-15 21:49:31.000000 datasette_enrichments_gpt-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:49:43.870145 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-15 21:49:31.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:49:43.870145 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 21:49:31.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt/templates/enrichment-gpt.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:49:43.870145 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-15 21:49:43.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-15 21:49:43.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:49:43.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 21:49:43.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 21:49:43.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 21:49:43.000000 datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-15 21:49:31.000000 datasette_enrichments_gpt-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:49:43.874145 datasette_enrichments_gpt-0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:49:43.870145 datasette_enrichments_gpt-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-15 21:49:31.000000 datasette_enrichments_gpt-0.5/tests/test_enrichments_gpt.py
```

### Comparing `datasette-enrichments-gpt-0.4/LICENSE` & `datasette_enrichments_gpt-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-enrichments-gpt-0.4/PKG-INFO` & `datasette_enrichments_gpt-0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments-gpt
-Version: 0.4
+Version: 0.5
 Summary: Datasette enrichment for analyzing row data using OpenAI's GPT models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-enrichments-gpt
 Project-URL: Changelog, https://github.com/datasette/datasette-enrichments-gpt/releases
 Project-URL: Issues, https://github.com/datasette/datasette-enrichments-gpt/issues
 Project-URL: CI, https://github.com/datasette/datasette-enrichments-gpt/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasette-enrichments>=0.2
+Requires-Dist: datasette-enrichments>=0.4.1
 Requires-Dist: sqlite-utils
 Provides-Extra: test
+Requires-Dist: datasette-test; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-recording; extra == "test"
 
 # datasette-enrichments-gpt
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-enrichments-gpt.svg)](https://pypi.org/project/datasette-enrichments-gpt/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-enrichments-gpt?include_prereleases&label=changelog)](https://github.com/datasette/datasette-enrichments-gpt/releases)
 [![Tests](https://github.com/datasette/datasette-enrichments-gpt/workflows/Test/badge.svg)](https://github.com/datasette/datasette-enrichments-gpt/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-enrichments-gpt/blob/main/LICENSE)
@@ -32,33 +34,27 @@
 
 Install this plugin in the same environment as Datasette.
 ```bash
 datasette install datasette-enrichments-gpt
 ```
 ## Configuration
 
-This plugin needs an OpenAI API key. Configure that in `metadata.yml` like so
-```yaml
-plugins:
-  datasette-enrichments-gpt:
-    api_key: sk-..
-```
-Or to avoid that key being visible on `/-/metadata` set it as an environment variable and use this:
-```yaml
-plugins:
-  datasette-enrichments-gpt:
-    api_key:
-      $env: OPENAI_API_KEY
+This plugin can optionally be configured with an [OpenAI API key](https://platform.openai.com/api-keys). You can set this as an environment variable:
+```bash
+export DATASETTE_SECRETS_OPENAPI_API_KEY=sk-..
 ```
+Or you can configure it using the [datasette-secrets](https://datasette.io/plugins/datasette-secrets) plugin.
+
+If you do not configure an OpenAI API key users will be asked to enter one any time they execute the enrichment. The key they provide will not be stored anywhere other than in-memory during the enrichment run.
 
 ## Usage
 
-Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4-turbo`, saving the result of the prompt in the specified column.
+Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4o`, saving the result of the prompt in the specified column.
 
-The plugin also provides `gpt-4-turbo vision`, which can run prompts against an image identified by a URL.
+The plugin also provides `gpt-4o vision`, which can run prompts against an image identified by a URL.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-gpt
 python3 -m venv venv
```

### Comparing `datasette-enrichments-gpt-0.4/README.md` & `datasette_enrichments_gpt-0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,33 +11,27 @@
 
 Install this plugin in the same environment as Datasette.
 ```bash
 datasette install datasette-enrichments-gpt
 ```
 ## Configuration
 
-This plugin needs an OpenAI API key. Configure that in `metadata.yml` like so
-```yaml
-plugins:
-  datasette-enrichments-gpt:
-    api_key: sk-..
-```
-Or to avoid that key being visible on `/-/metadata` set it as an environment variable and use this:
-```yaml
-plugins:
-  datasette-enrichments-gpt:
-    api_key:
-      $env: OPENAI_API_KEY
+This plugin can optionally be configured with an [OpenAI API key](https://platform.openai.com/api-keys). You can set this as an environment variable:
+```bash
+export DATASETTE_SECRETS_OPENAPI_API_KEY=sk-..
 ```
+Or you can configure it using the [datasette-secrets](https://datasette.io/plugins/datasette-secrets) plugin.
+
+If you do not configure an OpenAI API key users will be asked to enter one any time they execute the enrichment. The key they provide will not be stored anywhere other than in-memory during the enrichment run.
 
 ## Usage
 
-Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4-turbo`, saving the result of the prompt in the specified column.
+Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4o`, saving the result of the prompt in the specified column.
 
-The plugin also provides `gpt-4-turbo vision`, which can run prompts against an image identified by a URL.
+The plugin also provides `gpt-4o vision`, which can run prompts against an image identified by a URL.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-gpt
 python3 -m venv venv
```

### Comparing `datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/__init__.py` & `datasette_enrichments_gpt-0.5/datasette_enrichments_gpt/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 from __future__ import annotations
 from datasette_enrichments import Enrichment
+from datasette_secrets import Secret
 from datasette import hookimpl
 from datasette.database import Database
 import httpx
 from typing import List, Optional
 from wtforms import (
     Form,
     StringField,
     TextAreaField,
     BooleanField,
-    PasswordField,
     SelectField,
 )
 from wtforms.validators import ValidationError, DataRequired
-import secrets
 import sqlite_utils
 
 
 @hookimpl
 def register_enrichments():
     return [GptEnrichment()]
 
 
 class GptEnrichment(Enrichment):
     name = "AI analysis with OpenAI GPT"
     slug = "gpt"
     description = "Analyze data using OpenAI's GPT models"
     runs_in_process = True
     batch_size = 1
+    secret = Secret(
+        name="OPENAI_API_KEY",
+        description="OpenAI API key",
+        obtain_label="Get an OpenAI API key",
+        obtain_url="https://platform.openai.com/api-keys",
+    )
 
     async def get_config_form(self, datasette, db, table):
         columns = await db.table_columns(table)
 
         # Default template uses all string columns
         default = " ".join("{{ COL }}".replace("COL", col) for col in columns)
 
         url_columns = [col for col in columns if "url" in col.lower()]
         image_url_suggestion = ""
         if url_columns:
             image_url_suggestion = "{{ %s }}" % url_columns[0]
 
         class ConfigForm(Form):
-            # Select box to pick model from gpt-3.5-turbo or gpt-4-turbo
             model = SelectField(
                 "Model",
                 choices=[
                     ("gpt-3.5-turbo", "gpt-3.5-turbo"),
-                    ("gpt-4-turbo", "gpt-4-turbo"),
-                    ("gpt-4-vision", "gpt-4-turbo vision"),
+                    ("gpt-4o", "gpt-4o"),
+                    ("gpt-4o-vision", "gpt-4o vision"),
                 ],
                 default="gpt-3.5-turbo",
             )
             prompt = TextAreaField(
                 "Prompt",
                 description="A template to run against each row to generate a prompt. Use {{ COL }} for columns.",
                 default=default,
                 validators=[DataRequired(message="Prompt is required.")],
                 render_kw={"style": "height: 8em"},
             )
             image_url = StringField(
                 "Image URL",
-                description="Image URL template. Only used with gpt-4-vision.",
+                description="Image URL template. Only used with gpt-4o-vision.",
                 default=image_url_suggestion,
             )
             system_prompt = TextAreaField(
                 "System prompt",
                 description="Instructions to apply to the main prompt. Can only be a static string, no {{ columns }}",
                 default="",
             )
@@ -86,38 +90,15 @@
                     and "json" not in field.data.lower()
                     and "json" not in self.system_prompt.data.lower()
                 ):
                     raise ValidationError(
                         'The prompt or system prompt must contain the word "JSON" when JSON format is selected.'
                     )
 
-        def stash_api_key(form, field):
-            if not (field.data or "").startswith("sk-"):
-                raise ValidationError("API key must start with sk-")
-            if not hasattr(datasette, "_enrichments_gpt_stashed_keys"):
-                datasette._enrichments_gpt_stashed_keys = {}
-            key = secrets.token_urlsafe(16)
-            datasette._enrichments_gpt_stashed_keys[key] = field.data
-            field.data = key
-
-        class ConfigFormWithKey(ConfigForm):
-            api_key = PasswordField(
-                "API key",
-                description="Your OpenAI API key",
-                validators=[
-                    DataRequired(message="API key is required."),
-                    stash_api_key,
-                ],
-                render_kw={"autocomplete": "off"},
-            )
-
-        plugin_config = datasette.plugin_config("datasette-enrichments-gpt") or {}
-        api_key = plugin_config.get("api_key")
-
-        return ConfigForm if api_key else ConfigFormWithKey
+        return ConfigForm
 
     async def initialize(self, datasette, db, table, config):
         # Ensure column exists
         output_column = config["output_column"]
 
         def add_column_if_not_exists(conn):
             db = sqlite_utils.Database(conn)
@@ -170,28 +151,28 @@
                 "role": "user",
                 "content": [
                     {"type": "text", "text": prompt},
                     {"type": "image_url", "image_url": {"url": image_url}},
                 ],
             }
         )
-        return await self._chat_completion(api_key, "gpt-4-turbo", messages)
+        return await self._chat_completion(api_key, "gpt-4o", messages)
 
     async def enrich_batch(
         self,
         datasette: "Datasette",
         db: Database,
         table: str,
         rows: List[dict],
         pks: List[str],
         config: dict,
         job_id: int,
     ) -> List[Optional[str]]:
         # API key should be in plugin settings OR pointed to by config
-        api_key = resolve_api_key(datasette, config)
+        api_key = await self.get_secret(datasette, config)
         if rows:
             row = rows[0]
         else:
             return
         prompt = config["prompt"] or ""
         system = config["system_prompt"] or None
         json_format = bool(config.get("json_format"))
@@ -202,43 +183,21 @@
                 "{{%s}}" % key, str(value or "")
             )
             if image_url:
                 image_url = image_url.replace(
                     "{{ %s }}" % key, str(value or "")
                 ).replace("{{%s}}" % key, str(value or ""))
         model = config["model"]
-        if model == "gpt-4-vision":
+        if model == "gpt-4o-vision":
             output = await self.gpt4_vision(api_key, prompt, image_url, system)
         else:
             output = await self.turbo_completion(
                 api_key, model, prompt, system, json_format
             )
         await db.execute_write(
             "update [{table}] set [{output_column}] = ? where {wheres}".format(
                 table=table,
                 output_column=output_column,
                 wheres=" and ".join('"{}" = ?'.format(pk) for pk in pks),
             ),
             [output] + list(row[pk] for pk in pks),
         )
-
-
-class ApiKeyError(Exception):
-    pass
-
-
-def resolve_api_key(datasette, config):
-    plugin_config = datasette.plugin_config("datasette-enrichments-gpt") or {}
-    api_key = plugin_config.get("api_key")
-    if api_key:
-        return api_key
-    # Look for it in config
-    api_key_name = config.get("api_key")
-    if not api_key_name:
-        raise ApiKeyError("No API key reference found in config")
-    # Look it up in the stash
-    if not hasattr(datasette, "_enrichments_gpt_stashed_keys"):
-        raise ApiKeyError("No API key stash found")
-    stashed_keys = datasette._enrichments_gpt_stashed_keys
-    if api_key_name not in stashed_keys:
-        raise ApiKeyError("No API key found in stash for {}".format(api_key_name))
-    return stashed_keys[api_key_name]
```

### Comparing `datasette-enrichments-gpt-0.4/datasette_enrichments_gpt/templates/enrichment-gpt.html` & `datasette_enrichments_gpt-0.5/datasette_enrichments_gpt/templates/enrichment-gpt.html`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 <script>
 const modelSelect = document.querySelector('#model');
 const divForImageUrlLabel = document.querySelector('label[for="image_url"]').parentNode;
 const divForImageUrlInput = document.querySelector('#image_url').parentNode;
 const divForJsonFormatLabel = document.querySelector('label[for="json_format"]').parentNode;
 const divForJsonFormatInput = document.querySelector('#json_format').parentNode;
 function handleModelChange() {
-    // If gpt-4-vision-preview, hide JSON, show image URL
-    if (modelSelect.value === 'gpt-4-vision') {
+    // If gpt-4o-vision, hide JSON, show image URL
+    if (modelSelect.value === 'gpt-4o-vision') {
         divForImageUrlLabel.style.display = '';
         divForImageUrlInput.style.display = '';
         divForJsonFormatLabel.style.display = 'none';
         divForJsonFormatInput.style.display = 'none';
     } else {
         divForImageUrlLabel.style.display = 'none';
         divForImageUrlInput.style.display = 'none';
```

### Comparing `datasette-enrichments-gpt-0.4/datasette_enrichments_gpt.egg-info/PKG-INFO` & `datasette_enrichments_gpt-0.5/datasette_enrichments_gpt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: datasette-enrichments-gpt
-Version: 0.4
+Version: 0.5
 Summary: Datasette enrichment for analyzing row data using OpenAI's GPT models
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/datasette/datasette-enrichments-gpt
 Project-URL: Changelog, https://github.com/datasette/datasette-enrichments-gpt/releases
 Project-URL: Issues, https://github.com/datasette/datasette-enrichments-gpt/issues
 Project-URL: CI, https://github.com/datasette/datasette-enrichments-gpt/actions
 Classifier: Framework :: Datasette
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: datasette-enrichments>=0.2
+Requires-Dist: datasette-enrichments>=0.4.1
 Requires-Dist: sqlite-utils
 Provides-Extra: test
+Requires-Dist: datasette-test; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-recording; extra == "test"
 
 # datasette-enrichments-gpt
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-enrichments-gpt.svg)](https://pypi.org/project/datasette-enrichments-gpt/)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-enrichments-gpt?include_prereleases&label=changelog)](https://github.com/datasette/datasette-enrichments-gpt/releases)
 [![Tests](https://github.com/datasette/datasette-enrichments-gpt/workflows/Test/badge.svg)](https://github.com/datasette/datasette-enrichments-gpt/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-enrichments-gpt/blob/main/LICENSE)
@@ -32,33 +34,27 @@
 
 Install this plugin in the same environment as Datasette.
 ```bash
 datasette install datasette-enrichments-gpt
 ```
 ## Configuration
 
-This plugin needs an OpenAI API key. Configure that in `metadata.yml` like so
-```yaml
-plugins:
-  datasette-enrichments-gpt:
-    api_key: sk-..
-```
-Or to avoid that key being visible on `/-/metadata` set it as an environment variable and use this:
-```yaml
-plugins:
-  datasette-enrichments-gpt:
-    api_key:
-      $env: OPENAI_API_KEY
+This plugin can optionally be configured with an [OpenAI API key](https://platform.openai.com/api-keys). You can set this as an environment variable:
+```bash
+export DATASETTE_SECRETS_OPENAPI_API_KEY=sk-..
 ```
+Or you can configure it using the [datasette-secrets](https://datasette.io/plugins/datasette-secrets) plugin.
+
+If you do not configure an OpenAI API key users will be asked to enter one any time they execute the enrichment. The key they provide will not be stored anywhere other than in-memory during the enrichment run.
 
 ## Usage
 
-Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4-turbo`, saving the result of the prompt in the specified column.
+Once installed, this plugin will allow users to select rows to enrich and run them through prompts using `gpt-3.5-turbo` or `gpt-4o`, saving the result of the prompt in the specified column.
 
-The plugin also provides `gpt-4-turbo vision`, which can run prompts against an image identified by a URL.
+The plugin also provides `gpt-4o vision`, which can run prompts against an image identified by a URL.
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-enrichments-gpt
 python3 -m venv venv
```

### Comparing `datasette-enrichments-gpt-0.4/pyproject.toml` & `datasette_enrichments_gpt-0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [project]
 name = "datasette-enrichments-gpt"
-version = "0.4"
+version = "0.5"
 description = "Datasette enrichment for analyzing row data using OpenAI's GPT models"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers=[
     "Framework :: Datasette",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "datasette-enrichments>=0.2",
+    "datasette-enrichments>=0.4.1",
     "sqlite-utils"
 ]
 
 [project.urls]
 Homepage = "https://github.com/datasette/datasette-enrichments-gpt"
 Changelog = "https://github.com/datasette/datasette-enrichments-gpt/releases"
 Issues = "https://github.com/datasette/datasette-enrichments-gpt/issues"
 CI = "https://github.com/datasette/datasette-enrichments-gpt/actions"
 
 [project.entry-points.datasette]
 enrichments_gpt = "datasette_enrichments_gpt"
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-asyncio"]
+test = ["datasette-test", "pytest", "pytest-asyncio", "pytest-recording"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
 
 [tool.setuptools.package-data]
 datasette_enrichments_gpt = ["templates/*"]
```

