# Comparing `tmp/staticjinjaplus-2.0.0.tar.gz` & `tmp/staticjinjaplus-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticjinjaplus-2.0.0.tar", last modified: Thu Apr 25 06:55:53 2024, max compression
+gzip compressed data, was "staticjinjaplus-2.0.1.tar", last modified: Wed May 15 11:58:20 2024, max compression
```

## Comparing `staticjinjaplus-2.0.0.tar` & `staticjinjaplus-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/
--rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-2.0.0/LICENSE.md
--rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    27015 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    25252 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4150 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/staticjinjaplus/
--rw-rw-rw-   0        0        0     4300 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/__init__.py
--rw-rw-rw-   0        0        0       23 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/__version__.py
--rw-rw-rw-   0        0        0     6240 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/cli.py
--rw-rw-rw-   0        0        0     3084 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/http.py
--rw-rw-rw-   0        0        0     1051 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/jinja_helpers.py
--rw-rw-rw-   0        0        0     4039 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.0/staticjinjaplus/staticjinja_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-25 06:55:53.238922 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/
--rw-rw-rw-   0        0        0    27015 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      146 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 06:55:53.000000 staticjinjaplus-2.0.0/staticjinjaplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 11:58:20.899192 staticjinjaplus-2.0.1/
+-rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-2.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3134 2024-05-15 11:58:20.899192 staticjinjaplus-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1342 2024-05-14 13:45:26.000000 staticjinjaplus-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 11:58:20.899192 staticjinjaplus-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4158 2024-05-14 13:45:26.000000 staticjinjaplus-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:58:20.891192 staticjinjaplus-2.0.1/staticjinjaplus/
+-rw-rw-rw-   0        0        0     4383 2024-05-15 11:53:42.000000 staticjinjaplus-2.0.1/staticjinjaplus/__init__.py
+-rw-rw-rw-   0        0        0       23 2024-05-15 11:56:44.000000 staticjinjaplus-2.0.1/staticjinjaplus/__version__.py
+-rw-rw-rw-   0        0        0     6240 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.1/staticjinjaplus/cli.py
+-rw-rw-rw-   0        0        0     3084 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.1/staticjinjaplus/http.py
+-rw-rw-rw-   0        0        0     1051 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.1/staticjinjaplus/jinja_helpers.py
+-rw-rw-rw-   0        0        0     4039 2024-04-25 06:52:11.000000 staticjinjaplus-2.0.1/staticjinjaplus/staticjinja_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-15 11:58:20.895192 staticjinjaplus-2.0.1/staticjinjaplus.egg-info/
+-rw-rw-rw-   0        0        0     3134 2024-05-15 11:58:20.000000 staticjinjaplus-2.0.1/staticjinjaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2024-05-15 11:58:20.000000 staticjinjaplus-2.0.1/staticjinjaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 11:58:20.000000 staticjinjaplus-2.0.1/staticjinjaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-15 11:58:20.000000 staticjinjaplus-2.0.1/staticjinjaplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2024-05-15 11:58:20.000000 staticjinjaplus-2.0.1/staticjinjaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-15 11:58:20.000000 staticjinjaplus-2.0.1/staticjinjaplus.egg-info/top_level.txt
```

### Comparing `staticjinjaplus-2.0.0/LICENSE.md` & `staticjinjaplus-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-2.0.0/setup.py` & `staticjinjaplus-2.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ]
 
 EXTRAS = {
     'dev': {
         'build~=1.2',
         'twine~=5.0',
         'setuptools~=69.5',
+        'mkdocs~=1.6'
     }
 }
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Operating System :: OS Independent',
     'Environment :: Console',
@@ -45,17 +46,17 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Intended Audience :: Developers',
 ]
 
 PROJECT_URLS = {
-    'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme',
-    'Source': 'https://github.com/EpocDotFr/staticjinjaplus',
-    'Tracker': 'https://github.com/EpocDotFr/staticjinjaplus/issues',
+    'Documentation': 'https://epocdotfr.github.io/staticjinjaplus/',
+    'Source code': 'https://github.com/EpocDotFr/staticjinjaplus',
+    'Issue tracker': 'https://github.com/EpocDotFr/staticjinjaplus/issues',
     'Changelog': 'https://github.com/EpocDotFr/staticjinjaplus/releases',
 }
 
 KEYWORDS = ['static', 'website', 'site', 'generator', 'staticjinja', 'jinja', 'jinja2']
 
 here = path.abspath(path.dirname(__file__))
```

### Comparing `staticjinjaplus-2.0.0/staticjinjaplus/__init__.py` & `staticjinjaplus-2.0.1/staticjinjaplus/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,24 +46,27 @@
             k: v for k, v in vars(actual_config).items() if k.isupper()
         })
     except FileNotFoundError:
         pass
 
 
 def smart_build_url(filename: str) -> Tuple[str, str]:
-    """Build a webserver and SEO-friendly (if configured so) URL to an HTML file"""
+    """Build a pretty URL (if configured so) pointing to an HTML file"""
     _, ext = path.splitext(filename)
     ext = ext.lstrip('.')
 
     url = '/' + filename.lstrip('/')
 
     if url.endswith(('/index.html', '/index.md')):
         url = url.removesuffix('/index.html').removesuffix('/index.md') + '/'
-    elif ext in ('html', 'md') and not config['USE_HTML_EXTENSION']:
-        url, _ = path.splitext(url)
+    elif ext in ('html', 'md'):
+        if not config['USE_HTML_EXTENSION']:
+            url, _ = path.splitext(url)
+        elif ext == 'md':
+            url, = url.removesuffix('.md') + '.html'
 
     return url, ext
 
 
 def collect_templates() -> Iterator[Dict[str, Any]]:
     """Iterates over all valid files found in the templates directory and return several kind of information about
     them."""
```

### Comparing `staticjinjaplus-2.0.0/staticjinjaplus/cli.py` & `staticjinjaplus-2.0.1/staticjinjaplus/cli.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-2.0.0/staticjinjaplus/http.py` & `staticjinjaplus-2.0.1/staticjinjaplus/http.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-2.0.0/staticjinjaplus/jinja_helpers.py` & `staticjinjaplus-2.0.1/staticjinjaplus/jinja_helpers.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-2.0.0/staticjinjaplus/staticjinja_helpers.py` & `staticjinjaplus-2.0.1/staticjinjaplus/staticjinja_helpers.py`

 * *Files identical despite different names*

