# Comparing `tmp/cruds-1.0.2.tar.gz` & `tmp/cruds-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruds-1.0.2.tar", last modified: Thu Apr 11 19:50:15 2024, max compression
+gzip compressed data, was "cruds-1.1.0.tar", last modified: Tue May 14 12:17:21 2024, max compression
```

## Comparing `cruds-1.0.2.tar` & `cruds-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:50:15.406464 cruds-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:50:12.000000 cruds-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-11 19:50:15.406464 cruds-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-11 19:50:12.000000 cruds-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:50:15.406464 cruds-1.0.2/cruds/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-11 19:50:12.000000 cruds-1.0.2/cruds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-11 19:50:12.000000 cruds-1.0.2/cruds/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:50:15.406464 cruds-1.0.2/cruds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-11 19:50:15.000000 cruds-1.0.2/cruds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-11 19:50:15.000000 cruds-1.0.2/cruds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:50:15.000000 cruds-1.0.2/cruds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 19:50:15.000000 cruds-1.0.2/cruds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 19:50:15.000000 cruds-1.0.2/cruds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-11 19:50:15.406464 cruds-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 19:50:12.000000 cruds-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:50:15.406464 cruds-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:50:12.000000 cruds-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-11 19:50:12.000000 cruds-1.0.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:17:21.110457 cruds-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-14 12:17:17.000000 cruds-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-14 12:17:21.110457 cruds-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-14 12:17:17.000000 cruds-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:17:21.106457 cruds-1.1.0/cruds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-14 12:17:17.000000 cruds-1.1.0/cruds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-14 12:17:17.000000 cruds-1.1.0/cruds/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-14 12:17:17.000000 cruds-1.1.0/cruds/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 12:17:17.000000 cruds-1.1.0/cruds/interface_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:17:21.110457 cruds-1.1.0/cruds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-14 12:17:21.000000 cruds-1.1.0/cruds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-14 12:17:21.000000 cruds-1.1.0/cruds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:17:21.000000 cruds-1.1.0/cruds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 12:17:21.000000 cruds-1.1.0/cruds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 12:17:21.000000 cruds-1.1.0/cruds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-14 12:17:21.110457 cruds-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 12:17:17.000000 cruds-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:17:21.106457 cruds-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:17:17.000000 cruds-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:17:21.110457 cruds-1.1.0/tests/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:17:17.000000 cruds-1.1.0/tests/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17979 2024-05-14 12:17:17.000000 cruds-1.1.0/tests/interfaces/test_planhat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-14 12:17:17.000000 cruds-1.1.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-14 12:17:17.000000 cruds-1.1.0/tests/test_interface.py
```

### Comparing `cruds-1.0.2/LICENSE` & `cruds-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cruds-1.0.2/PKG-INFO` & `cruds-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,93 @@
-Metadata-Version: 2.1
-Name: cruds
-Version: 1.0.2
-Summary: CRUDs is a simple high level library for Humans, inspired by Python Requests
-Home-page: https://github.com/johnbrandborg/cruds
-Author: John Brandborg
-Author-email: john.brandborg+pypi@pm.me
-License: MIT
-Project-URL: Source, https://github.com/johnbrandborg/cruds
-Project-URL: Tracker, https://github.com/johnbrandborg/cruds/issues
-Keywords: rest api crud http https
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: certifi
-Requires-Dist: urllib3
-Provides-Extra: develop
-Requires-Dist: flake8; extra == "develop"
-Requires-Dist: pytest; extra == "develop"
-Requires-Dist: pytest-cov; extra == "develop"
-
 # CRUDs
-[![Python appliction](https://github.com/johnbrandborg/cruds/workflows/Python%20application/badge.svg)](https://github.com/johnbrandborg/cruds/actions?query=workflow%3A%22Python+application%22)
+[![Development](https://github.com/johnbrandborg/cruds/actions/workflows/development.yml/badge.svg)](https://github.com/johnbrandborg/cruds/actions/workflows/development.yml)
 [![PyPI version](https://badge.fury.io/py/cruds.svg)](https://pypi.org/project/cruds/)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=johnbrandborg_cruds&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=johnbrandborg_cruds)
 
 CRUDs is a simple high level library for Humans, inspired by [Python Requests](https://requests.readthedocs.io/en/latest/)
+and written using [URLLib3 Team](https://github.com/urllib3).
 
 ```python
 >>> import cruds
 >>> catfact_ninja = cruds.Client(host="https://catfact.ninja/")
 >>> data = catfact_ninja.read("fact")
+>>> print(data)
 ```
 
-Interact with RESTful API using Create, Read, Update and Delete requests.
-Focus on using Python data types instead of worrying about serialization.
-Authentication, timeouts, retries, and rate limit back-off are all built in
-and can be adjusted.
+Interact with RESTful APIs using Create, Read, Update and Delete requests quickly,
+easily, and safely.
+
+Features:
+ * Authentication with a bearer token or username and password
+ * Data serialization/deserialize (Only JSON format)
+ * Request parameters as Dictionaries and automatically URL encoded
+ * Default connection timeout (300 seconds)
+ * Raises exceptions on bad status codes (Can be white listed)
+ * Retries with back-off
+ * SSL Verification
+ * Logging for monitoring
+ * Interfaces as Configuration
 
 ### Installation
 
-You can install the client using PIP like so.
+To install a stable version use [PyPI](https://pypi.org/project/cruds/).
 
 ```bash
 pip install cruds
 ```
 
+### Usage
+
+All features can be adjusted on the Client to suit most needs.
+
+```python
+from cruds import Client
+
+# Authentication with Username and Password
+api = Client(host="https://localhost/api/v1/",
+             auth=("username", "password"))
+
+# Authentication with Token
+api = Client(host="https://localhost/api/v1/",
+             auth="bearer-token")
+
+# Send and receive raw data and ignore bad status codes
+api = Client(host="https://localhost/api/v1/",
+             serialize=False,
+             raise_status=False)
+
+# Disable SSL Verification
+api = Client(host="https://localhost/api/v1/",
+             verify_ssl=False)
+```
+
 ### Logging
 
 If you want to see logging set the level using the standard logging interface.
 DEBUG will show you URLLib3, but INFO will give you general information from
-the cruds.
+the CRUDs Client.
 
 ``` python
->>> import logging
->>> import cruds
->>> logging.basicConfig(level=logging.INFO)
+import logging
+import cruds
+logging.basicConfig(level=logging.INFO)
 ```
 
 ### Extensibility
 
-The library has been created with extensibility in mind.  You can Sub Class Client
-for example and add the logic requirements needed to make the requests.
+The library has been created with extensibility in mind.  There is two ways that
+this can be done:
+
+1. Subclass the Client and add methods
+2. Interface as Configuration  (More Advanced)
+
+**Subclass Client**
+
+The approach is to create a new class and add the logic requirements needed to
+make the requests.
 
 ```python
 from cruds import Client
 
 class CatFactNinja(Client):
     """Cat Fact Ninja Interface"""
 
@@ -99,15 +102,38 @@
         """ Get a Fact about Cats"""
         return self.read(self._fact_uri)
 
 cat = CatFactNinja()
 print(cat.fact)
 ```
 
-## Todo List
+**Interface as Configuration**
+
+CRUDs supports creating interfaces with large amounts of models as configuration.
+This significantly reduces the amount of python coding needed, and the common
+methods can be reused.
+
+Within the CRUDs package pre-configured Interfaces have been created.  To use an
+Interface import them from `cruds.interfaces`
+
+Currently available:
+* Planhat - https://docs.planhat.com/
+
+Example:
+```python
+from cruds.interfaces.planhat import Planhat
+
+planhat = Planhat(api_token="9PhAfMO3WllHUmmhJA4eO3tJPhDck1aKLvQ5osvNUfKYdJ7H")
+
+help(planhat)
+```
+
+
+## To Do List
 - [ ] OAuth Client for Authentication
+- [X] Interfaces as Configuration
 
 ## License
-cruds is released under the MIT License. See the bundled LICENSE file for details.
+CRUDs is released under the MIT License. See the bundled LICENSE file for details.
 
 ## Credits
 * [URLLib3 Team](https://github.com/urllib3)
```

### Comparing `cruds-1.0.2/cruds/__init__.py` & `cruds-1.1.0/cruds/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
-RESTful is a simple API library for Humans, inspired by Python Requests
+CRUDs is a simple high level library for Humans, inspired by Python Requests
+and written URLLib3.
 """
 
 from .core import Client
```

### Comparing `cruds-1.0.2/cruds/core.py` & `cruds-1.1.0/cruds/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Clients that can be used for easily accessing RESTful APIs
 """
 
+
 import logging
+from json.decoder import JSONDecodeError
 import sys
+
 from typing import Any, Dict, List, Union
 from urllib.parse import urlencode
 
 import certifi
 import urllib3
 
-logger = logging.getLogger(__name__)
+logger= logging.getLogger(__name__)
 
-DEFAULT_TIMEOUT = 20.0
+DEFAULT_TIMEOUT = 300.0
 
 
 class Client:
     """
     Represents an platform interface that supports CRUD operations as methods.
 
     Data supplied as Dictionaries are automatically serialised and deserialized
@@ -290,15 +293,15 @@
             ) -> Union[Dict[Any, Any], bytes]:
         """
         Processes the Responce from HTTP Requests in a standardize manner, and
         displays information.
         """
         logger.info(
             f"Method: {method}, Status Code: {response.status}, "
-            f"Data: {sys.getsizeof(response.data)} Bytes"
+            f"Memory: {sys.getsizeof(response.data)} Bytes"
         )
 
         if self.raise_status and response.status not in self.status_whitelist:
             if 400 <= response.status < 500:
                 error_type = "Client"
             elif 500 <= response.status < 600:
                 error_type = "Server"
@@ -306,11 +309,18 @@
                 error_type = None
 
             if error_type:
                 msg = f"{error_type} Error with status code {response.status}" \
                       f" Message: {response.data.decode('utf-8')}"
                 raise urllib3.exceptions.HTTPError(msg)
 
-        if self.serialize and 'application/json' in response.headers.get('Content-Type', ''):
-            return response.json()
+        if self.serialize:
+            if 'application/json' in response.headers.get('Content-Type', ''):
+                return response.json()
+
+            logger.warning("Response content type is not declared as JSON but serialize is enabled")
+            try:
+                return response.json()
+            except JSONDecodeError:
+                return response.data
 
         return response.data
```

### Comparing `cruds-1.0.2/setup.cfg` & `cruds-1.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 [metadata]
 name = cruds
-version = 1.0.2
+version = 1.1.0
 description = CRUDs is a simple high level library for Humans, inspired by Python Requests
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/johnbrandborg/cruds
 author = John Brandborg
 author_email = john.brandborg+pypi@pm.me
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
+	Environment :: Console
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries
-	Topic :: Software Development :: Testing
 	Topic :: Utilities
-keywords = rest api crud http https
+keywords = rest api crud http https planhat
 project_urls = 
 	Source=https://github.com/johnbrandborg/cruds
 	Tracker=https://github.com/johnbrandborg/cruds/issues
 
 [options]
 packages = find:
 install_requires = 
-	certifi
-	urllib3
-python_requires = >=3.8
+	certifi>=2024.2.2
+	urllib3>=2.2.1,<3.0.0
+	PyYAML>=6.0.1,<7.0.0
+	jsonschema>=4.21.1,<5.0.0
+python_requires = >=3.8,<4.0.0
+
+[options.package_data]
+cruds = 
+	*.yaml
 
 [options.extras_require]
 develop = 
 	flake8
 	pytest
 	pytest-cov
 
 [tool:pytest]
 addopts = --cov=. tests/
 
 [coverage:run]
+branch = True
 relative_files = True
 omit = 
 	env/*
 	.env/*
 	venv/*
 	tests/*
 	setup.py
```

