# Comparing `tmp/pywebframework_uz-0.1.1.tar.gz` & `tmp/pywebframework_uz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebframework_uz-0.1.1.tar", last modified: Wed May 15 09:13:40 2024, max compression
+gzip compressed data, was "pywebframework_uz-0.1.2.tar", last modified: Wed May 15 09:16:33 2024, max compression
```

## Comparing `pywebframework_uz-0.1.1.tar` & `pywebframework_uz-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:13:40.925589 pywebframework_uz-0.1.1/
--rw-rw-rw-   0        0        0     4750 2024-05-15 09:13:40.924159 pywebframework_uz-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3878 2024-05-15 09:05:04.000000 pywebframework_uz-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 09:13:40.921163 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/
--rw-rw-rw-   0        0        0     4750 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:13:40.000000 pywebframework_uz-0.1.1/pywebframework_uz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 09:13:40.925902 pywebframework_uz-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     4069 2024-05-15 09:13:12.000000 pywebframework_uz-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:16:33.166936 pywebframework_uz-0.1.2/
+-rw-rw-rw-   0        0        0     4736 2024-05-15 09:16:33.165935 pywebframework_uz-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3864 2024-05-15 09:16:20.000000 pywebframework_uz-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:16:33.162946 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/
+-rw-rw-rw-   0        0        0     4736 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:16:33.000000 pywebframework_uz-0.1.2/pywebframework_uz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:16:33.166936 pywebframework_uz-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     4069 2024-05-15 09:16:20.000000 pywebframework_uz-0.1.2/setup.py
```

### Comparing `pywebframework_uz-0.1.1/PKG-INFO` & `pywebframework_uz-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebframework_uz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python web-framework building for learning purpose
 Home-page: https://github.com/me/myproject
 Author: Madaminov Khojiakbar
 Author-email: hojiakbarmadaminov45@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -18,28 +18,28 @@
 Requires-Dist: parse==1.20.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
 
 
-#PY-WEB-FRAMEWORK is a Python web framework build for purposes
+PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
 ![purpose](https://image.shields.io/badge/purpose-learning-green)
 ![PyPy - Version](https://image.shields.io/pypi/v/pywebframework)
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
-##Installation
+Installation
 ```shell
 pip install pywebframework-uz
 ```
 
-###Basic usage
+Basic usage
 
 ```python
 
 from app import PyFrameBuilding
 from middleware import CustomMiddleware
 
 server = PyFrameBuilding()
@@ -109,15 +109,15 @@
 
 
 server.add_middleware(SimpleMiddleware)
 
 
 ```
 
-###Unit Tests
+Unit Tests
 The recommended way of writing unit tests is with pytest. There are two built in fixtures that you may want to use when writing unit tests with PYWEBFRAMEWORK.
 The first one is app which is an instance of the main API class:
 
 ```python
 
 def test_basic_route_adding(app):
     @app.route('/home')
@@ -144,15 +144,15 @@
 
     app.add_route('/new-handler', new_handler)
 
     assert test_client.get('http://testserver/new-handler').text == 'From new handler'
 
 ```
 
-###TEMPLATES
+TEMPLATES
 
 The default folder for templates is 'template'. You can change it when
 initializing the  'PyFrameBuilding' class.
 
 ```python
 @server.route('/template')
 def template_handler(request, response):
@@ -161,15 +161,15 @@
             "new_title": 'New Title',
             "new_body": f"Hello 1243"
         }
     )
 ```
 
 
-##Static files
+Static files
 Just like templates, the default folder for static files is static and you can override it:
 server = PyFrameBuilding(static_dir='path/to/static/files/)
 ```html
 <html>
     <header>
         <title>{{new_title}}</title>
```

### Comparing `pywebframework_uz-0.1.1/README.md` & `pywebframework_uz-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#PY-WEB-FRAMEWORK is a Python web framework build for purposes
+PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
 ![purpose](https://image.shields.io/badge/purpose-learning-green)
 ![PyPy - Version](https://image.shields.io/pypi/v/pywebframework)
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
-##Installation
+Installation
 ```shell
 pip install pywebframework-uz
 ```
 
-###Basic usage
+Basic usage
 
 ```python
 
 from app import PyFrameBuilding
 from middleware import CustomMiddleware
 
 server = PyFrameBuilding()
@@ -85,15 +85,15 @@
 
 
 server.add_middleware(SimpleMiddleware)
 
 
 ```
 
-###Unit Tests
+Unit Tests
 The recommended way of writing unit tests is with pytest. There are two built in fixtures that you may want to use when writing unit tests with PYWEBFRAMEWORK.
 The first one is app which is an instance of the main API class:
 
 ```python
 
 def test_basic_route_adding(app):
     @app.route('/home')
@@ -120,15 +120,15 @@
 
     app.add_route('/new-handler', new_handler)
 
     assert test_client.get('http://testserver/new-handler').text == 'From new handler'
 
 ```
 
-###TEMPLATES
+TEMPLATES
 
 The default folder for templates is 'template'. You can change it when
 initializing the  'PyFrameBuilding' class.
 
 ```python
 @server.route('/template')
 def template_handler(request, response):
@@ -137,15 +137,15 @@
             "new_title": 'New Title',
             "new_body": f"Hello 1243"
         }
     )
 ```
 
 
-##Static files
+Static files
 Just like templates, the default folder for static files is static and you can override it:
 server = PyFrameBuilding(static_dir='path/to/static/files/)
 ```html
 <html>
     <header>
         <title>{{new_title}}</title>
```

### Comparing `pywebframework_uz-0.1.1/pywebframework_uz.egg-info/PKG-INFO` & `pywebframework_uz-0.1.2/pywebframework_uz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebframework_uz
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python web-framework building for learning purpose
 Home-page: https://github.com/me/myproject
 Author: Madaminov Khojiakbar
 Author-email: hojiakbarmadaminov45@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -18,28 +18,28 @@
 Requires-Dist: parse==1.20.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
 
 
-#PY-WEB-FRAMEWORK is a Python web framework build for purposes
+PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
 ![purpose](https://image.shields.io/badge/purpose-learning-green)
 ![PyPy - Version](https://image.shields.io/pypi/v/pywebframework)
 
 
 PY-WEB-FRAMEWORK is a Python web framework build for purposes
 
-##Installation
+Installation
 ```shell
 pip install pywebframework-uz
 ```
 
-###Basic usage
+Basic usage
 
 ```python
 
 from app import PyFrameBuilding
 from middleware import CustomMiddleware
 
 server = PyFrameBuilding()
@@ -109,15 +109,15 @@
 
 
 server.add_middleware(SimpleMiddleware)
 
 
 ```
 
-###Unit Tests
+Unit Tests
 The recommended way of writing unit tests is with pytest. There are two built in fixtures that you may want to use when writing unit tests with PYWEBFRAMEWORK.
 The first one is app which is an instance of the main API class:
 
 ```python
 
 def test_basic_route_adding(app):
     @app.route('/home')
@@ -144,15 +144,15 @@
 
     app.add_route('/new-handler', new_handler)
 
     assert test_client.get('http://testserver/new-handler').text == 'From new handler'
 
 ```
 
-###TEMPLATES
+TEMPLATES
 
 The default folder for templates is 'template'. You can change it when
 initializing the  'PyFrameBuilding' class.
 
 ```python
 @server.route('/template')
 def template_handler(request, response):
@@ -161,15 +161,15 @@
             "new_title": 'New Title',
             "new_body": f"Hello 1243"
         }
     )
 ```
 
 
-##Static files
+Static files
 Just like templates, the default folder for static files is static and you can override it:
 server = PyFrameBuilding(static_dir='path/to/static/files/)
 ```html
 <html>
     <header>
         <title>{{new_title}}</title>
```

### Comparing `pywebframework_uz-0.1.1/setup.py` & `pywebframework_uz-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywebframework_uz'
 DESCRIPTION = 'Python web-framework building for learning purpose'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'hojiakbarmadaminov45@gmail.com'
 AUTHOR = 'Madaminov Khojiakbar'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     'requests-wsgi-adapter==0.4.1',
```

