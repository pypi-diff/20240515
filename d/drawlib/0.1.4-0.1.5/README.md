# Comparing `tmp/drawlib-0.1.4.tar.gz` & `tmp/drawlib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawlib-0.1.4.tar", max compression
+gzip compressed data, was "drawlib-0.1.5.tar", max compression
```

## Comparing `drawlib-0.1.4.tar` & `drawlib-0.1.5.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.4/README.md
--rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.4/drawlib/.pylintrc
--rw-r--r--   0        0        0     1039 2024-05-12 02:04:42.720811 drawlib-0.1.4/drawlib/__init__.py
--rw-r--r--   0        0        0      688 2024-04-06 11:43:47.512263 drawlib-0.1.4/drawlib/__main__.py
--rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.4/drawlib/apis.py
--rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.4/drawlib/assets/__init__.py
--rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.4/drawlib/assets/v0_1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.4/drawlib/assets/v0_1/fonticons/__init__.py
--rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.4/drawlib/assets/v0_1/fonts/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.4/drawlib/v0_1/__init__.py
--rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.4/drawlib/v0_1/__main__.py
--rw-r--r--   0        0        0     2437 2024-05-04 13:37:40.227151 drawlib-0.1.4/drawlib/v0_1/apis.py
--rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.4/drawlib/v0_1/private/__init__.py
--rw-r--r--   0        0        0     5949 2024-04-27 06:45:13.999149 drawlib-0.1.4/drawlib/v0_1/private/arg_validator.py
--rw-r--r--   0        0        0     6207 2024-04-27 06:44:59.377242 drawlib-0.1.4/drawlib/v0_1/private/command.py
--rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.4/drawlib/v0_1/private/core/__init__.py
--rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.4/drawlib/v0_1/private/core/colors.py
--rw-r--r--   0        0        0    13577 2024-04-28 11:41:37.164049 drawlib-0.1.4/drawlib/v0_1/private/core/dimage.py
--rw-r--r--   0        0        0    14228 2024-05-01 15:22:54.625259 drawlib-0.1.4/drawlib/v0_1/private/core/fonts.py
--rw-r--r--   0        0        0    32410 2024-05-11 15:17:05.404584 drawlib-0.1.4/drawlib/v0_1/private/core/model.py
--rw-r--r--   0        0        0     7060 2024-04-27 01:01:21.281062 drawlib-0.1.4/drawlib/v0_1/private/core/model_validator.py
--rw-r--r--   0        0        0    49184 2024-05-12 01:39:42.759450 drawlib-0.1.4/drawlib/v0_1/private/core/theme.py
--rw-r--r--   0        0        0    26316 2024-05-01 14:16:45.894958 drawlib-0.1.4/drawlib/v0_1/private/core/util.py
--rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/__init__.py
--rw-r--r--   0        0        0    20400 2024-05-11 17:25:26.212255 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/base.py
--rw-r--r--   0        0        0     2328 2024-04-29 17:11:04.449382 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/canvas.py
--rw-r--r--   0        0        0     5297 2024-05-12 01:03:24.423089 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/image.py
--rw-r--r--   0        0        0     8444 2024-05-12 00:55:21.009215 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/line.py
--rw-r--r--   0        0        0     5051 2024-05-12 00:48:19.055312 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_arrow.py
--rw-r--r--   0        0        0    20315 2024-05-12 00:50:38.663131 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_polygon.py
--rw-r--r--   0        0        0    20051 2024-05-12 00:41:36.243898 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/patches.py
--rw-r--r--   0        0        0     3862 2024-04-29 17:10:15.748016 drawlib-0.1.4/drawlib/v0_1/private/core_canvas/text.py
--rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.4/drawlib/v0_1/private/download.py
--rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.4/drawlib/v0_1/private/dutil.py
--rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.4/drawlib/v0_1/private/icons/__init__.py
--rw-r--r--   0        0        0   901217 2024-05-12 01:55:52.732933 drawlib-0.1.4/drawlib/v0_1/private/icons/phosphor.py
--rw-r--r--   0        0        0     2705 2024-05-12 01:58:41.948187 drawlib-0.1.4/drawlib/v0_1/private/icons/util.py
--rw-r--r--   0        0        0     1206 2024-04-27 06:44:36.108567 drawlib-0.1.4/drawlib/v0_1/private/logging.py
--rw-r--r--   0        0        0     6687 2024-05-02 12:04:01.063777 drawlib-0.1.4/drawlib/v0_1/private/settings.py
--rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.4/drawlib/v0_1/private/smartarts/__init__.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.4/drawlib/v0_1/private/smartarts/cycle.py
--rw-r--r--   0        0        0      617 2024-04-14 10:51:41.389757 drawlib-0.1.4/drawlib/v0_1/private/smartarts/dsart.py
--rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.4/drawlib/v0_1/private/smartarts/groups.py
--rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.4/drawlib/v0_1/private/smartarts/pyramid.py
--rw-r--r--   0        0        0     6787 2024-05-01 15:20:41.772611 drawlib-0.1.4/drawlib/v0_1/private/smartarts/sourcecode.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.4/drawlib/v0_1/private/smartarts/table.py
--rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.4/drawlib/v0_1/private/smartarts/tree.py
--rw-r--r--   0        0        0     5807 2024-04-27 01:15:26.015254 drawlib-0.1.4/drawlib/v0_1/private/tools.py
--rw-r--r--   0        0        0    10163 2024-05-02 13:00:08.257932 drawlib-0.1.4/drawlib/v0_1/private/util.py
--rw-r--r--   0        0        0      758 2024-05-12 02:05:22.899811 drawlib-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.5/README.md
+-rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.5/drawlib/.pylintrc
+-rw-r--r--   0        0        0     1039 2024-05-12 02:06:34.115175 drawlib-0.1.5/drawlib/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-06 11:43:47.512263 drawlib-0.1.5/drawlib/__main__.py
+-rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.5/drawlib/apis.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.5/drawlib/assets/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.5/drawlib/assets/v0_1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.5/drawlib/assets/v0_1/fonticons/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.5/drawlib/assets/v0_1/fonts/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.5/drawlib/v0_1/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.5/drawlib/v0_1/__main__.py
+-rw-r--r--   0        0        0     2437 2024-05-04 13:37:40.227151 drawlib-0.1.5/drawlib/v0_1/apis.py
+-rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.5/drawlib/v0_1/private/__init__.py
+-rw-r--r--   0        0        0     5949 2024-04-27 06:45:13.999149 drawlib-0.1.5/drawlib/v0_1/private/arg_validator.py
+-rw-r--r--   0        0        0     6207 2024-04-27 06:44:59.377242 drawlib-0.1.5/drawlib/v0_1/private/command.py
+-rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.5/drawlib/v0_1/private/core/__init__.py
+-rw-r--r--   0        0        0    12776 2024-04-23 00:24:17.718876 drawlib-0.1.5/drawlib/v0_1/private/core/colors.py
+-rw-r--r--   0        0        0    13577 2024-04-28 11:41:37.164049 drawlib-0.1.5/drawlib/v0_1/private/core/dimage.py
+-rw-r--r--   0        0        0    14625 2024-05-15 13:23:29.613225 drawlib-0.1.5/drawlib/v0_1/private/core/fonts.py
+-rw-r--r--   0        0        0    32410 2024-05-11 15:17:05.404584 drawlib-0.1.5/drawlib/v0_1/private/core/model.py
+-rw-r--r--   0        0        0     7060 2024-04-27 01:01:21.281062 drawlib-0.1.5/drawlib/v0_1/private/core/model_validator.py
+-rw-r--r--   0        0        0    16776 2024-05-15 02:16:15.760375 drawlib-0.1.5/drawlib/v0_1/private/core/theme.py
+-rw-r--r--   0        0        0    11892 2024-05-15 02:28:43.559352 drawlib-0.1.5/drawlib/v0_1/private/core/theme_officials.py
+-rw-r--r--   0        0        0    51240 2024-05-15 02:07:29.794753 drawlib-0.1.5/drawlib/v0_1/private/core/theme_styles.py
+-rw-r--r--   0        0        0    26318 2024-05-15 01:22:19.949970 drawlib-0.1.5/drawlib/v0_1/private/core/util.py
+-rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/__init__.py
+-rw-r--r--   0        0        0    16947 2024-05-15 05:40:26.581031 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/base.py
+-rw-r--r--   0        0        0     7915 2024-05-15 05:52:41.212524 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/canvas.py
+-rw-r--r--   0        0        0     5304 2024-05-15 00:05:43.225865 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/image.py
+-rw-r--r--   0        0        0     8496 2024-05-15 00:08:44.285403 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/line.py
+-rw-r--r--   0        0        0     5347 2024-05-15 04:10:20.846079 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/original_arrow.py
+-rw-r--r--   0        0        0    22449 2024-05-15 04:12:26.141167 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/original_polygon.py
+-rw-r--r--   0        0        0    22935 2024-05-15 04:15:18.818992 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/patches.py
+-rw-r--r--   0        0        0     4073 2024-05-15 01:17:52.844301 drawlib-0.1.5/drawlib/v0_1/private/core_canvas/text.py
+-rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.5/drawlib/v0_1/private/download.py
+-rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.5/drawlib/v0_1/private/dutil.py
+-rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.5/drawlib/v0_1/private/icons/__init__.py
+-rw-r--r--   0        0        0   901219 2024-05-15 01:19:30.023797 drawlib-0.1.5/drawlib/v0_1/private/icons/phosphor.py
+-rw-r--r--   0        0        0     2707 2024-05-15 01:20:36.171244 drawlib-0.1.5/drawlib/v0_1/private/icons/util.py
+-rw-r--r--   0        0        0     1206 2024-04-27 06:44:36.108567 drawlib-0.1.5/drawlib/v0_1/private/logging.py
+-rw-r--r--   0        0        0     6687 2024-05-02 12:04:01.063777 drawlib-0.1.5/drawlib/v0_1/private/settings.py
+-rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.5/drawlib/v0_1/private/smartarts/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.5/drawlib/v0_1/private/smartarts/cycle.py
+-rw-r--r--   0        0        0      617 2024-04-14 10:51:41.389757 drawlib-0.1.5/drawlib/v0_1/private/smartarts/dsart.py
+-rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.5/drawlib/v0_1/private/smartarts/groups.py
+-rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.5/drawlib/v0_1/private/smartarts/pyramid.py
+-rw-r--r--   0        0        0     5905 2024-05-15 01:26:18.168883 drawlib-0.1.5/drawlib/v0_1/private/smartarts/sourcecode.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.5/drawlib/v0_1/private/smartarts/table.py
+-rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.5/drawlib/v0_1/private/smartarts/tree.py
+-rw-r--r--   0        0        0     5807 2024-04-27 01:15:26.015254 drawlib-0.1.5/drawlib/v0_1/private/tools.py
+-rw-r--r--   0        0        0    10163 2024-05-02 13:00:08.257932 drawlib-0.1.5/drawlib/v0_1/private/util.py
+-rw-r--r--   0        0        0      758 2024-05-15 13:27:11.092581 drawlib-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.5/PKG-INFO
```

### Comparing `drawlib-0.1.4/LICENSE.txt` & `drawlib-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/README.md` & `drawlib-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/__init__.py` & `drawlib-0.1.5/drawlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 - drawlib.v0_1: API v0.1 interface (latest)
 
 """
 
 from typing import Final
 
 # please update here when you release new version
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 
 # might not be changed
 LIB_NAME: Final[str] = "drawlib"
 AUTHOR: Final[str] = "Yuichi Ito"
 CONTACT: Final[str] = "yuichi@yuichi.com"
 __version__: Final[str] = VERSION
```

### Comparing `drawlib-0.1.4/drawlib/__main__.py` & `drawlib-0.1.5/drawlib/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/apis.py` & `drawlib-0.1.5/drawlib/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/__init__.py` & `drawlib-0.1.5/drawlib/v0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/__main__.py` & `drawlib-0.1.5/drawlib/v0_1/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/apis.py` & `drawlib-0.1.5/drawlib/v0_1/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/__init__.py` & `drawlib-0.1.5/drawlib/v0_1/private/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/arg_validator.py` & `drawlib-0.1.5/drawlib/v0_1/private/arg_validator.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/command.py` & `drawlib-0.1.5/drawlib/v0_1/private/command.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core/__init__.py` & `drawlib-0.1.5/drawlib/v0_1/private/core/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core/colors.py` & `drawlib-0.1.5/drawlib/v0_1/private/core/colors.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core/dimage.py` & `drawlib-0.1.5/drawlib/v0_1/private/core/dimage.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core/fonts.py` & `drawlib-0.1.5/drawlib/v0_1/private/core/fonts.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,22 +47,22 @@
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     # sansserif
-    SANSSERIF_LIGHT = get_fontfile_tuple("noto_sansserif_cjk/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
-    SANSSERIF_REGULAR = get_fontfile_tuple("noto_sansserif_cjk/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
-    SANSSERIF_BOLD = get_fontfile_tuple("noto_sansserif_cjk/bold.otf", "64d01f4e75814352cc9dea68074f4067")
+    SANSSERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_sans/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
+    SANSSERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_sans/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
+    SANSSERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_sans/bold.otf", "64d01f4e75814352cc9dea68074f4067")
 
     # serif
-    SERIF_LIGHT = get_fontfile_tuple("noto_serif_cjk/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
-    SERIF_REGULAR = get_fontfile_tuple("noto_serif_cjk/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
-    SERIF_BOLD = get_fontfile_tuple("noto_serif_cjk/bold.otf", "ea7175c0325777d126622340f9c94a66")
+    SERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_serif/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
+    SERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_serif/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
+    SERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_serif/bold.otf", "ea7175c0325777d126622340f9c94a66")
 
     # roboto
     ROBOTO_LIGHT = get_fontfile_tuple("roboto/light.ttf", "881e150ab929e26d1f812c4342c15a7c")
     ROBOTO_REGULAR = get_fontfile_tuple("roboto/regular.ttf", "8a36205bd9b83e03af0591a004bc97f4")
     ROBOTO_BOLD = get_fontfile_tuple("roboto/bold.ttf", "b8e42971dec8d49207a8c8e2b919a6ac")
 
 
@@ -104,169 +104,172 @@
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
-    # nontserrat
-    MONTSERRAT_LIGHT = get_fontfile_tuple("monstserrat/light.ttf", "94fbe93542f684134cad1d775947ca92")
-    MONTSERRAT_REGULAR = get_fontfile_tuple("monstserrat/regular.ttf", "5e077c15f6e1d334dd4e9be62b28ac75")
-    MONTSERRAT_BOLD = get_fontfile_tuple("monstserrat/bold.ttf", "ed86af2ed5bbaf879e9f2ec2e2eac929")
-
     # lato
-    LATO_LIGHT = get_fontfile_tuple("lato/light.ttf", "2bcc211c05fc425a57b2767a4cdcf174")
-    LATO_REGULAR = get_fontfile_tuple("lato/regular.ttf", "122dd68d69fe9587e062d20d9ff5de2a")
-    LATO_BOLD = get_fontfile_tuple("lato/bold.ttf", "24b516c266d7341c954cb2918f1c8f38")
-
-    # raleways
-    RALEWAYS_LIGHT = get_fontfile_tuple("raleways/light.ttf", "a36750fa9f5530b0c2760267df04ae37")
-    RALEWAYS_REGULAR = get_fontfile_tuple("raleways/regular.ttf", "d95649da7dfb965a289ac29105ce8771")
-    RALEWAYS_BOLD = get_fontfile_tuple("raleways/bold.ttf", "21c82294041b1504a5cbe4f566c8acd6")
+    LATO_LIGHT = get_fontfile_tuple("sans_lato/light.ttf", "2bcc211c05fc425a57b2767a4cdcf174")
+    LATO_REGULAR = get_fontfile_tuple("sans_lato/regular.ttf", "122dd68d69fe9587e062d20d9ff5de2a")
+    LATO_BOLD = get_fontfile_tuple("sans_lato/bold.ttf", "24b516c266d7341c954cb2918f1c8f38")
+
+    # montserrat
+    MONTSERRAT_LIGHT = get_fontfile_tuple("sans_monstserrat/light.ttf", "94fbe93542f684134cad1d775947ca92")
+    MONTSERRAT_REGULAR = get_fontfile_tuple("sans_monstserrat/regular.ttf", "5e077c15f6e1d334dd4e9be62b28ac75")
+    MONTSERRAT_BOLD = get_fontfile_tuple("sans_monstserrat/bold.ttf", "ed86af2ed5bbaf879e9f2ec2e2eac929")
 
     # oswald
-    OSWALD_LIGHT = get_fontfile_tuple("oswald/light.ttf", "fb3af9a7ffb259726bb3cb30b74ab7dc")
-    OSWALD_REGULAR = get_fontfile_tuple("oswald/regular.ttf", "b299a657c45aa257f1458b327f491bfb")
-    OSWALD_BOLD = get_fontfile_tuple("oswald/bold.ttf", "c95751378db3c5c8bfd993b164e13422")
+    OSWALD_LIGHT = get_fontfile_tuple("sans_oswald/light.ttf", "fb3af9a7ffb259726bb3cb30b74ab7dc")
+    OSWALD_REGULAR = get_fontfile_tuple("sans_oswald/regular.ttf", "b299a657c45aa257f1458b327f491bfb")
+    OSWALD_BOLD = get_fontfile_tuple("sans_oswald/bold.ttf", "c95751378db3c5c8bfd993b164e13422")
 
     # poppins
-    POPPINS_LIGHT = get_fontfile_tuple("poppins/light.ttf", "fcc40ae9a542d001971e53eaed948410")
-    POPPINS_REGULAR = get_fontfile_tuple("poppins/regular.ttf", "093ee89be9ede30383f39a899c485a82")
-    POPPINS_BOLD = get_fontfile_tuple("poppins/bold.ttf", "08c20a487911694291bd8c5de41315ad")
+    POPPINS_LIGHT = get_fontfile_tuple("sans_poppins/light.ttf", "fcc40ae9a542d001971e53eaed948410")
+    POPPINS_REGULAR = get_fontfile_tuple("sans_poppins/regular.ttf", "093ee89be9ede30383f39a899c485a82")
+    POPPINS_BOLD = get_fontfile_tuple("sans_poppins/bold.ttf", "08c20a487911694291bd8c5de41315ad")
+
+    # raleways
+    RALEWAYS_LIGHT = get_fontfile_tuple("sans_raleways/light.ttf", "a36750fa9f5530b0c2760267df04ae37")
+    RALEWAYS_REGULAR = get_fontfile_tuple("sans_raleways/regular.ttf", "d95649da7dfb965a289ac29105ce8771")
+    RALEWAYS_BOLD = get_fontfile_tuple("sans_raleways/bold.ttf", "21c82294041b1504a5cbe4f566c8acd6")
 
 
 class FontSerif(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     # courier
-    COURIER_REGULAR = get_fontfile_tuple("courier/regular.ttf", "fba4686ed1d1b4ef05ab14db78805dbe")
-    COURIER_BOLD = get_fontfile_tuple("courier/bold.ttf", "4acfa45d29d240044e0075a8e58f0862")
+    COURIER_REGULAR = get_fontfile_tuple("mono_courier/regular.ttf", "fba4686ed1d1b4ef05ab14db78805dbe")
+    COURIER_BOLD = get_fontfile_tuple("mono_courier/bold.ttf", "4acfa45d29d240044e0075a8e58f0862")
 
     # merriweather
-    MERRIWEATHER_LIGHT = get_fontfile_tuple("merriweather/light.ttf", "eccb6c6a243a3d44219648b6cdbc58ce")
-    MERRIWEATHER_REGULAR = get_fontfile_tuple("merriweather/regular.ttf", "e2f219e63a575a41e10f991e9c95819a")
-    MERRIWEATHER_BOLD = get_fontfile_tuple("merriweather/bold.ttf", "79ea53fed59f391498dfc6f2fbea97c2")
-
-    # playfairdisplay
-    PLAYFAIRDISPLAY_REGULAR = get_fontfile_tuple("playfairdisplay/regular.ttf", "1a28efdbd2876d90e554a67faabad24b")
-    PLAYFAIRDISPLAY_BOLD = get_fontfile_tuple("playfairdisplay/bold.ttf", "9b38798112efb7cf6eca1de031cec4ca")
+    MERRIWEATHER_LIGHT = get_fontfile_tuple("serif_merriweather/light.ttf", "eccb6c6a243a3d44219648b6cdbc58ce")
+    MERRIWEATHER_REGULAR = get_fontfile_tuple("serif_merriweather/regular.ttf", "e2f219e63a575a41e10f991e9c95819a")
+    MERRIWEATHER_BOLD = get_fontfile_tuple("serif_merriweather/bold.ttf", "79ea53fed59f391498dfc6f2fbea97c2")
 
     # platypi
-    PLATYPI_LIGHT = get_fontfile_tuple("platypi/light.ttf", "113ff25ffa6c98594583200398ab5c71")
-    PLATYPI_REGULAR = get_fontfile_tuple("platypi/regular.ttf", "a7f199dd97ff6567df8978b579213e3d")
-    PLATYPI_BOLD = get_fontfile_tuple("platypi/bold.ttf", "344e0525c3f473c8959c66e1df44e2e1")
+    PLATYPI_LIGHT = get_fontfile_tuple("serif_platypi/light.ttf", "113ff25ffa6c98594583200398ab5c71")
+    PLATYPI_REGULAR = get_fontfile_tuple("serif_platypi/regular.ttf", "a7f199dd97ff6567df8978b579213e3d")
+    PLATYPI_BOLD = get_fontfile_tuple("serif_platypi/bold.ttf", "344e0525c3f473c8959c66e1df44e2e1")
+
+    # playfairdisplay
+    PLAYFAIRDISPLAY_REGULAR = get_fontfile_tuple(
+        "serif_playfairdisplay/regular.ttf",
+        "1a28efdbd2876d90e554a67faabad24b",
+    )
+    PLAYFAIRDISPLAY_BOLD = get_fontfile_tuple("serif_playfairdisplay/bold.ttf", "9b38798112efb7cf6eca1de031cec4ca")
 
 
 class FontJapanese(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     # sansserif
-    SANSSERIF_LIGHT = get_fontfile_tuple("noto_sansserif_cjk/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
-    SANSSERIF_REGULAR = get_fontfile_tuple("noto_sansserif_cjk/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
-    SANSSERIF_BOLD = get_fontfile_tuple("noto_sansserif_cjk/bold.otf", "64d01f4e75814352cc9dea68074f4067")
+    SANSSERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_sans/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
+    SANSSERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_sans/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
+    SANSSERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_sans/bold.otf", "64d01f4e75814352cc9dea68074f4067")
 
     # serif
-    SERIF_LIGHT = get_fontfile_tuple("noto_serif_cjk/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
-    SERIF_REGULAR = get_fontfile_tuple("noto_serif_cjk/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
-    SERIF_BOLD = get_fontfile_tuple("noto_serif_cjk/bold.otf", "ea7175c0325777d126622340f9c94a66")
+    SERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_serif/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
+    SERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_serif/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
+    SERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_serif/bold.otf", "ea7175c0325777d126622340f9c94a66")
 
     # mplus1p
-    MPLUS1P_LIGHT = get_fontfile_tuple("mplus_1p/light.ttf", "01fea1cae2979588652514d83e9c0423")
-    MPLUS1P_REGULAR = get_fontfile_tuple("mplus_1p/regular.ttf", "bfab3ff358a7fa14c5703ad49063cb16")
-    MPLUS1P_BOLD = get_fontfile_tuple("mplus_1p/bold.ttf", "aa140061f44d0dda19ab2573a0ad93d3")
+    MPLUS1P_LIGHT = get_fontfile_tuple("japanese_mplus_1p/light.ttf", "01fea1cae2979588652514d83e9c0423")
+    MPLUS1P_REGULAR = get_fontfile_tuple("japanese_mplus_1p/regular.ttf", "bfab3ff358a7fa14c5703ad49063cb16")
+    MPLUS1P_BOLD = get_fontfile_tuple("japanese_mplus_1p/bold.ttf", "aa140061f44d0dda19ab2573a0ad93d3")
 
 
 class FontKorean(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     # sansserif
-    SANSSERIF_LIGHT = get_fontfile_tuple("noto_sansserif_cjk/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
-    SANSSERIF_REGULAR = get_fontfile_tuple("noto_sansserif_cjk/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
-    SANSSERIF_BOLD = get_fontfile_tuple("noto_sansserif_cjk/bold.otf", "64d01f4e75814352cc9dea68074f4067")
+    SANSSERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_sans/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
+    SANSSERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_sans/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
+    SANSSERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_sans/bold.otf", "64d01f4e75814352cc9dea68074f4067")
 
     # serif
-    SERIF_LIGHT = get_fontfile_tuple("noto_serif_cjk/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
-    SERIF_REGULAR = get_fontfile_tuple("noto_serif_cjk/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
-    SERIF_BOLD = get_fontfile_tuple("noto_serif_cjk/bold.otf", "ea7175c0325777d126622340f9c94a66")
+    SERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_serif/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
+    SERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_serif/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
+    SERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_serif/bold.otf", "ea7175c0325777d126622340f9c94a66")
 
 
 class FontChinese(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     # sansserif
-    SANSSERIF_LIGHT = get_fontfile_tuple("noto_sansserif_cjk/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
-    SANSSERIF_REGULAR = get_fontfile_tuple("noto_sansserif_cjk/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
-    SANSSERIF_BOLD = get_fontfile_tuple("noto_sansserif_cjk/bold.otf", "64d01f4e75814352cc9dea68074f4067")
+    SANSSERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_sans/light.otf", "88ce9ab7e76fed605c822b52605ac2fd")
+    SANSSERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_sans/regular.otf", "6d57a40c6695bd46457315e2a9dc757a")
+    SANSSERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_sans/bold.otf", "64d01f4e75814352cc9dea68074f4067")
 
     # serif
-    SERIF_LIGHT = get_fontfile_tuple("noto_serif_cjk/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
-    SERIF_REGULAR = get_fontfile_tuple("noto_serif_cjk/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
-    SERIF_BOLD = get_fontfile_tuple("noto_serif_cjk/bold.otf", "ea7175c0325777d126622340f9c94a66")
+    SERIF_LIGHT = get_fontfile_tuple("cjk_japanese_noto_serif/light.otf", "0def63d37c63f0945d1046dae5ab4d83")
+    SERIF_REGULAR = get_fontfile_tuple("cjk_japanese_noto_serif/regular.otf", "069123ca4dcbdee5cef81ef2f1d2ba8d")
+    SERIF_BOLD = get_fontfile_tuple("cjk_japanese_noto_serif/bold.otf", "ea7175c0325777d126622340f9c94a66")
 
 
 class FontThai(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     # sansserif
-    SANSSERIF_LIGHT = get_fontfile_tuple("noto_thai_sans/light.ttf", "fa192df61c8ef9a6a204c6323fdae9dc")
-    SANSSERIF_REGULAR = get_fontfile_tuple("noto_thai_sans/regular.ttf", "a84996ee5e940db8c7c2e1375728ca68")
-    SANSSERIF_BOLD = get_fontfile_tuple("noto_thai_sans/bold.ttf", "1296256d14a6c704f87967dc06583a64")
+    SANSSERIF_LIGHT = get_fontfile_tuple("thai_noto_sans/light.ttf", "fa192df61c8ef9a6a204c6323fdae9dc")
+    SANSSERIF_REGULAR = get_fontfile_tuple("thai_noto_sans/regular.ttf", "a84996ee5e940db8c7c2e1375728ca68")
+    SANSSERIF_BOLD = get_fontfile_tuple("thai_noto_sans/bold.ttf", "1296256d14a6c704f87967dc06583a64")
 
     # serif
-    SERIF_LIGHT = get_fontfile_tuple("noto_thai_serif/light.ttf", "70c158b4144d83cba0f7266952ddad2f")
-    SERIF_REGULAR = get_fontfile_tuple("noto_thai_serif/regular.ttf", "fe28175fbf4e79f1562d30f60933cab7")
-    SERIF_BOLD = get_fontfile_tuple("noto_thai_serif/bold.ttf", "dc10158f174b8141c810880b98ba5a5a")
+    SERIF_LIGHT = get_fontfile_tuple("thai_noto_serif/light.ttf", "70c158b4144d83cba0f7266952ddad2f")
+    SERIF_REGULAR = get_fontfile_tuple("thai_noto_serif/regular.ttf", "fe28175fbf4e79f1562d30f60933cab7")
+    SERIF_BOLD = get_fontfile_tuple("thai_noto_serif/bold.ttf", "dc10158f174b8141c810880b98ba5a5a")
 
 
 class FontArabic(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     # sans
-    SANSSERIF_LIGHT = get_fontfile_tuple("noto_arabic_sans/light.ttf", "ffcfcc231a05032bca6e0819aa60eacb")
-    SANSSERIF_REGULAR = get_fontfile_tuple("noto_arabic_sans/regular.ttf", "75527903c6a793772b02807c5343f4c8")
-    SANSSERIF_BOLD = get_fontfile_tuple("noto_arabic_sans/bold.ttf", "cda675687ed1576b7bda072838c0ed5f")
-
-    # naskh
-    NASKH_REGULAR = get_fontfile_tuple("noto_arabic_naskh/regular.ttf", "08f2d6bfe92d3e78721a0e1746397344")
-    NASKH_BOLD = get_fontfile_tuple("noto_arabic_naskh/bold.ttf", "3e8ac1d70691caf5ddfd36fee8acce3d")
+    SANSSERIF_LIGHT = get_fontfile_tuple("arabic_noto_sans/light.ttf", "ffcfcc231a05032bca6e0819aa60eacb")
+    SANSSERIF_REGULAR = get_fontfile_tuple("arabic_noto_sans/regular.ttf", "75527903c6a793772b02807c5343f4c8")
+    SANSSERIF_BOLD = get_fontfile_tuple("arabic_noto_sans/bold.ttf", "cda675687ed1576b7bda072838c0ed5f")
 
     # kufi
-    KUFI_LIGHT = get_fontfile_tuple("noto_arabic_kufi/light.ttf", "23517c64b528b3c744bfb3be94e58836")
-    KUFI_REGULAR = get_fontfile_tuple("noto_arabic_kufi/regular.ttf", "600b529eb4849a54dde020e3ea389de2")
-    KUFI_BOLD = get_fontfile_tuple("noto_arabic_kufi/bold.ttf", "34886bd59d48cf9113e1e9386bee615e")
+    KUFI_LIGHT = get_fontfile_tuple("arabic_noto_kufi/light.ttf", "23517c64b528b3c744bfb3be94e58836")
+    KUFI_REGULAR = get_fontfile_tuple("arabic_noto_kufi/regular.ttf", "600b529eb4849a54dde020e3ea389de2")
+    KUFI_BOLD = get_fontfile_tuple("arabic_noto_kufi/bold.ttf", "34886bd59d48cf9113e1e9386bee615e")
+
+    # naskh
+    NASKH_REGULAR = get_fontfile_tuple("arabic_noto_naskh/regular.ttf", "08f2d6bfe92d3e78721a0e1746397344")
+    NASKH_BOLD = get_fontfile_tuple("arabic_noto_naskh/bold.ttf", "3e8ac1d70691caf5ddfd36fee8acce3d")
 
 
 class FontMonoSpace(FontBase):
     """Drawlib Fonts.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
@@ -275,34 +278,37 @@
 
     # robotomono
     ROBOTO_MONO_LIGHT = get_fontfile_tuple("roboto_mono/light.ttf", "c9166464b1db95fc3cdf9b50fc7f98e2")
     ROBOTO_MONO_REGULAR = get_fontfile_tuple("roboto_mono/regular.ttf", "5b04fdfec4c8c36e8ca574e40b7148bb")
     ROBOTO_MONO_BOLD = get_fontfile_tuple("roboto_mono/bold.ttf", "90190d91283189e340b2a44fe560f2cd")
 
     # courier
-    COURIER_REGULAR = get_fontfile_tuple("courier/regular.ttf", "fba4686ed1d1b4ef05ab14db78805dbe")
-    COURIER_BOLD = get_fontfile_tuple("courier/bold.ttf", "4acfa45d29d240044e0075a8e58f0862")
+    COURIER_REGULAR = get_fontfile_tuple("mono_courier/regular.ttf", "fba4686ed1d1b4ef05ab14db78805dbe")
+    COURIER_BOLD = get_fontfile_tuple("mono_courier/bold.ttf", "4acfa45d29d240044e0075a8e58f0862")
 
     # source code pro
-    SOURCECODEPRO_LIGHT = get_fontfile_tuple("source_han_code_jp/light.otf", "ef1eb2fa9ff7c02e8a3336a70826ad47")
-    SOURCECODEPRO_REGULAR = get_fontfile_tuple("source_han_code_jp/regular.otf", "abcdbd5449ad6a30d540221a12f4a0b5")
-    SOURCECODEPRO_BOLD = get_fontfile_tuple("source_han_code_jp/bold.otf", "dff5826247909bb8e04b8bf3be893386")
+    SOURCECODEPRO_LIGHT = get_fontfile_tuple("mono_source_han_code_jp/light.otf", "ef1eb2fa9ff7c02e8a3336a70826ad47")
+    SOURCECODEPRO_REGULAR = get_fontfile_tuple(
+        "mono_source_han_code_jp/regular.otf",
+        "abcdbd5449ad6a30d540221a12f4a0b5",
+    )
+    SOURCECODEPRO_BOLD = get_fontfile_tuple("mono_source_han_code_jp/bold.otf", "dff5826247909bb8e04b8bf3be893386")
 
 
 class FontSourceCode(FontBase):
     """Drawlib Fonts which good for source code.
 
     Drawlib avoid using system font since it depends on host OS.
     Using only internal font files and user provided font file.
 
     """
 
     ROBOTO_MONO = get_fontfile_tuple("roboto_mono/regular.ttf", "5b04fdfec4c8c36e8ca574e40b7148bb")
-    COURIER = get_fontfile_tuple("courier/regular.ttf", "fba4686ed1d1b4ef05ab14db78805dbe")
-    SOURCECODEPRO = get_fontfile_tuple("source_han_code_jp/regular.otf", "abcdbd5449ad6a30d540221a12f4a0b5")
+    COURIER = get_fontfile_tuple("mono_courier/regular.ttf", "fba4686ed1d1b4ef05ab14db78805dbe")
+    SOURCECODEPRO = get_fontfile_tuple("mono_source_han_code_jp/regular.otf", "abcdbd5449ad6a30d540221a12f4a0b5")
 
 
 @dataclasses.dataclass
 class FontFile:
     file: str
 
     @property  # type: ignore[no-redef]
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core/model.py` & `drawlib-0.1.5/drawlib/v0_1/private/core/model.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core/model_validator.py` & `drawlib-0.1.5/drawlib/v0_1/private/core/model_validator.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core/util.py` & `drawlib-0.1.5/drawlib/v0_1/private/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,22 +690,22 @@
 
         Returns:
             Optional[FontProperties]: return None if arg is None.
 
         """
 
         if style is None or isinstance(style, TextStyle):
-            default = dtheme.textstyle_get()
+            default = dtheme.textstyles.get()
             if default.size is None:
                 default.size = TextStyleDefault.size
             if default.font is None:
                 default.font = TextStyleDefault.font
 
         if isinstance(style, ShapeTextStyle):
-            default = dtheme.shapetextstyle_get()
+            default = dtheme.shapetextstyles.get()
             if default.size is None:
                 default.size = ShapeTextStyleDefault.size
             if default.font is None:
                 default.font = ShapeTextStyleDefault.font
 
         DEFAULT_SIZE = default.size
         DEFAULT_FONT = default.font
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/__init__.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/base.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,42 +19,40 @@
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-public-methods
 
 # !!! Temporary Lint Escape !!!
 # pylint: disable=unnecessary-ellipsis
 # pylint: disable=unused-argument
 
-import os
+
 import math
 from typing import Final, Union, Optional, List, Tuple, Literal
 import matplotlib.font_manager
 import matplotlib.artist
 import matplotlib.lines
 import matplotlib.text
 from matplotlib.path import Path
 from matplotlib.patches import PathPatch
 from matplotlib import pyplot
 import PIL.Image
 
 from drawlib.v0_1.private.core.theme import dtheme
 from drawlib.v0_1.private.util import (
     error_handler,
-    get_script_path,
-    get_script_relative_path,
     get_center_and_size,
     minus_2points,
 )
 from drawlib.v0_1.private.core.model import (
     LineStyle,
     ShapeStyle,
     ShapeTextStyle,
 )
 from drawlib.v0_1.private.core.colors import Colors
 from drawlib.v0_1.private.core.dimage import Dimage
-from drawlib.v0_1.private.core.util import ColorUtil, ShapeUtil
+from drawlib.v0_1.private.core.util import ShapeUtil
 from drawlib.v0_1.private.arg_validator import ArgValidator
 
 
 class CanvasBase:
     """Base class of Canvas and its features.
 
     This class is designed for diamond inheritance.
@@ -91,14 +89,16 @@
             None,
         ] = None  # apply theme default later if no update
         self._background_alpha: Optional[float] = None  # apply theme default later if no update
         self._grid = self.DEFAULT_GRID
         self._grid_only = self.DEFAULT_GRID_ONLY
         self._grid_style = self.DEFAULT_GRID_STYLE
         self._grid_centerstyle = self.DEFAULT_GRID_CENTERSTYLE
+        self._grid_xpitch: Optional[int] = None
+        self._grid_ypitch: Optional[int] = None
         self._artists: List[matplotlib.artist.Artist] = []
 
         # it is decleared only for typing system
         self._fig = pyplot.figure()
         self._ax = self._fig.add_subplot(1, 1, 1)
 
         # initialize fig and ax
@@ -116,15 +116,16 @@
         It will wipe params which are set by config().
         And also, all drawing states.
 
         Returns:
             None
 
         Note:
-            ``dtheme`` is not initialized.
+            ``clear()`` doesn't make theme default.
+            If you want to change theme to default, please call ``config(theme="default")`` after ``clear()``.
 
         """
 
         pyplot.close()
         # pylint: disable=unnecessary-dunder-call
         CanvasBase.__init__(self)  # type: ignore[misc]
         # pylint: enable=unnecessary-dunder-call
@@ -147,14 +148,16 @@
             None,
         ] = None,
         background_alpha: Optional[float] = None,
         grid: Optional[bool] = None,
         grid_only: Optional[bool] = None,
         grid_style: Optional[LineStyle] = None,
         grid_centerstyle: Optional[LineStyle] = None,
+        grid_xpitch: Optional[int] = None,
+        grid_ypitch: Optional[int] = None,
     ) -> None:
         """Configure drawlib Canvas
 
         Configure drawlib canvas parameters.
         Parameters will be wiped when ``clear()`` method is called except ``theme``.
         You can call this function many times.
 
@@ -239,15 +242,15 @@
             self._ax.set_aspect("equal")
             self._ax.axis("off")
             self._ax.margins(0, 0)
 
         def config_theme():
             if theme is None:
                 return
-            dtheme.theme_apply_by_name(theme)
+            dtheme.apply_official_theme(theme)
 
         def config_background():
             if background_color is not None:
                 self._background_color = background_color
             if background_alpha is not None:
                 self._background_alpha = background_alpha
 
@@ -263,147 +266,31 @@
                 self._grid_centerstyle = grid_centerstyle
 
             if grid_only is not None:
                 self._grid_only = grid_only
                 if grid_only:
                     self._grid = True
 
+            if grid_xpitch is not None:
+                self._grid_xpitch = grid_xpitch
+
+            if grid_ypitch is not None:
+                self._grid_ypitch = grid_ypitch
+
             if grid is not None:
                 self._grid = grid
 
             # grid is drawn at method _render()
 
         pyplot.close()
         config_size_dpi()
         config_theme()
         config_background()
         config_grid()
 
-    @error_handler
-    def save(
-        self,
-        file: Optional[str] = None,
-        format: Optional[Literal["jpg", "png", "webp", "pdf"]] = None,
-    ) -> None:
-        """Save canvas illustration to file.
-
-        Args:
-            file(optional): saving image file path. Default is "<script-name>.png".
-            format(optional): supported image format. default is "png".
-
-        Returns:
-            None
-
-        Note:
-            Without arg, save to "<scriptfilename>.png" on script dir.
-            For example, calling "save()" at script "mydir/image1.py" will
-            generate "mydir/image1.png"
-
-        """
-
-        # validate args
-
-        if file is not None:
-            ArgValidator.validate_str("file", file)
-        if format is not None:
-            if file is not None:
-                raise ValueError('Can not specify format when arg "file" is provided.')
-            supported = ["jpg", "png", "webp", "pdf"]
-            if format not in supported:
-                raise ValueError(f'Save format supports only {supported}. But "{format}" is provided.')
-
-        # create save file path
-
-        if file is None:
-            script_path = get_script_path()
-            parent_dir = os.path.dirname(script_path)
-            name = os.path.basename(script_path)
-            name_without_ext = os.path.splitext(name)[0]
-            ext = "png" if format is None else format
-            file_path = f"{os.path.join(parent_dir, name_without_ext)}.{ext}"
-        else:
-            file_path = get_script_relative_path(file)
-
-        # set background
-
-        has_color_alpha = False
-        if self._background_color is not None:
-            background_color = self._background_color
-            if len(background_color) == 4:
-                has_color_alpha
-        else:
-            background_color = dtheme.background_color_get()
-
-        if self._background_alpha is not None:
-            background_alpha = self._background_alpha
-        elif has_color_alpha:
-            # set user specified alpha in color as alpha-value
-            background_alpha = background_color[3]
-        else:
-            background_alpha = dtheme.background_alpha_get()
-
-        mplot_rgba = ColorUtil.get_mplot_rgba(background_color, background_alpha)
-        self._fig.patch.set_facecolor(mplot_rgba)
-        self._ax.patch.set_alpha(0)
-
-        # draw artist (image, patches, line, text)
-
-        zorder = 0
-        for artist in self._artists:
-            artist.zorder = zorder
-            zorder += 1
-            self._ax.add_artist(artist)
-        self._artists = []
-
-        # remove margin
-
-        self._fig.tight_layout()
-        self._fig.subplots_adjust(left=0, right=1, bottom=0, top=1)
-
-        # save to file
-
-        directory = os.path.dirname(file_path)
-        os.makedirs(directory, exist_ok=True)
-
-        if not self._grid_only:
-            pyplot.savefig(file_path)
-            if not self._grid:
-                return
-
-        # draw grid
-        grid_width = self._width / 10
-        grid_height = self._height / 10
-        for i in range(1, 10):
-            style = self._grid_centerstyle if i == 5 else self._grid_style
-            self.line(
-                xy1=(i * grid_width, 0),
-                xy2=(i * grid_width, self._height),
-                style=style,
-            )
-        for i in range(1, 10):
-            style = self._grid_centerstyle if i == 5 else self._grid_style
-            self.line(
-                xy1=(0, i * grid_height),
-                xy2=(self._width, i * grid_height),
-                style=style,
-            )
-
-        for artist in self._artists:
-            artist.zorder = zorder
-            zorder += 1
-            self._ax.add_artist(artist)
-        self._artists = []
-
-        # save to file
-        if self._grid_only:
-            pyplot.savefig(file_path)
-        else:
-            name, extension = os.path.splitext(file_path)
-            pyplot.savefig(f"{name}_grid{extension}")
-
     #######################
     ### low level shape ###
     #######################
 
     def shape(
         self,
         xy: Tuple[float, float],
@@ -411,15 +298,15 @@
             Union[
                 Tuple[float, float],
                 Tuple[float, float, float, float],
                 Tuple[float, float, float, float, float, float],
             ]
         ],
         angle: Optional[float] = None,
-        style: Optional[ShapeStyle] = None,
+        style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
         textstyle: Optional[ShapeTextStyle] = None,
         is_default_center: bool = False,
     ) -> None:
         """Draw basic shape.
 
         This function is useful for drawing user original shapes.
@@ -442,14 +329,16 @@
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_path_points("path_points", path_points)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.shapestyles.get(name=style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
         if is_default_center is not None:
             ArgValidator.validate_bool("is_default_center", is_default_center)
@@ -462,16 +351,16 @@
             angle_rad = math.radians(angle)
             x_rotated = x * math.cos(angle_rad) - y * math.sin(angle_rad)
             y_rotated = x * math.sin(angle_rad) + y * math.cos(angle_rad)
             return x_rotated + move_x, y_rotated + move_y
 
         # apply default style
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyles.get())
 
         # shift to center (0, 0)
 
         points_without_cp = []
         for pp in path_points:
             points_without_cp.append(pp[-2:])
         center, (width, height) = get_center_and_size(points_without_cp)
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/image.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,27 +61,27 @@
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_int("width", width)
         ArgValidator.validate_image_objects("image", image)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.imagestyle_get(style)
+                style = dtheme.imagestyles.get(name=style)
             ArgValidator.validate_imagestyle("style", style)
 
         # standadize
 
         x, y = xy
         pimg = Dimage(image, copy=True)
         image_width, image_height = pimg.get_image_size()
         height = image_height / image_width * width
         zoom = self.get_image_zoom_from_width(pimg, width)
 
         # set default alignment if not specified
-        style = ImageUtil.get_merged_style(style, dtheme.imagestyle_get())
+        style = ImageUtil.get_merged_style(style, dtheme.imagestyles.get())
         if style.halign is None:
             if angle is None:
                 style.halign = "left"
             else:
                 style.halign = "center"
         if style.valign is None:
             if angle is None:
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/line.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/line.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,25 +88,25 @@
         ArgValidator.validate_xy("xy1", xy1)
         ArgValidator.validate_xy("xy2", xy2)
         ArgValidator.validate_float("bend", bend)
         if not -2.0 <= bend <= 2.0:
             raise ValueError(f'Arg "bend" supports float between -2.0 ~ 2.0. But {bend} is given.')
         if style is not None:
             if isinstance(style, str):
-                if dtheme.linestyle_has(style):
-                    style = dtheme.linestyle_get(style)
-                elif dtheme.linearrowstyle_has(style):
-                    style = dtheme.linearrowstyle_get(style)
+                if dtheme.linestyles.has(name=style):
+                    style = dtheme.linestyles.get(name=style)
+                elif dtheme.linearrowstyles.has(name=style):
+                    style = dtheme.linearrowstyles.get(name=style)
                 else:
                     raise Exception(f'Both LineStyle and LineArrowStyle does not have theme name "{style}"')
             ArgValidator.validate_linestyle_or_linearrowstyle("style", style)
 
         # create FancyArrowPatch
 
-        style = LineUtil.get_merged_style(style, dtheme.linestyle_get(), dtheme.linearrowstyle_get())
+        style = LineUtil.get_merged_style(style, dtheme.linestyles.get(), dtheme.linearrowstyles.get())
         options = LineUtil.get_fancyarrowpatch_options(style)
         self._artists.append(
             FancyArrowPatch(
                 posA=xy1,
                 posB=xy2,
                 connectionstyle=ConnectionStyle.Arc3(rad=bend),
                 **options,
@@ -239,18 +239,18 @@
 
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_path_points("path_points", path_points)
         if style is not None:
             if isinstance(style, str):
-                if dtheme.linestyle_has(style):
-                    style = dtheme.linestyle_get(style)
-                elif dtheme.linearrowstyle_has(style):
-                    style = dtheme.linearrowstyle_get(style)
+                if dtheme.linestyles.has(name=style):
+                    style = dtheme.linestyles.get(name=style)
+                elif dtheme.linearrowstyles.has(name=style):
+                    style = dtheme.linearrowstyles.get(name=style)
                 else:
                     raise Exception(f'Both LineStyle and LineArrowStyle does not have theme name "{style}"')
             ArgValidator.validate_linestyle_or_linearrowstyle("style", style)
 
         # create Path
 
         vertices = [xy]
@@ -268,10 +268,10 @@
             else:
                 vertices.extend([(p[0], p[1]), (p[2], p[3]), (p[4], p[5])])
                 codes.extend([Path.CURVE4] * 3)
         path = Path(vertices=vertices, codes=codes)
 
         # create FancyArrowPatch
 
-        style = LineUtil.get_merged_style(style, dtheme.linestyle_get(), dtheme.linearrowstyle_get())
+        style = LineUtil.get_merged_style(style, dtheme.linestyles.get(), dtheme.linearrowstyles.get())
         options = LineUtil.get_fancyarrowpatch_options(style)
         self._artists.append(FancyArrowPatch(path=path, **options))
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_arrow.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/original_arrow.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         head_style: Literal[
             "-|>",
             "<|-",
             "<|-|>",
         ] = "-|>",
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw sing and double heads arrow.
 
         Args:
             xy1: Arrow start point
             xy2: Arrow end point.
             tail_width: Arrow tail width.
@@ -67,33 +67,38 @@
         """
 
         # matplotlib FancyArrow, FancyArrowPatch seems not good
         # for implement this function.
         # Calculate arrow points pass it to shape().
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.arrowtextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy1", xy1)
         ArgValidator.validate_xy("xy2", xy2)
         ArgValidator.validate_float("tail_width", tail_width)
         ArgValidator.validate_float("head_width", head_width)
         ArgValidator.validate_float("head_length", head_length)
         if head_style not in ["-|>", "<|-", "<|-|>"]:
             raise ValueError('Arg "tail_edge" must be one of ["-|>", "<|-", "<|-|>"].')
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_arrow_get(style)
+                style = dtheme.arrowstyles.get(name=style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.arrowtextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_arrow_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.arrowstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.arrowtextstyles.get())
 
         x1, y1 = xy1
         x2, y2 = xy2
         x, y = ((x1 + x2) / 2, (y1 + y2) / 2)
         angle = get_angle(xy1, xy2)
         style.halign = "center"  # no choice
         style.valign = "center"  # no choice
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/original_polygon.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/original_polygon.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         height: float,
         tail_edge: Literal["left", "top", "right", "bottom"],
         tail_from_ratio: float,
         tail_vertex_xy: Tuple[float, float],
         tail_to_ratio: float,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw bubble speech.
 
         Almost same to rectangle. But having tail.
 
         Args:
             xy: always left bottom. Aligns are ignored.
@@ -65,40 +65,46 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.bubblespeechtextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         if tail_edge not in ["left", "top", "right", "bottom"]:
             raise ValueError('Arg "tail_edge" must be one of ["left", "top", "right", "bottom"].')
         ArgValidator.validate_float("tail_from_ratio", tail_from_ratio)
         ArgValidator.validate_xy("tail_vertex_xy", tail_vertex_xy)
         ArgValidator.validate_float("tail_to_ratio", tail_to_ratio)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_bubblespeech_get(style)
+                style = dtheme.bubblespeechstyles.get(name=style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
+
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.bubblespeechtextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         if tail_from_ratio > tail_to_ratio:
             raise ValueError("tail_from_ratio must be smaller than tail_to_ratio.")
         if tail_to_ratio > 1.0:
             raise ValueError(f"tail_from_ratio and tail_to_ratio must be smaller than 1.0")
 
         x, y = xy
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_bubblespeech_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.bubblespeechstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.bubblespeechtextstyles.get())
 
         xys = []
         xys.append((x, y))  # left bottom
         if tail_edge == "left":
             xys.append((x, y + height * tail_from_ratio))
             xys.append(tail_vertex_xy)
             xys.append((x, y + height * tail_to_ratio))
@@ -138,15 +144,15 @@
         xy: Tuple[float, float],
         width: float,
         height: float,
         topvertex_x: Optional[float] = None,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw triangle.
 
         Args:
             xy: default left bottom.
             width: width of triangle bottom
             height: height of traiangle
@@ -158,35 +164,41 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.triangletextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         if topvertex_x is not None:
             ArgValidator.validate_float("topvertex_x", topvertex_x)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_triangle_get(style)
+                style = dtheme.trianglestyles.get(name=style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
+
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.triangletextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_triangle_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.trianglestyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.triangletextstyles.get())
 
         if topvertex_x is None:
             topvertex_x = width / 2
         p1 = (0, 0)
         p2 = (topvertex_x, height)
         p3 = (width, 0)
         self.shape(
@@ -203,15 +215,15 @@
         xy: Tuple[float, float],
         width: float,
         height: float,
         corner_angle: float,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ):
         """Draw parallelogram.
 
         Args:
             xy: default left bottom.
             width: width of triangle bottom
             height: height of traiangle
@@ -223,39 +235,44 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.parallelogramtextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         ArgValidator.validate_float("corner_angle", corner_angle)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_parallelogram_get(style)
+                style = dtheme.parallelogramstyles.get(name=style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.parallelogramtextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
 
         def calculate_parallelogram_lefttop_coordinate():
             angle_rad = math.radians(corner_angle)
             x = height / math.tan(angle_rad)
             return x, height
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_parallelogram_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.parallelogramstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.parallelogramtextstyles.get())
 
         p1 = (0, 0)
         p2 = calculate_parallelogram_lefttop_coordinate()
         p3 = (p2[0] + width, height)
         p4 = (width, 0)
 
         self.shape(
@@ -273,15 +290,15 @@
         height: float,
         bottomedge_width: float,
         topedge_width: float,
         topedge_x: Optional[float] = None,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ):
         """Draw triangle.
 
         Args:
             xy: default left bottom.
             height: height of traiangle
             bottomedge_width: width of bottom
@@ -294,36 +311,41 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.trapezoidtextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("height", height)
         ArgValidator.validate_float("bottomedge_width", bottomedge_width)
         ArgValidator.validate_float("topedge_width", topedge_width)
         if topedge_x is not None:
             ArgValidator.validate_float("topedge_xstart", topedge_x)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_trapezoid_get(style)
+                style = dtheme.trapezoidstyles.get(name=style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.trapezoidtextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_trapezoid_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.trapezoidstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.trapezoidtextstyles.get())
 
         if topedge_x is None:
             topedge_x = (bottomedge_width - topedge_width) / 2
         p1 = (0, 0)
         p2 = (topedge_x, height)
         p3 = (topedge_x + topedge_width, height)
         p4 = (bottomedge_width, 0)
@@ -341,15 +363,15 @@
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ):
         """Draw rhombus.
 
         Args:
             xy: default left bottom.
             width: width of rhombus
             height: height of rhombus
@@ -360,31 +382,36 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.rhombustextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_rhombus_get(style)
+                style = dtheme.rhombusstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.rhombustextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_rhombus_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.rhombusstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.rhombustextstyles.get())
 
         p1 = (0, height / 2)
         p2 = (width / 2, height)
         p3 = (width, height / 2)
         p4 = (width / 2, 0)
 
         self.shape(
@@ -402,15 +429,15 @@
         width: float,
         height: float,
         corner_angle: float,
         mirror: bool = False,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw chevron.
 
         Vertex is right on default. Provide True for mirror makes left side vertex.
 
         Args:
             xy: default left bottom.
@@ -425,35 +452,40 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.chevrontextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         ArgValidator.validate_float("corner_angle", corner_angle)
         if not 0.0 <= corner_angle <= 90.0:
             raise ValueError(f"corner_angles supports 0.0 ~ 90.0. But {corner_angle} is given.")
         ArgValidator.validate_bool("mirror", mirror)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_chevron_get(style)
+                style = dtheme.chevronstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.chevrontextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_chevron_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.chevronstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.chevrontextstyles.get())
 
         if mirror:
             corner_angle = 180 - corner_angle
 
         p1 = (0, 0)
         p2x = height / 2 * math.cos(math.radians(corner_angle))
         p2 = (p2x, height / 2)
@@ -476,15 +508,15 @@
         xy: Tuple[float, float],
         num_vertex: int,
         radius_ext: float,
         radius_int: float,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw star.
 
         Args:
             xy: default center, center.
             num_vertex: numver of external vertex. 3 ~.
             radius_ext: radius of external vertex.
@@ -496,28 +528,33 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.startextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_int("num_vertex", num_vertex)
         ArgValidator.validate_float("radius_ext", radius_ext)
         ArgValidator.validate_float("radius_int", radius_int)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_star_get(style)
+                style = dtheme.starstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.startextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         if num_vertex < 3:
             raise ValueError()
         if radius_ext < radius_int:
             raise ValueError()
 
@@ -529,16 +566,16 @@
             angle_rad = math.radians(angle)
             x_rotated = x * math.cos(angle_rad) - y * math.sin(angle_rad)
             y_rotated = x * math.sin(angle_rad) + y * math.cos(angle_rad)
             return x_rotated + move_x, y_rotated + move_y
 
         # apply default style
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_star_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.starstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.startextstyles.get())
 
         # calculate points
 
         points = []
         start_angle = math.pi / 2
         for i in range(2 * num_vertex):
             r = radius_ext if i % 2 == 0 else radius_int
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/patches.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/patches.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         width: float,
         height: float,
         from_angle: int = 0,
         to_angle: int = 360,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw arc.
 
         Args:
             xy: center of arc.
             width: width of arc.
             height: height of arc.
@@ -71,35 +71,40 @@
 
         Returns:
             None.
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.arctextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         ArgValidator.validate_angle("from_angle", from_angle)
         ArgValidator.validate_angle("to_angle", to_angle)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_arc_get(style)
+                style = dtheme.arcstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.arctextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if style not specified
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_arc_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.arcstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.arctextstyles.get())
         xy, style = ShapeUtil.apply_alignment(xy, width, height, angle, style, is_default_center=True)
         if angle is None:
             angle = 0
 
         options = ShapeUtil.get_shape_options(style, default_no_line=False)
         self._artists.append(
             Arc(
@@ -119,15 +124,15 @@
     def circle(
         self,
         xy: Tuple[float, float],
         radius: float,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw cicle.
 
         Args:
             xy: center of circle.
             radius: radius of circle.
             angle(optional): rotate inside text with specified angle
@@ -137,30 +142,35 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.circletextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("radius", radius)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_circle_get(style)
+                style = dtheme.circlestyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.circletextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_circle_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.circlestyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.circletextstyles.get())
         width = radius * 2
         height = radius * 2
         xy, style = ShapeUtil.apply_alignment(xy, width, height, angle, style, is_default_center=True)
         options = ShapeUtil.get_shape_options(style)
         self._artists.append(Circle(xy, radius, **options))
         if text:
             self._artists.append(ShapeUtil.get_shape_text(xy=xy, text=text, angle=angle, style=textstyle))
@@ -170,15 +180,15 @@
         self,
         xy: Tuple[float, float],
         width: float,
         height: float,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw ellipse
 
         Args:
             xy: center of ellipse
             width: width of ellipse.
             height: height of ellipse.
@@ -189,48 +199,53 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.ellipsetextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_ellipse_get(style)
+                style = dtheme.ellipsestyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.ellipsetextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_ellipse_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.ellipsestyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.ellipsetextstyles.get())
         xy, style = ShapeUtil.apply_alignment(xy, width, height, angle, style, is_default_center=True)
         if angle is None:
             angle = 0
         options = ShapeUtil.get_shape_options(style)
         self._artists.append(Ellipse(xy, width=width, height=height, angle=angle, **options))
         if text:
             self._artists.append(ShapeUtil.get_shape_text(xy=xy, text=text, angle=angle, style=textstyle))
 
     @error_handler
     def polygon(
         self,
         xys: List[Tuple[float, float]],
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw polygon.
 
         Args:
             xys: List of points. [(x1, y1), ...(x_n, y_n)].
             style(optional): style of polygon.
             text(optional): text which is shown at center of ellipse.
@@ -238,29 +253,34 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.polygontextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xys("xys", xys)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_polygon_get(style)
+                style = dtheme.polygonstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.polygontextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_polygon_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.polygonstyles.get())
         style.halign = None
         style.valign = None
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.polygontextstyles.get())
         options = ShapeUtil.get_shape_options(style)
         self._artists.append(Polygon(xy=xys, closed=True, **options))
 
         if text:
             center, (_, _) = get_center_and_size(xys)
             self._artists.append(ShapeUtil.get_shape_text(center, text=text, angle=0, style=textstyle))
 
@@ -269,15 +289,15 @@
         self,
         xy: Tuple[float, float],
         radius: float,
         num_vertex: int,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw regular polygon.
 
         Args:
             xy: center of regular polygon
             radius: radius of regular polygon's vertex.
             num_vertex: number of vertex.
@@ -287,30 +307,36 @@
             textstyle(optional): style of text.
 
         Returns:
             None
 
         """
 
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.regularpolygontextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
+
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("radius", radius)
         ArgValidator.validate_int("num_vertex", num_vertex)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_regularpolygon_get(style)
+                style = dtheme.regularpolygonstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.regularpolygontextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_regularpolygon_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.regularpolygonstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.regularpolygontextstyles.get())
         width = radius * 2
         height = radius * 2
         xy, style = ShapeUtil.apply_alignment(xy, width, height, angle, style, is_default_center=True)
         if angle is None:
             angle = 0
 
         options = ShapeUtil.get_shape_options(style)
@@ -332,15 +358,15 @@
         xy: Tuple[float, float],
         width: float,
         height: float,
         r: float = 0.0,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw rectangle
 
         Args:
             xy: left bottom of rectangle.
             width: width of rounded rectangle.
             height: height of rounded rectangle.
@@ -352,34 +378,39 @@
 
         Returns:
             None
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.rectangletextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("width", width)
         ArgValidator.validate_float("height", height)
         ArgValidator.validate_float("r", r)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_rectangle_get(style)
+                style = dtheme.rectanglestyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.rectangletextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if styles are not specified
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_rectangle_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.rectanglestyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.rectangletextstyles.get())
         (x, y), style = ShapeUtil.apply_alignment(xy, width, height, angle, style)
 
         options = ShapeUtil.get_shape_options(style)
         rectangle = FancyBboxPatch(
             (x + r, y + r),
             width - r * 2,
             height - r * 2,
@@ -411,15 +442,15 @@
         radius: float,
         width: Optional[float] = None,
         from_angle: float = 0,
         to_angle: float = 360,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw wedge
 
         Args:
             xy: center of wedge
             radius: radius of wedge.
             width(optional): length from outer to inner circumference. default is same to radius value.
@@ -432,36 +463,41 @@
 
         Returns:
             None.
 
         """
 
         # validate args
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.wedgetextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_float("radius", radius)
         if width is not None:
             ArgValidator.validate_float("width", width)
         ArgValidator.validate_angle("from_angle", from_angle)
         ArgValidator.validate_angle("to_angle", to_angle)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_wedge_get(style)
+                style = dtheme.wedgestyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
         if text is not None:
             ArgValidator.validate_str("text", text)
         if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.wedgetextstyles.get(name=textstyle)
             ArgValidator.validate_shapetextstyle("textstyle", textstyle)
 
         # apply default if style not specified
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_wedge_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.wedgestyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.wedgetextstyles.get())
         ext_width = radius * 2
         ext_height = radius * 2
         xy, style = ShapeUtil.apply_alignment(xy, ext_width, ext_height, angle, style, is_default_center=True)
         if angle is None:
             angle = 0
 
         options = ShapeUtil.get_shape_options(style)
@@ -484,15 +520,15 @@
         self,
         xy: Tuple[float, float],
         radius: float,
         width: Optional[float] = None,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw donuts
 
         Args:
             xy: center of donuts
             radius: radius of donuts.
             width(optional): length from outer to inner circumference. default is same to radius value.
@@ -502,21 +538,30 @@
             textstyle(optional): style of text.
 
         Returns:
             None.
 
         """
 
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.donutstextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
+
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_donuts_get(style)
+                style = dtheme.donutsstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_donuts_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.donutstextstyles.get(name=textstyle)
+            ArgValidator.validate_shapetextstyle("textstyle", textstyle)
+
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.donutsstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.donutstextstyles.get())
         self.wedge(
             xy=xy,
             radius=radius,
             width=width,
             angle=angle,
             style=style,
             text=text,
@@ -529,15 +574,15 @@
         xy: Tuple[float, float],
         radius: float,
         from_angle: float = 0,
         to_angle: float = 180,
         angle: Optional[float] = None,
         style: Union[ShapeStyle, str, None] = None,
         text: Optional[str] = None,
-        textstyle: Optional[ShapeTextStyle] = None,
+        textstyle: Union[ShapeTextStyle, str, None] = None,
     ) -> None:
         """Draw fan
 
         Args:
             xy: center of fan
             radius: radius of fan.
             from_angle(optional): where drawing arc start. default is angle 0.0
@@ -547,22 +592,30 @@
             text(optional): text which is shown at center of wedge.
             textstyle(optional): style of text.
 
         Returns:
             None.
 
         """
+        if isinstance(style, str) and textstyle is None:
+            if dtheme.fantextstyles.has(style) or dtheme.shapetextstyles.has(style):
+                textstyle = style
 
         if style is not None:
             if isinstance(style, str):
-                style = dtheme.shapestyle_fan_get(style)
+                style = dtheme.fanstyles.get(style)
             ArgValidator.validate_shapestyle("style", style)
 
-        style = ShapeUtil.get_merged_shapestyle(style, dtheme.shapestyle_fan_get())
-        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyle_get())
+        if textstyle is not None:
+            if isinstance(textstyle, str):
+                textstyle = dtheme.fantextstyles.get(name=textstyle)
+            ArgValidator.validate_shapetextstyle("textstyle", textstyle)
+
+        style = ShapeUtil.get_merged_shapestyle(style, dtheme.fanstyles.get())
+        textstyle = ShapeUtil.get_merged_shapetextstyle(textstyle, dtheme.shapetextstyles.get())
         self.wedge(
             xy=xy,
             radius=radius,
             width=None,
             from_angle=from_angle,
             to_angle=to_angle,
             angle=angle,
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/core_canvas/text.py` & `drawlib-0.1.5/drawlib/v0_1/private/core_canvas/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Matplotlib is difficult for just drawing text.
 This module wraps it and provides easy to use interfaces.
 
 """
 
 # pylint: disable=too-many-arguments
 
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 from matplotlib.text import Text
 
 from drawlib.v0_1.private.core.model import TextStyle
 from drawlib.v0_1.private.core.util import TextUtil
 from drawlib.v0_1.private.util import error_handler
 from drawlib.v0_1.private.core.theme import dtheme
 from drawlib.v0_1.private.core_canvas.base import CanvasBase
@@ -33,15 +33,15 @@
 
     @error_handler
     def text(
         self,
         xy: Tuple[float, float],
         text: str,
         angle: Optional[float] = None,
-        style: Optional[TextStyle] = None,
+        style: Union[TextStyle, str, None] = None,
     ) -> None:
         """Draw text
 
         Args:
             xy: left bottom
             text: text
             angle: angle of texts
@@ -55,20 +55,22 @@
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_str("text", text)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.textstyles.get(name=style)
             ArgValidator.validate_textstyle("style", style)
 
         # apply default if style not specified
 
         x, y = xy
-        style = TextUtil.get_merged_textstyle(style, dtheme.textstyle_get())
+        style = TextUtil.get_merged_textstyle(style, dtheme.textstyles.get())
 
         options = TextUtil.get_text_options(style)
         fp = TextUtil.get_font_properties(style)
         bx = TextUtil.get_bbox_dict(style)
 
         # set default alignment
         if angle is None or angle == 0:
@@ -120,17 +122,19 @@
         # validate args
 
         ArgValidator.validate_xy("xy", xy)
         ArgValidator.validate_str("text", text)
         if angle is not None:
             ArgValidator.validate_angle("angle", angle)
         if style is not None:
+            if isinstance(style, str):
+                style = dtheme.textstyles.get(name=style)
             ArgValidator.validate_textstyle("style", style)
 
         # change text
 
-        style = TextUtil.get_merged_textstyle(style, dtheme.textstyle_get())
+        style = TextUtil.get_merged_textstyle(style, dtheme.textstyles.get())
         vertical_text = "\n".join(text)
 
         # call text()
 
         self.text(xy=xy, text=vertical_text, angle=angle, style=style)
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/download.py` & `drawlib-0.1.5/drawlib/v0_1/private/download.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/dutil.py` & `drawlib-0.1.5/drawlib/v0_1/private/dutil.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/icons/__init__.py` & `drawlib-0.1.5/drawlib/v0_1/private/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/icons/phosphor.py` & `drawlib-0.1.5/drawlib/v0_1/private/icons/phosphor.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     style: typing.Union[drawlib.v0_1.private.core.model.IconStyle, str, None] = None,
 ) -> None:
 
     DEFAULT_STYLE = "thin"
 
     # None, str -> IconStyle
     if style is None:
-        style = drawlib.v0_1.private.core.theme.dtheme.iconstyle_get()
+        style = drawlib.v0_1.private.core.theme.dtheme.iconstyles.get()
     elif isinstance(style, str):
-        style = drawlib.v0_1.private.core.theme.dtheme.iconstyle_get(style)
+        style = drawlib.v0_1.private.core.theme.dtheme.iconstyles.get(style)
     elif isinstance(style, drawlib.v0_1.private.core.model.IconStyle):
         ...
     else:
         raise ValueError(
             f'Unsupported type "{type(style)}" is passed to arg style. ' "Supports only IconStyle, str, None."
         )
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/icons/util.py` & `drawlib-0.1.5/drawlib/v0_1/private/icons/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     ArgValidator.validate_float("width", width)
     ArgValidator.validate_str("code", code)
     ArgValidator.validate_str("file", file)
     if angle is not None:
         ArgValidator.validate_angle("angle", angle)
     if style is not None:
         if isinstance(style, str):
-            style = dtheme.iconstyle_get(name=style)
+            style = dtheme.iconstyles.get(name=style)
         ArgValidator.validate_iconstyle("style", style)
 
     # set default parameters if not provided
 
-    style = IconUtil.get_merged_style(style, dtheme.iconstyle_get())
+    style = IconUtil.get_merged_style(style, dtheme.iconstyles.get())
     if style.halign is None:
         style.halign = "left" if angle is None else "center"
     if style.valign is None:
         style.valign = "bottom" if angle is None else "center"
 
     # get good font size from width
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/logging.py` & `drawlib-0.1.5/drawlib/v0_1/private/logging.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/settings.py` & `drawlib-0.1.5/drawlib/v0_1/private/settings.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/smartarts/__init__.py` & `drawlib-0.1.5/drawlib/v0_1/private/smartarts/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/smartarts/dsart.py` & `drawlib-0.1.5/drawlib/v0_1/private/smartarts/dsart.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/smartarts/groups.py` & `drawlib-0.1.5/drawlib/v0_1/private/smartarts/groups.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/smartarts/pyramid.py` & `drawlib-0.1.5/drawlib/v0_1/private/smartarts/pyramid.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/smartarts/sourcecode.py` & `drawlib-0.1.5/drawlib/v0_1/private/smartarts/sourcecode.py`

 * *Files 26% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             else:
                 return get_lexer_by_name(language)
 
         def get_formatter():
             pygments_style = get_style_by_name(style)
 
             if font is None:
-                file_path, download_url, md5_hash = dtheme.sourcecodefont_get().value
+                file_path, download_url, md5_hash = dtheme.sourcecodefonts.get().value
                 download_if_not_exist(
                     file_path=file_path,
                     download_url=download_url,
                     md5_hash=md5_hash,
                 )
             elif isinstance(font, FontFile):
                 file_path = font.file
@@ -184,33 +184,7 @@
         xy: Tuple[float, float],
         width: float,
         code: str,
         style: Optional[ImageStyle] = None,
     ) -> None:
         image_ = self.get_image(code=code)
         image(xy=xy, width=width, image=image_, style=style)
-
-        """
-        if not self._show_border:
-            return
-
-        im_width, im_height = image_.get_image_size()
-        height = (im_height / im_width) * width
-        if self._borderstyle is None:
-            self._borderstyle = LineStyle()
-
-        default = dtheme.shapestyle_get()
-        if self._borderstyle.color is None:
-            self._borderstyle.color = default.lcolor
-        if self._borderstyle.width is None:
-            self._borderstyle.width = default.lwidth
-        if self._borderstyle.style is None:
-            self._borderstyle.style = default.lstyle
-
-        rect_style = ShapeStyle(
-            lcolor=self._borderstyle.color,
-            lwidth=self._borderstyle.width,
-            lstyle=self._borderstyle.style,
-            fcolor=Colors.Transparent,
-        )
-        rectangle(xy=xy, width=width, height=height, style=rect_style)
-        """
```

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/smartarts/tree.py` & `drawlib-0.1.5/drawlib/v0_1/private/smartarts/tree.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/tools.py` & `drawlib-0.1.5/drawlib/v0_1/private/tools.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/drawlib/v0_1/private/util.py` & `drawlib-0.1.5/drawlib/v0_1/private/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.4/pyproject.toml` & `drawlib-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "drawlib"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python drawing library. Illustration as Code."
 homepage = "https://www.drawlib.com"
 repository = "https://github.com/yuichi110/drawlib"
 authors = [ "Yuichi Ito <yuichi@yuichi.com>",]
 readme = "README.md"
 
 [tool.black]
```

### Comparing `drawlib-0.1.4/PKG-INFO` & `drawlib-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawlib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python drawing library. Illustration as Code.
 Home-page: https://www.drawlib.com
 Author: Yuichi Ito
 Author-email: yuichi@yuichi.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

