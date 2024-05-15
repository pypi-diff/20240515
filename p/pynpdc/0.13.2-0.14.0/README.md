# Comparing `tmp/pynpdc-0.13.2.tar.gz` & `tmp/pynpdc-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynpdc-0.13.2.tar", last modified: Thu May  2 12:05:05 2024, max compression
+gzip compressed data, was "pynpdc-0.14.0.tar", last modified: Tue May 14 12:44:16 2024, max compression
```

## Comparing `pynpdc-0.13.2.tar` & `pynpdc-0.14.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-05-02 12:05:05.985391 pynpdc-0.13.2/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     6577 2024-04-11 12:20:53.000000 pynpdc-0.13.2/README.md
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/pynpdc/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1019 2024-05-02 12:01:47.000000 pynpdc-0.13.2/pynpdc/__init__.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    10243 2024-04-30 10:50:07.000000 pynpdc-0.13.2/pynpdc/auth.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    39396 2024-05-02 12:03:42.000000 pynpdc-0.13.2/pynpdc/dataset.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      443 2024-04-11 09:18:52.000000 pynpdc-0.13.2/pynpdc/exception.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-26 08:07:44.000000 pynpdc-0.13.2/pynpdc/py.typed
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1504 2024-04-11 09:18:52.000000 pynpdc-0.13.2/pynpdc/types.py
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/pynpdc.egg-info/
--rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      318 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/SOURCES.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/dependency_links.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       54 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/requires.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        7 2024-05-02 12:05:05.000000 pynpdc-0.13.2/pynpdc.egg-info/top_level.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      932 2024-05-02 12:01:10.000000 pynpdc-0.13.2/pyproject.toml
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-05-02 12:05:05.985391 pynpdc-0.13.2/setup.cfg
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-02 12:05:05.985391 pynpdc-0.13.2/tests/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     7253 2024-04-11 09:18:52.000000 pynpdc-0.13.2/tests/test_auth.py
--rw-rw-r--   0 olaf      (1000) olaf      (1000)    27966 2024-04-26 11:20:41.000000 pynpdc-0.13.2/tests/test_dataset.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-14 12:44:16.523606 pynpdc-0.14.0/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-05-14 12:44:16.523606 pynpdc-0.14.0/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     6577 2024-04-11 12:20:53.000000 pynpdc-0.14.0/README.md
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-14 12:44:16.523606 pynpdc-0.14.0/pynpdc/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      953 2024-05-14 12:17:54.000000 pynpdc-0.14.0/pynpdc/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     9730 2024-05-14 12:41:38.000000 pynpdc-0.14.0/pynpdc/auth.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    39396 2024-05-02 12:03:42.000000 pynpdc-0.14.0/pynpdc/dataset.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      443 2024-04-11 09:18:52.000000 pynpdc-0.14.0/pynpdc/exception.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        0 2024-04-26 08:07:44.000000 pynpdc-0.14.0/pynpdc/py.typed
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1426 2024-05-14 12:18:42.000000 pynpdc-0.14.0/pynpdc/types.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-14 12:44:16.523606 pynpdc-0.14.0/pynpdc.egg-info/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     7415 2024-05-14 12:44:16.000000 pynpdc-0.14.0/pynpdc.egg-info/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      318 2024-05-14 12:44:16.000000 pynpdc-0.14.0/pynpdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-05-14 12:44:16.000000 pynpdc-0.14.0/pynpdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       54 2024-05-14 12:44:16.000000 pynpdc-0.14.0/pynpdc.egg-info/requires.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        7 2024-05-14 12:44:16.000000 pynpdc-0.14.0/pynpdc.egg-info/top_level.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      932 2024-05-14 12:22:03.000000 pynpdc-0.14.0/pyproject.toml
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-05-14 12:44:16.523606 pynpdc-0.14.0/setup.cfg
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-05-14 12:44:16.523606 pynpdc-0.14.0/tests/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     6693 2024-05-14 12:41:46.000000 pynpdc-0.14.0/tests/test_auth.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    27966 2024-04-26 11:20:41.000000 pynpdc-0.14.0/tests/test_dataset.py
```

### Comparing `pynpdc-0.13.2/PKG-INFO` & `pynpdc-0.14.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynpdc
-Version: 0.13.2
+Version: 0.14.0
 Summary: Python lib to interact with the NPDC stack
 Author-email: Olaf Schneider <olaf.schneider@npolar.no>, Mikhail Itkin <mikhail.itkin@npolar.no>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynpdc-0.13.2/README.md` & `pynpdc-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.2/pynpdc/__init__.py` & `pynpdc-0.14.0/pynpdc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # flake8: noqa
 
 from pynpdc.auth import (
     AUTH_LIFE_ENTRYPOINT as AUTH_LIFE_ENTRYPOINT,
     AUTH_STAGING_ENTRYPOINT as AUTH_STAGING_ENTRYPOINT,
     Account as Account,
-    AccountWithCleartextPassword as AccountWithCleartextPassword,
     AccountWithToken as AccountWithToken,
     AuthClient as AuthClient,
 )
 
 from pynpdc.dataset import (
     DATASET_LIFE_ENTRYPOINT as DATASET_LIFE_ENTRYPOINT,
     DATASET_STAGING_ENTRYPOINT as DATASET_STAGING_ENTRYPOINT,
```

### Comparing `pynpdc-0.13.2/pynpdc/auth.py` & `pynpdc-0.14.0/pynpdc/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import requests
 from typing import Optional
 
 from .exception import APIException
 from .types import (
     AccessLevel,
     AccountAPIResponse,
-    AccountWithPasswordAPIResponse,
     AccountWithTokenAPIResponse,
     KeepaliveAPIResponse,
 )
 
 AUTH_STAGING_ENTRYPOINT = "https://beta.data.npolar.no/-/auth/"
 AUTH_LIFE_ENTRYPOINT = "https://auth.data.npolar.no/"
 
@@ -77,15 +76,15 @@
     def directory_user(self) -> bool:
         """
         Retrieve a flag that indicates whether the account is managed by AD
 
         Returns:
             bool: the AD flag
         """
-        return self.raw["directoryUser"]
+        return self.raw.get("directoryUser", False)
 
 
 class AccountWithToken(Account):
     """
     A logged in account with token.
 
     Attributes:
@@ -113,36 +112,14 @@
         Args:
             token (str): The new token
 
         """
         self.raw["token"] = token
 
 
-class AccountWithCleartextPassword(Account):
-    """
-    An freshly created Account with cleartext password.
-
-    Attributes:
-        raw (AccountWithPasswordAPIResponse): The API response data parsed from JSON
-        client (AuthClient | None) The client for the auth module
-    """
-
-    raw: AccountWithPasswordAPIResponse
-
-    @property
-    def password(self) -> str:
-        """
-        Retrieve the cleartext password after account creation by an admin.
-
-        Returns:
-            str: the cleartext password
-        """
-        return self.raw["password"]
-
-
 class AuthClient:
     entrypoint: str
     verify_ssl: bool
 
     """
     A client to communicate with the NPDC auth module.
 
@@ -227,45 +204,47 @@
 
         if response.status_code != 200:
             raise APIException(response)
 
         return Account(response.json())
 
     def create_account(
-        self, originator_account: AccountWithToken, email: str
-    ) -> AccountWithCleartextPassword:
+        self, originator_account: AccountWithToken, email: str, link_prefix: str
+    ) -> Account:
         """
         Create a new external account
 
         Only admins have access to this method
 
         Args:
             originator_account (AccountWithToken ): the account used to create the new
                 account. Has to have accessLevel admin.
             email (str): the email for the account. The email domain must not be
                 an internal one (npolar.no in the production system)
+            link_prefix (str): the link prefix. Used to build a URL in the
+                email.
 
         Returns:
-            AccountWithCleartextPassword
+            Account
 
         Raises:
             APIException: if the HTTP status code of the response is not 201
         """
 
         endpoint = f"{self.entrypoint}account/"
         headers = {"Authorization": f"Bearer {originator_account.token}"}
-        payload = {"email": email}
+        payload = {"email": email, "linkPrefix": link_prefix}
         response = requests.post(
             endpoint, headers=headers, json=payload, verify=self.verify_ssl
         )
 
         if response.status_code != 201:
             raise APIException(response)
 
-        return AccountWithCleartextPassword(response.json())
+        return Account(response.json())
 
     def get_account(self, account_id: str) -> Account | None:
         """
         Retrieve an account by ID
 
                 When the account is not found, None is returned.
```

### Comparing `pynpdc-0.13.2/pynpdc/dataset.py` & `pynpdc-0.14.0/pynpdc/dataset.py`

 * *Files identical despite different names*

### Comparing `pynpdc-0.13.2/pynpdc/types.py` & `pynpdc-0.14.0/pynpdc/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,18 +20,14 @@
 class AccountAPIResponse(TypedDict):
     id: str
     email: str
     accessLevel: AccessLevel
     directoryUser: bool
 
 
-class AccountWithPasswordAPIResponse(AccountAPIResponse):
-    password: str
-
-
 class AccountWithTokenAPIResponse(AccountAPIResponse):
     token: str
 
 
 class KeepaliveAPIResponse(TypedDict):
     token: str
```

### Comparing `pynpdc-0.13.2/pynpdc.egg-info/PKG-INFO` & `pynpdc-0.14.0/pynpdc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynpdc
-Version: 0.13.2
+Version: 0.14.0
 Summary: Python lib to interact with the NPDC stack
 Author-email: Olaf Schneider <olaf.schneider@npolar.no>, Mikhail Itkin <mikhail.itkin@npolar.no>
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynpdc-0.13.2/pyproject.toml` & `pynpdc-0.14.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pynpdc"
-version = "0.13.2"
+version = "0.14.0"
 dependencies = [
     "requests",
     "requests-toolbelt",
     "typing-extensions",
     "werkzeug",
 ]
 requires-python = ">= 3.8"
```

### Comparing `pynpdc-0.13.2/tests/test_auth.py` & `pynpdc-0.14.0/tests/test_auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
         account.token = "124"
         self.assertEqual(account.token, "124")
 
 
 @pytest.mark.usefixtures("run_fixtures")
 class TestAuth(unittest.TestCase):
+
+    LINK_PREFIX = "https://example.org/"
+
     def setUp(self):
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     def test_login_succeeds(self):
         account = self.client.login(self.user, self.password)
         self.assertEqual(account.email, self.user)
         self.assertIsInstance(account.token, str)
@@ -147,54 +150,39 @@
         This function tests both create_account and update_account.
 
         Normally we keep the tests separated, but since it is not possible to
         delete accounts through the API we want to create accounts as little as
         possible in the unit tests.
         """
 
-        # create_account
-        # --------------
-
         originator_account = self.client.login(self.admin_user, self.admin_password)
         new_account_email = f"test-{uuid.uuid4()}@example.org"
 
-        account = self.client.create_account(originator_account, new_account_email)
+        account = self.client.create_account(
+            originator_account, new_account_email, self.LINK_PREFIX
+        )
 
         self.assertEqual(account.email, new_account_email)
         self.assertEqual(account.access_level, AccessLevel.EXTERNAL)
         self.assertFalse(account.directory_user)
-        self.assertGreater(len(account.password), 0)
-
-        # check if it is possible to login with the new account
-
-        logged_in_account = self.client.login(new_account_email, account.password)
-
-        self.assertEqual(logged_in_account.email, new_account_email)
-        self.assertEqual(logged_in_account.access_level, AccessLevel.EXTERNAL)
-        self.assertFalse(logged_in_account.directory_user)
 
-        # update_account
-        # --------------
+        # load the account
 
-        self.client.update_account(originator_account, account.id, active=False)
+        loaded_account = self.client.get_account(account.id)
 
-        # now login should not be possible anymore
-
-        with pytest.raises(APIException) as e_info:
-            self.client.login(new_account_email, account.password)
-
-        e = e_info.value
-        self.assertEqual(e.status_code, 401)
+        self.assertIsInstance(loaded_account, Account)
 
     def test_creating_an_account_without_admin_level_fails(self):
         originator_account = self.client.login(self.user, self.password)
         new_account_email = f"test-{uuid.uuid4()}@example.org"
 
         with pytest.raises(APIException) as e_info:
-            self.client.create_account(originator_account, new_account_email)
+            self.client.create_account(
+                originator_account, new_account_email, self.LINK_PREFIX
+            )
 
         e = e_info.value
         self.assertEqual(e.status_code, 403)
 
     def test_updating_an_account_without_admin_level_fails(self):
         account = self.client.login(self.user, self.password)
         account_id = account.id
```

### Comparing `pynpdc-0.13.2/tests/test_dataset.py` & `pynpdc-0.14.0/tests/test_dataset.py`

 * *Files identical despite different names*

