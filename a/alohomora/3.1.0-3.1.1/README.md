# Comparing `tmp/alohomora-3.1.0.tar.gz` & `tmp/alohomora-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alohomora-3.1.0.tar", last modified: Wed Mar 13 18:17:53 2024, max compression
+gzip compressed data, was "alohomora-3.1.1.tar", last modified: Wed May 15 18:54:08 2024, max compression
```

## Comparing `alohomora-3.1.0.tar` & `alohomora-3.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:17:53.230152 alohomora-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-13 18:17:45.000000 alohomora-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-13 18:17:53.230152 alohomora-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-03-13 18:17:45.000000 alohomora-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:17:53.230152 alohomora-3.1.0/alohomora/
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-13 18:17:45.000000 alohomora-3.1.0/alohomora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-13 18:17:45.000000 alohomora-3.1.0/alohomora/keys.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10364 2024-03-13 18:17:45.000000 alohomora-3.1.0/alohomora/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36175 2024-03-13 18:17:45.000000 alohomora-3.1.0/alohomora/req.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-13 18:17:45.000000 alohomora-3.1.0/alohomora/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:17:53.230152 alohomora-3.1.0/alohomora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-13 18:17:53.000000 alohomora-3.1.0/alohomora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-13 18:17:53.000000 alohomora-3.1.0/alohomora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 18:17:53.000000 alohomora-3.1.0/alohomora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-13 18:17:53.000000 alohomora-3.1.0/alohomora.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-13 18:17:53.000000 alohomora-3.1.0/alohomora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-13 18:17:53.000000 alohomora-3.1.0/alohomora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-13 18:17:53.230152 alohomora-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-13 18:17:45.000000 alohomora-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:08.897765 alohomora-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 18:53:59.000000 alohomora-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-15 18:54:08.897765 alohomora-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-15 18:53:59.000000 alohomora-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:08.897765 alohomora-3.1.1/alohomora/
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-15 18:53:59.000000 alohomora-3.1.1/alohomora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-15 18:53:59.000000 alohomora-3.1.1/alohomora/keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10364 2024-05-15 18:53:59.000000 alohomora-3.1.1/alohomora/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36850 2024-05-15 18:53:59.000000 alohomora-3.1.1/alohomora/req.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-15 18:53:59.000000 alohomora-3.1.1/alohomora/saml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:54:08.897765 alohomora-3.1.1/alohomora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-15 18:54:08.000000 alohomora-3.1.1/alohomora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-15 18:54:08.000000 alohomora-3.1.1/alohomora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:54:08.000000 alohomora-3.1.1/alohomora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 18:54:08.000000 alohomora-3.1.1/alohomora.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 18:54:08.000000 alohomora-3.1.1/alohomora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 18:54:08.000000 alohomora-3.1.1/alohomora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 18:54:08.901765 alohomora-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-15 18:53:59.000000 alohomora-3.1.1/setup.py
```

### Comparing `alohomora-3.1.0/LICENSE` & `alohomora-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alohomora-3.1.0/PKG-INFO` & `alohomora-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: alohomora
-Version: 3.1.0
+Version: 3.1.1
 Summary: Get AWS API keys for a SAML-federated identity
 Home-page: https://github.com/Viasat/alohomora
 Author: Viasat
 Author-email: vice-support@viasat.com
-License: (c) 2022 Viasat, Inc. See the LICENSE file for more details.
+License: (c) 2024 Viasat, Inc. See the LICENSE file for more details.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.3.1
 Requires-Dist: beautifulsoup4>=4.5.1
 Requires-Dist: requests>=2.11.1
 Provides-Extra: fido2
 Requires-Dist: fido2==0.9.3; extra == "fido2"
```

### Comparing `alohomora-3.1.0/README.md` & `alohomora-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alohomora-3.1.0/alohomora/__init__.py` & `alohomora-3.1.1/alohomora/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
-__version__ = '3.1.0'
+__version__ = '3.1.1'
 __author__ = 'Viasat'
 __author_email__ = 'vice-support@viasat.com'
-__license__ = '(c) 2022 Viasat, Inc. See the LICENSE file for more details.'
+__license__ = '(c) 2024 Viasat, Inc. See the LICENSE file for more details.'
 __url__ = 'https://github.com/Viasat/alohomora'
 __description__ = 'Get AWS API keys for a SAML-federated identity'
 
 
 def die(msg):
     """Exit with non-zero and a message"""
     print(msg)
```

### Comparing `alohomora-3.1.0/alohomora/keys.py` & `alohomora-3.1.1/alohomora/keys.py`

 * *Files identical despite different names*

### Comparing `alohomora-3.1.0/alohomora/main.py` & `alohomora-3.1.1/alohomora/main.py`

 * *Files identical despite different names*

### Comparing `alohomora-3.1.0/alohomora/req.py` & `alohomora-3.1.1/alohomora/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import re
 import json
 import logging
 import time
 import os
 import base64
+from datetime import datetime, timedelta
 from http.cookiejar import LWPCookieJar
 
 try:
     import urlparse
 except ImportError:
     import urllib.parse as urlparse
 
@@ -802,13 +803,22 @@
             pass
         LOG.debug("Pre cookie jar: %s", self.session.cookies)
         LOG.debug("Fetching from URL: %s", url)
         response = func(url, data=data, headers=headers)
         LOG.debug("Post cookie jar: %s", self.session.cookies)
         LOG.debug("Request headers: %s", response.request.headers)
         LOG.debug("Response headers: %s", response.headers)
+        # On Windows the python builtin cookiejar chokes on a returned timestamp
+        # in the DUO status cookie.  It is set to expire far in the future in the
+        # year 9999.  Windows can not parse this timestamp, so we overwite it with
+        # an expiration 30 days in the future so it is parsable in Windows.
+        future_ts = (datetime.now() + timedelta(days=30)).timestamp()
+        for cookie in self.session.cookies:
+            if cookie.expires and cookie.expires > future_ts:
+                LOG.debug(f"rewrite coookie expires from: {cookie.expires} to: {future_ts}")
+                cookie.expires = future_ts
         self.session.cookies.save(ignore_discard=True, ignore_expires=True)
         if soup:
             the_soup = BeautifulSoup(response.text, 'html.parser')
         else:
             the_soup = None
         return (response, the_soup)
```

### Comparing `alohomora-3.1.0/alohomora/saml.py` & `alohomora-3.1.1/alohomora/saml.py`

 * *Files identical despite different names*

### Comparing `alohomora-3.1.0/alohomora.egg-info/PKG-INFO` & `alohomora-3.1.1/alohomora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: alohomora
-Version: 3.1.0
+Version: 3.1.1
 Summary: Get AWS API keys for a SAML-federated identity
 Home-page: https://github.com/Viasat/alohomora
 Author: Viasat
 Author-email: vice-support@viasat.com
-License: (c) 2022 Viasat, Inc. See the LICENSE file for more details.
+License: (c) 2024 Viasat, Inc. See the LICENSE file for more details.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3>=1.3.1
 Requires-Dist: beautifulsoup4>=4.5.1
 Requires-Dist: requests>=2.11.1
 Provides-Extra: fido2
 Requires-Dist: fido2==0.9.3; extra == "fido2"
```

### Comparing `alohomora-3.1.0/setup.py` & `alohomora-3.1.1/setup.py`

 * *Files identical despite different names*

