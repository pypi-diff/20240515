# Comparing `tmp/sustainalytics-0.3.2.tar.gz` & `tmp/sustainalytics-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sustainalytics-0.3.2.tar", max compression
+gzip compressed data, was "sustainalytics-0.3.3.tar", max compression
```

## Comparing `sustainalytics-0.3.2.tar` & `sustainalytics-0.3.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      777 2024-03-12 10:20:02.065543 sustainalytics-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9357 2024-03-12 10:09:58.610837 sustainalytics-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-03-12 10:08:00.363041 sustainalytics-0.3.2/sustainalytics/__init__.py
--rw-r--r--   0        0        0    43144 2024-03-04 06:06:00.000000 sustainalytics-0.3.2/sustainalytics/api.py
--rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 sustainalytics-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      787 2024-05-15 09:55:10.111317 sustainalytics-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9345 2023-12-28 09:04:12.574967 sustainalytics-0.3.3/README.md
+-rw-r--r--   0        0        0       23 2023-12-28 09:04:12.806487 sustainalytics-0.3.3/sustainalytics/__init__.py
+-rw-r--r--   0        0        0    43919 2024-05-15 08:42:10.826626 sustainalytics-0.3.3/sustainalytics/api.py
+-rw-r--r--   0        0        0     2976 2024-05-15 08:50:52.570276 sustainalytics-0.3.3/sustainalytics/main.py
+-rw-r--r--   0        0        0    10276 1970-01-01 00:00:00.000000 sustainalytics-0.3.3/PKG-INFO
```

### Comparing `sustainalytics-0.3.2/pyproject.toml` & `sustainalytics-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sustainalytics"
-version = "0.3.2"
+version = "0.3.3"
 description = "This is a package that helps clients access sustainalytics API"
 readme = "README.md"
 authors = ["Kienka Cromwell Kio <kienka.kio@morningstar.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
@@ -22,13 +22,14 @@
 python-dateutil = "*"
 pytz = "*"
 requests = "*"
 six = "*"
 tqdm = "*"
 tzdata = "*"
 urllib3 = "*"
+re = "*"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sustainalytics-0.3.2/README.md` & `sustainalytics-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 ```
 
 ```python
 # GetData for time series research data (default dtype='json') - TimeSeriesData endpoint.
 timestamped_research_data = con.get_data(identifiers=[], packageIds=[], productId=x, fieldClusterIds=[], fieldIds=[], dtype='dataframe', time_series=True)
 print(timestamped_research_data)
 
-# GetData for time series timestamped research data (default dtype='json') - TimeSeriesDataWTimestamps endpoint.
+# GetData for timestamped research data (default dtype='json') - TimeSeriesDataWTimestamps endpoint.
 timestamped_research_data = con.get_data(identifiers=[], packageIds=[], productId=x, fieldClusterIds=[], fieldIds=[], dtype='dataframe', time_series=True, timestamps=True)
 print(timestamped_research_data)
 ```
 
 #### Get LastChangesSince
 Retrieves data from the LastChangesSince endpoint. 'startdate' and 'productId' are **mandatory** arguments.
```

### Comparing `sustainalytics-0.3.2/sustainalytics/api.py` & `sustainalytics-0.3.3/sustainalytics/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import requests
+import re
 import pandas as pd
 import numpy as np
 import itertools
 from dateutil.relativedelta import relativedelta
 from typing import Any, Union
 from tqdm import tqdm
 
@@ -614,14 +615,28 @@
         requests_url = requests.get(f"https://api.sustainalytics.com/v2/{endpoint}",
                                     headers=self.access_headers, params=params, timeout=180).json()
         if dtype == 'json':
             temp_data = requests_url
             extracted_data = extracted_data + temp_data
             return extracted_data
         else:
+            if 'message' in requests_url:
+                identifiers = re.findall(r"'(.*?)'", requests_url['message'])
+                identifiers = identifiers[0].split(',')
+                # Initialize list to store dictionaries
+                identifiers_list = list()
+
+                # Construct dictionary for each identifier
+                for identifier in identifiers:
+                    identifier_dict = {'identifier': identifier, 'status': {'matched': 'No', 'hasPermissions': False}}
+                    identifiers_list.append(identifier_dict)
+                temp_data = pd.DataFrame(identifiers_list)
+                extracted_data = pd.concat([extracted_data, temp_data], ignore_index=True)
+                return extracted_data
+
             temp_data = pd.DataFrame(requests_url)
             extracted_data = pd.concat([extracted_data, temp_data], ignore_index=True)
             return extracted_data
 
     def __make_request_to_endpoint(self, all_parameter_values: tuple, extracted_data: Union[list, pd.DataFrame],
                                    endpoint: str, dtype: str) -> Union[list, pd.DataFrame]:
         """Makes a request to a given V2 endpoint.
```

### Comparing `sustainalytics-0.3.2/PKG-INFO` & `sustainalytics-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sustainalytics
-Version: 0.3.2
+Version: 0.3.3
 Summary: This is a package that helps clients access sustainalytics API
 License: MIT
 Author: Kienka Cromwell Kio
 Author-email: kienka.kio@morningstar.com
 Requires-Python: >=3.6
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,15 @@
 Requires-Dist: charset-normalizer
 Requires-Dist: colorama
 Requires-Dist: idna
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
+Requires-Dist: re
 Requires-Dist: requests
 Requires-Dist: six
 Requires-Dist: tqdm
 Requires-Dist: tzdata
 Requires-Dist: urllib3
 Description-Content-Type: text/markdown
 
@@ -149,15 +150,15 @@
 ```
 
 ```python
 # GetData for time series research data (default dtype='json') - TimeSeriesData endpoint.
 timestamped_research_data = con.get_data(identifiers=[], packageIds=[], productId=x, fieldClusterIds=[], fieldIds=[], dtype='dataframe', time_series=True)
 print(timestamped_research_data)
 
-# GetData for time series timestamped research data (default dtype='json') - TimeSeriesDataWTimestamps endpoint.
+# GetData for timestamped research data (default dtype='json') - TimeSeriesDataWTimestamps endpoint.
 timestamped_research_data = con.get_data(identifiers=[], packageIds=[], productId=x, fieldClusterIds=[], fieldIds=[], dtype='dataframe', time_series=True, timestamps=True)
 print(timestamped_research_data)
 ```
 
 #### Get LastChangesSince
 Retrieves data from the LastChangesSince endpoint. 'startdate' and 'productId' are **mandatory** arguments.
```

