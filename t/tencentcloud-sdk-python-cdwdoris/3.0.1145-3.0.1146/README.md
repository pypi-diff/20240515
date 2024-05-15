# Comparing `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1145.tar.gz` & `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1146.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1145.tar", last modified: Mon May 13 20:36:56 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1146.tar", last modified: Tue May 14 20:50:06 2024, max compression
```

## Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145.tar` & `tencentcloud-sdk-python-cdwdoris-3.0.1146.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/
--rw-r--r--   0 root         (0) root         (0)    16479 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   129648 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      752 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/README.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-13 20:36:56.000000 tencentcloud-sdk-python-cdwdoris-3.0.1145/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/README.rst
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/
+-rw-r--r--   0 root         (0) root         (0)    16479 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
+-rw-r--r--   0 root         (0) root         (0)   132125 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-14 20:50:06.000000 tencentcloud-sdk-python-cdwdoris-3.0.1146/setup.py
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1145'
+__version__ = '3.0.1146'
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/errorcodes.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud/cdwdoris/v20211228/models.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud/cdwdoris/v20211228/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2129,20 +2129,32 @@
         :type QueryDurationMs: int
         :param _StartTime: 开始时间
         :type StartTime: str
         :param _EndTime: 结束时间
         :type EndTime: str
         :param _DurationMs: 排序参数
         :type DurationMs: str
+        :param _Sql: 查询sql
+        :type Sql: str
+        :param _ReadRows: 排序参数
+        :type ReadRows: str
+        :param _ResultBytes: 排序参数
+        :type ResultBytes: str
+        :param _MemoryUsage: 排序参数
+        :type MemoryUsage: str
         """
         self._InstanceId = None
         self._QueryDurationMs = None
         self._StartTime = None
         self._EndTime = None
         self._DurationMs = None
+        self._Sql = None
+        self._ReadRows = None
+        self._ResultBytes = None
+        self._MemoryUsage = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -2176,21 +2188,57 @@
     def DurationMs(self):
         return self._DurationMs
 
     @DurationMs.setter
     def DurationMs(self, DurationMs):
         self._DurationMs = DurationMs
 
+    @property
+    def Sql(self):
+        return self._Sql
+
+    @Sql.setter
+    def Sql(self, Sql):
+        self._Sql = Sql
+
+    @property
+    def ReadRows(self):
+        return self._ReadRows
+
+    @ReadRows.setter
+    def ReadRows(self, ReadRows):
+        self._ReadRows = ReadRows
+
+    @property
+    def ResultBytes(self):
+        return self._ResultBytes
+
+    @ResultBytes.setter
+    def ResultBytes(self, ResultBytes):
+        self._ResultBytes = ResultBytes
+
+    @property
+    def MemoryUsage(self):
+        return self._MemoryUsage
+
+    @MemoryUsage.setter
+    def MemoryUsage(self, MemoryUsage):
+        self._MemoryUsage = MemoryUsage
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._QueryDurationMs = params.get("QueryDurationMs")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._DurationMs = params.get("DurationMs")
+        self._Sql = params.get("Sql")
+        self._ReadRows = params.get("ReadRows")
+        self._ResultBytes = params.get("ResultBytes")
+        self._MemoryUsage = params.get("MemoryUsage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2257,25 +2305,37 @@
         :type DurationMs: str
         :param _DbName: 数据库名称
         :type DbName: list of str
         :param _IsQuery: 是否是查询，0：否， 1：是
         :type IsQuery: int
         :param _CatalogName: catalog名称
         :type CatalogName: list of str
+        :param _Sql: sql名
+        :type Sql: str
+        :param _ReadRows: ReadRows排序字段
+        :type ReadRows: str
+        :param _ResultBytes: ResultBytes排序字段
+        :type ResultBytes: str
+        :param _MemoryUsage: MemoryUsage排序字段
+        :type MemoryUsage: str
         """
         self._InstanceId = None
         self._QueryDurationMs = None
         self._StartTime = None
         self._EndTime = None
         self._PageSize = None
         self._PageNum = None
         self._DurationMs = None
         self._DbName = None
         self._IsQuery = None
         self._CatalogName = None
+        self._Sql = None
+        self._ReadRows = None
+        self._ResultBytes = None
+        self._MemoryUsage = None
 
     @property
     def InstanceId(self):
         return self._InstanceId
 
     @InstanceId.setter
     def InstanceId(self, InstanceId):
@@ -2349,26 +2409,62 @@
     def CatalogName(self):
         return self._CatalogName
 
     @CatalogName.setter
     def CatalogName(self, CatalogName):
         self._CatalogName = CatalogName
 
+    @property
+    def Sql(self):
+        return self._Sql
+
+    @Sql.setter
+    def Sql(self, Sql):
+        self._Sql = Sql
+
+    @property
+    def ReadRows(self):
+        return self._ReadRows
+
+    @ReadRows.setter
+    def ReadRows(self, ReadRows):
+        self._ReadRows = ReadRows
+
+    @property
+    def ResultBytes(self):
+        return self._ResultBytes
+
+    @ResultBytes.setter
+    def ResultBytes(self, ResultBytes):
+        self._ResultBytes = ResultBytes
+
+    @property
+    def MemoryUsage(self):
+        return self._MemoryUsage
+
+    @MemoryUsage.setter
+    def MemoryUsage(self, MemoryUsage):
+        self._MemoryUsage = MemoryUsage
+
 
     def _deserialize(self, params):
         self._InstanceId = params.get("InstanceId")
         self._QueryDurationMs = params.get("QueryDurationMs")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._PageSize = params.get("PageSize")
         self._PageNum = params.get("PageNum")
         self._DurationMs = params.get("DurationMs")
         self._DbName = params.get("DbName")
         self._IsQuery = params.get("IsQuery")
         self._CatalogName = params.get("CatalogName")
+        self._Sql = params.get("Sql")
+        self._ReadRows = params.get("ReadRows")
+        self._ResultBytes = params.get("ResultBytes")
+        self._MemoryUsage = params.get("MemoryUsage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1145
+Version: 3.0.1146
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1145
+Version: 3.0.1146
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/README.rst` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1145/setup.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1146/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdwdoris',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1145"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1146"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdwdoris SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

