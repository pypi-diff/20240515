# Comparing `tmp/sphinx-github-style-1.2.1.tar.gz` & `tmp/sphinx-github-style-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-github-style-1.2.1.tar", last modified: Sun Apr  7 11:29:53 2024, max compression
+gzip compressed data, was "sphinx-github-style-1.2.2.tar", last modified: Wed May 15 04:58:17 2024, max compression
```

## Comparing `sphinx-github-style-1.2.1.tar` & `sphinx-github-style-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/
--rw-rw-rw-   0        0        0     1087 2023-04-27 12:00:21.000000 sphinx-github-style-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     7123 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6373 2024-04-07 11:29:26.000000 sphinx-github-style-1.2.1/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1519 2024-01-21 05:39:18.000000 sphinx-github-style-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.053723 sphinx-github-style-1.2.1/sphinx_github_style/
--rw-rw-rw-   0        0        0     1881 2024-04-07 11:23:50.000000 sphinx-github-style-1.2.1/sphinx_github_style/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.069351 sphinx-github-style-1.2.1/sphinx_github_style/_static/
--rw-rw-rw-   0        0        0     1128 2023-08-25 05:08:55.000000 sphinx-github-style-1.2.1/sphinx_github_style/_static/github_style.css
--rw-rw-rw-   0        0        0      931 2024-04-07 10:42:36.000000 sphinx-github-style-1.2.1/sphinx_github_style/add_linkcode_class.py
--rw-rw-rw-   0        0        0     5464 2024-04-07 10:42:36.000000 sphinx-github-style-1.2.1/sphinx_github_style/github_style.py
--rw-rw-rw-   0        0        0     1977 2024-02-18 22:51:01.000000 sphinx-github-style-1.2.1/sphinx_github_style/lexer.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.084973 sphinx-github-style-1.2.1/sphinx_github_style/utils/
--rw-rw-rw-   0        0        0        0 2024-04-07 10:47:00.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-04-07 10:51:38.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/git.py
--rw-rw-rw-   0        0        0     4658 2024-04-07 10:57:21.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/linkcode.py
--rw-rw-rw-   0        0        0      733 2024-04-07 11:17:17.000000 sphinx-github-style-1.2.1/sphinx_github_style/utils/sphinx.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:29:53.069351 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/
--rw-rw-rw-   0        0        0     7123 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-04-07 11:29:53.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-07 11:29:52.000000 sphinx-github-style-1.2.1/sphinx_github_style.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 04:58:17.693663 sphinx-github-style-1.2.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-27 12:00:21.000000 sphinx-github-style-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7123 2024-05-15 04:58:17.693663 sphinx-github-style-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6373 2024-05-15 04:57:01.000000 sphinx-github-style-1.2.2/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-15 04:58:17.693663 sphinx-github-style-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1519 2024-01-21 05:39:18.000000 sphinx-github-style-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:58:17.673523 sphinx-github-style-1.2.2/sphinx_github_style/
+-rw-rw-rw-   0        0        0     1945 2024-05-15 04:55:10.000000 sphinx-github-style-1.2.2/sphinx_github_style/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:58:17.685583 sphinx-github-style-1.2.2/sphinx_github_style/_static/
+-rw-rw-rw-   0        0        0     1128 2023-08-25 05:08:55.000000 sphinx-github-style-1.2.2/sphinx_github_style/_static/github_style.css
+-rw-rw-rw-   0        0        0      931 2024-04-07 10:42:36.000000 sphinx-github-style-1.2.2/sphinx_github_style/add_linkcode_class.py
+-rw-rw-rw-   0        0        0     5464 2024-04-07 10:42:36.000000 sphinx-github-style-1.2.2/sphinx_github_style/github_style.py
+-rw-rw-rw-   0        0        0     1977 2024-02-18 22:51:01.000000 sphinx-github-style-1.2.2/sphinx_github_style/lexer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:58:17.685583 sphinx-github-style-1.2.2/sphinx_github_style/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-07 10:47:00.000000 sphinx-github-style-1.2.2/sphinx_github_style/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-04-07 10:51:38.000000 sphinx-github-style-1.2.2/sphinx_github_style/utils/git.py
+-rw-rw-rw-   0        0        0     4658 2024-04-07 10:57:21.000000 sphinx-github-style-1.2.2/sphinx_github_style/utils/linkcode.py
+-rw-rw-rw-   0        0        0      733 2024-05-15 04:54:57.000000 sphinx-github-style-1.2.2/sphinx_github_style/utils/sphinx.py
+drwxrwxrwx   0        0        0        0 2024-05-15 04:58:17.685583 sphinx-github-style-1.2.2/sphinx_github_style.egg-info/
+-rw-rw-rw-   0        0        0     7123 2024-05-15 04:58:17.000000 sphinx-github-style-1.2.2/sphinx_github_style.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-15 04:58:17.000000 sphinx-github-style-1.2.2/sphinx_github_style.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 04:58:17.000000 sphinx-github-style-1.2.2/sphinx_github_style.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-15 04:58:17.000000 sphinx-github-style-1.2.2/sphinx_github_style.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-15 04:58:17.000000 sphinx-github-style-1.2.2/sphinx_github_style.egg-info/top_level.txt
```

### Comparing `sphinx-github-style-1.2.1/LICENSE` & `sphinx-github-style-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/PKG-INFO` & `sphinx-github-style-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-github-style
-Version: 1.2.1
+Version: 1.2.2
 Summary: GitHub source code links and syntax highlighting for Sphinx documentation
 Home-page: https://github.com/tdkorn/sphinx-github-style
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-github-style/tarball/master
 Keywords: sphinx,sphinx-extension,sphinx-theme,pygments,pygments-style,github,linkcode
@@ -44,15 +44,15 @@
    :title: Sphinx Github Style
    :description: A Sphinx extension to add GitHub source code links and syntax highlighting
 
 
 sphinx-github-style - GitHub source code links and syntax highlighting for Sphinx documentation
 -------------------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/logo_pypi.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/logo_pypi.png
    :alt: Sphinx GitHub Style: GitHub Integration and Pygments Style for Sphinx Documentation
    :width: 50%
    :align: center
 
 
 
 
@@ -109,23 +109,23 @@
 
 Using |.sphinx.ext.linkcode|_,  a ``View on GitHub`` link is added to the documentation of every class, method, function, and property:
 
 |
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_link.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/github_link.png
    :alt: sphinx-github-style adds a "View on GitHub" link
 
 
 They link to and highlight the corresponding code block in your GitHub repository:
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_linked_code.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/github_linked_code.png
    :alt: The linked corresponding highlighted source code block on GitHub
 
 
 
 .. list-table::
    :header-rows: 1
    
@@ -138,15 +138,15 @@
 Syntax Highlighting
 ====================
 
 ``sphinx-github-style`` also contains a ``Pygments`` style to highlight code blocks similar to GitHub:
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/syntax_highlighting.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/syntax_highlighting.png
    :alt: A code block highlighted by the Pygments style. It looks identical to GitHub.
 
 
 
 Installation
 ~~~~~~~~~~~~~~~~
```

### Comparing `sphinx-github-style-1.2.1/README.rst` & `sphinx-github-style-1.2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    :title: Sphinx Github Style
    :description: A Sphinx extension to add GitHub source code links and syntax highlighting
 
 
 sphinx-github-style - GitHub source code links and syntax highlighting for Sphinx documentation
 -------------------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/logo_pypi.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/logo_pypi.png
    :alt: Sphinx GitHub Style: GitHub Integration and Pygments Style for Sphinx Documentation
    :width: 50%
    :align: center
 
 
 
 
@@ -91,23 +91,23 @@
 
 Using |.sphinx.ext.linkcode|_,  a ``View on GitHub`` link is added to the documentation of every class, method, function, and property:
 
 |
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_link.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/github_link.png
    :alt: sphinx-github-style adds a "View on GitHub" link
 
 
 They link to and highlight the corresponding code block in your GitHub repository:
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_linked_code.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/github_linked_code.png
    :alt: The linked corresponding highlighted source code block on GitHub
 
 
 
 .. list-table::
    :header-rows: 1
    
@@ -120,15 +120,15 @@
 Syntax Highlighting
 ====================
 
 ``sphinx-github-style`` also contains a ``Pygments`` style to highlight code blocks similar to GitHub:
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/syntax_highlighting.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/syntax_highlighting.png
    :alt: A code block highlighted by the Pygments style. It looks identical to GitHub.
 
 
 
 Installation
 ~~~~~~~~~~~~~~~~
```

### Comparing `sphinx-github-style-1.2.1/setup.py` & `sphinx-github-style-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/__init__.py` & `sphinx-github-style-1.2.2/sphinx_github_style/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sphinx
 from pathlib import Path
 from typing import Dict, Any
 from sphinx.application import Sphinx
 from .utils.sphinx import get_conf_val, set_conf_val
 from .utils.linkcode import get_linkcode_url, get_linkcode_revision, get_linkcode_resolve
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __author__ = 'Adam Korn <hello@dailykitten.net>'
 
 from .add_linkcode_class import add_linkcode_node_class
 from .github_style import GitHubStyle
 from .lexer import GitHubLexer
 
 
@@ -33,17 +33,19 @@
         print(
             "Function `linkcode_resolve` not found in ``conf.py``; "
             "using default function from ``sphinx_github_style``"
         )
         linkcode_func = get_linkcode_resolve(linkcode_url)
         set_conf_val(app, 'linkcode_resolve', linkcode_func)
 
+    if not get_conf_val(app, 'pygments_style'):
+        set_conf_val(app, 'pygments_style', 'sphinx_github_style.GitHubStyle')
+
     app.add_lexer('python', GitHubLexer)
     app.add_css_file('github_style.css')
-    app.config.pygments_style = 'sphinx_github_style.GitHubStyle'
 
     return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
 
 
 def add_static_path(app) -> None:
     """Add the path for the ``_static`` folder"""
     app.config.html_static_path.append(
```

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/_static/github_style.css` & `sphinx-github-style-1.2.2/sphinx_github_style/_static/github_style.css`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/add_linkcode_class.py` & `sphinx-github-style-1.2.2/sphinx_github_style/add_linkcode_class.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/github_style.py` & `sphinx-github-style-1.2.2/sphinx_github_style/github_style.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/lexer.py` & `sphinx-github-style-1.2.2/sphinx_github_style/lexer.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/utils/git.py` & `sphinx-github-style-1.2.2/sphinx_github_style/utils/git.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/utils/linkcode.py` & `sphinx-github-style-1.2.2/sphinx_github_style/utils/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style/utils/sphinx.py` & `sphinx-github-style-1.2.2/sphinx_github_style/utils/sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style.egg-info/PKG-INFO` & `sphinx-github-style-1.2.2/sphinx_github_style.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-github-style
-Version: 1.2.1
+Version: 1.2.2
 Summary: GitHub source code links and syntax highlighting for Sphinx documentation
 Home-page: https://github.com/tdkorn/sphinx-github-style
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-github-style/tarball/master
 Keywords: sphinx,sphinx-extension,sphinx-theme,pygments,pygments-style,github,linkcode
@@ -44,15 +44,15 @@
    :title: Sphinx Github Style
    :description: A Sphinx extension to add GitHub source code links and syntax highlighting
 
 
 sphinx-github-style - GitHub source code links and syntax highlighting for Sphinx documentation
 -------------------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/logo_pypi.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/logo_pypi.png
    :alt: Sphinx GitHub Style: GitHub Integration and Pygments Style for Sphinx Documentation
    :width: 50%
    :align: center
 
 
 
 
@@ -109,23 +109,23 @@
 
 Using |.sphinx.ext.linkcode|_,  a ``View on GitHub`` link is added to the documentation of every class, method, function, and property:
 
 |
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_link.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/github_link.png
    :alt: sphinx-github-style adds a "View on GitHub" link
 
 
 They link to and highlight the corresponding code block in your GitHub repository:
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/github_linked_code.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/github_linked_code.png
    :alt: The linked corresponding highlighted source code block on GitHub
 
 
 
 .. list-table::
    :header-rows: 1
    
@@ -138,15 +138,15 @@
 Syntax Highlighting
 ====================
 
 ``sphinx-github-style`` also contains a ``Pygments`` style to highlight code blocks similar to GitHub:
 
 
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.1/docs/source/_static/syntax_highlighting.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-github-style/v1.2.2/docs/source/_static/syntax_highlighting.png
    :alt: A code block highlighted by the Pygments style. It looks identical to GitHub.
 
 
 
 Installation
 ~~~~~~~~~~~~~~~~
```

### Comparing `sphinx-github-style-1.2.1/sphinx_github_style.egg-info/SOURCES.txt` & `sphinx-github-style-1.2.2/sphinx_github_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

