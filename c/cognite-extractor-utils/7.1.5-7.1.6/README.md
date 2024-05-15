# Comparing `tmp/cognite_extractor_utils-7.1.5.tar.gz` & `tmp/cognite_extractor_utils-7.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-7.1.5.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-7.1.6.tar", max compression
```

## Comparing `cognite_extractor_utils-7.1.5.tar` & `cognite_extractor_utils-7.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10173 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/LICENSE
--rw-r--r--   0        0        0     4090 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/README.md
--rw-r--r--   0        0        0      739 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    16391 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     3059 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    21564 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0    16317 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1084 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    15509 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0        0 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    18667 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3605 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/threading.py
--rw-r--r--   0        0        0     3110 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     5304 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3247 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     5628 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/assets.py
--rw-r--r--   0        0        0     5680 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    18329 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     6738 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26817 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7732 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1020 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    17198 2024-05-10 08:27:23.976598 cognite_extractor_utils-7.1.5/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2088 2024-05-10 08:27:23.976598 cognite_extractor_utils-7.1.5/pyproject.toml
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/LICENSE
+-rw-r--r--   0        0        0     4090 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/README.md
+-rw-r--r--   0        0        0      739 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    16391 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     3059 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    21564 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0    16317 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1084 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    15509 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0        0 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    18667 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3605 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/threading.py
+-rw-r--r--   0        0        0     3110 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5304 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3247 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5628 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/assets.py
+-rw-r--r--   0        0        0     5680 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    18329 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6738 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26817 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7732 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1020 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    17198 2024-05-15 10:34:22.116807 cognite_extractor_utils-7.1.6/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2088 2024-05-15 10:34:22.116807 cognite_extractor_utils-7.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.6/PKG-INFO
```

### Comparing `cognite_extractor_utils-7.1.5/LICENSE` & `cognite_extractor_utils-7.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/README.md` & `cognite_extractor_utils-7.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "7.1.5"
+__version__ = "7.1.6"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/base.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/elements.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/statestore.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/threading.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/threading.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/assets.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/events.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/files.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/cognite/extractorutils/util.py` & `cognite_extractor_utils-7.1.6/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.5/pyproject.toml` & `cognite_extractor_utils-7.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "7.1.5"
+version = "7.1.6"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
@@ -49,15 +49,15 @@
 show_error_codes = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 exclude = "tests/*"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-cognite-sdk = "^7.41.0"
+cognite-sdk = "^7.43.3"
 prometheus-client = ">0.7.0, <=1.0.0"
 arrow = "^1.0.0"
 pyyaml = ">=5.3.0, <7"
 dacite = "^1.6.0"
 psutil = "^5.7.0"
 decorator = "^5.1.1"
 more-itertools = "^10.0.0"
```

### Comparing `cognite_extractor_utils-7.1.5/PKG-INFO` & `cognite_extractor_utils-7.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 7.1.5
+Version: 7.1.6
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: experimental
 Requires-Dist: arrow (>=1.0.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.14.0,<2.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
-Requires-Dist: cognite-sdk (>=7.41.0,<8.0.0)
+Requires-Dist: cognite-sdk (>=7.43.3,<8.0.0)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
 Requires-Dist: prometheus-client (>0.7.0,<=1.0.0)
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=5.3.0,<7)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.5 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.6 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: experimental Requires-Dist: arrow (>=1.0.0,<2.0.0) Requires-
 Dist: azure-identity (>=1.14.0,<2.0.0) Requires-Dist: azure-keyvault-secrets
-(>=4.7.0,<5.0.0) Requires-Dist: cognite-sdk (>=7.41.0,<8.0.0) Requires-Dist:
+(>=4.7.0,<5.0.0) Requires-Dist: cognite-sdk (>=7.43.3,<8.0.0) Requires-Dist:
 dacite (>=1.6.0,<2.0.0) Requires-Dist: decorator (>=5.1.1,<6.0.0) Requires-
 Dist: more-itertools (>=10.0.0,<11.0.0) Requires-Dist: prometheus-client
 (>0.7.0,<=1.0.0) Requires-Dist: psutil (>=5.7.0,<6.0.0) Requires-Dist: python-
 dotenv (>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=5.3.0,<7) Requires-Dist:
 typing-extensions (>=3.7.4,<5) Project-URL: Repository, https://github.com/
 cognitedata/python-extractor-utils Description-Content-Type: text/markdown
 _[_C_o_g_n_i_t_e_ _l_o_g_o_]Cognite Python `extractor-utils` ================================
```

