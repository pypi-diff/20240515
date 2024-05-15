# Comparing `tmp/ibm-eventnotifications-0.5.0.tar.gz` & `tmp/ibm-eventnotifications-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-eventnotifications-0.5.0.tar", last modified: Fri May  3 07:39:11 2024, max compression
+gzip compressed data, was "ibm-eventnotifications-0.5.1.tar", last modified: Wed May 15 14:08:53 2024, max compression
```

## Comparing `ibm-eventnotifications-0.5.0.tar` & `ibm-eventnotifications-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    37297 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    36258 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/ibm_eventnotifications/
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   534941 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/event_notifications_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      667 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)    37297 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      512 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2024-05-03 07:39:11.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-03 07:37:18.000000 ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      149 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-03 07:39:11.769153 ibm-eventnotifications-0.5.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2680 2024-05-03 07:36:51.000000 ibm-eventnotifications-0.5.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-15 14:08:53.288360 ibm-eventnotifications-0.5.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37297 2024-05-15 14:08:53.288360 ibm-eventnotifications-0.5.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36258 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-15 14:08:53.288360 ibm-eventnotifications-0.5.1/ibm_eventnotifications/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   537554 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications/event_notifications_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      667 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-15 14:08:53.288360 ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)    37297 2024-05-15 14:08:53.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      512 2024-05-15 14:08:53.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-15 14:08:53.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-05-15 14:08:53.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2024-05-15 14:08:53.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-15 14:07:05.000000 ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      149 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-15 14:08:53.288360 ibm-eventnotifications-0.5.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2680 2024-05-15 14:06:36.000000 ibm-eventnotifications-0.5.1/setup.py
```

### Comparing `ibm-eventnotifications-0.5.0/LICENSE` & `ibm-eventnotifications-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.5.0/PKG-INFO` & `ibm-eventnotifications-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-eventnotifications
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python server SDK for IBM Cloud Event Notifications service
 Home-page: https://github.com/IBM/event-notifications-python-admin-sdk
 Author: IBM
 Author-email: Notifications-prod@ibm.com
 License: Apache 2.0
 Keywords: ibm_eventnotifications
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IBM Cloud Event Notifications Python Admin SDK 0.5.0
+# IBM Cloud Event Notifications Python Admin SDK 0.5.1
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -62,19 +62,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.5.0"
+pip install --upgrade "ibm_eventnotifications>=0.5.1"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.5.0"
+easy_install --upgrade "ibm_eventnotifications>=0.5.1"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
```

### Comparing `ibm-eventnotifications-0.5.0/README.md` & `ibm-eventnotifications-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# IBM Cloud Event Notifications Python Admin SDK 0.5.0
+# IBM Cloud Event Notifications Python Admin SDK 0.5.1
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -37,19 +37,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.5.0"
+pip install --upgrade "ibm_eventnotifications>=0.5.1"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.5.0"
+easy_install --upgrade "ibm_eventnotifications>=0.5.1"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
```

### Comparing `ibm-eventnotifications-0.5.0/ibm_eventnotifications/__init__.py` & `ibm-eventnotifications-0.5.1/ibm_eventnotifications/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.5.0/ibm_eventnotifications/common.py` & `ibm-eventnotifications-0.5.1/ibm_eventnotifications/common.py`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.5.0/ibm_eventnotifications/event_notifications_v1.py` & `ibm-eventnotifications-0.5.1/ibm_eventnotifications/event_notifications_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -5801,45 +5801,45 @@
         return not self == other
 
 
 class SMTPConfig:
     """
     Payload describing a SMTP configuration.
 
-    :attr DKIMAttributes dkim: (optional) The DKIM attributes.
+    :attr SMTPDKIMAttributes dkim: (optional) The SMTP DKIM attributes.
     :attr ENAuthAttributes en_authorization: (optional) The en_authorization
           attributes.
     :attr SPFAttributes spf: (optional) The SPF attributes.
     """
 
     def __init__(
         self,
         *,
-        dkim: 'DKIMAttributes' = None,
+        dkim: 'SMTPDKIMAttributes' = None,
         en_authorization: 'ENAuthAttributes' = None,
         spf: 'SPFAttributes' = None,
     ) -> None:
         """
         Initialize a SMTPConfig object.
 
-        :param DKIMAttributes dkim: (optional) The DKIM attributes.
+        :param SMTPDKIMAttributes dkim: (optional) The SMTP DKIM attributes.
         :param ENAuthAttributes en_authorization: (optional) The en_authorization
                attributes.
         :param SPFAttributes spf: (optional) The SPF attributes.
         """
         self.dkim = dkim
         self.en_authorization = en_authorization
         self.spf = spf
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'SMTPConfig':
         """Initialize a SMTPConfig object from a json dictionary."""
         args = {}
         if 'dkim' in _dict:
-            args['dkim'] = DKIMAttributes.from_dict(_dict.get('dkim'))
+            args['dkim'] = SMTPDKIMAttributes.from_dict(_dict.get('dkim'))
         if 'en_authorization' in _dict:
             args['en_authorization'] = ENAuthAttributes.from_dict(_dict.get('en_authorization'))
         if 'spf' in _dict:
             args['spf'] = SPFAttributes.from_dict(_dict.get('spf'))
         return cls(**args)
 
     @classmethod
@@ -6235,14 +6235,88 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'SMTPCreateResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class SMTPDKIMAttributes:
+    """
+    The SMTP DKIM attributes.
+
+    :attr str txt_name: (optional) DMIM text name.
+    :attr str txt_value: (optional) DMIM text value.
+    :attr str verification: (optional) DKIM verification.
+    """
+
+    def __init__(
+        self,
+        *,
+        txt_name: str = None,
+        txt_value: str = None,
+        verification: str = None,
+    ) -> None:
+        """
+        Initialize a SMTPDKIMAttributes object.
+
+        :param str txt_name: (optional) DMIM text name.
+        :param str txt_value: (optional) DMIM text value.
+        :param str verification: (optional) DKIM verification.
+        """
+        self.txt_name = txt_name
+        self.txt_value = txt_value
+        self.verification = verification
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'SMTPDKIMAttributes':
+        """Initialize a SMTPDKIMAttributes object from a json dictionary."""
+        args = {}
+        if 'txt_name' in _dict:
+            args['txt_name'] = _dict.get('txt_name')
+        if 'txt_value' in _dict:
+            args['txt_value'] = _dict.get('txt_value')
+        if 'verification' in _dict:
+            args['verification'] = _dict.get('verification')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a SMTPDKIMAttributes object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'txt_name') and self.txt_name is not None:
+            _dict['txt_name'] = self.txt_name
+        if hasattr(self, 'txt_value') and self.txt_value is not None:
+            _dict['txt_value'] = self.txt_value
+        if hasattr(self, 'verification') and self.verification is not None:
+            _dict['verification'] = self.verification
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this SMTPDKIMAttributes object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'SMTPDKIMAttributes') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'SMTPDKIMAttributes') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class SMTPUser:
     """
     Payload describing a SMTP User.
 
     :attr str id: Id.
     :attr str smtp_config_id: SMTP confg Id.
     :attr str description: SMTP User description.
```

### Comparing `ibm-eventnotifications-0.5.0/ibm_eventnotifications/version.py` & `ibm-eventnotifications-0.5.1/ibm_eventnotifications/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_eventnotifications
 """
-__version__ = '0.5.0'
+__version__ = '0.5.1'
```

### Comparing `ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/PKG-INFO` & `ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-eventnotifications
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python server SDK for IBM Cloud Event Notifications service
 Home-page: https://github.com/IBM/event-notifications-python-admin-sdk
 Author: IBM
 Author-email: Notifications-prod@ibm.com
 License: Apache 2.0
 Keywords: ibm_eventnotifications
 Platform: UNKNOWN
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# IBM Cloud Event Notifications Python Admin SDK 0.5.0
+# IBM Cloud Event Notifications Python Admin SDK 0.5.1
 
 Python client library to interact with various [IBM Cloud Event Notifications APIs](https://cloud.ibm.com/apidocs?category=event-notifications).
 
 ## Table of Contents
 
 <!-- toc -->
 
@@ -62,19 +62,19 @@
 * Python 3.6 or above.
 
 ## Installation
 
 
 To install, use pip or easy_install:
 ```bash
-pip install --upgrade "ibm_eventnotifications>=0.5.0"
+pip install --upgrade "ibm_eventnotifications>=0.5.1"
 ```
 or
 ```bash
-easy_install --upgrade "ibm_eventnotifications>=0.5.0"
+easy_install --upgrade "ibm_eventnotifications>=0.5.1"
 ```
 
 ## Initialize SDK
 Initialize the sdk to connect with your Event Notifications service instance.
 
 ```py
 from ibm_eventnotifications.event_notifications_v1 import EventNotificationsV1
```

### Comparing `ibm-eventnotifications-0.5.0/ibm_eventnotifications.egg-info/SOURCES.txt` & `ibm-eventnotifications-0.5.1/ibm_eventnotifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-eventnotifications-0.5.0/setup.py` & `ibm-eventnotifications-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 PACKAGE_NAME = 'ibm_eventnotifications'
 PACKAGE_DESC = 'Python server SDK for IBM Cloud Event Notifications service'
 
 with open('requirements.txt') as f:
     install_requires = [
         str(req) for req in pkg_resources.parse_requirements(f)
     ]
```

