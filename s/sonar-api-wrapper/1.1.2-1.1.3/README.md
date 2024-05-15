# Comparing `tmp/sonar_api_wrapper-1.1.2-py3-none-any.whl.zip` & `tmp/sonar_api_wrapper-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6106 bytes, number of entries: 7
+Zip file size: 6095 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      189 b- defN 20-Feb-02 00:00 sonar_api_wrapper/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 sonar_api_wrapper/__version__.py
--rw-r--r--  2.0 unx     5302 b- defN 20-Feb-02 00:00 sonar_api_wrapper/client.py
-?rw-r--r--  2.0 unx     4720 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      599 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.2.dist-info/RECORD
-7 files, 11997 bytes uncompressed, 5034 bytes compressed:  58.0%
+-rw-r--r--  2.0 unx     5286 b- defN 20-Feb-02 00:00 sonar_api_wrapper/client.py
+?rw-r--r--  2.0 unx     4704 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      599 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.3.dist-info/RECORD
+7 files, 11965 bytes uncompressed, 5023 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: sonar_api_wrapper/__version__.py
 Comment: 
 
 Filename: sonar_api_wrapper/client.py
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.2.dist-info/METADATA
+Filename: sonar_api_wrapper-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.2.dist-info/WHEEL
+Filename: sonar_api_wrapper-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.2.dist-info/licenses/LICENSE
+Filename: sonar_api_wrapper-1.1.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.2.dist-info/RECORD
+Filename: sonar_api_wrapper-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sonar_api_wrapper/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.2"
+__version__ = "1.1.3"
```

## sonar_api_wrapper/client.py

```diff
@@ -73,28 +73,28 @@
     :param username: Username used for authentication.
         Default is set via the environment variable `SONAR_USERNAME` or "admin".
     :param password: Password used for authentication.
         Default is set via the environment variable `SONAR_PASSWORD` or "admin".
     :param token: Token used for authentication. It overrides username and password if present.
         Default value is set via the environment variable `SONAR_TOKEN` or None.
     :param base_path: The base endpoint used to build the API call.
-        Default is set via the environment variable `DEFAULT_SONAR_ENDPOINT` or "http://localhost:9000/api/".
+        Default is set via the environment variable `SONAR_ENDPOINT` or "http://localhost:9000/api/".
     :return: Returns the API response as `list[dict]`, `dict`,
         or any other type based on the response content or raises an exception.
         ### Example
 
         ```python
         import os
 
         from sonar_api_wrapper import api_call
 
         # override default access config
         os.environ['SONAR_PASSWORD'] = 'Username'
         os.environ['SONAR_PASSWORD'] = 'YourPassword'
-        os.environ['DEFAULT_SONAR_ENDPOINT'] = 'https://yours.sonarqube/api/'
+        os.environ['SONAR_ENDPOINT'] = 'https://yours.sonarqube/api/'
 
         response = api_call('GET', 'qualityprofiles/search', parameters={
             'defaults': 'true'
         })
 
         print(f'{response["projects"] = }')
         ```
```

## Comparing `sonar_api_wrapper-1.1.2.dist-info/METADATA` & `sonar_api_wrapper-1.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sonar-api-wrapper
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sonar API Wrapper - a Sonarqube api wrapper
 Project-URL: Homepage, https://github.com/AlessandroStaffolani/sonar-api-wrapper
 Project-URL: Repository, https://github.com/AlessandroStaffolani/sonar-api-wrapper.git
 Author-email: Alessandro Staffolani <alestam93@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Alessandro Staffolani
@@ -68,15 +68,15 @@
 - `body` (`dict` | `None`): Body of the request. Default is `None`.
 - `files` (`Any`): Files to be sent in the request. Default is `None`.
 - `headers` (`dict` | `None`): Headers of the request. Default is `None`.
 - `is_json` (`bool`): If set to `True`, the response will be parsed as JSON. Otherwise, it returns the decoded content. Default is `True`.
 - `username` (`str` | `None`): Username used for authentication. Default is set via the environment variable `SONAR_USERNAME` or "admin".
 - `password` (`str` | `None`): Password used for authentication. Default is set via the environment variable `SONAR_PASSWORD` or "admin".
 - `token` (`str` | `None`): Token used for authentication. It overrides username and password if present. Default value is set via the environment variable `SONAR_TOKEN` or None.
-- `base_path` (`str` | `None`): The base endpoint used to build the API call. Default is set via the environment variable `DEFAULT_SONAR_ENDPOINT` or "http://localhost:9000/api/".
+- `base_path` (`str` | `None`): The base endpoint used to build the API call. Default is set via the environment variable `SONAR_ENDPOINT` or "http://localhost:9000/api/".
 
 ### Returns
 
 Returns the API response as `list[dict]`, `dict`, or any other type based on the response content or raises an exception.
 
 ### Example
 
@@ -84,15 +84,15 @@
 import os
 
 from sonar_api_wrapper import api_call
 
 # override default access config
 os.environ['SONAR_PASSWORD'] = 'Username'
 os.environ['SONAR_PASSWORD'] = 'YourPassword'
-os.environ['DEFAULT_SONAR_ENDPOINT'] = 'https://yours.sonarqube/api/'
+os.environ['SONAR_ENDPOINT'] = 'https://yours.sonarqube/api/'
 
 response = api_call('GET', 'qualityprofiles/search', parameters={
     'defaults': 'true'
 })
 
 print(f'{response["projects"] = }')
 ```
```

## Comparing `sonar_api_wrapper-1.1.2.dist-info/licenses/LICENSE` & `sonar_api_wrapper-1.1.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `sonar_api_wrapper-1.1.2.dist-info/RECORD` & `sonar_api_wrapper-1.1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sonar_api_wrapper/__init__.py,sha256=OoxhDQ4PM1RubQFx9vVNvoLVX_6rSlCErFHqZw3FnZI,189
-sonar_api_wrapper/__version__.py,sha256=5SgGjThsHu_ITn8V83BvCziqCwxdXxTQqcC3KQMHPfM,22
-sonar_api_wrapper/client.py,sha256=fSmv94jGWY0ztsvKcpl5EaY_FR3OUDo5rKmynvJ5l-g,5302
-sonar_api_wrapper-1.1.2.dist-info/METADATA,sha256=_DFTdb50S6PzKcHA-nBx7aZm4VkqTa_x63znt8aSzUc,4720
-sonar_api_wrapper-1.1.2.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-sonar_api_wrapper-1.1.2.dist-info/licenses/LICENSE,sha256=3-LJXFE1en-RhdAZ-BUZ1L3ztHSXxK-UwEOKXMcZKz0,1078
-sonar_api_wrapper-1.1.2.dist-info/RECORD,,
+sonar_api_wrapper/__version__.py,sha256=u9ExJqoMv3fQc8WmLTw4I2FnQo6u4xRrBc6DLy6G1IE,22
+sonar_api_wrapper/client.py,sha256=HFepzsI6x7WlVwqpEuV6LJKke95hRITvoSVDmYgq7zo,5286
+sonar_api_wrapper-1.1.3.dist-info/METADATA,sha256=xLdm9o3haDiNGrcOAuHcjzGMHOKnDsvU00_LFbQ4m7g,4704
+sonar_api_wrapper-1.1.3.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+sonar_api_wrapper-1.1.3.dist-info/licenses/LICENSE,sha256=3-LJXFE1en-RhdAZ-BUZ1L3ztHSXxK-UwEOKXMcZKz0,1078
+sonar_api_wrapper-1.1.3.dist-info/RECORD,,
```

