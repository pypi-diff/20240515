# Comparing `tmp/jinjafx_server-24.3.0.tar.gz` & `tmp/jinjafx_server-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjafx_server-24.3.0.tar", last modified: Thu Mar  7 23:46:10 2024, max compression
+gzip compressed data, was "jinjafx_server-24.5.0.tar", last modified: Wed May 15 06:22:26 2024, max compression
```

## Comparing `jinjafx_server-24.3.0.tar` & `jinjafx_server-24.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:46:10.153428 jinjafx_server-24.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-03-07 23:46:10.153428 jinjafx_server-24.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:46:10.149428 jinjafx_server-24.3.0/jinjafx_server/
--rwxr-xr-x   0 runner    (1001) docker     (127)    45466 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:46:10.149428 jinjafx_server-24.3.0/jinjafx_server/pandoc/
--rw-r--r--   0 runner    (1001) docker     (127)    22696 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/pandoc/reference.docx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:46:10.153428 jinjafx_server-24.3.0/jinjafx_server/www/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/dt.html
--rw-r--r--   0 runner    (1001) docker     (127)    26751 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/jinjafx.css
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/jinjafx.png
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_dt.js
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_m.css
--rw-r--r--   0 runner    (1001) docker     (127)    64627 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_m.js
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_o.css
--rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_o.js
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/obsolete.html
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/obsolete.js
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/jinjafx_server/www/output.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 23:46:10.149428 jinjafx_server-24.3.0/jinjafx_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-03-07 23:46:10.000000 jinjafx_server-24.3.0/jinjafx_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-07 23:46:10.000000 jinjafx_server-24.3.0/jinjafx_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 23:46:10.000000 jinjafx_server-24.3.0/jinjafx_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-07 23:46:10.000000 jinjafx_server-24.3.0/jinjafx_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-07 23:46:10.000000 jinjafx_server-24.3.0/jinjafx_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-07 23:46:10.000000 jinjafx_server-24.3.0/jinjafx_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 23:46:10.153428 jinjafx_server-24.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-07 23:46:08.000000 jinjafx_server-24.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:22:26.003006 jinjafx_server-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-15 06:22:26.003006 jinjafx_server-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:22:25.999006 jinjafx_server-24.5.0/jinjafx_server/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45466 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:22:25.999006 jinjafx_server-24.5.0/jinjafx_server/pandoc/
+-rw-r--r--   0 runner    (1001) docker     (127)    22696 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/pandoc/reference.docx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:22:26.003006 jinjafx_server-24.5.0/jinjafx_server/www/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/dt.html
+-rw-r--r--   0 runner    (1001) docker     (127)    26754 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/jinjafx.css
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/jinjafx.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_dt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_m.css
+-rw-r--r--   0 runner    (1001) docker     (127)    64627 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_m.js
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_o.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_o.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/obsolete.html
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/obsolete.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/jinjafx_server/www/output.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:22:25.999006 jinjafx_server-24.5.0/jinjafx_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-15 06:22:25.000000 jinjafx_server-24.5.0/jinjafx_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 06:22:25.000000 jinjafx_server-24.5.0/jinjafx_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:22:25.000000 jinjafx_server-24.5.0/jinjafx_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 06:22:25.000000 jinjafx_server-24.5.0/jinjafx_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 06:22:25.000000 jinjafx_server-24.5.0/jinjafx_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 06:22:25.000000 jinjafx_server-24.5.0/jinjafx_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:22:26.003006 jinjafx_server-24.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 06:22:20.000000 jinjafx_server-24.5.0/setup.py
```

### Comparing `jinjafx_server-24.3.0/LICENSE` & `jinjafx_server-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/PKG-INFO` & `jinjafx_server-24.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: jinjafx_server
-Version: 24.3.0
+Version: 24.5.0
 Summary: JinjaFx Server - Jinja2 Templating Tool
 Home-page: https://github.com/cmason3/jinjafx_server
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img src="https://img.shields.io/badge/url-https%3A%2F%2Fjinjafx.io-blue" align="right">](https://jinjafx.io)
 &nbsp;
 <h1 align="center">JinjaFx Server - Jinja2 Templating Tool</h1>
```

### Comparing `jinjafx_server-24.3.0/README.md` & `jinjafx_server-24.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![PyPI](https://img.shields.io/pypi/v/jinjafx-server.svg)](https://pypi.python.org/pypi/jinjafx-server/)
-![Python](https://img.shields.io/badge/python-≥&nbsp;3.8-brightgreen)
+![Python](https://img.shields.io/badge/python-≥&nbsp;3.9-brightgreen)
 [<img src="https://img.shields.io/badge/url-https%3A%2F%2Fjinjafx.io-blue" align="right">](https://jinjafx.io)
 &nbsp;
 <h1 align="center">JinjaFx Server - Jinja2 Templating Tool</h1>
 
 JinjaFx Server is a lightweight web server that provides a Web UI to JinjaFx. It is a separate Python module which imports the "jinjafx" module to generate outputs from a web interface - it does require the "requests" module which isn't in the base install. Usage instructions are provided below, although it is considered an additional component and not part of the base JinjaFx tool, although it is probably a much easier way to use it.
 
 ### Installation
```

### Comparing `jinjafx_server-24.3.0/jinjafx_server/__init__.py` & `jinjafx_server-24.5.0/jinjafx_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 import sys
-if sys.version_info < (3, 8):
-  sys.exit('Requires Python >= 3.8')
+if sys.version_info < (3, 9):
+  sys.exit('Requires Python >= 3.9')
 
 from http.cookies import SimpleCookie
 from http.server import HTTPServer, BaseHTTPRequestHandler
 from urllib.parse import urlparse, parse_qs
 from jinja2 import __version__ as jinja2_version
 
 import jinjafx, os, io, socket, signal, threading, yaml, json, base64, time, datetime, resource
 import re, argparse, hashlib, traceback, glob, hmac, uuid, struct, binascii, gzip, requests, ctypes, subprocess
 import cmarkgfm, emoji
 
-__version__ = '24.3.0'
+__version__ = '24.5.0'
 
 llock = threading.RLock()
 rlock = threading.RLock()
 base = os.path.abspath(os.path.dirname(__file__))
 
 aws_s3_url = None
 aws_access_key = None
@@ -544,15 +544,15 @@
                 output = '\n'.join(outputs[o]) + '\n'
                 if len(output.strip()) > 0:
                   if oformat == 'markdown' or oformat == 'md':
                     o = oname + ':html'
                     options = (cmarkgfm.cmark.Options.CMARK_OPT_GITHUB_PRE_LANG | cmarkgfm.cmark.Options.CMARK_OPT_SMART | cmarkgfm.cmark.Options.CMARK_OPT_UNSAFE)
                     output = cmarkgfm.github_flavored_markdown_to_html(html_escape(output), options).replace('&amp;amp;', '&amp;').replace('&amp;', '&')
                     head = '<!DOCTYPE html>\n<html>\n<head>\n'
-                    head += '<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/github-markdown-css/5.5.0/github-markdown.min.css" crossorigin="anonymous">\n'
+                    head += '<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/github-markdown-css/5.5.1/github-markdown.min.css" crossorigin="anonymous">\n'
                     head += '<style>\n  pre, code { white-space: pre-wrap !important; word-wrap: break-word !important; }\n</style>\n</head>\n'
                     output = emoji.emojize(output, language='alias').encode('ascii', 'xmlcharrefreplace').decode('utf-8')
                     output = head + '<body>\n<div class="markdown-body">\n' + output + '</div>\n</body>\n</html>\n'
 
                   elif oformat == 'html':
                     output = output.encode('ascii', 'xmlcharrefreplace').decode('utf-8')
```

### Comparing `jinjafx_server-24.3.0/jinjafx_server/__main__.py` & `jinjafx_server-24.5.0/jinjafx_server/__main__.py`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/pandoc/reference.docx` & `jinjafx_server-24.5.0/jinjafx_server/pandoc/reference.docx`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/dt.html` & `jinjafx_server-24.5.0/jinjafx_server/www/dt.html`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
   <head>
     <meta charset="utf-8">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self'; style-src 'self' https://cdnjs.cloudflare.com 'unsafe-inline'">
     <meta name="viewport" content="width=1536, user-scalable=no">
     <title>JinjaFx DataTemplate</title>
     <link rel="shortcut icon" href="/874f2915/jinjafx.png">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" integrity="sha512-b2QcS5SsA8tZodcDtGRELiGv5SaKSk1vDHDaQRda0htPYWZ6046lr3kJ5bAAQdpV2mmA/4v0wQF9MyU6/pDIAg==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css" integrity="sha512-jnSuA4Ss2PkkikSOLtYs8BlYIeeIK1h99ty4YfvRPAlzr377vr3CXDb7sb7eEEBYjDtcYj+AjBH3FLv5uSJuXg==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="/f8555653/jinjafx.css">
     <script src="/00abd23c/jinjafx_dt.js"></script>
   </head>
   <body>
     <div id="wrap" class="p-2 bg-transparent">
       <button id="saveas" class="btn btn-secondary text-white float-end me-3 mt-3 d-none" type="button" title="Save DataTemplate As">
         <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
```

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/index.html` & `jinjafx_server-24.5.0/jinjafx_server/www/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     <meta charset="utf-8">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self'; style-src 'self' https://cdnjs.cloudflare.com 'unsafe-inline'; script-src 'self' https://cdnjs.cloudflare.com; img-src 'self' data:">
     <meta name="viewport" content="width=1536, user-scalable=no">
     <meta name="description" content="JinjaFx is a Python based Jinja2 Templating Tool with support for Ansible filters that renders output based on CSV or YAML datasets">
     <title>JinjaFx - Jinja2 Templating Tool</title>
     <script src="/6d052dbe/obsolete.js"></script>
     <link rel="shortcut icon" href="/874f2915/jinjafx.png">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" integrity="sha512-b2QcS5SsA8tZodcDtGRELiGv5SaKSk1vDHDaQRda0htPYWZ6046lr3kJ5bAAQdpV2mmA/4v0wQF9MyU6/pDIAg==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css" integrity="sha512-jnSuA4Ss2PkkikSOLtYs8BlYIeeIK1h99ty4YfvRPAlzr377vr3CXDb7sb7eEEBYjDtcYj+AjBH3FLv5uSJuXg==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/codemirror.min.css" integrity="sha512-uf06llspW44/LZpHzHT6qBOIVODjWtv4MxCricRxkzvopAlSWnTf6hpZTFxuuZcuNE9CBQhqE0Seu1CoRk84nQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/dialog/dialog.min.css" integrity="sha512-Vogm+Cii1SXP5oxWQyPdkA91rHB776209ZVvX4C/i4ypcfBlWVRXZGodoTDAyyZvO36JlTqDqkMhVKAYc7CMjQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/display/fullscreen.min.css" integrity="sha512-T8xB3MmwpA77VK9lUH3UkdUTnkmpqOxHF8OceOKaHrvpcXMSNX0xtpa9FoLTDAVO1JnB2UiMdVeI2V0HTHjTWA==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/fold/foldgutter.min.css" integrity="sha512-YwkMTlTHn8dBnwa47IF+cKsS00HPiiVhQ4DpwT1KF2gUftfFR7aefepabSPLAs6zrMyD89M3w0Ow6mQ5XJEUCw==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="/f8555653/jinjafx.css">
     <link rel="stylesheet" href="/af18a9f8/jinjafx_m.css">
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/js/bootstrap.bundle.min.js" integrity="sha512-X/YkDZyjTf4wyc2Vy16YGCPHwAY8rZJY+POgokZjQB2mhIRFJCckEGc6YyX9eNsPfn0PzThEuNs+uaomE5CO6A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/js/bootstrap.bundle.min.js" integrity="sha512-7Pi/otdlbbCR+LnW+F7PwFcSDJOuUJB3OxtEHbg4vSMvzvJjde4Po1v4BR9Gdc9aXNUNFVUY+SK51wWT8WF0Gg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/codemirror.min.js" integrity="sha512-OeZ4Yrb/W7d2W4rAMOO0HQ9Ro/aWLtpW9BUSR2UOWnSV2hprXLkkYnnCGc9NeLUxxE4ZG7zN16UuT1Elqq8Opg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/selection/mark-selection.min.js" integrity="sha512-XaS0JPIY5yDTDaYIMjkoXz+LF/DEVhRn1eq9QOhJPhMuJGGPOKZTulF+LY8/uwd18k00CIaSe4f8fCyp/5U7IQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/dialog/dialog.min.js" integrity="sha512-NAJeqwfpM7/nfX90EweQhjudb66diK3Y9mkBjb4xJ6wufuVqFVAjHd8mJW//CGHNR9cI8wUfDRJ0jtLzZ9v8Qg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/display/fullscreen.min.js" integrity="sha512-8Rk4wB3MfgQfuOw95XW/vAU8PSTHWI5HddVRXfg+Ykk8CzsiOZkDpxVSrnYq2u/IqO499ooZ61fFHppuzB2ghA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/search/search.min.js" integrity="sha512-Mw3RqCUHTyvN3iSp5TSs731TiLqnKrxzyy2UVZv3+tJa524Rj7pBC7Ivv3ka2oDnkQwLOMHNDKU5nMJ16YRgrA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/search/searchcursor.min.js" integrity="sha512-+ZfZDC9gi1y9Xoxi9UUsSp+5k+AcFE0TRNjI0pfaAHQ7VZTaaoEpBZp9q9OvHdSomOze/7s5w27rcsYpT6xU6g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/edit/trailingspace.min.js" integrity="sha512-xcccdc2hhCFOxhdb8nh6lTpOS7gNTw36W/TIaDoNfydtLhxbebAqiqhY8zty5K5V57/Pgpb9wD27fH1UHYk8yQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
@@ -27,16 +27,16 @@
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/fold/foldgutter.min.js" integrity="sha512-TRBGROluEM9UrFPnoCk0vW2PqqcMUyGJETe60qzktKTEiXmPhmxqJLYqOf7TsX4ulMbANjdpLY+DYk0aoht4gA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/addon/mode/overlay.min.js" integrity="sha512-SNwKDMYQwymOPjleeZy1xbdlK1PAjJ6EAplvx0CvNFJbW/pF5ec3h0mAdDl1yySq9r3Qont4STM4W3le7FTm9w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/mode/jinja2/jinja2.min.js" integrity="sha512-Z4le1RxwhD8lDCrspbBxjTLLP2HGC1+mKb9KHR2N/sEx8uOe2vre5XQo8YMPAz8FQTo43HjefjlDtjY4LtfaaQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.16/mode/yaml/yaml.min.js" integrity="sha512-Prlj899DsOyGWU8noS4ZqQ8Z4jy+215JiZPxt/cT3ds3VqbwwsjSYZ64zCWQ/Z7AUZvymKGRllUSLPW5RKylNQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/pako/2.1.0/pako_deflate.min.js" integrity="sha512-oEsmlMj4bUaKNfYtsxV2eZm+5L0I/JhLsXftLFKeywkgAq8QMLKRlZrMIkMC2AHZQ/gT8YtI+fP1WUwNjF1PoQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/split.js/1.6.5/split.min.js" integrity="sha512-lNjb0qWDVvt1zfSiXufaxtlFtenve3BLbvljxuMXuSr0DE0HYp5OhX0u89uwNd6MvlX1bgJ8ulfG4JMGurs8UA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js" integrity="sha512-CSBhVREyzHAjAFfBlIBakjoRUKp5h7VSweP0InR/pAJyptH7peuhCsqAI/snV+TwZmXZqoUklpXp6R6wMnYf5Q==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.10/dayjs.min.js" integrity="sha512-FwNWaxyfy2XlEINoSnZh1JQ5TRRtGow0D6XcmAWmYCRgvqOUTnzCxPc9uF35u5ZEpirk1uhlPVA19tflhvnW1g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.10/plugin/relativeTime.min.js" integrity="sha512-MVzDPmm7QZ8PhEiqJXKz/zw2HJuv61waxb8XXuZMMs9b+an3LoqOqhOEt5Nq3LY1e4Ipbbd/e+AWgERdHlVgaA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.11/dayjs.min.js" integrity="sha512-FwNWaxyfy2XlEINoSnZh1JQ5TRRtGow0D6XcmAWmYCRgvqOUTnzCxPc9uF35u5ZEpirk1uhlPVA19tflhvnW1g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.11/plugin/relativeTime.min.js" integrity="sha512-MVzDPmm7QZ8PhEiqJXKz/zw2HJuv61waxb8XXuZMMs9b+an3LoqOqhOEt5Nq3LY1e4Ipbbd/e+AWgERdHlVgaA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="/73874bbf/jinjafx_m.js"></script>
   </head>
   <body>
     <div id="overlay"></div>
     <div id="wrap">
       <h1 class="d-none">JinjaFx - Jinja2 Templating Tool</h1>
       <div id="header" class="p-3">
@@ -152,15 +152,15 @@
             <div id="cdata" class="split-horizontal position-relative">
               <div class="badge lb-data float-start labels">D<br />A<br />T<br />A<br />.<br />C<br />S<br />V<br /></div>
               <textarea id="data"></textarea>
               <div id="csv"></div>
             </div>
             <div id="cvars" class="split-horizontal">
               <div id="xgvars" class="position-relative d-none">
-                <div class="badge lb-gvars float-start labels">G<br />L<br />O<br />B<br />A<br />L<br />.<br />Y<br />M</br />L</br /></div>
+                <div class="badge lb-gvars float-start labels">G<br />L<br />O<br />B<br />A<br />L<br />.<br />Y<br />M<br />L<br /></div>
                 <textarea id="t_gvars"></textarea>
               </div>
               <div id="xlvars" class="position-relative h-100">
                 <div class="badge lb-vars float-start labels">V<br />A<br />R<br />S<br />.<br />Y<br />M<br />L<br /></div>
                 <textarea id="vars"></textarea>
               </div>
             </div>
@@ -202,15 +202,15 @@
 usnh-pe-1a, pe
 usnh-pe-1b, pe</pre>
                 <p>We also support the ability to expand rows based on numerical counters using the <span class="cm-jfx-tag">{ start[-end]:step }</span> syntax, e.g:</p>
 <pre class="code-block">INTERFACE
 et-0/0/<span class="cm-jfx-tag">{0-9:1}</span></pre>
                 <p>The above syntax would convert one row into ten rows using the values 0 to 9. If the <span class="cm-jfx-tag">end</span> value is omitted then it is a passive counter and will only increment if something else is expanding the rows.</p>
                 <br /><h3>Inputs</h3><hr>
-                <p>Normally data is provided to JinjaFx via CSV or YAML using the above panes, but JinjaFx can also prompt the user for input using the "jinjafx_input" variable in "vars.yml", e.g:</p>
+                <p>Normally data is provided to JinjaFx via CSV or YAML/JSON using the above panes, but JinjaFx can also prompt the user for input using the "jinjafx_input" variable in "vars.yml", e.g:</p>
 <pre class="code-block">jinjafx_input:
   prompt:
     name:
       text: "Name"
       required: True
     age:
       text: "Age"
```

#### html2text {}

```diff
@@ -18,15 +18,16 @@
 L
 O
 B
 A
 L
 .
 Y
-ML
+M
+L
 V
 A
 R
 S
 .
 Y
 M
@@ -92,17 +93,17 @@
 et-0/0/{0-9:1}
 The above syntax would convert one row into ten rows using the values 0 to 9.
 If the end value is omitted then it is a passive counter and will only
 increment if something else is expanding the rows.
 
 ******** IInnppuuttss ********
 ===============================================================================
-Normally data is provided to JinjaFx via CSV or YAML using the above panes, but
-JinjaFx can also prompt the user for input using the "jinjafx_input" variable
-in "vars.yml", e.g:
+Normally data is provided to JinjaFx via CSV or YAML/JSON using the above
+panes, but JinjaFx can also prompt the user for input using the "jinjafx_input"
+variable in "vars.yml", e.g:
 jinjafx_input:
   prompt:
     name:
       text: "Name"
       required: True
     age:
       text: "Age"
```

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/jinjafx.css` & `jinjafx_server-24.5.0/jinjafx_server/www/jinjafx.css`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_dt.js` & `jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_dt.js`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_m.css` & `jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_m.css`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_m.js` & `jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_m.js`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_o.css` & `jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_o.css`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/jinjafx_o.js` & `jinjafx_server-24.5.0/jinjafx_server/www/jinjafx_o.js`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/logs.html` & `jinjafx_server-24.5.0/jinjafx_server/www/logs.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=1280, user-scalable=no">
     <title>JinjaFx Logs</title>
     <link rel="shortcut icon" href="/874f2915/jinjafx.png">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" integrity="sha512-b2QcS5SsA8tZodcDtGRELiGv5SaKSk1vDHDaQRda0htPYWZ6046lr3kJ5bAAQdpV2mmA/4v0wQF9MyU6/pDIAg==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css" integrity="sha512-jnSuA4Ss2PkkikSOLtYs8BlYIeeIK1h99ty4YfvRPAlzr377vr3CXDb7sb7eEEBYjDtcYj+AjBH3FLv5uSJuXg==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/firacode/6.2.0/fira_code.min.css" integrity="sha512-MbysAYimH1hH2xYzkkMHB6MqxBqfP0megxsCLknbYqHVwXTCg9IqHbk+ZP/vnhO8UEW6PaXAkKe2vQ+SWACxxA==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="/f8555653/jinjafx.css">
     <style>
       body {
         color: white;
         background: #000040;
       }
```

### Comparing `jinjafx_server-24.3.0/jinjafx_server/www/output.html` & `jinjafx_server-24.5.0/jinjafx_server/www/output.html`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 <html lang="en">
   <head>
     <meta charset="utf-8">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self'; style-src 'self' https://cdnjs.cloudflare.com 'unsafe-inline'; script-src 'self' https://cdnjs.cloudflare.com">
     <meta name="viewport" content="width=1536, user-scalable=no">
     <title>Generating...</title>
     <link rel="shortcut icon" href="/874f2915/jinjafx.png">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/css/bootstrap.min.css" integrity="sha512-b2QcS5SsA8tZodcDtGRELiGv5SaKSk1vDHDaQRda0htPYWZ6046lr3kJ5bAAQdpV2mmA/4v0wQF9MyU6/pDIAg==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css" integrity="sha512-jnSuA4Ss2PkkikSOLtYs8BlYIeeIK1h99ty4YfvRPAlzr377vr3CXDb7sb7eEEBYjDtcYj+AjBH3FLv5uSJuXg==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="/f8555653/jinjafx.css">
     <link rel="stylesheet" href="/6ba409b7/jinjafx_o.css">
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.2/js/bootstrap.bundle.min.js" integrity="sha512-X/YkDZyjTf4wyc2Vy16YGCPHwAY8rZJY+POgokZjQB2mhIRFJCckEGc6YyX9eNsPfn0PzThEuNs+uaomE5CO6A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/js/bootstrap.bundle.min.js" integrity="sha512-7Pi/otdlbbCR+LnW+F7PwFcSDJOuUJB3OxtEHbg4vSMvzvJjde4Po1v4BR9Gdc9aXNUNFVUY+SK51wWT8WF0Gg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/pako/2.1.0/pako_deflate.min.js" integrity="sha512-oEsmlMj4bUaKNfYtsxV2eZm+5L0I/JhLsXftLFKeywkgAq8QMLKRlZrMIkMC2AHZQ/gT8YtI+fP1WUwNjF1PoQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.10/dayjs.min.js" integrity="sha512-FwNWaxyfy2XlEINoSnZh1JQ5TRRtGow0D6XcmAWmYCRgvqOUTnzCxPc9uF35u5ZEpirk1uhlPVA19tflhvnW1g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.10/plugin/advancedFormat.min.js" integrity="sha512-oOF6H/+bcZjL9xEZ71lPxWSLn62axEgf6jDBuge0rTy7HjcMmWLQ7Y46WVC0m1hGibeYyTeHLi1ZUrZTvt2QxQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.11/dayjs.min.js" integrity="sha512-FwNWaxyfy2XlEINoSnZh1JQ5TRRtGow0D6XcmAWmYCRgvqOUTnzCxPc9uF35u5ZEpirk1uhlPVA19tflhvnW1g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.11/plugin/advancedFormat.min.js" integrity="sha512-oOF6H/+bcZjL9xEZ71lPxWSLn62axEgf6jDBuge0rTy7HjcMmWLQ7Y46WVC0m1hGibeYyTeHLi1ZUrZTvt2QxQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.10.1/jszip.min.js" integrity="sha512-XMVd28F1oH/O71fzwBnV7HucLxVwtxf26XV8P4wPk26EDxuGZ91N8bsOttmnomcCD3CS5ZMRL50H0GgOHvegtg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="/21f07ee6/jinjafx_o.js"></script>
   </head>
   <body>
     <div id="status" class="alert alert-primary wait fw-bold">Generating Output...</div>
     <div id="wrap" class="d-none">
       <div id="header" class="p-3">
```

### Comparing `jinjafx_server-24.3.0/jinjafx_server.egg-info/PKG-INFO` & `jinjafx_server-24.5.0/jinjafx_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: jinjafx-server
-Version: 24.3.0
+Version: 24.5.0
 Summary: JinjaFx Server - Jinja2 Templating Tool
 Home-page: https://github.com/cmason3/jinjafx_server
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img src="https://img.shields.io/badge/url-https%3A%2F%2Fjinjafx.io-blue" align="right">](https://jinjafx.io)
 &nbsp;
 <h1 align="center">JinjaFx Server - Jinja2 Templating Tool</h1>
```

### Comparing `jinjafx_server-24.3.0/jinjafx_server.egg-info/SOURCES.txt` & `jinjafx_server-24.5.0/jinjafx_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jinjafx_server-24.3.0/setup.py` & `jinjafx_server-24.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 README = (HERE / "README.md").read_text()
 README = re.sub(r'^.*\[<img', '[<img', README, flags=re.DOTALL)
 README = re.sub(r'<p.+?</p>', '', README, flags=re.DOTALL)    
 
 setup(
   name="jinjafx_server",
   version=__version__,
-  python_requires=">=3.8",
+  python_requires=">=3.9",
   description="JinjaFx Server - Jinja2 Templating Tool",
   long_description=README,
   long_description_content_type="text/markdown",
   url="https://github.com/cmason3/jinjafx_server",
   author="Chris Mason",
   author_email="chris@netnix.org",
   license="MIT",
```

