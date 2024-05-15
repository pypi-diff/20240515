# Comparing `tmp/http_uploader_cli-0.1.0.tar.gz` & `tmp/http_uploader_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_uploader_cli-0.1.0.tar", max compression
+gzip compressed data, was "http_uploader_cli-0.1.1.tar", max compression
```

## Comparing `http_uploader_cli-0.1.0.tar` & `http_uploader_cli-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      157 2024-05-15 19:48:12.119711 http_uploader_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-14 14:24:59.626808 http_uploader_cli-0.1.0/http_uploader/__init__.py
--rw-r--r--   0        0        0      808 2024-05-15 19:14:10.429257 http_uploader_cli-0.1.0/http_uploader/__main__.py
--rw-r--r--   0        0        0        0 2024-05-15 01:19:07.532409 http_uploader_cli-0.1.0/http_uploader/cli/__init__.py
--rw-r--r--   0        0        0      133 2024-05-15 18:29:20.585359 http_uploader_cli-0.1.0/http_uploader/cli/engine/__init__.py
--rw-r--r--   0        0        0      167 2024-05-15 18:27:39.210674 http_uploader_cli-0.1.0/http_uploader/cli/engine/common.py
--rw-r--r--   0        0        0        0 2024-05-15 02:56:37.081111 http_uploader_cli-0.1.0/http_uploader/cli/engine/dto/__init__.py
--rw-r--r--   0        0        0       62 2024-05-15 18:27:52.854638 http_uploader_cli-0.1.0/http_uploader/cli/engine/dto/args/__init__.py
--rw-r--r--   0        0        0      223 2024-05-15 18:27:06.039141 http_uploader_cli-0.1.0/http_uploader/cli/engine/dto/args/common.py
--rw-r--r--   0        0        0       60 2024-05-15 03:03:35.236855 http_uploader_cli-0.1.0/http_uploader/cli/engine/dto/response/__init__.py
--rw-r--r--   0        0        0      127 2024-05-15 18:00:46.836071 http_uploader_cli-0.1.0/http_uploader/cli/engine/dto/response/common.py
--rw-r--r--   0        0        0     1663 2024-05-15 19:15:35.236484 http_uploader_cli-0.1.0/http_uploader/cli/engine/http_uploader.py
--rw-r--r--   0        0        0        0 2024-05-15 03:03:20.402845 http_uploader_cli-0.1.0/http_uploader/facade/__init__.py
--rw-r--r--   0        0        0      169 2024-05-15 03:04:00.654680 http_uploader_cli-0.1.0/http_uploader/facade/common.py
--rw-r--r--   0        0        0     4155 2024-05-15 19:36:46.384857 http_uploader_cli-0.1.0/http_uploader/facade/http_uploader.py
--rw-r--r--   0        0        0      356 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.0/http_uploader/facade/proxy.py
--rw-r--r--   0        0        0       92 2024-05-15 03:12:56.629106 http_uploader_cli-0.1.0/http_uploader/finder/__init__.py
--rw-r--r--   0        0        0      161 2024-05-15 18:44:31.720768 http_uploader_cli-0.1.0/http_uploader/finder/common.py
--rw-r--r--   0        0        0     1168 2024-05-15 18:45:32.296898 http_uploader_cli-0.1.0/http_uploader/finder/json.py
--rw-r--r--   0        0        0      108 2024-05-15 03:09:45.380393 http_uploader_cli-0.1.0/http_uploader/http/__init__.py
--rw-r--r--   0        0        0      197 2024-05-14 18:10:43.034518 http_uploader_cli-0.1.0/http_uploader/http/common.py
--rw-r--r--   0        0        0        0 2024-05-14 18:09:03.656460 http_uploader_cli-0.1.0/http_uploader/http/dto/__init__.py
--rw-r--r--   0        0        0      322 2024-05-15 18:15:43.114231 http_uploader_cli-0.1.0/http_uploader/http/dto/client_request.py
--rw-r--r--   0        0        0      110 2024-05-14 18:10:25.287008 http_uploader_cli-0.1.0/http_uploader/http/dto/response.py
--rw-r--r--   0        0        0      703 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.0/http_uploader/http/post.py
--rw-r--r--   0        0        0        0 2024-05-14 15:11:39.866758 http_uploader_cli-0.1.0/http_uploader/utils/__init__.py
--rw-r--r--   0        0        0       97 2024-05-15 03:07:48.478399 http_uploader_cli-0.1.0/http_uploader/utils/file/__init__.py
--rw-r--r--   0        0        0      304 2024-05-15 18:20:54.025277 http_uploader_cli-0.1.0/http_uploader/utils/file/common.py
--rw-r--r--   0        0        0     1216 2024-05-15 19:25:06.249374 http_uploader_cli-0.1.0/http_uploader/utils/file/txt.py
--rw-r--r--   0        0        0      263 2024-05-15 18:48:33.058576 http_uploader_cli-0.1.0/http_uploader/utils/filter/__init__.py
--rw-r--r--   0        0        0      172 2024-05-15 02:43:18.401218 http_uploader_cli-0.1.0/http_uploader/utils/filter/common.py
--rw-r--r--   0        0        0      603 2024-05-15 02:37:58.119623 http_uploader_cli-0.1.0/http_uploader/utils/filter/compare.py
--rw-r--r--   0        0        0     1057 2024-05-15 02:37:59.573025 http_uploader_cli-0.1.0/http_uploader/utils/filter/extented_compare.py
--rw-r--r--   0        0        0      307 2024-05-15 19:38:01.824988 http_uploader_cli-0.1.0/http_uploader/utils/parts.py
--rw-r--r--   0        0        0     1505 2024-05-15 19:06:48.455623 http_uploader_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 http_uploader_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      157 2024-05-15 19:48:12.119711 http_uploader_cli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 14:24:59.626808 http_uploader_cli-0.1.1/http_uploader/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-15 19:14:10.429257 http_uploader_cli-0.1.1/http_uploader/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:19:07.532409 http_uploader_cli-0.1.1/http_uploader/cli/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-15 18:29:20.585359 http_uploader_cli-0.1.1/http_uploader/cli/engine/__init__.py
+-rw-r--r--   0        0        0      167 2024-05-15 18:27:39.210674 http_uploader_cli-0.1.1/http_uploader/cli/engine/common.py
+-rw-r--r--   0        0        0        0 2024-05-15 02:56:37.081111 http_uploader_cli-0.1.1/http_uploader/cli/engine/dto/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-15 18:27:52.854638 http_uploader_cli-0.1.1/http_uploader/cli/engine/dto/args/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-15 18:27:06.039141 http_uploader_cli-0.1.1/http_uploader/cli/engine/dto/args/common.py
+-rw-r--r--   0        0        0       60 2024-05-15 03:03:35.236855 http_uploader_cli-0.1.1/http_uploader/cli/engine/dto/response/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-15 18:00:46.836071 http_uploader_cli-0.1.1/http_uploader/cli/engine/dto/response/common.py
+-rw-r--r--   0        0        0     1663 2024-05-15 19:15:35.236484 http_uploader_cli-0.1.1/http_uploader/cli/engine/http_uploader.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:03:20.402845 http_uploader_cli-0.1.1/http_uploader/facade/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-15 03:04:00.654680 http_uploader_cli-0.1.1/http_uploader/facade/common.py
+-rw-r--r--   0        0        0     4155 2024-05-15 19:36:46.384857 http_uploader_cli-0.1.1/http_uploader/facade/http_uploader.py
+-rw-r--r--   0        0        0      356 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.1/http_uploader/facade/proxy.py
+-rw-r--r--   0        0        0       92 2024-05-15 03:12:56.629106 http_uploader_cli-0.1.1/http_uploader/finder/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-15 18:44:31.720768 http_uploader_cli-0.1.1/http_uploader/finder/common.py
+-rw-r--r--   0        0        0     1168 2024-05-15 18:45:32.296898 http_uploader_cli-0.1.1/http_uploader/finder/json.py
+-rw-r--r--   0        0        0      108 2024-05-15 03:09:45.380393 http_uploader_cli-0.1.1/http_uploader/http/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-14 18:10:43.034518 http_uploader_cli-0.1.1/http_uploader/http/common.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:09:03.656460 http_uploader_cli-0.1.1/http_uploader/http/dto/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-15 18:15:43.114231 http_uploader_cli-0.1.1/http_uploader/http/dto/client_request.py
+-rw-r--r--   0        0        0      110 2024-05-14 18:10:25.287008 http_uploader_cli-0.1.1/http_uploader/http/dto/response.py
+-rw-r--r--   0        0        0      703 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.1/http_uploader/http/post.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:11:39.866758 http_uploader_cli-0.1.1/http_uploader/utils/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-15 03:07:48.478399 http_uploader_cli-0.1.1/http_uploader/utils/file/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-15 18:20:54.025277 http_uploader_cli-0.1.1/http_uploader/utils/file/common.py
+-rw-r--r--   0        0        0     1216 2024-05-15 19:25:06.249374 http_uploader_cli-0.1.1/http_uploader/utils/file/txt.py
+-rw-r--r--   0        0        0      263 2024-05-15 18:48:33.058576 http_uploader_cli-0.1.1/http_uploader/utils/filter/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-15 02:43:18.401218 http_uploader_cli-0.1.1/http_uploader/utils/filter/common.py
+-rw-r--r--   0        0        0      603 2024-05-15 02:37:58.119623 http_uploader_cli-0.1.1/http_uploader/utils/filter/compare.py
+-rw-r--r--   0        0        0     1057 2024-05-15 02:37:59.573025 http_uploader_cli-0.1.1/http_uploader/utils/filter/extented_compare.py
+-rw-r--r--   0        0        0      307 2024-05-15 19:38:01.824988 http_uploader_cli-0.1.1/http_uploader/utils/parts.py
+-rw-r--r--   0        0        0     1524 2024-05-15 20:11:44.884781 http_uploader_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 http_uploader_cli-0.1.1/PKG-INFO
```

### Comparing `http_uploader_cli-0.1.0/http_uploader/__main__.py` & `http_uploader_cli-0.1.1/http_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/http_uploader/cli/engine/http_uploader.py` & `http_uploader_cli-0.1.1/http_uploader/cli/engine/http_uploader.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/http_uploader/facade/http_uploader.py` & `http_uploader_cli-0.1.1/http_uploader/facade/http_uploader.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/http_uploader/finder/json.py` & `http_uploader_cli-0.1.1/http_uploader/finder/json.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/http_uploader/http/post.py` & `http_uploader_cli-0.1.1/http_uploader/http/post.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/http_uploader/utils/file/txt.py` & `http_uploader_cli-0.1.1/http_uploader/utils/file/txt.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/http_uploader/utils/filter/compare.py` & `http_uploader_cli-0.1.1/http_uploader/utils/filter/compare.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/http_uploader/utils/filter/extented_compare.py` & `http_uploader_cli-0.1.1/http_uploader/utils/filter/extented_compare.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.0/pyproject.toml` & `http_uploader_cli-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "http-uploader-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = "Simple HTTP CLI json data uploader"
 repository = "https://github.com/rafailmdzdv/http-uploader-cli"
 authors = ["rafailmdzdv <rafayt323@xmail.ru>"]
 readme = "README.md"
 packages = [ {include = "http_uploader"} ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
+aiohttp = "^3.9.5"
 aiofiles = "^23.2.1"
 aiomultiprocess = "^0.9.1"
 prettytable = "^3.10.0"
 
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.4.4"
```

### Comparing `http_uploader_cli-0.1.0/PKG-INFO` & `http_uploader_cli-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: http-uploader-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple HTTP CLI json data uploader
 Home-page: https://github.com/rafailmdzdv/http-uploader-cli
 Author: rafailmdzdv
 Author-email: rafayt323@xmail.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: aiomultiprocess (>=0.9.1,<0.10.0)
 Requires-Dist: prettytable (>=3.10.0,<4.0.0)
 Project-URL: Repository, https://github.com/rafailmdzdv/http-uploader-cli
 Description-Content-Type: text/markdown
 
 ### Http Uploader CLI
```

