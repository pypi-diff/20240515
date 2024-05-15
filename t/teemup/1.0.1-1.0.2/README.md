# Comparing `tmp/teemup-1.0.1.tar.gz` & `tmp/teemup-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teemup-1.0.1.tar", max compression
+gzip compressed data, was "teemup-1.0.2.tar", max compression
```

## Comparing `teemup-1.0.1.tar` & `teemup-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1085 2023-08-31 13:16:48.364436 teemup-1.0.1/LICENSE
--rw-r--r--   0        0        0     3290 2023-08-31 13:16:48.364436 teemup-1.0.1/README.md
--rw-r--r--   0        0        0      572 2023-08-31 13:16:48.364436 teemup-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1374 2023-08-31 13:16:48.364436 teemup-1.0.1/teemup.py
--rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 teemup-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-15 10:51:32.405284 teemup-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3334 2024-05-15 10:51:32.405284 teemup-1.0.2/README.md
+-rw-r--r--   0        0        0      572 2024-05-15 10:51:32.405284 teemup-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1374 2024-05-15 10:51:32.405284 teemup-1.0.2/teemup.py
+-rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 teemup-1.0.2/PKG-INFO
```

### Comparing `teemup-1.0.1/LICENSE` & `teemup-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `teemup-1.0.1/README.md` & `teemup-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,43 @@
+Metadata-Version: 2.1
+Name: teemup
+Version: 1.0.2
+Summary: If Meetup didn't become a walled garden, the world wouldn't need Teemup
+License: MIT
+Author: Honza Javorek
+Author-email: mail@honzajavorek.cz
+Requires-Python: ==3.11.*
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cssselect (==1.2.0)
+Requires-Dist: lxml (==5.2.2)
+Description-Content-Type: text/markdown
+
 # teemup
 
 _If Meetup didn't become a walled garden, the world wouldn't need Teemup_
 
 ## Purpose and scope
 
 This library takes HTML source of a meetup group page on Meetup and returns a list of their upcoming events.
 
 ## Usage
 
 ```python
 >>> import urllib.request
 >>> from teemup import parse
->>> with urllib.request.urlopen('https://www.meetup.com/reactgirls/') as f:
+>>> with urllib.request.urlopen('https://www.meetup.com/dresdenjs-io-javascript-user-group/') as f:
 ...     html = f.read()
 ...
 >>> events = parse(html)
->>> sorted(events[0].keys())
+>>> event = next(event for event in events if event['venue'] is not None)
+>>> sorted(event.keys())
 ['description', 'ends_at', 'starts_at', 'title', 'url', 'venue']
->>> sorted(events[0]['venue'])
+>>> sorted(event['venue'])
 ['address', 'city', 'country', 'name', 'state']
 
 ```
 
 The example above is [tested](https://docs.pytest.org/doctest.html) and thus doesn't contain any variable data, but should be enough to give you an idea.
 
 ## If something breaks
@@ -38,15 +54,14 @@
 
 -   Make sure the tests really pass: `poetry run pytest`
 -   Format the code: `poetry run black .`
 -   Raise the version number in `pyproject.toml`
 -   Commit the changes: `git commit -am "release vX.Y.Z"`
 -   Create a version tag: `git tag vX.Y.Z`
 -   Push the tag: `git push --tags`
--   Publish to PyPI: `poetry publish --build`
 
 **Note:** If there are no upcoming events, choose a different group page for testing.
 Do not remove live testing from the repository!
 The whole purpose of the library is to be up-to-date with the current website.
 It must be monitored every day and fixed as soon as it breaks.
 
 ## Why
@@ -71,7 +86,8 @@
 
 All out war then!
 I moved the code to this separate library so it's easier to develop, re-use, contribute to, and monitor.
 
 ## License
 
 [MIT](LICENSE)
+
```

### Comparing `teemup-1.0.1/pyproject.toml` & `teemup-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "teemup"
-version = "1.0.1"
+version = "1.0.2"
 description = "If Meetup didn't become a walled garden, the world wouldn't need Teemup"
 authors = ["Honza Javorek <mail@honzajavorek.cz>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.*"
-lxml = "4.9.3"
+lxml = "5.2.2"
 cssselect = "1.2.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "7.4.0"
-black = "23.7.0"
+pytest = "8.2.0"
+black = "24.4.2"
 
 [tool.pytest.ini_options]
 python_files = "test_*.py"
 testpaths = "."
 addopts = "-v --doctest-glob=README.md"
 
 [build-system]
```

### Comparing `teemup-1.0.1/teemup.py` & `teemup-1.0.2/teemup.py`

 * *Files identical despite different names*

