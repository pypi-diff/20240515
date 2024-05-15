# Comparing `tmp/smart_redis_storage-0.0.2.tar.gz` & `tmp/smart_redis_storage-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_redis_storage-0.0.2.tar", last modified: Mon May 13 02:46:53 2024, max compression
+gzip compressed data, was "smart_redis_storage-0.1.0.tar", last modified: Wed May 15 06:23:33 2024, max compression
```

## Comparing `smart_redis_storage-0.0.2.tar` & `smart_redis_storage-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 02:46:53.942129 smart_redis_storage-0.0.2/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-13 02:17:03.000000 smart_redis_storage-0.0.2/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)     3510 2024-05-13 02:46:53.942129 smart_redis_storage-0.0.2/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     2538 2024-05-13 02:46:17.000000 smart_redis_storage-0.0.2/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)     1056 2024-05-13 02:46:53.942129 smart_redis_storage-0.0.2/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      483 2024-05-13 02:35:33.000000 smart_redis_storage-0.0.2/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 02:46:53.938796 smart_redis_storage-0.0.2/smart_redis_storage/
--rw-r--r--   0 smart     (1000) smart     (1000)      358 2024-05-13 02:33:16.000000 smart_redis_storage-0.0.2/smart_redis_storage/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     1565 2024-05-13 02:33:16.000000 smart_redis_storage-0.0.2/smart_redis_storage/redis_storage.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-13 02:46:53.942129 smart_redis_storage-0.0.2/smart_redis_storage.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     3510 2024-05-13 02:46:53.000000 smart_redis_storage-0.0.2/smart_redis_storage.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      361 2024-05-13 02:46:53.000000 smart_redis_storage-0.0.2/smart_redis_storage.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-13 02:46:53.000000 smart_redis_storage-0.0.2/smart_redis_storage.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-13 02:46:53.000000 smart_redis_storage-0.0.2/smart_redis_storage.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-13 02:46:53.000000 smart_redis_storage-0.0.2/smart_redis_storage.egg-info/requires.txt
--rw-r--r--   0 smart     (1000) smart     (1000)       20 2024-05-13 02:46:53.000000 smart_redis_storage-0.0.2/smart_redis_storage.egg-info/top_level.txt
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 06:23:33.191462 smart_redis_storage-0.1.0/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-13 02:17:03.000000 smart_redis_storage-0.1.0/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)     4138 2024-05-15 06:23:33.191462 smart_redis_storage-0.1.0/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     3130 2024-05-15 06:20:31.000000 smart_redis_storage-0.1.0/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)     1094 2024-05-15 06:23:33.194795 smart_redis_storage-0.1.0/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      483 2024-05-13 02:35:33.000000 smart_redis_storage-0.1.0/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 06:23:33.191462 smart_redis_storage-0.1.0/smart_redis_storage/
+-rw-r--r--   0 smart     (1000) smart     (1000)      393 2024-05-15 06:18:56.000000 smart_redis_storage-0.1.0/smart_redis_storage/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     1580 2024-05-15 06:01:42.000000 smart_redis_storage-0.1.0/smart_redis_storage/redis_storage.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 06:23:33.191462 smart_redis_storage-0.1.0/smart_redis_storage.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     4138 2024-05-15 06:23:33.000000 smart_redis_storage-0.1.0/smart_redis_storage.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      361 2024-05-15 06:23:33.000000 smart_redis_storage-0.1.0/smart_redis_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 06:23:33.000000 smart_redis_storage-0.1.0/smart_redis_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 06:23:33.000000 smart_redis_storage-0.1.0/smart_redis_storage.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       13 2024-05-15 06:23:33.000000 smart_redis_storage-0.1.0/smart_redis_storage.egg-info/requires.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)       20 2024-05-15 06:23:33.000000 smart_redis_storage-0.1.0/smart_redis_storage.egg-info/top_level.txt
```

### Comparing `smart_redis_storage-0.0.2/LICENSE` & `smart_redis_storage-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_redis_storage-0.0.2/PKG-INFO` & `smart_redis_storage-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: smart-redis-storage
-Version: 0.0.2
+Version: 0.1.0
 Summary: Convenient work with Redis.
 Home-page: https://github.com/smartlegionlab/smart_redis_storage/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smart_redis_storage/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smart_redis_storage/releases
-Keywords: redis,django,smartlegionlab
+Keywords: redis,django,smartlegionlab,redis storage,redis storage manager
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: redis~=5.0.4
 
-# smart_redis_storage <sup>0.0.2</sup>
-Convenient work with Redis.
+# smart_redis_storage <sup>0.1.0</sup>
+Redis storage manager.
 
 ***
 
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smart_redis_storage)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smart_redis_storage?label=pypi%20downloads)](https://pypi.org/project/smart_redis_storage/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smart_redis_storage)](https://github.com/smartlegionlab/smart_redis_storage/)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smart_redis_storage)](https://github.com/smartlegionlab/smart_redis_storage/blob/master/LICENSE)
@@ -38,14 +38,37 @@
 
 ***
 
 Author and developer: ___A.A Suvorov___
 
 ***
 
+## Help:
+
+`pip install smart-redis-storage`
+
+> CRUD (Create, Read, Update, Delete) for Redis.
+> Used in a large corporate project in a multi-user CRM (Django) to store intermediate data.
+> I used user ids as uniq_key.
+> 
+> 
+
+```python
+from smart_redis_storage.redis_storage import RedisStorageManager
+
+user_id = 1
+redis_storage_manager = RedisStorageManager()
+redis_storage_manager.set_data(uniq_key=user_id, key='data', value={'id': 1, 'age': 33})
+data = redis_storage_manager.get_data(uniq_key=user_id, key='data')
+print(data) # {'id': 1, 'age': 33}
+print(type(data)) # <class 'dict'>
+```
+
+***
+
 ## Disclaimer of liability:
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
     AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
     IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
     DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
     FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
```

### Comparing `smart_redis_storage-0.0.2/README.md` & `smart_redis_storage-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# smart_redis_storage <sup>0.0.2</sup>
-Convenient work with Redis.
+# smart_redis_storage <sup>0.1.0</sup>
+Redis storage manager.
 
 ***
 
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smart_redis_storage)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smart_redis_storage?label=pypi%20downloads)](https://pypi.org/project/smart_redis_storage/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smart_redis_storage)](https://github.com/smartlegionlab/smart_redis_storage/)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smart_redis_storage)](https://github.com/smartlegionlab/smart_redis_storage/blob/master/LICENSE)
@@ -15,14 +15,37 @@
 
 ***
 
 Author and developer: ___A.A Suvorov___
 
 ***
 
+## Help:
+
+`pip install smart-redis-storage`
+
+> CRUD (Create, Read, Update, Delete) for Redis.
+> Used in a large corporate project in a multi-user CRM (Django) to store intermediate data.
+> I used user ids as uniq_key.
+> 
+> 
+
+```python
+from smart_redis_storage.redis_storage import RedisStorageManager
+
+user_id = 1
+redis_storage_manager = RedisStorageManager()
+redis_storage_manager.set_data(uniq_key=user_id, key='data', value={'id': 1, 'age': 33})
+data = redis_storage_manager.get_data(uniq_key=user_id, key='data')
+print(data) # {'id': 1, 'age': 33}
+print(type(data)) # <class 'dict'>
+```
+
+***
+
 ## Disclaimer of liability:
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
     AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
     IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
     DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
     FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
```

### Comparing `smart_redis_storage-0.0.2/setup.cfg` & `smart_redis_storage-0.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smart-redis-storage
-version = 0.0.2
+version = 0.1.0
 author = A.A Suvorov
 author_email = smartlegiondev@gmail.com
 description = Convenient work with Redis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smartlegionlab/smart_redis_storage/
 project_urls = 
@@ -19,14 +19,16 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Software Development :: Libraries :: Python Modules
 keywords = 
 	redis
 	django
 	smartlegionlab
+	redis storage
+	redis storage manager
 
 [options]
 package_dir = 
 packages = find:
 python_requires = >= 3.6
 include_package_data = true
 zip_safe = false
```

### Comparing `smart_redis_storage-0.0.2/smart_redis_storage.egg-info/PKG-INFO` & `smart_redis_storage-0.1.0/smart_redis_storage.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: smart-redis-storage
-Version: 0.0.2
+Version: 0.1.0
 Summary: Convenient work with Redis.
 Home-page: https://github.com/smartlegionlab/smart_redis_storage/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smart_redis_storage/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smart_redis_storage/releases
-Keywords: redis,django,smartlegionlab
+Keywords: redis,django,smartlegionlab,redis storage,redis storage manager
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: redis~=5.0.4
 
-# smart_redis_storage <sup>0.0.2</sup>
-Convenient work with Redis.
+# smart_redis_storage <sup>0.1.0</sup>
+Redis storage manager.
 
 ***
 
 ![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/smart_redis_storage)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/smart_redis_storage?label=pypi%20downloads)](https://pypi.org/project/smart_redis_storage/)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/smart_redis_storage)](https://github.com/smartlegionlab/smart_redis_storage/)
 [![GitHub](https://img.shields.io/github/license/smartlegionlab/smart_redis_storage)](https://github.com/smartlegionlab/smart_redis_storage/blob/master/LICENSE)
@@ -38,14 +38,37 @@
 
 ***
 
 Author and developer: ___A.A Suvorov___
 
 ***
 
+## Help:
+
+`pip install smart-redis-storage`
+
+> CRUD (Create, Read, Update, Delete) for Redis.
+> Used in a large corporate project in a multi-user CRM (Django) to store intermediate data.
+> I used user ids as uniq_key.
+> 
+> 
+
+```python
+from smart_redis_storage.redis_storage import RedisStorageManager
+
+user_id = 1
+redis_storage_manager = RedisStorageManager()
+redis_storage_manager.set_data(uniq_key=user_id, key='data', value={'id': 1, 'age': 33})
+data = redis_storage_manager.get_data(uniq_key=user_id, key='data')
+print(data) # {'id': 1, 'age': 33}
+print(type(data)) # <class 'dict'>
+```
+
+***
+
 ## Disclaimer of liability:
 
     THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
     AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
     IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
     DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
     FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
```

