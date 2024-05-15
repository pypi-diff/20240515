# Comparing `tmp/blurry_cli-0.8.1.tar.gz` & `tmp/blurry_cli-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurry_cli-0.8.1.tar", max compression
+gzip compressed data, was "blurry_cli-0.8.2.tar", max compression
```

## Comparing `blurry_cli-0.8.1.tar` & `blurry_cli-0.8.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/LICENSE
--rw-r--r--   0        0        0     1782 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/README.md
--rw-r--r--   0        0        0    10037 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/__init__.py
--rw-r--r--   0        0        0       32 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/__main__.py
--rw-r--r--   0        0        0      526 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/async_typer.py
--rw-r--r--   0        0        0     1009 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/cli.py
--rw-r--r--   0        0        0      111 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/constants.py
--rw-r--r--   0        0        0     3537 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/images.py
--rw-r--r--   0        0        0     7897 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/markdown/__init__.py
--rw-r--r--   0        0        0     1778 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/markdown/front_matter.py
--rw-r--r--   0        0        0        0 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/markdown/renderer_functions/__init__.py
--rw-r--r--   0        0        0      787 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/markdown/renderer_functions/render_video.py
--rw-r--r--   0        0        0     1993 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/open_graph.py
--rw-r--r--   0        0        0      349 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/html_plugins/__init__.py
--rw-r--r--   0        0        0     1124 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/html_plugins/minify_html_plugin.py
--rw-r--r--   0        0        0        0 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/jinja_plugins/__init__.py
--rw-r--r--   0        0        0     2614 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/jinja_plugins/blurry_image_extension.py
--rw-r--r--   0        0        0        0 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/markdown_plugins/__init__.py
--rw-r--r--   0        0        0     1119 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/markdown_plugins/container_plugin.py
--rw-r--r--   0        0        0      683 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/markdown_plugins/punctuation_plugin.py
--rw-r--r--   0        0        0     1509 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/plugins/markdown_plugins/python_code_plugin.py
--rw-r--r--   0        0        0        0 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/py.typed
--rw-r--r--   0        0        0     1817 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/schema_validation.py
--rw-r--r--   0        0        0     2347 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/settings.py
--rw-r--r--   0        0        0     1752 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/sitemap.py
--rw-r--r--   0        0        0      777 2024-04-28 14:56:29.077645 blurry_cli-0.8.1/blurry/types.py
--rw-r--r--   0        0        0     4376 2024-04-28 14:56:29.081645 blurry_cli-0.8.1/blurry/utils.py
--rw-r--r--   0        0        0     2355 2024-04-28 14:56:29.081645 blurry_cli-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 blurry_cli-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1782 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/README.md
+-rw-r--r--   0        0        0    10037 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/__main__.py
+-rw-r--r--   0        0        0      526 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/async_typer.py
+-rw-r--r--   0        0        0     1009 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/cli.py
+-rw-r--r--   0        0        0      111 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/constants.py
+-rw-r--r--   0        0        0     3537 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/images.py
+-rw-r--r--   0        0        0     7756 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/markdown/__init__.py
+-rw-r--r--   0        0        0     1778 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/markdown/front_matter.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/markdown/renderer_functions/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/markdown/renderer_functions/render_video.py
+-rw-r--r--   0        0        0     1993 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/open_graph.py
+-rw-r--r--   0        0        0      349 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/html_plugins/__init__.py
+-rw-r--r--   0        0        0     1124 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/html_plugins/minify_html_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/jinja_plugins/__init__.py
+-rw-r--r--   0        0        0     2764 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/jinja_plugins/blurry_image_extension.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/markdown_plugins/__init__.py
+-rw-r--r--   0        0        0     1119 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/markdown_plugins/container_plugin.py
+-rw-r--r--   0        0        0      683 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/markdown_plugins/punctuation_plugin.py
+-rw-r--r--   0        0        0     1509 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/plugins/markdown_plugins/python_code_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/py.typed
+-rw-r--r--   0        0        0     1817 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/schema_validation.py
+-rw-r--r--   0        0        0     2347 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/settings.py
+-rw-r--r--   0        0        0     1752 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/sitemap.py
+-rw-r--r--   0        0        0      777 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/types.py
+-rw-r--r--   0        0        0     3783 2024-05-15 12:07:13.653983 blurry_cli-0.8.2/blurry/utils.py
+-rw-r--r--   0        0        0     2355 2024-05-15 12:07:13.657983 blurry_cli-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 blurry_cli-0.8.2/PKG-INFO
```

### Comparing `blurry_cli-0.8.1/LICENSE` & `blurry_cli-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/README.md` & `blurry_cli-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/__init__.py` & `blurry_cli-0.8.2/blurry/__init__.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/async_typer.py` & `blurry_cli-0.8.2/blurry/async_typer.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/cli.py` & `blurry_cli-0.8.2/blurry/cli.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/images.py` & `blurry_cli-0.8.2/blurry/images.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/markdown/__init__.py` & `blurry_cli-0.8.2/blurry/markdown/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from blurry.plugins import discovered_markdown_plugins
 from blurry.settings import get_content_directory
 from blurry.settings import SETTINGS
 from blurry.types import is_str
 from blurry.utils import content_path_to_url
 from blurry.utils import convert_relative_path_in_markdown_file_to_pathname
 from blurry.utils import path_to_url_pathname
-from blurry.utils import remove_lazy_loading_from_first_image
 from blurry.utils import resolve_relative_path_in_markdown
 
 
 # https://schema.org/ImageObject
 ImageObject: TypeAlias = dict
 
 
@@ -174,17 +173,14 @@
     initial_state.env["__file__"] = str(filepath)  # type: ignore
     markdown_text, state = parse_front_matter(markdown, state=initial_state)
     html, state = markdown.parse(markdown_text, state=state)
 
     if not is_str(html):
         raise Exception(f"Expected html to be a string but got: {type(html)}")
 
-    # Post-process HTML
-    html = remove_lazy_loading_from_first_image(html)
-
     # Seed front_matter with schema_data from config file
     front_matter: dict[str, Any] = dict(SETTINGS.get("SCHEMA_DATA", {}))
     front_matter.update(state.env.get("front_matter", {}))
 
     # Add inferred/computed/relative values
     # https://schema.org/image
     # https://schema.org/thumbnailUrl
```

### Comparing `blurry_cli-0.8.1/blurry/markdown/front_matter.py` & `blurry_cli-0.8.2/blurry/markdown/front_matter.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/markdown/renderer_functions/render_video.py` & `blurry_cli-0.8.2/blurry/markdown/renderer_functions/render_video.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/open_graph.py` & `blurry_cli-0.8.2/blurry/open_graph.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/plugins/html_plugins/minify_html_plugin.py` & `blurry_cli-0.8.2/blurry/plugins/html_plugins/minify_html_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/plugins/jinja_plugins/blurry_image_extension.py` & `blurry_cli-0.8.2/blurry/plugins/jinja_plugins/blurry_image_extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from jinja2_simple_tags import StandaloneTag
 from rich.console import Console
 from wand.exceptions import BlobError
 from wand.image import Image
 
 from blurry.images import add_image_width_to_path
 from blurry.settings import get_build_directory
+from blurry.settings import get_content_directory
 from blurry.utils import build_path_to_url
 
 warning_console = Console(stderr=True, style="bold yellow")
 
 
 class BlurryImage(StandaloneTag):
     safe_output = True
@@ -21,24 +22,25 @@
     def render(self, *args, **kwargs):
         if len(args) == 2:
             (image_url, width) = args
         else:
             image_url = args[0]
             width = None
 
-        image_content_path: str = "." + urlparse(image_url).path
-        image_path = get_build_directory() / image_content_path
+        image_relative_pathname = "." + urlparse(image_url).path
+        image_content_path = get_content_directory() / image_relative_pathname
+        image_path = get_build_directory() / image_relative_pathname
 
         try:
-            with Image(filename=str(image_path)) as image:
+            with Image(filename=str(image_content_path)) as image:
                 image_width = image.width
                 image_height = image.height
                 image_mimetype = image.mimetype
         except BlobError:
-            warning_console.print(f"Could not find image: {image_path}")
+            warning_console.print(f"Could not find image: {image_content_path}")
             return ""
 
         attributes = {
             "width": image_width,
             "height": image_height,
         }
         for attribute_key in kwargs:
```

### Comparing `blurry_cli-0.8.1/blurry/plugins/markdown_plugins/container_plugin.py` & `blurry_cli-0.8.2/blurry/plugins/markdown_plugins/container_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/plugins/markdown_plugins/punctuation_plugin.py` & `blurry_cli-0.8.2/blurry/plugins/markdown_plugins/punctuation_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/plugins/markdown_plugins/python_code_plugin.py` & `blurry_cli-0.8.2/blurry/plugins/markdown_plugins/python_code_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/schema_validation.py` & `blurry_cli-0.8.2/blurry/schema_validation.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/settings.py` & `blurry_cli-0.8.2/blurry/settings.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/sitemap.py` & `blurry_cli-0.8.2/blurry/sitemap.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/types.py` & `blurry_cli-0.8.2/blurry/types.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.8.1/blurry/utils.py` & `blurry_cli-0.8.2/blurry/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from pathlib import Path
 
-from selectolax.parser import HTMLParser
-
 from blurry.settings import get_build_directory
 from blurry.settings import get_content_directory
 from blurry.settings import SETTINGS
 from blurry.types import DirectoryFileData
 
 
 def get_domain_with_scheme():
@@ -112,23 +110,7 @@
     return directory_file_data
 
 
 def format_schema_data(schema_data: dict) -> dict:
     formatted_schema_data = {"@context": "https://schema.org"}
     formatted_schema_data.update(schema_data)
     return formatted_schema_data
-
-
-def remove_lazy_loading_from_first_image(html: str) -> str:
-    parser = HTMLParser(html, use_meta_tags=False)
-    if not parser.body or not parser.body.html:
-        raise Exception("Could not parse HTML")
-    first_img_tag = parser.css_first("img")
-    if not first_img_tag:
-        return html
-    updated_tag = first_img_tag
-    try:
-        del updated_tag.attrs["loading"]  # type: ignore
-        first_img_tag.replace_with(HTMLParser(updated_tag.html).body.child)  # type: ignore
-    except KeyError:
-        pass
-    return parser.body.html
```

### Comparing `blurry_cli-0.8.1/pyproject.toml` & `blurry_cli-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blurry-cli"
-version = "0.8.1"
+version = "0.8.2"
 description = "A Mistune-based static site generator for Python"
 authors = ["John Franey <franey@duck.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blurry-dev/blurry"
 keywords = ["static-site-generator", "seo", "pagespeed"]
 classifiers = [
```

### Comparing `blurry_cli-0.8.1/PKG-INFO` & `blurry_cli-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurry-cli
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Mistune-based static site generator for Python
 Home-page: https://github.com/blurry-dev/blurry
 License: MIT
 Keywords: static-site-generator,seo,pagespeed
 Author: John Franey
 Author-email: franey@duck.com
 Requires-Python: >=3.10,<4.0
```

