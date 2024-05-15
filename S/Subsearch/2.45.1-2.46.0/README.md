# Comparing `tmp/subsearch-2.45.1.tar.gz` & `tmp/subsearch-2.46.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsearch-2.45.1.tar", last modified: Sun May 12 16:31:39 2024, max compression
+gzip compressed data, was "subsearch-2.46.0.tar", last modified: Wed May 15 13:31:25 2024, max compression
```

## Comparing `subsearch-2.45.1.tar` & `subsearch-2.46.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.540203 subsearch-2.45.1/
--rw-rw-rw-   0        0        0     1093 2024-05-12 16:31:02.000000 subsearch-2.45.1/LICENSE
--rw-rw-rw-   0        0        0      121 2024-05-12 16:31:02.000000 subsearch-2.45.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7491 2024-05-12 16:31:39.540203 subsearch-2.45.1/PKG-INFO
--rw-rw-rw-   0        0        0     5741 2024-05-12 16:31:02.000000 subsearch-2.45.1/README.md
--rw-rw-rw-   0        0        0     2556 2024-05-12 16:31:02.000000 subsearch-2.45.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 16:31:39.540203 subsearch-2.45.1/setup.cfg
--rw-rw-rw-   0        0        0      114 2024-05-12 16:31:02.000000 subsearch-2.45.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.508951 subsearch-2.45.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.540203 subsearch-2.45.1/src/Subsearch.egg-info/
--rw-rw-rw-   0        0        0     7491 2024-05-12 16:31:39.000000 subsearch-2.45.1/src/Subsearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2078 2024-05-12 16:31:39.000000 subsearch-2.45.1/src/Subsearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:31:39.000000 subsearch-2.45.1/src/Subsearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-12 16:31:39.000000 subsearch-2.45.1/src/Subsearch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-12 16:31:39.000000 subsearch-2.45.1/src/Subsearch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      377 2024-05-12 16:31:39.000000 subsearch-2.45.1/src/Subsearch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 16:31:39.000000 subsearch-2.45.1/src/Subsearch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.524655 subsearch-2.45.1/src/subsearch/
--rw-rw-rw-   0        0        0     1487 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/__init__.py
--rw-rw-rw-   0        0        0       38 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/__main__.py
--rw-rw-rw-   0        0        0     9540 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/core.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.524655 subsearch-2.45.1/src/subsearch/data/
--rw-rw-rw-   0        0        0       99 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/data/__init__.py
--rw-rw-rw-   0        0        0       53 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/data/guid.py
--rw-rw-rw-   0        0        0     7704 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/data/language_data.toml
--rw-rw-rw-   0        0        0       24 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/data/version.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.524655 subsearch-2.45.1/src/subsearch/globals/
--rw-rw-rw-   0        0        0       62 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/__init__.py
--rw-rw-rw-   0        0        0     6405 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/_logging.py
--rw-rw-rw-   0        0        0      513 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/constants.py
--rw-rw-rw-   0        0        0     2505 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/dataclasses.py
--rw-rw-rw-   0        0        0     5159 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/decorators.py
--rw-rw-rw-   0        0        0      980 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/exceptions.py
--rw-rw-rw-   0        0        0      258 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/metaclasses.py
--rw-rw-rw-   0        0        0     1269 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/globals/thread_handle.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.524655 subsearch-2.45.1/src/subsearch/gui/
--rw-rw-rw-   0        0        0      588 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/__init__.py
--rw-rw-rw-   0        0        0     3180 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/common_utils.py
--rw-rw-rw-   0        0        0     1053 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resource_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.524655 subsearch-2.45.1/src/subsearch/gui/resources/
--rw-rw-rw-   0        0        0        0 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.524655 subsearch-2.45.1/src/subsearch/gui/resources/assets/
--rw-rw-rw-   0        0        0        0 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/assets/__init__.py
--rw-rw-rw-   0        0        0     7119 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/assets/spritesheet.png
--rw-rw-rw-   0        0        0   105808 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/assets/subsearch.ico
--rw-rw-rw-   0        0        0     1674 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/config.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.524655 subsearch-2.45.1/src/subsearch/gui/resources/styles/
--rw-rw-rw-   0        0        0        0 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/styles/__init__.py
--rw-rw-rw-   0        0        0     1780 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/styles/sprites.tcl
--rw-rw-rw-   0        0        0     7247 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/styles/style_subsearch.tcl
--rw-rw-rw-   0        0        0     1451 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/resources/styles/theme_setter.tcl
--rw-rw-rw-   0        0        0     6949 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/screen_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.540203 subsearch-2.45.1/src/subsearch/gui/screens/
--rw-rw-rw-   0        0        0        0 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/screens/__init__.py
--rw-rw-rw-   0        0        0     5727 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/screens/download_manager.py
--rw-rw-rw-   0        0        0     2935 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/screens/language_options.py
--rw-rw-rw-   0        0        0    15230 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/screens/search_options.py
--rw-rw-rw-   0        0        0    13523 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/screens/subsearch_options.py
--rw-rw-rw-   0        0        0     1195 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/gui/system_tray.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.540203 subsearch-2.45.1/src/subsearch/providers/
--rw-rw-rw-   0        0        0        2 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/providers/__init__.py
--rw-rw-rw-   0        0        0     5947 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/providers/common_utils.py
--rw-rw-rw-   0        0        0     3172 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/providers/opensubtitles.py
--rw-rw-rw-   0        0        0     3330 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/providers/subscene.py
--rw-rw-rw-   0        0        0     2459 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/providers/yifysubtitles.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:31:39.540203 subsearch-2.45.1/src/subsearch/utils/
--rw-rw-rw-   0        0        0        2 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/__init__.py
--rw-rw-rw-   0        0        0     1992 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/imdb_lookup.py
--rw-rw-rw-   0        0        0     4803 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/io_app.py
--rw-rw-rw-   0        0        0     6344 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/io_file_system.py
--rw-rw-rw-   0        0        0     4094 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/io_toml.py
--rw-rw-rw-   0        0        0     4424 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/io_winreg.py
--rw-rw-rw-   0        0        0     8453 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/string_parser.py
--rw-rw-rw-   0        0        0     2890 2024-05-12 16:31:02.000000 subsearch-2.45.1/src/subsearch/utils/update.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.885909 subsearch-2.46.0/
+-rw-rw-rw-   0        0        0     1093 2024-05-15 13:30:44.000000 subsearch-2.46.0/LICENSE
+-rw-rw-rw-   0        0        0      198 2024-05-15 13:30:44.000000 subsearch-2.46.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7491 2024-05-15 13:31:25.885909 subsearch-2.46.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5741 2024-05-15 13:30:44.000000 subsearch-2.46.0/README.md
+-rw-rw-rw-   0        0        0     2556 2024-05-15 13:30:44.000000 subsearch-2.46.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-15 13:31:25.885909 subsearch-2.46.0/setup.cfg
+-rw-rw-rw-   0        0        0      114 2024-05-15 13:30:44.000000 subsearch-2.46.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.854654 subsearch-2.46.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.885909 subsearch-2.46.0/src/Subsearch.egg-info/
+-rw-rw-rw-   0        0        0     7491 2024-05-15 13:31:25.000000 subsearch-2.46.0/src/Subsearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2042 2024-05-15 13:31:25.000000 subsearch-2.46.0/src/Subsearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 13:31:25.000000 subsearch-2.46.0/src/Subsearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-15 13:31:25.000000 subsearch-2.46.0/src/Subsearch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 13:31:25.000000 subsearch-2.46.0/src/Subsearch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      377 2024-05-15 13:31:25.000000 subsearch-2.46.0/src/Subsearch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-15 13:31:25.000000 subsearch-2.46.0/src/Subsearch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.870283 subsearch-2.46.0/src/subsearch/
+-rw-rw-rw-   0        0        0     1368 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/__init__.py
+-rw-rw-rw-   0        0        0       38 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/__main__.py
+-rw-rw-rw-   0        0        0     9275 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/core.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.870283 subsearch-2.46.0/src/subsearch/data/
+-rw-rw-rw-   0        0        0       99 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/data/__init__.py
+-rw-rw-rw-   0        0        0       53 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/data/guid.py
+-rw-rw-rw-   0        0        0     5959 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/data/language_data.toml
+-rw-rw-rw-   0        0        0       24 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/data/version.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.870283 subsearch-2.46.0/src/subsearch/globals/
+-rw-rw-rw-   0        0        0       48 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/__init__.py
+-rw-rw-rw-   0        0        0     6457 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/_logging.py
+-rw-rw-rw-   0        0        0      513 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/constants.py
+-rw-rw-rw-   0        0        0     2394 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/dataclasses.py
+-rw-rw-rw-   0        0        0     4985 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/decorators.py
+-rw-rw-rw-   0        0        0      980 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/exceptions.py
+-rw-rw-rw-   0        0        0      258 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/metaclasses.py
+-rw-rw-rw-   0        0        0     1269 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/globals/thread_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.870283 subsearch-2.46.0/src/subsearch/gui/
+-rw-rw-rw-   0        0        0      588 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/__init__.py
+-rw-rw-rw-   0        0        0     3180 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/common_utils.py
+-rw-rw-rw-   0        0        0     1053 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resource_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.870283 subsearch-2.46.0/src/subsearch/gui/resources/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.870283 subsearch-2.46.0/src/subsearch/gui/resources/assets/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/assets/__init__.py
+-rw-rw-rw-   0        0        0     7119 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/assets/spritesheet.png
+-rw-rw-rw-   0        0        0   105808 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/assets/subsearch.ico
+-rw-rw-rw-   0        0        0     1674 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/config.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.870283 subsearch-2.46.0/src/subsearch/gui/resources/styles/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/styles/__init__.py
+-rw-rw-rw-   0        0        0     1780 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/styles/sprites.tcl
+-rw-rw-rw-   0        0        0     7247 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/styles/style_subsearch.tcl
+-rw-rw-rw-   0        0        0     1451 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/resources/styles/theme_setter.tcl
+-rw-rw-rw-   0        0        0     6949 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/screen_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.885909 subsearch-2.46.0/src/subsearch/gui/screens/
+-rw-rw-rw-   0        0        0        0 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/screens/__init__.py
+-rw-rw-rw-   0        0        0     5568 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/screens/download_manager.py
+-rw-rw-rw-   0        0        0     2935 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/screens/language_options.py
+-rw-rw-rw-   0        0        0    15188 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/screens/search_options.py
+-rw-rw-rw-   0        0        0    13523 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/screens/subsearch_options.py
+-rw-rw-rw-   0        0        0     1195 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/gui/system_tray.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.885909 subsearch-2.46.0/src/subsearch/providers/
+-rw-rw-rw-   0        0        0        2 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/providers/__init__.py
+-rw-rw-rw-   0        0        0     3585 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/providers/common_utils.py
+-rw-rw-rw-   0        0        0     3172 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/providers/opensubtitles.py
+-rw-rw-rw-   0        0        0     2469 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/providers/yifysubtitles.py
+drwxrwxrwx   0        0        0        0 2024-05-15 13:31:25.885909 subsearch-2.46.0/src/subsearch/utils/
+-rw-rw-rw-   0        0        0        2 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/__init__.py
+-rw-rw-rw-   0        0        0     1992 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/imdb_lookup.py
+-rw-rw-rw-   0        0        0     4787 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/io_app.py
+-rw-rw-rw-   0        0        0     6344 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/io_file_system.py
+-rw-rw-rw-   0        0        0     4094 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/io_toml.py
+-rw-rw-rw-   0        0        0     4424 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/io_winreg.py
+-rw-rw-rw-   0        0        0     7908 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/string_parser.py
+-rw-rw-rw-   0        0        0     2890 2024-05-15 13:30:44.000000 subsearch-2.46.0/src/subsearch/utils/update.py
```

### Comparing `subsearch-2.45.1/LICENSE` & `subsearch-2.46.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/PKG-INFO` & `subsearch-2.46.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.45.1
+Version: 2.46.0
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subtitles,sub,srt,tool,tools,download,movies,shows,scrape,opensubtitles,subscene,subsearch,subtitles,yifysubtitles
 Platform: win32
```

### Comparing `subsearch-2.45.1/README.md` & `subsearch-2.46.0/README.md`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/pyproject.toml` & `subsearch-2.46.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/Subsearch.egg-info/PKG-INFO` & `subsearch-2.46.0/src/Subsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.45.1
+Version: 2.46.0
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subtitles,sub,srt,tool,tools,download,movies,shows,scrape,opensubtitles,subscene,subsearch,subtitles,yifysubtitles
 Platform: win32
```

### Comparing `subsearch-2.45.1/src/Subsearch.egg-info/SOURCES.txt` & `subsearch-2.46.0/src/Subsearch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 src/subsearch/gui/screens/download_manager.py
 src/subsearch/gui/screens/language_options.py
 src/subsearch/gui/screens/search_options.py
 src/subsearch/gui/screens/subsearch_options.py
 src/subsearch/providers/__init__.py
 src/subsearch/providers/common_utils.py
 src/subsearch/providers/opensubtitles.py
-src/subsearch/providers/subscene.py
 src/subsearch/providers/yifysubtitles.py
 src/subsearch/utils/__init__.py
 src/subsearch/utils/imdb_lookup.py
 src/subsearch/utils/io_app.py
 src/subsearch/utils/io_file_system.py
 src/subsearch/utils/io_toml.py
 src/subsearch/utils/io_winreg.py
```

### Comparing `subsearch-2.45.1/src/subsearch/__init__.py` & `subsearch-2.46.0/src/subsearch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,23 +15,20 @@
 class Subsearch:
     def __init__(self) -> None:
         self.subsearch_core = core.SubsearchCore(PREF_COUNTER)
 
     def search_for_subtitles(self) -> None:
         self.subsearch_core.init_search(
             self.provider_opensubtitles,
-            self.provider_subscene,
             self.provider_yifysubtitles,
         )
 
     def provider_opensubtitles(self) -> None:
         self.subsearch_core.opensubtitles()
 
-    def provider_subscene(self) -> None:
-        self.subsearch_core.subscene()
 
     def provider_yifysubtitles(self) -> None:
         self.subsearch_core.yifysubtitles()
 
     def process_files(self) -> None:
         self.subsearch_core.download_files()
         self.subsearch_core.download_manager()
```

### Comparing `subsearch-2.45.1/src/subsearch/core.py` & `subsearch-2.46.0/src/subsearch/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Callable
 
 from subsearch.globals import decorators, log, thread_handle
 from subsearch.globals.constants import APP_PATHS, DEVICE_INFO, FILE_PATHS, VIDEO_FILE
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.gui import screen_manager, system_tray
 from subsearch.gui.screens import download_manager
-from subsearch.providers import opensubtitles, subscene, yifysubtitles
+from subsearch.providers import opensubtitles, yifysubtitles
 from subsearch.utils import io_file_system, io_toml, string_parser
 
 
 class Initializer:
     def __init__(self, pref_counter: float) -> None:
         log.brackets("Initializing")
         log.stdout(f"Loading components...", level="info", end_new_line=True)
@@ -61,16 +61,15 @@
         io_file_system.del_directory_content(APP_PATHS.tmp_dir)
         if self.file_exist:
             io_file_system.create_directory(VIDEO_FILE.subs_dir)
             io_file_system.create_directory(VIDEO_FILE.tmp_dir)
 
     def all_providers_disabled(self) -> bool:
         if (
-            self.app_config.providers["subscene_site"] is False
-            and self.app_config.providers["opensubtitles_site"] is False
+            self.app_config.providers["opensubtitles_site"] is False
             and self.app_config.providers["opensubtitles_hash"] is False
             and self.app_config.providers["yifysubtitles_site"] is False
         ):
             return True
         return False
 
 
@@ -99,35 +98,28 @@
         for thread_count, target in enumerate(tasks, start=1):
             func_name = str(target.__name__).split("_")[-1]
             name = f"thread_{thread_count}_{func_name}"
             task_thread = thread_handle.CreateThread(target=target, name=name)
             task_thread.start()
             task_thread.join()
 
-    def start_search(self, provider, flag: str = "") -> None:
+    def _start_search(self, provider, flag: str) -> None:
         search_provider = provider(**self.search_kwargs)
-        if flag:
-            search_provider.start_search(flag=flag)
-        else:
-            search_provider.start_search()
+        search_provider.start_search(flag=flag)
         self.accepted_subtitles.extend(search_provider.accepted_subtitles)
         self.rejected_subtitles.extend(search_provider.rejected_subtitles)
 
     @decorators.call_func
     def opensubtitles(self) -> None:
-        self.start_search(provider=opensubtitles.OpenSubtitles, flag="hash")
-        self.start_search(provider=opensubtitles.OpenSubtitles, flag="site")
-
-    @decorators.call_func
-    def subscene(self) -> None:
-        self.start_search(provider=subscene.Subscene)
+        self._start_search(provider=opensubtitles.OpenSubtitles, flag="hash")
+        self._start_search(provider=opensubtitles.OpenSubtitles, flag="site")
 
     @decorators.call_func
     def yifysubtitles(self) -> None:
-        self.start_search(provider=yifysubtitles.YifiSubtitles)
+        self._start_search(provider=yifysubtitles.YifiSubtitles, flag="site")
 
     @decorators.call_func
     def download_files(self) -> None:
         log.brackets(f"Downloading subtitles")
         index_size = len(self.accepted_subtitles)
         for enum, subtitle in enumerate(self.accepted_subtitles, 1):
             io_file_system.download_subtitle(subtitle, enum, index_size)
```

### Comparing `subsearch-2.45.1/src/subsearch/globals/_logging.py` & `subsearch-2.46.0/src/subsearch/globals/_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import dataclasses
 import inspect
 import threading
 from datetime import datetime
 from pathlib import Path
-from typing import Optional, TypeVar
+from typing import Callable, Optional
 
 import picologging as logging
 
 from subsearch.globals import metaclasses
 from subsearch.globals.constants import APP_PATHS, FILE_PATHS
+from subsearch.globals.dataclasses import GenericDataClass
 
-DATACLASS = TypeVar("DATACLASS")
 
-
-def capture_call_info(func):
+def capture_call_info(func) -> Callable[..., None]:
     def wrapper(*args, **kwargs):
         frame = inspect.currentframe().f_back  # type: ignore
         current_time = datetime.now().time()
         call_time = current_time.strftime("%H:%M:%S.%f")[:-3]
         kwargs["call_module"] = frame.f_globals["__name__"].split(".")[-1]  # type: ignore
         kwargs["call_lineno"] = frame.f_lineno  # type: ignore
         kwargs["call_ct"] = call_time
@@ -32,15 +31,15 @@
     """
 
     RESET = "\033[0m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
 
 
-class Logger(metaclass=metaclasses.Singleton):
+class _Logging(metaclass=metaclasses.Singleton):
     def __init__(self, *args, **kwargs) -> None:
         self.logger_name = kwargs.get("logger_name", "subsearch")
         if not APP_PATHS.appdata_subsearch.exists():
             APP_PATHS.appdata_subsearch.mkdir(parents=True, exist_ok=True)
         self.log_file_path = kwargs.get("debug_log_file", FILE_PATHS.log)
         self._debug_logger = self.create_logger()
         self._lock = threading.Lock()
@@ -94,17 +93,17 @@
 
     def _color_print(self, message: str, hex_color: str, style: str) -> None:
         color_code = self._hex_to_ansi(hex_color)
         style_code = getattr(self._ansi, style.upper()) if style != "" else ""
         print(f"{style_code}{color_code}{message}{self._ansi.RESET}")
 
 
-class StdoutHandler(metaclass=metaclasses.Singleton):
+class Logger(metaclass=metaclasses.Singleton):
     def __init__(self) -> None:
-        self._logger = Logger()
+        self._logger = _Logging()
 
     def __call__(self, message: str, **kwargs) -> None:
         self.log(message, **kwargs)
 
     def log(self, message: str, **kwargs) -> None:
         end_new_line = kwargs.get("end_new_line", False)
         self._logger.log(message, **kwargs)
@@ -149,15 +148,15 @@
 
         if not message:
             raise ValueError("Invalid action type")
 
         self(message, **kwargs)
 
     @capture_call_info
-    def dataclass(self, instance: DATACLASS, **kwargs) -> None:
+    def dataclass(self, instance: GenericDataClass, **kwargs) -> None:
         if not dataclasses.is_dataclass(instance):
             raise ValueError("Input is not a dataclass instance.")
         instance_name = f"--- [{instance.__class__.__name__}] ---"
         self(instance_name, hex_color="#fab387", style="bold", **kwargs)
         for field in dataclasses.fields(instance):
             key = field.name
             value = getattr(instance, key)
```

### Comparing `subsearch-2.45.1/src/subsearch/globals/constants.py` & `subsearch-2.46.0/src/subsearch/globals/constants.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/globals/dataclasses.py` & `subsearch-2.46.0/src/subsearch/globals/dataclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from dataclasses import dataclass
+from dataclasses import Field, dataclass
 from pathlib import Path
-from typing import Any
+from typing import Any, ClassVar, Protocol
 
 
 @dataclass(order=True)
 class LanguageData:
     name: str
     alpha_1: str
     alpha_2b: str
     incompatibility: list[str]
-    subscene_id: int
 
 
 @dataclass(order=True, slots=True)
 class ProviderAlphaCodeData:
     provider: str
     alpha_code: str
 
@@ -67,38 +66,28 @@
     open_on_no_matches: bool
     always_open: bool
     no_automatic_downloads: bool
     single_instance: bool
 
 
 @dataclass(order=True, slots=True)
-class SubsceneCookie:
-    dark_theme: bool
-    sort_subtitle_by_date: str
-    language_filter: int
-    hearing_impaired: int
-    foreigen_only: bool
-
-
-@dataclass(order=True, slots=True)
 class ReleaseData:
     title: str
     year: int
     season: str
     season_ordinal: str
     episode: str
     episode_ordinal: str
     tvseries: bool
     release: str
     group: str
 
 
 @dataclass(order=True, slots=True)
 class ProviderUrls:
-    subscene: str
     opensubtitles: str
     opensubtitles_hash: str
     yifysubtitles: str
 
 
 @dataclass(order=True, slots=True)
 class Subtitle:
@@ -119,7 +108,11 @@
 @dataclass(order=True, slots=True, frozen=True)
 class WindowsRegistryPaths:
     classes: str
     asterisk: str
     shell: str
     subsearch: str
     subsearch_command: str
+
+
+class GenericDataClass(Protocol):
+    __dataclass_fields__: ClassVar[dict[str, Field[Any]]]
```

### Comparing `subsearch-2.45.1/src/subsearch/globals/decorators.py` & `subsearch-2.46.0/src/subsearch/globals/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,18 +90,14 @@
         func_name = kwargs["func_name"]
         conditions: dict[str, list[bool]] = {
             "init_search": [],
             "opensubtitles": [
                 _CoreSubsearchFuncCondtitons.language_compatibility("opensubtitles"),
                 cfg.providers["opensubtitles_hash"] or cfg.providers["opensubtitles_site"],
             ],
-            "subscene": [
-                _CoreSubsearchFuncCondtitons.language_compatibility("subscene"),
-                cfg.providers["subscene_site"],
-            ],
             "yifysubtitles": [
                 not cfg.only_foreign_parts,
                 _CoreSubsearchFuncCondtitons.language_compatibility("yifysubtitles"),
                 not cls.release_data.tvseries,
                 not cls.provider_urls.yifysubtitles == "",
                 cfg.providers["yifysubtitles_site"],
             ],
```

### Comparing `subsearch-2.45.1/src/subsearch/globals/exceptions.py` & `subsearch-2.46.0/src/subsearch/globals/exceptions.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/globals/thread_handle.py` & `subsearch-2.46.0/src/subsearch/globals/thread_handle.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/__init__.py` & `subsearch-2.46.0/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/common_utils.py` & `subsearch-2.46.0/src/subsearch/gui/common_utils.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/resource_loader.py` & `subsearch-2.46.0/src/subsearch/gui/resource_loader.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/resources/assets/spritesheet.png` & `subsearch-2.46.0/src/subsearch/gui/resources/assets/spritesheet.png`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/resources/assets/subsearch.ico` & `subsearch-2.46.0/src/subsearch/gui/resources/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/resources/config.py` & `subsearch-2.46.0/src/subsearch/gui/resources/config.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/resources/styles/sprites.tcl` & `subsearch-2.46.0/src/subsearch/gui/resources/styles/sprites.tcl`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/resources/styles/style_subsearch.tcl` & `subsearch-2.46.0/src/subsearch/gui/resources/styles/style_subsearch.tcl`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/resources/styles/theme_setter.tcl` & `subsearch-2.46.0/src/subsearch/gui/resources/styles/theme_setter.tcl`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/screen_manager.py` & `subsearch-2.46.0/src/subsearch/gui/screen_manager.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/screens/download_manager.py` & `subsearch-2.46.0/src/subsearch/gui/screens/download_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,14 @@
         self.sub_listbox.unbind("<<ListboxSelect>>")
         _selection = self.sub_listbox.curselection()
         selection = _selection[0]
         subtitle = self.listbox_index[selection]
         if subtitle in (self.downloaded_subtitle or self.failed_subtitle_downloads):
             self.sub_listbox.bind("<ButtonPress-1>", self.mouse_b1_press)
             return
-        if subtitle.provider == "subscene":
-            subtitle.download_url = common_utils.ProviderHelper.subscene_get_download_url(subtitle.download_url)
         self.update_text(selection, "⊙", subtitle, cfg.color.orange)
         self.sub_listbox.bind("<ButtonRelease-1>", lambda event: self.download(event, subtitle, selection))
 
     def download(self, event, subtitle: Subtitle, selection: int) -> None:
         self.sub_listbox.unbind("<ButtonRelease-1>")
         try:
             if string_parser.valid_filename(subtitle.release_name):
```

### Comparing `subsearch-2.45.1/src/subsearch/gui/screens/language_options.py` & `subsearch-2.46.0/src/subsearch/gui/screens/language_options.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/screens/search_options.py` & `subsearch-2.46.0/src/subsearch/gui/screens/search_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         self.data = io_toml.load_toml_data(FILE_PATHS.config)
         self.chekboxes = {}
         self.last_key = ""
 
         self.provider_options: dict = {
             "opensubtitles_site": "Opensubtitles",
             "opensubtitles_hash": "Opensubtitles with hash",
-            "subscene_site": "Subscene",
             "yifysubtitles_site": "YIFYsubtitles",
         }
         for name, description in self.provider_options.items():
             self.provider_options[name] = [
                 io_toml.load_toml_value(FILE_PATHS.config, "providers")[name],
                 description,
             ]
```

### Comparing `subsearch-2.45.1/src/subsearch/gui/screens/subsearch_options.py` & `subsearch-2.46.0/src/subsearch/gui/screens/subsearch_options.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/gui/system_tray.py` & `subsearch-2.46.0/src/subsearch/gui/system_tray.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/providers/opensubtitles.py` & `subsearch-2.46.0/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/providers/subscene.py` & `subsearch-2.46.0/src/subsearch/providers/yifysubtitles.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,59 @@
 from selectolax.parser import Node
 
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.providers import common_utils
 
 
-class SubsceneScraper(common_utils.ProviderHelper):
+class YifySubtitlesScraper(common_utils.ProviderHelper):
     def __init__(self, **kwargs) -> None:
         common_utils.ProviderHelper.__init__(self, **kwargs)
 
-    def find_title(self, url: str, current_language: str, definitive_match: list[str]) -> str | None:
-        tree = common_utils.get_html_parser(url)
-        products = tree.css("div.title")
-        for item in products:
-            node = item.css_first("a")
-            result_href = node.attributes["href"]
-            result_title = str(node.child.html).lower()  # type: ignore
-            if result_title not in definitive_match:
-                continue
-            current_language = current_language.lower()
-            return f"https://subscene.com{result_href}/{current_language}"
-
-    def skip_item(self, item: Node, hi_sub: bool, regular_sub: bool) -> bool:
-        if item.css_matches("td.banner-inlist"):
+    def skip_item(self, item: Node, hi_sub: bool, regular_sub: bool, current_language: str) -> bool:
+        subtitle_language = item.css_first("span.sub-lang").child.text_content  # type: ignore
+        hearing_impaired = item.css_matches("span.hi-subtitle")
+        if subtitle_language.lower() != current_language.lower():  # type: ignore
             return True
         if (hi_sub and regular_sub) or (hi_sub is False and regular_sub is False):
             pass
-        elif hi_sub is False and item.css_matches("td.a40"):
+        elif hi_sub is False and hearing_impaired:
             return True
-        elif regular_sub is False and item.css_matches("td.a41"):
+        elif regular_sub is True and hearing_impaired:
             return True
         return False
 
-    def find_subtitles(self, url: str, hi_sub: bool, regular_sub: bool, subscene_header) -> dict[str, str]:
+    def get_subtitle(self, url: str, current_language: str, hi_sub: bool, non_hi_sub: bool) -> dict[str, str]:
         subtitles: dict[str, str] = {}
-        tree = common_utils.get_html_parser(url, subscene_header)
-        products = tree.css("tr")
-        for item in products[1:]:
-            if self.skip_item(item, hi_sub, regular_sub):
+        tree = common_utils.get_html_parser(url)
+        product = tree.select("tr")
+        for item in product.matches[1:]:  # type: ignore
+            if self.skip_item(item, hi_sub, non_hi_sub, current_language):
                 continue
             node = item.css_first("a")
-            if node.child.text_content == "upload":  # type: ignore
-                continue
-            subtitle_href = node.attributes["href"]
-            filename = item.css_first("span:nth-child(2)").child.text_content.strip()  # type: ignore
-            subtitles[filename] = f"https://subscene.com{subtitle_href}"
+            titles = node.text().strip().split("subtitle ")[-1].split("\n")
+            _href = node.attributes["href"].split("/")  # type: ignore
+            href = _href[-1]
+            for title in titles:
+                subtitles[title] = f"https://yifysubtitles.org/subtitle/{href}.zip"
         return subtitles
 
 
-class Subscene(SubsceneScraper):
+class YifiSubtitles(YifySubtitlesScraper):
     def __init__(self, **kwargs) -> None:
-        SubsceneScraper.__init__(self, **kwargs)
+        YifySubtitlesScraper.__init__(self, **kwargs)
         self.provider_name = self.__class__.__name__.lower()
 
-    def start_search(self):
-        custom_subscene_header = common_utils.CustomSubsceneHeader(self.app_config)
-        header = custom_subscene_header.create_header()
-        definitive_match = self._definitive_match()
-        found_title_url = self.find_title(self.url_subscene, self.current_language, definitive_match)
+    def start_search(self, **kwargs) -> list[Subtitle] | None:
+        subtitle_data = self.get_subtitle(self.url_yifysubtitles, self.current_language, self.hi_sub, self.non_hi_sub)
 
-        if not found_title_url:
+        if not subtitle_data:
             return []
 
-        subtitle_data = self.find_subtitles(found_title_url, self.hi_sub, self.non_hi_sub, header)
         self._process_subtitle_data(self.provider_name, subtitle_data)
 
-    def _definitive_match(self) -> list[str]:
-        if self.tvseries:
-            return [f"{self.title} - {self.season_ordinal} season"]
-        return [f"{self.title} ({self.year})", f"{self.title} ({(self.year-1)})"]
-
     @property
     def accepted_subtitles(self) -> list[Subtitle]:
         return self._accepted_subtitles
 
     @property
     def rejected_subtitles(self) -> list[Subtitle]:
         return self._rejected_subtitles
```

### Comparing `subsearch-2.45.1/src/subsearch/utils/imdb_lookup.py` & `subsearch-2.46.0/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/utils/io_app.py` & `subsearch-2.46.0/src/subsearch/utils/io_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         "swf",
         "mswmm",
     ]
     return exts
 
 
 def get_supported_providers() -> list[str]:
-    providers = ["opensubtitles_site", "opensubtitles_hash", "subscene_site", "yifysubtitles_site"]
+    providers = ["opensubtitles_site", "opensubtitles_hash",  "yifysubtitles_site"]
     return providers
 
 
 def get_windows_registry_paths() -> WindowsRegistryPaths:
     registry_paths = WindowsRegistryPaths(
         classes=r"Software\Classes",
         asterisk=r"Software\Classes\*",
```

### Comparing `subsearch-2.45.1/src/subsearch/utils/io_file_system.py` & `subsearch-2.46.0/src/subsearch/utils/io_file_system.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/utils/io_toml.py` & `subsearch-2.46.0/src/subsearch/utils/io_toml.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/utils/io_winreg.py` & `subsearch-2.46.0/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.45.1/src/subsearch/utils/string_parser.py` & `subsearch-2.46.0/src/subsearch/utils/string_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,22 +79,16 @@
     def __init__(self, app_config: AppConfig, release_data: ReleaseData, language_data: dict[str, Any]) -> None:
         self.app_config = app_config
         self.release_data = release_data
         self.language_data = language_data
         self.current_language_data: LanguageData = LanguageData(**language_data[app_config.language])
 
     def retrieve_urls(self) -> ProviderUrls:
-        return ProviderUrls(self.subscene(), self.opensubtitles(), self.opensubtitles_hash(), self.yifysubtitles())
+        return ProviderUrls(self.opensubtitles(), self.opensubtitles_hash(), self.yifysubtitles())
 
-    def subscene(self) -> str:
-        domain = "https://subscene.com"
-        query = "subtitles/searchbytitle?query"
-        search_parameters = self._subscene_search_parameters()
-        url_subscene = f"{domain}/{query}={search_parameters}"
-        return url_subscene.replace(" ", "%20")
 
     def opensubtitles(self) -> str:
         domain = "https://www.opensubtitles.org"
         subtitle_type = self._opensubtitles_subtitle_type()
         search_parameters = self._opensubtitles_search_parameters()
         return f"{domain}/{subtitle_type}/{search_parameters}/rss_2_00".replace(" ", "%20")
 
@@ -106,18 +100,14 @@
     def yifysubtitles(self) -> str:
         if self.release_data.tvseries:
             return ""
         domain = "https://yifysubtitles.org"
         tt_id = imdb_lookup.FindImdbID(self.release_data.title, self.release_data.year).id
         return f"{domain}/movie-imdb/{tt_id}" if tt_id is not None else ""
 
-    def _subscene_search_parameters(self) -> str:
-        if self.release_data.tvseries:
-            return f"{self.release_data.title} - {self.release_data.season_ordinal} season"
-        return f"{self.release_data.title}"
 
     def _opensubtitles_subtitle_type(self) -> str:
         alpha_2b = self.current_language_data.alpha_2b
         hearing_imparied, hearing_imparied_foreign_parts, foreign_parts = self.subtitle_type_logic()
         if hearing_imparied:
             return f"en/search/sublanguageid-{alpha_2b}/hearingimpaired-on"
         elif foreign_parts:
```

### Comparing `subsearch-2.45.1/src/subsearch/utils/update.py` & `subsearch-2.46.0/src/subsearch/utils/update.py`

 * *Files identical despite different names*

