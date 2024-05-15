# Comparing `tmp/passbolt-python-api-0.3.4.tar.gz` & `tmp/passbolt_python_api-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passbolt-python-api-0.3.4.tar", last modified: Thu Mar 16 16:35:09 2023, max compression
+gzip compressed data, was "passbolt_python_api-0.3.5.tar", last modified: Wed May 15 18:58:18 2024, max compression
```

## Comparing `passbolt-python-api-0.3.4.tar` & `passbolt_python_api-0.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-03-16 16:35:09.747553 passbolt-python-api-0.3.4/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1073 2023-03-16 09:53:38.000000 passbolt-python-api-0.3.4/LICENSE
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     3608 2023-03-16 16:35:09.747408 passbolt-python-api-0.3.4/PKG-INFO
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     3150 2023-03-16 09:53:38.000000 passbolt-python-api-0.3.4/README.md
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-03-16 16:35:09.745988 passbolt-python-api-0.3.4/passbolt_python_api.egg-info/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     3608 2023-03-16 16:35:09.000000 passbolt-python-api-0.3.4/passbolt_python_api.egg-info/PKG-INFO
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      286 2023-03-16 16:35:09.000000 passbolt-python-api-0.3.4/passbolt_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)        1 2023-03-16 16:35:09.000000 passbolt-python-api-0.3.4/passbolt_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)      148 2023-03-16 16:35:09.000000 passbolt-python-api-0.3.4/passbolt_python_api.egg-info/requires.txt
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       12 2023-03-16 16:35:09.000000 passbolt-python-api-0.3.4/passbolt_python_api.egg-info/top_level.txt
-drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2023-03-16 16:35:09.746925 passbolt-python-api-0.3.4/passboltapi/
--rw-r--r--   0 shubhamdipt   (501) staff       (20)    20084 2023-03-16 09:53:38.000000 passbolt-python-api-0.3.4/passboltapi/__init__.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     6373 2023-03-16 16:32:59.000000 passbolt-python-api-0.3.4/passboltapi/schema.py
--rw-r--r--   0 shubhamdipt   (501) staff       (20)       38 2023-03-16 16:35:09.747630 passbolt-python-api-0.3.4/setup.cfg
--rw-r--r--   0 shubhamdipt   (501) staff       (20)     1570 2023-03-16 16:34:42.000000 passbolt-python-api-0.3.4/setup.py
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2024-05-15 18:58:18.462462 passbolt_python_api-0.3.5/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1073 2024-05-15 18:53:09.000000 passbolt_python_api-0.3.5/LICENSE
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     4097 2024-05-15 18:58:18.462269 passbolt_python_api-0.3.5/PKG-INFO
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     3371 2024-05-15 18:53:09.000000 passbolt_python_api-0.3.5/README.md
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2024-05-15 18:58:18.462064 passbolt_python_api-0.3.5/passbolt_python_api.egg-info/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     4097 2024-05-15 18:58:18.000000 passbolt_python_api-0.3.5/passbolt_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      286 2024-05-15 18:58:18.000000 passbolt_python_api-0.3.5/passbolt_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)        1 2024-05-15 18:58:18.000000 passbolt_python_api-0.3.5/passbolt_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)      148 2024-05-15 18:58:18.000000 passbolt_python_api-0.3.5/passbolt_python_api.egg-info/requires.txt
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       12 2024-05-15 18:58:18.000000 passbolt_python_api-0.3.5/passbolt_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 shubhamdipt   (501) staff       (20)        0 2024-05-15 18:58:18.461828 passbolt_python_api-0.3.5/passboltapi/
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)    20196 2024-05-15 18:53:09.000000 passbolt_python_api-0.3.5/passboltapi/__init__.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     6373 2024-05-15 18:53:09.000000 passbolt_python_api-0.3.5/passboltapi/schema.py
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)       38 2024-05-15 18:58:18.462504 passbolt_python_api-0.3.5/setup.cfg
+-rw-r--r--   0 shubhamdipt   (501) staff       (20)     1570 2024-05-15 18:54:38.000000 passbolt_python_api-0.3.5/setup.py
```

### Comparing `passbolt-python-api-0.3.4/LICENSE` & `passbolt_python_api-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `passbolt-python-api-0.3.4/PKG-INFO` & `passbolt_python_api-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-Metadata-Version: 2.1
-Name: passbolt-python-api
-Version: 0.3.4
-Summary: A python client for Passbolt.
-Home-page: https://github.com/shubhamdipt/passbolt-python-api
-Author: Shubham Dipt
-Author-email: shubham.dipt@gmail.com
-License: MIT
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Passbolt-python-API
 
+It is a python api client for Passbolt.
+
+#### Disclaimer
+* This project is a community driven project that is not associated with Passbolt S.A.
+* Passbolt and the Passbolt logo are registered trademarks of Passbolt S.A.
+
 ## Installation
 
     $pip install passbolt-python-api 
 
 ## Dependencies
 
   - Python >= 3.6
```

### Comparing `passbolt-python-api-0.3.4/README.md` & `passbolt_python_api-0.3.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,38 @@
+Metadata-Version: 2.1
+Name: passbolt-python-api
+Version: 0.3.5
+Summary: A python client for Passbolt.
+Home-page: https://github.com/shubhamdipt/passbolt-python-api
+Author: Shubham Dipt
+Author-email: shubham.dipt@gmail.com
+License: MIT
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: certifi>=2019.6.16
+Requires-Dist: chardet>=3.0.4
+Requires-Dist: charset-normalizer>=2.0.8
+Requires-Dist: idna>=2.8
+Requires-Dist: python-gnupg>=0.4.7
+Requires-Dist: requests==2.26.0
+Requires-Dist: typing-extensions==4.0.0
+Requires-Dist: urllib3>=1.25.3
+
 # Passbolt-python-API
 
+It is a python api client for Passbolt.
+
+#### Disclaimer
+* This project is a community driven project that is not associated with Passbolt S.A.
+* Passbolt and the Passbolt logo are registered trademarks of Passbolt S.A.
+
 ## Installation
 
     $pip install passbolt-python-api 
 
 ## Dependencies
 
   - Python >= 3.6
```

### Comparing `passbolt-python-api-0.3.4/passbolt_python_api.egg-info/PKG-INFO` & `passbolt_python_api-0.3.5/passbolt_python_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 Metadata-Version: 2.1
 Name: passbolt-python-api
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python client for Passbolt.
 Home-page: https://github.com/shubhamdipt/passbolt-python-api
 Author: Shubham Dipt
 Author-email: shubham.dipt@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi>=2019.6.16
+Requires-Dist: chardet>=3.0.4
+Requires-Dist: charset-normalizer>=2.0.8
+Requires-Dist: idna>=2.8
+Requires-Dist: python-gnupg>=0.4.7
+Requires-Dist: requests==2.26.0
+Requires-Dist: typing-extensions==4.0.0
+Requires-Dist: urllib3>=1.25.3
 
 # Passbolt-python-API
 
+It is a python api client for Passbolt.
+
+#### Disclaimer
+* This project is a community driven project that is not associated with Passbolt S.A.
+* Passbolt and the Passbolt logo are registered trademarks of Passbolt S.A.
+
 ## Installation
 
     $pip install passbolt-python-api 
 
 ## Dependencies
 
   - Python >= 3.6
```

### Comparing `passbolt-python-api-0.3.4/passboltapi/__init__.py` & `passbolt_python_api-0.3.5/passboltapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,33 +47,35 @@
 class APIClient:
     def __init__(
         self,
         config: Optional[str] = None,
         config_path: Optional[str] = None,
         new_keys: bool = False,
         delete_old_keys: bool = False,
+        ssl_verify: bool = False,
     ):
         """
         :param config: Config as a dictionary
         :param config_path: Path to the config file.
         :param delete_old_keys: Set true if old keys need to be deleted
         """
+        self.ssl_verify = ssl_verify
         self.config = config
         if config_path:
             self.config = configparser.ConfigParser()
             self.config.read_file(open(config_path, "r"))
         self.requests_session = requests.Session()
 
         if not self.config:
             raise ValueError("Missing config. Provide config as dictionary or path to configuration file.")
         if not self.config["PASSBOLT"]["SERVER"]:
             raise ValueError("Missing value for SERVER in config.ini")
 
         self.server_url = self.config["PASSBOLT"]["SERVER"].rstrip("/")
-        self.user_fingerprint = self.config["PASSBOLT"]["USER_FINGERPRINT"].upper()
+        self.user_fingerprint = self.config["PASSBOLT"]["USER_FINGERPRINT"].upper().replace(" ", "")
         self.gpg = gnupg.GPG()
         if delete_old_keys:
             self._delete_old_keys()
         if new_keys:
             self._import_gpg_keys()
         try:
             self.gpg_fingerprint = [i for i in self.gpg.list_keys() if i["fingerprint"] == self.user_fingerprint][0][
@@ -105,15 +107,15 @@
             raise ValueError("Missing value for USER_PUBLIC_KEY_FILE in config.ini")
         if not self.config["PASSBOLT"]["USER_PRIVATE_KEY_FILE"]:
             raise ValueError("Missing value for USER_PRIVATE_KEY_FILE in config.ini")
         self.gpg.import_keys(open(self.config["PASSBOLT"]["USER_PUBLIC_KEY_FILE"], "r").read())
         self.gpg.import_keys(open(self.config["PASSBOLT"]["USER_PRIVATE_KEY_FILE"], "r").read())
 
     def _login(self):
-        r = self.requests_session.post(self.server_url + LOGIN_URL, json={"gpg_auth": {"keyid": self.gpg_fingerprint}})
+        r = self.requests_session.post(self.server_url + LOGIN_URL, json={"gpg_auth": {"keyid": self.gpg_fingerprint}}, verify=self.ssl_verify)
         encrypted_token = r.headers["X-GPGAuth-User-Auth-Token"]
         encrypted_token = urllib.parse.unquote(encrypted_token)
         encrypted_token = encrypted_token.replace("\+", " ")
         token = self.decrypt(encrypted_token)
         self.requests_session.post(
             self.server_url + LOGIN_URL,
             json={
```

### Comparing `passbolt-python-api-0.3.4/passboltapi/schema.py` & `passbolt_python_api-0.3.5/passboltapi/schema.py`

 * *Files identical despite different names*

### Comparing `passbolt-python-api-0.3.4/setup.py` & `passbolt_python_api-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 links = []  # for repo urls (dependency_links)
 
 with open("requirements.txt") as fp:
     install_requires = fp.read()
 
 DESCRIPTION = "A python client for Passbolt."
-VERSION = "0.3.4"
+VERSION = "0.3.5"
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name="passbolt-python-api",
     version=VERSION,
```

