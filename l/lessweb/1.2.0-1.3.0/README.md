# Comparing `tmp/lessweb-1.2.0.tar.gz` & `tmp/lessweb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-1.2.0.tar", last modified: Sun Apr  7 07:34:04 2024, max compression
+gzip compressed data, was "lessweb-1.3.0.tar", last modified: Wed May 15 03:12:47 2024, max compression
```

## Comparing `lessweb-1.2.0.tar` & `lessweb-1.3.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.523677 lessweb-1.2.0/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.515708 lessweb-1.2.0/.github/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.517634 lessweb-1.2.0/.github/workflows/
--rw-r--r--   0 zhangji    (502) staff       (20)      941 2024-03-28 06:37:50.000000 lessweb-1.2.0/.github/workflows/python-package.yml
--rw-r--r--   0 zhangji    (502) staff       (20)     1093 2024-03-28 06:00:47.000000 lessweb-1.2.0/.gitignore
--rw-r--r--   0 zhangji    (502) staff       (20)      556 2024-03-28 00:41:05.000000 lessweb-1.2.0/LICENSE.txt
--rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-07 07:34:04.523489 lessweb-1.2.0/PKG-INFO
--rw-r--r--   0 zhangji    (502) staff       (20)     1706 2024-03-28 00:41:05.000000 lessweb-1.2.0/README.md
--rw-r--r--   0 zhangji    (502) staff       (20)      315 2024-03-28 06:43:43.000000 lessweb-1.2.0/changelog.md
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.516368 lessweb-1.2.0/examples/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.517879 lessweb-1.2.0/examples/100_hello_world/
--rw-r--r--   0 zhangji    (502) staff       (20)      244 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/100_hello_world/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.518266 lessweb-1.2.0/examples/100_hello_world_config/
--rw-r--r--   0 zhangji    (502) staff       (20)       21 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/100_hello_world_config/config.toml
--rw-r--r--   0 zhangji    (502) staff       (20)      264 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/100_hello_world_config/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.518447 lessweb-1.2.0/examples/101_handle_request/
--rw-r--r--   0 zhangji    (502) staff       (20)      676 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/101_handle_request/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.518977 lessweb-1.2.0/examples/102_response/
--rw-r--r--   0 zhangji    (502) staff       (20)     1284 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/102_response/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519096 lessweb-1.2.0/examples/103_get_request/
--rw-r--r--   0 zhangji    (502) staff       (20)      772 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/103_get_request/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519315 lessweb-1.2.0/examples/205_mysql_crud/
--rw-r--r--   0 zhangji    (502) staff       (20)      169 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/config.toml
--rw-r--r--   0 zhangji    (502) staff       (20)      370 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519499 lessweb-1.2.0/examples/205_mysql_crud/myapp/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/__init__.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519936 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)      211 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/create_pet.py
--rw-r--r--   0 zhangji    (502) staff       (20)      225 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/get_pet_detail.py
--rw-r--r--   0 zhangji    (502) staff       (20)      295 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/get_pet_total.py
--rw-r--r--   0 zhangji    (502) staff       (20)     1544 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/mapper.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520059 lessweb-1.2.0/examples/205_mysql_crud/schema/
--rw-r--r--   0 zhangji    (502) staff       (20)      307 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/schema/pet.sql
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520176 lessweb-1.2.0/examples/302_cookie/
--rw-r--r--   0 zhangji    (502) staff       (20)      550 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/302_cookie/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520360 lessweb-1.2.0/examples/303_middleware/
--rw-r--r--   0 zhangji    (502) staff       (20)      533 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/303_middleware/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520548 lessweb-1.2.0/examples/304_websocket/
--rw-r--r--   0 zhangji    (502) staff       (20)     1198 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/304_websocket/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.521183 lessweb-1.2.0/examples/305_schedule_task/
--rw-r--r--   0 zhangji    (502) staff       (20)      814 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/305_schedule_task/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.521773 lessweb-1.2.0/lessweb/
--rw-r--r--   0 zhangji    (502) staff       (20)      232 2024-03-28 00:41:05.000000 lessweb-1.2.0/lessweb/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)    15065 2024-04-07 07:32:44.000000 lessweb-1.2.0/lessweb/bridge.py
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.2.0/lessweb/py.typed
--rw-r--r--   0 zhangji    (502) staff       (20)    10000 2024-04-07 06:49:29.000000 lessweb-1.2.0/lessweb/typecast.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.523238 lessweb-1.2.0/lessweb.egg-info/
--rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (502) staff       (20)     1178 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (502) staff       (20)        1 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       43 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/requires.txt
--rw-r--r--   0 zhangji    (502) staff       (20)        8 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       62 2024-03-28 06:00:47.000000 lessweb-1.2.0/mypy.ini
--rw-r--r--   0 zhangji    (502) staff       (20)      538 2024-04-07 07:17:36.000000 lessweb-1.2.0/pyproject.toml
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.522696 lessweb-1.2.0/requirements/
--rw-r--r--   0 zhangji    (502) staff       (20)       42 2024-03-28 06:00:47.000000 lessweb-1.2.0/requirements/base.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       66 2024-03-28 06:00:47.000000 lessweb-1.2.0/requirements/test.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       38 2024-04-07 07:34:04.523711 lessweb-1.2.0/setup.cfg
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.523021 lessweb-1.2.0/tests/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 06:00:47.000000 lessweb-1.2.0/tests/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)     4669 2024-04-07 06:48:10.000000 lessweb-1.2.0/tests/test_typecast.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.165947 lessweb-1.3.0/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.156158 lessweb-1.3.0/.github/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.158430 lessweb-1.3.0/.github/workflows/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1014 2024-04-12 12:13:03.000000 lessweb-1.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0 zhangji    (502) staff       (20)     1093 2024-03-28 06:00:47.000000 lessweb-1.3.0/.gitignore
+-rw-r--r--   0 zhangji    (502) staff       (20)      556 2024-03-28 00:41:05.000000 lessweb-1.3.0/LICENSE.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)     2479 2024-05-15 03:12:47.165722 lessweb-1.3.0/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1706 2024-03-28 00:41:05.000000 lessweb-1.3.0/README.md
+-rw-r--r--   0 zhangji    (502) staff       (20)      797 2024-05-15 03:11:45.000000 lessweb-1.3.0/changelog.md
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.156903 lessweb-1.3.0/examples/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.158684 lessweb-1.3.0/examples/100_hello_world/
+-rw-r--r--   0 zhangji    (502) staff       (20)      244 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/100_hello_world/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.159365 lessweb-1.3.0/examples/100_hello_world_config/
+-rw-r--r--   0 zhangji    (502) staff       (20)       21 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/100_hello_world_config/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      264 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/100_hello_world_config/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.159748 lessweb-1.3.0/examples/101_handle_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      676 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/101_handle_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.159988 lessweb-1.3.0/examples/102_response/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1284 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/102_response/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.160116 lessweb-1.3.0/examples/103_get_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      772 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/103_get_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.160371 lessweb-1.3.0/examples/205_mysql_crud/
+-rw-r--r--   0 zhangji    (502) staff       (20)      169 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      370 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.160581 lessweb-1.3.0/examples/205_mysql_crud/myapp/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/__init__.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161035 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      211 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/create_pet.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      225 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/get_pet_detail.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      295 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/get_pet_total.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     1544 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/mapper.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161167 lessweb-1.3.0/examples/205_mysql_crud/schema/
+-rw-r--r--   0 zhangji    (502) staff       (20)      307 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/schema/pet.sql
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161317 lessweb-1.3.0/examples/302_cookie/
+-rw-r--r--   0 zhangji    (502) staff       (20)      550 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/302_cookie/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161563 lessweb-1.3.0/examples/303_middleware/
+-rw-r--r--   0 zhangji    (502) staff       (20)      533 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/303_middleware/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161743 lessweb-1.3.0/examples/304_websocket/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1198 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/304_websocket/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.162064 lessweb-1.3.0/examples/305_schedule_task/
+-rw-r--r--   0 zhangji    (502) staff       (20)      814 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/305_schedule_task/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.162795 lessweb-1.3.0/lessweb/
+-rw-r--r--   0 zhangji    (502) staff       (20)      202 2024-04-09 15:15:43.000000 lessweb-1.3.0/lessweb/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)    17522 2024-04-18 15:19:24.000000 lessweb-1.3.0/lessweb/bridge.py
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.3.0/lessweb/py.typed
+-rw-r--r--   0 zhangji    (502) staff       (20)    11750 2024-04-11 08:10:34.000000 lessweb-1.3.0/lessweb/typecast.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.164735 lessweb-1.3.0/lessweb.egg-info/
+-rw-r--r--   0 zhangji    (502) staff       (20)     2479 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1209 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        1 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)      137 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        8 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       62 2024-03-28 06:00:47.000000 lessweb-1.3.0/mypy.ini
+-rw-r--r--   0 zhangji    (502) staff       (20)      724 2024-04-12 14:18:18.000000 lessweb-1.3.0/pyproject.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)       38 2024-05-15 03:12:47.165992 lessweb-1.3.0/setup.cfg
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.163868 lessweb-1.3.0/tests/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 06:00:47.000000 lessweb-1.3.0/tests/__init__.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.164390 lessweb-1.3.0/tests/e2e/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-04-11 09:53:36.000000 lessweb-1.3.0/tests/e2e/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     1708 2024-04-12 13:07:13.000000 lessweb-1.3.0/tests/e2e/test_request_stack.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      453 2024-04-12 12:12:38.000000 lessweb-1.3.0/tests/test_bridge.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     6075 2024-04-10 06:59:02.000000 lessweb-1.3.0/tests/test_typecast.py
```

### Comparing `lessweb-1.2.0/.github/workflows/python-package.yml` & `lessweb-1.3.0/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install -r requirements/test.txt
+        python -m pip install -e ".[test]"
+    - name: Lint with autopep8
+      run: |
+        autopep8 --diff -r lessweb tests
     - name: Lint with mypy
       run: |
         mypy lessweb
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `lessweb-1.2.0/.gitignore` & `lessweb-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/LICENSE.txt` & `lessweb-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/PKG-INFO` & `lessweb-1.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: lessweb
-Version: 1.2.0
-Summary: A pythonic web framework
-Author-email: qorzj <goodhorsezxj@gmail.com>
-License: Apache 2
-Keywords: lessweb,web,web.py,aiohttp
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: aiohttp
-Requires-Dist: toml
-Requires-Dist: orjson
-Requires-Dist: lesscli
-Requires-Dist: typing_inspect
-
 # lessweb
 >「嘞是web」
 
 Lessweb is an extremely easy-to-use python web framework with the following goals.
 
 * Simple and efficient: based on the aiohttp library IOC capabilities, native support for configuration loading and logging settings to meet production-level development requirements
 * Pythonic: support for the latest python version and the latest python syntax
```

### Comparing `lessweb-1.2.0/examples/101_handle_request/index.py` & `lessweb-1.3.0/examples/101_handle_request/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/examples/102_response/index.py` & `lessweb-1.3.0/examples/102_response/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/examples/103_get_request/index.py` & `lessweb-1.3.0/examples/103_get_request/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/examples/205_mysql_crud/myapp/mapper.py` & `lessweb-1.3.0/examples/205_mysql_crud/myapp/mapper.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/examples/302_cookie/index.py` & `lessweb-1.3.0/examples/302_cookie/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/examples/303_middleware/index.py` & `lessweb-1.3.0/examples/303_middleware/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/examples/304_websocket/index.py` & `lessweb-1.3.0/examples/304_websocket/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/examples/305_schedule_task/index.py` & `lessweb-1.3.0/examples/305_schedule_task/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.2.0/lessweb/bridge.py` & `lessweb-1.3.0/lessweb/bridge.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,34 +2,45 @@
 import inspect
 import logging
 import re
 import sys
 from dataclasses import dataclass, is_dataclass
 from logging.handlers import TimedRotatingFileHandler
 from os import environ, listdir
-from typing import (Any, Awaitable, Callable, Dict, Optional, Type, TypeVar,
-                    Union)
+from typing import (Any, Awaitable, Callable, Dict, Literal, Optional, Type,
+                    TypeVar, Union, cast, get_type_hints)
 
 import orjson
 import toml
+import typing_inspect
 from aiohttp.typedefs import LooseHeaders
 from aiohttp.web import (Application, HTTPBadRequest, HTTPError, Request,
                          Response, middleware, run_app)
 
-from .typecast import is_typeddict, isinstance_safe, typecast
+from .typecast import (is_typeddict, isinstance_safe, semi_json_schema_type,
+                       typecast)
 
 ENDPOINT_TYPE = Callable[..., Awaitable[Any]]
 HANDLER_TYPE = Callable[[Request], Awaitable[Any]]
+HTTP_METHOD_TYPE = Literal['GET', 'POST',
+                           'PUT', 'DELETE', 'PATCH', 'OPTIONS', 'HEAD']
 
 T = TypeVar('T')
 ORJSON_OPTION = 0
 POSITIONAL_ONLY = 0
 KEYWORD_ONLY = 3
 
 
+def cast_http_method(method: str) -> HTTP_METHOD_TYPE:
+    method = method.upper()
+    tp_args = typing_inspect.get_args(HTTP_METHOD_TYPE)
+    assert method in tp_args, f'Invalid HTTP method: {method}'
+    return cast(HTTP_METHOD_TYPE, method)
+
+
 def make_environ_key(key_path: str):
     return '_'.join(re.findall('[A-Z]+', key_path.upper()))
 
 
 def func_arg_spec(fn) -> dict:
     """
     >>> def foo(a, /, b, c=2, *d, e, f=3, **g):
@@ -152,15 +163,16 @@
         return ctx.config_dict[ref]
     logging.debug('autowire-> %s %s', ctx, cls)
     if isinstance_safe(ctx, cls):
         return ctx  # type: ignore
     elif isinstance(ctx, Request) and cls is Application:
         return ctx.app  # type: ignore
     elif not hasattr(cls, '__lessweb_service__'):
-        raise TypeError(f'cannot autowire ({ref}) {ctx=} {cls=})')
+        raise TypeError(
+            f'cannot autowire class which is not a service: {ref} {ctx=} {cls=}')
     depends_on = get_depends_on(cls.__init__)
     args: list = []
     for name, depends_type in depends_on:
         args.append(autowire(ctx, depends_type, name))
     ctx[ref] = singleton = cls(*args)
     return singleton
 
@@ -201,56 +213,65 @@
         for name, (depends_type, _, kind) in func_arg_spec(sp_handler).items():
             kwargs[name] = autowire(app, depends_type, name)
         return await sp_handler(**kwargs)
 
     return aio_handler
 
 
-def getdoc(obj) -> str:
-    """
-    获得模块或对象的docstring
-    实现了递归包含，只需要以「:include 」开头
-    """
-    if isinstance(obj, str):
-        try:
-            module_or_object = importlib.import_module(obj)
-        except ModuleNotFoundError:
-            module_name, object_name = obj.rsplit('.', 1)
-            module_or_object = getattr(
-                importlib.import_module(module_name), object_name)
-        return getdoc(module_or_object)
-    result = []
-    docstring = inspect.getdoc(obj) or ''
-    for line in docstring.splitlines():
-        if line.strip().startswith(':include '):
-            include_doc = getdoc(line.replace(':include ', '').strip())
-            result.append(include_doc)
-        else:
-            result.append(line)
-    return '\n'.join(result) + '\n'
+@dataclass
+class Route:
+    method: HTTP_METHOD_TYPE
+    paths: list
+    summary: Optional[str]
+    params: dict
+    request_body: Optional[Type]
+    response_body: Optional[Type]
+    handler: HANDLER_TYPE
+    endpoint: ENDPOINT_TYPE
+    extra: dict
 
 
-def make_router(sp_endpoint: ENDPOINT_TYPE) -> HANDLER_TYPE:
+def make_router(method: str, paths: list, sp_endpoint: ENDPOINT_TYPE) -> Route:
     """
-    :param sp_endpoint:
-        1.POSITIONAL_ONLY参数表示requestbody
-        2.int和str类型参数表示路径参数
-        3.其他参数支持可注入类型
+    :param method: HTTP方法
+    :param paths: 路径列表
+    :param sp_endpoint: 用户定义的endpoint
     :return: 形如foo(request)这样的函数
+    :raise: `TypeCastError`
     """
+    if not inspect.iscoroutinefunction(sp_endpoint):
+        raise TypeError(f'endpoint must be coroutine function: {sp_endpoint=}')
+    params: dict = {}
+    request_body: Optional[Type] = None
+    response_body: Optional[Type] = None
+    for name, (depends_type, default, kind) in func_arg_spec(sp_endpoint).items():
+        if kind == POSITIONAL_ONLY and request_body is None:
+            request_body = depends_type
+        elif kind == KEYWORD_ONLY:
+            params[name] = {
+                'name': name, 'required': default is not None, 'schema': semi_json_schema_type(depends_type)}
+
+    if get_type_hints(sp_endpoint).get('return') is not None:
+        response_body = get_type_hints(sp_endpoint)['return']
 
     async def aio_endpoint(request: Request):
-        assert inspect.iscoroutinefunction(
-            sp_endpoint), f'{sp_endpoint} must be coroutine function'
         args = []
         kwargs: Dict[str, Any] = {}
+        has_read_request_body = False
         for name, (depends_type, default, kind) in func_arg_spec(sp_endpoint).items():
             if kind == POSITIONAL_ONLY:
+                if (request_stack := request.get('lessweb.request_stack')) and isinstance(request_stack, list):
+                    request_text = request_stack.pop()
+                elif not has_read_request_body:
+                    request_text = await request.text()
+                    has_read_request_body = True
+                else:
+                    raise TypeError(f'EOF when reading request body: {name=}')
                 try:
-                    data = orjson.loads(await request.text())
+                    data = orjson.loads(request_text)
                 except orjson.JSONDecodeError:
                     raise HTTPBadRequest(
                         text=f'BadRequest: request body raise JSONDecodeError')
                 try:
                     args.append(typecast(data, depends_type))
                 except Exception as e:
                     raise HTTPBadRequest(
@@ -274,88 +295,119 @@
                 kwargs[name] = autowire(request, depends_type, name)
         result = await sp_endpoint(*args, **kwargs)
         if isinstance(result, (dict, list)) or is_dataclass(result):
             return rest_response(result)
         else:
             return result
 
-    return aio_endpoint
+    route = Route(
+        method=cast_http_method(method),
+        paths=paths,
+        summary=inspect.getdoc(sp_endpoint),
+        params=params,
+        request_body=request_body,
+        response_body=response_body,
+        handler=aio_endpoint,
+        endpoint=sp_endpoint,
+        extra={},
+    )
+    return route
 
 
-@dataclass
-class Route:
-    method: str
-    paths: list
-    handler: HANDLER_TYPE
+def contains_sub_string(s: str, sub: str) -> bool:
+    p = q = 0
+    while p < len(s) and q < len(sub):
+        if s[p] == sub[q]:
+            q += 1
+        p += 1
+    return q == len(sub)
+
+
+def assert_endpoint_name_compatible(sp_endpoint: ENDPOINT_TYPE, method: str, path: str) -> None:
+    """
+    限制endpoint函数名必须字面上包含method+path。
+    作用：1.避免无谓的思考;2.杜绝在endpoint上滥用修饰器。
+
+    :raise: NameError
+    """
+    method_path_slug = f'{method.lower()}_' + \
+        '_'.join(re.findall('[a-z0-9]+', path.lower()))
+    if not contains_sub_string(sp_endpoint.__name__,  method_path_slug):
+        raise NameError(
+            f'endpoint name "{sp_endpoint.__name__}" should contain "{method_path_slug}" to compatible with [{method} {path}]')
 
 
 def rest_mapping(method: str, paths: list) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
-        handler = make_router(sp_endpoint)
-        route = Route(method=method.upper(), paths=paths, handler=handler)
-        route.__doc__ = inspect.getdoc(sp_endpoint)
-        return route
+        assert_endpoint_name_compatible(sp_endpoint, method, '')
+        return make_router(method, paths, sp_endpoint)
 
     return g
 
 
 def get_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
+        assert_endpoint_name_compatible(sp_endpoint, 'GET', path)
         return rest_mapping(method='GET', paths=[path])(sp_endpoint)
 
     return g
 
 
 def post_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
+        assert_endpoint_name_compatible(sp_endpoint, 'POST', path)
         return rest_mapping(method='POST', paths=[path])(sp_endpoint)
 
     return g
 
 
 def put_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
+        assert_endpoint_name_compatible(sp_endpoint, 'PUT', path)
         return rest_mapping(method='PUT', paths=[path])(sp_endpoint)
 
     return g
 
 
 def patch_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
+        assert_endpoint_name_compatible(sp_endpoint, 'PATCH', path)
         return rest_mapping(method='PATCH', paths=[path])(sp_endpoint)
 
     return g
 
 
 def delete_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
+        assert_endpoint_name_compatible(sp_endpoint, 'DELETE', path)
         return rest_mapping(method='DELETE', paths=[path])(sp_endpoint)
 
     return g
 
 
 class Bridge:
     app: Application
     config: Optional[str]
 
-    def __init__(self, config: Optional[str] = None, app: Optional[Application] = None):
+    def __init__(self, config: Optional[str] = None, app: Optional[Application] = None) -> None:
         if app is None:
             self.app = Application()
         else:
             self.app = app
         self.config = config
         self._load_config()
+        self.app['lessweb.bridge'] = self
+        self.app['lessweb.routes'] = []
 
-    def _load_config(self):
-        self.app['bootstrap'] = self
+    def _load_config(self) -> None:
         self.app['config'] = self._load_config_with_env()
         self._load_logger()
         self._load_orjson()
 
-    def _load_config_with_env(self):
+    def _load_config_with_env(self) -> dict[str, Any]:
         if self.config:
             config = toml.loads(open(self.config).read())
         else:
             config = {}
         config.setdefault('bootstrap', {})
         dfs = [('', config)]  # list[(prefix, data)]
         while dfs:
@@ -367,15 +419,15 @@
                     dfs.append((key_path, value))
                 else:
                     env_key = make_environ_key(key_path)
                     if env_key in environ:
                         data[key] = environ[env_key]
         return config
 
-    def _load_logger(self):
+    def _load_logger(self) -> None:
         logger_conf = self.app['config'].get('logger', {})
         logger = logging.getLogger(logger_conf.get('name'))
         logger.setLevel(logger_conf.get('level', 'INFO'))
         stream_str = logger_conf.get('stream', 'stdout')
         formatter = None  # https://docs.python.org/zh-cn/3/library/logging.html#logrecord-attributes
         if logger_conf.get('format'):
             formatter = logging.Formatter(logger_conf['format'])
@@ -394,51 +446,52 @@
         else:
             stream = sys.stdout if stream_str == 'stdout' else sys.stderr
             stream_handler = logging.StreamHandler(stream)
             if formatter:
                 stream_handler.setFormatter(formatter)
             logger.addHandler(stream_handler)
 
-    def _load_orjson(self):
+    def _load_orjson(self) -> None:
         init_orjson_option(self.app['config']
                            ['bootstrap'].get('orjson_option', ''))
 
-    def add_middleware(self, handler):
+    def add_middleware(self, handler) -> None:
         self.app.middlewares.append(make_middleware(handler))
 
-    def add_on_startup(self, handler):
+    def add_on_startup(self, handler) -> None:
         self.app.on_startup.append(make_app_signal(handler))
 
-    def add_on_cleanup(self, handler):
+    def add_on_cleanup(self, handler) -> None:
         self.app.on_cleanup.append(make_app_signal(handler))
 
-    def add_mod_ctx(self, handler_on_startup, handler_on_cleanup):
+    def add_mod_ctx(self, handler_on_startup, handler_on_cleanup) -> None:
         async def aio_handler(app):
             await make_app_signal(handler_on_startup)(app)
             yield
             await make_app_signal(handler_on_cleanup)(app)
 
         self.app.cleanup_ctx.append(aio_handler)
 
-    def add_on_shutdown(self, handler):
+    def add_on_shutdown(self, handler) -> None:
         self.app.on_shutdown.append(make_app_signal(handler))
 
     def add_route(self, route: Route) -> None:
         for path in route.paths:
             self.app.router.add_route(
                 method=route.method, path=path, handler=route.handler)
+            self.app['lessweb.routes'].append(route)
 
-    def add_route_scan(self, endpoint_package: str):
+    def add_route_scan(self, endpoint_package: str) -> None:
         endpoint_mdl = importlib.import_module(endpoint_package)
         if endpoint_mdl.__spec__ is None or not endpoint_mdl.__spec__.submodule_search_locations:
             raise ImportError(f'{endpoint_package} is an empty package')
         for filename in listdir(endpoint_mdl.__spec__.submodule_search_locations[0]):
             if filename.endswith('.py'):
                 sub_mdl = importlib.import_module(
                     f'{endpoint_package}.{filename[:-3]}')
                 for item in sub_mdl.__dict__.values():
                     if isinstance(item, Route):
                         self.add_route(item)
 
-    def run_app(self, **kwargs):
+    def run_app(self, **kwargs) -> None:
         port = int(self.app['config']['bootstrap'].get('port', 8080))
         run_app(app=self.app, port=port, **kwargs)
```

### Comparing `lessweb-1.2.0/lessweb/typecast.py` & `lessweb-1.3.0/lessweb/typecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     """
     inspect_type(int) => (int,)
     inspect_type(list) => (list,)
     inspect_type(list[int]) => (list, int)
     inspect_type(int | None) => (Union, (int, NoneType))
     inspect_type(int | str) => (Union, (int, str))
     inspect_type(int | str | None) => (Union, (int, str, NoneType))
+    inspect_type(None | str | int) => (Union, (str, int, NoneType))
     inspect_type(Literal['a', 'b']) => (Literal, ('a', 'b'))
     inspect_type(NewType) => (NewType, __supertype__)
     inspect_type(dict) => (dict,)
     inspect_type(dict[str, int]) => NotImplementedError
     inspect_type(typeddict) => (dict, __annotations__)
     inspect_type(cls) => (cls,)
     inspect_type(_else_) => NotImplementedError
@@ -92,14 +93,54 @@
     raise NotImplementedError(f'cannot inspect type {tp=}')
 
 
 def is_list_type(tp):
     return tp is list or typing_inspect.get_origin(tp) is list
 
 
+def semi_json_schema_type(tp):
+    """
+    semi_json_schema_type(list) => {'type': 'array'}
+    semi_json_schema_type(list[int]) => {'type': 'array', 'items': {'type': int}}
+    semi_json_schema_type(Union[int, None]) => {'type': int, 'optional': True}
+    semi_json_schema_type(Union[int, str]) => {'union': [{'type': int}, {'type': str}], 'optional': False}
+    semi_json_schema_type(Union[None, int, str]) => {'union': [{'type': int}, {'type': str}], 'optional': True}
+    semi_json_schema_type(Literal['a', 'b']) => {'enum': ['a', 'b']}
+    semi_json_schema_type(Any) => {}
+    semi_json_schema_type(cls) => {'type': cls}
+    """
+    origin_type, *type_args_wrapped = inspect_type(tp)
+    if not type_args_wrapped:
+        if origin_type == list:
+            return {'type': 'array'}
+        elif origin_type == Any:
+            return {}
+        else:
+            return {'type': tp}
+    type_args = type_args_wrapped[0]
+    if origin_type == list:
+        return {'type': 'array', 'items': semi_json_schema_type(type_args)}
+    elif origin_type == Union:
+        if NoneType in type_args:
+            type_args_list = [
+                item for item in type_args if item is not NoneType]
+            is_optional = True
+        else:
+            type_args_list = list(type_args)
+            is_optional = False
+        if len(type_args_list) == 1:
+            return {**semi_json_schema_type(type_args_list[0]), 'optional': is_optional}
+        else:
+            return {'union': [semi_json_schema_type(item) for item in type_args_list], 'optional': is_optional}
+    elif origin_type == Literal:
+        return {'enum': list(type_args)}
+    else:
+        return {'type': tp}
+
+
 def typecast(data, tp):
     if isinstance_safe(tp, str):
         if tp not in classname_dict:
             raise TypeCastError(
                 f'typename {tp=} is not valid ref')  # 5xx Error in fact
         else:
             tp = classname_dict[tp]
```

### Comparing `lessweb-1.2.0/lessweb.egg-info/PKG-INFO` & `lessweb-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 Metadata-Version: 2.1
 Name: lessweb
-Version: 1.2.0
+Version: 1.3.0
 Summary: A pythonic web framework
 Author-email: qorzj <goodhorsezxj@gmail.com>
 License: Apache 2
 Keywords: lessweb,web,web.py,aiohttp
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp
 Requires-Dist: toml
 Requires-Dist: orjson
-Requires-Dist: lesscli
 Requires-Dist: typing_inspect
+Provides-Extra: test
+Requires-Dist: autopep8; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-aiohttp; extra == "test"
+Requires-Dist: types-toml; extra == "test"
 
 # lessweb
 >「嘞是web」
 
 Lessweb is an extremely easy-to-use python web framework with the following goals.
 
 * Simple and efficient: based on the aiohttp library IOC capabilities, native support for configuration loading and logging settings to meet production-level development requirements
```

### Comparing `lessweb-1.2.0/lessweb.egg-info/SOURCES.txt` & `lessweb-1.3.0/lessweb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,12 @@
 lessweb/py.typed
 lessweb/typecast.py
 lessweb.egg-info/PKG-INFO
 lessweb.egg-info/SOURCES.txt
 lessweb.egg-info/dependency_links.txt
 lessweb.egg-info/requires.txt
 lessweb.egg-info/top_level.txt
-requirements/base.txt
-requirements/test.txt
 tests/__init__.py
-tests/test_typecast.py
+tests/test_bridge.py
+tests/test_typecast.py
+tests/e2e/__init__.py
+tests/e2e/test_request_stack.py
```

### Comparing `lessweb-1.2.0/pyproject.toml` & `lessweb-1.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lessweb"
-version = "1.2.0"
+version = "1.3.0"
 description = 'A pythonic web framework'
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ['lessweb', 'web', 'web.py', 'aiohttp']
 authors = [
     {name = "qorzj", email = "goodhorsezxj@gmail.com"},
 ]
 license = {text = "Apache 2"}
 dependencies = [
     "aiohttp",
     "toml",
     "orjson",
-    "lesscli",
     "typing_inspect",
 ]
 
+[project.optional-dependencies]
+test = [
+    "autopep8",
+    "mypy",
+    "coverage",
+    "pytest",
+    "pytest-cov",
+    "pytest-mock",
+    "pytest-asyncio",
+    "pytest-aiohttp",
+    "types-toml",
+]
+
 [tool.setuptools.package-data]
 "lessweb" = ["py.typed"]
```

### Comparing `lessweb-1.2.0/tests/test_typecast.py` & `lessweb-1.3.0/tests/test_typecast.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys
 import unittest
 from datetime import date, datetime, time
 from enum import Enum
-from typing import (Dict, Generator, List, Literal, NewType, Optional,
+from typing import (Any, Dict, Generator, List, Literal, NewType, Optional,
                     TypedDict, Union)
 
-from lessweb.typecast import TypeCastError, inspect_type, typecast
+from lessweb.typecast import (TypeCastError, inspect_type,
+                              semi_json_schema_type, typecast)
 
 NoneType = type(None)
 
 
 class SampleTypedDict(TypedDict):
     name: str
     age: int
@@ -30,23 +31,26 @@
         self.assertEqual(inspect_type(Optional[int]), (Union, (int, NoneType)))
         if sys.version_info[:2] >= (3, 11):
             self.assertEqual(inspect_type(int | None),
                              (Union, (int, NoneType)))
             self.assertEqual(inspect_type(int | str), (Union, (int, str)))
             self.assertEqual(inspect_type(int | str | None),
                              (Union, (int, str, NoneType)))
+            self.assertEqual(inspect_type(None | str | int),
+                             (Union, (NoneType, str, int)))
         self.assertEqual(inspect_type(
             Literal['a', 'b']), (Literal, ('a', 'b')))
         self.assertEqual(inspect_type(UserId), (NewType, int))
         self.assertEqual(inspect_type(dict), (dict,))
         self.assertRaises(NotImplementedError, inspect_type, dict[str, int])
         self.assertRaises(NotImplementedError, inspect_type,
                           Dict[str, Union[str, int]])
         self.assertEqual(inspect_type(SampleTypedDict),
                          (dict, {'age': int, 'name': str}))
+        self.assertEqual(inspect_type(Any), (Any,))
         self.assertEqual(inspect_type(SampleElse), (SampleElse,))
         self.assertRaises(NotImplementedError, inspect_type, Generator)
 
 
 class SampleEnum(Enum):
     VALUE1 = 'V1'
     VALUE2 = 'V2'
@@ -143,9 +147,42 @@
         result = typecast(data, tp)
         self.assertEqual(result, UserId(10))
         data = "12.3"
         with self.assertRaises(TypeCastError):
             typecast(data, tp)
 
 
+class TestSemiJsonSchemaType(unittest.TestCase):
+    def test_list(self):
+        result = semi_json_schema_type(list)
+        self.assertEqual(result, {'type': 'array'})
+
+        result = semi_json_schema_type(list[int])
+        self.assertEqual(result, {'type': 'array', 'items': {'type': int}})
+
+    def test_union(self):
+        result = semi_json_schema_type(Union[int, str])
+        self.assertEqual(
+            result, {'union': [{'type': int}, {'type': str}], 'optional': False})
+
+        result = semi_json_schema_type(Union[int, None])
+        self.assertEqual(result, {'type': int, 'optional': True})
+
+        result = semi_json_schema_type(Union[None, int, str])
+        self.assertEqual(
+            result, {'union': [{'type': int}, {'type': str}], 'optional': True})
+
+    def test_literal(self):
+        result = semi_json_schema_type(Literal['a', 'b'])
+        self.assertEqual(result, {'enum': ['a', 'b']})
+
+    def test_any(self):
+        result = semi_json_schema_type(Any)
+        self.assertEqual(result, {})
+
+    def test_custom_class(self):
+        result = semi_json_schema_type(SampleElse)
+        self.assertEqual(result, {'type': SampleElse})
+
+
 if __name__ == '__main__':
     unittest.main()
```

