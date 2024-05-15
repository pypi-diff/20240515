# Comparing `tmp/uploadcare-migro-1.8.0.tar.gz` & `tmp/uploadcare_migro-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadcare-migro-1.8.0.tar", last modified: Tue Jun 14 14:53:02 2022, max compression
+gzip compressed data, was "uploadcare_migro-2.0.0.tar", last modified: Wed May 15 13:44:01 2024, max compression
```

## Comparing `uploadcare-migro-1.8.0.tar` & `uploadcare_migro-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxrwxr-x   0 mojo      (1000) mojo      (1000)        0 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     1081 2022-05-25 14:26:10.000000 uploadcare-migro-1.8.0/LICENSE
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     5252 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/PKG-INFO
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     4560 2022-05-25 14:19:00.000000 uploadcare-migro-1.8.0/README.rst
-drwxrwxr-x   0 mojo      (1000) mojo      (1000)        0 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/migro/
--rw-rw-r--   0 mojo      (1000) mojo      (1000)      105 2022-06-14 14:48:15.000000 uploadcare-migro-1.8.0/migro/__init__.py
--rwxrwxr-x   0 mojo      (1000) mojo      (1000)     6547 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/migro/cli.py
-drwxrwxr-x   0 mojo      (1000) mojo      (1000)        0 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/migro/filestack/
--rw-rw-r--   0 mojo      (1000) mojo      (1000)       96 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/migro/filestack/__init__.py
--rw-rw-r--   0 mojo      (1000) mojo      (1000)      452 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/migro/filestack/utils.py
--rw-rw-r--   0 mojo      (1000) mojo      (1000)      573 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/migro/settings.py
-drwxrwxr-x   0 mojo      (1000) mojo      (1000)        0 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/migro/uploader/
--rw-rw-r--   0 mojo      (1000) mojo      (1000)       83 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/migro/uploader/__init__.py
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     2077 2022-06-14 14:48:15.000000 uploadcare-migro-1.8.0/migro/uploader/utils.py
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     8990 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/migro/uploader/worker.py
--rw-rw-r--   0 mojo      (1000) mojo      (1000)      109 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/setup.cfg
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     1437 2022-05-25 14:28:05.000000 uploadcare-migro-1.8.0/setup.py
-drwxrwxr-x   0 mojo      (1000) mojo      (1000)        0 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/tests/
--rw-rw-r--   0 mojo      (1000) mojo      (1000)        0 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/tests/__init__.py
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     1015 2022-05-25 13:54:21.000000 uploadcare-migro-1.8.0/tests/conftest.py
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     1119 2022-06-14 14:48:15.000000 uploadcare-migro-1.8.0/tests/test_uploader.py
-drwxrwxr-x   0 mojo      (1000) mojo      (1000)        0 2022-06-14 14:53:02.961348 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/
--rw-rw-r--   0 mojo      (1000) mojo      (1000)     5252 2022-06-14 14:53:02.000000 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/PKG-INFO
--rw-rw-r--   0 mojo      (1000) mojo      (1000)      555 2022-06-14 14:53:02.000000 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/SOURCES.txt
--rw-rw-r--   0 mojo      (1000) mojo      (1000)        1 2022-06-14 14:53:02.000000 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/dependency_links.txt
--rw-rw-r--   0 mojo      (1000) mojo      (1000)       41 2022-06-14 14:53:02.000000 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/entry_points.txt
--rw-rw-r--   0 mojo      (1000) mojo      (1000)        1 2022-05-25 14:41:12.000000 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/not-zip-safe
--rw-rw-r--   0 mojo      (1000) mojo      (1000)       80 2022-06-14 14:53:02.000000 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/requires.txt
--rw-rw-r--   0 mojo      (1000) mojo      (1000)       12 2022-06-14 14:53:02.000000 uploadcare-migro-1.8.0/uploadcare_migro.egg-info/top_level.txt
+drwxr-xr-x   0 mojo      (1000) mojo      (1000)        0 2024-05-15 13:44:01.801701 uploadcare_migro-2.0.0/
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     1081 2024-05-15 13:21:07.000000 uploadcare_migro-2.0.0/LICENSE
+-rw-r--r--   0 mojo      (1000) mojo      (1000)    10429 2024-05-15 13:44:01.801701 uploadcare_migro-2.0.0/PKG-INFO
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     9401 2024-05-15 13:43:49.000000 uploadcare_migro-2.0.0/README.rst
+drwxr-xr-x   0 mojo      (1000) mojo      (1000)        0 2024-05-15 13:44:01.798701 uploadcare_migro-2.0.0/db/
+-rw-r--r--   0 mojo      (1000) mojo      (1000)       58 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/db/__init__.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     8545 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/db/db_manager.py
+drwxr-xr-x   0 mojo      (1000) mojo      (1000)        0 2024-05-15 13:44:01.798701 uploadcare_migro-2.0.0/migro/
+-rw-r--r--   0 mojo      (1000) mojo      (1000)      105 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/__init__.py
+-rwxr-xr-x   0 mojo      (1000) mojo      (1000)     8923 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/cli.py
+drwxr-xr-x   0 mojo      (1000) mojo      (1000)        0 2024-05-15 13:44:01.798701 uploadcare_migro-2.0.0/migro/filestack/
+-rw-rw-r--   0 mojo      (1000) mojo      (1000)       96 2022-06-08 13:32:35.000000 uploadcare_migro-2.0.0/migro/filestack/__init__.py
+-rw-rw-r--   0 mojo      (1000) mojo      (1000)      452 2022-06-08 13:32:35.000000 uploadcare_migro-2.0.0/migro/filestack/utils.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)      817 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/settings.py
+drwxr-xr-x   0 mojo      (1000) mojo      (1000)        0 2024-05-15 13:44:01.799701 uploadcare_migro-2.0.0/migro/uploader/
+-rw-rw-r--   0 mojo      (1000) mojo      (1000)       83 2022-06-08 13:32:35.000000 uploadcare_migro-2.0.0/migro/uploader/__init__.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     6035 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/uploader/fetcher.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     1240 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/uploader/process_loop.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     3258 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/uploader/s3_client.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     2090 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/uploader/utils.py
+-rw-rw-r--   0 mojo      (1000) mojo      (1000)     8990 2022-06-08 13:32:35.000000 uploadcare_migro-2.0.0/migro/uploader/worker.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)      591 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/migro/utils.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)      264 2024-05-15 13:22:25.000000 uploadcare_migro-2.0.0/pyproject.toml
+-rw-rw-r--   0 mojo      (1000) mojo      (1000)      108 2024-05-15 13:44:01.801701 uploadcare_migro-2.0.0/setup.cfg
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     1624 2024-05-15 13:36:34.000000 uploadcare_migro-2.0.0/setup.py
+drwxr-xr-x   0 mojo      (1000) mojo      (1000)        0 2024-05-15 13:44:01.799701 uploadcare_migro-2.0.0/tests/
+-rw-rw-r--   0 mojo      (1000) mojo      (1000)        0 2022-06-08 13:32:35.000000 uploadcare_migro-2.0.0/tests/__init__.py
+-rw-rw-r--   0 mojo      (1000) mojo      (1000)     1015 2022-06-08 14:50:08.000000 uploadcare_migro-2.0.0/tests/conftest.py
+-rw-r--r--   0 mojo      (1000) mojo      (1000)     1119 2024-05-15 13:11:52.000000 uploadcare_migro-2.0.0/tests/test_uploader.py
+drwxr-xr-x   0 mojo      (1000) mojo      (1000)        0 2024-05-15 13:44:01.800701 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/
+-rw-r--r--   0 mojo      (1000) mojo      (1000)    10429 2024-05-15 13:44:01.000000 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/PKG-INFO
+-rw-r--r--   0 mojo      (1000) mojo      (1000)      702 2024-05-15 13:44:01.000000 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/SOURCES.txt
+-rw-r--r--   0 mojo      (1000) mojo      (1000)        1 2024-05-15 13:44:01.000000 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/dependency_links.txt
+-rw-r--r--   0 mojo      (1000) mojo      (1000)       40 2024-05-15 13:44:01.000000 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/entry_points.txt
+-rw-r--r--   0 mojo      (1000) mojo      (1000)        1 2024-05-15 13:27:22.000000 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/not-zip-safe
+-rw-r--r--   0 mojo      (1000) mojo      (1000)      134 2024-05-15 13:44:01.000000 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/requires.txt
+-rw-r--r--   0 mojo      (1000) mojo      (1000)       15 2024-05-15 13:44:01.000000 uploadcare_migro-2.0.0/uploadcare_migro.egg-info/top_level.txt
```

### Comparing `uploadcare-migro-1.8.0/LICENSE` & `uploadcare_migro-2.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Uploadcare, Inc
+Copyright (c) 2024 Uploadcare, Inc
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `uploadcare-migro-1.8.0/migro/uploader/utils.py` & `uploadcare_migro-2.0.0/migro/uploader/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
     Helpers functions.
 
 """
 import hashlib
 import hmac
 import time
-
-from aiohttp import ClientSession, TCPConnector
 from asyncio import get_event_loop
 from urllib.parse import urljoin
 
-from migro import settings, __version__ as version
+from aiohttp import ClientSession, TCPConnector
 
+from migro import __version__ as version
+from migro import settings
 
 loop = get_event_loop()
 session = ClientSession(connector=TCPConnector(verify_ssl=False, loop=loop))
 
 
 async def request(path, params=None):
     """Makes GET upload API request with specific path and params.
@@ -38,19 +38,19 @@
     }
 
     if params is None:
         params = {}
     params['pub_key'] = settings.PUBLIC_KEY
     params['UPLOADCARE_PUB_KEY'] = settings.PUBLIC_KEY
 
-    if (settings.SECRET_KEY):
+    if settings.SECRET_KEY:
         expire_timestamp = generate_expire_timestamp()
         upload_signature = generate_secure_signature(settings.SECRET_KEY, expire_timestamp)
 
-        params['signature'] =  upload_signature
+        params['signature'] = upload_signature
         params['expire'] = expire_timestamp
 
     response = await session.request(
         method='get',
         url=url,
         headers=headers,
         allow_redirects=True,
```

### Comparing `uploadcare-migro-1.8.0/migro/uploader/worker.py` & `uploadcare_migro-2.0.0/migro/uploader/worker.py`

 * *Files identical despite different names*

### Comparing `uploadcare-migro-1.8.0/setup.py` & `uploadcare_migro-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 with open('migro/__init__.py', 'r') as fd:
     version = re.search(r"^__version__\s*=\s*['\']([^'\']*)['\']",
                         fd.read(), re.MULTILINE).group(1)
 
 long_description = open('README.rst', encoding='utf-8').read()
 
+
 setup(
     name='uploadcare-migro',
     version=version,
     description='Uploadcare migration tool',
     long_description=long_description,
     url='https://github.com/uploadcare/migro',
     license='MIT',
@@ -28,26 +29,31 @@
     entry_points={
         'console_scripts': [
             'migro = migro.cli:cli',
         ]
     },
     zip_safe=False,
     install_requires=[
-        'aiohttp==3.8.1',
-        'click==8.1.3',
+        'aiohttp==3.9.5',
+        'click==8.1.7',
         'python-dateutil==2.8.2',
-        'tqdm==4.64.0',
-        'colorama==0.4.4',
+        'tqdm==4.66.4',
+        'colorama==0.4.6',
+        'boto3==1.34.80',
+        'botocore==1.34.80',
+        'python-dotenv==1.0.1'
     ],
     include_package_data=True,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ]
 )
```

### Comparing `uploadcare-migro-1.8.0/tests/conftest.py` & `uploadcare_migro-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uploadcare-migro-1.8.0/tests/test_uploader.py` & `uploadcare_migro-2.0.0/tests/test_uploader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from unittest.mock import AsyncMock
 
+from migro import __version__, settings
 from migro.uploader.utils import loop, request, session
-from migro.uploader.worker import Uploader, Events
-from migro import settings, __version__
+from migro.uploader.worker import Events, Uploader
 
 
 def test_uploader(mock_session):
     successful = []
     failed = []
 
     uploader = Uploader(loop=loop)
```

