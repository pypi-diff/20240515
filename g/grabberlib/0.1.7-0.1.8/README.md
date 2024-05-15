# Comparing `tmp/grabberlib-0.1.7.tar.gz` & `tmp/grabberlib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.1.7.tar", max compression
+gzip compressed data, was "grabberlib-0.1.8.tar", max compression
```

## Comparing `grabberlib-0.1.7.tar` & `grabberlib-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.1.7/README.md
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.1.7/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     5270 2024-05-10 14:48:30.795989 grabberlib-0.1.7/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 14:35:12.060596 grabberlib-0.1.7/grabber/core/bot/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-10 12:20:10.885923 grabberlib-0.1.7/grabber/core/bot/core.py
--rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/exc.py
--rw-r--r--   0        0        0      772 2024-05-09 12:59:39.317729 grabberlib-0.1.7/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3320 2024-05-10 14:42:57.044880 grabberlib-0.1.7/grabber/core/sources/common.py
--rw-r--r--   0        0        0     3653 2024-05-09 13:30:04.157477 grabberlib-0.1.7/grabber/core/sources/everia.py
--rw-r--r--   0        0        0     2698 2024-05-10 12:33:08.173014 grabberlib-0.1.7/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     3218 2024-05-10 12:29:42.290554 grabberlib-0.1.7/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3409 2024-05-13 15:57:32.514304 grabberlib-0.1.7/grabber/core/sources/nudecosplay.py
--rw-r--r--   0        0        0     2818 2024-05-09 12:59:39.317729 grabberlib-0.1.7/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     2950 2024-05-10 12:23:01.737325 grabberlib-0.1.7/grabber/core/sources/xiuren.py
--rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    19423 2024-05-13 16:21:26.079038 grabberlib-0.1.7/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-05-13 16:21:30.398921 grabberlib-0.1.7/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.7/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1036 2024-05-13 16:21:33.986823 grabberlib-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.755675 grabberlib-0.1.8/README.md
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.755675 grabberlib-0.1.8/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     5403 2024-05-14 12:31:46.304901 grabberlib-0.1.8/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 14:35:12.060596 grabberlib-0.1.8/grabber/core/bot/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-10 12:20:10.885923 grabberlib-0.1.8/grabber/core/bot/core.py
+-rw-r--r--   0        0        0       65 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/exc.py
+-rw-r--r--   0        0        0      772 2024-05-09 12:59:39.317729 grabberlib-0.1.8/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3320 2024-05-10 14:42:57.044880 grabberlib-0.1.8/grabber/core/sources/common.py
+-rw-r--r--   0        0        0     3653 2024-05-09 13:30:04.157477 grabberlib-0.1.8/grabber/core/sources/everia.py
+-rw-r--r--   0        0        0     2698 2024-05-10 12:33:08.173014 grabberlib-0.1.8/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4156 2024-05-14 12:33:33.314298 grabberlib-0.1.8/grabber/core/sources/hotgirl_asia.py
+-rw-r--r--   0        0        0     3290 2024-05-14 12:17:41.832296 grabberlib-0.1.8/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3409 2024-05-13 15:57:32.514304 grabberlib-0.1.8/grabber/core/sources/nudecosplay.py
+-rw-r--r--   0        0        0     2818 2024-05-09 12:59:39.317729 grabberlib-0.1.8/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     2950 2024-05-10 12:23:01.737325 grabberlib-0.1.8/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    19475 2024-05-14 12:31:08.197949 grabberlib-0.1.8/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-05-14 12:37:11.872860 grabberlib-0.1.8/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-20 14:47:15.759675 grabberlib-0.1.8/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-14 12:37:16.236749 grabberlib-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 grabberlib-0.1.8/PKG-INFO
```

### Comparing `grabberlib-0.1.7/grabber/__main__.py` & `grabberlib-0.1.8/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/controllers/base.py` & `grabberlib-0.1.8/grabber/controllers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from cement import Controller, ex
 from telegraph import Telegraph
 
 from grabber.core.settings import TELEGRAPH_TOKEN
 from grabber.core.sources.common import get_sources_for_common
 from grabber.core.sources.everia import get_sources_for_everia
 from grabber.core.sources.graph import get_for_telegraph
+from grabber.core.sources.hotgirl_asia import get_sources_for_hotgirl_asia
 from grabber.core.sources.khd import get_sources_for_4khd
 from grabber.core.sources.nudecosplay import get_sources_for_nudecosplay
 from grabber.core.sources.xiuren import get_sources_for_xiuren
 from grabber.core.utils import upload_folders_to_telegraph
 
 from ..core.version import get_version
 
@@ -133,14 +134,15 @@
             "nudecosplay": get_sources_for_nudecosplay,
             "nudebird": get_sources_for_nudecosplay,
             "hotgirl": get_sources_for_nudecosplay,
             "everia": get_sources_for_everia,
             "bestgirlsexy": get_sources_for_common,
             "asigirl": get_sources_for_common,
             "cosplaytele": get_sources_for_common,
+            "hotgirl.asia": get_sources_for_hotgirl_asia,
         }
 
         if upload:
             upload_folders_to_telegraph(
                 folder_name=folder,
                 limit=limit,
                 send_to_channel=send_to_telegram,
```

### Comparing `grabberlib-0.1.7/grabber/core/bot/core.py` & `grabberlib-0.1.8/grabber/core/bot/core.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/settings.py` & `grabberlib-0.1.8/grabber/core/settings.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/sources/common.py` & `grabberlib-0.1.8/grabber/core/sources/common.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/sources/everia.py` & `grabberlib-0.1.8/grabber/core/sources/everia.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/sources/graph.py` & `grabberlib-0.1.8/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/sources/khd.py` & `grabberlib-0.1.8/grabber/core/sources/khd.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     tags, _ = get_tags(url, headers=headers, query=page_nav_query)
     return [a.attrs["href"] for a in tags if tags]
 
 
 def get_sources_for_4khd(
     sources: List[str],
     entity: str,
-    telegraph_client: Telegraph,
+    telegraph_client: Optional[Telegraph] = None,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
-    **kwargs,
+    is_tag: Optional[bool] = False,
+    limit: Optional[int] = None,
 ) -> None:
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
```

### Comparing `grabberlib-0.1.7/grabber/core/sources/nudecosplay.py` & `grabberlib-0.1.8/grabber/core/sources/nudecosplay.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/sources/xasiat.py` & `grabberlib-0.1.8/grabber/core/sources/xasiat.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/sources/xiuren.py` & `grabberlib-0.1.8/grabber/core/sources/xiuren.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.1.7/grabber/core/utils.py` & `grabberlib-0.1.8/grabber/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         "div.elementor-widget-container a[href^='https://terabox.com']",
         "href",
     ),
     "everia": ("div.entry-content img", "src"),
     "bestgirlsexy": ("div.elementor-widget-container p img", "data-src"),
     "asigirl": ("a.asigirl-item", "href"),
     "cosplaytele": ("img.attachment-full.size-full", "src"),
+    "hotgirl.asia": ("div.galeria_img img", "src"),
 }
 
 
 @dataclass(kw_only=True)
 class PaginationXPath:
     pagination_query: str
     pages_count_query: str
```

### Comparing `grabberlib-0.1.7/pyproject.toml` & `grabberlib-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.1.7/PKG-INFO` & `grabberlib-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

