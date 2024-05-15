# Comparing `tmp/pypi_browser_webapp-0.0.7.tar.gz` & `tmp/pypi_browser_webapp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_browser_webapp-0.0.7.tar", max compression
+gzip compressed data, was "pypi_browser_webapp-0.0.8.tar", max compression
```

## Comparing `pypi_browser_webapp-0.0.7.tar` & `pypi_browser_webapp-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2722 2022-09-19 17:14:49.153055 pypi_browser_webapp-0.0.7/README.md
--rw-r--r--   0        0        0        0 2022-09-14 17:58:04.594576 pypi_browser_webapp-0.0.7/pypi_browser/__init__.py
--rw-r--r--   0        0        0    13037 2023-11-29 04:39:04.780847 pypi_browser_webapp-0.0.7/pypi_browser/app.py
--rw-r--r--   0        0        0     4501 2023-11-29 04:57:06.880417 pypi_browser_webapp-0.0.7/pypi_browser/packaging.py
--rw-r--r--   0        0        0     3397 2022-09-22 03:18:39.564609 pypi_browser_webapp-0.0.7/pypi_browser/pypi.py
--rw-r--r--   0        0        0   195498 2022-09-15 18:36:16.351200 pypi_browser_webapp-0.0.7/pypi_browser/static/bootstrap-5.2.1.min.css
--rw-r--r--   0        0        0    80457 2022-09-15 18:36:16.351200 pypi_browser_webapp-0.0.7/pypi_browser/static/bootstrap-5.2.1.min.js
--rw-r--r--   0        0        0     1584 2022-09-15 23:36:06.000000 pypi_browser_webapp-0.0.7/pypi_browser/static/favicon.png
--rw-r--r--   0        0        0      380 2022-09-15 22:08:28.471295 pypi_browser_webapp-0.0.7/pypi_browser/static/site.css
--rw-r--r--   0        0        0       78 2022-09-15 18:30:23.657727 pypi_browser_webapp-0.0.7/pypi_browser/static/site.js
--rw-r--r--   0        0        0     2293 2022-09-19 17:28:01.240392 pypi_browser_webapp-0.0.7/pypi_browser/templates/_base.html
--rw-r--r--   0        0        0      743 2022-09-16 22:22:19.084897 pypi_browser_webapp-0.0.7/pypi_browser/templates/_macros.html
--rw-r--r--   0        0        0     1389 2022-09-19 17:19:48.788264 pypi_browser_webapp-0.0.7/pypi_browser/templates/home.html
--rw-r--r--   0        0        0     1397 2022-09-15 21:57:27.577224 pypi_browser_webapp-0.0.7/pypi_browser/templates/package.html
--rw-r--r--   0        0        0     2495 2022-09-16 22:22:37.924601 pypi_browser_webapp-0.0.7/pypi_browser/templates/package_file.html
--rw-r--r--   0        0        0     2434 2022-09-19 17:34:55.073994 pypi_browser_webapp-0.0.7/pypi_browser/templates/package_file_archive_path.html
--rw-r--r--   0        0        0      950 2023-11-29 04:57:37.044282 pypi_browser_webapp-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 pypi_browser_webapp-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2722 2024-05-15 15:56:44.626790 pypi_browser_webapp-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 15:56:44.627604 pypi_browser_webapp-0.0.8/pypi_browser/__init__.py
+-rw-r--r--   0        0        0    13223 2024-05-15 16:06:29.200394 pypi_browser_webapp-0.0.8/pypi_browser/app.py
+-rw-r--r--   0        0        0     4493 2024-05-15 16:12:10.130971 pypi_browser_webapp-0.0.8/pypi_browser/packaging.py
+-rw-r--r--   0        0        0     3397 2024-05-15 15:56:44.628229 pypi_browser_webapp-0.0.8/pypi_browser/pypi.py
+-rw-r--r--   0        0        0   195498 2024-05-15 15:56:44.628752 pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.css
+-rw-r--r--   0        0        0    80457 2024-05-15 15:56:44.629169 pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.js
+-rw-r--r--   0        0        0     1584 2024-05-15 15:56:44.629315 pypi_browser_webapp-0.0.8/pypi_browser/static/favicon.png
+-rw-r--r--   0        0        0      380 2024-05-15 15:56:44.629430 pypi_browser_webapp-0.0.8/pypi_browser/static/site.css
+-rw-r--r--   0        0        0       78 2024-05-15 15:56:44.629535 pypi_browser_webapp-0.0.8/pypi_browser/static/site.js
+-rw-r--r--   0        0        0     2293 2024-05-15 15:56:44.629718 pypi_browser_webapp-0.0.8/pypi_browser/templates/_base.html
+-rw-r--r--   0        0        0      743 2024-05-15 15:56:44.629842 pypi_browser_webapp-0.0.8/pypi_browser/templates/_macros.html
+-rw-r--r--   0        0        0     1389 2024-05-15 15:56:44.629967 pypi_browser_webapp-0.0.8/pypi_browser/templates/home.html
+-rw-r--r--   0        0        0     1397 2024-05-15 15:56:44.630129 pypi_browser_webapp-0.0.8/pypi_browser/templates/package.html
+-rw-r--r--   0        0        0     2495 2024-05-15 15:56:44.630297 pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file.html
+-rw-r--r--   0        0        0     2434 2024-05-15 15:56:44.630465 pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file_archive_path.html
+-rw-r--r--   0        0        0      869 2024-05-15 16:12:42.720743 pypi_browser_webapp-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 pypi_browser_webapp-0.0.8/PKG-INFO
```

### Comparing `pypi_browser_webapp-0.0.7/README.md` & `pypi_browser_webapp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/app.py` & `pypi_browser_webapp-0.0.8/pypi_browser/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from starlette.middleware import Middleware
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 from starlette.responses import RedirectResponse
 from starlette.responses import Response
 from starlette.responses import StreamingResponse
+from starlette.routing import Route
 from starlette.staticfiles import StaticFiles
 from starlette.templating import Jinja2Templates
 
 import pypi_browser.packaging
 from pypi_browser import pypi
 from pypi_browser.packaging import PackageFormat
 
@@ -74,22 +75,14 @@
 
 config = starlette.config.Config()
 pypi_config = pypi.PyPIConfig(
     cache_path=config('PYPI_BROWSER_PACKAGE_CACHE_PATH', default='/tmp'),
     pypi_url=config('PYPI_BROWSER_PYPI_URL', default='https://pypi.org'),
 )
 
-app = Starlette(
-    debug=os.environ.get('PYPI_BROWSER_DEBUG') == '1',
-    middleware=[
-        Middleware(CacheControlHeaderMiddleware),
-    ],
-)
-app.mount('/static', StaticFiles(directory=os.path.join(install_root, 'static')), name='static')
-
 templates = Jinja2Templates(
     directory=os.path.join(install_root, 'templates'),
 )
 
 
 def _pluralize(n: int) -> str:
     return '' if n == 1 else 's'
@@ -107,20 +100,18 @@
 
 
 templates.env.filters['human_size'] = _human_size
 templates.env.filters['pluralize'] = _pluralize
 templates.env.globals['pypi_browser_version'] = importlib.metadata.version('pypi-browser-webapp')
 
 
-@app.route('/')
 async def home(request: Request) -> Response:
     return templates.TemplateResponse('home.html', {'request': request})
 
 
-@app.route('/package/{package}')
 async def package(request: Request) -> Response:
     package_name = request.path_params['package']
     normalized_package_name = pypi_browser.packaging.pep426_normalize(package_name)
     if package_name != normalized_package_name:
         return RedirectResponse(request.url_for('package', package=normalized_package_name))
 
     try:
@@ -143,15 +134,14 @@
                 'package': package_name,
                 'version_to_files': version_to_files_sorted,
                 'total_files': len(set(itertools.chain.from_iterable(version_to_files.values()))),
             },
         )
 
 
-@app.route('/package/{package}/{filename}')
 async def package_file(request: Request) -> Response:
     package_name = request.path_params['package']
     file_name = request.path_params['filename']
 
     normalized_package_name = pypi_browser.packaging.pep426_normalize(package_name)
     if package_name != normalized_package_name:
         return RedirectResponse(
@@ -216,15 +206,14 @@
             'entries': entries,
             'metadata_path': metadata_path,
             'metadata': metadata,
         },
     )
 
 
-@app.route('/package/{package}/{filename}/{archive_path:path}')
 async def package_file_archive_path(request: Request) -> Response:
     package_name = request.path_params['package']
     file_name = request.path_params['filename']
     archive_path = request.path_params['archive_path']
 
     normalized_package_name = pypi_browser.packaging.pep426_normalize(package_name)
     if package_name != normalized_package_name:
@@ -371,10 +360,25 @@
             'archive_path': archive_path,
             'metadata': metadata,
             'cannot_render_error': 'This file appears to be a binary.',
         },
     )
 
 
-@app.route('/search')
 async def search(request: Request) -> Response:
     return RedirectResponse(request.url_for('package', package=request.query_params['package']))
+
+
+app = Starlette(
+    debug=os.environ.get('PYPI_BROWSER_DEBUG') == '1',
+    middleware=[
+        Middleware(CacheControlHeaderMiddleware),
+    ],
+    routes=[
+        Route('/', endpoint=home),
+        Route('/package/{package}', endpoint=package),
+        Route('/package/{package}/{filename}', endpoint=package_file),
+        Route('/package/{package}/{filename}/{archive_path:path}', endpoint=package_file_archive_path),
+        Route('/search', endpoint=search),
+    ],
+)
+app.mount('/static', StaticFiles(directory=os.path.join(install_root, 'static')), name='static')
```

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/packaging.py` & `pypi_browser_webapp-0.0.8/pypi_browser/packaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typing
 import zipfile
 from dataclasses import dataclass
 from types import TracebackType
 
 
 def pep426_normalize(package_name: str) -> str:
-    return re.sub(r'[-_.]+', '-', package_name).lower()
+    return re.sub(r'[-_.]+', '-', package_name.strip()).lower()
 
 
 class UnsupportedPackageType(Exception):
     pass
 
 
 class PackageType(enum.Enum):
@@ -124,15 +124,15 @@
             return await asyncio.to_thread(_package_entries_from_tarball, self.path)
         else:
             raise AssertionError(self.package_format)
 
     @contextlib.asynccontextmanager
     async def open_from_archive(self, path: str) -> typing.AsyncIterator[AsyncArchiveFile]:
         if self.package_format is PackageFormat.ZIPFILE:
-            zf = await asyncio.to_thread(zipfile.ZipFile, self.path)  # type: ignore
+            zf = await asyncio.to_thread(zipfile.ZipFile, self.path)
             try:
                 zip_archive_file = await asyncio.to_thread(zf.open, path)
                 async with AsyncArchiveFile(zip_archive_file) as wrapped:
                     yield wrapped
             finally:
                 await asyncio.to_thread(zf.close)
         elif self.package_format is PackageFormat.TARBALL:
```

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/pypi.py` & `pypi_browser_webapp-0.0.8/pypi_browser/pypi.py`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/static/bootstrap-5.2.1.min.css` & `pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.css`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/static/bootstrap-5.2.1.min.js` & `pypi_browser_webapp-0.0.8/pypi_browser/static/bootstrap-5.2.1.min.js`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/static/favicon.png` & `pypi_browser_webapp-0.0.8/pypi_browser/static/favicon.png`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/templates/_base.html` & `pypi_browser_webapp-0.0.8/pypi_browser/templates/_base.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/templates/_macros.html` & `pypi_browser_webapp-0.0.8/pypi_browser/templates/_macros.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/templates/home.html` & `pypi_browser_webapp-0.0.8/pypi_browser/templates/home.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/templates/package.html` & `pypi_browser_webapp-0.0.8/pypi_browser/templates/package.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/templates/package_file.html` & `pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pypi_browser/templates/package_file_archive_path.html` & `pypi_browser_webapp-0.0.8/pypi_browser/templates/package_file_archive_path.html`

 * *Files identical despite different names*

### Comparing `pypi_browser_webapp-0.0.7/pyproject.toml` & `pypi_browser_webapp-0.0.8/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "pypi-browser-webapp"
-version = "0.0.7"
+version = "0.0.8"
 description = "PyPI package browsing web application"
 authors = ["Chris Kuehl <ckuehl@ckuehl.me>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "pypi_browser"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 starlette = "*"
-fluffy-code = "^0.0.2"
-Jinja2 = "^3.1.2"
-httpx = "^0.23.0"
-aiofiles = "^22.1.0"
-identify = "^2.5.5"
-Pygments = "^2.13.0"
-MarkupSafe = "^2.1.1"
-packaging = "^21.3"
+fluffy-code = "*"
+Jinja2 = "*"
+httpx = "*"
+aiofiles = "*"
+identify = "*"
+Pygments = "*"
+MarkupSafe = "*"
+packaging = "*"
 
 
 [tool.poetry.group.dev.dependencies]
-uvicorn = "^0.18.3"
-pre-commit = "^2.20.0"
-pytest = "^7.1.3"
-mypy = "^0.971"
-coverage = "^6.4.4"
-types-aiofiles = "^22.1.0"
-types-Pygments = "^2.13.0"
+uvicorn = "*"
+pre-commit = "*"
+pytest = "*"
+mypy = "*"
+coverage = "*"
+types-aiofiles = "*"
+types-Pygments = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [mypy]
 check_untyped_defs = true
```

### Comparing `pypi_browser_webapp-0.0.7/PKG-INFO` & `pypi_browser_webapp-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pypi-browser-webapp
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI package browsing web application
 License: Apache-2.0
 Author: Chris Kuehl
 Author-email: ckuehl@ckuehl.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: MarkupSafe (>=2.1.1,<3.0.0)
-Requires-Dist: Pygments (>=2.13.0,<3.0.0)
-Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
-Requires-Dist: fluffy-code (>=0.0.2,<0.0.3)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: identify (>=2.5.5,<3.0.0)
-Requires-Dist: packaging (>=21.3,<22.0)
+Requires-Dist: Jinja2
+Requires-Dist: MarkupSafe
+Requires-Dist: Pygments
+Requires-Dist: aiofiles
+Requires-Dist: fluffy-code
+Requires-Dist: httpx
+Requires-Dist: identify
+Requires-Dist: packaging
 Requires-Dist: starlette
 Description-Content-Type: text/markdown
 
 PyPI Browser
 ============
 
 **PyPI Browser** is a web application for browsing the contents of packages on
```

