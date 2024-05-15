# Comparing `tmp/washpy-0.2.2.tar.gz` & `tmp/washpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "washpy-0.2.2.tar", max compression
+gzip compressed data, was "washpy-0.3.0.tar", max compression
```

## Comparing `washpy-0.2.2.tar` & `washpy-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0    42028 2024-04-23 21:57:43.954435 washpy-0.2.2/LICENSE
--rw-r--r--   0        0        0     2731 2024-05-01 15:14:30.938342 washpy-0.2.2/README.md
--rw-r--r--   0        0        0      526 2024-05-09 16:21:35.367515 washpy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      315 2024-04-23 21:57:43.991103 washpy-0.2.2/washpy/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-30 21:55:27.785903 washpy-0.2.2/washpy/authenticate.py
--rw-r--r--   0        0        0     3595 2024-04-30 22:11:51.271198 washpy-0.2.2/washpy/device_user.py
--rw-r--r--   0        0        0     1224 2024-04-30 21:21:21.958949 washpy-0.2.2/washpy/pExtended.py
--rw-r--r--   0        0        0      778 2024-04-30 22:06:54.530814 washpy-0.2.2/washpy/post_new_password.py
--rw-r--r--   0        0        0     6158 2024-04-30 21:12:46.347166 washpy-0.2.2/washpy/state.py
--rw-r--r--   0        0        0     3453 2024-04-23 21:57:43.987770 washpy-0.2.2/washpy/status.py
--rw-r--r--   0        0        0     3520 1970-01-01 00:00:00.000000 washpy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    42028 2024-05-14 21:13:05.974878 washpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3296 2024-05-15 18:58:32.047829 washpy-0.3.0/README.md
+-rw-r--r--   0        0        0      612 2024-05-14 23:15:44.787766 washpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-05-14 21:13:05.974878 washpy-0.3.0/washpy/__init__.py
+-rw-r--r--   0        0        0     2185 2024-05-14 21:13:05.978211 washpy-0.3.0/washpy/authenticate.py
+-rw-r--r--   0        0        0     9687 2024-05-15 18:36:09.024907 washpy-0.3.0/washpy/device_user.py
+-rw-r--r--   0        0        0     1224 2024-05-14 21:13:05.978211 washpy-0.3.0/washpy/pExtended.py
+-rw-r--r--   0        0        0     2585 2024-05-14 23:09:17.713438 washpy-0.3.0/washpy/permission.py
+-rw-r--r--   0        0        0      827 2024-05-15 11:13:09.808240 washpy-0.3.0/washpy/post_new_password.py
+-rw-r--r--   0        0        0      865 2024-05-15 17:42:51.893287 washpy-0.3.0/washpy/role.py
+-rw-r--r--   0        0        0     6215 2024-05-14 21:13:05.978211 washpy-0.3.0/washpy/state.py
+-rw-r--r--   0        0        0     6133 2024-05-14 23:13:12.557401 washpy-0.3.0/washpy/status.py
+-rw-r--r--   0        0        0     1077 2024-05-15 18:51:39.295645 washpy-0.3.0/washpy/user.py
+-rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 washpy-0.3.0/PKG-INFO
```

### Comparing `washpy-0.2.2/LICENSE` & `washpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `washpy-0.2.2/README.md` & `washpy-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 washpy offers a partial implementation of the Miele Professional IP Profile API.
 
 The project focusses on implementing the parts of the API
 for washing machines from Miele Professional.
 
 ## Getting started
 
+### Documentation
+
+Read the [documentation of washpy](https://johann-cm.codeberg.page/washpy/washpy.html).
+
 ## Installation
 
 [washpy is available on PyPI](https://pypi.org/project/washpy/),
 so washpy can be installed via `pip`, [poetry](https://python-poetry.org/), 
 or any other tool that interfaces with PyPI.
 
 ### Hardware setup
@@ -45,41 +49,65 @@
 
 On the KOM module, there exists the `Admin` default user,
 with the default password `""` (the empty string).
 
 I had to activate the admin user by changing its password:
 
 ```python
-from washpy import postNewPassword
+from washpy import post_new_password
 
-postNewPassword("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
+post_new_password(
+    "https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!"
+)
 ```
 
-#### Add new Account
+#### Add new User
+
+```python
+from washpy import DeviceUser
+from washpy.user import User
+
+d = DeviceUser(
+    "https://192.168.1.251/Devices/000116343328", "Admin", "verySecurePassword!"
+)
+
+user = User(
+    ID=102,
+    LoginName="MyUser",
+    Password="evenStrongerPassword!",
+    Description="My first User",
+    Roles=[1, 2],
+)
 
-TODO
+# user the Admin standard user to add a new user
+d.post_new_user(user)
+```
 
 #### Interact with a device
 
 The core of washpy is the `DeviceUser` class. Once constructed,
 it provides many methods to control the Miele device.
 
 The script
 ```python
 from washpy import DeviceUser
 
-my_device = DeviceUser("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
+my_device = DeviceUser(
+    "https://192.168.1.251/Devices/000116343328", "Admin", "verySecurePassword!"
+)
 
-print(my_device.get_State().Status)
+print(my_device.get_state().Status)
 ```
 will yield
 ```python
 <Status.RUNNING: 5>
 ```
 
+See also the [exapmles](examples) folder for more usage examples.
+
 ## Is there documentation of the IP Profile API?
 
 Yes, you have to request access to it from [Miele Professional](https://www.miele.com/en/com/index-pro.htm).
 
 ## known issues
 
 Do not upgrade requests, as it will upgrade to urllib3 version `2.x`.
```

### Comparing `washpy-0.2.2/pyproject.toml` & `washpy-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "washpy"
-version = "0.2.2"
+version = "0.3.0"
 description = "A partial implementation of the Miele Professional IP Profile API"
 authors = ["Johann Carl Meyer <info@johannc.de>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 repository = "https://codeberg.org/johann-cm/washpy"
+documentation = "https://johann-cm.codeberg.page/washpy/washpy.html"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "2.29.0"
 isodate = "^0.6.1"
 pydantic = "^2.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
+pdoc = "^14.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `washpy-0.2.2/washpy/authenticate.py` & `washpy-0.3.0/washpy/authenticate.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     """
 
 
 def authenticate(
     device_url: str, user: str, password: str
 ) -> Tuple[str, datetime.timedelta]:
     """
-    device_url: e.g. 'https://192.168.1.251/Devices/000116343328'
+    `device_url`: e.g. `'https://192.168.1.251/Devices/000116343328'`
 
-    user: e.g. 'MYUSER'
+    `user`: e.g. `'MYUSER'`
 
-    password e.g. 'verySecurePassword!'
+    `password`: e.g. `'verySecurePassword!'`
 
-    returns: a string, containing a bearer token, and a time duration for which the token is valid.
+    **returns**: a string, containing a bearer token, and a time duration for which the token is valid.
     If the token is used again within the valid time period, the valid time period is refreshed.
 
-    raises:
-        - NoUserException, if HTTP response code 401
-        - WrongCredentialsException, if HTTP response code 403
-        - LoginTimeoutException, if HTTP response code 429
-        - ValueError, else, and not HTTP code 200
+    **raises**:
+      - `NoUserException`, if HTTP response code 401
+      - `WrongCredentialsException`, if HTTP response code 403
+      - `LoginTimeoutException`, if HTTP response code 429
+      - `ValueError`, else, and not HTTP code 200
     """
     url = device_url + "/profSession"
 
     payload = json.dumps({"LoginName": user, "Password": password})
     headers = {"Content-Type": "application/json"}
 
     response = requests.request(
```

### Comparing `washpy-0.2.2/washpy/pExtended.py` & `washpy-0.3.0/washpy/pExtended.py`

 * *Files identical despite different names*

### Comparing `washpy-0.2.2/washpy/post_new_password.py` & `washpy-0.3.0/washpy/post_new_password.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 import json
 
 
 def post_new_password(
     device_url: str, user: str, password_old: str, password_new: str
 ) -> None:
     """
-    device_url: e.g. 'https://192.168.1.251/Devices/000116343328'
+    `device_url`: e.g. `'https://192.168.1.251/Devices/000116343328'`
 
-    user: e.g. 'MYUSER'
+    `user`: e.g. `'MYUSER'`
 
-    password_old: old password
+    `password_old`: old password
 
-    password_new: the new password to be set
+    `password_new`: the new password to be set
 
-    raises: ValueError, if the password change was unsuccessfull
+    **raises**: `ValueError`, if the password change was unsuccessfull
     """
     payload = json.dumps(
         {"LoginName": user, "Password": password_old, "PasswordNew": password_new}
     )
     headers = {"Content-Type": "application/json"}
 
+    url = device_url + "/profSession"
     response = requests.request(
-        "POST", device_url, headers=headers, data=payload, verify=False
+        "POST", url, headers=headers, data=payload, verify=False
     )
     if response.status_code != 204:
         raise ValueError(f"something went wrong: got HTTP response {response}")
```

### Comparing `washpy-0.2.2/washpy/state.py` & `washpy-0.3.0/washpy/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import isodate
 from pydantic import BaseModel
 from washpy.status import Status
 
 
 class StateModel(BaseModel):
     """
-    captures the output format of the /State endpoint.
+    captures the output format of the `/State` endpoint.
 
     For pExtended: the contents of the field are device specific.
     For the PWM 507 machine, look at the `pExtendedPWM507` class.
 
+    View `State` for more details on the class fields.
     """
 
     Status: Status
     ProgramID: int
     ProgramPhase: int
     SyncState: int
     pRemainingTime: str
```

### Comparing `washpy-0.2.2/PKG-INFO` & `washpy-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: washpy
-Version: 0.2.2
+Version: 0.3.0
 Summary: A partial implementation of the Miele Professional IP Profile API
 Home-page: https://codeberg.org/johann-cm/washpy
 License: LGPL-3.0-only
 Author: Johann Carl Meyer
 Author-email: info@johannc.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (==2.29.0)
+Project-URL: Documentation, https://johann-cm.codeberg.page/washpy/washpy.html
 Project-URL: Repository, https://codeberg.org/johann-cm/washpy
 Description-Content-Type: text/markdown
 
 # washpy
 
 [![PyPI](https://img.shields.io/pypi/v/washpy.svg)](https://pypi.org/project/washpy/)
 
 washpy offers a partial implementation of the Miele Professional IP Profile API.
 
 The project focusses on implementing the parts of the API
 for washing machines from Miele Professional.
 
 ## Getting started
 
+### Documentation
+
+Read the [documentation of washpy](https://johann-cm.codeberg.page/washpy/washpy.html).
+
 ## Installation
 
 [washpy is available on PyPI](https://pypi.org/project/washpy/),
 so washpy can be installed via `pip`, [poetry](https://python-poetry.org/), 
 or any other tool that interfaces with PyPI.
 
 ### Hardware setup
@@ -65,41 +70,65 @@
 
 On the KOM module, there exists the `Admin` default user,
 with the default password `""` (the empty string).
 
 I had to activate the admin user by changing its password:
 
 ```python
-from washpy import postNewPassword
+from washpy import post_new_password
 
-postNewPassword("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
+post_new_password(
+    "https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!"
+)
 ```
 
-#### Add new Account
+#### Add new User
+
+```python
+from washpy import DeviceUser
+from washpy.user import User
+
+d = DeviceUser(
+    "https://192.168.1.251/Devices/000116343328", "Admin", "verySecurePassword!"
+)
+
+user = User(
+    ID=102,
+    LoginName="MyUser",
+    Password="evenStrongerPassword!",
+    Description="My first User",
+    Roles=[1, 2],
+)
 
-TODO
+# user the Admin standard user to add a new user
+d.post_new_user(user)
+```
 
 #### Interact with a device
 
 The core of washpy is the `DeviceUser` class. Once constructed,
 it provides many methods to control the Miele device.
 
 The script
 ```python
 from washpy import DeviceUser
 
-my_device = DeviceUser("https://192.168.1.251/Devices/000116343328", "Admin", "", "verySecurePassword!")
+my_device = DeviceUser(
+    "https://192.168.1.251/Devices/000116343328", "Admin", "verySecurePassword!"
+)
 
-print(my_device.get_State().Status)
+print(my_device.get_state().Status)
 ```
 will yield
 ```python
 <Status.RUNNING: 5>
 ```
 
+See also the [exapmles](examples) folder for more usage examples.
+
 ## Is there documentation of the IP Profile API?
 
 Yes, you have to request access to it from [Miele Professional](https://www.miele.com/en/com/index-pro.htm).
 
 ## known issues
 
 Do not upgrade requests, as it will upgrade to urllib3 version `2.x`.
```

