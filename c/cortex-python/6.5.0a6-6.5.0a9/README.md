# Comparing `tmp/cortex_python-6.5.0a6.tar.gz` & `tmp/cortex_python-6.5.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_python-6.5.0a6.tar", max compression
+gzip compressed data, was "cortex_python-6.5.0a9.tar", max compression
```

## Comparing `cortex_python-6.5.0a6.tar` & `cortex_python-6.5.0a9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11368 2024-04-16 02:35:18.682957 cortex_python-6.5.0a6/LICENSE
--rw-r--r--   0        0        0     4274 2024-05-03 04:33:14.451244 cortex_python-6.5.0a6/README.md
--rw-r--r--   0        0        0      667 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/__init__.py
--rw-r--r--   0        0        0     1600 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/auth.py
--rw-r--r--   0        0        0     1989 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/camel.py
--rw-r--r--   0        0        0    27332 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/client.py
--rw-r--r--   0        0        0     3428 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/connection.py
--rw-r--r--   0        0        0      684 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/constant.py
--rw-r--r--   0        0        0     9669 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/content.py
--rw-r--r--   0        0        0     2532 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/env.py
--rw-r--r--   0        0        0     2477 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/exceptions.py
--rw-r--r--   0        0        0      675 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/experiment/__init__.py
--rw-r--r--   0        0        0     7794 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/experiment/local.py
--rw-r--r--   0        0        0    10717 2024-04-16 02:35:18.683956 cortex_python-6.5.0a6/cortex/experiment/model.py
--rw-r--r--   0        0        0    37474 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/experiment/remote.py
--rw-r--r--   0        0        0     3195 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/message.py
--rw-r--r--   0        0        0     3460 2024-05-03 13:56:51.034809 cortex_python-6.5.0a6/cortex/models.py
--rw-r--r--   0        0        0    10071 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/properties.py
--rw-r--r--   0        0        0     2517 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/secrets.py
--rw-r--r--   0        0        0    11766 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/serviceconnector.py
--rw-r--r--   0        0        0     4460 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/session.py
--rw-r--r--   0        0        0     8521 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/skill.py
--rw-r--r--   0        0        0     1347 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/timer.py
--rw-r--r--   0        0        0     1950 2024-04-16 02:35:18.684957 cortex_python-6.5.0a6/cortex/types.py
--rw-r--r--   0        0        0     9079 2024-04-16 02:35:18.685957 cortex_python-6.5.0a6/cortex/utils.py
--rw-r--r--   0        0        0     4410 2024-04-16 02:35:18.685957 cortex_python-6.5.0a6/cortex/viz.py
--rw-r--r--   0        0        0     2522 2024-05-03 21:59:50.142056 cortex_python-6.5.0a6/pyproject.toml
--rw-r--r--   0        0        0     5823 1970-01-01 00:00:00.000000 cortex_python-6.5.0a6/PKG-INFO
+-rw-r--r--   0        0        0    11368 2024-04-16 02:35:18.682957 cortex_python-6.5.0a9/LICENSE
+-rw-r--r--   0        0        0     5622 2024-05-15 04:59:52.279671 cortex_python-6.5.0a9/README.md
+-rw-r--r--   0        0        0      667 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/__init__.py
+-rw-r--r--   0        0        0     1600 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/auth.py
+-rw-r--r--   0        0        0     1989 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/camel.py
+-rw-r--r--   0        0        0    27419 2024-05-15 04:59:52.280671 cortex_python-6.5.0a9/cortex/client.py
+-rw-r--r--   0        0        0     3428 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/connection.py
+-rw-r--r--   0        0        0      684 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/constant.py
+-rw-r--r--   0        0        0     9669 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/content.py
+-rw-r--r--   0        0        0     2724 2024-05-15 04:59:52.280671 cortex_python-6.5.0a9/cortex/env.py
+-rw-r--r--   0        0        0     2477 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/exceptions.py
+-rw-r--r--   0        0        0      675 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/experiment/__init__.py
+-rw-r--r--   0        0        0     7794 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/experiment/local.py
+-rw-r--r--   0        0        0    10717 2024-04-16 02:35:18.683956 cortex_python-6.5.0a9/cortex/experiment/model.py
+-rw-r--r--   0        0        0    37474 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/experiment/remote.py
+-rw-r--r--   0        0        0     3195 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/message.py
+-rw-r--r--   0        0        0     3580 2024-05-15 04:59:52.280671 cortex_python-6.5.0a9/cortex/models.py
+-rw-r--r--   0        0        0    10071 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/properties.py
+-rw-r--r--   0        0        0     2517 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/secrets.py
+-rw-r--r--   0        0        0    11766 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/serviceconnector.py
+-rw-r--r--   0        0        0     4460 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/session.py
+-rw-r--r--   0        0        0     8521 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/skill.py
+-rw-r--r--   0        0        0     1347 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/timer.py
+-rw-r--r--   0        0        0     1950 2024-04-16 02:35:18.684957 cortex_python-6.5.0a9/cortex/types.py
+-rw-r--r--   0        0        0     9329 2024-05-15 04:59:52.280671 cortex_python-6.5.0a9/cortex/utils.py
+-rw-r--r--   0        0        0     4410 2024-04-16 02:35:18.685957 cortex_python-6.5.0a9/cortex/viz.py
+-rw-r--r--   0        0        0     2887 2024-05-15 13:35:36.590609 cortex_python-6.5.0a9/pyproject.toml
+-rw-r--r--   0        0        0     7172 1970-01-01 00:00:00.000000 cortex_python-6.5.0a9/PKG-INFO
```

### Comparing `cortex_python-6.5.0a6/LICENSE` & `cortex_python-6.5.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/README.md` & `cortex_python-6.5.0a9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -77,23 +77,38 @@
 - `make test` to run test suite
 
 To run an individual file or class method, use pytest. Example tests shown below:
 
 - file: `pytest test/unit/agent_test.py` 
 - class method: `pytest test/unit/agent_test.py::TestAgent::test_get_agent`
 
-#### Publishing an alpha build
+### Pre-release to staging
+**Note:** this repository using git tag for versionning
+
+1. Create and push an alpha release:
+
+```bash
+git tag -a 6.5.0a<N> -m 'alpha tag'
+git push --tags
+make dev.push
+```
+    This will build an alpha-tagged package.
+2. Merge `develop` to `staging` branch:
 
-Suppose you want to release new functionality so it can be installed without releasing a new official version. We need to use an alpha version in PyPi.
+```bash
+make stage
+```
 
-- we need to create and publish an alpha release:
-- get credentials to the `cortex-python` pypi CognitiveScale account (via lastpass)
-- run `make dev.push`. The alpha pre-release number (the N in X.Y.ZaN) with be determined automatically.
+3. In GitHub, create a pull request from `staging` to `master`.
+```
+git tag -a 6.5.0 -m 'rlease tag'
+git push --tags
+```
 
-### Contribution 
+### Contributing 
 
 After contributing to the library, and before you submit changes as a PR, please do the following
 
 1. Run unit tests via `make test`
 2. Manually verification (i.e. try the new changes out in Cortex) to make sure everything is going well. Not required, but highly encouraged.
 3. Bump up `setup.py` version and update the `CHANGELOG.md` 
 
@@ -114,29 +129,46 @@
 The package documentation is built with Sphinx and generates versioned documentation for all tag matching the `release/X.Y.Z` pattern and for the `master` branch. To build the documentation:
 
 ```bash
 make docs.multi
 ```
 The documentation will be rendered in HTML format under the `docs/_build/${VERSION}` directory.
 
-### Pre-release to staging
-**Note:** this repository using git tag for versionning
-
-1. Create and push an alpha release:
-
-```bash
-git tag -a 6.5.0a<N> -m 'alpha tag'
-git push --tags
-make dev.push
-```
-    This will build an alpha-tagged package.
-2. Merge `develop` to `staging` branch:
+## Configuring the client
 
-```bash
-make stage
-```
+There are four mechanisms for configuring a client connection. 
 
-3. In GitHub, create a pull request from `staging` to `master`.
-```
-git tag -a 6.5.0 -m 'rlease tag'
-git push --tags
-```
+1) Use `$HOME/.cortex/config` file setup via `cortex configure`.
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.client(verify_ssl_cert=True|False)
+   ```
+   
+2) Use environment variables CORTEX_URL, CORTEX_TOKEN, and CORTEX_PROJECT
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.client(verify_ssl_cert=True|False)
+   ```
+    
+This is a table of supported environment variables.
+
+These ENV vars are injected by the Sensa RUNTIME for use during skill startup.
+
+| Environment variables         | Description                                                             |
+|-------------------------------|-------------------------------------------------------------------------|
+| CORTEX_PERSONAL_ACCESS_CONFIG | JSON string containing a Pesonal Access Token obtained from the console UI |
+| CORTEX_CONFIG_DIR             | A folder containing the `config` created by the `cortex configure` command |
+| CORTEX_TOKEN                  | A JWT token generate by `cortex configure token` or provided during skill invokes |
+| CORTEX_PROJECT                | Project used during api requests                                        |
+| CORTEX_URL                    | URL for Sensa apis                                                      |
+
+3) Use method kwargs with `Cortex.client()` 
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.client(api_endpoint="<URL>", token="<token>", project="<project>", verify_ssl_cert=True|False)
+   ```
+   
+4) Using the skills invoke message, this allows for authentication using the caller's identity.
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.from_message({})    
+   ```
```

### Comparing `cortex_python-6.5.0a6/cortex/__init__.py` & `cortex_python-6.5.0a9/cortex/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/auth.py` & `cortex_python-6.5.0a9/cortex/auth.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/camel.py` & `cortex_python-6.5.0a9/cortex/camel.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/client.py` & `cortex_python-6.5.0a9/cortex/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,17 @@
 
     def _repr_pretty_(self, p, cycle):
         # pylint: disable=unused-argument,invalid-name
         p.text(str(self))
         p.text(f"Url: {self._url}\n")
         p.text(f"Project: {self._project}\n")
 
+    def __str__(self):
+        return f"Url: {self._url}\nProject: {self._project}\n"
+
     @property
     def experiments(self) -> ExperimentClient:
         """Returns a pre-initialised ExperimentClient whose project has been set to the project configured for the Cortex.client.
 
         If you want to access experiments for a project that is
         different from the one configured with Cortex.client, please use :meth:`cortex.client.Client.experiments_client` instead
```

### Comparing `cortex_python-6.5.0a6/cortex/connection.py` & `cortex_python-6.5.0a9/cortex/connection.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/constant.py` & `cortex_python-6.5.0a9/cortex/constant.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/content.py` & `cortex_python-6.5.0a9/cortex/content.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/env.py` & `cortex_python-6.5.0a9/cortex/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,45 +12,43 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import os
 import json
-from .utils import get_cortex_profile
+from .utils import get_cortex_profile, config_file_path
 from .exceptions import BadTokenException
 
-
-BAD_TOKEN_MSG = (
-    "Your Cortex credentials cannot be retrieved.",
-    "Check your profile settings with `cortex configure`.",
-)
-
-
 class CortexEnv:
     """
     Sets environment variables for Cortex.
     """
 
     def __init__(
         self,
         api_endpoint: str = None,
         token: str = None,
         config: dict = None,
         project: str = None,
         profile: str = None,
     ):
-        profile_inst = CortexEnv.get_cortex_profile(profile)
 
         cortex_token = token or os.getenv("CORTEX_TOKEN")
-        cortex_config = config or json.loads(
-            os.getenv("CORTEX_PERSONAL_ACCESS_CONFIG", json.dumps(profile_inst))
-        )
+
+        if config or os.getenv("CORTEX_PERSONAL_ACCESS_CONFIG") is not None:
+            cortex_config = config or json.loads(os.getenv("CORTEX_PERSONAL_ACCESS_CONFIG"))
+        else:
+            cortex_config = CortexEnv.get_cortex_profile(profile)
         if not cortex_token and not cortex_config:
-            raise BadTokenException(BAD_TOKEN_MSG)
+            bad_token_msg = (
+                f"Your Cortex credentials cannot be retrieved from: {config_file_path()} or CORTEX_TOKEN environment variable.",
+                "Create or update your profile settings with `cortex configure`.",
+            )
+            raise BadTokenException(bad_token_msg)
 
         self.api_endpoint = api_endpoint or os.getenv(
             "CORTEX_URL", cortex_config.get("url", None)
         )
         self.token = cortex_token
         self.config = cortex_config
         self.project = project or os.getenv(
```

### Comparing `cortex_python-6.5.0a6/cortex/exceptions.py` & `cortex_python-6.5.0a9/cortex/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/experiment/__init__.py` & `cortex_python-6.5.0a9/cortex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/experiment/local.py` & `cortex_python-6.5.0a9/cortex/experiment/local.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/experiment/model.py` & `cortex_python-6.5.0a9/cortex/experiment/model.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/experiment/remote.py` & `cortex_python-6.5.0a9/cortex/experiment/remote.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/message.py` & `cortex_python-6.5.0a9/cortex/message.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/models.py` & `cortex_python-6.5.0a9/cortex/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,18 @@
 class ModelClient(_Client):
     """
     Client for model registry, this class requires the `models_sdk` extras to be installed
     """
 
     def _setup_model_client(self, verify_ssl_cert=True, ttl="2h"):
         # Generate a JWT, this call stores the JWT in `_serviceconnector.jwt` ( meh )
-        token = generate_token(self._serviceconnector._config, verify_ssl_cert=verify_ssl_cert, validity=ttl)  # pylint: disable=protected-access
+        if self._serviceconnector.token is not None:
+            token = self._serviceconnector.token
+        else:
+            token = generate_token(self._serviceconnector._config, verify_ssl_cert=verify_ssl_cert, validity=ttl)  # pylint: disable=protected-access
         mlflow.set_tracking_uri(self._serviceconnector.url)
         os.environ['MLFLOW_TRACKING_URI'] = self._serviceconnector.url
         os.environ['MLFLOW_TRACKING_TOKEN'] = token
         # Following behavior from python requests https://requests.readthedocs.io/en/latest/user/advanced/#ssl-cert-verification
         if verify_ssl_cert is False:
             os.environ['MLFLOW_TRACKING_INSECURE_TLS'] = "true"
         elif isinstance(verify_ssl_cert, str):
```

### Comparing `cortex_python-6.5.0a6/cortex/properties.py` & `cortex_python-6.5.0a9/cortex/properties.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/secrets.py` & `cortex_python-6.5.0a9/cortex/secrets.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/serviceconnector.py` & `cortex_python-6.5.0a9/cortex/serviceconnector.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/session.py` & `cortex_python-6.5.0a9/cortex/session.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/skill.py` & `cortex_python-6.5.0a9/cortex/skill.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/timer.py` & `cortex_python-6.5.0a9/cortex/timer.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/types.py` & `cortex_python-6.5.0a9/cortex/types.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/cortex/utils.py` & `cortex_python-6.5.0a9/cortex/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 limitations under the License.
 """
 
 import json
 import base64
 import hashlib
 import logging
+import os
 import urllib.parse
 from collections import namedtuple
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Union
 
 import jwt
@@ -193,27 +194,34 @@
     except Exception as err:
         gen_token_msg = (
             "Unable to generate a JWT token, " "check PAT config or cortex profile: {}"
         ).format(err)
         raise BadTokenException(gen_token_msg) from err
 
 
+def config_file_path():
+    """
+    Return config file location.
+    """
+    return os.path.abspath(os.path.join(os.getenv("CORTEX_CONFIG_DIR", Path.home() / ".cortex"), "config"))
+
+
 def get_cortex_profile(profile_name=None):
     """
     Gets the current cortex profile or the profile that matches the optional given name.
     """
 
-    cortex_config_path = Path.home() / ".cortex" / "config"
-
-    if cortex_config_path.exists():
-        with cortex_config_path.open() as filed:
+    cortex_config_path = config_file_path()
+    print("#####", cortex_config_path)
+    if os.path.exists(cortex_config_path):
+        with open(cortex_config_path, encoding='utf-8') as filed:
             cortex_config = json.load(filed)
 
         if profile_name is None:
-            profile_name = cortex_config.get("currentProfile")
+            profile_name = cortex_config.get("currentProfile", "default")
 
         return cortex_config.get("profiles", {}).get(profile_name, {})
     return {}
 
 
 def get_logger(name):
     """
```

### Comparing `cortex_python-6.5.0a6/cortex/viz.py` & `cortex_python-6.5.0a9/cortex/viz.py`

 * *Files identical despite different names*

### Comparing `cortex_python-6.5.0a6/pyproject.toml` & `cortex_python-6.5.0a9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "cortex-python"
-version = "6.5.0a6"
+version = "6.5.0a9"
 description = "Python module for the Tecnotree Sensa Platform"
 authors = ["Tecnotree <support@tecnotree.com>"]
 readme = "README.md"
 packages = [{include='cortex/**/*.py'}]
 license = "Apache-2.0"
 
 [[tool.poetry.source]]
 name = "sensa"
 url = "https://cognitivescale.jfrog.io/artifactory/api/pypi/cognitivescale_local/simple/"
 priority = "explicit"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
+#strict = true
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 requests = ">=2.31.0,<3,"
 requests-toolbelt = ">=1.0.0,"
 pyyaml = ">=5.4.1,"
 python-dateutil = ">=2.8.2,<3,"
@@ -28,22 +29,23 @@
 pytimeparse2 = "^1.7.1"
 matplotlib = { version=">3,<4", optional=true}
 seaborn = { version=">0.13,<0.14", optional=true}
 setuptools = "*"  #  mlflow requires this https://github.com/mlflow/mlflow/issues/11330
 pandas = { version="<3", optional=true}
 ipython = { version=">=8.10,<9", optional=true}
 jinja2={ version="<4", optional=true}
-mlflow={ version=">1", optional=true}
+mlflow={ version=">2,<3", optional=true}
 
-# have to explicilty point these to the private repo
-certifai-evaluator-plugin={ version="^1.3.17", optional=true, source="sensa" }
-cortex-certifai-common={ version="^1.3.17", optional=true, source="sensa" }
-cortex_certifai_engine={ version="^1.3.17", optional=true, source="sensa" }
-cortex_certifai_model_sdk={ version="^1.3.17", optional=true, source="sensa" }
-cortex_certifai_scanner={ version="^1.3.17", optional=true, source="sensa" }
+# have to explicilty point these to the `sensa` private repo
+# this also causes pip to resolve these, so they MUST be added to the `certifai` extra as well.
+certifai-evaluator-plugin={ version="*", optional=true, source="sensa" }
+cortex-certifai-common={ version="*", optional=true, source="sensa" }
+cortex_certifai_engine={ version="*", optional=true, source="sensa" }
+cortex_certifai_model_sdk={ version="*", optional=true, source="sensa" }
+cortex_certifai_scanner={ version="*", optional=true, source="sensa" }
 
 [tool.poetry.group.dev.dependencies]
 tox = ">=4.0,<5.0"
 requests-mock = ">=1.10.0"
 pipdeptree = "^2.16.1"
 pytest = ">=8,<9"
 pylint = "*"  # TODO dill verision couldn't pin this
@@ -52,36 +54,28 @@
 black = "<25"
 sphinx = "^7.2.6"
 gitpython = "^3.1.42"
 sphinx-multiversion = "^0.2.4"
 sphinx-rtd-theme = "^2.0.0"
 sphinxcontrib-restbuilder = "^0.3"
 
+[tool.poetry.group.daemon]
+optional=true
+
 [tool.poetry.group.daemon.dependencies]
 flask="*"
 fastapi-cli="*"
 uvicorn="*"
 
-
-
-
-
-
-
-
-
-
-
-
-
 [tool.poetry.extras]
 # Basic dependencies for developing models within jupyter
 models_dev = ["mlflow","ipython", "jinja2", "matplotlib", "seaborn", "pandas"]
 # dependencies for running models as skills
 models_runtime=["mlflow"]
-#certifai evaluator plugin
-certifai=["certifai-evaluator-plugin"]
+# certifai evaluator plugin
+# cortex-certifai are transitive deps for the eval plugin, they are added here so pip/poetry/conda don't always attempt resolve them.
+certifai=["certifai-evaluator-plugin", "cortex-certifai-common", "cortex_certifai_engine", "cortex_certifai_model_sdk", "cortex_certifai_scanner"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 # Wrapper around poetry.core.masonry.api
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cortex_python-6.5.0a6/PKG-INFO` & `cortex_python-6.5.0a9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.5.0a6
+Version: 6.5.0a9
 Summary: Python module for the Tecnotree Sensa Platform
 License: Apache-2.0
 Author: Tecnotree
 Author-email: support@tecnotree.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: certifai
 Provides-Extra: models-dev
 Provides-Extra: models-runtime
-Requires-Dist: certifai-evaluator-plugin (>=1.3.17,<2.0.0) ; extra == "certifai"
-Requires-Dist: cortex-certifai-common (>=1.3.17,<2.0.0)
-Requires-Dist: cortex_certifai_engine (>=1.3.17,<2.0.0)
-Requires-Dist: cortex_certifai_model_sdk (>=1.3.17,<2.0.0)
-Requires-Dist: cortex_certifai_scanner (>=1.3.17,<2.0.0)
+Requires-Dist: certifai-evaluator-plugin ; extra == "certifai"
+Requires-Dist: cortex-certifai-common ; extra == "certifai"
+Requires-Dist: cortex_certifai_engine ; extra == "certifai"
+Requires-Dist: cortex_certifai_model_sdk ; extra == "certifai"
+Requires-Dist: cortex_certifai_scanner ; extra == "certifai"
 Requires-Dist: cuid (>=0.3,<0.4)
 Requires-Dist: dill (<=0.3.4)
 Requires-Dist: ipython (>=8.10,<9) ; extra == "models-dev"
 Requires-Dist: jinja2 (<4) ; extra == "models-dev"
 Requires-Dist: matplotlib (>3,<4) ; extra == "models-dev"
-Requires-Dist: mlflow (>1) ; extra == "models-dev" or extra == "models-runtime"
+Requires-Dist: mlflow (>2,<3) ; extra == "models-dev" or extra == "models-runtime"
 Requires-Dist: pandas (<3) ; extra == "models-dev"
 Requires-Dist: pyjwt[crypto] (<3)
 Requires-Dist: python-dateutil (>=2.8.2,<3)
 Requires-Dist: pytimeparse2 (>=1.7.1,<2.0.0)
 Requires-Dist: pyyaml (>=5.4.1)
 Requires-Dist: requests (>=2.31.0,<3)
 Requires-Dist: requests-toolbelt (>=1.0.0)
@@ -114,23 +114,38 @@
 - `make test` to run test suite
 
 To run an individual file or class method, use pytest. Example tests shown below:
 
 - file: `pytest test/unit/agent_test.py` 
 - class method: `pytest test/unit/agent_test.py::TestAgent::test_get_agent`
 
-#### Publishing an alpha build
+### Pre-release to staging
+**Note:** this repository using git tag for versionning
 
-Suppose you want to release new functionality so it can be installed without releasing a new official version. We need to use an alpha version in PyPi.
+1. Create and push an alpha release:
 
-- we need to create and publish an alpha release:
-- get credentials to the `cortex-python` pypi CognitiveScale account (via lastpass)
-- run `make dev.push`. The alpha pre-release number (the N in X.Y.ZaN) with be determined automatically.
+```bash
+git tag -a 6.5.0a<N> -m 'alpha tag'
+git push --tags
+make dev.push
+```
+    This will build an alpha-tagged package.
+2. Merge `develop` to `staging` branch:
 
-### Contribution 
+```bash
+make stage
+```
+
+3. In GitHub, create a pull request from `staging` to `master`.
+```
+git tag -a 6.5.0 -m 'rlease tag'
+git push --tags
+```
+
+### Contributing 
 
 After contributing to the library, and before you submit changes as a PR, please do the following
 
 1. Run unit tests via `make test`
 2. Manually verification (i.e. try the new changes out in Cortex) to make sure everything is going well. Not required, but highly encouraged.
 3. Bump up `setup.py` version and update the `CHANGELOG.md` 
 
@@ -151,30 +166,46 @@
 The package documentation is built with Sphinx and generates versioned documentation for all tag matching the `release/X.Y.Z` pattern and for the `master` branch. To build the documentation:
 
 ```bash
 make docs.multi
 ```
 The documentation will be rendered in HTML format under the `docs/_build/${VERSION}` directory.
 
-### Pre-release to staging
-**Note:** this repository using git tag for versionning
-
-1. Create and push an alpha release:
-
-```bash
-git tag -a 6.5.0a<N> -m 'alpha tag'
-git push --tags
-make dev.push
-```
-    This will build an alpha-tagged package.
-2. Merge `develop` to `staging` branch:
-
-```bash
-make stage
-```
+## Configuring the client
 
-3. In GitHub, create a pull request from `staging` to `master`.
-```
-git tag -a 6.5.0 -m 'rlease tag'
-git push --tags
-```
+There are four mechanisms for configuring a client connection. 
 
+1) Use `$HOME/.cortex/config` file setup via `cortex configure`.
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.client(verify_ssl_cert=True|False)
+   ```
+   
+2) Use environment variables CORTEX_URL, CORTEX_TOKEN, and CORTEX_PROJECT
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.client(verify_ssl_cert=True|False)
+   ```
+    
+This is a table of supported environment variables.
+
+These ENV vars are injected by the Sensa RUNTIME for use during skill startup.
+
+| Environment variables         | Description                                                             |
+|-------------------------------|-------------------------------------------------------------------------|
+| CORTEX_PERSONAL_ACCESS_CONFIG | JSON string containing a Pesonal Access Token obtained from the console UI |
+| CORTEX_CONFIG_DIR             | A folder containing the `config` created by the `cortex configure` command |
+| CORTEX_TOKEN                  | A JWT token generate by `cortex configure token` or provided during skill invokes |
+| CORTEX_PROJECT                | Project used during api requests                                        |
+| CORTEX_URL                    | URL for Sensa apis                                                      |
+
+3) Use method kwargs with `Cortex.client()` 
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.client(api_endpoint="<URL>", token="<token>", project="<project>", verify_ssl_cert=True|False)
+   ```
+   
+4) Using the skills invoke message, this allows for authentication using the caller's identity.
+    ```python
+   from cortex.client import Cortex
+   client=Cortex.from_message({})    
+   ```
```

