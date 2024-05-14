# Comparing `tmp/deepmodeling_sphinx-0.2.6.tar.gz` & `tmp/deepmodeling_sphinx-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmodeling_sphinx-0.2.6.tar", last modified: Tue May 14 20:14:16 2024, max compression
+gzip compressed data, was "deepmodeling_sphinx-0.2.7.tar", last modified: Tue May 14 20:39:16 2024, max compression
```

## Comparing `deepmodeling_sphinx-0.2.6.tar` & `deepmodeling_sphinx-0.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.906937 deepmodeling_sphinx-0.2.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.906937 deepmodeling_sphinx-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.906937 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.css
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.html
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.js
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/dark_rtd.css
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/inject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 20:14:16.000000 deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-14 20:14:12.000000 deepmodeling_sphinx-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:14:16.910936 deepmodeling_sphinx-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:16.503728 deepmodeling_sphinx-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:16.499728 deepmodeling_sphinx-0.2.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:16.499728 deepmodeling_sphinx-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-14 20:39:16.503728 deepmodeling_sphinx-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:16.499728 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/banner.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/banner.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/dark_rtd.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/inject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:16.503728 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-14 20:39:16.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 20:39:16.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:39:16.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 20:39:16.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 20:39:16.000000 deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:39:16.503728 deepmodeling_sphinx-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-14 20:39:11.000000 deepmodeling_sphinx-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:39:16.503728 deepmodeling_sphinx-0.2.7/setup.cfg
```

### Comparing `deepmodeling_sphinx-0.2.6/.github/workflows/release.yml` & `deepmodeling_sphinx-0.2.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/.gitignore` & `deepmodeling_sphinx-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/.pre-commit-config.yaml` & `deepmodeling_sphinx-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/.readthedocs.yaml` & `deepmodeling_sphinx-0.2.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/LICENSE` & `deepmodeling_sphinx-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/PKG-INFO` & `deepmodeling_sphinx-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepmodeling_sphinx
-Version: 0.2.6
+Version: 0.2.7
 Summary: Sphinx extension for DeepModeling projects.
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `deepmodeling_sphinx-0.2.6/README.md` & `deepmodeling_sphinx-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/authors.py` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/authors.py`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.css` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/banner.css`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.html` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/banner.html`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/banner.js` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/banner.js`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/config.py` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/config.py`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/dark_rtd.css` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/dark_rtd.css`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx/inject.py` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx/inject.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,20 @@
 
 def minify_html_files(app, pagename, templatename, context, doctree):
     if not hasattr(app.builder.templates.render, "_deepmodeling_minified"):
         old_render = app.builder.templates.render
 
         def render(self, template, render_context):
             content = old_render(template, render_context)
-            return minify_html_onepass.minify(content, minify_js=True)
+            try:
+                return minify_html_onepass.minify(
+                    content, minify_js=True, minify_css=True
+                )
+            except SyntaxError:
+                return content
 
         render.__dict__.update(old_render.__dict__)
         render._deepmodeling_minified = True
         app.builder.templates.render = types.MethodType(render, app.builder.templates)
 
 
 def minify_js_files(app, exception):
```

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/PKG-INFO` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepmodeling_sphinx
-Version: 0.2.6
+Version: 0.2.7
 Summary: Sphinx extension for DeepModeling projects.
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `deepmodeling_sphinx-0.2.6/deepmodeling_sphinx.egg-info/SOURCES.txt` & `deepmodeling_sphinx-0.2.7/deepmodeling_sphinx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/docs/conf.py` & `deepmodeling_sphinx-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `deepmodeling_sphinx-0.2.6/pyproject.toml` & `deepmodeling_sphinx-0.2.7/pyproject.toml`

 * *Files identical despite different names*

