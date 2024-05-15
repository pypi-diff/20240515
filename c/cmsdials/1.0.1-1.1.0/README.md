# Comparing `tmp/cmsdials-1.0.1.tar.gz` & `tmp/cmsdials-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmsdials-1.0.1.tar", max compression
+gzip compressed data, was "cmsdials-1.1.0.tar", max compression
```

## Comparing `cmsdials-1.0.1.tar` & `cmsdials-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0    35149 2024-04-28 10:36:23.872227 cmsdials-1.0.1/LICENSE
--rw-r--r--   0        0        0     5484 2024-04-29 19:09:44.714827 cmsdials-1.0.1/README.md
--rw-r--r--   0        0        0       49 2024-04-28 10:36:23.872227 cmsdials-1.0.1/cmsdials/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.872227 cmsdials-1.0.1/cmsdials/auth/__init__.py
--rw-r--r--   0        0        0     4136 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/_base.py
--rw-r--r--   0        0        0     4998 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/bearer.py
--rw-r--r--   0        0        0     3491 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/client.py
--rw-r--r--   0        0        0      107 2024-04-28 10:36:23.873227 cmsdials-1.0.1/cmsdials/auth/exceptions.py
--rw-r--r--   0        0        0      425 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/auth/models.py
--rw-r--r--   0        0        0     1041 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/auth/secret_key.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/clients/file_index/__init__.py
--rw-r--r--   0        0        0      318 2024-04-28 10:36:23.874227 cmsdials-1.0.1/cmsdials/clients/file_index/client.py
--rw-r--r--   0        0        0      962 2024-04-29 19:06:30.058424 cmsdials-1.0.1/cmsdials/clients/file_index/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.1/cmsdials/clients/h1d/__init__.py
--rw-r--r--   0        0        0      402 2024-04-29 11:53:55.385012 cmsdials-1.0.1/cmsdials/clients/h1d/client.py
--rw-r--r--   0        0        0     1313 2024-04-30 23:50:22.265289 cmsdials-1.0.1/cmsdials/clients/h1d/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.875227 cmsdials-1.0.1/cmsdials/clients/h2d/__init__.py
--rw-r--r--   0        0        0      402 2024-04-29 11:53:59.860011 cmsdials-1.0.1/cmsdials/clients/h2d/client.py
--rw-r--r--   0        0        0     1364 2024-04-30 23:50:22.265289 cmsdials-1.0.1/cmsdials/clients/h2d/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.1/cmsdials/clients/lumisection/__init__.py
--rw-r--r--   0        0        0      946 2024-04-29 13:18:14.360705 cmsdials-1.0.1/cmsdials/clients/lumisection/client.py
--rw-r--r--   0        0        0      856 2024-04-30 23:50:22.265289 cmsdials-1.0.1/cmsdials/clients/lumisection/models.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.877227 cmsdials-1.0.1/cmsdials/clients/run/__init__.py
--rw-r--r--   0        0        0      854 2024-04-29 13:18:14.362705 cmsdials-1.0.1/cmsdials/clients/run/client.py
--rw-r--r--   0        0        0      667 2024-04-29 19:07:09.219346 cmsdials-1.0.1/cmsdials/clients/run/models.py
--rw-r--r--   0        0        0      847 2024-04-29 19:13:59.398882 cmsdials-1.0.1/cmsdials/cmsdials.py
--rw-r--r--   0        0        0      439 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/filters.py
--rw-r--r--   0        0        0        0 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/__init__.py
--rw-r--r--   0        0        0      671 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/_json.py
--rw-r--r--   0        0        0     3557 2024-04-29 19:13:59.688881 cmsdials-1.0.1/cmsdials/utils/api_client.py
--rw-r--r--   0        0        0      174 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/base_model.py
--rw-r--r--   0        0        0      145 2024-04-28 10:36:23.878227 cmsdials-1.0.1/cmsdials/utils/logger.py
--rw-r--r--   0        0        0     2720 2024-04-30 23:50:22.265289 cmsdials-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6431 1970-01-01 00:00:00.000000 cmsdials-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 21:48:00.845728 cmsdials-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7312 2024-05-15 15:43:58.486431 cmsdials-1.1.0/README.md
+-rw-r--r--   0        0        0       50 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.846728 cmsdials-1.1.0/cmsdials/auth/__init__.py
+-rw-r--r--   0        0        0     4155 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/auth/_base.py
+-rw-r--r--   0        0        0     5021 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/auth/bearer.py
+-rw-r--r--   0        0        0     3654 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/auth/client.py
+-rw-r--r--   0        0        0      112 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/auth/exceptions.py
+-rw-r--r--   0        0        0      425 2024-04-30 21:48:00.846728 cmsdials-1.1.0/cmsdials/auth/models.py
+-rw-r--r--   0        0        0     1050 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/auth/secret_key.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.846728 cmsdials-1.1.0/cmsdials/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.846728 cmsdials-1.1.0/cmsdials/clients/file_index/__init__.py
+-rw-r--r--   0        0        0      318 2024-04-30 21:48:00.846728 cmsdials-1.1.0/cmsdials/clients/file_index/client.py
+-rw-r--r--   0        0        0      985 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/clients/file_index/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.846728 cmsdials-1.1.0/cmsdials/clients/h1d/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-30 23:31:22.272853 cmsdials-1.1.0/cmsdials/clients/h1d/client.py
+-rw-r--r--   0        0        0     1336 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/clients/h1d/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.846728 cmsdials-1.1.0/cmsdials/clients/h2d/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-30 23:31:22.273853 cmsdials-1.1.0/cmsdials/clients/h2d/client.py
+-rw-r--r--   0        0        0     1393 2024-05-15 15:43:58.486431 cmsdials-1.1.0/cmsdials/clients/h2d/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.847728 cmsdials-1.1.0/cmsdials/clients/lumisection/__init__.py
+-rw-r--r--   0        0        0      976 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/clients/lumisection/client.py
+-rw-r--r--   0        0        0      885 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/clients/lumisection/models.py
+-rw-r--r--   0        0        0        0 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/clients/mes/__init__.py
+-rw-r--r--   0        0        0      251 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/clients/mes/client.py
+-rw-r--r--   0        0        0      359 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/clients/mes/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.847728 cmsdials-1.1.0/cmsdials/clients/run/__init__.py
+-rw-r--r--   0        0        0      884 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/clients/run/client.py
+-rw-r--r--   0        0        0      696 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/clients/run/models.py
+-rw-r--r--   0        0        0      981 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/cmsdials.py
+-rw-r--r--   0        0        0      499 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/filters.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:48:00.847728 cmsdials-1.1.0/cmsdials/utils/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-30 21:48:00.847728 cmsdials-1.1.0/cmsdials/utils/_json.py
+-rw-r--r--   0        0        0     4594 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/utils/api_client.py
+-rw-r--r--   0        0        0      711 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/utils/base_model.py
+-rw-r--r--   0        0        0      146 2024-05-15 15:43:58.487431 cmsdials-1.1.0/cmsdials/utils/logger.py
+-rw-r--r--   0        0        0     2910 2024-05-15 15:44:13.668421 cmsdials-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8404 1970-01-01 00:00:00.000000 cmsdials-1.1.0/PKG-INFO
```

### Comparing `cmsdials-1.0.1/LICENSE` & `cmsdials-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.1/README.md` & `cmsdials-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 To install dials-py, simply
 
 ```bash
 $ pip install cmsdials
 ```
 
+It is also possible to specify the following extras, to enable optional features:
+
+```
+pandas, tqdm
+```
+
 ## Usage
 
 Before interfacing with any route you need to generate valid credentials, it is possible to authenticate trough the `device authorization flow` or using the `client secret key` of any application registered in DIALS. Note that, the device flow is an interactively authentication procedure that is possible to distinguish users in DIALS backend and the client secret flow is not interactive and is not possible to distinguish users so it should only be used for automation scripts.
 
 ### Generating credentials with client secret
 
 ```python
@@ -133,20 +139,44 @@
 dials.lumi.list_all(LumisectionFilters(run_number=360392), max_pages=5)
 
 dials.run.list_all(RunFilters(run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
 
 ### Dials MEs
 
-It is possible to inspect the list of selected MEs considered in DIALS during ETL requesting the endpoint `configured-mes` trough the method:
+It is possible to inspect the list of ingested MEs in DIALS listing the endpoint `mes` trough the method:
+
+```python
+dials.mes.list()
+```
+
+### Automatically convert paginated results to pandas DataFrame
+
+You can enable this optional feature by installing the package with the `pandas` extra.
+
+All `Paginated` metaclasses contain the method `to_pandas` that will automatically transform the `results` attribute of the metaclass into a pandas dataframe, for example:
+
+```python
+data = dials.h1d.list_all(LumisectionHistogram1DFilters(me="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
+data.to_pandas()
+```
+
+### Indefinite progress bar when fetch multi-page result
+
+You can enable this optional feature by installing the package with the `tqdm` extra.
+
+Whenever you call a `list_all` method that fetches multiple pages a dynamic progress will be rendered to indicate duration and number of pages, for example:
 
 ```python
-dials.lumi.configured_mes()
+>>> dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="PXBarrel", ls_number=78, entries__gte=100), max_pages=5)
+Progress: 100%|█████████████████████████████████████| 5/5 [00:02<00:00,  1.70it/s]
 ```
 
+The total attribute of the bar is dynamically updated while fetching the pages.
+
 ## Usage with local DIALS
 
 All classes that interface the DIALS service inherits the class `BaseAPIClient` which propagate the `base_url`, `route` and `version` attributes with production values. In order to use dials-py with a local version of DIALS it is possible to overwrite those attributes when instantiating the `AuthClient` and the `Dials` client, for example:
 
 ```python
 from cmsdials.auth.client import AuthClient
 from cmsdials.auth.bearer import Credentials
@@ -158,7 +188,17 @@
 
 auth = AuthClient(base_url=DEV_URL)
 creds = Credentials.from_creds_file(cache_dir=DEV_CACHE_DIR, client=auth)  # Make sure to specify the auth client with overwritten values, using another cache_dir is recommended
 dials = Dials(creds, base_url=DEV_URL)
 
 dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="EEOT digi occupancy EE +", entries__gte=100, run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
+
+## Running tests
+
+The repository has some tests written to make sure DIALS responses are compatible with pydantic metaclasses, you can use pytest to run all tests but you need to specify a secret key to authenticate non-interactively against DIALS api:
+
+```bash
+SECRET_KEY=... pytest tests
+```
+
+The secret key is an api client enabled secret key and can be obtained from the applications portal, any api client secret key whitelisted in DIALS can be used. The interactive authentication flow should be tested manually, an example for this can be found in [this line](/tests/integration/test_auth_client.py#L33).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmsdials-1.0.1/cmsdials/auth/_base.py` & `cmsdials-1.1.0/cmsdials/auth/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import threading
 from abc import ABC, abstractmethod
+from collections.abc import Mapping
 from datetime import datetime, timedelta
 from enum import Enum
-from typing import Mapping
 
-from .exceptions import ImpossibleToRefreshToken
+from .exceptions import ImpossibleToRefreshTokenError
 
 
 class TokenState(Enum):
     """
     Tracks the state of a token.
 
     FRESH: The token is valid and can be used.
@@ -112,15 +112,15 @@
     def before_request(self, headers: Mapping[str, str]):
         """
         Performs credential-specific before request logic.
         """
         # If token is invalid (both token and refresh token expired): Throw error
         # User need to interactively authenticate again
         if self.token_state == TokenState.INVALID:
-            raise ImpossibleToRefreshToken
+            raise ImpossibleToRefreshTokenError
 
         # If token is stale (token is close to expire)
         # Re-use the token but launch a new thread to refresh the token
         if self.token_state == TokenState.STALE and self._stale_lock.locked() is False:
             worker = threading.Thread(target=self._nonblocking_refresh)
             worker.start()
```

### Comparing `cmsdials-1.0.1/cmsdials/auth/bearer.py` & `cmsdials-1.1.0/cmsdials/auth/bearer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import json
 import os
 import os.path
+from collections.abc import Mapping
 from datetime import datetime
-from typing import Mapping, Optional
+from typing import Optional
 
 from ..utils._json import TokenDecoder, TokenEncoder
 from ..utils.logger import logger
 from ._base import BaseCredentials, TokenState
 from .client import AuthClient
 from .models import Token
 
+
 DEFAULT_CACHE_DIR = ".cache"
 DEFAULT_CACHE_FILENAME = "creds"
 
 
 class Credentials(BaseCredentials):
     """
     Token credentials.
@@ -99,15 +101,15 @@
         )
 
     @staticmethod
     def from_creds_file(cache_dir: str = DEFAULT_CACHE_DIR, client: Optional[AuthClient] = None) -> "Credentials":
         client = client or AuthClient()
         fpath = Credentials._handle_creds_filepath(cache_dir)
         try:
-            with open(fpath, "r") as filebuffer:
+            with open(fpath) as filebuffer:
                 fcontents = json.load(filebuffer, cls=TokenDecoder)
             token = Token(**fcontents)
         except FileNotFoundError:
             logger.info("Credentials file not found, triggering device authentication flow...")
             token: Token = client.device_auth_flow()
 
         return Credentials.from_authclient_token(token, cache_dir, client)
```

### Comparing `cmsdials-1.0.1/cmsdials/auth/client.py` & `cmsdials-1.1.0/cmsdials/auth/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,38 +10,42 @@
 
 
 class AuthClient(BaseAPIClient):
     """
     Client for DIALS auth endpoint
     """
 
+    default_timeout = 30  # seconds
+
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def new_device(self) -> Device:
         endpoint_url = self.api_url + "auth/new-device/"
         response = requests.get(
             url=endpoint_url,
             headers={
                 "accept": "application/json",
             },
+            timeout=self.default_timeout,
         )
         response.raise_for_status()
         response = response.json()
         return Device(**response)
 
     def device_token(self, device_code: str) -> Token:
         endpoint_url = self.api_url + "auth/device-token/"
         response = requests.post(
             url=endpoint_url,
             headers={
                 "accept": "application/json",
                 "Content-Type": "application/json",
             },
             json={"device_code": device_code},
+            timeout=self.default_timeout,
         )
 
         if response.status_code == 400 and "authorization_pending" in response.text:
             raise PendingAuthorizationError
 
         response.raise_for_status()
         response = response.json()
@@ -59,14 +63,15 @@
             url=endpoint_url,
             headers={
                 "accept": "application/json",
                 "Content-Type": "application/json",
                 "Authorization": f"{token_type} {access_token}",
             },
             json={"refresh_token": refresh_token},
+            timeout=self.default_timeout,
         )
         response.raise_for_status()
         response = response.json()
         curr_datetime = datetime.now()
         token = RefreshToken(**response)
         return Token(
             **token.dict(),
```

### Comparing `cmsdials-1.0.1/cmsdials/auth/secret_key.py` & `cmsdials-1.1.0/cmsdials/auth/secret_key.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Mapping
+from collections.abc import Mapping
 
 from ._base import BaseCredentials
 
 
 class Credentials(BaseCredentials):
     """
     Client secret key credentials.
```

### Comparing `cmsdials-1.0.1/cmsdials/clients/file_index/models.py` & `cmsdials-1.1.0/cmsdials/clients/file_index/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from datetime import datetime
-from typing import List, Optional
+from typing import Optional
 
 from pydantic import AnyUrl, BaseModel, Field
 
-from ...utils.base_model import OBaseModel
+from ...utils.base_model import OBaseModel, PaginatedBaseModel
 
 
 class FileIndex(BaseModel):
     dataset_id: int
     dataset: str = Field(..., max_length=255)
     file_id: int
     file_size: int
     creation_date: datetime
     last_modification_date: datetime
     logical_file_name: str
     status: str = Field(..., max_length=15)
     err_trace: Optional[str] = Field(..., max_length=5000)
 
 
-class PaginatedFileIndexList(BaseModel):
+class PaginatedFileIndexList(PaginatedBaseModel):
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
-    results: List[FileIndex]
+    results: list[FileIndex]
 
 
 class FileIndexFilters(OBaseModel):
     next_token: Optional[str] = None
     dataset_id: Optional[int] = None
     logical_file_name: Optional[str] = None
     logical_file_name__regex: Optional[str] = None
```

### Comparing `cmsdials-1.0.1/cmsdials/clients/h1d/models.py` & `cmsdials-1.1.0/cmsdials/clients/h2d/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-from typing import List, Optional
+from typing import Optional
 
 from pydantic import AnyUrl, BaseModel, Field
 
-from ...utils.base_model import OBaseModel
+from ...utils.base_model import OBaseModel, PaginatedBaseModel
 
 
-class LumisectionHistogram1D(BaseModel):
+class LumisectionHistogram2D(BaseModel):
     hist_id: int
     dataset: str = Field(..., max_length=255)
     me: str = Field(..., max_length=255)
     dataset_id: int
     file_id: int
     run_number: int
     ls_number: int
     me_id: int
     x_min: float
     x_max: float
     x_bin: float
+    y_min: float
+    y_max: float
+    y_bin: float
     entries: int
-    data: list[float]
+    data: list[list[float]]
 
 
-class PaginatedLumisectionHistogram1DList(BaseModel):
+class PaginatedLumisectionHistogram2DList(PaginatedBaseModel):
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
-    results: List[LumisectionHistogram1D]
+    results: list[LumisectionHistogram2D]
 
 
-class LumisectionHistogram1DFilters(OBaseModel):
+class LumisectionHistogram2DFilters(OBaseModel):
     next_token: Optional[str] = None
     dataset_id: Optional[int] = None
     file_id: Optional[int] = None
     run_number: Optional[int] = None
     run_number__lte: Optional[int] = None
     run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
```

### Comparing `cmsdials-1.0.1/cmsdials/clients/h2d/models.py` & `cmsdials-1.1.0/cmsdials/clients/lumisection/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 from typing import Optional
 
 from pydantic import AnyUrl, BaseModel, Field
 
-from ...utils.base_model import OBaseModel
+from ...utils.base_model import OBaseModel, PaginatedBaseModel
 
 
-class LumisectionHistogram2D(BaseModel):
-    hist_id: int
-    dataset: str = Field(..., max_length=255)
-    me: str = Field(..., max_length=255)
+class Lumisection(BaseModel):
     dataset_id: int
-    file_id: int
+    dataset: str = Field(..., max_length=255)
     run_number: int
     ls_number: int
-    me_id: int
-    x_min: float
-    x_max: float
-    x_bin: float
-    y_min: float
-    y_max: float
-    y_bin: float
-    entries: int
-    data: list[list[float]]
+    th1_count: int
+    th2_count: int
 
 
-class PaginatedLumisectionHistogram2DList(BaseModel):
+class PaginatedLumisectionList(PaginatedBaseModel):
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
-    results: list[LumisectionHistogram2D]
+    results: list[Lumisection]
 
 
-class LumisectionHistogram2DFilters(OBaseModel):
+class LumisectionFilters(OBaseModel):
     next_token: Optional[str] = None
     dataset_id: Optional[int] = None
-    file_id: Optional[int] = None
     run_number: Optional[int] = None
     run_number__lte: Optional[int] = None
     run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
-    ls_numbet__lte: Optional[int] = None
+    ls_number__lte: Optional[int] = None
     ls_number__gte: Optional[int] = None
-    me_id: Optional[int] = None
-    entries__gte: Optional[int] = None
     dataset: Optional[str] = None
     dataset__regex: Optional[str] = None
-    logical_file_name: Optional[str] = None
-    logical_file_name__regex: Optional[str] = None
-    me: Optional[str] = None
-    me__regex: Optional[str] = None
```

### Comparing `cmsdials-1.0.1/cmsdials/clients/lumisection/client.py` & `cmsdials-1.1.0/cmsdials/clients/lumisection/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     pagination_model = PaginatedLumisectionList
     filter_class = LumisectionFilters
     lookup_url = "lumisection/"
 
     def get(self, dataset_id: int, run_number: int, ls_number: int):
         endpoint_url = f"{self.api_url}{self.lookup_url}{dataset_id}/{run_number}/{ls_number}/"
         headers = self._build_headers()
-        response = requests.get(endpoint_url, headers=headers)
+        response = requests.get(endpoint_url, headers=headers, timeout=self.default_timeout)
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
```

### Comparing `cmsdials-1.0.1/cmsdials/clients/lumisection/models.py` & `cmsdials-1.1.0/cmsdials/clients/h1d/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 from typing import Optional
 
 from pydantic import AnyUrl, BaseModel, Field
 
-from ...utils.base_model import OBaseModel
+from ...utils.base_model import OBaseModel, PaginatedBaseModel
 
 
-class Lumisection(BaseModel):
-    dataset_id: int
+class LumisectionHistogram1D(BaseModel):
+    hist_id: int
     dataset: str = Field(..., max_length=255)
+    me: str = Field(..., max_length=255)
+    dataset_id: int
+    file_id: int
     run_number: int
     ls_number: int
-    th1_count: int
-    th2_count: int
+    me_id: int
+    x_min: float
+    x_max: float
+    x_bin: float
+    entries: int
+    data: list[float]
 
 
-class PaginatedLumisectionList(BaseModel):
+class PaginatedLumisectionHistogram1DList(PaginatedBaseModel):
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
-    results: list[Lumisection]
+    results: list[LumisectionHistogram1D]
 
 
-class LumisectionFilters(OBaseModel):
+class LumisectionHistogram1DFilters(OBaseModel):
     next_token: Optional[str] = None
     dataset_id: Optional[int] = None
+    file_id: Optional[int] = None
     run_number: Optional[int] = None
     run_number__lte: Optional[int] = None
     run_number__gte: Optional[int] = None
     ls_number: Optional[int] = None
-    ls_number__lte: Optional[int] = None
+    ls_numbet__lte: Optional[int] = None
     ls_number__gte: Optional[int] = None
+    me_id: Optional[int] = None
+    entries__gte: Optional[int] = None
     dataset: Optional[str] = None
     dataset__regex: Optional[str] = None
+    logical_file_name: Optional[str] = None
+    logical_file_name__regex: Optional[str] = None
+    me: Optional[str] = None
+    me__regex: Optional[str] = None
```

### Comparing `cmsdials-1.0.1/cmsdials/clients/run/client.py` & `cmsdials-1.1.0/cmsdials/clients/run/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     pagination_model = PaginatedRunList
     filter_class = RunFilters
     lookup_url = "run/"
 
     def get(self, dataset_id: int, run_number: int):
         endpoint_url = f"{self.api_url}{self.lookup_url}{dataset_id}/{run_number}/"
         headers = self._build_headers()
-        response = requests.get(endpoint_url, headers=headers)
+        response = requests.get(endpoint_url, headers=headers, timeout=self.default_timeout)
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
```

### Comparing `cmsdials-1.0.1/cmsdials/clients/run/models.py` & `cmsdials-1.1.0/cmsdials/clients/run/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional
 
 from pydantic import AnyUrl, BaseModel, Field
 
-from ...utils.base_model import OBaseModel
+from ...utils.base_model import OBaseModel, PaginatedBaseModel
 
 
 class Run(BaseModel):
     dataset_id: int
     dataset: str = Field(..., max_length=255)
     run_number: int
     ls_count: int
 
 
-class PaginatedRunList(BaseModel):
+class PaginatedRunList(PaginatedBaseModel):
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: list[Run]
 
 
 class RunFilters(OBaseModel):
     next_token: Optional[str] = None
```

### Comparing `cmsdials-1.0.1/cmsdials/cmsdials.py` & `cmsdials-1.1.0/cmsdials/cmsdials.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Optional
 
 from .auth._base import BaseCredentials
 from .clients.file_index.client import FileIndexClient
 from .clients.h1d.client import LumisectionHistogram1DClient
 from .clients.h2d.client import LumisectionHistogram2DClient
 from .clients.lumisection.client import LumisectionClient
+from .clients.mes.client import MonitoringElementClient
 from .clients.run.client import RunClient
 
 
 class Dials:
     def __init__(self, creds: BaseCredentials, workspace: Optional[str] = None, *args, **kwargs) -> None:
         self.file_index = FileIndexClient(creds, workspace, *args, **kwargs)
         self.h1d = LumisectionHistogram1DClient(creds, workspace, *args, **kwargs)
         self.h2d = LumisectionHistogram2DClient(creds, workspace, *args, **kwargs)
         self.lumi = LumisectionClient(creds, workspace, *args, **kwargs)
         self.run = RunClient(creds, workspace, *args, **kwargs)
+        self.mes = MonitoringElementClient(creds, workspace, *args, **kwargs)
```

### Comparing `cmsdials-1.0.1/cmsdials/utils/_json.py` & `cmsdials-1.1.0/cmsdials/utils/_json.py`

 * *Files identical despite different names*

### Comparing `cmsdials-1.0.1/cmsdials/utils/api_client.py` & `cmsdials-1.1.0/cmsdials/utils/api_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+from importlib import util as importlib_util
 from typing import Optional
 from urllib.parse import parse_qs, urlparse
 
 import requests
 from requests.exceptions import HTTPError
 
 from ..auth._base import BaseCredentials
 from ..utils.logger import logger
 
 
+if importlib_util.find_spec("tqdm"):
+    from tqdm import tqdm
+
+    TQDM_INSTALLED = True
+else:
+    TQDM_INSTALLED = False
+
+
 class BaseAPIClient:
     PRODUCTION_BASE_URL = "https://cmsdials-api.web.cern.ch/"
     PRODUCTION_API_ROUTE = "api/"
     PRODUCTION_API_VERSION = "v1/"
 
     def __init__(
         self, base_url: Optional[str] = None, route: Optional[str] = None, version: Optional[str] = None
@@ -32,14 +41,15 @@
 
 
 class BaseAuthorizedAPIClient(BaseAPIClient):
     data_model = None
     pagination_model = None
     filter_class = None
     lookup_url = None
+    default_timeout = 30  # seconds
 
     def __init__(
         self,
         creds: BaseCredentials,
         workspace: Optional[str] = None,
         *args: str,
         **kwargs: str,
@@ -51,59 +61,81 @@
     def _build_headers(self) -> dict:
         base = {"accept": "application/json"}
         if self.workspace is not None:
             base["Workspace"] = self.workspace
         self.creds.before_request(base)
         return base
 
-    def get(self, id: int):
+    def get(self, id: int):  # noqa: A002
         endpoint_url = self.api_url + self.lookup_url + str(id) + "/"
         headers = self._build_headers()
-        response = requests.get(endpoint_url, headers=headers)
+        response = requests.get(endpoint_url, headers=headers, timeout=self.default_timeout)
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
 
         response = response.json()
         return self.data_model(**response)
 
     def list(self, filters=None):
         filters = filters or self.filter_class()
         endpoint_url = self.api_url + self.lookup_url
         headers = self._build_headers()
-        response = requests.get(endpoint_url, headers=headers, params=filters.cleandict())
+        response = requests.get(endpoint_url, headers=headers, params=filters.cleandict(), timeout=self.default_timeout)
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
 
         response = response.json()
-        return self.pagination_model(**response)
+        if self.pagination_model:
+            return self.pagination_model(**response)
+        elif isinstance(response, list):
+            return [self.data_model(**res) for res in response]
+
+        raise ValueError("pagination model is None and response is not a list.")
 
     def __list_sync(self, filters, max_pages: Optional[int] = None):
         next_token = None
         results = []
         is_last_page = False
         total_pages = 0
 
+        if TQDM_INSTALLED:
+            progress = tqdm(desc="Progress", total=1)
+
         while is_last_page is False:
             curr_filters = self.filter_class(**filters.dict())
             curr_filters.next_token = next_token
             response = self.list(curr_filters)
             results.extend(response.results)
             is_last_page = response.next is None
             next_token = parse_qs(urlparse(response.next).query).get("next_token") if response.next else None
             total_pages += 1
-            if max_pages and total_pages > max_pages:
+            max_pages_reached = max_pages and total_pages >= max_pages
+            if TQDM_INSTALLED:
+                if is_last_page or max_pages_reached:
+                    progress.update()
+                else:
+                    progress.total = total_pages + 1
+                    progress.update(1)
+            if max_pages_reached:
                 break
 
+        if TQDM_INSTALLED:
+            progress.close()
+
         return self.pagination_model(
-            next=None, previous=None, results=results  # No problem re-using last response count
+            next=None,
+            previous=None,
+            results=results,  # No problem re-using last response count
         )
 
     def list_all(self, filters, max_pages: Optional[int] = None):
+        if self.pagination_model is None:
+            return self.list(filters)
         return self.__list_sync(filters, max_pages)
```

### Comparing `cmsdials-1.0.1/pyproject.toml` & `cmsdials-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmsdials"
-version = "1.0.1"
+version = "1.1.0"
 description = "The Python api client interface to DIALS service"
 authors = ["Gabriel Moreira <gabrielmscampos@gmail.com>"]
 readme = "README.md"
 include = ["LICENSE"]
 repository = "https://github.com/cms-DQM/dials-py"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -17,18 +17,26 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 pydantic = "<2, >=1"
 typing-extensions = "<4.6.0, >=3.6.6"
+pandas = {version = ">=1.5.3", optional = true}
+tqdm = {version = ">=4.66.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.6.2"
 ruff = "^0.4.2"
+notebook = "^7.1.3"
+pytest = "^8.2.0"
+
+[tool.poetry.extras]
+pandas = ["pandas"]
+tqdm = ["tqdm"]
 
 [tool.ruff]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
@@ -48,15 +56,15 @@
     "build",
     "dist",
     "venv",
     "virtualenvs",
 ]
 line-length = 120
 indent-width = 4
-target-version = "py310"
+target-version = "py39"
 
 [tool.ruff.lint]
 select = [
     # pycodestyle
     "E",
     # Pyflakes
     "F",
```

### Comparing `cmsdials-1.0.1/PKG-INFO` & `cmsdials-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: cmsdials
-Version: 1.0.1
+Version: 1.1.0
 Summary: The Python api client interface to DIALS service
 Home-page: https://github.com/cms-DQM/dials-py
 Author: Gabriel Moreira
 Author-email: gabrielmscampos@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: pandas
+Provides-Extra: tqdm
+Requires-Dist: pandas (>=1.5.3) ; extra == "pandas"
 Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tqdm (>=4.66.1) ; extra == "tqdm"
 Requires-Dist: typing-extensions (>=3.6.6,<4.6.0)
 Project-URL: Repository, https://github.com/cms-DQM/dials-py
 Description-Content-Type: text/markdown
 
 # dials-py
 
 The Python api client interface to DIALS service.
@@ -29,14 +33,20 @@
 
 To install dials-py, simply
 
 ```bash
 $ pip install cmsdials
 ```
 
+It is also possible to specify the following extras, to enable optional features:
+
+```
+pandas, tqdm
+```
+
 ## Usage
 
 Before interfacing with any route you need to generate valid credentials, it is possible to authenticate trough the `device authorization flow` or using the `client secret key` of any application registered in DIALS. Note that, the device flow is an interactively authentication procedure that is possible to distinguish users in DIALS backend and the client secret flow is not interactive and is not possible to distinguish users so it should only be used for automation scripts.
 
 ### Generating credentials with client secret
 
 ```python
@@ -156,20 +166,44 @@
 dials.lumi.list_all(LumisectionFilters(run_number=360392), max_pages=5)
 
 dials.run.list_all(RunFilters(run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
 
 ### Dials MEs
 
-It is possible to inspect the list of selected MEs considered in DIALS during ETL requesting the endpoint `configured-mes` trough the method:
+It is possible to inspect the list of ingested MEs in DIALS listing the endpoint `mes` trough the method:
+
+```python
+dials.mes.list()
+```
+
+### Automatically convert paginated results to pandas DataFrame
+
+You can enable this optional feature by installing the package with the `pandas` extra.
+
+All `Paginated` metaclasses contain the method `to_pandas` that will automatically transform the `results` attribute of the metaclass into a pandas dataframe, for example:
+
+```python
+data = dials.h1d.list_all(LumisectionHistogram1DFilters(me="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
+data.to_pandas()
+```
+
+### Indefinite progress bar when fetch multi-page result
+
+You can enable this optional feature by installing the package with the `tqdm` extra.
+
+Whenever you call a `list_all` method that fetches multiple pages a dynamic progress will be rendered to indicate duration and number of pages, for example:
 
 ```python
-dials.lumi.configured_mes()
+>>> dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="PXBarrel", ls_number=78, entries__gte=100), max_pages=5)
+Progress: 100%|█████████████████████████████████████| 5/5 [00:02<00:00,  1.70it/s]
 ```
 
+The total attribute of the bar is dynamically updated while fetching the pages.
+
 ## Usage with local DIALS
 
 All classes that interface the DIALS service inherits the class `BaseAPIClient` which propagate the `base_url`, `route` and `version` attributes with production values. In order to use dials-py with a local version of DIALS it is possible to overwrite those attributes when instantiating the `AuthClient` and the `Dials` client, for example:
 
 ```python
 from cmsdials.auth.client import AuthClient
 from cmsdials.auth.bearer import Credentials
@@ -182,7 +216,17 @@
 auth = AuthClient(base_url=DEV_URL)
 creds = Credentials.from_creds_file(cache_dir=DEV_CACHE_DIR, client=auth)  # Make sure to specify the auth client with overwritten values, using another cache_dir is recommended
 dials = Dials(creds, base_url=DEV_URL)
 
 dials.h2d.list_all(LumisectionHistogram2DFilters(me__regex="EEOT digi occupancy EE +", entries__gte=100, run_number__gte=360392, run_number__lte=365000), max_pages=5)
 ```
 
+## Running tests
+
+The repository has some tests written to make sure DIALS responses are compatible with pydantic metaclasses, you can use pytest to run all tests but you need to specify a secret key to authenticate non-interactively against DIALS api:
+
+```bash
+SECRET_KEY=... pytest tests
+```
+
+The secret key is an api client enabled secret key and can be obtained from the applications portal, any api client secret key whitelisted in DIALS can be used. The interactive authentication flow should be tested manually, an example for this can be found in [this line](/tests/integration/test_auth_client.py#L33).
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

