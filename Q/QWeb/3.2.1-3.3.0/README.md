# Comparing `tmp/QWeb-3.2.1.tar.gz` & `tmp/QWeb-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QWeb-3.2.1.tar", last modified: Mon Apr  8 06:20:29 2024, max compression
+gzip compressed data, was "QWeb-3.3.0.tar", last modified: Wed May 15 06:40:07 2024, max compression
```

## Comparing `QWeb-3.2.1.tar` & `QWeb-3.3.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 06:20:29.929434 QWeb-3.2.1/
--rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-3.2.1/LICENSE
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11340 2024-04-08 06:20:29.930671 QWeb-3.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 06:20:29.953351 QWeb-3.2.1/QWeb/
--rw-rw-rw-   0        0        0    16564 2024-01-26 10:08:26.000000 QWeb-3.2.1/QWeb/__init__.py
--rw-rw-rw-   0        0        0     2283 2024-01-26 10:08:26.000000 QWeb-3.2.1/QWeb/__main__.py
--rw-rw-rw-   0        0        0      519 2024-04-08 06:20:29.953351 QWeb-3.2.1/QWeb/_version.py
--rw-rw-rw-   0        0        0     1408 2023-12-20 13:58:51.000000 QWeb-3.2.1/QWeb/custom_config.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:20:29.406277 QWeb-3.2.1/QWeb/internal/
--rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-3.2.1/QWeb/internal/__init__.py
--rw-rw-rw-   0        0        0    22031 2024-04-05 12:00:29.000000 QWeb-3.2.1/QWeb/internal/actions.py
--rw-rw-rw-   0        0        0     3840 2022-06-16 12:12:06.000000 QWeb-3.2.1/QWeb/internal/ajax.py
--rw-rw-rw-   0        0        0     1699 2022-06-16 12:12:06.000000 QWeb-3.2.1/QWeb/internal/alert.py
--rw-rw-rw-   0        0        0     3689 2022-06-16 12:12:06.000000 QWeb-3.2.1/QWeb/internal/blocks.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:20:29.524738 QWeb-3.2.1/QWeb/internal/browser/
--rw-rw-rw-   0        0        0     5495 2023-04-26 08:15:55.000000 QWeb-3.2.1/QWeb/internal/browser/__init__.py
--rw-rw-rw-   0        0        0     1581 2023-10-20 07:45:42.000000 QWeb-3.2.1/QWeb/internal/browser/android.py
--rw-rw-rw-   0        0        0     3419 2024-01-26 10:08:26.000000 QWeb-3.2.1/QWeb/internal/browser/bs_desktop.py
--rw-rw-rw-   0        0        0     2162 2024-01-26 10:08:26.000000 QWeb-3.2.1/QWeb/internal/browser/bs_mobile.py
--rw-rw-rw-   0        0        0     6161 2023-11-10 09:40:45.000000 QWeb-3.2.1/QWeb/internal/browser/chrome.py
--rw-rw-rw-   0        0        0     4108 2023-10-20 07:45:42.000000 QWeb-3.2.1/QWeb/internal/browser/edge.py
--rw-rw-rw-   0        0        0     4975 2023-10-20 07:45:42.000000 QWeb-3.2.1/QWeb/internal/browser/firefox.py
--rw-rw-rw-   0        0        0     1934 2023-12-20 13:58:51.000000 QWeb-3.2.1/QWeb/internal/browser/safari.py
--rw-rw-rw-   0        0        0     6626 2022-11-22 10:56:24.000000 QWeb-3.2.1/QWeb/internal/checkbox.py
--rw-rw-rw-   0        0        0     4329 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/internal/config.py
--rw-rw-rw-   0        0        0     4379 2022-06-16 12:12:06.000000 QWeb-3.2.1/QWeb/internal/config_defaults.py
--rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-3.2.1/QWeb/internal/cookies.py
--rw-rw-rw-   0        0        0     9346 2024-04-02 14:06:24.000000 QWeb-3.2.1/QWeb/internal/decorators.py
--rw-rw-rw-   0        0        0     5613 2024-01-26 10:08:26.000000 QWeb-3.2.1/QWeb/internal/download.py
--rw-rw-rw-   0        0        0     3143 2023-10-20 07:45:42.000000 QWeb-3.2.1/QWeb/internal/dragdrop.py
--rw-rw-rw-   0        0        0     7808 2022-12-12 14:30:56.000000 QWeb-3.2.1/QWeb/internal/dropdown.py
--rw-rw-rw-   0        0        0    29790 2024-04-02 14:06:24.000000 QWeb-3.2.1/QWeb/internal/element.py
--rw-rw-rw-   0        0        0     3087 2022-06-16 12:12:06.000000 QWeb-3.2.1/QWeb/internal/exceptions.py
--rw-rw-rw-   0        0        0     3463 2022-12-09 08:03:29.000000 QWeb-3.2.1/QWeb/internal/file.py
--rw-rw-rw-   0        0        0    11924 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/internal/frame.py
--rw-rw-rw-   0        0        0     1960 2023-09-12 08:26:02.000000 QWeb-3.2.1/QWeb/internal/frame_checker.py
--rw-rw-rw-   0        0        0    20876 2023-12-20 13:58:51.000000 QWeb-3.2.1/QWeb/internal/icon.py
--rw-rw-rw-   0        0        0    11050 2023-08-02 09:59:23.000000 QWeb-3.2.1/QWeb/internal/input_.py
--rw-rw-rw-   0        0        0     7282 2024-04-05 12:00:29.000000 QWeb-3.2.1/QWeb/internal/input_handler.py
--rw-rw-rw-   0        0        0    21104 2023-09-12 08:44:36.000000 QWeb-3.2.1/QWeb/internal/javascript.py
--rw-rw-rw-   0        0        0     9479 2022-11-22 10:56:24.000000 QWeb-3.2.1/QWeb/internal/lists.py
--rw-rw-rw-   0        0        0     3194 2022-06-16 12:12:06.000000 QWeb-3.2.1/QWeb/internal/meas.py
--rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-3.2.1/QWeb/internal/platform.py
--rw-rw-rw-   0        0        0    13395 2023-09-05 13:39:03.000000 QWeb-3.2.1/QWeb/internal/screenshot.py
--rw-rw-rw-   0        0        0     7250 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/internal/search_strategy.py
--rw-rw-rw-   0        0        0     8673 2024-01-26 10:08:26.000000 QWeb-3.2.1/QWeb/internal/secrets.py
--rw-rw-rw-   0        0        0    17095 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/internal/table.py
--rw-rw-rw-   0        0        0    18553 2024-04-05 12:00:29.000000 QWeb-3.2.1/QWeb/internal/text.py
--rw-rw-rw-   0        0        0     1411 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/internal/user.py
--rw-rw-rw-   0        0        0    13538 2024-04-05 12:00:29.000000 QWeb-3.2.1/QWeb/internal/util.py
--rw-rw-rw-   0        0        0     4423 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/internal/window.py
--rw-rw-rw-   0        0        0     3321 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/internal/xhr.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:20:29.925590 QWeb-3.2.1/QWeb/keywords/
--rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.2.1/QWeb/keywords/__init__.py
--rw-rw-rw-   0        0        0     4238 2022-12-09 08:03:37.000000 QWeb-3.2.1/QWeb/keywords/ajax.py
--rw-rw-rw-   0        0        0     4920 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/keywords/alert.py
--rw-rw-rw-   0        0        0     5910 2024-04-05 12:00:29.000000 QWeb-3.2.1/QWeb/keywords/blocks.py
--rw-rw-rw-   0        0        0    24178 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/keywords/browser.py
--rw-rw-rw-   0        0        0    12960 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/keywords/checkbox.py
--rw-rw-rw-   0        0        0    37939 2024-03-08 11:59:59.000000 QWeb-3.2.1/QWeb/keywords/config.py
--rw-rw-rw-   0        0        0     3053 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/keywords/cookies.py
--rw-rw-rw-   0        0        0     2500 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/keywords/debug.py
--rw-rw-rw-   0        0        0     3998 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/keywords/download.py
--rw-rw-rw-   0        0        0     6268 2022-11-22 10:56:24.000000 QWeb-3.2.1/QWeb/keywords/dragdrop.py
--rw-rw-rw-   0        0        0    14590 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/keywords/dropdown.py
--rw-rw-rw-   0        0        0    27838 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/keywords/element.py
--rw-rw-rw-   0        0        0    12455 2023-09-05 13:39:03.000000 QWeb-3.2.1/QWeb/keywords/file.py
--rw-rw-rw-   0        0        0     4612 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/keywords/frame.py
--rw-rw-rw-   0        0        0     8675 2023-03-23 15:17:25.000000 QWeb-3.2.1/QWeb/keywords/icon.py
--rw-rw-rw-   0        0        0    38042 2024-01-26 10:08:26.000000 QWeb-3.2.1/QWeb/keywords/input_.py
--rw-rw-rw-   0        0        0     1887 2023-12-20 13:58:51.000000 QWeb-3.2.1/QWeb/keywords/javascript.py
--rw-rw-rw-   0        0        0     8703 2022-11-21 09:35:10.000000 QWeb-3.2.1/QWeb/keywords/lists.py
--rw-rw-rw-   0        0        0     2968 2023-12-20 13:58:51.000000 QWeb-3.2.1/QWeb/keywords/screenshot.py
--rw-rw-rw-   0        0        0     8486 2022-06-16 12:12:07.000000 QWeb-3.2.1/QWeb/keywords/search_strategy.py
--rw-rw-rw-   0        0        0    20611 2024-03-08 11:29:33.000000 QWeb-3.2.1/QWeb/keywords/table.py
--rw-rw-rw-   0        0        0    68435 2024-04-05 12:00:29.000000 QWeb-3.2.1/QWeb/keywords/text.py
--rw-rw-rw-   0        0        0    17323 2023-12-20 13:58:51.000000 QWeb-3.2.1/QWeb/keywords/window.py
-drwxrwxrwx   0        0        0        0 2024-04-08 06:20:29.010340 QWeb-3.2.1/QWeb.egg-info/
--rw-rw-rw-   0        0        0    11340 2024-04-08 06:20:28.000000 QWeb-3.2.1/QWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2024-04-08 06:20:28.000000 QWeb-3.2.1/QWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 06:20:28.000000 QWeb-3.2.1/QWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-3.2.1/QWeb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      351 2024-04-08 06:20:28.000000 QWeb-3.2.1/QWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 06:20:28.000000 QWeb-3.2.1/QWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10600 2023-10-20 07:45:42.000000 QWeb-3.2.1/README.md
--rw-rw-rw-   0        0        0     1209 2024-04-08 06:20:29.950568 QWeb-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2532 2024-04-05 12:00:29.000000 QWeb-3.2.1/setup.py
--rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-3.2.1/versioneer.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:40:07.543135 QWeb-3.3.0/
+-rw-rw-rw-   0        0        0    11558 2021-09-04 19:02:10.000000 QWeb-3.3.0/LICENSE
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11340 2024-05-15 06:40:07.543635 QWeb-3.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 06:40:07.553430 QWeb-3.3.0/QWeb/
+-rw-rw-rw-   0        0        0    16938 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/__init__.py
+-rw-rw-rw-   0        0        0     2259 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/__main__.py
+-rw-rw-rw-   0        0        0      519 2024-05-15 06:40:07.553947 QWeb-3.3.0/QWeb/_version.py
+-rw-rw-rw-   0        0        0     1408 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/custom_config.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:40:06.801869 QWeb-3.3.0/QWeb/internal/
+-rw-rw-rw-   0        0        0       64 2021-09-04 19:02:10.000000 QWeb-3.3.0/QWeb/internal/__init__.py
+-rw-rw-rw-   0        0        0    21711 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/actions.py
+-rw-rw-rw-   0        0        0     3671 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/ajax.py
+-rw-rw-rw-   0        0        0     1709 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/alert.py
+-rw-rw-rw-   0        0        0     3691 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/blocks.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:40:06.993141 QWeb-3.3.0/QWeb/internal/browser/
+-rw-rw-rw-   0        0        0     4879 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/__init__.py
+-rw-rw-rw-   0        0        0     1548 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/android.py
+-rw-rw-rw-   0        0        0     3426 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/bs_desktop.py
+-rw-rw-rw-   0        0        0     2166 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/bs_mobile.py
+-rw-rw-rw-   0        0        0     6072 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/chrome.py
+-rw-rw-rw-   0        0        0     4308 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/browser/edge.py
+-rw-rw-rw-   0        0        0     5093 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/browser/firefox.py
+-rw-rw-rw-   0        0        0     1884 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/browser/safari.py
+-rw-rw-rw-   0        0        0     6141 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/checkbox.py
+-rw-rw-rw-   0        0        0     4314 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/config.py
+-rw-rw-rw-   0        0        0     4442 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/config_defaults.py
+-rw-rw-rw-   0        0        0     1294 2022-11-22 10:56:24.000000 QWeb-3.3.0/QWeb/internal/cookies.py
+-rw-rw-rw-   0        0        0     9703 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/decorators.py
+-rw-rw-rw-   0        0        0     5625 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/download.py
+-rw-rw-rw-   0        0        0     3096 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/dragdrop.py
+-rw-rw-rw-   0        0        0     7881 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/dropdown.py
+-rw-rw-rw-   0        0        0    29827 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/element.py
+-rw-rw-rw-   0        0        0     3105 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/exceptions.py
+-rw-rw-rw-   0        0        0     3550 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/file.py
+-rw-rw-rw-   0        0        0    11694 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/frame.py
+-rw-rw-rw-   0        0        0     1960 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/frame_checker.py
+-rw-rw-rw-   0        0        0    21185 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/icon.py
+-rw-rw-rw-   0        0        0    10845 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/input_.py
+-rw-rw-rw-   0        0        0     7292 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/input_handler.py
+-rw-rw-rw-   0        0        0    21147 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/javascript.py
+-rw-rw-rw-   0        0        0     9115 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/lists.py
+-rw-rw-rw-   0        0        0     3180 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/meas.py
+-rw-rw-rw-   0        0        0      833 2022-06-16 12:12:06.000000 QWeb-3.3.0/QWeb/internal/platform.py
+-rw-rw-rw-   0        0        0    13285 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/screenshot.py
+-rw-rw-rw-   0        0        0     7236 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/search_strategy.py
+-rw-rw-rw-   0        0        0     8613 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/secrets.py
+-rw-rw-rw-   0        0        0    16553 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/table.py
+-rw-rw-rw-   0        0        0    18247 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/text.py
+-rw-rw-rw-   0        0        0     1373 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/user.py
+-rw-rw-rw-   0        0        0    13801 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/internal/util.py
+-rw-rw-rw-   0        0        0     4233 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/window.py
+-rw-rw-rw-   0        0        0     3303 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/internal/xhr.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:40:07.540136 QWeb-3.3.0/QWeb/keywords/
+-rw-rw-rw-   0        0        0       49 2021-09-04 19:02:10.000000 QWeb-3.3.0/QWeb/keywords/__init__.py
+-rw-rw-rw-   0        0        0     4473 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/ajax.py
+-rw-rw-rw-   0        0        0     4920 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/alert.py
+-rw-rw-rw-   0        0        0     5920 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/blocks.py
+-rw-rw-rw-   0        0        0    24523 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/browser.py
+-rw-rw-rw-   0        0        0    12198 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/checkbox.py
+-rw-rw-rw-   0        0        0    37935 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/config.py
+-rw-rw-rw-   0        0        0     3055 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/cookies.py
+-rw-rw-rw-   0        0        0     2508 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/debug.py
+-rw-rw-rw-   0        0        0     4028 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/download.py
+-rw-rw-rw-   0        0        0     6151 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/dragdrop.py
+-rw-rw-rw-   0        0        0    14990 2024-05-15 06:11:38.000000 QWeb-3.3.0/QWeb/keywords/dropdown.py
+-rw-rw-rw-   0        0        0    27779 2024-05-15 06:11:38.000000 QWeb-3.3.0/QWeb/keywords/element.py
+-rw-rw-rw-   0        0        0    14394 2024-05-15 06:11:38.000000 QWeb-3.3.0/QWeb/keywords/file.py
+-rw-rw-rw-   0        0        0     4624 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/frame.py
+-rw-rw-rw-   0        0        0    11998 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/icon.py
+-rw-rw-rw-   0        0        0    35769 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/input_.py
+-rw-rw-rw-   0        0        0     1887 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/javascript.py
+-rw-rw-rw-   0        0        0     8630 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/lists.py
+-rw-rw-rw-   0        0        0     2968 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/screenshot.py
+-rw-rw-rw-   0        0        0     8480 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/search_strategy.py
+-rw-rw-rw-   0        0        0    20397 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/table.py
+-rw-rw-rw-   0        0        0    66946 2024-05-06 12:35:56.000000 QWeb-3.3.0/QWeb/keywords/text.py
+-rw-rw-rw-   0        0        0    17192 2024-04-24 06:29:20.000000 QWeb-3.3.0/QWeb/keywords/window.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:40:05.890885 QWeb-3.3.0/QWeb.egg-info/
+-rw-rw-rw-   0        0        0    11340 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-09-08 09:34:25.000000 QWeb-3.3.0/QWeb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      351 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-15 06:40:05.000000 QWeb-3.3.0/QWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10600 2023-10-20 07:45:42.000000 QWeb-3.3.0/README.md
+-rw-rw-rw-   0        0        0     1209 2024-05-15 06:40:07.550763 QWeb-3.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2532 2024-04-05 12:00:29.000000 QWeb-3.3.0/setup.py
+-rw-rw-rw-   0        0        0    70433 2021-09-04 19:02:10.000000 QWeb-3.3.0/versioneer.py
```

### Comparing `QWeb-3.2.1/LICENSE` & `QWeb-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `QWeb-3.2.1/PKG-INFO` & `QWeb-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 3.2.1
+Version: 3.3.0
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `QWeb-3.2.1/QWeb/__init__.py` & `QWeb-3.3.0/QWeb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,39 @@
 import types
 import time
 
 from functools import wraps
 from QWeb import custom_config
 
 try:
-    from QWeb.keywords import (alert, browser, window, frame, element, text, checkbox, input_,
-                               javascript, screenshot, download, table, search_strategy, dropdown,
-                               cookies, config, icon, dragdrop, lists, file, debug, ajax, blocks)
+    from QWeb.keywords import (
+        alert,
+        browser,
+        window,
+        frame,
+        element,
+        text,
+        checkbox,
+        input_,
+        javascript,
+        screenshot,
+        download,
+        table,
+        search_strategy,
+        dropdown,
+        cookies,
+        config,
+        icon,
+        dragdrop,
+        lists,
+        file,
+        debug,
+        ajax,
+        blocks,
+    )
 
     from QWeb.internal import util
     from QWeb.internal.config_defaults import CONFIG
     from robot.api import logger
     from robot.utils import timestr_to_secs as _timestr_to_secs
     from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
     from robot.libraries import Dialogs
@@ -267,27 +289,51 @@
     .. tip:: It's preferable to use QWeb's automatic wait times instead of Sleep keyword.
 
        - **Sleep** keyword waits for the specified amount of time.
        - QWeb automatically waits until element is visible or until timeout limit is reached and
          then continue.
 
     """
-    ROBOT_LIBRARY_SCOPE = 'Global'
+
+    ROBOT_LIBRARY_SCOPE = "Global"
 
     def __init__(self, run_on_failure_keyword: str = "Log Screenshot") -> None:
-        '''Initializes the QWeb library and adds all the keywords to the instance.
+        """Initializes the QWeb library and adds all the keywords to the instance.
 
         - ``run_on_failure_keyword``:
           The keyword to run when a failure occurs. Default is "Log Screenshot".
 
-        '''
+        """
         self._run_on_failure_keyword = run_on_failure_keyword
-        for module in (alert, browser, window, frame, element, text, checkbox, input_, javascript,
-                       screenshot, custom_config, download, search_strategy, table, dropdown,
-                       cookies, config, icon, dragdrop, lists, file, debug, ajax, blocks):
+        for module in (
+            alert,
+            browser,
+            window,
+            frame,
+            element,
+            text,
+            checkbox,
+            input_,
+            javascript,
+            screenshot,
+            custom_config,
+            download,
+            search_strategy,
+            table,
+            dropdown,
+            cookies,
+            config,
+            icon,
+            dragdrop,
+            lists,
+            file,
+            debug,
+            ajax,
+            blocks,
+        ):
             for name in dir(module):
                 if not name.startswith("_"):
                     attr = getattr(module, name)
                     if isinstance(attr, types.FunctionType):
                         attr = self._run_on_failure_decorator(attr)
                         attr = self._xpath_decorator(attr)
                         setattr(self, name, attr)
@@ -297,46 +343,47 @@
 
         If keyword fails then this method executes self.run_on_failure_keyword.
         """
 
         @wraps(keyword_method)  # Preserves docstring of the original method.
         def inner(*args: Any, **kwargs: Any) -> None:  # pylint: disable=R1710
             kwargs = {k.lower(): v for k, v in kwargs.items()}  # Kwargs keys to lowercase
-            if 'type_secret' not in str(keyword_method):
-                logger.debug('args: {}, kwargs: {}'.format(args, kwargs))
+            if "type_secret" not in str(keyword_method):
+                logger.debug("args: {}, kwargs: {}".format(args, kwargs))
             try:
-                time.sleep(_timestr_to_secs(kwargs.get('delay', CONFIG['Delay'])))
-                run_before = CONFIG['RunBefore']
-                valid_pw = ['click', 'get_text', 'drop_down']
+                time.sleep(_timestr_to_secs(kwargs.get("delay", CONFIG["Delay"])))
+                run_before = CONFIG["RunBefore"]
+                valid_pw = ["click", "get_text", "drop_down"]
                 if run_before and any(pw in str(keyword_method) for pw in valid_pw):
-                    logger.info('executing run before kw {}'.format(run_before))
+                    logger.info("executing run before kw {}".format(run_before))
                     # robot fw or python syntax
                     if isinstance(run_before, list):
                         BuiltIn().run_keyword(run_before[0], *run_before[1:])
                     elif util.is_py_func(run_before):
                         eval(run_before)  # pylint: disable=W0123
                     else:
                         BuiltIn().run_keyword(run_before)
                 logger.trace(f"{keyword_method=}")
                 logger.trace(f"{args=}, {kwargs=}")
                 return keyword_method(*args, **kwargs)
             except Exception as e:  # pylint: disable=W0703
                 logger.debug(traceback.format_exc())
                 if not self._is_run_on_failure_keyword(keyword_method):
-                    if not util.par2bool(kwargs.get('skip_screenshot', False)):
+                    if not util.par2bool(kwargs.get("skip_screenshot", False)):
                         try:
                             BuiltIn().run_keyword(self._run_on_failure_keyword)
                         except RobotNotRunningError:
                             logger.debug("Robot not running")
-                devmode = util.par2bool(util.get_rfw_variable_value('${DEV_MODE}', False))
-                if devmode and not config.get_config('Debug_Run'):
-                    Dialogs.pause_execution('Keyword {} {} {} failed. \n'
-                                            'Got {}'.format(
-                                                str(keyword_method).split(' ')[1].upper(),
-                                                str(args), str(kwargs), e))
+                devmode = util.par2bool(util.get_rfw_variable_value("${DEV_MODE}", False))
+                if devmode and not config.get_config("Debug_Run"):
+                    Dialogs.pause_execution(
+                        "Keyword {} {} {} failed. \n" "Got {}".format(
+                            str(keyword_method).split(" ")[1].upper(), str(args), str(kwargs), e
+                        )
+                    )
                     debug.debug_on()
                 else:
                     raise
 
         return inner
 
     @staticmethod
@@ -344,30 +391,29 @@
         """Decorator method for selector-attribute. If selector attribute
         is given, method uses it's value and text to form simple xpath
         locator.
         """
 
         @wraps(keyword_method)  # Preserves docstring of the original method.
         def create_xpath(*args: Any, **kwargs: Any) -> Callable[..., Any]:
-            """Handle xpath before passing it to keyword.
-            """
+            """Handle xpath before passing it to keyword."""
             args_list = list(args)
-            if 'selector' in kwargs:
+            if "selector" in kwargs:
                 attr_value = str(args_list[0])
-                args_list[0] = '//*[@{}="{}"]'.format(kwargs['selector'], attr_value)
-                del kwargs['selector']
+                args_list[0] = '//*[@{}="{}"]'.format(kwargs["selector"], attr_value)
+                del kwargs["selector"]
                 args = tuple(args_list)
             return keyword_method(*args, **kwargs)
 
         return create_xpath
 
     def _is_run_on_failure_keyword(self, method: Callable[..., Any]) -> bool:
         """Helper function to find out if method name is the
-         one registered as kw to run on failure"""
+        one registered as kw to run on failure"""
         return self._run_on_failure_keyword.replace(" ", "_").lower() == method.__name__
 
 
 # pylint: disable=wrong-import-position
 from ._version import get_versions  # noqa: E402
 
-__version__ = get_versions()['version']
+__version__ = get_versions()["version"]
 del get_versions
```

### Comparing `QWeb-3.2.1/QWeb/__main__.py` & `QWeb-3.3.0/QWeb/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,39 +18,42 @@
 import sys
 from ._version import get_versions  # pylint: disable-msg=E0611
 from robot import libdoc  # type: ignore
 
 
 def cli() -> None:
     parser = argparse.ArgumentParser(
-        prog='QWeb',
-        usage='python %(prog)s [options] INPUT'
-        '\n\nEXAMPLES:\n'
-        '%(prog)s --all (lists all keywords)\n'
+        prog="QWeb",
+        usage="python %(prog)s [options] INPUT"
+        "\n\nEXAMPLES:\n"
+        "%(prog)s --all (lists all keywords)\n"
         '%(prog)s --list Get (lists all keywords startin with "Get")\n'
         '%(prog)s --show TypeText (displays documentation for keyword "TypeText")',
-        description='Note: This module is meant to be used as a robot famework library.'
-        'Command line interface only provides access to keyword documentation.')
-    parser.add_argument('-V',
-                        '--version',
-                        action='version',
-                        version='%(prog)s {version}'.format(version=__version__))
-    parser.add_argument('-A', '--all', action='store_true', help='lists ALL keywords')
-    parser.add_argument('-L', '--list', action='store', help='lists keywords based on input string')
-    parser.add_argument('-S', '--show', action='store', help='show docs for keyword(s)')
+        description="Note: This module is meant to be used as a robot famework library."
+        "Command line interface only provides access to keyword documentation.",
+    )
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version="%(prog)s {version}".format(version=__version__),
+    )
+    parser.add_argument("-A", "--all", action="store_true", help="lists ALL keywords")
+    parser.add_argument("-L", "--list", action="store", help="lists keywords based on input string")
+    parser.add_argument("-S", "--show", action="store", help="show docs for keyword(s)")
     if len(sys.argv) == 1:
         parser.print_help()
     args = parser.parse_args()
 
     # handle known options
     if args.all:
         print(libdoc.libdoc_cli(["QWeb", "list"]))
     elif args.list:
         print(libdoc.libdoc_cli(["QWeb", "list", args.list]))
     elif args.show:
         print(libdoc.libdoc_cli(["QWeb", "show", args.show]))
 
 
 if __name__ == "__main__":
-    __version__ = get_versions()['version']
+    __version__ = get_versions()["version"]
     del get_versions
     cli()
```

### Comparing `QWeb-3.2.1/QWeb/_version.py` & `QWeb-3.3.0/QWeb/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-08T09:18:30+0300",
+ "date": "2024-05-15T09:38:03+0300",
  "dirty": false,
  "error": null,
- "full-revisionid": "8340ddbaf3eff96259c8c3b07467fdba9a27e331",
- "version": "v3.2.1"
+ "full-revisionid": "0fd1c7dfe8396e97924772cc016ddaf47cc36bdb",
+ "version": "v3.3.0"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `QWeb-3.2.1/QWeb/custom_config.py` & `QWeb-3.3.0/QWeb/custom_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     function : function
         Function that does not need to return anything.
     """
     previous = frame.wait_page_loaded
     if callable(function):
         frame.wait_page_loaded = function
     else:
-        raise ValueError('Argument needs to be callable: {}'.format(function))
+        raise ValueError("Argument needs to be callable: {}".format(function))
     return previous
 
 
 def set_active_area_function(function: Callable[..., Any]):
     """Set function that sets active area where elements are searched.
 
     Parameters
```

### Comparing `QWeb-3.2.1/QWeb/internal/actions.py` & `QWeb-3.3.0/QWeb/internal/actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,162 +20,175 @@
 Coding rules:
     1.) When implementing new features connect those to
         timeout_decorator_for_actions decorator for consistency.
     2.) Always use QWeb exceptions instead of Selenium or Python ones.
     3.) All exception and retry related logic should be handle
         in decorators for consistency and usability reasons.
 """
+
 from __future__ import annotations
 from typing import Optional, Union, Any
 
 import time
 import fnmatch
 from robot.api import logger
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.common.action_chains import ActionChains
-from selenium.common.exceptions import WebDriverException, NoSuchElementException, \
-    MoveTargetOutOfBoundsException, ElementNotInteractableException
-from QWeb.internal.exceptions import QWebValueMismatchError, QWebValueError, \
-    QWebUnexpectedConditionError, QWebInvalidElementStateError, QWebTimeoutError, \
-    QWebTextNotFoundError
+from selenium.common.exceptions import (
+    WebDriverException,
+    NoSuchElementException,
+    MoveTargetOutOfBoundsException,
+    ElementNotInteractableException,
+)
+from QWeb.internal.exceptions import (
+    QWebValueMismatchError,
+    QWebValueError,
+    QWebUnexpectedConditionError,
+    QWebInvalidElementStateError,
+    QWebTimeoutError,
+    QWebTextNotFoundError,
+)
 from QWeb.internal import text as internal_text, util
 from QWeb.internal import javascript, decorators, checkbox, browser
 from QWeb.internal.input_handler import INPUT_HANDLER as input_handler
 from QWeb.internal.config_defaults import CONFIG
 
 
 @decorators.timeout_decorator_for_actions
 def write(
-        input_element: WebElement,
-        input_text: str,
-        timeout: int,  # pylint: disable=unused-argument
-        **kwargs: Any) -> None:
-    click = util.par2bool(kwargs.get('click', CONFIG['ClickToFocus']))
+    input_element: WebElement,
+    input_text: str,
+    timeout: int,  # pylint: disable=unused-argument
+    **kwargs: Any,
+) -> None:
+    click = util.par2bool(kwargs.get("click", CONFIG["ClickToFocus"]))
     if click:
         wd_click(input_element)
     if _ends_with_line_break(input_text):
         # input_text might be set to None from _remove_ending_line_break(input_text)
         input_text, key = _remove_ending_line_break(  # type: ignore[assignment]
-            input_text)
-        kwargs['key'] = key
-    check = util.par2bool(kwargs.get('check', CONFIG['CheckInputValue']))
-    kwargs['shadow_dom'] = CONFIG['ShadowDOM']
+            input_text
+        )
+        kwargs["key"] = key
+    check = util.par2bool(kwargs.get("check", CONFIG["CheckInputValue"]))
+    kwargs["shadow_dom"] = CONFIG["ShadowDOM"]
     if check is True:
-        kwargs['check'] = True
+        kwargs["check"] = True
         input_handler.write(input_element, input_text, **kwargs)
         time.sleep(1)
-        compare_input_values(input_element, kwargs.get('expected', input_text), timeout=2, **kwargs)
+        compare_input_values(input_element, kwargs.get("expected", input_text), timeout=2, **kwargs)
         try:
-            input_element.send_keys(kwargs.get('key', input_handler.line_break_key))
+            input_element.send_keys(kwargs.get("key", input_handler.line_break_key))
         except ElementNotInteractableException:
             # this can happen with firefox for shadow dom elements
             # log, but do not fail the test case as value was written correctly
             logger.debug("Could not send line break key to input")
     else:
         input_handler.write(input_element, input_text, **kwargs)
     logger.debug(f'Preferred text: "{input_text}"')
 
 
 @decorators.timeout_decorator_for_actions
 def compare_input_values(
-        input_element: WebElement,
-        expected_value: str,
-        timeout: int,  # pylint: disable=unused-argument
-        **kwargs: Any) -> bool:
+    input_element: WebElement,
+    expected_value: str,
+    timeout: int,  # pylint: disable=unused-argument
+    **kwargs: Any,
+) -> bool:
     try:
         real_value = input_value(input_element, timeout="0.5s", **kwargs)
         if expected_value == real_value:  # Full match
             return True
         real_value = util.get_substring(real_value, **kwargs)
         expected_value = str(util.get_substring(expected_value, **kwargs))
     except QWebValueError:
         real_value = ""
-    logger.debug(f'Real value: {real_value}, expected value {expected_value}')
+    logger.debug(f"Real value: {real_value}, expected value {expected_value}")
     if fnmatch.fnmatch(str(real_value).strip(), expected_value):
         return True
     raise QWebValueMismatchError(
         f"""Expected value "{expected_value}" didn\'t match to real value "{real_value}\""""
     )
 
 
 @decorators.timeout_decorator_for_actions
 def input_value(input_element: WebElement, timeout: int, **kwargs: Any) -> str:
-    blind = util.par2bool(kwargs.get('blind', CONFIG['BlindReturn']))
-    shadow_dom = CONFIG['ShadowDOM']
+    blind = util.par2bool(kwargs.get("blind", CONFIG["BlindReturn"]))
+    shadow_dom = CONFIG["ShadowDOM"]
 
     if input_handler.is_editable_text_element(input_element) and not shadow_dom:
-        value = input_element.get_attribute('innerText')
+        value = input_element.get_attribute("innerText")
     else:
-        value = input_element.get_attribute('value')
+        value = input_element.get_attribute("value")
     if value:
         return value.strip()
     if blind:
-        return ''
-    raise QWebValueError(f'No Value found after {timeout} sec')
+        return ""
+    raise QWebValueError(f"No Value found after {timeout} sec")
 
 
 @decorators.timeout_decorator_for_actions
 def scroll(web_element: WebElement, timeout: int) -> None:  # pylint: disable=unused-argument
-    javascript.execute_javascript('arguments[0].scrollIntoView();', web_element)
+    javascript.execute_javascript("arguments[0].scrollIntoView();", web_element)
 
 
 @decorators.timeout_decorator_for_actions
-def execute_click_and_verify_condition(web_element: WebElement,
-                                       text_appear: bool = True,
-                                       **kwargs: Any) -> bool:
+def execute_click_and_verify_condition(
+    web_element: WebElement, text_appear: bool = True, **kwargs: Any
+) -> bool:
     """Click and optionally verify condition after click.
 
     Accepted kwargs:
         text(str) = In case we want to verify that some text appears/disappears after click
         interval = How long we wait between the clicks
         timeout = How long we are trying if element is not enabled or some other error exists
         js = if js parameter exists, try javascript click instead of selenium
     """
-    js = True if util.is_safari() else util.par2bool(kwargs.get('js', False))
-    dbl_click = util.par2bool(kwargs.get('doubleclick', CONFIG["DoubleClick"]))
+    js = True if util.is_safari() else util.par2bool(kwargs.get("js", False))
+    dbl_click = util.par2bool(kwargs.get("doubleclick", CONFIG["DoubleClick"]))
     if web_element.is_enabled():
         try:
             if dbl_click:
                 if js:
                     js_double_click(web_element)
                 else:
                     double_click(web_element)
             elif js:
                 js_click(web_element)
             else:
                 wd_click(web_element, **kwargs)
-                logger.debug('element clicked')
+                logger.debug("element clicked")
         except WebDriverException as e:
-            logger.info(f'Got {e} when tried to click.')
-            if 'text' not in kwargs:
+            logger.info(f"Got {e} when tried to click.")
+            if "text" not in kwargs:
                 raise e
-        if 'text' in kwargs:
-            logger.debug('button clicked. Verifying expected condition..')
+        if "text" in kwargs:
+            logger.debug("button clicked. Verifying expected condition..")
             try:
-                if text_appearance(kwargs['text'],
-                                   text_appear=text_appear,
-                                   timeout=kwargs.get('interval')):
+                if text_appearance(
+                    kwargs["text"], text_appear=text_appear, timeout=kwargs.get("interval")
+                ):
                     return True
             except QWebTimeoutError as e:
-                logger.debug('timeout err')
-                raise QWebUnexpectedConditionError('Unexpected condition') from e
+                logger.debug("timeout err")
+                raise QWebUnexpectedConditionError("Unexpected condition") from e
         return True
-    raise QWebInvalidElementStateError('Element is not enabled')
+    raise QWebInvalidElementStateError("Element is not enabled")
 
 
 def right_click(element: WebElement) -> None:
     driver = browser.get_current_browser()
     ac = ActionChains(driver)
     ac.context_click(element).perform()
 
 
 def js_click(web_element: WebElement) -> None:
-    javascript.execute_javascript('arguments[0].click()', web_element)
+    javascript.execute_javascript("arguments[0].click()", web_element)
     logger.debug("Js click performed")
 
 
 def js_double_click(web_element: WebElement) -> None:
     js = """var target = arguments[0];
             var clickEvent = document.createEvent('MouseEvents');
             clickEvent.initEvent ('dblclick', true, true);
@@ -185,80 +198,80 @@
 
 
 def double_click(web_element: WebElement) -> None:
     driver = browser.get_current_browser()
     ac = ActionChains(driver)
     ac.double_click(web_element)
     ac.perform()
-    logger.debug('element double-clicked')
+    logger.debug("element double-clicked")
 
 
 def wd_click(web_element: WebElement, **kwargs: Any) -> None:
     try:
         web_element.click()
     except WebDriverException as e:
         logger.debug(str(e))
-        js_click_on_failure = util.par2bool(kwargs.get('js_click', True))
+        js_click_on_failure = util.par2bool(kwargs.get("js_click", True))
         if js_click_on_failure:
             js_click(web_element)
 
 
 @decorators.timeout_decorator_for_actions
 def checkbox_set(  # pylint: disable=unused-argument
-        checkbox_element: WebElement,
-        locator_element: WebElement,
-        value: bool,
-        **kwargs: Any) -> None:
+    checkbox_element: WebElement, locator_element: WebElement, value: bool, **kwargs: Any
+) -> None:
     if checkbox.is_checked(checkbox_element) != value:
         try:
             checkbox_element.click()
         except WebDriverException:
             if locator_element:
                 locator_element.click()
             else:
                 parent_elem = checkbox_element.find_element(By.XPATH, "..")
                 if parent_elem.tag_name.lower() == "label":
                     parent_elem.click()
                 if checkbox_element.is_selected() != value:
                     javascript.execute_javascript(
                         "arguments[0].checked={}".format("true" if value else "false"),
-                        checkbox_element)
+                        checkbox_element,
+                    )
 
 
 # pylint: disable=too-many-branches
 @decorators.timeout_decorator_for_actions
 def select_option(
-        select: Select,  # pylint: disable=unused-argument
-        option: str,
-        unselect: bool = False,
-        **kwargs: Any) -> bool:
+    select: Select,  # pylint: disable=unused-argument
+    option: str,
+    unselect: bool = False,
+    **kwargs: Any,
+) -> bool:
     """Click and optionally verify condition after click.
 
     Parameters
     ----------
     select : object
         Instance of Select class
     option : str
         Text to select
     unselect : bool
         Select (False, default) or unselect (True) given option
     """
     option_list = []
     value_list = []
-    if option.startswith('[[') and option.endswith(']]'):
-        option = option.strip('[]')
+    if option.startswith("[[") and option.endswith("]]"):
+        option = option.strip("[]")
         if option.isdigit():
             try:
                 if unselect:
                     select.deselect_by_index(option)  # type: ignore
                 else:
                     select.select_by_index(option)  # type: ignore
                 return True
             except TypeError as te:
-                raise QWebValueMismatchError('Index out of range') from te
+                raise QWebValueMismatchError("Index out of range") from te
     try:
         if unselect:
             select.deselect_by_visible_text(option)
         else:
             select.select_by_visible_text(option)
         return True
     except NoSuchElementException:
@@ -268,41 +281,42 @@
             else:
                 select.select_by_value(option)
             return True
         except NoSuchElementException:
             if select:
                 for opt in select.options:
                     option_list.append(opt.text)
-                    value_list.append(opt.get_attribute('value'))
+                    value_list.append(opt.get_attribute("value"))
         if option_list != value_list:
             raise QWebValueMismatchError(  # pylint: disable=W0707
                 f'Option "{option}" is not in the options list.\n'
-                f'The list contained these options: {option_list}.\n'
-                f'The list contained these values: {value_list}.')
+                f"The list contained these options: {option_list}.\n"
+                f"The list contained these values: {value_list}."
+            )
         raise QWebValueMismatchError(  # pylint: disable=W0707
             f'Option "{option}" is not in the options list.\n'
-            f'The list contained these options: {option_list}.\n')
+            f"The list contained these options: {option_list}.\n"
+        )
 
 
 @decorators.timeout_decorator_for_actions
 def is_not_in_dropdown(select: Select, option: str, **kwargs: Any) -> bool:
-    """"Verifies that the selected option is not in the dropdown list"""
+    """ "Verifies that the selected option is not in the dropdown list"""
     option_list = get_select_options(select, **kwargs)
     if option in option_list:
-        raise QWebValueError(
-            f"Found the value {option} from the dropdown menu: {option_list}."
-        )
+        raise QWebValueError(f"Found the value {option} from the dropdown menu: {option_list}.")
     return True
 
 
 @decorators.timeout_decorator_for_actions
 def get_selected_value(
-        select: Select,  # pylint: disable=unused-argument
-        expected: Optional[str] = None,
-        **kwargs: Any) -> Union[bool, str]:
+    select: Select,  # pylint: disable=unused-argument
+    expected: Optional[str] = None,
+    **kwargs: Any,
+) -> Union[bool, str]:
     """Get or verify selected value.
 
     Parameters
     ----------
     select : object
         Instance of Select class
     expected : str
@@ -320,39 +334,42 @@
             f"""Expected value "{expected}" didn\'t match to real value "{txt_selected}"."""
         )
     return txt_selected
 
 
 @decorators.timeout_decorator_for_actions
 def get_select_options(
-        select: Select,  # pylint: disable=unused-argument
-        expected: Optional[str] = None,
-        **kwargs: Any) -> Union[bool, list[str]]:
+    select: Select,  # pylint: disable=unused-argument
+    expected: Optional[str] = None,
+    **kwargs: Any,
+) -> Union[bool, list[str]]:
     options = select.options
     if expected:
         for option in options:
             logger.debug(option.text)
             if fnmatch.fnmatch(expected, option.text):
                 return True
         raise QWebValueMismatchError(
-            f'Expected value "{expected}" not found from selectable options')
+            f'Expected value "{expected}" not found from selectable options'
+        )
     # parse all options to a list and return it
     option_list = []
     for option in options:
         option_list.append(option.text)
     return option_list
 
 
 @decorators.timeout_decorator_for_actions
 def hover_to(web_element: WebElement, timeout: int = 0) -> None:  # pylint: disable=unused-argument
     driver = browser.get_current_browser()
     # firefox & safari specific fix
     needs_js_scroll = [
-        x for x in [browser.firefox.NAMES, browser.safari.NAMES]
-        if driver.capabilities['browserName'].lower() in x
+        x
+        for x in [browser.firefox.NAMES, browser.safari.NAMES]
+        if driver.capabilities["browserName"].lower() in x
     ]
     if needs_js_scroll:
         # use javascript to scroll
         logger.debug("Needs javascript to scoll")
         driver.execute_script("arguments[0].scrollIntoView(true);", web_element)
     try:
         hover = ActionChains(driver).move_to_element(web_element)
@@ -360,90 +377,96 @@
     except MoveTargetOutOfBoundsException:
         # chrome > 90, use javascript
         driver.execute_script("arguments[0].scrollIntoView(true);", web_element)
 
 
 @decorators.timeout_decorator_for_actions
 def text_appearance(text: str, **kwargs: Any) -> bool:
-    """ Sub for retry click.
+    """Sub for retry click.
 
     Works as keywords is_text and is_no_text. Returns True if
     text exists/not exists in given time. Raises QWebValueMismatchErr
     for decorator to handle if condition is not expected (False).
     """
     try:
         element = internal_text.get_element_by_locator_text(text, allow_non_existent=True, **kwargs)
     except QWebTimeoutError as te:
-        if kwargs['text_appear'] is False:
+        if kwargs["text_appear"] is False:
             return True
-        raise QWebValueMismatchError('return value should be true') from te
+        raise QWebValueMismatchError("return value should be true") from te
     try:
-        if element and kwargs['text_appear'] is True:
+        if element and kwargs["text_appear"] is True:
             return True
-        if not element and kwargs['text_appear'] is False:
+        if not element and kwargs["text_appear"] is False:
             return True
     except QWebUnexpectedConditionError:
-        logger.debug('StaleElement Err from text appearance')
-    raise QWebValueMismatchError('return value should be true')
+        logger.debug("StaleElement Err from text appearance")
+    raise QWebValueMismatchError("return value should be true")
 
 
+# pylint: disable=unused-argument
 @decorators.timeout_decorator_for_actions
-def get_element_text(web_element: WebElement, expected=None, timeout: int = 0) -> Union[bool, str]:  # pylint: disable=unused-argument
+def get_element_text(
+    web_element: WebElement, expected=None, timeout: int = 0, partial_match: bool = False
+) -> Union[bool, str]:
     # if both text and innerText are missing, innerText would return None instead of ""
     # This needs to be handled here.
-    real_text = (
-        (web_element.text or "").strip()
-        or (web_element.get_attribute('innerText') or "").strip()
-    )
+    real_text = (web_element.text or "").strip() or (
+        web_element.get_attribute("innerText") or ""
+    ).strip()
 
     if expected is not None:
         try:
-            return _compare_texts(real_text, expected.strip(), timeout)
+            return _compare_texts(real_text, expected.strip(), partial_match)
         except QWebValueMismatchError as e:
-            raise QWebValueError(f'Expected {expected}, found {real_text}') from e
+            raise QWebValueError(f"Expected {expected}, found {real_text}") from e
     if real_text is not None:
         return real_text
-    raise QWebValueMismatchError('Text not found')
+    raise QWebValueMismatchError("Text not found")
 
 
-def _compare_texts(text_to_compare: str, expected: str, timeout: int) -> bool:  # pylint: disable=unused-argument
-    if fnmatch.fnmatch(text_to_compare, expected) is False:
-        raise QWebValueMismatchError(f'Expected {expected}, found {text_to_compare}')
-    return True
+def _compare_texts(text_to_compare: str, expected: str, partial_match: bool = True) -> bool:
+    if text_to_compare == expected or (partial_match and expected in text_to_compare):
+        return True
+    raise QWebValueMismatchError(f"Expected {expected}, found {text_to_compare}")
 
 
 def _ends_with_line_break(input_text: str) -> bool:
-    line_break = ('\n', '\ue007', '\t', '\ue004')
+    line_break = ("\n", "\ue007", "\t", "\ue004")
     return input_text.endswith(line_break)
 
 
 def _remove_ending_line_break(input_text: str) -> tuple[Optional[str], Optional[str]]:
-    enter_key = ('\n', '\ue007')
-    tab_key = ('\t', '\ue004')
+    enter_key = ("\n", "\ue007")
+    tab_key = ("\t", "\ue004")
     if input_text.endswith(enter_key):
-        input_list = input_text.replace('\n', '\ue007').rsplit('\ue007', 1)
-        return input_list[0], '\ue007'
+        input_list = input_text.replace("\n", "\ue007").rsplit("\ue007", 1)
+        return input_list[0], "\ue007"
     if input_text.endswith(tab_key):
-        input_list = input_text.replace('\t', '\ue004').rsplit('\ue004', 1)
-        return input_list[0], '\ue004'
+        input_list = input_text.replace("\t", "\ue004").rsplit("\ue004", 1)
+        return input_list[0], "\ue004"
     return None, None
 
 
 def _contains_enter(input_text: str) -> bool:
-    return bool('\n' in input_text or '\ue007' in input_text)
+    return bool("\n" in input_text or "\ue007" in input_text)
 
 
 def _contains_tab(input_text: str) -> bool:
-    return bool('\t' in input_text or '\ue004' in input_text)
+    return bool("\t" in input_text or "\ue004" in input_text)
 
 
-def scroll_first_scrollable_parent_element(locator: str, anchor: str, text_to_find: str,
-                                           scroll_length: Optional[Union[int, str]],
-                                           slow_mode: bool, timeout: Union[int, float,
-                                                                           str]) -> None:
+def scroll_first_scrollable_parent_element(
+    locator: str,
+    anchor: str,
+    text_to_find: str,
+    scroll_length: Optional[Union[int, str]],
+    slow_mode: bool,
+    timeout: Union[int, float, str],
+) -> None:
     visible = None
     js_get_parent_element = """
         function getScrollParent(node) {
           if (node == null) {
             return null;
           }
 
@@ -462,72 +485,80 @@
     current_pos = javascript.execute_javascript(js_element_position, scrollable_element)
     old_pos = None
     start = time.time()
     if not slow_mode:
         while not visible and old_pos != current_pos and time.time() < float(timeout) + start:
             old_pos = javascript.execute_javascript(js_element_position, scrollable_element)
             javascript.execute_javascript(js_element_scroll, scrollable_element)
-            time.sleep(.5)
+            time.sleep(0.5)
             current_pos = javascript.execute_javascript(js_element_position, scrollable_element)
-            visible = internal_text.get_element_by_locator_text(text_to_find,
-                                                                allow_non_existent=True)
+            visible = internal_text.get_element_by_locator_text(
+                text_to_find, allow_non_existent=True
+            )
             logger.info(
-                f'Old pos: {old_pos}\nNew pos: {current_pos}\nVisible: {visible}',
+                f"Old pos: {old_pos}\nNew pos: {current_pos}\nVisible: {visible}",
                 also_console=True,
             )
     else:
         logger.info(
             f'\nSlow mode is on, execution will only stop if the text "{text_to_find}" '
-            ' is found or if the timeout is reached.',
+            " is found or if the timeout is reached.",
             also_console=True,
         )
         while not visible and time.time() < float(timeout) + start:
             javascript.execute_javascript(js_element_scroll, scrollable_element)
-            time.sleep(.5)
-            visible = internal_text.get_element_by_locator_text(text_to_find,
-                                                                allow_non_existent=True)
-            logger.info(f'\nVisible: {visible}', also_console=True)
+            time.sleep(0.5)
+            visible = internal_text.get_element_by_locator_text(
+                text_to_find, allow_non_existent=True
+            )
+            logger.info(f"\nVisible: {visible}", also_console=True)
     if visible:
         return
-    raise QWebTextNotFoundError(f'Text {text_to_find} not found.')
+    raise QWebTextNotFoundError(f"Text {text_to_find} not found.")
 
 
-def scroll_dynamic_web_page(text_to_find: str, scroll_length: Optional[Union[int, str]],
-                            slow_mode: bool, timeout: Union[int, float, str]) -> bool:
+def scroll_dynamic_web_page(
+    text_to_find: str,
+    scroll_length: Optional[Union[int, str]],
+    slow_mode: bool,
+    timeout: Union[int, float, str],
+) -> bool:
     visible = None
     js_browser_height = "return window.innerHeight"
     height = javascript.execute_javascript(js_browser_height)  # Length of one scroll
     js_current_pos = "return window.pageYOffset;"
-    js_scroll = f'window.scrollBy(0,{scroll_length or height})'
+    js_scroll = f"window.scrollBy(0,{scroll_length or height})"
     current_pos = javascript.execute_javascript(js_current_pos)
     old_pos = None
     start = time.time()
     if not slow_mode:
         while not visible and old_pos != current_pos and time.time() < float(timeout) + start:
             old_pos = javascript.execute_javascript(js_current_pos)
             javascript.execute_javascript(js_scroll)
-            time.sleep(.5)
+            time.sleep(0.5)
             current_pos = javascript.execute_javascript(js_current_pos)
-            visible = internal_text.get_element_by_locator_text(text_to_find,
-                                                                allow_non_existent=True)
+            visible = internal_text.get_element_by_locator_text(
+                text_to_find, allow_non_existent=True
+            )
             logger.info(
-                f'\nOld pos: {old_pos}\nCurrent pos: {current_pos}\nVisible: {visible}',
+                f"\nOld pos: {old_pos}\nCurrent pos: {current_pos}\nVisible: {visible}",
                 also_console=True,
             )
     else:
         logger.info(
-            '\nSlow mode is on, execution will only stop if '
+            "\nSlow mode is on, execution will only stop if "
             f'the text "{text_to_find}" is found or if the timeout is reached.',
             also_console=True,
         )
         while not visible and time.time() < float(timeout) + start:
             javascript.execute_javascript(js_scroll)
-            time.sleep(.5)
-            visible = internal_text.get_element_by_locator_text(text_to_find,
-                                                                allow_non_existent=True)
-            logger.info(f'\nVisible: {visible}', also_console=True)
+            time.sleep(0.5)
+            visible = internal_text.get_element_by_locator_text(
+                text_to_find, allow_non_existent=True
+            )
+            logger.info(f"\nVisible: {visible}", also_console=True)
 
     if visible:
         return True
     raise QWebTextNotFoundError(
         f'Could not find text "{text_to_find}" after scrolling for {current_pos} pixels.'
     )
```

### Comparing `QWeb-3.2.1/QWeb/internal/ajax.py` & `QWeb-3.3.0/QWeb/internal/ajax.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,76 +24,76 @@
 from pathlib import Path
 from QWeb.internal.exceptions import QWebValueError, QWebElementNotFoundError
 from QWeb.internal import download, text, browser, element
 from QWeb.internal import javascript as js
 from robot.api import logger
 
 
-def http_request_with_browser_cookies(url: str,
-                                      headers: Optional[dict[str, Any]] = None) -> Response:
-    """ Copy cookies from current browser session
-        and use them with request session
+def http_request_with_browser_cookies(
+    url: str, headers: Optional[dict[str, Any]] = None
+) -> Response:
+    """Copy cookies from current browser session
+    and use them with request session
     """
     driver = browser.get_current_browser()
     if not headers:
-        headers = {'User-Agent': '{}'.format(js.execute_javascript('return navigator.userAgent'))}
+        headers = {"User-Agent": "{}".format(js.execute_javascript("return navigator.userAgent"))}
     cookies = driver.get_cookies()
     s = requests.Session()
     for cookie in cookies:
-        s.cookies.set(cookie['name'], cookie['value'])
+        s.cookies.set(cookie["name"], cookie["value"])
     return s.get(url, headers=headers)
 
 
 def get_url_for_http_request(locator: str, anchor: str, **kwargs: Any) -> str:
-    """ Get href-attribute (=url) from found web element.
-    """
+    """Get href-attribute (=url) from found web element."""
     script = """
        var href = function(el) {
                if (el.hasAttribute("href")) {
                    return el.href;
                    console.log(el.attributes["href"].value);
                }
                return arguments[0].closest("a").href;
            }
            return href(arguments[0]);
        """
-    index = int(kwargs.get('index', 1) - 1)
+    index = int(kwargs.get("index", 1) - 1)
     try:
         elem = text.get_item_using_anchor(locator, anchor, **kwargs)
     except QWebElementNotFoundError:
         elem = None
     if not elem:
         elem = text.get_text_using_anchor(locator, anchor, **kwargs)
-    if kwargs.get('parent', None):
-        elem = element.get_parent_element(elem, str(kwargs.get('parent')))
-    if kwargs.get('child', None):
-        elem = element.get_element_from_childnodes(elem,
-                                                   str(kwargs.get('child')),
-                                                   dom_traversing=False)[index]
+    if kwargs.get("parent", None):
+        elem = element.get_parent_element(elem, str(kwargs.get("parent")))
+    if kwargs.get("child", None):
+        elem = element.get_element_from_childnodes(
+            elem, str(kwargs.get("child")), dom_traversing=False
+        )[index]
     url = js.execute_javascript(script, elem)
     if url:
         return url
-    raise QWebValueError('Unable to find valid url for locator {}'.format(locator))
+    raise QWebValueError("Unable to find valid url for locator {}".format(locator))
 
 
-def save_response_as_file(response: Response,
-                          filename: str,
-                          root_path: Optional[str] = None) -> None:
+def save_response_as_file(
+    response: Response, filename: str, root_path: Optional[str] = None
+) -> None:
     if root_path is None:
         path = download.get_downloads_dir()
     else:
         path = root_path
 
-    logger.debug('path before {}'.format(path))
-    if '/' in filename:
-        folders = filename.split('/')
+    logger.debug("path before {}".format(path))
+    if "/" in filename:
+        folders = filename.split("/")
         for i in range(len(folders) - 1):
             logger.debug(folders[i])
             if not Path(os.path.join(path, folders[i])).exists():
                 os.makedirs(os.path.join(path, folders[i]))
             path = os.path.join(path, folders[i])
         real_path = Path(path) / folders[len(folders) - 1]
     else:
         real_path = Path(path) / filename
-    logger.info('path is {}'.format(path))
-    with open(real_path, 'wb') as file:
+    logger.info("path is {}".format(path))
+    with open(real_path, "wb") as file:
         file.write(response.content)
```

### Comparing `QWeb-3.2.1/QWeb/internal/alert.py` & `QWeb-3.3.0/QWeb/internal/alert.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 
 from QWeb.internal.exceptions import QWebDriverError
 from QWeb.internal import browser, decorators
 
 
 @decorators.timeout_decorator_for_actions
 def close_alert(alert: Alert, action: str) -> None:
-    if action.upper() == 'ACCEPT':
+    if action.upper() == "ACCEPT":
         alert.accept()
-    elif action.upper() == 'DISMISS':
+    elif action.upper() == "DISMISS":
         alert.dismiss()
-    elif action.upper() == 'NOTHING':
+    elif action.upper() == "NOTHING":
         return
     else:
         raise QWebDriverError(
-            "Invalid alert action '{}'. Must be ACCEPT, DISMISS or LEAVE".format(action))
+            "Invalid alert action '{}'. Must be ACCEPT, DISMISS or LEAVE".format(action)
+        )
 
 
 @decorators.timeout_decorator_for_actions
 def wait_alert(timeout: Union[int, float, str]) -> Alert:  # pylint: disable=unused-argument
     driver = browser.get_current_browser()
     return driver.switch_to.alert
```

### Comparing `QWeb-3.2.1/QWeb/internal/blocks.py` & `QWeb-3.3.0/QWeb/internal/blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,41 +29,41 @@
         else:
             new_args.append(a)
     for key, val in kwargs.items():
         if _contains_var(key):
             key = BuiltIn().get_variable_value(key)
         if _contains_var(val):
             val = BuiltIn().get_variable_value(val)
-        new_args.append('{}={}'.format(key, val))
+        new_args.append("{}={}".format(key, val))
     return new_args
 
 
 def get_steps(name: str, caller_fn: str, **kwargs: Any) -> Optional[list[dict[str, Any]]]:
-    file = Path(BuiltIn().get_variable_value('${SUITE SOURCE}'))
-    test_case = BuiltIn().get_variable_value('${TEST_NAME}')
+    file = Path(BuiltIn().get_variable_value("${SUITE SOURCE}"))
+    test_case = BuiltIn().get_variable_value("${TEST_NAME}")
     with open(file, "r+") as fo:
         data = fo.readlines()
     idx = 0
     while data:
         if data[idx].strip() == test_case:
-            data = data[idx:len(data)]
+            data = data[idx : len(data)]  # noqa: E203
             for i, line in enumerate(data):
-                if caller_fn in line.replace(' ', '').strip().lower() and name in line.strip():
+                if caller_fn in line.replace(" ", "").strip().lower() and name in line.strip():
                     steps = _parse_steps(data, i + 1, **kwargs)
                     return steps
         idx += 1
     return None
 
 
 def _parse_steps(data: list[str], iterator: int, **kwargs: Any) -> list[dict[str, Any]]:
     steps = []
-    while not data[iterator].replace(' ', '').lower().strip().startswith('endblock'):
+    while not data[iterator].replace(" ", "").lower().strip().startswith("endblock"):
         varname = None
-        line = re.split(r'\s{2,}', data[iterator].strip())
-        if line[0].startswith('#'):
+        line = re.split(r"\s{2,}", data[iterator].strip())
+        if line[0].startswith("#"):
             iterator += 1
             continue
         if _contains_var(line[0]):
             pw = line[1].strip()
             varname = line[0].strip()
             args, kwargs = _parse_arguments(line, starting_point=2, **kwargs)
         else:
@@ -71,27 +71,28 @@
             args, kwargs = _parse_arguments(line, starting_point=1, **kwargs)
         step = {"variable": varname, "paceword": pw, "args": args, "kwargs": kwargs}
         steps.append(step)
         iterator += 1
     return steps
 
 
-def _parse_arguments(line: list[str], starting_point: int,
-                     **kwargs: Any) -> tuple[list[str], dict[Any, Any]]:
+def _parse_arguments(
+    line: list[str], starting_point: int, **kwargs: Any
+) -> tuple[list[str], dict[Any, Any]]:
     args = []
     for a in range(starting_point, len(line)):
-        if line[a].strip() != '':
-            if '=' not in line[a]:
+        if line[a].strip() != "":
+            if "=" not in line[a]:
                 args.append(line[a].strip())
-            elif '\\=' in line[a]:
+            elif "\\=" in line[a]:
                 args.append(line[a].strip())
             else:
-                key, value = line[a].strip().split('=', 1)
+                key, value = line[a].strip().split("=", 1)
                 kwargs.update({key: value})
     return args, kwargs
 
 
 def _contains_var(arg: str, from_start: bool = True) -> bool:
-    var_types = ['${', '@{', '&{']
+    var_types = ["${", "@{", "&{"]
     if from_start:
         return any(arg.strip().startswith(v) for v in var_types)
-    return any(v in arg and '}' in arg for v in var_types)
+    return any(v in arg and "}" in arg for v in var_types)
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/__init__.py` & `QWeb-3.3.0/QWeb/internal/browser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,103 +15,105 @@
 # limitations under the License.
 # ---------------------------
 from __future__ import annotations
 from typing import Union, Optional
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from QWeb.internal.exceptions import QWebDriverError, QWebValueError
+
 # These mime types were retrieved from
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Complete_list_of_MIME_types
-MIME_TYPES = ("application/epub+zip;"
-              "application/java-archive;"
-              "application/javascript;"
-              "application/json;"
-              "application/msword;"
-              "application/octet-stream;"
-              "application/octet-stream;"
-              "application/ogg;"
-              "application/pdf;"
-              "application/rtf;"
-              "application/typescript;"
-              "application/vnd.amazon.ebook;"
-              "application/vnd.apple.installer+xml;"
-              "application/vnd.mozilla.xul+xml;"
-              "application/vnd.ms-excel;"
-              "application/vnd.ms-fontobject;"
-              "application/vnd.ms-powerpoint;"
-              "application/vnd.oasis.opendocument.text;"
-              "application/vnd.oasis.opendocument;"
-              "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet;"
-              "application/vnd.visio;"
-              "application/x-7z-compressed"
-              "application/x-abiword;"
-              "application/x-bzip2;"
-              "application/x-bzip;"
-              "application/x-csh;"
-              "application/x-rar-compressed;"
-              "application/x-sh;"
-              "application/x-shockwave-flash;"
-              "application/x-tar;"
-              "application/xhtml+xml;"
-              "application/xml;"
-              "application/zip;"
-              "audio/aac;"
-              "audio/midi;"
-              "audio/ogg;"
-              "audio/webm;"
-              "audio/x-wav;"
-              "font/otf;"
-              "font/ttf;"
-              "font/woff2;"
-              "font/woff;"
-              "image/gif;"
-              "image/jpeg;"
-              "image/png;"
-              "image/svg+xml;"
-              "image/tiff;"
-              "image/webp;"
-              "image/x-icon;"
-              "text/calendar;"
-              "text/css;"
-              "text/csv;"
-              "text/html;"
-              "text/plain;"
-              "video/3gpp2audio/3gpp2;"
-              "video/3gppaudio/3gpp;"
-              "video/mpeg;"
-              "video/ogg;"
-              "video/webm;"
-              "video/x-msvideo")
+MIME_TYPES = (
+    "application/epub+zip;"
+    "application/java-archive;"
+    "application/javascript;"
+    "application/json;"
+    "application/msword;"
+    "application/octet-stream;"
+    "application/octet-stream;"
+    "application/ogg;"
+    "application/pdf;"
+    "application/rtf;"
+    "application/typescript;"
+    "application/vnd.amazon.ebook;"
+    "application/vnd.apple.installer+xml;"
+    "application/vnd.mozilla.xul+xml;"
+    "application/vnd.ms-excel;"
+    "application/vnd.ms-fontobject;"
+    "application/vnd.ms-powerpoint;"
+    "application/vnd.oasis.opendocument.text;"
+    "application/vnd.oasis.opendocument;"
+    "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet;"
+    "application/vnd.visio;"
+    "application/x-7z-compressed"
+    "application/x-abiword;"
+    "application/x-bzip2;"
+    "application/x-bzip;"
+    "application/x-csh;"
+    "application/x-rar-compressed;"
+    "application/x-sh;"
+    "application/x-shockwave-flash;"
+    "application/x-tar;"
+    "application/xhtml+xml;"
+    "application/xml;"
+    "application/zip;"
+    "audio/aac;"
+    "audio/midi;"
+    "audio/ogg;"
+    "audio/webm;"
+    "audio/x-wav;"
+    "font/otf;"
+    "font/ttf;"
+    "font/woff2;"
+    "font/woff;"
+    "image/gif;"
+    "image/jpeg;"
+    "image/png;"
+    "image/svg+xml;"
+    "image/tiff;"
+    "image/webp;"
+    "image/x-icon;"
+    "text/calendar;"
+    "text/css;"
+    "text/csv;"
+    "text/html;"
+    "text/plain;"
+    "video/3gpp2audio/3gpp2;"
+    "video/3gppaudio/3gpp;"
+    "video/mpeg;"
+    "video/ogg;"
+    "video/webm;"
+    "video/x-msvideo"
+)
 
 _current_browser: Optional[WebDriver] = None
 _open_browsers: list[WebDriver] = []
 
 
 def get_current_browser() -> WebDriver:
     if _current_browser is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     return _current_browser
 
 
 def set_current_browser(index: Union[int, str]) -> None:
     # pylint: disable=global-statement
     global _current_browser
 
     if str(index).isdigit():
         if int(index) == 0:
-            raise QWebValueError('SwitchBrowser index starts at 1.')
+            raise QWebValueError("SwitchBrowser index starts at 1.")
 
         i = int(index) - 1
 
         if i < len(_open_browsers):
             _current_browser = _open_browsers[i]
         else:
-            raise QWebDriverError(f'Tried to select browser with index {index} but there are \
-                                  {len(_open_browsers)} browsers open')
+            raise QWebDriverError(f"Tried to select browser with index {index} but there are \
+                                  {len(_open_browsers)} browsers open")
     elif str(index) == "NEW":
         _current_browser = _open_browsers[-1]
     else:
         raise QWebValueError('Given argument "{}" is not a digit or NEW'.format(index))
 
 
 def get_open_browsers() -> list[WebDriver]:
@@ -124,26 +126,26 @@
     # pylint: disable=global-statement, global-variable-not-assigned
     global _open_browsers
     _current_browser = driver
     _open_browsers.append(driver)
 
 
 def remove_from_browser_cache(driver: WebDriver) -> None:
-    ''' Removes specific entry from browser cache.
-    Control is moved to previously opened browser'''
+    """Removes specific entry from browser cache.
+    Control is moved to previously opened browser"""
     # pylint: disable=global-statement
     global _current_browser
     # pylint: disable=global-statement, global-variable-not-assigned
     global _open_browsers
     _open_browsers.remove(driver)
     # there's at least one browser open, move to latest
     _current_browser = _open_browsers[-1] if _open_browsers else None
 
 
 def clear_browser_cache() -> None:
-    ''' Removes all entries from browser cache. Used before quitting'''
+    """Removes all entries from browser cache. Used before quitting"""
     # pylint: disable=global-statement
     global _current_browser
     # pylint: disable=global-statement
     global _open_browsers
     _current_browser = None
     _open_browsers = []
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/android.py` & `QWeb-3.3.0/QWeb/internal/browser/android.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 from QWeb.internal import browser
 
 NAMES: list[str] = ["android", "androidphone", "androidmobile"]
 
 
 def open_browser() -> WebDriver:
     try:
-        adb_output = subprocess.check_output(['adb', 'devices']).decode()
+        adb_output = subprocess.check_output(["adb", "devices"]).decode()
     except IOError as e:
-        logger.error('Adb not installed or working incorrectly\n' + str(e))
+        logger.error("Adb not installed or working incorrectly\n" + str(e))
         raise
-    ss_type = 'false'
+    ss_type = "false"
     devices = [
-        x for x in adb_output.split() if x not in ('List', 'of', 'device', 'devices', 'attached')
+        x for x in adb_output.split() if x not in ("List", "of", "device", "devices", "attached")
     ]
     if len(devices) != 1:
-        logger.error('Number of attached devices is not 1\n')
+        logger.error("Number of attached devices is not 1\n")
         raise ValueError
-    if 'emulator' in devices:  # this is here so screenshots work on emulators
-        ss_type = 'true'
-    version = subprocess.check_output(['adb', 'shell',
-                                       'getprop ro.build.version.release']).decode().strip()
+    if "emulator" in devices:  # this is here so screenshots work on emulators
+        ss_type = "true"
+    version = (
+        subprocess.check_output(["adb", "shell", "getprop ro.build.version.release"])
+        .decode()
+        .strip()
+    )
 
     options = Options()
-    options.set_capability('platformName', 'Android')
-    options.set_capability('platformVersion', version)
-    options.set_capability('deviceName', devices[0])
-    options.set_capability('browserName', 'Chrome')
-    options.set_capability('nativeWebScreenshot', ss_type)
+    options.set_capability("platformName", "Android")
+    options.set_capability("platformVersion", version)
+    options.set_capability("deviceName", devices[0])
+    options.set_capability("browserName", "Chrome")
+    options.set_capability("nativeWebScreenshot", ss_type)
 
-    driver = webdriver.Remote(command_executor='http://localhost:4723/wd/hub',
-                              options=options)
+    driver = webdriver.Remote(command_executor="http://localhost:4723/wd/hub", options=options)
     browser.cache_browser(driver)
     return driver
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/bs_desktop.py` & `QWeb-3.3.0/QWeb/internal/browser/bs_desktop.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,70 +9,71 @@
 from selenium.common.exceptions import WebDriverException
 from typing import Any, Union
 from robot.api import logger
 from QWeb.internal import browser, exceptions, util
 
 NAMES: dict[str, tuple[str, str]] = {
     # Default  versions for different browsers.
-    'chrome': ('Chrome', 'latest'),
-    'gc': ('Chrome', 'latest'),
-    'edge': ('Edge', 'latest'),
-    'firefox': ('Firefox', 'latest'),
-    'ff': ('Firefox', 'latest'),
-    'safari': ('Safari', '16.5')
+    "chrome": ("Chrome", "latest"),
+    "gc": ("Chrome", "latest"),
+    "edge": ("Edge", "latest"),
+    "firefox": ("Firefox", "latest"),
+    "ff": ("Firefox", "latest"),
+    "safari": ("Safari", "16.5"),
 }
 
 OS: dict[str, str] = {
     # Default versions for Windows and OSX.
-    'osx': 'Ventura',
-    'windows': '10'
+    "osx": "Ventura",
+    "windows": "10",
 }
 
 
 def open_browser(bs_browser: str, project_name: str, run_id: str, **kwargs: Any) -> WebDriver:
-    bs_key = util.get_rfw_variable_value('${APIKEY}') or os.environ.get('bskey')
-    bs_user = util.get_rfw_variable_value('${USERNAME}') or os.environ.get('bsuser')
-    bs_os = util.get_rfw_variable_value('${BSOS}') or 'windows'
-    browser_name = util.get_rfw_variable_value('${BROWSER}') or NAMES[bs_browser][0]
+    bs_key = util.get_rfw_variable_value("${APIKEY}") or os.environ.get("bskey")
+    bs_user = util.get_rfw_variable_value("${USERNAME}") or os.environ.get("bsuser")
+    bs_os = util.get_rfw_variable_value("${BSOS}") or "windows"
+    browser_name = util.get_rfw_variable_value("${BROWSER}") or NAMES[bs_browser][0]
 
     desired_caps: dict = {
         "buildName": project_name,
         "projectName": project_name,
         "sessionName": run_id,
-        'os': bs_os,
-        'osVersion': util.get_rfw_variable_value('${BSOSVERSION}') or OS[bs_os.lower()],
-        'resolution': util.get_rfw_variable_value('${BSRESOLUTION}') or '1920x1080',
-        "local": util.get_rfw_variable_value('${BSLOCAL}') or "false",
-        "localIdentifier": util.get_rfw_variable_value('${BSLOCALID}') or '',
-        **kwargs, }
+        "os": bs_os,
+        "osVersion": util.get_rfw_variable_value("${BSOSVERSION}") or OS[bs_os.lower()],
+        "resolution": util.get_rfw_variable_value("${BSRESOLUTION}") or "1920x1080",
+        "local": util.get_rfw_variable_value("${BSLOCAL}") or "false",
+        "localIdentifier": util.get_rfw_variable_value("${BSLOCALID}") or "",
+        **kwargs,
+    }
 
     # handle issue where any, even empty value in localIdentifier turns local to true
-    if desired_caps["local"] == 'false':
+    if desired_caps["local"] == "false":
         del desired_caps["localIdentifier"]
 
     # create options instance based on selected browser
     options: Union[chrome_options, edge_options, firefox_options, safari_options]
 
-    if browser_name.lower() == 'chrome' or browser_name.lower() == 'gc':
+    if browser_name.lower() == "chrome" or browser_name.lower() == "gc":
         options = chrome_options()
-    elif browser_name.lower() == 'edge':
+    elif browser_name.lower() == "edge":
         options = edge_options()
-    elif browser_name.lower() == 'firefox' or browser_name.lower() == 'ff':
+    elif browser_name.lower() == "firefox" or browser_name.lower() == "ff":
         options = firefox_options()
-    elif browser_name.lower() == 'safari':
+    elif browser_name.lower() == "safari":
         options = safari_options()
     else:
-        raise exceptions.QWebException('Incorrect Browser name.')
+        raise exceptions.QWebException("Incorrect Browser name.")
 
-    browser_version = util.get_rfw_variable_value('${BROWSERVERSION}') or NAMES[bs_browser][1]
-    options.set_capability('browserVersion', browser_version)
-    options.set_capability('bstack:options', desired_caps)
+    browser_version = util.get_rfw_variable_value("${BROWSERVERSION}") or NAMES[bs_browser][1]
+    options.set_capability("browserVersion", browser_version)
+    options.set_capability("bstack:options", desired_caps)
 
     try:
-        executor_url = f'https://{bs_user}:{bs_key}@hub-cloud.browserstack.com/wd/hub'
+        executor_url = f"https://{bs_user}:{bs_key}@hub-cloud.browserstack.com/wd/hub"
         driver = webdriver.Remote(command_executor=executor_url, options=options)
-        logger.info(f'BrowserStack session ID: {driver.session_id}', also_console=True)
+        logger.info(f"BrowserStack session ID: {driver.session_id}", also_console=True)
     except WebDriverException as e:
         logger.error(str(e))
-        raise exceptions.QWebException('Incorrect Browserstack capabilities.')
+        raise exceptions.QWebException("Incorrect Browserstack capabilities.")
     browser.cache_browser(driver)
     return driver
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/bs_mobile.py` & `QWeb-3.3.0/QWeb/internal/browser/bs_mobile.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,49 +6,50 @@
 from selenium.common.exceptions import WebDriverException
 from typing import Any, Union
 from robot.api import logger
 from QWeb.internal import browser, exceptions, util
 
 
 def open_browser(bs_device: str, project_name: str, run_id: str, **kwargs: Any) -> WebDriver:
-
     desired_cap = {
         "buildName": project_name,
         "projectName": project_name,
         "sessionName": run_id,
         "deviceName": bs_device,
         "realMobile": "true",
-        "local": util.get_rfw_variable_value('${BSLOCAL}') or "false",
-        "localIdentifier": util.get_rfw_variable_value('${BSLOCALID}') or '',
-        **kwargs, }
+        "local": util.get_rfw_variable_value("${BSLOCAL}") or "false",
+        "localIdentifier": util.get_rfw_variable_value("${BSLOCALID}") or "",
+        **kwargs,
+    }
 
-    os_version = util.get_rfw_variable_value('${BSOSVERSION}')
+    os_version = util.get_rfw_variable_value("${BSOSVERSION}")
     if os_version:
         desired_cap["osVersion"] = os_version
 
     # handle issue where any, even empty value in localIdentifier turns local to true
-    if desired_cap["local"] == 'false':
+    if desired_cap["local"] == "false":
         del desired_cap["localIdentifier"]
 
     # create options instance based on selected browser
     options: Union[chrome_options, safari_options]
     if any(model in bs_device.lower() for model in ("iphone", "ipad")):
         options = safari_options()
     else:
         options = chrome_options()
 
-    options.set_capability('bstack:options', desired_cap)
+    options.set_capability("bstack:options", desired_cap)
 
-    bs_key = util.get_rfw_variable_value('${APIKEY}') or os.environ.get('bskey')
-    bs_user = util.get_rfw_variable_value('${USERNAME}') or os.environ.get('bsuser')
+    bs_key = util.get_rfw_variable_value("${APIKEY}") or os.environ.get("bskey")
+    bs_user = util.get_rfw_variable_value("${USERNAME}") or os.environ.get("bsuser")
 
     try:
         driver = webdriver.Remote(
-                 command_executor=f'http://{bs_user}:{bs_key}@hub.browserstack.com:80/wd/hub',
-                 options=options)
+            command_executor=f"http://{bs_user}:{bs_key}@hub.browserstack.com:80/wd/hub",
+            options=options,
+        )
 
-        logger.info(f'BrowserStack session ID: {driver.session_id}', also_console=True)
+        logger.info(f"BrowserStack session ID: {driver.session_id}", also_console=True)
     except WebDriverException as e:
         logger.error(str(e))
-        raise exceptions.QWebException('Incorrect Browserstack capabilities.')
+        raise exceptions.QWebException("Incorrect Browserstack capabilities.")
     browser.cache_browser(driver)
     return driver
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/chrome.py` & `QWeb-3.3.0/QWeb/internal/browser/chrome.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,42 +11,44 @@
 from QWeb.internal.config_defaults import CONFIG
 
 NAMES: list[str] = ["chrome", "gc"]
 
 
 def check_browser_reuse(**kwargs: Any) -> tuple[bool, Optional[str], Optional[str]]:
     try:
-        browser_reuse = util.par2bool(util.get_rfw_variable_value('${BROWSER_REUSE}')) or False
-        dbg_addr = kwargs.get('debugger_address', None) or \
-            util.get_rfw_variable_value('${BROWSER_DEBUGGER_ADDRESS}')
-        executor_url = kwargs.get('executor_url', None) or \
-            util.get_rfw_variable_value('${BROWSER_EXECUTOR_URL}')
+        browser_reuse = util.par2bool(util.get_rfw_variable_value("${BROWSER_REUSE}")) or False
+        dbg_addr = kwargs.get("debugger_address", None) or util.get_rfw_variable_value(
+            "${BROWSER_DEBUGGER_ADDRESS}"
+        )
+        executor_url = kwargs.get("executor_url", None) or util.get_rfw_variable_value(
+            "${BROWSER_EXECUTOR_URL}"
+        )
         return browser_reuse, dbg_addr, executor_url
     except RobotNotRunningError:
         pass
 
     return False, None, None
 
 
-def write_browser_session_argsfile(dbg_addr: str,
-                                   executor_url: str,
-                                   fname: str = 'browser_session.arg') -> str:
-    robot_output = util.get_rfw_variable_value('${OUTPUT DIR}')
+def write_browser_session_argsfile(
+    dbg_addr: str, executor_url: str, fname: str = "browser_session.arg"
+) -> str:
+    robot_output = util.get_rfw_variable_value("${OUTPUT DIR}")
     args_fn = os.path.join(robot_output or os.getcwd(), fname)
-    with open(args_fn, 'w') as args_file:
-        args_file.write(f'-v BROWSER_REUSE:{True}{os.linesep}')
-        args_file.write(f'-v BROWSER_DEBUGGER_ADDRESS:{dbg_addr}{os.linesep}')
-        args_file.write(f'-v BROWSER_EXECUTOR_URL:{executor_url}{os.linesep}')
+    with open(args_fn, "w") as args_file:
+        args_file.write(f"-v BROWSER_REUSE:{True}{os.linesep}")
+        args_file.write(f"-v BROWSER_DEBUGGER_ADDRESS:{dbg_addr}{os.linesep}")
+        args_file.write(f"-v BROWSER_EXECUTOR_URL:{executor_url}{os.linesep}")
 
     return args_fn
 
 
-def open_browser(executable_path: str = "",
-                 chrome_args: Optional[list[str]] = None,
-                 **kwargs: Any) -> WebDriver:
+def open_browser(
+    executable_path: str = "", chrome_args: Optional[list[str]] = None, **kwargs: Any
+) -> WebDriver:
     """Open Chrome browser instance and cache the driver.
 
     Parameters
     ----------
     executable_path : str (Default "chromedriver")
         path to the executable. If the default is used it assumes the
         executable is in the $PATH.
@@ -56,78 +58,80 @@
     desired_capabilities : dict (Default None)
         Dictionary object with non-browser specific capabilities only, such as
         "proxy" or "loggingPref".
     chrome_args : Optional arguments to modify browser settings
     """
     options = Options()
 
-    logger.debug('opt: {}'.format(options))
+    logger.debug("opt: {}".format(options))
     # Gets rid of Devtools listening .... printing
-    options.add_experimental_option('excludeSwitches', ['enable-logging'])
+    options.add_experimental_option("excludeSwitches", ["enable-logging"])
 
     # If user wants to re-use existing browser session then
     # he/she has to set variable BROWSER_REUSE_ENABLED to True.
     # If enabled, then web driver connection details are written
     # to an argument file. This file enables re-use of the current
     # chrome session.
     #
     # When variables BROWSER_DEBUGGER_ADDRESS and BROWSER_EXECUTOR_URL are
     # set from argument file, then OpenBrowser will use those
     # parameters instead of opening new chrome session.
     # New Remote Web Driver is created in headless mode.
-    chromedriver_path = util.get_rfw_variable_value('${CHROMEDRIVER_PATH}') or executable_path
-    chrome_path = kwargs.get('chrome_path', None) or util.get_rfw_variable_value('${CHROME_PATH}')
-    chrome_version_kwarg = kwargs.get('browser_version', None)
-    chrome_version = chrome_version_kwarg or util.get_rfw_variable_value('${BROWSER_VERSION}')
+    chromedriver_path = util.get_rfw_variable_value("${CHROMEDRIVER_PATH}") or executable_path
+    chrome_path = kwargs.get("chrome_path", None) or util.get_rfw_variable_value("${CHROME_PATH}")
+    chrome_version_kwarg = kwargs.get("browser_version", None)
+    chrome_version = chrome_version_kwarg or util.get_rfw_variable_value("${BROWSER_VERSION}")
     if chrome_path:
         options.binary_location = chrome_path
     if chrome_version:
         options.browser_version = chrome_version
     browser_reuse, debugger_address, executor_url = check_browser_reuse(**kwargs)
-    logger.debug(f'browser_reuse: {browser_reuse}, '
-                 f'executor_url: {executor_url}, '
-                 f'debugger_address: {debugger_address}')
+    logger.debug(
+        f"browser_reuse: {browser_reuse}, "
+        f"executor_url: {executor_url}, "
+        f"debugger_address: {debugger_address}"
+    )
     if browser_reuse and executor_url and debugger_address:
         options_new = Options()
         options_new.add_argument("headless")
         options_new.debugger_address = debugger_address
         service = Service()
-        driver = Chrome(service=service,
-                        options=options_new)
+        driver = Chrome(service=service, options=options_new)
     else:
         if user.is_root():
             options.add_argument("no-sandbox")
         if chrome_args:
-            if any('headless' in _.lower() for _ in chrome_args):
-                CONFIG.set_value('Headless', True)
+            if any("headless" in _.lower() for _ in chrome_args):
+                CONFIG.set_value("Headless", True)
             for item in chrome_args:
                 options.add_argument(item.lstrip())
         options.add_argument("start-maximized")
         options.add_argument("--disable-notifications")
-        if 'headless' in kwargs:
-            CONFIG.set_value('Headless', True)
+        if "headless" in kwargs:
+            CONFIG.set_value("Headless", True)
             options.add_argument("headless")
-        if 'prefs' in kwargs:
-            tmp_prefs = kwargs.get('prefs')
+        if "prefs" in kwargs:
+            tmp_prefs = kwargs.get("prefs")
             prefs = util.parse_prefs(tmp_prefs)
-            options.add_experimental_option('prefs', prefs)
-        if 'emulation' in kwargs:
-            emulation = kwargs['emulation']
+            options.add_experimental_option("prefs", prefs)
+        if "emulation" in kwargs:
+            emulation = kwargs["emulation"]
             emulate_device = util.get_emulation_pref(emulation)
             options.add_experimental_option("mobileEmulation", emulate_device)
 
         service = Service(chromedriver_path) if chromedriver_path else Service()
         driver = Chrome(service=service, options=options)
 
-        browser_reuse_enabled = util.par2bool(
-            util.get_rfw_variable_value('${BROWSER_REUSE_ENABLED}')) or False
+        browser_reuse_enabled = (
+            util.par2bool(util.get_rfw_variable_value("${BROWSER_REUSE_ENABLED}")) or False
+        )
         if browser_reuse_enabled:
             # Write WebDriver session info to RF arguments file for re-use
             dbg_address = driver.capabilities["goog:chromeOptions"]["debuggerAddress"]
             write_browser_session_argsfile(dbg_address, driver.command_executor._url)  # type: ignore # pylint: disable=protected-access,line-too-long
 
             # Clear possible existing global values
-            BuiltIn().set_global_variable('${BROWSER_EXECUTOR_URL}', None)
-            BuiltIn().set_global_variable('${BROWSER_DEBUGGER_ADDRESS}', None)
+            BuiltIn().set_global_variable("${BROWSER_EXECUTOR_URL}", None)
+            BuiltIn().set_global_variable("${BROWSER_DEBUGGER_ADDRESS}", None)
 
     browser.cache_browser(driver)
     return driver
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/edge.py` & `QWeb-3.3.0/QWeb/internal/browser/edge.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from robot.api import logger
 from QWeb.internal.config_defaults import CONFIG
 from QWeb.internal import browser, user, util
 
 NAMES: list[str] = ["edge", "msedge"]
 
 
-def open_browser(executable_path: str = "",
-                 edge_args: Optional[list[str]] = None,
-                 **kwargs: Any) -> WebDriver:
+def open_browser(
+    executable_path: str = "", edge_args: Optional[list[str]] = None, **kwargs: Any
+) -> WebDriver:
     """Open Edge browser instance and cache the driver.
 
     Parameters
     ----------
     executable_path : str (Default "msedgedriver")
         path to the executable. If the default is used it assumes the
         executable is in the $PATH.
@@ -34,51 +34,57 @@
     #     Remove all usages of the EdgeOptions.UseChromium property.
     #     This property no longer exists in Selenium 4,
     #     because Selenium 4 supports only Microsoft Edge (Chromium)
     # options.use_chromium = True  # pylint: disable=no-member
 
     # Gets rid of Devtools listening .... printing
     # other non-sensical error messages
-    options.add_experimental_option('excludeSwitches', ['enable-logging'])  # pylint: disable=no-member
+    options.add_experimental_option("excludeSwitches", ["enable-logging"])  # pylint: disable=no-member
 
     # If user wants to re-use existing browser session then
     # he/she has to set variable BROWSER_REUSE_ENABLED to True.
     # If enabled, then web driver connection details are written
     # to an argument file. This file enables re-use of the current
     # chrome session.
     #
     # When variables BROWSER_SESSION_ID and BROWSER_EXECUTOR_URL are
     # set from argument file, then OpenBrowser will use those
     # parameters instead of opening new chrome session.
     # New Remote Web Driver is created in headless mode.
-    edgedriver_path = util.get_rfw_variable_value('${EDGEDRIVER_PATH}') or executable_path
-    edge_path = kwargs.get('edge_path', None) or util.get_rfw_variable_value('${EDGE_PATH}')
+    edgedriver_path = util.get_rfw_variable_value("${EDGEDRIVER_PATH}") or executable_path
+    edge_path = kwargs.get("edge_path", None) or util.get_rfw_variable_value("${EDGE_PATH}")
     if edge_path:
         options.binary_location = edge_path  # pylint: disable=no-member
 
+    edge_version_kwarg = kwargs.get("browser_version", None)
+    edge_version = edge_version_kwarg or util.get_rfw_variable_value("${BROWSER_VERSION}")
+
+    if edge_version:
+        options.browser_version = edge_version
+
     if user.is_root() or user.is_docker():
         options.add_argument("no-sandbox")  # pylint: disable=no-member
     if edge_args:
-        if any('--headless' in _.lower() for _ in edge_args):
-            CONFIG.set_value('Headless', True)
+        if any("--headless" in _.lower() for _ in edge_args):
+            CONFIG.set_value("Headless", True)
         for item in edge_args:
             options.add_argument(item.lstrip())  # pylint: disable=no-member
     options.add_argument("start-maximized")  # pylint: disable=no-member
     options.add_argument("--disable-notifications")  # pylint: disable=no-member
-    if 'headless' in kwargs:
-        CONFIG.set_value('Headless', True)
+    if "headless" in kwargs:
+        CONFIG.set_value("Headless", True)
         options.add_argument("--headless")  # pylint: disable=no-member
-    if 'prefs' in kwargs:
-        tmp_prefs = kwargs.get('prefs')
+    if "prefs" in kwargs:
+        tmp_prefs = kwargs.get("prefs")
         prefs = util.parse_prefs(tmp_prefs)
-        options.add_experimental_option('prefs', prefs)
+        options.add_experimental_option("prefs", prefs)
         logger.warn("prefs: {}".format(prefs))
 
-    if 'emulation' in kwargs:
-        emulation = kwargs['emulation']
+    if "emulation" in kwargs:
+        emulation = kwargs["emulation"]
         emulate_device = util.get_emulation_pref(emulation)
         options.add_experimental_option("mobileEmulation", emulate_device)
 
     service = Service(edgedriver_path) if edgedriver_path else Service()
     driver = Edge(service=service, options=options)
 
     # driver = Edge(
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/firefox.py` & `QWeb-3.3.0/QWeb/internal/browser/firefox.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
 LOGGER: Logger = logging.getLogger(__name__)
 
 NAMES: list[str] = ["firefox", "ff"]
 
 
 # pylint: disable=too-many-branches
-def open_browser(profile_dir: Optional[str] = None,
-                 headless: bool = False,
-                 binary: Optional[str] = None,
-                 driver_path: str = "",
-                 firefox_args: Optional[list[str]] = None,
-                 log_path: str = "geckodriver.log",
-                 **kwargs: Any) -> WebDriver:
+def open_browser(
+    profile_dir: Optional[str] = None,
+    headless: bool = False,
+    binary: Optional[str] = None,
+    driver_path: str = "",
+    firefox_args: Optional[list[str]] = None,
+    log_path: str = "geckodriver.log",
+    **kwargs: Any,
+) -> WebDriver:
     """Open Firefox browser and cache the driver.
 
     Parameters
     ----------
     binary : FirefoxBinary or str
         If string then is needs to be the absolute path to the binary. If
         undefined, the system default Firefox installation will be used.
@@ -46,64 +48,69 @@
         Where to log information from the driver.
     firefox_args : list
         Optional arguments to modify browser settings.
         https://developer.mozilla.org/en-US/docs/Mozilla/Command_Line_Options
     """
     options = Options()
     if headless:
-        logger.warn('Deprecated.\n'
-                    'Headless mode can be activated just like any other firefox option:\n'
-                    '"OpenBrowser   https://qentinel.com    ${BROWSER}   -headless"')
-        options.add_argument('-headless')
+        logger.warn(
+            "Deprecated.\n"
+            "Headless mode can be activated just like any other firefox option:\n"
+            '"OpenBrowser   https://qentinel.com    ${BROWSER}   -headless"'
+        )
+        options.add_argument("-headless")
         CONFIG.set_value("Headless", True)
     # if profile_dir:
     #     logger.warn('Deprecated.\n'
     #                 'Profile directory can be selected like any other firefox option:\n'
     #                 '"OpenBrowser   https://site.com   ${BROWSER}  -profile /path/to/profile"')
     #     # options.add_argument('-profile {}'.format(profile_dir))
-
+    ff_version_kwarg = kwargs.get("browser_version", None)
+    ff_version = ff_version_kwarg or util.get_rfw_variable_value("${BROWSER_VERSION}")
+    if ff_version:
+        options.browser_version = ff_version
     options.set_preference("browser.helperApps.neverAsk.saveToDisk", browser.MIME_TYPES)
     options.set_preference("extensions.update.enabled", False)
     options.set_preference("app.update.enabled", False)
     options.set_preference("app.update.auto", False)
     options.set_preference("dom.webnotifications.enabled", False)
     options.set_preference("privacy.socialtracking.block_cookies.enabled", False)
     kwargs = {k.lower(): v for k, v in kwargs.items()}  # Kwargs keys to lowercase
-    if 'prefs' in kwargs:
-        tmp_prefs = kwargs.get('prefs')
+    if "prefs" in kwargs:
+        tmp_prefs = kwargs.get("prefs")
         prefs = util.parse_prefs(tmp_prefs)
 
         for item in prefs.items():  # type: ignore[union-attr]
             key, value = item[0], item[1]
-            logger.info('Using prefs: {} = {}'.format(key, value), also_console=True)
+            logger.info("Using prefs: {} = {}".format(key, value), also_console=True)
             if not isinstance(value, int) and value.isdigit():
                 value = int(value)
             options.set_preference(key, value)
     if firefox_args:
-        if any('headless' in _.lower() for _ in firefox_args):
+        if any("headless" in _.lower() for _ in firefox_args):
             CONFIG.set_value("Headless", True)
         for option in firefox_args:
             option = option.strip()
             if option.startswith("-profile"):
                 profile_dir = _get_profile_dir(option)
                 options.add_argument("-profile")
                 options.add_argument(profile_dir)
             elif option.startswith("-"):
                 options.add_argument(option)
             else:
-                logger.warn(f'Firefox arguments start with "-". '
-                            f'Argument "{option}" has incorrect format and was ignored')
+                logger.warn(
+                    f'Firefox arguments start with "-". '
+                    f'Argument "{option}" has incorrect format and was ignored'
+                )
 
     if binary:
         options.binary_location = binary
     service = Service(driver_path, log_path=log_path) if driver_path else Service(log_path=log_path)
-    driver = webdriver.Firefox(service=service,
-                               options=options
-                               )
-    if os.name == 'nt':  # Maximize window if running on windows, doesn't work on linux
+    driver = webdriver.Firefox(service=service, options=options)
+    if os.name == "nt":  # Maximize window if running on windows, doesn't work on linux
         driver.maximize_window()
     browser.cache_browser(driver)
     return driver
 
 
 def _get_profile_dir(option_str: str) -> Optional[str]:
     try:
```

### Comparing `QWeb-3.2.1/QWeb/internal/browser/safari.py` & `QWeb-3.3.0/QWeb/internal/browser/safari.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,37 @@
 
 from QWeb.internal import browser
 
 NAMES: list[str] = ["safari", "sf"]
 open_windows: list[str] = []
 
 
-def open_browser(port: int = 0,
-                 driver_path: str = '',
-                 desired_capabilities: Optional[dict[str, Any]] = None,
-                 quiet: bool = False) -> WebDriver:
-
+def open_browser(
+    port: int = 0,
+    driver_path: str = "",
+    desired_capabilities: Optional[dict[str, Any]] = None,
+    quiet: bool = False,
+) -> WebDriver:
     options = Options()
 
     # safari options can be given as desired_capabilities (dict)
     # Example:
     #   &{caps}=   Create Dictionary  safari:automaticInspection=True
     #   openbrowser  https://www.google.com  safari   desired_capabilities=${caps}
     if desired_capabilities:
         try:
             for k, v in desired_capabilities.items():
                 options.set_capability(k, v)
         except AttributeError:
-            logger.warn("Safari options/desired capabilities "
-                        "should be given as a dictionary. Example:\n\n"
-                        "&{caps}=\tCreate Dictionary\tsafari:automaticInspection=True\n"
-                        "OpenBrowser\thttps://www.google.com\tsafari\tdesired_capabilities=${caps}"
-                        )
+            logger.warn(
+                "Safari options/desired capabilities "
+                "should be given as a dictionary. Example:\n\n"
+                "&{caps}=\tCreate Dictionary\tsafari:automaticInspection=True\n"
+                "OpenBrowser\thttps://www.google.com\tsafari\tdesired_capabilities=${caps}"
+            )
 
     if driver_path:
         service = service = Service(driver_path, port=port, quiet=quiet)
     else:
         service = Service(port=port, quiet=quiet)
 
     driver = webdriver.Safari(service=service, options=options)
```

### Comparing `QWeb-3.2.1/QWeb/internal/checkbox.py` & `QWeb-3.3.0/QWeb/internal/checkbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,23 +68,24 @@
     if locator.startswith("xpath=") or locator.startswith("//"):
         index = util.anchor_to_index(anchor)
         checkbox_element = element.get_unique_element_by_xpath(locator, index=index)
         # TODO: Check that the element is actually a checkbox
     else:  # No prefix given
         text_element = text.get_text_using_anchor(locator, anchor)
         xpath = '//input[@type="checkbox"]|//*[@role="checkbox"]'
-        checkbox_elements = element.get_webelements_in_active_area(xpath,
-                                                                   stay_in_current_frame=True)
+        checkbox_elements = element.get_webelements_in_active_area(
+            xpath, stay_in_current_frame=True
+        )
         checkbox_element = element.get_closest_element(text_element, checkbox_elements)
     return checkbox_element, None
 
 
-def get_checkbox_elements_from_all_documents(locator: str, anchor: str, index: Union[int, str],
-                                             **kwargs: Any
-                                             ) -> tuple[WebElement, Optional[WebElement]]:
+def get_checkbox_elements_from_all_documents(
+    locator: str, anchor: str, index: Union[int, str], **kwargs: Any
+) -> tuple[WebElement, Optional[WebElement]]:
     """Function for finding checkbox elements.
     Parameters
     ----------
     locator : str
         Label text or attribute that points to the checkbox.
     anchor : str
         in case there is duplicates.
@@ -99,57 +100,57 @@
 
     index = int(index) - 1
     css_selector = CONFIG["CssSelectors"]
     css = '[type="checkbox"], [role="checkbox"]'
     if Table.is_table_coordinates(locator):
         table = Table.ACTIVE_TABLE.update_table()
         if table is None:
-            raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+            raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
         locator_element = table.get_table_cell(locator, anchor)
-        checkbox_elements = element.get_element_from_childnodes(locator_element,
-                                                                css,
-                                                                dom_traversing=False,
-                                                                **kwargs)
+        checkbox_elements = element.get_element_from_childnodes(
+            locator_element, css, dom_traversing=False, **kwargs
+        )
         if checkbox_elements:
             return checkbox_elements[index], locator_element
-        raise QWebElementNotFoundError('No matching checkbox found')
-    if not css_selector or locator.startswith('xpath=') or locator.startswith('//'):
+        raise QWebElementNotFoundError("No matching checkbox found")
+    if not css_selector or locator.startswith("xpath=") or locator.startswith("//"):
         checkbox_element, locator_element = get_checkbox_by_locator(locator, anchor=anchor)
     else:
-        checkbox_element, locator_element = get_checkbox_by_css_selector(locator,
-                                                                         anchor=anchor,
-                                                                         index=index,
-                                                                         **kwargs)
+        checkbox_element, locator_element = get_checkbox_by_css_selector(
+            locator, anchor=anchor, index=index, **kwargs
+        )
         if not checkbox_element:
             checkbox_element, locator_element = get_checkbox_by_locator(locator, anchor)
     if checkbox_element:
         return checkbox_element, locator_element
-    raise QWebElementNotFoundError('No matching element found')
+    raise QWebElementNotFoundError("No matching element found")
 
 
 def get_checkbox_by_css_selector(
-        locator: str, anchor: str, index: int,
-        **kwargs: Any) -> tuple[Optional[WebElement], Optional[WebElement]]:
+    locator: str, anchor: str, index: int, **kwargs: Any
+) -> tuple[Optional[WebElement], Optional[WebElement]]:
     """Get checkbox using css selectors."""
     checkbox_elements = []
     partial_matches: list[WebElement] = []
     css = '[type="checkbox"], [role="checkbox"]'
-    if 'qweb_old' not in kwargs:
+    if "qweb_old" not in kwargs:
         full_matches, partial_matches = element.get_elements_by_css(locator, css, **kwargs)
         if full_matches:
             checkbox_elements = element.get_visible_elements_from_elements(full_matches, **kwargs)
             if checkbox_elements:
                 return checkbox_elements[index], None
     try:
         locator_element = text.get_text_using_anchor(locator, anchor)
         checkbox_elements = list(
             dict.fromkeys(
                 element.get_element_from_childnodes(locator_element, css, **kwargs)
-                + partial_matches))
+                + partial_matches
+            )
+        )
         return checkbox_elements[index], locator_element
     except QWebElementNotFoundError:
-        logger.trace('Element not found by visible text. Trying with partial match')
+        logger.trace("Element not found by visible text. Trying with partial match")
         checkbox_elements = partial_matches
     if checkbox_elements:
         logger.debug("Found element {}, index {}".format(checkbox_elements, index))
         return checkbox_elements[index], None
     return None, None
```

### Comparing `QWeb-3.2.1/QWeb/internal/config.py` & `QWeb-3.3.0/QWeb/internal/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,35 +17,34 @@
 from __future__ import annotations
 from typing import Any, Optional
 
 import copy
 
 
 class Config:
-
     DROPPED_DELIMITER_CHARS: str = " _-"
 
     def __init__(self, config_defaults: dict[str, Any]) -> None:
         self._config_defaults = {}
         # Clean config_defaults key values before storage
         _config_defaults = {}
         for k, v in config_defaults.items():
             _k = self._clean_string(k)
             _config_defaults[_k] = copy.deepcopy(v)
         self._config_defaults.update(_config_defaults)
         self.config = copy.deepcopy(self._config_defaults)
 
     def is_value(self, par: str) -> bool:
-        """ Return True if parameter exists. """
+        """Return True if parameter exists."""
         _par = self._clean_string(par)
         return _par in self.config
 
     def get_value(self, par: str) -> Optional[Any]:
-        """ Return value(s) for given parameter,
-            or None if parameter doesn't exist. """
+        """Return value(s) for given parameter,
+        or None if parameter doesn't exist."""
         _par = self._clean_string(par)
         config_value, _ = self.config.get(_par, (None, None))
         return config_value
 
     def get_all_values(self) -> dict[str, Any]:
         """
         Return all configuration values in a dictionary.
@@ -53,26 +52,26 @@
         """
         _all_configs = {}
         for k, v in self.config.items():
             _all_configs[k] = copy.deepcopy(v[0])
         return _all_configs
 
     def set_value(self, par: str, value: Any) -> Any:
-        """ Set value for given parameter. Setter uses pre-defined adapter function to process value
-        before storage. Adapter functions are set in config_defaults. Returns old value. """
+        """Set value for given parameter. Setter uses pre-defined adapter function to process value
+        before storage. Adapter functions are set in config_defaults. Returns old value."""
         _par = self._clean_string(par)
         if not self.is_value(_par):
             raise ValueError("Parameter {} doesn't exist".format(par))
         old_val, adapter_func = self.config[_par]
         stored_value = adapter_func(value) if adapter_func else value
         self.config[_par] = (stored_value, adapter_func)
         return old_val
 
     def reset_value(self, par: Optional[str] = None) -> None:
-        """ Reset value(s) to original. """
+        """Reset value(s) to original."""
         if par:
             _par = self._clean_string(par)
             self.config[_par] = copy.deepcopy(self._config_defaults[_par])
             # trigger adapter func for clearkey
             if "clearkey" in _par:
                 val, adapter_func = self.config[_par]
                 if adapter_func:
@@ -81,15 +80,15 @@
             self.config = copy.deepcopy(self._config_defaults)
             # handle clearkey separately
             _par = self._clean_string("ClearKey")
             val, adapter_func = self.config[_par]
             self.set_value(_par, str(val))
 
     def __getitem__(self, par: str) -> Any:
-        """ Allow accessing parameters in dictionary like syntax."""
+        """Allow accessing parameters in dictionary like syntax."""
         _par = self._clean_string(par)
         config_value, _ = self.config[_par]
         return config_value
 
     def __repr__(self) -> dict[str, Any]:  # type: ignore[override]
         return self.config
```

### Comparing `QWeb-3.2.1/QWeb/internal/config_defaults.py` & `QWeb-3.3.0/QWeb/internal/config_defaults.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 Usage from test script:
 SetConfig    ScreenshotType    all
 
 Usage from code:
 from QWeb.internal.config_defaults import CONFIG
 val = CONFIG["ScreenshotType"]
 """
+
 from __future__ import annotations
 from typing import Any, Union
 
 from QWeb.internal.search_strategy import SearchStrategies
 from QWeb.internal import util
 from QWeb.internal.config import Config
 
@@ -48,23 +49,31 @@
     "SearchDirection": ("closest", SearchStrategies.search_direction_validation),
     "CheckInputValue": (False, util.par2bool),
     "DefaultTimeout": ("10s", SearchStrategies.default_timeout_validation),
     "XHRTimeout": ("30", SearchStrategies.xhr_timeout_validation),
     "DefaultDocument": (True, util.par2bool),
     "InputHandler": ("selenium", util.set_input_handler),
     "CaseInsensitive": (False, util.par2bool),
-    "AllInputElements":
-    (SearchStrategies.ALL_INPUT_ELEMENTS, SearchStrategies.all_input_elements_validation),
-    "MatchingInputElement":
-    (SearchStrategies.MATCHING_INPUT_ELEMENT, SearchStrategies.matching_input_element_validation),
-    "ActiveAreaXpath":
-    (SearchStrategies.ACTIVE_AREA_XPATH, SearchStrategies.active_area_xpath_validation),
+    "AllInputElements": (
+        SearchStrategies.ALL_INPUT_ELEMENTS,
+        SearchStrategies.all_input_elements_validation,
+    ),
+    "MatchingInputElement": (
+        SearchStrategies.MATCHING_INPUT_ELEMENT,
+        SearchStrategies.matching_input_element_validation,
+    ),
+    "ActiveAreaXpath": (
+        SearchStrategies.ACTIVE_AREA_XPATH,
+        SearchStrategies.active_area_xpath_validation,
+    ),
     "TextMatch": (SearchStrategies.TEXT_MATCH, SearchStrategies.text_match_validation),
-    "ContainingTextMatch": (SearchStrategies.CONTAINING_TEXT_MATCH_CASE_SENSITIVE,
-                            SearchStrategies.containing_text_match_validation),
+    "ContainingTextMatch": (
+        SearchStrategies.CONTAINING_TEXT_MATCH_CASE_SENSITIVE,
+        SearchStrategies.containing_text_match_validation,
+    ),
     "IsModalXpath": (SearchStrategies.IS_MODAL_XPATH, SearchStrategies.clear_xpath),
     "VerifyAppAccuracy": (0.9999, None),
     "OffsetCheck": (True, util.par2bool),
     "Visibility": (True, util.par2bool),
     "InViewport": (False, util.par2bool),
     "WindowSize": ((0, 0), util.set_window_size),
     "DoubleClick": (False, util.par2bool),
@@ -74,25 +83,25 @@
     "MultipleAnchors": (False, util.par2bool),
     "WindowFind": (False, util.par2bool),
     "ClickToFocus": (False, util.par2bool),
     "Debug_Run": (False, False),
     "HandleAlerts": (True, util.par2bool),
     "BlindReturn": (False, util.par2bool),
     "Headless": (False, util.par2bool),
-    "Delay": ('0s', SearchStrategies.default_timeout_validation),
+    "Delay": ("0s", SearchStrategies.default_timeout_validation),
     "RunBefore": (None, util.validate_run_before),
-    "RetryInterval": ('5s', SearchStrategies.default_timeout_validation),
+    "RetryInterval": ("5s", SearchStrategies.default_timeout_validation),
     "RetryError": (None, None),
     "StayInCurrentFrame": (False, util.par2bool),
     "FrameTimeout": ("10s", SearchStrategies.default_timeout_validation),
     "AllTextNodes": (False, util.par2bool),
     "OSScreenshots": (False, util.par2bool),
     "RetinaDisplay": (util.is_retina(), util.par2bool),
     "LogMatchedIcons": (False, util.par2bool),
     "ShadowDOM": (False, util.par2bool),
-    "HighlightColor": ("blue", util.highlight_validation)
+    "HighlightColor": ("blue", util.highlight_validation),
 }
 
 CONFIG: Config = Config(CONFIG_DEFAULTS)
 RETRIES_AMOUNT: int = 3
 SHORT_DELAY: Union[int, float] = 0.2
 LONG_DELAY: Union[int, float] = 1
```

### Comparing `QWeb-3.2.1/QWeb/internal/cookies.py` & `QWeb-3.3.0/QWeb/internal/cookies.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.2.1/QWeb/internal/decorators.py` & `QWeb-3.3.0/QWeb/internal/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,181 +19,216 @@
 from typing import Callable, Any, Union
 
 import time
 from inspect import signature
 from functools import wraps
 from robot.utils import timestr_to_secs
 from robot.api import logger
-from selenium.common.exceptions import InvalidSelectorException, \
-    NoSuchElementException, StaleElementReferenceException, WebDriverException, \
-    UnexpectedAlertPresentException, InvalidSessionIdException
+from selenium.common.exceptions import (
+    InvalidSelectorException,
+    NoSuchElementException,
+    StaleElementReferenceException,
+    WebDriverException,
+    UnexpectedAlertPresentException,
+    InvalidSessionIdException,
+)
 from QWeb.keywords import config
 from QWeb.internal import frame
 from QWeb.internal.config_defaults import CONFIG, SHORT_DELAY, LONG_DELAY
-from QWeb.internal.exceptions import QWebElementNotFoundError, \
-    QWebStalingElementError, QWebDriverError, QWebTimeoutError, QWebValueError, \
-    QWebUnexpectedConditionError, QWebValueMismatchError, QWebSearchingMode, QWebUnexpectedAlert, \
-    QWebIconNotFoundError, QWebBrowserError, FATAL_MESSAGES
+from QWeb.internal.exceptions import (
+    QWebElementNotFoundError,
+    QWebStalingElementError,
+    QWebDriverError,
+    QWebTimeoutError,
+    QWebValueError,
+    QWebUnexpectedConditionError,
+    QWebValueMismatchError,
+    QWebSearchingMode,
+    QWebUnexpectedAlert,
+    QWebIconNotFoundError,
+    QWebBrowserError,
+    FATAL_MESSAGES,
+)
 
 
 # pylint: disable=too-many-statements
 # pylint: disable=too-many-branches
 def timeout_decorator(fn: Callable[..., Any]) -> Callable[..., Any]:
-
     @wraps(fn)
     def get_elements_from_dom_content(  # type: ignore[return] # pylint: disable=R1710
-            *args: Any, **kwargs: Any) -> Union[Callable[..., Any], int, bool, None]:
+        *args: Any, **kwargs: Any
+    ) -> Union[Callable[..., Any], int, bool, None]:
         try:
             args, kwargs, locator = _equal_sign_handler(args, kwargs, fn)
             msg: Union[WebDriverException, QWebDriverError, QWebValueError, None] = None
             params = signature(fn).parameters
             args, kwargs = _args_to_kwargs(params, args, kwargs)
             timeout = get_timeout(**kwargs)
-            logger.debug('Timeout is {} sec'.format(timeout))
+            logger.debug("Timeout is {} sec".format(timeout))
 
             try:
-                if 'go_to' not in str(fn) and 'switch_window' not in str(fn):
+                if "go_to" not in str(fn) and "switch_window" not in str(fn):
                     frame.wait_page_loaded()
             except UnexpectedAlertPresentException as e:
                 if not CONFIG["HandleAlerts"]:
                     raise QWebUnexpectedAlert(str(e)) from e
-                logger.debug('Got {}. Trying to retry..'.format(e))
+                logger.debug("Got {}. Trying to retry..".format(e))
                 time.sleep(SHORT_DELAY)
             start = time.time()
             while time.time() < timeout + start:
                 try:
-                    kwargs['timeout'] = float(timeout + start - time.time())
-                    config.set_config('FrameTimeout', float(timeout + start - time.time()))
+                    kwargs["timeout"] = float(timeout + start - time.time())
+                    config.set_config("FrameTimeout", float(timeout + start - time.time()))
                     return fn(*args, **kwargs)
                 except (QWebUnexpectedConditionError, QWebTimeoutError) as e:
-                    logger.debug('Got {}'.format(e))
-                except (InvalidSelectorException, NoSuchElementException, QWebElementNotFoundError,
-                        UnexpectedAlertPresentException, QWebStalingElementError,
-                        StaleElementReferenceException, QWebIconNotFoundError) as e:
+                    logger.debug("Got {}".format(e))
+                except (
+                    InvalidSelectorException,
+                    NoSuchElementException,
+                    QWebElementNotFoundError,
+                    UnexpectedAlertPresentException,
+                    QWebStalingElementError,
+                    StaleElementReferenceException,
+                    QWebIconNotFoundError,
+                ) as e:
                     time.sleep(SHORT_DELAY)
-                    logger.debug('Got exception: {}. Trying to retry..'.format(e))
+                    logger.debug("Got exception: {}. Trying to retry..".format(e))
                 except InvalidSessionIdException as e:
                     CONFIG.set_value("OSScreenshots", True)
                     raise QWebBrowserError("Browser session lost. Did browser crash?") from e
                 except (WebDriverException, QWebDriverError) as e:
                     if any(s in str(e) for s in FATAL_MESSAGES):
                         CONFIG.set_value("OSScreenshots", True)
                         raise QWebBrowserError(e)  # pylint: disable=W0707
-                    logger.debug('From timeout decorator: Webdriver exception. Retrying..')
+                    logger.debug("From timeout decorator: Webdriver exception. Retrying..")
                     logger.debug(str(e))
                     time.sleep(SHORT_DELAY)
                     err = QWebDriverError
                     msg = e
                 except QWebValueError as ve:
-                    logger.debug('Got QWebValueError: {}. Trying to retry..'.format(ve))
+                    logger.debug("Got QWebValueError: {}. Trying to retry..".format(ve))
                     err = QWebValueError  # type: ignore[assignment]
                     msg = ve
                     time.sleep(SHORT_DELAY)
             if msg:
                 # pylint: disable=used-before-assignment
                 raise err(msg)
-            if 'count' in str(fn):
+            if "count" in str(fn):
                 return 0
-            if 'is_text' in str(fn) or 'is_no_text' in str(fn):
+            if "is_text" in str(fn) or "is_no_text" in str(fn):
                 return False
-            raise QWebElementNotFoundError('Unable to find element for locator {} in {} sec'.format(
-                locator, timeout))
+            raise QWebElementNotFoundError(
+                "Unable to find element for locator {} in {} sec".format(locator, timeout)
+            )
         except QWebSearchingMode:
             pass
 
     return get_elements_from_dom_content
 
 
 def timeout_decorator_for_actions(fn: Callable[..., Any]) -> Callable[..., Any]:
-
     @wraps(fn)
     def perform(*args: Any, **kwargs: Any) -> Callable[..., Any]:
         params = signature(fn).parameters
         args, kwargs = _args_to_kwargs(params, args, kwargs)
         timeout = get_timeout(**kwargs)
         err = None
         msg = None
         performed = False
-        logger.debug('time to run {}'.format(timeout))
+        logger.debug("time to run {}".format(timeout))
         start = time.time()
         while time.time() < timeout + start:
             try:
                 return fn(*args, **kwargs)
             except QWebValueMismatchError as mismatch:
-                if 'text_appearance' not in str(fn) and 'get_or_compare_text' not in str(fn):
+                if "text_appearance" not in str(fn) and "get_or_compare_text" not in str(fn):
                     err = QWebValueError
                     msg = mismatch
-                logger.trace('Value mismatch: {}'.format(mismatch))
+                logger.trace("Value mismatch: {}".format(mismatch))
                 continue
             except (QWebElementNotFoundError, UnexpectedAlertPresentException):
-                logger.debug('Not found')
+                logger.debug("Not found")
                 time.sleep(SHORT_DELAY)
             except QWebValueError as ve:
                 if performed:
                     break
                 raise ve
             except (QWebStalingElementError, StaleElementReferenceException) as S:
-                if 'execute_click' in str(fn) or 'text_appearance' in str(fn):
-                    logger.debug('Got staling element err from retry click.'
-                                 'Action is probably triggered.')
+                if "execute_click" in str(fn) or "text_appearance" in str(fn):
+                    logger.debug(
+                        "Got staling element err from retry click. Action is probably triggered."
+                    )
                     raise QWebUnexpectedConditionError(S)  # pylint: disable=W0707
-                raise QWebStalingElementError('Staling element')  # pylint: disable=W0707
+                raise QWebStalingElementError("Staling element")  # pylint: disable=W0707
             except (WebDriverException, QWebDriverError) as wde:
-                if 'alert' in str(fn):
+                if "alert" in str(fn):
                     time.sleep(LONG_DELAY)
                     logger.debug("Got webdriver exception..{}. Retrying..".format(wde))
                     err = QWebDriverError  # type: ignore[assignment]
                     msg = wde  # type: ignore[assignment]
                 else:
                     raise QWebDriverError(wde)  # pylint: disable=W0707
         if msg:
             raise err(msg)  # type: ignore[misc]
-        raise QWebTimeoutError('Timeout exceeded')
+        raise QWebTimeoutError("Timeout exceeded")
 
     return perform
 
 
 def get_timeout(**kwargs: Any) -> Union[int, float]:
     timeout = timestr_to_secs(CONFIG["DefaultTimeout"])
-    if 'timeout' in kwargs:
-        if timestr_to_secs(kwargs['timeout']) != 0:
-            timeout = timestr_to_secs(kwargs['timeout'])
+    if "timeout" in kwargs:
+        if timestr_to_secs(kwargs["timeout"]) != 0:
+            timeout = timestr_to_secs(kwargs["timeout"])
     return timeout
 
 
-def _args_to_kwargs(params: MappingProxyType[str, Any], args: tuple,
-                    kwargs: dict) -> tuple[tuple, dict]:
-    if 'timeout' not in kwargs:
+def _args_to_kwargs(
+    params: MappingProxyType[str, Any], args: tuple, kwargs: dict
+) -> tuple[tuple, dict]:
+    if "timeout" not in kwargs:
         for i, p in enumerate(params.values()):
             if p.name not in kwargs:
                 if len(args) > i:
                     kwargs[p.name] = args[i]
                 else:
                     kwargs[p.name] = p.default
-        args = tuple('')
+        args = tuple("")
     return tuple(args), kwargs
 
 
-def _equal_sign_handler(args: Union[tuple, list], kwargs: dict,
-                        function_name: Union[str, Callable[..., Any]]) -> tuple[tuple, dict, str]:
+def _equal_sign_handler(
+    args: Union[tuple, list], kwargs: dict, function_name: Union[str, Callable[..., Any]]
+) -> tuple[tuple, dict, str]:
     try:
         locator = args[0]
     except IndexError:
         for key, value in kwargs.items():
             # if present any of these is always the first argument
             # locator can be the 2nd arg but it is handled later on
-            if key in ('locator', 'xpath', 'steps', 'image', 'input_texts', 'input_values', 'text',
-                       'coordinates', 'texts_to_verify', 'url', 'title'):
+            if key in (
+                "locator",
+                "xpath",
+                "steps",
+                "image",
+                "input_texts",
+                "input_values",
+                "text",
+                "coordinates",
+                "texts_to_verify",
+                "url",
+                "title",
+            ):
                 locator = value
                 break
         else:
             # index can be unnamed first argument or named argument
-            locator = kwargs.get('index', None)
+            locator = kwargs.get("index", None)
 
         # The only decorated method with 'locator' as NOT the first argument
         if str(function_name) == "scroll_to":
-            locator = kwargs.get('text_to_find', None)
+            locator = kwargs.get("text_to_find", None)
 
     if locator is None:
         logger.console(f"args: {args}, \nkwargs: {kwargs}")
         raise QWebElementNotFoundError("Use \\= instead of = in xpaths")
     return tuple(args), kwargs, locator
```

### Comparing `QWeb-3.2.1/QWeb/internal/download.py` & `QWeb-3.3.0/QWeb/internal/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
     Returns
     -------
     str
         Downloads directory's path.
     """
     home_dir = platform.get_home_dir()
-    download_dir = Path(home_dir) / 'Downloads'
-    logger.debug('Downloads directory is {}'.format(download_dir))
+    download_dir = Path(home_dir) / "Downloads"
+    logger.debug("Downloads directory is {}".format(download_dir))
     return str(download_dir)
 
 
 def get_modified_files(directory: str, epoch: float) -> list[str]:
     """Get modified files in directory that were modified after given epoch.
 
     Parameters
@@ -68,26 +68,25 @@
         return []
     for filename in filenamelist:
         filepath = os.path.join(directory, filename)
         if os.path.isfile(filepath):
             modification_epoch = os.path.getmtime(filepath)
             if modification_epoch > epoch:
                 modified_files.append(filepath)
-    epoch_str = time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(epoch))
-    logger.debug('Files that were altered after {} were {}'.format(epoch_str, modified_files))
+    epoch_str = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(epoch))
+    logger.debug("Files that were altered after {} were {}".format(epoch_str, modified_files))
     return modified_files
 
 
 def remove_win_temp(modified_files: list[str]) -> list[str]:
-    """Remove Windows temporary files from modified files list
-    """
-    exp = '.{8}-.{4}-.{4}-.{4}-.{12}\\.tmp'
+    """Remove Windows temporary files from modified files list"""
+    exp = ".{8}-.{4}-.{4}-.{4}-.{12}\\.tmp"
     for f in modified_files:
         if len(re.findall(exp, f)) == 1:
-            logger.debug('Removing Windows temp file: {}'.format(f))
+            logger.debug("Removing Windows temp file: {}".format(f))
             modified_files.remove(f)
     return modified_files
 
 
 def is_tmp_file(filepath: str) -> bool:
     """Is downloaded file a temporary file.
 
@@ -101,50 +100,52 @@
 
     Returns
     -------
     bool
     """
     driver = browser.get_current_browser()
     if isinstance(driver, webdriver.Chrome):
-        partial_download_suffix = 'crdownload'
+        partial_download_suffix = "crdownload"
     elif isinstance(driver, webdriver.Firefox):
-        partial_download_suffix = '.part'
+        partial_download_suffix = ".part"
     elif isinstance(driver, webdriver.Edge):
-        partial_download_suffix = 'crdownload'
+        partial_download_suffix = "crdownload"
     else:
-        raise ValueError('Unknown browser {}'.format(driver.name))
+        raise ValueError("Unknown browser {}".format(driver.name))
     return filepath.endswith(partial_download_suffix)
 
 
 def get_path(filename: str) -> Path:
     if Path(filename).exists():
         return Path(filename)
-    files = Path(BuiltIn().get_variable_value('${SUITE SOURCE}')).parent.parent / 'files' / filename
-    images = Path(
-        BuiltIn().get_variable_value('${SUITE SOURCE}')).parent.parent / 'images' / filename
+    files = Path(BuiltIn().get_variable_value("${SUITE SOURCE}")).parent.parent / "files" / filename
+    images = (
+        Path(BuiltIn().get_variable_value("${SUITE SOURCE}")).parent.parent / "images" / filename
+    )
     downloads = Path(get_downloads_dir()) / filename
-    exec_dir = BuiltIn().get_variable_value('${EXECDIR}')
+    exec_dir = BuiltIn().get_variable_value("${EXECDIR}")
     files_exec_dir = Path(f"{get_exec_subdir(exec_dir, 'files')}/{filename}")
     images_exec_dir = Path(f"{get_exec_subdir(exec_dir, 'images')}/{filename}")
     paths = [downloads, files, images, files_exec_dir, images_exec_dir]
 
     for path in paths:
         logger.debug(f"{path=}")
         if path.exists():
             logger.debug(f"Path exists: {path}")
             return path
     try:
-        base_path = BuiltIn().get_variable_value('${base_image_path}')
+        base_path = BuiltIn().get_variable_value("${base_image_path}")
         full_path = os.path.join(base_path, "{}".format(filename.lower()))
         if not Path(full_path).exists():
             raise QWebFileNotFoundError("File not found from base image path")
         return Path(full_path)
     except (TypeError, QWebFileNotFoundError) as e:
         raise QWebFileNotFoundError(
-            'File not found from default folders. Set variable for base image path') from e
+            "File not found from default folders. Set variable for base image path"
+        ) from e
 
 
 def get_exec_subdir(base_path: str, target_dir: str) -> str:
     """Finds a "special" subdirectory under execution dir.
 
     Returns full path to special dir if found.
     Returns base_path if special dir is not found.
```

### Comparing `QWeb-3.2.1/QWeb/internal/dragdrop.py` & `QWeb-3.3.0/QWeb/internal/dragdrop.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,46 +21,53 @@
 from robot.api import logger
 from QWeb.internal.text import get_text_using_anchor
 from QWeb.internal import element, javascript, frame
 from QWeb.internal.exceptions import QWebElementNotFoundError, QWebValueError
 
 
 @frame.all_frames
-def get_draggable_element(text: str, index: Union[int, str],
-                          anchor: str) -> Union[WebElement, list[WebElement]]:
-    attribute_match = '[title^="{0}"][draggable="true"],[alt^="{0}"][draggable="true"],' \
-                      '[tooltip^="{0}"][draggable="true"],' \
-                      '[data-tooltip^="{0}"][draggable="true"],' \
-                      '[data-icon^="{0}"][draggable="true"],' \
-                      '[aria-label^="{0}"][draggable="true"],' \
-                      '[title^="{0}"][class*="draggableCell"]'.format(text)
+def get_draggable_element(
+    text: str, index: Union[int, str], anchor: str
+) -> Union[WebElement, list[WebElement]]:
+    attribute_match = (
+        '[title^="{0}"][draggable="true"],[alt^="{0}"][draggable="true"],'
+        '[tooltip^="{0}"][draggable="true"],'
+        '[data-tooltip^="{0}"][draggable="true"],'
+        '[data-icon^="{0}"][draggable="true"],'
+        '[aria-label^="{0}"][draggable="true"],'
+        '[title^="{0}"][class*="draggableCell"]'.format(text)
+    )
     web_elements = []
     matches: Optional[list[WebElement]] = []
     try:
         index = int(index) - 1
     except ValueError as e:
-        raise QWebValueError('Index needs to be number') from e
-    if text.startswith('xpath=') or text.startswith('//'):
+        raise QWebValueError("Index needs to be number") from e
+    if text.startswith("xpath=") or text.startswith("//"):
         web_element = element.get_unique_element_by_xpath(text, index)
         if web_element:
             return web_element
-        raise QWebElementNotFoundError('Draggable element not found by locator {}'.format(text))
+        raise QWebElementNotFoundError("Draggable element not found by locator {}".format(text))
     web_elements = javascript.execute_javascript(
-        'return document.querySelectorAll(\'{}\')'.format(attribute_match))
+        "return document.querySelectorAll('{}')".format(attribute_match)
+    )
     if web_elements:
         return web_elements[index]
     web_elements = javascript.execute_javascript(
-        'return document.querySelectorAll(\'[draggable="true"]\')')
+        "return document.querySelectorAll('[draggable=\"true\"]')"
+    )
     if web_elements:
         matches = _find_matches(web_elements, text)
         if matches:
             return matches[index]
-        if text == 'index':
-            logger.warn('Text is not matching to any draggable element. Found {} '
-                        'draggable elements. Using index..'.format(len(web_elements)))
+        if text == "index":
+            logger.warn(
+                "Text is not matching to any draggable element. Found {} "
+                "draggable elements. Using index..".format(len(web_elements))
+            )
             return web_elements[index]
     return get_text_using_anchor(text, anchor)
 
 
 def _find_matches(web_elements: list[WebElement], text: str) -> Optional[list[WebElement]]:
     matches = []
     for elem in web_elements:
```

### Comparing `QWeb-3.2.1/QWeb/internal/dropdown.py` & `QWeb-3.3.0/QWeb/internal/dropdown.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,169 +1,178 @@
-# -*- coding: utf-8 -*-
-# --------------------------
-# Copyright © 2014 -            Qentinel Group.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ---------------------------
-
-from __future__ import annotations
-from typing import Union, Any, Optional
-from robot.api import logger
-from selenium.webdriver.remote.webelement import WebElement
-from selenium.webdriver.support.ui import Select
-from QWeb.internal.exceptions import QWebElementNotFoundError, QWebInstanceDoesNotExistError
-from QWeb.internal import text, element, javascript, util
-from QWeb.internal.table import Table
-from QWeb.internal.config_defaults import CONFIG
-
-
-def get_dropdown_element_by_locator(locator: str, anchor: str) -> WebElement:
-    """Find dropdown element.
-
-    Parameters
-    ----------
-    locator : str
-        Text that locates the input field. The input field that is closest
-        to the text is selected. Also one can use xpath by adding xpath= prefix
-        and then the xpath. Error is raised if the xpath matches to multiple
-        elements.
-    anchor : str
-        Text near the input field's locator element. If the page contains
-        many places where the locator is then anchor is used to get the
-        one that is closest to it.
-    """
-    if locator.startswith("xpath=") or locator.startswith("//"):
-        index = util.anchor_to_index(anchor)
-        dropdown_element = element.get_unique_element_by_xpath(locator, index=index)
-    else:  # Search using text
-        # First we look through all select elements' options, matching locator
-        matches = []
-        elements = _get_all_dropdown_elements()
-
-        shadow_dom = CONFIG['ShadowDOM']
-        if shadow_dom:
-            shadow_dropdowns = element.get_all_dropdowns_from_shadow_dom()
-            #  remove duplicates (normal search and including shadow search)
-            elements = util.remove_duplicates_from_list(shadow_dropdowns, elements)
-
-        for dd_element in elements:
-            options = [x.text for x in Select(dd_element).options]
-            if locator in options:
-                logger.debug("Found dropdown with options %s" % options)
-                matches.append(dd_element)
-        if matches:
-            correct_element = text.get_element_using_anchor(matches, anchor)
-            return correct_element
-
-        # Then we try to find the element using attributes and text
-        dropdown_xpath = (
-            #  pylint: disable=line-too-long
-            '//select[normalize-space(@placeholder)="{0}" or normalize-space(@value)="{0}" or  normalize-space(text())="{0}"]'
-            .format(locator))
-        dropdown_elements = element.get_webelements_in_active_area(dropdown_xpath)
-        if len(dropdown_elements) == 1:
-            dropdown_element = dropdown_elements[0]
-        elif not dropdown_elements:  # Find dropdown element using locator
-            locator_element = text.get_text_using_anchor(locator, anchor)
-            dropdown_elements = _get_all_dropdown_elements(stay_in_current_frame=True)
-            shadow_dom = CONFIG['ShadowDOM']
-            if shadow_dom:
-                shadow_dropdowns = element.get_all_dropdowns_from_shadow_dom()
-                #  remove duplicates (normal search and including shadow search)
-                dropdown_elements = util.remove_duplicates_from_list(shadow_dropdowns,
-                                                                     dropdown_elements)
-            dropdown_element = element.get_closest_element(locator_element, dropdown_elements)
-        else:  # Found many
-            logger.debug("found many, using anchor")
-            dropdown_element = text.get_element_using_anchor(dropdown_elements, anchor)
-    return dropdown_element
-
-
-def get_dd_elements_from_all_documents(locator: str, anchor: str, index: Union[int, str],
-                                       **kwargs: Any) -> Select:
-    select: Optional[WebElement]
-    if int(index) > 0:
-        index = int(index) - 1
-    css_selector = CONFIG["CssSelectors"]
-    if not css_selector or locator.startswith('xpath=') or locator.startswith('//'):
-        select = get_dropdown_element_by_locator(locator, anchor)
-    elif Table.is_table_coordinates(locator):
-        table = Table.ACTIVE_TABLE.update_table()
-        if table is None:
-            raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
-        web_element = table.get_table_cell(locator, anchor)
-        select = element.get_element_from_childnodes(web_element, 'select',
-                                                     dom_traversing=False)[int(index)]
-    else:
-        select = get_dropdown_element_by_css_selector(locator, anchor, int(index), **kwargs)
-    if not select:
-        select = get_dropdown_element_by_locator(locator, anchor)
-    if select:
-        if CONFIG['SearchMode']:
-            element.draw_borders(select)
-        return Select(select)
-    raise QWebElementNotFoundError('No matching elements found')
-
-
-def get_dropdown_element_by_css_selector(locator: str, anchor: str, index: int,
-                                         **kwargs: Any) -> Optional[WebElement]:
-    """Get Dropdown element using css selectors.
-       Parameters
-       ----------
-       locator : str
-           Label text or attribute that points to the dropdown.
-           Looking for placeholder and commonly used tooltip-attributes first.
-           If locator is label text, finds input element by it's for attribute.
-           if for attribute is not available, then finds element by doing some
-           DOM traversing.
-       anchor : str
-           Using if locator is not an XPath.
-       index : int
-           If multiple elements use index to pick correct one.
-       Returns
-       -------
-       WebElement
-   """
-    dropdown_elements = []
-    partial_matches: list[WebElement] = []
-    css = 'select'
-    if 'qweb_old' not in kwargs:
-        full_matches, partial_matches = element.get_elements_by_css(locator, css, **kwargs)
-        if full_matches:
-            if index != 0:
-                try:
-                    return full_matches[index]
-                except IndexError as e:
-                    raise QWebInstanceDoesNotExistError(
-                        f'Found {len(full_matches)} elements. Given index was {index}') from e
-            correct_element = text.get_element_using_anchor(full_matches, anchor)
-            return correct_element
-    try:
-        locator_element = text.get_text_using_anchor(locator, anchor)
-        # if this is option, return parent select immediately
-        if locator_element.tag_name.lower() == "option":
-            return javascript.execute_javascript("return arguments[0].parentNode;", locator_element)
-        dropdown_elements = list(
-            dict.fromkeys(
-                element.get_element_from_childnodes(locator_element, css, **kwargs)
-                + partial_matches))
-    except QWebElementNotFoundError:
-        logger.trace('Element not found by visible text. Trying with partial match')
-        dropdown_elements = partial_matches
-    if dropdown_elements:
-        return dropdown_elements[index]
-    return None
-
-
-def _get_all_dropdown_elements(**kwargs: Any) -> list[WebElement]:
-    dropdown_elements = element.get_webelements('//select', **kwargs)
-    return dropdown_elements
+# -*- coding: utf-8 -*-
+# --------------------------
+# Copyright © 2014 -            Qentinel Group.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ---------------------------
+
+from __future__ import annotations
+from typing import Union, Any, Optional
+from robot.api import logger
+from selenium.webdriver.remote.webelement import WebElement
+from selenium.webdriver.support.ui import Select
+from QWeb.internal.exceptions import QWebElementNotFoundError, QWebInstanceDoesNotExistError
+from QWeb.internal import text, element, javascript, util
+from QWeb.internal.table import Table
+from QWeb.internal.config_defaults import CONFIG
+
+
+def get_dropdown_element_by_locator(locator: str, anchor: str) -> WebElement:
+    """Find dropdown element.
+
+    Parameters
+    ----------
+    locator : str
+        Text that locates the input field. The input field that is closest
+        to the text is selected. Also one can use xpath by adding xpath= prefix
+        and then the xpath. Error is raised if the xpath matches to multiple
+        elements.
+    anchor : str
+        Text near the input field's locator element. If the page contains
+        many places where the locator is then anchor is used to get the
+        one that is closest to it.
+    """
+    if locator.startswith("xpath=") or locator.startswith("//"):
+        index = util.anchor_to_index(anchor)
+        dropdown_element = element.get_unique_element_by_xpath(locator, index=index)
+    else:  # Search using text
+        # First we look through all select elements' options, matching locator
+        matches = []
+        elements = _get_all_dropdown_elements()
+
+        shadow_dom = CONFIG["ShadowDOM"]
+        if shadow_dom:
+            shadow_dropdowns = element.get_all_dropdowns_from_shadow_dom()
+            #  remove duplicates (normal search and including shadow search)
+            elements = util.remove_duplicates_from_list(shadow_dropdowns, elements)
+
+        for dd_element in elements:
+            options = [x.text for x in Select(dd_element).options]
+            if locator in options:
+                logger.debug("Found dropdown with options %s" % options)
+                matches.append(dd_element)
+        if matches:
+            correct_element = text.get_element_using_anchor(matches, anchor)
+            return correct_element
+
+        # Then we try to find the element using attributes and text
+        dropdown_xpath = (
+            #  pylint: disable=line-too-long
+            '//select[normalize-space(@placeholder)="{0}" or normalize-space(@value)="{0}" or  normalize-space(text())="{0}"]'.format(
+                locator
+            )
+        )
+        dropdown_elements = element.get_webelements_in_active_area(dropdown_xpath)
+        if len(dropdown_elements) == 1:
+            dropdown_element = dropdown_elements[0]
+        elif not dropdown_elements:  # Find dropdown element using locator
+            locator_element = text.get_text_using_anchor(locator, anchor)
+            dropdown_elements = _get_all_dropdown_elements(stay_in_current_frame=True)
+            shadow_dom = CONFIG["ShadowDOM"]
+            if shadow_dom:
+                shadow_dropdowns = element.get_all_dropdowns_from_shadow_dom()
+                #  remove duplicates (normal search and including shadow search)
+                dropdown_elements = util.remove_duplicates_from_list(
+                    shadow_dropdowns, dropdown_elements
+                )
+            dropdown_element = element.get_closest_element(locator_element, dropdown_elements)
+        else:  # Found many
+            logger.debug("found many, using anchor")
+            dropdown_element = text.get_element_using_anchor(dropdown_elements, anchor)
+    return dropdown_element
+
+
+def get_dd_elements_from_all_documents(
+    locator: str, anchor: str, index: Union[int, str], **kwargs: Any
+) -> Select:
+    select: Optional[WebElement]
+    if int(index) > 0:
+        index = int(index) - 1
+    css_selector = CONFIG["CssSelectors"]
+    if not css_selector or locator.startswith("xpath=") or locator.startswith("//"):
+        select = get_dropdown_element_by_locator(locator, anchor)
+    elif Table.is_table_coordinates(locator):
+        table = Table.ACTIVE_TABLE.update_table()
+        if table is None:
+            raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
+        web_element = table.get_table_cell(locator, anchor)
+        select = element.get_element_from_childnodes(web_element, "select", dom_traversing=False)[
+            int(index)
+        ]
+    else:
+        select = get_dropdown_element_by_css_selector(locator, anchor, int(index), **kwargs)
+    if not select:
+        select = get_dropdown_element_by_locator(locator, anchor)
+    if select:
+        if CONFIG["SearchMode"]:
+            element.draw_borders(select)
+        return Select(select)
+    raise QWebElementNotFoundError("No matching elements found")
+
+
+def get_dropdown_element_by_css_selector(
+    locator: str, anchor: str, index: int, **kwargs: Any
+) -> Optional[WebElement]:
+    """Get Dropdown element using css selectors.
+    Parameters
+    ----------
+    locator : str
+        Label text or attribute that points to the dropdown.
+        Looking for placeholder and commonly used tooltip-attributes first.
+        If locator is label text, finds input element by it's for attribute.
+        if for attribute is not available, then finds element by doing some
+        DOM traversing.
+    anchor : str
+        Using if locator is not an XPath.
+    index : int
+        If multiple elements use index to pick correct one.
+    Returns
+    -------
+    WebElement
+    """
+    dropdown_elements = []
+    partial_matches: list[WebElement] = []
+    css = "select"
+    if "qweb_old" not in kwargs:
+        full_matches, partial_matches = element.get_elements_by_css(locator, css, **kwargs)
+        if full_matches:
+            if index != 0:
+                try:
+                    return full_matches[index]
+                except IndexError as e:
+                    raise QWebInstanceDoesNotExistError(
+                        f"Found {len(full_matches)} elements. Given index was {index}"
+                    ) from e
+            correct_element = text.get_element_using_anchor(full_matches, anchor)
+            return correct_element
+    try:
+        locator_element = text.get_text_using_anchor(locator, anchor)
+        # if this is option, return parent select immediately
+        if locator_element.tag_name.lower() == "option":
+            return javascript.execute_javascript("return arguments[0].parentNode;", locator_element)
+        dropdown_elements = list(
+            dict.fromkeys(
+                element.get_element_from_childnodes(locator_element, css, **kwargs)
+                + partial_matches
+            )
+        )
+    except QWebElementNotFoundError:
+        logger.trace("Element not found by visible text. Trying with partial match")
+        dropdown_elements = partial_matches
+    if dropdown_elements:
+        return dropdown_elements[index]
+    return None
+
+
+def _get_all_dropdown_elements(**kwargs: Any) -> list[WebElement]:
+    dropdown_elements = element.get_webelements("//select", **kwargs)
+    return dropdown_elements
```

### Comparing `QWeb-3.2.1/QWeb/internal/element.py` & `QWeb-3.3.0/QWeb/internal/element.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,29 @@
 from __future__ import annotations
 from typing import Optional, Callable, Any, Union
 
 import math
 from robot.api import logger
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.common.by import By
-from selenium.common.exceptions import NoSuchElementException, \
-    StaleElementReferenceException, JavascriptException, InvalidSelectorException, \
-    WebDriverException, NoSuchFrameException
+from selenium.common.exceptions import (
+    NoSuchElementException,
+    StaleElementReferenceException,
+    JavascriptException,
+    InvalidSelectorException,
+    WebDriverException,
+    NoSuchFrameException,
+)
 from QWeb.internal import frame
-from QWeb.internal.exceptions import QWebElementNotFoundError, QWebStalingElementError, \
-    QWebValueError, QWebSearchingMode
+from QWeb.internal.exceptions import (
+    QWebElementNotFoundError,
+    QWebStalingElementError,
+    QWebValueError,
+    QWebSearchingMode,
+)
 from QWeb.internal import browser, javascript, util
 from QWeb.internal.config_defaults import CONFIG
 
 ACTIVE_AREA_FUNCTION: Optional[Callable[..., Any]] = None
 DEFAULT_DISTANCE = 1000000.0  # Just some large number
 
 
@@ -44,15 +53,15 @@
     ----------
     element : WebElement
 
     Returns
     -------
     bool
     """
-    disabled = element.get_attribute('disabled')
+    disabled = element.get_attribute("disabled")
     return not bool(disabled)
 
 
 def is_readonly(element: WebElement) -> bool:
     """Is the element interactable?
 
     Uses the readonly attribute to determine if form element is enabled or
@@ -63,15 +72,16 @@
     element : WebElement
 
     Returns
     -------
     bool
     """
     return util.par2bool(
-        javascript.execute_javascript('return arguments[0].hasAttribute("readonly")', element))
+        javascript.execute_javascript('return arguments[0].hasAttribute("readonly")', element)
+    )
 
 
 def is_visible(element: WebElement) -> bool:
     """Is the element interactable?
 
     Uses the display attribute to determine if form element is visible or
     not.
@@ -80,40 +90,41 @@
     ----------
     element : WebElement
 
     Returns
     -------
     bool
     """
-    visibility = javascript.execute_javascript('return arguments[0].style.display', element)
-    return bool(visibility.lower() != 'none')
+    visibility = javascript.execute_javascript("return arguments[0].style.display", element)
+    return bool(visibility.lower() != "none")
 
 
-def get_closest_element(locator_element: WebElement,
-                        candidate_elements: list[WebElement]) -> WebElement:
+def get_closest_element(
+    locator_element: WebElement, candidate_elements: list[WebElement]
+) -> WebElement:
     """Get the closest element in a list of elements to a wanted element.
 
     Parameters
     ----------
     locator_element : WebElement
     candidate_elements : :obj:`list` of :obj:`WebElement`
 
     Returns
     -------
     WebElement
     """
     if not candidate_elements:
-        raise QWebElementNotFoundError('No elements visible')
+        raise QWebElementNotFoundError("No elements visible")
     closest_element_list = []
     closest_distance = DEFAULT_DISTANCE
     for candidate_element in candidate_elements:
         element_info = _list_info(candidate_element)
         logger.debug("Measuring distance for: {}".format(element_info))
         if _overlap(locator_element, candidate_element):
-            logger.debug('Elements overlap, returning this: {}'.format(element_info))
+            logger.debug("Elements overlap, returning this: {}".format(element_info))
             return candidate_element
         distance = _calculate_closest_distance(locator_element, candidate_element)
         logger.debug("Candidate {}: distance: {}".format(candidate_element, distance))
 
         if abs(distance - closest_distance) < 2:
             closest_element_list.append(candidate_element)
             closest_distance = distance
@@ -130,17 +141,17 @@
     closest_element = _get_closest_ortho_element(locator_element, closest_element_list)
 
     logger.debug(f"Closest distance found is {closest_distance}")
     logger.debug(f"Closest element is: {_list_info(closest_element)}")
     return closest_element
 
 
-def get_unique_element_by_xpath(xpath: str,
-                                index: Union[str, int] = 0,
-                                **kwargs: Any) -> WebElement:
+def get_unique_element_by_xpath(
+    xpath: str, index: Union[str, int] = 0, **kwargs: Any
+) -> WebElement:
     """Get element if it is needed to be unique.
 
     One use case is that when xpath is written in the test script with
     the prefix xpath=.
 
     Parameters
     ----------
@@ -154,21 +165,22 @@
     try:
         index = int(index)
     except ValueError:
         index = 0
     elements = get_webelements_in_active_area(xpath, **kwargs)
     # pylint: disable=no-else-return
     if elements and len(elements) > index:
-        if CONFIG['SearchMode']:
+        if CONFIG["SearchMode"]:
             draw_borders(elements[index])
         return elements[index]
     elif not elements:
-        raise QWebElementNotFoundError('XPath {} did not find any elements'.format(xpath))
-    raise QWebValueError(f'XPath {xpath} matched {len(elements)} elements.'
-                         f'Used index was {index+1}')
+        raise QWebElementNotFoundError("XPath {} did not find any elements".format(xpath))
+    raise QWebValueError(
+        f"XPath {xpath} matched {len(elements)} elements." f"Used index was {index+1}"
+    )
 
 
 @frame.all_frames
 def get_webelements(xpath: str, **kwargs: Any) -> list[WebElement]:
     """Get visible web elements that correspond to given XPath.
 
     To check that element is visible it is checked that it has width. This
@@ -211,27 +223,28 @@
         CSS selector to find the element.
 
     Returns
     -------
     :obj:`list` of :obj:`WebElement`
         List of visible WebElements.
     """
-    index = kwargs.get('index', 1)
+    index = kwargs.get("index", 1)
     driver = browser.get_current_browser()
     web_elements = driver.find_elements(By.CSS_SELECTOR, css)
     logger.debug("CSS selector {} matched {} WebElements".format(css, len(web_elements)))
     web_elements = get_visible_elements_from_elements(web_elements, **kwargs)
 
     index = int(index) - 1
     if len(web_elements) >= 1:
         try:
             return web_elements[index]
         except IndexError as ie:
             raise QWebValueError(
-                f'Used index {index} was greater than amount of found elements.') from ie
+                f"Used index {index} was greater than amount of found elements."
+            ) from ie
 
     return web_elements
 
 
 @frame.all_frames
 def get_webelements_in_active_area(xpath: str, **kwargs: Any) -> Optional[list[WebElement]]:
     """Find element under another element.
@@ -249,105 +262,111 @@
     :obj:`list` of :obj:`WebElement`
         List of visible WebElements.
     """
     active_area_xpath = CONFIG["ActiveAreaXpath"]
     if ACTIVE_AREA_FUNCTION is not None:
         active_area = ACTIVE_AREA_FUNCTION()  # pylint:disable=E1102
         if active_area:
-            xpath = xpath.replace('//', './/', 1)
+            xpath = xpath.replace("//", ".//", 1)
         else:
             driver = browser.get_current_browser()
             active_area = driver.find_element(By.XPATH, active_area_xpath)
     else:
         driver = browser.get_current_browser()
         try:
             active_area = driver.find_element(By.XPATH, active_area_xpath)
             if active_area is None:
-                logger.debug('Got None for active area. Is page still loading '
-                             'or is it missing body tag?')
+                logger.debug(
+                    "Got None for active area. Is page still loading  or is it missing body tag?"
+                )
                 return None
         # //body not found, is page still loading? Return None to continue looping
         except NoSuchElementException:
             logger.debug("Cannot locate //body element. Is page still loading?")
             return None
 
     try:
         webelements = active_area.find_elements(By.XPATH, xpath)
 
-        logger.trace('XPath {} matched {} webelements'.format(xpath, len(webelements)))
+        logger.trace("XPath {} matched {} webelements".format(xpath, len(webelements)))
         webelements = get_visible_elements_from_elements(webelements, **kwargs)
     except StaleElementReferenceException as se:
-        raise QWebStalingElementError('Got StaleElementException') from se
+        raise QWebStalingElementError("Got StaleElementException") from se
     except (JavascriptException, InvalidSelectorException) as e:
-        logger.debug('Got {}, returning None'.format(e))
+        logger.debug("Got {}, returning None".format(e))
         webelements = None
     return webelements
 
 
-def get_visible_elements_from_elements(web_elements: list[WebElement],
-                                       **kwargs: Any) -> list[WebElement]:
+def get_visible_elements_from_elements(
+    web_elements: list[WebElement], **kwargs: Any
+) -> list[WebElement]:
     visible_elements = []
     hiding_elements = []
-    vis_check = util.par2bool(kwargs.get('visibility', CONFIG['Visibility']))
+    vis_check = util.par2bool(kwargs.get("visibility", CONFIG["Visibility"]))
     if not vis_check:
-        logger.debug('allow invisible elements')
+        logger.debug("allow invisible elements")
         return web_elements
-    viewport_check = util.par2bool(kwargs.get('viewport', CONFIG['InViewport']))
+    viewport_check = util.par2bool(kwargs.get("viewport", CONFIG["InViewport"]))
     try:
         elem_objects = javascript.get_visibility(web_elements)
-        logger.debug('Checking visibility from all found elements: {}'.format(len(elem_objects)))
+        logger.debug("Checking visibility from all found elements: {}".format(len(elem_objects)))
     except (JavascriptException, StaleElementReferenceException, TypeError) as e:
         raise QWebStalingElementError("Exception from visibility check: {}".format(e)) from e
     for el in elem_objects:
-        onscreen = el.get('viewport')
-        logger.debug('Is element in viewport: {}'.format(onscreen))
-        css_visibility = el.get('css')
-        logger.debug('CSS visibility is not hidden and '
-                     'display is not none: {}'.format(css_visibility))
-        offset = el.get('offset')
-        logger.debug('Element offsetWidth is > 0: {}'.format(offset))
+        onscreen = el.get("viewport")
+        logger.debug("Is element in viewport: {}".format(onscreen))
+        css_visibility = el.get("css")
+        logger.debug(
+            "CSS visibility is not hidden and " "display is not none: {}".format(css_visibility)
+        )
+        offset = el.get("offset")
+        logger.debug("Element offsetWidth is > 0: {}".format(offset))
         if css_visibility and onscreen:
-            if util.par2bool(kwargs.get('offset', CONFIG['OffsetCheck'])):
+            if util.par2bool(kwargs.get("offset", CONFIG["OffsetCheck"])):
                 if offset and onscreen:
-                    visible_elements.append(el.get('elem'))
+                    visible_elements.append(el.get("elem"))
                 elif offset:
-                    hiding_elements.append(el.get('elem'))
+                    hiding_elements.append(el.get("elem"))
             elif onscreen:
-                visible_elements.append(el.get('elem'))
+                visible_elements.append(el.get("elem"))
             else:
-                hiding_elements.append(el.get('elem'))
+                hiding_elements.append(el.get("elem"))
         elif css_visibility:
-            hiding_elements.append(el.get('elem'))
-    logger.debug('found {} visible elements and {} hiding ones'.format(
-        len(visible_elements), len(hiding_elements)))
+            hiding_elements.append(el.get("elem"))
+    logger.debug(
+        "found {} visible elements and {} hiding ones".format(
+            len(visible_elements), len(hiding_elements)
+        )
+    )
     if viewport_check:
         return visible_elements  # type: ignore
     return visible_elements + hiding_elements  # type: ignore
 
 
 def get_all_inputs_from_shadow_dom() -> list[WebElement]:
     return javascript.get_all_input_elements_from_shadow_dom()
 
 
 def get_all_dropdowns_from_shadow_dom() -> list[WebElement]:
     return javascript.get_all_dropdown_elements_from_shadow_dom()
 
 
 def draw_borders(elements: Union[WebElement, list[WebElement]]) -> None:
-    mode = CONFIG['SearchMode']
-    color = CONFIG['HighlightColor']
+    mode = CONFIG["SearchMode"]
+    color = CONFIG["HighlightColor"]
     if not isinstance(elements, list):
         elements = [elements]
     for e in elements:
-        if mode.lower() == 'debug':
+        if mode.lower() == "debug":
             javascript.highlight_element(e, False, color=color)
-            raise QWebSearchingMode('Element highlighted')
-        if mode.lower() == 'draw':
+            raise QWebSearchingMode("Element highlighted")
+        if mode.lower() == "draw":
             javascript.highlight_element(e, True, color=color)
-        elif mode.lower() == 'flash':
+        elif mode.lower() == "flash":
             javascript.highlight_element(e, False, True, color=color)
 
 
 def _calculate_closest_distance(element1: WebElement, element2: WebElement) -> float:
     """Calculate closest distance between elements in pixel units.
 
     Gets corners' locations for both elements and use them to calculate the
@@ -366,40 +385,45 @@
     """
     search_direction = CONFIG["SearchDirection"]
     corners_locations1 = _get_corners_locations(element1)
     corners_locations2 = _get_corners_locations(element2)
     closest_distance = DEFAULT_DISTANCE
     for corner1 in corners_locations1:
         for corner2 in corners_locations2:
-            distance = _manhattan_distance(corner1['x'], corner1['y'], corner2['x'], corner2['y'])
-            if search_direction != 'closest':
+            distance = _manhattan_distance(corner1["x"], corner1["y"], corner2["x"], corner2["y"])
+            if search_direction != "closest":
                 # y coordinate goes up downwards on page
                 # small y is above
                 angle = math.degrees(
-                    math.atan2(corner2['y'] - corner1['y'], corner2['x'] - corner1['x']))
+                    math.atan2(corner2["y"] - corner1["y"], corner2["x"] - corner1["x"])
+                )
 
-            if search_direction in ('down', 'down!'):
+            if search_direction in ("down", "down!"):
                 if not 5 < angle < 175:
                     logger.debug(
-                        'Search direction is {} and element is not in arc'.format(search_direction))
+                        "Search direction is {} and element is not in arc".format(search_direction)
+                    )
                     distance = DEFAULT_DISTANCE
-            elif search_direction in ('up', 'up!'):
+            elif search_direction in ("up", "up!"):
                 if not -175 < angle < -5:
                     logger.debug(
-                        'Search direction is {} and element is not in arc'.format(search_direction))
+                        "Search direction is {} and element is not in arc".format(search_direction)
+                    )
                     distance = DEFAULT_DISTANCE
-            elif search_direction in ('left', 'left!'):
+            elif search_direction in ("left", "left!"):
                 if not abs(angle) > 95:
                     logger.debug(
-                        'Search direction is {} and element is not in arc'.format(search_direction))
+                        "Search direction is {} and element is not in arc".format(search_direction)
+                    )
                     distance = DEFAULT_DISTANCE
-            elif search_direction in ('right', 'right!'):
+            elif search_direction in ("right", "right!"):
                 if not -85 < angle < 85:
                     logger.debug(
-                        'Search direction is {} and element is not in arc'.format(search_direction))
+                        "Search direction is {} and element is not in arc".format(search_direction)
+                    )
                     distance = DEFAULT_DISTANCE
 
             if closest_distance > distance > 0:
                 closest_distance = distance
     return closest_distance
 
 
@@ -413,21 +437,21 @@
 
     Returns
     -------
     float
     """
     center_1 = _get_center_location(element1)
     center_2 = _get_center_location(element2)
-    distance_h = abs(center_1['x'] - center_2['x'])
-    distance_v = abs(center_1['y'] - center_2['y'])
+    distance_h = abs(center_1["x"] - center_2["x"])
+    distance_v = abs(center_1["y"] - center_2["y"])
     return min(distance_h, distance_v)
 
 
 def _get_center_location(element: WebElement) -> dict[str, float]:
-    """ Calculate rectangle's center locations
+    """Calculate rectangle's center locations
 
        Each element on a web page is in a rectangle. Uses the WebElement's
     location and size attributes to get center.
 
     Parameters
     ----------
     element : WebElement
@@ -435,20 +459,20 @@
     Returns
     -------
     tuple
         A tuple with 2 elements: center x and y coordinates.
     """
     location = element.location
     size = element.size
-    center = {'x': location['x'] + (size['width'] / 2), 'y': location['y'] + (size['height'] / 2)}
+    center = {"x": location["x"] + (size["width"] / 2), "y": location["y"] + (size["height"] / 2)}
     return center
 
 
 def _get_corners_locations(
-    element: WebElement
+    element: WebElement,
 ) -> tuple[dict[str, float], dict[str, float], dict[str, float], dict[str, float]]:
     """Calculate rectangle's corners' locations
 
     Each element on a web page is in a rectangle. Uses the WebElement's
     location and size attributes to get all corners.
 
     Parameters
@@ -459,56 +483,56 @@
     -------
     tuple
         A tuple with 4 elements: top left corner, top right corner, bottom
         left corner, bottom right corner.
     """
     location = element.location
     size = element.size
-    top_left_corner = {'x': location['x'], 'y': location['y']}
-    top_right_corner = {'x': location['x'] + size['width'], 'y': location['y']}
-    bottom_left_corner = {'x': location['x'], 'y': location['y'] + size['height']}
-    bottom_right_corner = {'x': top_right_corner['x'], 'y': bottom_left_corner['y']}
+    top_left_corner = {"x": location["x"], "y": location["y"]}
+    top_right_corner = {"x": location["x"] + size["width"], "y": location["y"]}
+    bottom_left_corner = {"x": location["x"], "y": location["y"] + size["height"]}
+    bottom_right_corner = {"x": top_right_corner["x"], "y": bottom_left_corner["y"]}
     corners_locations = (top_left_corner, top_right_corner, bottom_left_corner, bottom_right_corner)
     return corners_locations
 
 
 def _manhattan_distance(x0: float, y0: float, x1: float, y1: float) -> float:
     """Get manhattan distance between points (x0, y0) and (x1, y1)."""
     return abs(x0 - x1) + abs(y0 - y1)
 
 
 def _overlap(element1: WebElement, element2: WebElement) -> float:
-    """Detects if two rectangles overlap
-    """
+    """Detects if two rectangles overlap"""
     corners_locations1 = _get_corners_locations(element1)
     corners_locations2 = _get_corners_locations(element2)
 
     # pylint: disable=R1728
-    r1_left = min([i['x'] for i in corners_locations1])
-    r1_right = max([i['x'] for i in corners_locations1])
-    r1_top = max([i['y'] for i in corners_locations1])
-    r1_bottom = min([i['y'] for i in corners_locations1])
-
-    r2_left = min([i['x'] for i in corners_locations2])
-    r2_right = max([i['x'] for i in corners_locations2])
-    r2_top = max([i['y'] for i in corners_locations2])
-    r2_bottom = min([i['y'] for i in corners_locations2])
-
-    return _range_overlap(r1_left, r1_right, r2_left, r2_right) \
-        and _range_overlap(r1_bottom, r1_top, r2_bottom, r2_top)
+    r1_left = min([i["x"] for i in corners_locations1])
+    r1_right = max([i["x"] for i in corners_locations1])
+    r1_top = max([i["y"] for i in corners_locations1])
+    r1_bottom = min([i["y"] for i in corners_locations1])
+
+    r2_left = min([i["x"] for i in corners_locations2])
+    r2_right = max([i["x"] for i in corners_locations2])
+    r2_top = max([i["y"] for i in corners_locations2])
+    r2_bottom = min([i["y"] for i in corners_locations2])
+
+    return _range_overlap(r1_left, r1_right, r2_left, r2_right) and _range_overlap(
+        r1_bottom, r1_top, r2_bottom, r2_top
+    )
 
 
 def _range_overlap(a_min: float, a_max: float, b_min: float, b_max: float) -> float:
-    """Neither range is completely greater than the other
-    """
+    """Neither range is completely greater than the other"""
     return (a_min <= b_max) and (b_min <= a_max)
 
 
-def _get_closest_ortho_element(locator_element: WebElement,
-                               element_list: list[WebElement]) -> WebElement:
+def _get_closest_ortho_element(
+    locator_element: WebElement, element_list: list[WebElement]
+) -> WebElement:
     """Return closest element by orthogonal distance
 
     Compares all elements from a list against locator element based on their horizontal
     or vertical distance. Returns one that has shortest.
 
     Parameters
     ----------
@@ -555,197 +579,216 @@
     valid_operators.extend(GREATER_THAN_OR_EQUAL)
     valid_operators.append("contains")
     valid_operators.append("not contains")
 
     operator = operator.lower()
 
     if operator not in valid_operators:
-        raise QWebValueError(f'Incorrect operator "{operator}" given. Supported operators are:'
-                             f'"{valid_operators}"')
+        raise QWebValueError(
+            f'Incorrect operator "{operator}" given. Supported operators are:'
+            f'"{valid_operators}"'
+        )
 
     if operator in EQUALS and value != expected:
         raise QWebValueError(
-            f"Expected attribute value differs from real value: {expected}/{value}")
+            f"Expected attribute value differs from real value: {expected}/{value}"
+        )
     if operator in NOT_EQUAL and value == expected:
         raise QWebValueError(f"Expected attribute value matches real value: {expected}/{value}")
     if operator == "contains" and expected not in value:
         raise QWebValueError(f'Attribute value "{value}" does not contain: "{expected}"')
     if operator == "not contains" and expected in value:
         raise QWebValueError(f'Attribute value "{value}" contains: "{expected}"')
 
     # numeric comparison operator used but either value not numeric
     if [
-            x for x in [GREATER_THAN, LESS_THAN, LESS_THAN_OR_EQUAL, GREATER_THAN_OR_EQUAL]
-            if operator in x
+        x
+        for x in [GREATER_THAN, LESS_THAN, LESS_THAN_OR_EQUAL, GREATER_THAN_OR_EQUAL]
+        if operator in x
     ]:
         if not (value.isdigit() and expected.isdigit()):
             raise QWebValueError(f'Attribute value "{value}" is not numeric!')
 
     if operator in GREATER_THAN and int(value) <= int(expected):
         raise QWebValueError(
-            f'Attribute value: "{value}" is not greater than expected: "{expected}"')
+            f'Attribute value: "{value}" is not greater than expected: "{expected}"'
+        )
 
     if operator in LESS_THAN and int(value) >= int(expected):
         raise QWebValueError(f'Attribute value: "{value}" is greater than expected: "{expected}"')
     if operator in GREATER_THAN_OR_EQUAL and int(value) < int(expected):
         raise QWebValueError(
-            f'Attribute value: "{value}" is not greater or equal than expected: "{expected}"')
+            f'Attribute value: "{value}" is not greater or equal than expected: "{expected}"'
+        )
     if operator in LESS_THAN_OR_EQUAL and int(value) > int(expected):
         raise QWebValueError(
-            f'Attribute value: "{value}" is not less or equal than expected: "{expected}"')
+            f'Attribute value: "{value}" is not less or equal than expected: "{expected}"'
+        )
 
 
 def _list_info(candidate_element):
-    """Log element id, title or placeholder
-    """
-    outer_html = candidate_element.get_attribute('outerHTML')
-    if outer_html != '' or outer_html is not None:
+    """Log element id, title or placeholder"""
+    outer_html = candidate_element.get_attribute("outerHTML")
+    if outer_html != "" or outer_html is not None:
         return "OuterHTML: {}".format(outer_html)
     return candidate_element
 
 
 @frame.all_frames
 def get_elements_by_attributes(
-        css: str,
-        locator: Optional[str] = None,
-        **kwargs) -> Union[list[WebElement], tuple[list[WebElement], list[WebElement]]]:
-    any_element = util.par2bool(kwargs.get('any_element', None))
-    partial = util.par2bool(kwargs.get('partial_match', CONFIG['PartialMatch']))
-    if 'tag' in kwargs:
-        css = str(kwargs.get('tag'))
+    css: str, locator: Optional[str] = None, **kwargs
+) -> Union[list[WebElement], tuple[list[WebElement], list[WebElement]]]:
+    any_element = util.par2bool(kwargs.get("any_element", None))
+    partial = util.par2bool(kwargs.get("partial_match", CONFIG["PartialMatch"]))
+    if "tag" in kwargs:
+        css = str(kwargs.get("tag"))
     try:
         elements = javascript.get_all_elements(css)
         if any_element:
             return elements
         matches = javascript.get_by_attributes(
             elements,
-            locator.replace("\'", "\\'"),  # type: ignore[union-attr]
-            partial)
+            locator.replace("'", "\\'"),  # type: ignore[union-attr]
+            partial,
+        )
 
         # try with xpath if no matches
         # there have been few where css search doesn't work
         # this is supported only if tag argument is given
         if len(matches.get("full", [])) == 0 and len(matches.get("partial", [])) == 0:
             try:
                 driver = browser.get_current_browser()
-                elements = driver.find_elements(By.XPATH, f'//{css}')
+                elements = driver.find_elements(By.XPATH, f"//{css}")
 
                 matches = javascript.get_by_attributes(
                     elements,
-                    locator.replace("\'", "\\'"),  # type: ignore[union-attr]
-                    partial)
+                    locator.replace("'", "\\'"),  # type: ignore[union-attr]
+                    partial,
+                )
             except InvalidSelectorException:
-                matches = {'full': [], 'partial': []}
+                matches = {"full": [], "partial": []}
 
-        logger.debug('attrfunc found full matches: {}, partial matches: {}'.format(
-            matches.get('full', []), matches.get('partial', [])))
-        full_matches, partial_matches = matches.get('full', []), matches.get('partial', [])
+        logger.debug(
+            "attrfunc found full matches: {}, partial matches: {}".format(
+                matches.get("full", []), matches.get("partial", [])
+            )
+        )
+        full_matches, partial_matches = matches.get("full", []), matches.get("partial", [])
     except (WebDriverException, JavascriptException, AttributeError) as e:
-        logger.debug('Got exception from get elements by attributes: {}'.format(e))
+        logger.debug("Got exception from get elements by attributes: {}".format(e))
         full_matches, partial_matches = [], []
 
-    if 'element_kw' not in kwargs:
+    if "element_kw" not in kwargs:
         return full_matches, partial_matches
     web_elements = full_matches + partial_matches
 
     if web_elements:
-        if CONFIG['SearchMode']:
+        if CONFIG["SearchMode"]:
             draw_borders(web_elements)
         return web_elements
-    raise QWebElementNotFoundError('Element with {} attribute not found'.format(locator))
+    raise QWebElementNotFoundError("Element with {} attribute not found".format(locator))
 
 
 @frame.all_frames
 def get_element_by_label_for(
-        locator: str, css: str, **kwargs) -> tuple[list[WebElement], list[WebElement]]:  # pylint: disable=unused-argument
-    partial = util.par2bool(kwargs.get('partial_match', CONFIG['PartialMatch']))
-    limit = util.par2bool(kwargs.get('limit_traverse', CONFIG['LimitTraverse']))
+    locator: str, css: str, **kwargs
+) -> tuple[list[WebElement], list[WebElement]]:  # pylint: disable=unused-argument
+    partial = util.par2bool(kwargs.get("partial_match", CONFIG["PartialMatch"]))
+    limit = util.par2bool(kwargs.get("limit_traverse", CONFIG["LimitTraverse"]))
     level = 3 if limit is True else 6
     try:
-        matches = javascript.get_by_label(locator.replace("\'", "\\'"), css, level, partial)
-        logger.debug('labelfunc found full matches: {}, partial matches: {}'.format(
-            matches.get('full', []), matches.get('partial', [])))
-        return matches.get('full', []), matches.get('partial', [])
+        matches = javascript.get_by_label(locator.replace("'", "\\'"), css, level, partial)
+        logger.debug(
+            "labelfunc found full matches: {}, partial matches: {}".format(
+                matches.get("full", []), matches.get("partial", [])
+            )
+        )
+        return matches.get("full", []), matches.get("partial", [])
     except (WebDriverException, JavascriptException) as e:
-        logger.warn('Exception from label func: {}'.format(e))
+        logger.warn("Exception from label func: {}".format(e))
         return [], []
 
 
-def get_element_from_childnodes(locator_element: WebElement,
-                                css: str,
-                                dom_traversing: bool = True,
-                                **kwargs) -> list[WebElement]:
-    limit = util.par2bool(kwargs.get('limit_traverse', CONFIG['LimitTraverse']))
+def get_element_from_childnodes(
+    locator_element: WebElement, css: str, dom_traversing: bool = True, **kwargs
+) -> list[WebElement]:
+    limit = util.par2bool(kwargs.get("limit_traverse", CONFIG["LimitTraverse"]))
     level = 3 if limit is True else 6
     try:
         web_elements = get_visible_elements_from_elements(
-            javascript.get_childnodes(locator_element, css, level, dom_traversing))
+            javascript.get_childnodes(locator_element, css, level, dom_traversing)
+        )
     except (WebDriverException, JavascriptException) as e:
         web_elements = None
-        logger.debug('Got Exception from get_element_from_childnodes: {}'.format(e))
+        logger.debug("Got Exception from get_element_from_childnodes: {}".format(e))
     # if all else fails, try to find children with xpath
     if not web_elements:
         try:
             web_elements = locator_element.find_elements(By.XPATH, f".//{css}")
         except InvalidSelectorException:
             web_elements = None
     if web_elements:
         return web_elements
-    raise QWebElementNotFoundError('Child with tag {} not found.'.format(css))
+    raise QWebElementNotFoundError("Child with tag {} not found.".format(css))
 
 
-def get_elements_by_css(locator: str, css: str,
-                        **kwargs) -> tuple[list[WebElement], list[WebElement]]:
+def get_elements_by_css(
+    locator: str, css: str, **kwargs
+) -> tuple[list[WebElement], list[WebElement]]:
     try:
         f0, p0 = get_elements_by_attributes(css, locator, **kwargs)
     except NoSuchFrameException:
-        logger.debug('got no such frame exception from get elem bu attrs')
+        logger.debug("got no such frame exception from get elem bu attrs")
         f0, p0 = [], []
     if (len(f0 + p0)) > 0:
-        kwargs['stay_in_current_frame'] = True
+        kwargs["stay_in_current_frame"] = True
     try:
         f1, p1 = get_element_by_label_for(locator, css, **kwargs)
     except NoSuchFrameException:
-        logger.debug('got no such frame exception from get elem by label')
+        logger.debug("got no such frame exception from get elem by label")
         f1, p1 = [], []
     full_matches = list(dict.fromkeys(f0 + f1))
     partial_matches = list(dict.fromkeys(p0 + p1))
     return full_matches, partial_matches
 
 
 def get_parent_element(web_element: WebElement, tag: str) -> WebElement:
-    web_element = javascript.execute_javascript('return arguments[0].closest(\'{}\')'.format(tag),
-                                                web_element)
+    web_element = javascript.execute_javascript(
+        "return arguments[0].closest('{}')".format(tag), web_element
+    )
     if web_element:
         return web_element
-    raise QWebElementNotFoundError('Parent with tag {} not found.'.format(tag))
+    raise QWebElementNotFoundError("Parent with tag {} not found.".format(tag))
 
 
 def get_parent_list_element(locator_element: WebElement, css: str) -> WebElement:
     try:
         web_element = javascript.get_parent_list(locator_element, css)
     except (WebDriverException, JavascriptException) as e:
         web_element = None
-        logger.debug('Got Exception from get_parent_list: {}'.format(e))
+        logger.debug("Got Exception from get_parent_list: {}".format(e))
     if isinstance(web_element, WebElement):
         return web_element
-    raise QWebElementNotFoundError('Parent with tag {} not found.'.format(css))
+    raise QWebElementNotFoundError("Parent with tag {} not found.".format(css))
 
 
-def get_element_to_click_from_list(active_list: list[WebElement], index: int,
-                                   **kwargs) -> WebElement:
-    if 'tag' in kwargs:
+def get_element_to_click_from_list(
+    active_list: list[WebElement], index: int, **kwargs
+) -> WebElement:
+    if "tag" in kwargs:
         element = javascript.execute_javascript(
-            'return arguments[0].querySelector("{}")'.format(kwargs['tag']), active_list[index])
+            'return arguments[0].querySelector("{}")'.format(kwargs["tag"]), active_list[index]
+        )
     else:
         element = active_list[index]
     return element
 
 
 def get_element_by_index(elements: list[WebElement], index: Union[str, int]) -> WebElement:
     if str(index).isdigit():
         try:
             return elements[int(index) - 1]
         except IndexError as ie:
-            raise QWebValueError(f'Only "{len(elements)}" elements found.'
-                                 f'Used index was "{index}"') from ie
+            raise QWebValueError(
+                f'Only "{len(elements)}" elements found.' f'Used index was "{index}"'
+            ) from ie
     raise ValueError(f'Index should be numeric. Used index was: "{index}"')
```

### Comparing `QWeb-3.2.1/QWeb/internal/exceptions.py` & `QWeb-3.3.0/QWeb/internal/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 from __future__ import annotations
 
 FATAL_MESSAGES: list[str] = [
-    "Failed to decode response", "chrome not reachable", "window was already closed",
-    "Unable to get browser", "session deleted", "0 tabs open"
+    "Failed to decode response",
+    "chrome not reachable",
+    "window was already closed",
+    "Unable to get browser",
+    "session deleted",
+    "0 tabs open",
 ]
 
 
 class QWebException(Exception):
     """
     Base class for other QWebExceptions
 
@@ -71,20 +75,20 @@
 
 class QWebInvalidElementStateError(QWebDriverError):
     """Raise if element is in disabled state when trying
     to trigger keyword action."""
 
 
 class QWebValueMismatchError(QWebValueError):
-    """ Raise if real value is different than
+    """Raise if real value is different than
     expected value."""
 
 
 class QWebFileNotFoundError(QWebValueError):
-    """ Raise if reference file is missing. """
+    """Raise if reference file is missing."""
 
 
 class QWebTextNotFoundError(QWebException):
     """Raise when ScrollTo KW does not find searched text."""
 
 
 class QWebUnexpectedAlert(QWebException):
```

### Comparing `QWeb-3.2.1/QWeb/internal/frame.py` & `QWeb-3.3.0/QWeb/internal/frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,30 @@
 import time
 from functools import wraps
 from robot.api import logger
 from robot.utils import timestr_to_secs
 from robot.libraries.BuiltIn import BuiltIn
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
-from selenium.common.exceptions import NoSuchWindowException, \
-                                       StaleElementReferenceException, \
-                                       UnexpectedAlertPresentException, \
-                                       WebDriverException, InvalidSessionIdException
+from selenium.common.exceptions import (
+    NoSuchWindowException,
+    StaleElementReferenceException,
+    UnexpectedAlertPresentException,
+    WebDriverException,
+    InvalidSessionIdException,
+)
 from QWeb.keywords import config
 import QWeb.internal.frame_checker as fc
-from QWeb.internal.exceptions import QWebDriverError, QWebElementNotFoundError, \
-                                     QWebTimeoutError, QWebBrowserError, FATAL_MESSAGES
+from QWeb.internal.exceptions import (
+    QWebDriverError,
+    QWebElementNotFoundError,
+    QWebTimeoutError,
+    QWebBrowserError,
+    FATAL_MESSAGES,
+)
 from QWeb.internal import xhr, browser, util
 from QWeb.internal.config_defaults import CONFIG
 
 
 def wait_page_loaded() -> None:
     """Wait for webpage to be loaded.
 
@@ -49,37 +57,37 @@
     page has been loaded fully.
 
     Monkeypatch this method to have different wait.
     """
     if CONFIG["DefaultDocument"]:
         driver = browser.get_current_browser()
         if driver is None:
-            raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                                  " to open browser first")
+            raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
         try:
             driver.switch_to.default_content()
         except InvalidSessionIdException as ie:
             CONFIG.set_value("OSScreenshots", True)
             raise QWebBrowserError("Browser session lost. Did browser crash?") from ie
         except UnexpectedAlertPresentException as uea:
             raise uea
         except (NoSuchWindowException, WebDriverException) as e:
             logger.warn(
-                'Cannot switch to default context, maybe window is closed. Err: {}'.format(e))
+                "Cannot switch to default context, maybe window is closed. Err: {}".format(e)
+            )
             if any(s in str(e) for s in FATAL_MESSAGES):
                 CONFIG.set_value("OSScreenshots", True)
                 raise QWebBrowserError(e) from e
             driver.switch_to.default_content()
-    timeout = CONFIG['XHRTimeout']
+    timeout = CONFIG["XHRTimeout"]
     if timeout.lower() == "none":
         return
     try:
         xhr.wait_xhr(timestr_to_secs(timeout))
     except (WebDriverException, QWebDriverError) as e:
-        logger.debug(f'Unable to check AJAX requests due error: {e}')
+        logger.debug(f"Unable to check AJAX requests due error: {e}")
 
 
 def get_raw_html() -> str:
     driver = browser.get_current_browser()
     return driver.page_source
 
 
@@ -131,26 +139,28 @@
     Replace relative paths in the src and href attributes with the actual
     source. This way we get css properties and icons.
 
     Works only local log file, implement Jenkins (or some other) in the
     javascript.
     """
     filename = os.path.basename(filepath)
-    logger.info('''<tbody>
+    logger.info(
+        """<tbody>
 <a id="sourceLink{0}">{1}</a>
 <br />
 <iframe id="source{0}" width="1220px" height="650px"></iframe>
 <script type="text/javascript">
 element = document.getElementById("sourceLink{0}");
 var url = window.location.href;
 document.getElementById("sourceLink{0}").setAttribute("href", "{2}")
 document.getElementById("source{0}").setAttribute("src", "{1}")
 </script>
-</tbody>'''.format(count, filename, filepath.replace("\\", "\\\\")),
-                html=True)
+</tbody>""".format(count, filename, filepath.replace("\\", "\\\\")),
+        html=True,
+    )
 
 
 def get_output_dir() -> str:
     return str(BuiltIn().get_variable_value("${OUTPUT_DIR}"))
 
 
 def get_html_source_count() -> int:
@@ -168,121 +178,123 @@
     search_from_frames is recursive function which goes through
     all found frames until we find our element if that's not in
     main html's dom tree.
     """
 
     @wraps(fn)
     def wrapped(*args, **kwargs) -> Callable[..., Any]:
-
-        def search_from_frames(driver: Optional[WebDriver] = None,
-                               current_frame: Optional[WebElement] = None) -> Callable[..., Any]:
-            keep_frame = kwargs.get('stay_in_current_frame', CONFIG['StayInCurrentFrame'])
+        def search_from_frames(
+            driver: Optional[WebDriver] = None, current_frame: Optional[WebElement] = None
+        ) -> Callable[..., Any]:
+            keep_frame = kwargs.get("stay_in_current_frame", CONFIG["StayInCurrentFrame"])
             if keep_frame:
                 return fn(*args, **kwargs)
             err = None
             if not driver:
                 driver = browser.get_current_browser()
                 driver.switch_to.default_content()
             if current_frame:
                 try:
                     driver.switch_to.frame(current_frame)
-                    logger.debug('switching to childframe {}'.format(str(fn)))
+                    logger.debug("switching to childframe {}".format(str(fn)))
                 except (StaleElementReferenceException, WebDriverException) as e:
                     logger.debug(str(e))
                     driver.switch_to.default_content()
                     raise e
             try:
                 web_element = fn(*args, **kwargs)
             except QWebElementNotFoundError as e:
                 err = e
                 web_element = None
             if is_valid(web_element):
                 return web_element
             start = time.time()
-            timeout = CONFIG['FrameTimeout']
+            timeout = CONFIG["FrameTimeout"]
             while time.time() < timeout + start:
                 frames = fc.check_frames(driver)
                 for frame in frames:
                     web_element = search_from_frames(driver=driver, current_frame=frame)
                     if is_valid(web_element):
-                        logger.debug('Found webelement = {}'.format(web_element))
+                        logger.debug("Found webelement = {}".format(web_element))
                         return web_element
                     try:
                         driver.switch_to.parent_frame()
                     except WebDriverException as e:
                         driver.switch_to.default_content()
                         raise e
-                    config.set_config('FrameTimeout', float(timeout + start - time.time()))
-                    logger.trace('Frame timeout: {}'.format(timeout))
+                    config.set_config("FrameTimeout", float(timeout + start - time.time()))
+                    logger.trace("Frame timeout: {}".format(timeout))
                 if err:
                     raise err
                 return web_element
             driver.switch_to.default_content()
-            raise QWebTimeoutError('From frame decorator: Unable to locate element in given time')
+            raise QWebTimeoutError("From frame decorator: Unable to locate element in given time")
 
         # pylint: disable=W0102
-        def search_from_frames_safari(driver: Optional[WebDriver] = None,
-                                      current_frame: Union[Optional[WebElement], int] = None,
-                                      parent_tree: list[Union[WebElement, int]] = []):
-            keep_frame = kwargs.get('stay_in_current_frame', CONFIG['StayInCurrentFrame'])
+        def search_from_frames_safari(
+            driver: Optional[WebDriver] = None,
+            current_frame: Union[Optional[WebElement], int] = None,
+            parent_tree: list[Union[WebElement, int]] = [],
+        ):
+            keep_frame = kwargs.get("stay_in_current_frame", CONFIG["StayInCurrentFrame"])
             if keep_frame:
                 return fn(*args, **kwargs)
             err = None
             if not driver:
                 driver = browser.get_current_browser()
                 driver.switch_to.default_content()
             if current_frame is not None:
                 try:
                     driver.switch_to.frame(current_frame)
-                    logger.debug('switching to childframe {}'.format(str(fn)))
+                    logger.debug("switching to childframe {}".format(str(fn)))
                 except (StaleElementReferenceException, WebDriverException) as e:
                     logger.debug(str(e))
                     driver.switch_to.default_content()
                     raise e
             try:
                 web_element = fn(*args, **kwargs)
             except QWebElementNotFoundError as e:
                 err = e
                 web_element = None
             if is_valid(web_element):
                 return web_element
             start = time.time()
-            timeout = CONFIG['FrameTimeout']
+            timeout = CONFIG["FrameTimeout"]
             while time.time() < timeout + start:
                 frames = fc.check_frames(driver)
                 for count, frame in enumerate(frames):  # pylint: disable=W0612
                     parent_tree.append(count)
                     # using count instead of frame reference due to Safari bug
-                    web_element = search_from_frames_safari(driver=driver,
-                                                            current_frame=count,
-                                                            parent_tree=parent_tree)
+                    web_element = search_from_frames_safari(
+                        driver=driver, current_frame=count, parent_tree=parent_tree
+                    )
                     if is_valid(web_element):
-                        logger.debug('Found webelement = {}'.format(web_element))
+                        logger.debug("Found webelement = {}".format(web_element))
                         return web_element
                     try:
                         # switch_to.parent_frame not working in Safari
                         # doing moving to previuos frame "manually"
                         parent_tree.pop()
                         driver.switch_to.default_content()
                         for f in parent_tree:
                             driver.switch_to.frame(f)
                     except WebDriverException as e:
                         driver.switch_to.default_content()
                         raise e
-                    config.set_config('FrameTimeout', float(timeout + start - time.time()))
-                    logger.trace('Frame timeout: {}'.format(timeout))
+                    config.set_config("FrameTimeout", float(timeout + start - time.time()))
+                    logger.trace("Frame timeout: {}".format(timeout))
                 if err:
                     raise err
                 return web_element
             driver.switch_to.default_content()
-            raise QWebTimeoutError('From frame decorator: Unable to locate element in given time')
+            raise QWebTimeoutError("From frame decorator: Unable to locate element in given time")
 
         return search_from_frames_safari() if util.is_safari() else search_from_frames()
 
-    logger.debug('wrapped = {}'.format(wrapped))
+    logger.debug("wrapped = {}".format(wrapped))
     return wrapped
 
 
 def is_valid(web_element: Union[WebElement, tuple]) -> bool:
     if web_element and not isinstance(web_element, tuple):
         return True
     if isinstance(web_element, tuple) and any(web_element):
```

### Comparing `QWeb-3.2.1/QWeb/internal/frame_checker.py` & `QWeb-3.3.0/QWeb/internal/frame_checker.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
 def check_frames(driver: WebDriver, **kwargs) -> list[WebElement]:
     visible_frames: list[WebElement] = []
     frames = javascript.execute_javascript('return document.querySelectorAll("iframe, frame")')
     if not frames:
         frames = []
     frames += driver.find_elements(By.XPATH, "//iframe|//frame")
-    shadow_dom = CONFIG['ShadowDOM']
+    shadow_dom = CONFIG["ShadowDOM"]
     if shadow_dom:
         frames = javascript.get_all_frames_from_shadow_dom()
-    visible_only = kwargs.get('visibility', True)
+    visible_only = kwargs.get("visibility", True)
     if not visible_only:
         return frames
     frames_obj = javascript.get_visibility(list(dict.fromkeys(frames)))
     if not frames_obj:
         return frames
     for frame in frames_obj:
-        offset = frame.get('offset')
+        offset = frame.get("offset")
         if offset:
-            visible_frames.append(frame.get('elem'))  # type: ignore
+            visible_frames.append(frame.get("elem"))  # type: ignore
     if visible_frames:
-        logger.debug('Found {} visible frames'.format(len(visible_frames)))
+        logger.debug("Found {} visible frames".format(len(visible_frames)))
     return visible_frames
```

### Comparing `QWeb-3.2.1/QWeb/internal/icon.py` & `QWeb-3.3.0/QWeb/internal/icon.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,27 +78,26 @@
             1.50,
             1.25,
             1.75,
         ]
 
         if device_res_w <= 0 or template_res_w <= 0:
             raise ValueError(
-                "Device resolution {} or template resolution {}"
-                " can't be zero or less".format(device_res_w, template_res_w)
+                "Device resolution {} or template resolution {}" " can't be zero or less".format(
+                    device_res_w, template_res_w
+                )
             )
 
-        if not round(device_res_w / template_res_w, 2) in scale_ratios:
+        if round(device_res_w / template_res_w, 2) not in scale_ratios:
             scale_ratios.insert(0, round(device_res_w / template_res_w, 2))
 
         return scale_ratios
 
     @staticmethod
-    def _get_image_pyramid(
-        image_obj: ndarray, level: int
-    ) -> list[tuple[ndarray, float]]:
+    def _get_image_pyramid(image_obj: ndarray, level: int) -> list[tuple[ndarray, float]]:
         """
         Returns a list of up- and downsampled images of image_obj.
         Each sampling goes 10% up and down in size
         image_obj = Image as uint8 NumPy array in RGB color space.
         level = Image pyramid size - how many times the image is up- and downsampled.
         """
         print("*INFO* Start _get_image_pyramid")
@@ -174,22 +173,16 @@
             # pylint: disable=no-member
         color_template = template
         if isinstance(template, np.ndarray) and len(template.shape) > 2:
             template = cv2.cvtColor(template, cv2.COLOR_BGR2GRAY)
         width, height = self._get_image_size(template)
         img_width, img_height = self._get_image_size(image_obj)
 
-        print(
-            "*DEBUG* source haystack (image_obj) image size: {}x{}".format(
-                img_width, img_height
-            )
-        )
-        print(
-            "*DEBUG* original needle (template) image size: {}x{}".format(width, height)
-        )
+        print("*DEBUG* source haystack (image_obj) image size: {}x{}".format(img_width, img_height))
+        print("*DEBUG* original needle (template) image size: {}x{}".format(width, height))
 
         if height > img_height or width > img_width:
             raise ValueError(
                 "Image Size Error: Template image is larger than source image. "
                 "Template size: {}x{}, source image size: {}x{}.".format(
                     width, height, img_width, img_height
                 )
@@ -223,17 +216,15 @@
         for template_level in template_levels:
             w, h = self._get_image_size(template_level[0])
             print(
                 "*DEBUG* Resampled needle (template_level) with scale {}, "
                 "image size: {}x{}".format(template_level[1], w, h)
             )
             MEAS.start("CV2.MATCHTEMPLATE TIME")
-            res = cv2.matchTemplate(
-                image_levels[0][0], template_level[0], cv2.TM_CCOEFF_NORMED
-            )
+            res = cv2.matchTemplate(image_levels[0][0], template_level[0], cv2.TM_CCOEFF_NORMED)
             MEAS.stop()
             # print("did matchTemplate, res:\n")
             # print(res)
             MEAS.start("EXTRACT POINTS TIME")
             current_points, highest_max_val, highest_max_val_loc = self._extract_points(
                 h, res, threshold, w
             )
@@ -288,51 +279,55 @@
         self,
         needle: str,
         haystack: str,
         tolerance: float = 0.95,
         draw: int = 1,
         template_res_w: int = 1440,
         device_res_w: int = 1080,
+        grayscale: bool = True,
     ) -> tuple[int, int]:
         """Locate an image (needle) within an bigger image (haystack). Tolarance
         is pixel tolerance, i.e. 1.0 = all pixels are correct, 0.5 = 50% of the pixels
         are correct. If we know the original resolution, from which the template
         image is coming, we can supply it as template_res_w.
         Return value is the central (x,y) of the first image found.
         Draw function will plot red lines where needle image is found.
         """
 
         print("*INFO* _image_location Starts")
 
         image = cv2.imread(haystack)
-        image_gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-        _hay_h, hay_w = image_gray.shape[:2]
+        image_haystack = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) if grayscale else image
+        _hay_h, hay_w = image_haystack.shape[:2]
 
         needle_path = Path(needle)
         if not needle_path.exists():
             raise FileNotFoundError(f"Needle file does not exist. Tried: {needle_path}")
-        template = cv2.imread(str(needle_path.resolve()), 0)
+        template = (
+            cv2.imread(str(needle_path.resolve()), 0)
+            if grayscale
+            else cv2.imread(str(needle_path.resolve()), cv2.IMREAD_COLOR)
+        )  # Read in color
 
         if template is None:
             raise FileNotFoundError(f"Cannot read template image. Tried: {needle}")
+
         height, width = template.shape[:2]
 
         scale_ratios = self._get_scale_ratios(template_res_w, device_res_w)
         print(f"*DEBUG* Scale ratios to be used in order: {scale_ratios}")
 
         best_highest_max_val = 0.0
         best_highest_max_val_loc = (-1, -1)
         best_scale_ratio: float  # = None
         best_matched_image: ndarray  # = None
 
         print("*DEBUG* Resampling loop Starts")
         for scale_ratio in scale_ratios:
-            interpolation_method = (
-                cv2.INTER_LINEAR if scale_ratio > 1.0 else cv2.INTER_AREA
-            )
+            interpolation_method = cv2.INTER_LINEAR if scale_ratio > 1.0 else cv2.INTER_AREA
 
             print(f"*DEBUG* resize starts: for scale {scale_ratio}")
 
             if math.isclose(scale_ratio, 1.0, rel_tol=0.03):
                 scaled_img_template = template
             else:
                 scaled_img_template = cv2.resize(
@@ -340,17 +335,15 @@
                     None,
                     fx=scale_ratio,
                     fy=scale_ratio,
                     interpolation=interpolation_method,
                 )
             print("*DEBUG* matchTemplate Starts:")
 
-            res = cv2.matchTemplate(
-                image_gray, scaled_img_template, cv2.TM_CCOEFF_NORMED
-            )
+            res = cv2.matchTemplate(image_haystack, scaled_img_template, cv2.TM_CCOEFF_NORMED)
 
             ratio = device_res_w / hay_w
 
             if CONFIG.get_value("RetinaDisplay"):
                 ratio = ratio * 2
             elif ratio < 1.1:
                 ratio = 1.0
@@ -398,14 +391,15 @@
         )
         self._log_matched_image(
             image,
             template,
             best_matched_image,
             best_highest_max_val_loc,
             best_scale_ratio,
+            grayscale=grayscale,
         )
 
         if best_highest_max_val >= tolerance:
             return best_highest_max_val_loc
 
         return -1, -1
 
@@ -470,37 +464,39 @@
     @staticmethod
     def _log_matched_image(
         haystack: ndarray,
         needle: ndarray,
         scaled_needle: ndarray,
         loc: tuple[int, int],
         best_scale: float,
+        grayscale: bool = True,
     ) -> None:
         """Draw a composite image with the needle image, the haystack image,
         the scaled needle that matches the best and show where in haystack
         the best match is. This is best used in debugging, but it could be
         modified to add the image to the Robot log as well.
         """
-        needle = cv2.cvtColor(needle, cv2.COLOR_GRAY2BGR)
-        scaled_needle = cv2.cvtColor(scaled_needle, cv2.COLOR_GRAY2BGR)
+        if grayscale:
+            needle = cv2.cvtColor(needle, cv2.COLOR_GRAY2BGR)
+            scaled_needle = cv2.cvtColor(scaled_needle, cv2.COLOR_GRAY2BGR)
         h1, w1 = needle.shape[:2]
         hs, ws = scaled_needle.shape[:2]
         h2, w2 = haystack.shape[:2]
         max_left_w = max(w1, ws)
         cv2.rectangle(
             haystack,
             (loc[0] - int(w1 / 2 * best_scale), loc[1] - int(h1 / 2 * best_scale)),
             (loc[0] + int(w1 / 2 * best_scale), loc[1] + int(h1 / 2 * best_scale)),
             (0, 0, 255),
             2,
         )
         result = np.zeros((max(h2, h1), w2 + max_left_w, 3), np.uint8)
         result[:h1, :w1, :3] = needle
-        result[h1:h1 + hs, :ws, :3] = scaled_needle
-        result[:h2, max_left_w:max_left_w + w2, :3] = haystack
+        result[h1 : h1 + hs, :ws, :3] = scaled_needle  # noqa: E203
+        result[:h2, max_left_w : max_left_w + w2, :3] = haystack  # noqa: E203
 
         cv2.line(
             result,
             (ws, h1),
             (loc[0] + max_left_w + int(ws / 2), loc[1] - int(hs / 2)),
             (0, 0, 255),
             2,
@@ -518,25 +514,32 @@
             filename = f"temp_matched_image-{uuid4()}.png"
             filepath = os.path.join(output, SCREEN_SHOT_DIR_NAME, filename)
             cv2.imwrite(filepath, result)
             log_screenshot_file(filepath)
 
 
 def image_recognition(
-    image_path: str, template_res_w: int, browser_res_w: int, pyautog: bool
+    image_path: str,
+    template_res_w: int,
+    browser_res_w: int,
+    pyautog: bool,
+    tolerance: float = 0.95,
+    grayscale: bool = True,
 ) -> tuple[int, int]:
     """Return icon's coordinates."""
     image_rec = QIcon()
     frame.wait_page_loaded()
     screenshot_path = save_screenshot("screenshot.png", pyautog=pyautog)
     x, y = image_rec.image_location(
         needle=image_path,
         haystack=screenshot_path,
+        tolerance=tolerance,
         template_res_w=template_res_w,
         device_res_w=browser_res_w,
+        grayscale=grayscale,
     )
     return x, y
 
 
 def get_full_image_path(icon: str) -> Path:
     """Return image's full path."""
     if icon.endswith(".png") or icon.endswith(".jpg"):
```

### Comparing `QWeb-3.2.1/QWeb/internal/input_.py` & `QWeb-3.3.0/QWeb/internal/input_.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 # limitations under the License.
 # ---------------------------
 from __future__ import annotations
 from typing import Optional, Union
 from selenium.webdriver.remote.webelement import WebElement
 
 from robot.api import logger
-from QWeb.internal.exceptions import QWebElementNotFoundError, \
-    QWebInstanceDoesNotExistError
+from QWeb.internal.exceptions import QWebElementNotFoundError, QWebInstanceDoesNotExistError
 from QWeb.internal import element, text, frame, javascript, util
 from QWeb.internal.table import Table
 from QWeb.internal.config_defaults import CONFIG
 
 
 def get_input_element_by_locator(locator: str, anchor: Union[str, int], **kwargs) -> WebElement:
     """Find input element.
@@ -48,43 +47,46 @@
             xpath = locator
         input_element = element.get_unique_element_by_xpath(xpath, index=anchor, **kwargs)
     else:  # Search using text
         input_xpath = CONFIG["MatchingInputElement"].format(locator)
         input_elements = element.get_webelements_in_active_area(input_xpath, **kwargs)
         if not input_elements:  # Find input element using locator
             locator_element = text.get_text_using_anchor(locator, str(anchor), **kwargs)
-            input_elements = _get_all_input_elements()
+            # search for only file type inputs if upload is set
+            if kwargs.get("upload", False):
+                input_elements = _get_all_input_elements('//input[@type="file"]')
+            else:
+                input_elements = _get_all_input_elements(CONFIG["AllInputElements"])
 
-            shadow_dom = CONFIG['ShadowDOM']
+            shadow_dom = CONFIG["ShadowDOM"]
             if shadow_dom:
                 shadow_inputs = element.get_all_inputs_from_shadow_dom()
                 #  remove duplicates (normal search and including shadow search)
                 input_elements = util.remove_duplicates_from_list(shadow_inputs, input_elements)
 
             input_element = element.get_closest_element(locator_element, input_elements)
         elif len(input_elements) == 1:
             input_element = input_elements[0]  # pylint: disable=unsubscriptable-object
         else:  # Found many
             input_element = text.get_element_using_anchor(input_elements, anchor, **kwargs)
     return input_element
 
 
-def _get_all_input_elements() -> list[WebElement]:
-    input_elements = element.get_webelements_in_active_area(CONFIG["AllInputElements"],
-                                                            stay_in_current_frame=True)
-    return input_elements
+def _get_all_input_elements(xpath: str) -> list[WebElement]:
+    return element.get_webelements_in_active_area(xpath, stay_in_current_frame=True)
 
 
 def get_input_elements_from_all_documents(
-        locator: str,
-        anchor: str,
-        timeout: Union[int, float, str],  # pylint: disable=unused-argument
-        index: Union[int, str] = 1,
-        enable_check: bool = False,
-        **kwargs) -> WebElement:
+    locator: str,
+    anchor: str,
+    timeout: Union[int, float, str],  # pylint: disable=unused-argument
+    index: Union[int, str] = 1,
+    enable_check: bool = False,
+    **kwargs,
+) -> WebElement:
     """Function for finding input elements.
     Parameters
     ----------
     locator : str
        Label text or attribute that points to the checkbox.
     anchor : str
        in case there is duplicates.
@@ -104,134 +106,138 @@
             finding relative input element for some label text.
     Returns
     -------
     WebElement
     """
     input_element: Optional[WebElement]
     index = int(index) - 1
-    css = 'input:not([type="hidden"]):not([type="submit"]):not([type="button"])' \
-          ':not([type="reset"]):not([type="checkbox"]):not([type="radio"])' \
-          ':not([aria-hidden="true"]),' \
-          'textarea:not([type="hidden"]),[contenteditable="true"]'
-    kwargs['css'] = kwargs.get('css', css)
+    css = (
+        'input:not([type="hidden"]):not([type="submit"]):not([type="button"])'
+        ':not([type="reset"]):not([type="checkbox"]):not([type="radio"])'
+        ':not([aria-hidden="true"]),'
+        'textarea:not([type="hidden"]),[contenteditable="true"]'
+    )
+    kwargs["css"] = kwargs.get("css", css)
     if Table.is_table_coordinates(locator):
         table = Table.ACTIVE_TABLE.update_table()
         if table is None:
-            raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+            raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
         locator_element = table.get_table_cell(locator, anchor)
-        input_elements = element.get_element_from_childnodes(locator_element,
-                                                             kwargs['css'],
-                                                             dom_traversing=False)
+        input_elements = element.get_element_from_childnodes(
+            locator_element, kwargs["css"], dom_traversing=False
+        )
         if input_elements:
             return input_elements[int(index)]
-        raise QWebElementNotFoundError('No matching table input found')
+        raise QWebElementNotFoundError("No matching table input found")
     css_selector = CONFIG["CssSelectors"]
-    if not css_selector or locator.startswith('xpath=') or locator.startswith('//'):
+    if not css_selector or locator.startswith("xpath=") or locator.startswith("//"):
         input_element = get_input_element_by_locator(locator, index, **kwargs)
     else:
-        logger.debug('Uses CSS-selectors to locate element')
-        input_element = get_input_element_by_css_selector(locator, anchor, int(index), enable_check,
-                                                          **kwargs)
+        logger.debug("Uses CSS-selectors to locate element")
+        input_element = get_input_element_by_css_selector(
+            locator, anchor, int(index), enable_check, **kwargs
+        )
         if not input_element:
             input_element = get_input_element_by_locator(locator, index, **kwargs)
     if input_element:
-        if CONFIG['SearchMode']:
+        if CONFIG["SearchMode"]:
             element.draw_borders(input_element)
         return input_element
-    raise QWebElementNotFoundError('No matching input elements found')
+    raise QWebElementNotFoundError("No matching input elements found")
 
 
-def get_input_element_by_css_selector(locator: str,
-                                      anchor: str,
-                                      index: int = 0,
-                                      enable_check: bool = False,
-                                      **kwargs) -> Optional[WebElement]:
+def get_input_element_by_css_selector(
+    locator: str, anchor: str, index: int = 0, enable_check: bool = False, **kwargs
+) -> Optional[WebElement]:
     """Get input element using css selectors.
-       Parameters
-       ----------
-       locator : str
-           Label text or attribute that points to the input.
-           Looking for placeholder and commonly used tooltip-attributes first.
-           If locator is label text, finds input element by it's for attribute.
-           if for attribute is not available, then finds element by doing some
-           DOM traversing.
-       anchor : str
-           Text near the locator element or index. If placeholder or another
-           direct attribute (title, tooltip, value) exists then anchor
-           has to be index. Text is aloud when searching by label or some other
-           text which is near to input element.
-       index: int
-            If multiple input elements is nested or in same table cell, index is needed.
-       enable_check: bool
-            If enable_check is set to true returns first match even if disabled one.
-       Returns
-       -------
-       WebElement
-       """
+    Parameters
+    ----------
+    locator : str
+        Label text or attribute that points to the input.
+        Looking for placeholder and commonly used tooltip-attributes first.
+        If locator is label text, finds input element by it's for attribute.
+        if for attribute is not available, then finds element by doing some
+        DOM traversing.
+    anchor : str
+        Text near the locator element or index. If placeholder or another
+        direct attribute (title, tooltip, value) exists then anchor
+        has to be index. Text is aloud when searching by label or some other
+        text which is near to input element.
+    index: int
+         If multiple input elements is nested or in same table cell, index is needed.
+    enable_check: bool
+         If enable_check is set to true returns first match even if disabled one.
+    Returns
+    -------
+    WebElement
+    """
     input_element: Union[Optional[WebElement], list[WebElement]]
     partial_matches: list[WebElement] = []
-    upload = kwargs.get('upload')
+    upload = kwargs.get("upload")
     if upload:
         try:
             index = int(locator) - 1
-            kwargs['any_element'] = True
+            kwargs["any_element"] = True
             input_elements = element.get_elements_by_attributes(**kwargs)
             if input_elements:
                 return input_elements[index]
         except ValueError:
-            logger.debug('locator was text')
-    if 'qweb_old' not in kwargs:
+            logger.debug("locator was text")
+    if "qweb_old" not in kwargs:
         full_matches, partial_matches = get_input_elements_by_css(locator, **kwargs)
 
         if full_matches:
             full_matches = text.filter_by_modal_ancestor(full_matches)
             input_element = element.get_visible_elements_from_elements(full_matches, **kwargs)
-            if input_element and str(anchor) == '1':
+            if input_element and str(anchor) == "1":
                 input_element = input_element[index]
                 return input_element
             if input_element:
                 input_element = text.get_element_using_anchor(input_element, anchor, **kwargs)
                 return input_element
     try:
         locator_element = text.get_text_using_anchor(locator, anchor, **kwargs)
         input_elements = list(
             dict.fromkeys(
-                element.get_element_from_childnodes(locator_element, **kwargs) + partial_matches))
+                element.get_element_from_childnodes(locator_element, **kwargs) + partial_matches
+            )
+        )
     except QWebElementNotFoundError:
-        logger.trace('Element not found by visible text. Trying with partial match')
+        logger.trace("Element not found by visible text. Trying with partial match")
         input_elements = partial_matches
     if input_elements:
         input_elements = text.filter_by_modal_ancestor(input_elements)
         visibles = element.get_visible_elements_from_elements(input_elements, **kwargs)
         if visibles:
             if element.is_enabled(visibles[index]) or enable_check is True:
                 return visibles[index]
     return None
 
 
 @frame.all_frames
 def get_inputs_including_shadow_dom(locator: str, **kwargs) -> list[WebElement]:
     web_elements = element.get_visible_elements_from_elements(
-        javascript.get_all_input_elements_from_shadow_dom(), **kwargs)
+        javascript.get_all_input_elements_from_shadow_dom(), **kwargs
+    )
 
     matches = javascript.get_by_attributes(web_elements, locator, False)
-    full, partial = matches.get('full', []), matches.get('partial', [])
+    full, partial = matches.get("full", []), matches.get("partial", [])
     shadow_elements = full + partial
     if shadow_elements:
-        logger.debug(f'Found {len(shadow_elements)} inputs when extending search to shadow dom')
+        logger.debug(f"Found {len(shadow_elements)} inputs when extending search to shadow dom")
     return shadow_elements
 
 
 def get_input_elements_by_css(locator: str, **kwargs):
     full_matches, partial_matches = element.get_elements_by_css(locator, **kwargs)
     # return if we already get a full match
     if full_matches:
         return full_matches, partial_matches
 
-    shadow_dom = CONFIG['ShadowDOM']
+    shadow_dom = CONFIG["ShadowDOM"]
     if shadow_dom:
         shadow_elements = get_inputs_including_shadow_dom(locator, **kwargs)
         #  remove duplicates (normal search and including shadow search)
         for el in shadow_elements:
             if full_matches is not None and el not in list(full_matches):
                 full_matches.append(el)  # type: ignore[union-attr]
     return full_matches, partial_matches
```

### Comparing `QWeb-3.2.1/QWeb/internal/input_handler.py` & `QWeb-3.3.0/QWeb/internal/input_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,158 +19,164 @@
 import os
 import pyperclip
 from pyautogui import KEY_NAMES
 from robot.api import logger
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.common.keys import Keys
 from selenium.common.exceptions import ElementNotInteractableException
-from QWeb.internal.exceptions import QWebInvalidElementStateError, QWebValueError, \
-    QWebEnvironmentError
+from QWeb.internal.exceptions import (
+    QWebInvalidElementStateError,
+    QWebValueError,
+    QWebEnvironmentError,
+)
 from QWeb.internal import javascript
 
 try:
-    if not os.getenv('QWEB_HEADLESS', None):
+    if not os.getenv("QWEB_HEADLESS", None):
         from pynput.keyboard import Controller
 except ImportError:
-    logger.warn('Cannot import pynput.keyboard, no display detected')
+    logger.warn("Cannot import pynput.keyboard, no display detected")
 
 
 class InputHandler:
-
-    def __init__(self,
-                 input_method: str = "selenium",
-                 line_break_key: str = "\ue004",
-                 clear_key: Optional[str] = None) -> None:
+    def __init__(
+        self,
+        input_method: str = "selenium",
+        line_break_key: str = "\ue004",
+        clear_key: Optional[str] = None,
+    ) -> None:
         self._input_method = input_method
         self.line_break_key = line_break_key
         self.clear_key = clear_key
 
     @property
     def input_method(self) -> str:
         return self._input_method
 
     @input_method.setter
     def input_method(self, input_method: str) -> None:
         required = ["javascript", "selenium", "raw"]
         if input_method not in required:
-            raise QWebValueError('Unknown input_method: {}, required: {}'.format(
-                input_method, required))
+            raise QWebValueError(
+                "Unknown input_method: {}, required: {}".format(input_method, required)
+            )
         self._input_method = input_method
 
     def write(self, input_element: WebElement, input_text: str, **kwargs) -> None:
-        """ Writes the given text using configured writer. """
+        """Writes the given text using configured writer."""
         write = self._get_writer()
         # By clearing the input field with Javascript,
         # we avoid triggering focus events right after
         # clear and trigger them only on send_keys call.
-        clear_key = self.check_key(kwargs.get('clear_key', self.clear_key))
-        shadow_dom = kwargs.get('shadow_dom', False)
+        clear_key = self.check_key(kwargs.get("clear_key", self.clear_key))
+        shadow_dom = kwargs.get("shadow_dom", False)
         if not clear_key:
             if self.is_editable_text_element(input_element):
                 javascript.execute_javascript('arguments[0].innerText=""', input_element)
             else:
-                javascript.execute_javascript("arguments[0].value = \"\"", input_element)
+                javascript.execute_javascript('arguments[0].value = ""', input_element)
         else:
             input_element.send_keys(*[key for key in clear_key if key is not None])
         try:
             write(input_element, input_text)
         # workaround for Firefox shadow dom inputs not always being reachable
         except ElementNotInteractableException as e:
             if shadow_dom:
                 javascript.execute_javascript(f'arguments[0].value = "{input_text}"', input_element)
-                kwargs['key'] = None
+                kwargs["key"] = None
             else:
                 raise e from e
 
-        if 'check' not in kwargs:
-            line_break = kwargs.get('key', self.check_key(self.line_break_key))
+        if "check" not in kwargs:
+            line_break = kwargs.get("key", self.check_key(self.line_break_key))
             if line_break:
                 input_element.send_keys(line_break)
 
     def _get_writer(self) -> Callable[..., Any]:
         if self._input_method == "selenium":
             return InputHandler._selenium_writer
         if self._input_method == "javascript":
             return InputHandler._js_writer
         return self._raw_writer
 
     @staticmethod
     def _selenium_writer(input_element: WebElement, input_text: str) -> None:
-        """ Use Selenium librarys input methods clear() and send_keys(). """
+        """Use Selenium librarys input methods clear() and send_keys()."""
         if not input_element.is_enabled():
             logger.warn("Element not enabled. Try with alternative input method?")
             raise QWebInvalidElementStateError("Input element is not enabled")
         input_element.send_keys(input_text)
 
     @staticmethod
     def _js_writer(input_element: WebElement, input_text: str) -> None:
-        """ Use JavaScript to set input element value."""
+        """Use JavaScript to set input element value."""
         if not input_element.is_enabled():
             logger.warn("Element not enabled. Try with alternative input method?")
             raise QWebInvalidElementStateError("Input element is not enabled")
         javascript.execute_javascript(f'arguments[0].value = "{input_text}"', input_element)
 
     @staticmethod
     def _raw_writer(input_element: WebElement, input_text: str) -> None:
-        """ Control keyboard and text input with pyautogui. This doesn't
-            do any checks for the element state.
+        """Control keyboard and text input with pyautogui. This doesn't
+        do any checks for the element state.
         """
         # Sanity check even if the input_element is not required for the input
         if not input_element:
-            raise QWebValueError('Input element is not available.')
-        if os.getenv('QWEB_HEADLESS', None):
-            raise QWebEnvironmentError('Running in headless environment. Pynput is unavailable.')
+            raise QWebValueError("Input element is not available.")
+        if os.getenv("QWEB_HEADLESS", None):
+            raise QWebEnvironmentError("Running in headless environment. Pynput is unavailable.")
         keyboard = Controller()
         keyboard.type(input_text)
 
     @staticmethod
     def is_editable_text_element(input_element: WebElement) -> bool:
         if javascript.execute_javascript(
-                'return arguments[0].getAttribute("contenteditable") == "true"', input_element):
+            'return arguments[0].getAttribute("contenteditable") == "true"', input_element
+        ):
             return True
         return False
 
     @staticmethod
     def check_key(key: Optional[str]) -> Union[Optional[str], list[Optional[str]]]:
         if not key:
             return None
-        if key == '{PASTE}':
+        if key == "{PASTE}":
             return pyperclip.paste()
         hotkey = []
-        if key.startswith('{') and key.endswith('}'):
+        if key.startswith("{") and key.endswith("}"):
             key = key[1:-1].upper()
-            if '+' in key:
-                keys = key.split('+')
+            if "+" in key:
+                keys = key.split("+")
                 for k in keys:
                     try:
                         key = getattr(Keys, k.strip())
                     except AttributeError:
                         key = k.lower().strip()
                     hotkey.append(key)
                 return hotkey
             key = getattr(Keys, key)
         return key
 
     @staticmethod
     def check_key_pyautogui(key: Optional[str]) -> Union[Optional[str], list[str]]:
         if not key:
             return None
-        if key == '{PASTE}':
+        if key == "{PASTE}":
             return pyperclip.paste()
         hotkey = []
-        if key.startswith('{') and key.endswith('}'):
+        if key.startswith("{") and key.endswith("}"):
             key = key[1:-1].lower()
-            if '+' in key:
-                keys = key.split('+')
+            if "+" in key:
+                keys = key.split("+")
                 for k in keys:
-                    if not k.strip() in KEY_NAMES:
+                    if k.strip() not in KEY_NAMES:
                         raise AttributeError
                     key = k.strip()
                     hotkey.append(key)
                 return hotkey
-            if not key.strip() in KEY_NAMES:
+            if key.strip() not in KEY_NAMES:
                 raise AttributeError
         return key
 
 
 # Instantiate here as global
 INPUT_HANDLER: InputHandler = InputHandler()
```

### Comparing `QWeb-3.2.1/QWeb/internal/javascript.py` & `QWeb-3.3.0/QWeb/internal/javascript.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,17 @@
         return elemObjects;
         }
         return(visibility(arguments[0]));
         """
     return execute_javascript(js, web_elements)
 
 
-def highlight_element(element: WebElement,
-                      draw_only: bool,
-                      flash_border: bool = False,
-                      color: str = "blue") -> None:
+def highlight_element(
+    element: WebElement, draw_only: bool, flash_border: bool = False, color: str = "blue"
+) -> None:
     """Highlight borders for given web element.
 
     Parameters
     ----------
     element : web element
         Element to highlight.
     draw_only : bool
@@ -125,16 +124,17 @@
 
            show(arguments[0], arguments[1], arguments[2], arguments[3]);
            """
     js = js.replace("{COLOR}", color)
     execute_javascript(js, element, draw_only, flash_border, color)
 
 
-def get_by_attributes(elements: list[WebElement], locator: str,
-                      partial_match: bool) -> dict[str, list[WebElement]]:
+def get_by_attributes(
+    elements: list[WebElement], locator: str, partial_match: bool
+) -> dict[str, list[WebElement]]:
     """Return web element by it's attribute value.
 
     Parameters
     ----------
     elements : web elements
         List of web elements.
     locator : str
@@ -171,15 +171,15 @@
                     }
                }
             }
             matches = {full:full, partial:part};
             return matches;
         }
         return(web_elements(arguments[0], arguments[1], arguments[2]));"""
-    return execute_javascript(js, elements, locator.replace("\'", "\\'"), partial_match)
+    return execute_javascript(js, elements, locator.replace("'", "\\'"), partial_match)
 
 
 def get_all_elements(css: str) -> list[WebElement]:
     """Return all web elements for given css-locator.
     Parameters
     ----------
     css : selector
@@ -188,18 +188,17 @@
     Returns
     -------
     list of web elements.
     """
     return execute_javascript("return document.querySelectorAll('{}')".format(css))
 
 
-def get_childnodes(locator_element: WebElement,
-                   css: str,
-                   level: int = 3,
-                   traverse: bool = True) -> list[WebElement]:
+def get_childnodes(
+    locator_element: WebElement, css: str, level: int = 3, traverse: bool = True
+) -> list[WebElement]:
     """Find matching childs for given locator element.
     Parameters
     ----------
     locator_element : web element
     css : css selector/html tag
         For example: input
     level : Traverse limit (how many steps we are going up while searching).
@@ -227,16 +226,17 @@
                 return [];
             }
         return(elements(arguments[0], arguments[1],  arguments[2], arguments[3]));
         """
     return execute_javascript(js, locator_element, css, level, traverse)
 
 
-def get_by_label(locator_text: str, css: str, level: int,
-                 partial_match: bool) -> dict[str, list[WebElement]]:
+def get_by_label(
+    locator_text: str, css: str, level: int, partial_match: bool
+) -> dict[str, list[WebElement]]:
     """Find element based on it's label.
 
     First we sneak if there is for-attribute available. If so, it's used
     to locate correct element. If for-attribute is not available then we are doing
     some dom-traversing to locate correct element.
 
     Parameters
@@ -325,19 +325,20 @@
                 }
             }
             matches = {full:full_matches.concat(part_with_for), partial:part_matches};
             return matches;
         }
         return(web_elements(arguments[0], arguments[1], arguments[2], arguments[3]));
         """
-    return execute_javascript(js, locator_text.replace("\'", "\\'"), css, level, partial_match)
+    return execute_javascript(js, locator_text.replace("'", "\\'"), css, level, partial_match)
 
 
-def get_parent_list(locator_element: Union[WebElement, str], css: str
-                    ) -> Union[WebElement, list[WebElement]]:
+def get_parent_list(
+    locator_element: Union[WebElement, str], css: str
+) -> Union[WebElement, list[WebElement]]:
     """Get parent list for web element.
 
     Parameters
     ----------
     locator_element : str
     css : css selector/html tag
         For example: div
@@ -393,21 +394,22 @@
                     textNodes.push(currentNode.parentElement);
                 }
             }
             return textNodes;
         }
         return(getTextNodes(arguments[0], arguments[1], arguments[2]))
         """
-    doc = 'html'
-    partial = kwargs.get('partial_match')
+    doc = "html"
+    partial = kwargs.get("partial_match")
     return execute_javascript(js, text, doc, partial)
 
 
 def get_clickable(locator: str) -> list[WebElement]:
-    js = """
+    js = (
+        """
     var web_elements = function(locator){
         var full = [];
         var partial = [];
         var candidates = [];
         var text = "";
         var elems = document.querySelectorAll('button, a, label,\
         *[type="submit"], *[type="button"], *[type="reset"], li[data-value], input[type="radio"],\
@@ -425,15 +427,18 @@
             else if (text.trim().toLowerCase() === locator.toLowerCase()){
                 partial.push(elems[i]);
             }
         }
         candidates = full.concat(partial);
         return candidates;
     }
-    return(web_elements('""" + locator.replace("\'", "\\'") + """'));"""
+    return(web_elements('"""
+        + locator.replace("'", "\\'")
+        + """'));"""
+    )
     return execute_javascript(js)
 
 
 def get_recursive_walk() -> str:
     return """var recursiveWalk = function(node, func) {
     var done = func(node);
     if(done) {
@@ -455,26 +460,28 @@
         node = node.nextSibling;
     }
 
     }"""
 
 
 def get_text_elements_from_shadow_dom(locator: str, partial: bool) -> list[WebElement]:
-    js = get_recursive_walk() + """
+    js = (
+        get_recursive_walk()
+        + """
     function find_text_from_shadow_dom(text, partial){
         var results = [];
         var unsupported_tags = ["script", "#document-fragment"]
         var elem = recursiveWalk(document.body, function(node) {
         //if (node.innerText == text) {
         // handle non-breaking spaces, they are not considered the same as normal space
         // when querying textContent
         if (node.textContent.replace(/\u00a0/g, ' ').includes(text) && !unsupported_tags.includes(node.nodeName.toLowerCase())) {
             nodetext = [].reduce.call(node.childNodes, function(a, b) { return a + (b.nodeType === 3 ? b.textContent.trim() : ''); }, '');
             // handle non-breaking spaces
-            nodetext = nodetext.replace(/\u00A0/g, ' ')
+            nodetext = nodetext.replace(/\u00a0/g, ' ')
             if (nodetext == text) {
                 results.push(node);
             }
             else if (partial && nodetext.includes(text)) {
                  results.push(node)
             }
         }
@@ -482,19 +489,22 @@
                 results.push(node)
         }
     });
 
         return results;
     }
     return(find_text_from_shadow_dom(arguments[0], arguments[1]))"""
+    )
     return execute_javascript(js, locator, partial)
 
 
 def get_clickable_from_shadow_dom(locator: str, partial: bool) -> list[WebElement]:
-    js = get_recursive_walk() + """
+    js = (
+        get_recursive_walk()
+        + """
     function find_clickable_from_shadow_dom(text, partial){
         var results = [];
         var full = [];
         var parts = [];
         var clickable_types = ["button", "reset", "submit"]
         var elem = recursiveWalk(document.body, function(node) {
             try {
@@ -517,77 +527,90 @@
                 }
             } catch(ex) {}
         });
         results = full.concat(parts);
         return results;
     }
     return(find_clickable_from_shadow_dom(arguments[0], arguments[1]))"""
+    )
     return execute_javascript(js, locator, partial)
 
 
 def get_all_frames_from_shadow_dom() -> list[WebElement]:
-    js = get_recursive_walk() + """
+    js = (
+        get_recursive_walk()
+        + """
     function find_all_frames_from_shadow_dom(){
         var results = [];
         var elem = recursiveWalk(document.body, function(node) {
             if (node.tagName == "IFRAME" || node.tagName == "FRAME") {
                     results.push(node);
             }
 
         });
         return results;
     }
 
     return(find_all_frames_from_shadow_dom(arguments[0]))"""
+    )
     return execute_javascript(js)
 
 
 def get_all_input_elements_from_shadow_dom() -> list[WebElement]:
-    js = get_recursive_walk() + """
+    js = (
+        get_recursive_walk()
+        + """
     function find_all_input_elements_from_shadow_dom(){
         var results = [];
         var elem = recursiveWalk(document.body, function(node) {
             if (node.tagName == "INPUT" || node.tagName == "TEXTAREA") {
                     results.push(node);
             }
 
         });
         return results;
     }
 
     return(find_all_input_elements_from_shadow_dom(arguments[0]))"""
+    )
     return execute_javascript(js)
 
 
 def get_all_dropdown_elements_from_shadow_dom() -> list[WebElement]:
-    js = get_recursive_walk() + """
+    js = (
+        get_recursive_walk()
+        + """
     function find_all_select_elements_from_shadow_dom(){
         var results = [];
         var elem = recursiveWalk(document.body, function(node) {
             if (node.tagName == "SELECT") {
                     results.push(node);
             }
 
         });
         return results;
     }
 
     return(find_all_select_elements_from_shadow_dom(arguments[0]))"""
+    )
     return execute_javascript(js)
 
 
 def get_item_elements_from_shadow_dom(tag: str) -> list[WebElement]:
-    js = get_recursive_walk() + """
+    js = (
+        get_recursive_walk()
+        + """
     function find_item_elements_from_shadow_dom(tag){
         var results = [];
         var supported_tags = tag === null ? ["A", "SPAN", "IMG", "LI", "H1", "H2", "H3", "H4", "H5", "H6", "DIV", "SVG", "P", "BUTTON", "INPUT", "TEXTAREA"] : [tag.toUpperCase()];
         var elem = recursiveWalk(document.body, function(node) {
             if (supported_tags.includes(node.tagName)) {
                     results.push(node);
             }
 
         });
         return results;
     }
 
     return(find_item_elements_from_shadow_dom(arguments[0], arguments[1]))"""
+    )
     return execute_javascript(js, tag)
```

### Comparing `QWeb-3.2.1/QWeb/internal/lists.py` & `QWeb-3.3.0/QWeb/internal/lists.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,42 +21,45 @@
 from robot.api import logger
 from QWeb.internal.exceptions import QWebElementNotFoundError
 from QWeb.internal import element, text, javascript, frame
 from QWeb.internal.config_defaults import CONFIG
 
 
 class List:
-
     ACTIVE_LIST: List
 
-    def __init__(self,
-                 web_list: list[str],
-                 web_element_list: list[WebElement],
-                 locator: str,
-                 anchor: str,
-                 parent: Optional[str] = None,
-                 child: Optional[str] = None,
-                 **kwargs) -> None:
+    def __init__(
+        self,
+        web_list: list[str],
+        web_element_list: list[WebElement],
+        locator: str,
+        anchor: str,
+        parent: Optional[str] = None,
+        child: Optional[str] = None,
+        **kwargs,
+    ) -> None:
         self.web_list = web_list
         self.web_element_list = web_element_list
         self.locator = locator
         self.anchor = anchor
         self.parent = parent
         self.child = child
         self.kwargs = kwargs
         List.ACTIVE_LIST = self
 
     @classmethod
     @frame.all_frames
-    def from_list_instance(cls,
-                           locator: str,
-                           anchor: str = "1",
-                           parent: Optional[str] = None,
-                           child: Optional[str] = None,
-                           **kwargs) -> List:
+    def from_list_instance(
+        cls,
+        locator: str,
+        anchor: str = "1",
+        parent: Optional[str] = None,
+        child: Optional[str] = None,
+        **kwargs,
+    ) -> List:
         """Find list and create list instance
 
         Parameters
         ----------
         locator : str
             Text that locates the table. The table that is closest
             to the text is selected. Also one can use xpath by adding xpath= prefix
@@ -75,115 +78,127 @@
         # TODO  How to type cls argument properly?
         web_list, web_element_list = cls.create_list(
             cls,  # type: ignore[arg-type]
             locator,
             anchor,
             parent=parent,
             child=child,
-            **kwargs)
+            **kwargs,
+        )
         return List(web_list, web_element_list, locator, anchor, parent, child, **kwargs)
 
-    def create_list(self, locator: str, anchor: str, **kwargs
-                    ) -> tuple[list[str], list[WebElement]]:
+    def create_list(
+        self, locator: str, anchor: str, **kwargs
+    ) -> tuple[list[str], list[WebElement]]:
         web_elements: Union[WebElement, list[WebElement]]
-        if locator.startswith('//') or locator.startswith('xpath='):
-            if locator.startswith('xpath='):
+        if locator.startswith("//") or locator.startswith("xpath="):
+            if locator.startswith("xpath="):
                 locator = locator.split("=", 1)[1]
             web_elements = self.get_elements_by_locator_xpath_and_tag_name(
-                locator, anchor, **kwargs)
+                locator, anchor, **kwargs
+            )
         else:
             web_elements = self.get_elements_by_locator_text_and_tag_name(locator, anchor, **kwargs)
-            logger.debug('webelems: {}'.format(web_elements))
+            logger.debug("webelems: {}".format(web_elements))
         if web_elements:
-            if CONFIG['SearchMode']:
+            if CONFIG["SearchMode"]:
                 element.draw_borders(web_elements)
             web_list = self.get_texts(web_elements)
             if isinstance(web_elements, WebElement):
                 return web_list, [web_elements]
             return web_list, web_elements
-        raise QWebElementNotFoundError('Suitable elements not found')
+        raise QWebElementNotFoundError("Suitable elements not found")
 
     @staticmethod
-    def get_elements_by_locator_text_and_tag_name(locator: str,
-                                                  anchor: str,
-                                                  index: int = 1,
-                                                  **kwargs) -> Union[WebElement, list[WebElement]]:
+    def get_elements_by_locator_text_and_tag_name(
+        locator: str, anchor: str, index: int = 1, **kwargs
+    ) -> Union[WebElement, list[WebElement]]:
         web_element: Optional[WebElement]
         locator_element: Optional[WebElement]
 
         index = int(index) - 1
-        if 'tag' in kwargs:
-            tag_name = kwargs.get('tag')
-        elif 'parent' in kwargs and kwargs['parent']:
-            tag_name = kwargs['parent']
-        elif 'child' in kwargs and kwargs['child']:
-            tag_name = kwargs['child']
+        if "tag" in kwargs:
+            tag_name = kwargs.get("tag")
+        elif "parent" in kwargs and kwargs["parent"]:
+            tag_name = kwargs["parent"]
+        elif "child" in kwargs and kwargs["child"]:
+            tag_name = kwargs["child"]
         else:
-            tag_name = 'ul'
+            tag_name = "ul"
 
         web_element = text.get_element_by_locator_text(locator, anchor)
-        if 'parent' in kwargs and kwargs['parent'] and web_element is not None:
-            tag = kwargs['parent']
+        if "parent" in kwargs and kwargs["parent"] and web_element is not None:
+            tag = kwargs["parent"]
             locator_element = element.get_parent_list_element(web_element, tag)
-        elif 'child' in kwargs and kwargs['child'] and web_element is not None:
-            tag = kwargs['child']
-            locator_element = element.get_element_from_childnodes(web_element,
-                                                                  tag,
-                                                                  dom_traversing=False)[index]
+        elif "child" in kwargs and kwargs["child"] and web_element is not None:
+            tag = kwargs["child"]
+            locator_element = element.get_element_from_childnodes(
+                web_element, tag, dom_traversing=False
+            )[index]
             if tag_name not in ["ul", "ol", "dl", "UL", "OL", "DL"]:
                 return locator_element
         else:
             locator_element = text.get_element_by_locator_text(locator, anchor)
 
         if tag_name not in ["ul", "ol", "dl", "UL", "OL", "DL"]:
             web_elements = javascript.execute_javascript(
-                'return arguments[0].querySelectorAll("{}")'.format(tag_name), locator_element)
+                'return arguments[0].querySelectorAll("{}")'.format(tag_name), locator_element
+            )
         else:
             web_elements = javascript.execute_javascript(
                 'return arguments[0].closest("{}").querySelectorAll("li, dt, dd")'.format(tag_name),
-                locator_element)
+                locator_element,
+            )
         return web_elements
 
     @staticmethod
-    def get_elements_by_locator_xpath_and_tag_name(locator: str,
-                                                   index: Union[int, str] = 1,
-                                                   **kwargs) -> list[WebElement]:
+    def get_elements_by_locator_xpath_and_tag_name(
+        locator: str, index: Union[int, str] = 1, **kwargs
+    ) -> list[WebElement]:
         index = int(index) - 1
-        if 'tag' in kwargs:
-            tag_name = kwargs.get('tag')
-        elif 'parent' in kwargs and kwargs['parent']:
-            tag_name = kwargs['parent']
-        elif 'child' in kwargs and kwargs['child']:
-            tag_name = kwargs['child']
+        if "tag" in kwargs:
+            tag_name = kwargs.get("tag")
+        elif "parent" in kwargs and kwargs["parent"]:
+            tag_name = kwargs["parent"]
+        elif "child" in kwargs and kwargs["child"]:
+            tag_name = kwargs["child"]
         else:
-            tag_name = 'ul'
-        if 'parent' in kwargs and kwargs['parent']:
+            tag_name = "ul"
+        if "parent" in kwargs and kwargs["parent"]:
             web_element = element.get_unique_element_by_xpath(locator, index=index)
-            css = kwargs.get('parent')
+            css = kwargs.get("parent")
             web_element = element.get_parent_list_element(web_element, str(css))
             if tag_name not in ["ul", "ol", "dl", "UL", "OL", "DL"]:
                 web_elements = javascript.execute_javascript(
-                    'return arguments[0].querySelectorAll("{}")'.format(tag_name), web_element)
+                    'return arguments[0].querySelectorAll("{}")'.format(tag_name), web_element
+                )
             else:
                 web_elements = javascript.execute_javascript(
                     'return arguments[0].closest("{}").querySelectorAll("li, dt, dd")'.format(
-                        tag_name), web_element)
-        elif 'child' in kwargs and kwargs['child']:
+                        tag_name
+                    ),
+                    web_element,
+                )
+        elif "child" in kwargs and kwargs["child"]:
             web_element = element.get_unique_element_by_xpath(locator)
-            css = kwargs.get('child')
-            web_elements = element.get_element_from_childnodes(web_element,
-                                                               str(css),
-                                                               dom_traversing=False)[index]
+            css = kwargs.get("child")
+            web_elements = element.get_element_from_childnodes(
+                web_element, str(css), dom_traversing=False
+            )[index]
             if tag_name not in ["ul", "ol", "dl", "UL", "OL", "DL"]:
                 web_elements = javascript.execute_javascript(
-                    'return arguments[0].querySelectorAll("{}")'.format(tag_name), web_element)
+                    'return arguments[0].querySelectorAll("{}")'.format(tag_name), web_element
+                )
             else:
                 web_elements = javascript.execute_javascript(
                     'return arguments[0].closest("{}").querySelectorAll("li, dt, dd")'.format(
-                        tag_name), web_element)
+                        tag_name
+                    ),
+                    web_element,
+                )
         else:
             web_elements = element.get_webelements_in_active_area(locator)
 
         return web_elements
 
     @staticmethod
     def get_texts(web_elements: Union[WebElement, list[WebElement]]) -> list[str]:
@@ -196,15 +211,16 @@
         return texts
 
     def contains(self, expected_match: str, index: Optional[int]) -> bool:
         if index is None:
             if expected_match in self.web_list:
                 return True
         else:
-            if expected_match in str(self.web_list[int(index)]).replace('\n', '').strip():
+            if expected_match in str(self.web_list[int(index)]).replace("\n", "").strip():
                 return True
         return False
 
     def update_list(self) -> List:
-        active_list = self.from_list_instance(self.locator, self.anchor, self.parent, self.child,
-                                              **self.kwargs)
+        active_list = self.from_list_instance(
+            self.locator, self.anchor, self.parent, self.child, **self.kwargs
+        )
         return active_list
```

### Comparing `QWeb-3.2.1/QWeb/internal/meas.py` & `QWeb-3.3.0/QWeb/internal/meas.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,38 +39,37 @@
    # some more inner code
    meas_obj().stop()
    meas_obj().stop()
 """
 
 
 class Meas(object):  # pylint: disable=bad-option-value, useless-object-inheritance
-
     def __init__(self, enabled: bool = True):
         """When initialized with enabled=False the functions
-           are no-ops"""
+        are no-ops"""
 
         if not enabled:
-            self.start = lambda a='': None  # type:ignore[assignment]
+            self.start = lambda a="": None  # type:ignore[assignment]
             self.stop = lambda a=True: None  # type:ignore[assignment]
             self.log = lambda a, b: None  # type:ignore[assignment, misc]
 
         self.timers: list[tuple[float, str]] = []
 
     # pylint: disable=method-hidden
-    def start(self, comment: str = '') -> None:
+    def start(self, comment: str = "") -> None:
         """Start a timer. Can be called multiple times without
-           a stop in between."""
+        a stop in between."""
         start_t = timeit.default_timer()
         self.timers.append((start_t, comment))
 
     # pylint: disable=method-hidden
     def stop(self, log: bool = True) -> Optional[float]:
         """Returns the calculated time against last started timer.
-           When called multiple times pops always the next available
-           timer."""
+        When called multiple times pops always the next available
+        timer."""
         stop_t = timeit.default_timer()
         start_t, comment = self.timers.pop()
         t = stop_t - start_t
         if log:
             # pylint: disable=too-many-function-args
             self.log(t, comment)
         return t
```

### Comparing `QWeb-3.2.1/QWeb/internal/platform.py` & `QWeb-3.3.0/QWeb/internal/platform.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.2.1/QWeb/internal/screenshot.py` & `QWeb-3.3.0/QWeb/internal/screenshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,36 +21,39 @@
 import base64
 import json
 import os
 from uuid import uuid4
 
 import cv2
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.common.exceptions import UnexpectedAlertPresentException, \
-                                       WebDriverException, InvalidSessionIdException
+from selenium.common.exceptions import (
+    UnexpectedAlertPresentException,
+    WebDriverException,
+    InvalidSessionIdException,
+)
 from QWeb.internal.browser import firefox, chrome, edge
 from QWeb.internal.exceptions import QWebDriverError
 from QWeb.internal import browser
 from QWeb.keywords import config
 from skimage.metrics import structural_similarity
 from robot.api import logger
 from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
 from robot.utils import get_link_path
 from pyautogui import screenshot as pyscreenshot
 from tempfile import gettempdir
 
-SCREEN_SHOT_DIR_NAME = 'screenshots'
-VERIFYAPP_DIR_NAME = 'verifyapp'
-VALID_FILENAME_CHARS = '-_.() abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'
+SCREEN_SHOT_DIR_NAME = "screenshots"
+VERIFYAPP_DIR_NAME = "verifyapp"
+VALID_FILENAME_CHARS = "-_.() abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
 MAX_LENGTH = 100  # filenames longer than 255 are not allowed by os
 
 
 def _create_screenshot_folder(foldername: str) -> str:
     try:
-        robot_output = BuiltIn().get_variable_value('${OUTPUT DIR}')
+        robot_output = BuiltIn().get_variable_value("${OUTPUT DIR}")
         screen_shot_dir = os.path.join(robot_output, foldername)
     except RobotNotRunningError:
         screen_shot_dir = os.path.join(os.getcwd(), foldername)
 
     if not os.access(screen_shot_dir, os.W_OK):
         screen_shot_dir = os.path.join(gettempdir(), foldername)
 
@@ -63,70 +66,70 @@
 def _remove_invalid_chars(text_to_check: str) -> str:
     """
     Removes invalid characters from filename
     :param text_to_check:
     :return:
     """
     valid = "".join(c for c in text_to_check if c in VALID_FILENAME_CHARS)
-    return valid if len(valid) <= MAX_LENGTH else valid[:MAX_LENGTH - 1]
+    return valid if len(valid) <= MAX_LENGTH else valid[: MAX_LENGTH - 1]
 
 
 def compare_screenshots(filename: str, accuracy: Union[str, float]) -> bool:
     # pylint: disable=no-member
     """Compare screenshot against reference, take reference if missing.
 
     :param filename:
     :return:
     """
     screenshot_dir = _create_screenshot_folder(SCREEN_SHOT_DIR_NAME)
     verifyapp_dir = _create_screenshot_folder(VERIFYAPP_DIR_NAME)
-    test_name = BuiltIn().get_variable_value('${TEST NAME}')
-    filename = _remove_invalid_chars('{0}_{1}'.format(test_name, filename))
+    test_name = BuiltIn().get_variable_value("${TEST NAME}")
+    filename = _remove_invalid_chars("{0}_{1}".format(test_name, filename))
     filename = filename.replace(" ", "_")
-    filename_ref = '{}_ref.png'.format(filename)
-    filename_cmp = '{}.png'.format(filename)
-    filename_dif = '{}_dif.png'.format(filename)
+    filename_ref = "{}_ref.png".format(filename)
+    filename_cmp = "{}.png".format(filename)
+    filename_dif = "{}_dif.png".format(filename)
     try:
         accuracy = float(accuracy)
     except ValueError as e:
-        raise ValueError('Invalid accuracy: {}'.format(accuracy)) from e
+        raise ValueError("Invalid accuracy: {}".format(accuracy)) from e
     # Save reference screenshot if it does not exist
     if not os.path.isfile(os.path.join(verifyapp_dir, filename_ref)):
         filepath_ref = save_screenshot(filename_ref, VERIFYAPP_DIR_NAME)
 
-        logger.info('Reference screenshot missing, saving.')
-        logger.info('Image path: {}'.format(filename_ref))
+        logger.info("Reference screenshot missing, saving.")
+        logger.info("Image path: {}".format(filename_ref))
         log_screenshot_file(filepath_ref)
         status = True
     # Compare screenshots if reference exists
     else:
         filepath_ref = os.path.join(verifyapp_dir, filename_ref)
         filepath_cmp = save_screenshot(filename_cmp, SCREEN_SHOT_DIR_NAME)
         ref_image = cv2.imread(filepath_ref, cv2.IMREAD_GRAYSCALE)
         ref_image_c = cv2.imread(filepath_ref, cv2.IMREAD_COLOR)
         new_image = cv2.imread(filepath_cmp, cv2.IMREAD_GRAYSCALE)
 
         (score, diff) = structural_similarity(ref_image, new_image, full=True)
         if score > accuracy:
-            logger.info('Images match with score: {}'.format(score))
+            logger.info("Images match with score: {}".format(score))
             log_screenshot_file(filepath_cmp)
-            logger.info('Image path: {}'.format(filename_cmp))
+            logger.info("Image path: {}".format(filename_cmp))
             status = True
         else:
-            logger.error('Images differ with score: {}'.format(score))
-            logger.info('Reference image: {}'.format(filename_ref))
+            logger.error("Images differ with score: {}".format(score))
+            logger.info("Reference image: {}".format(filename_ref))
             log_screenshot_file(filepath_ref)
-            logger.info('Comparison image: {}'.format(filename_cmp))
+            logger.info("Comparison image: {}".format(filename_cmp))
             ref_image_c = _draw_contours(diff, ref_image_c)
 
             log_screenshot_file(filepath_cmp)
 
             filepath_dif = os.path.join(screenshot_dir, filename_dif)
             cv2.imwrite(filepath_dif, ref_image_c)
-            logger.info('Difference image: {}'.format(filename_dif))
+            logger.info("Difference image: {}".format(filename_dif))
             log_screenshot_file(filepath_dif)
             status = False
     return status
 
 
 def _draw_contours(diff: ndarray, ref_image_c: ndarray) -> ndarray:
     # pylint: disable=no-member
@@ -146,18 +149,20 @@
     for c in contours[index]:
         (x, y, w, h) = cv2.boundingRect(c)
         cv2.rectangle(ref_image_c, (x, y), ((x + w), (y + h)), (0, 0, 255), 2)
     return ref_image_c
 
 
 # pylint: disable=too-many-branches
-def save_screenshot(filename: str = 'screenshot_{}.png',
-                    folder: str = SCREEN_SHOT_DIR_NAME,
-                    pyautog: bool = False,
-                    fullpage: bool = False) -> str:
+def save_screenshot(
+    filename: str = "screenshot_{}.png",
+    folder: str = SCREEN_SHOT_DIR_NAME,
+    pyautog: bool = False,
+    fullpage: bool = False,
+) -> str:
     """Save screenshot of web page to a file.
 
     If robot framework is running then screenshots are saved to
     ${OUTPUT DIR}/screenshots. Otherwise the file is saved to current working
     directory. If there is no write access to cwd (jupyter in windows for example seems set cwd to
     system32) screenshot dir is set to operating systems temp directory.
 
@@ -175,34 +180,34 @@
     Returns
     -------
     str
         Filepath to the saved file.
     """
     test_name = None
     try:
-        robot_output = BuiltIn().get_variable_value('${OUTPUT DIR}')
-        test_name = BuiltIn().get_variable_value('${TEST NAME}')
+        robot_output = BuiltIn().get_variable_value("${OUTPUT DIR}")
+        test_name = BuiltIn().get_variable_value("${TEST NAME}")
         screen_shot_dir = os.path.join(robot_output, folder)
 
     except RobotNotRunningError:
         screen_shot_dir = os.path.join(os.getcwd(), folder)
 
         if not os.access(screen_shot_dir, os.W_OK):
             screen_shot_dir = os.path.join(gettempdir(), folder)
 
     if not os.path.isdir(screen_shot_dir):
         os.makedirs(screen_shot_dir)
 
-    if filename == 'screenshot_{}.png' and test_name is None:
+    if filename == "screenshot_{}.png" and test_name is None:
         filename = filename.format(uuid4())
 
-    elif filename == 'screenshot_{}.png':
+    elif filename == "screenshot_{}.png":
         name_with_underscores = str(test_name).replace(" ", "_")
         valid_name = _remove_invalid_chars(name_with_underscores)
-        filename = "screenshot-" + valid_name + "-{}".format(uuid4()) + '.png'
+        filename = "screenshot-" + valid_name + "-{}".format(uuid4()) + ".png"
 
     filepath = os.path.join(screen_shot_dir, filename)
 
     try:
         driver = browser.get_current_browser()
     except QWebDriverError:
         driver = None
@@ -212,33 +217,37 @@
         # try to remove image, needed for scrot > 0.9
         try:
             os.remove(filepath)
         except OSError:
             pass
 
         pyscreenshot(filepath)
-        logger.info('Saved screenshot to {}'.format(filepath))
+        logger.info("Saved screenshot to {}".format(filepath))
         return filepath
 
     if driver:
         saved: Union[str, bool]
         try:
-            browser_name = driver.capabilities['browserName']
+            browser_name = driver.capabilities["browserName"]
             if not fullpage:
                 saved = driver.save_screenshot(filepath)
             else:
                 saved = full_page_screenshot(driver, filepath, browser_name)
 
-        except (UnexpectedAlertPresentException, WebDriverException, QWebDriverError,
-                InvalidSessionIdException):
+        except (
+            UnexpectedAlertPresentException,
+            WebDriverException,
+            QWebDriverError,
+            InvalidSessionIdException,
+        ):
             saved = pyscreenshot(filepath)
         if not saved:
-            raise ValueError(f'Saving screenshot to {filepath} did not succeed.')
+            raise ValueError(f"Saving screenshot to {filepath} did not succeed.")
 
-    logger.info('Saved screenshot to {}'.format(filepath))
+    logger.info("Saved screenshot to {}".format(filepath))
     return filepath
 
 
 def log_screenshot_file(filepath: str) -> None:
     """Log screenshot file to robot framework log.
 
     Uses robot.utils.get_link_path to determine the relative path to the robot
@@ -246,90 +255,94 @@
 
     Parameters
     ----------
     filepath : str
         Filepath to the screenshot file.
     """
     try:
-        robot_output = BuiltIn().get_variable_value('${OUTPUT DIR}')
+        robot_output = BuiltIn().get_variable_value("${OUTPUT DIR}")
         if not config.get_config("OSScreenshots"):
-            logger.info('Current url is: {}'.format(get_url()))
+            logger.info("Current url is: {}".format(get_url()))
         link = get_link_path(filepath, robot_output)
         logger.info('<a href="{0}"><img src="{0}" width="800px"></a>'.format(link), html=True)
 
     except RobotNotRunningError:
         return
 
 
 def log_html() -> None:
     source_html_counter = 1
     url = get_url()
-    logger.info('Current url: {}'.format(url))
+    logger.info("Current url: {}".format(url))
     raw_html = get_source()
-    log_dir = BuiltIn().get_variable_value('${OUTPUT DIR}')
+    log_dir = BuiltIn().get_variable_value("${OUTPUT DIR}")
     filename = "source_{}.html".format(uuid4())
-    filepath = os.path.join(log_dir, 'screenshots', filename)
-    with open(filepath, 'w', encoding="utf-8") as htmlfile:
+    filepath = os.path.join(log_dir, "screenshots", filename)
+    with open(filepath, "w", encoding="utf-8") as htmlfile:
         htmlfile.write(raw_html)
-    logger.info(r'''<a id="source_link_{0}">{1}</a></br>
+    logger.info(
+        r"""<a id="source_link_{0}">{1}</a></br>
     <iframe id="source_{0}" width="1220px", height="650px"></iframe>
     <script type="text/javascript">
     element = document.getElementById("source_link_{0}");
     element.setAttribute("href", "{2}");
     document.getElementById("source_{0}").setAttribute("src", "{1}");
-    </script>'''.format(source_html_counter, 'screenshots/' + filename,
-                        filepath.replace("\\", "\\\\")),
-                html=True)
+    </script>""".format(
+            source_html_counter, "screenshots/" + filename, filepath.replace("\\", "\\\\")
+        ),
+        html=True,
+    )
     source_html_counter += 1
 
 
 def get_url() -> Optional[str]:
     try:
         driver = browser.get_current_browser()
         return driver.current_url
     except QWebDriverError:
-        logger.warn('Could not take a screenshot of browser because it is not open.')
+        logger.warn("Could not take a screenshot of browser because it is not open.")
         return None
 
 
 def get_source() -> str:
     driver = browser.get_current_browser()
     return driver.page_source
 
 
 def chromium_full_screenshot(driver: WebDriver, filepath: str) -> str:
-
     def send(cmd, params):
         resource = f"/session/{driver.session_id}/chromium/send_command_and_get_result"
 
         # pylint:disable=W0212
         url = driver.command_executor._url + resource
-        body = json.dumps({'cmd': cmd, 'params': params})
-        response = driver.command_executor._request('POST', url, body)
-        return response.get('value')
+        body = json.dumps({"cmd": cmd, "params": params})
+        response = driver.command_executor._request("POST", url, body)
+        return response.get("value")
 
     def evaluate(script):
-        response = send('Runtime.evaluate', {'returnByValue': True, 'expression': script})
-        return response['result']['value']
+        response = send("Runtime.evaluate", {"returnByValue": True, "expression": script})
+        return response["result"]["value"]
 
-    metrics = evaluate("({"
-                       "width: Math.max(window.innerWidth, "
-                       "document.body.scrollWidth, "
-                       "document.documentElement.scrollWidth)|0,"
-                       "height: Math.max(window.innerHeight, document.body.scrollHeight, "
-                       "document.documentElement.scrollHeight)|0,"
-                       "deviceScaleFactor: window.devicePixelRatio || 1,"
-                       "mobile: typeof window.orientation !== 'undefined'"
-                       "})")
-    send('Emulation.setDeviceMetricsOverride', metrics)
-    screenshot = send('Page.captureScreenshot', {'format': 'png', 'fromSurface': True})
-    send('Emulation.clearDeviceMetricsOverride', {})
+    metrics = evaluate(
+        "({"
+        "width: Math.max(window.innerWidth, "
+        "document.body.scrollWidth, "
+        "document.documentElement.scrollWidth)|0,"
+        "height: Math.max(window.innerHeight, document.body.scrollHeight, "
+        "document.documentElement.scrollHeight)|0,"
+        "deviceScaleFactor: window.devicePixelRatio || 1,"
+        "mobile: typeof window.orientation !== 'undefined'"
+        "})"
+    )
+    send("Emulation.setDeviceMetricsOverride", metrics)
+    screenshot = send("Page.captureScreenshot", {"format": "png", "fromSurface": True})
+    send("Emulation.clearDeviceMetricsOverride", {})
 
-    image = base64.b64decode(screenshot['data'])
-    with open(filepath, 'wb') as f:
+    image = base64.b64decode(screenshot["data"])
+    with open(filepath, "wb") as f:
         f.write(image)
 
     return filepath
 
 
 def full_page_screenshot(driver: WebDriver, filepath: str, browser_name: str) -> str:
     if browser_name in firefox.NAMES:
```

### Comparing `QWeb-3.2.1/QWeb/internal/search_strategy.py` & `QWeb-3.3.0/QWeb/internal/search_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 # pylint: disable=line-too-long
 import re
 import string
 
 
 class SearchStrategies:
-    ALL_INPUT_ELEMENTS: str = '//input[@type="text" or @type="email" or @type="password" or @type="tel"]|//textarea'
+    ALL_INPUT_ELEMENTS: str = (
+        '//input[@type="text" or @type="email" or @type="password" or @type="tel"]|//textarea'
+    )
 
     MATCHING_INPUT_ELEMENT: str = '//*[(self::input or self::textarea) and (normalize-space(@placeholder)="{0}" or normalize-space(@value)="{0}")]'
     CONTAINING_INPUT_ELEMENT: str = '//*[(self::input or self::textarea) and (contains(normalize-space(@placeholder),"{0}") or contains(normalize-space(@value),"{0}"))]'
 
     ACTIVE_AREA_XPATH: str = "//body"
 
     TEXT_MATCH: str = '//*[not(self::script) and normalize-space(translate(., "\u00a0", " "))="{0}" and not(descendant::*[normalize-space(translate(., "\u00a0", " "))="{0}"])]|//input[(@type="button" or @type="reset" or @type="submit" or @type="checkbox") and normalize-space(translate(@value, "\u00a0", " "))="{0}"]'
@@ -136,17 +138,15 @@
             # field_name '0' matches {0} etc.
             elif elem[1] and elem[1].isnumeric():
                 index_placeholders.add(int(elem[1]))
 
         # Position placeholders are in a set. They must start from zero
         # so that we have {0}'s, {1}'s etc.
         if index_placeholders:
-            continuous = SearchStrategies._continuous_set(
-                index_placeholders, placeholder_num
-            )
+            continuous = SearchStrategies._continuous_set(index_placeholders, placeholder_num)
 
         if placeholder_num != (empty_placeholders + len(index_placeholders)):
             raise ValueError(
                 "xpath has invalid number of placeholders, got {}, {}".format(
                     empty_placeholders, len(index_placeholders)
                 )
             )
```

### Comparing `QWeb-3.2.1/QWeb/internal/secrets.py` & `QWeb-3.3.0/QWeb/internal/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
-""" Robot framework secrets handling.
+"""Robot framework secrets handling.
 
-    In Robot FW logs following things may expose secrets:
-        - "start keyword" log item
-        - "end keyword" log item
-        - Logs printed out inside the keyword implementation
+In Robot FW logs following things may expose secrets:
+    - "start keyword" log item
+    - "end keyword" log item
+    - Logs printed out inside the keyword implementation
 
-    For "start keyword" and "end keyword" filtering is applied:
-    instead of plain parameter only "*****" is printed.
+For "start keyword" and "end keyword" filtering is applied:
+instead of plain parameter only "*****" is printed.
 
-    For other logging, logs will be disabled. This ensures there's
-    no secrets in XML or HTML files.
+For other logging, logs will be disabled. This ensures there's
+no secrets in XML or HTML files.
 
-    Following adds secrets filtering to a keyword function "type_secret":
-        from QWeb.internal import secrets
-        secrets.add_filter("Type Secret", 1)
+Following adds secrets filtering to a keyword function "type_secret":
+    from QWeb.internal import secrets
+    secrets.add_filter("Type Secret", 1)
 
-     Note the function name vs. name used in the add_filter.
+ Note the function name vs. name used in the add_filter.
 """
+
 from __future__ import annotations
 from typing import Any, Optional
 from robot.model.keyword import Keyword
 
 from robot.output.logger import LOGGER
 from robot.libraries.BuiltIn import BuiltIn
 
@@ -51,33 +52,32 @@
         return
 
     except AttributeError:
         # Robot Framework 4.0/5.0 has ModelCombiner object that fails with this
         pass
 
     # Update according to the ModelCombiner object interface
-    if hasattr(keyword.result, 'args'):
-        setattr(keyword.result, 'args', args)
-    if hasattr(keyword.data, 'args'):
-        setattr(keyword.data, 'args', args)
+    if hasattr(keyword.result, "args"):
+        setattr(keyword.result, "args", args)
+    if hasattr(keyword.data, "args"):
+        setattr(keyword.data, "args", args)
 
 
 def _hide_keyword_arg_values(keyword: Keyword) -> list[str]:
-    if hasattr(keyword, 'kwname'):
+    if hasattr(keyword, "kwname"):
         par_index, secret = filtered_keywords[keyword.kwname]
     else:  # rfw 7
         # name is in different format
-        kw_name = ''.join(
-            f' {char}' if char.isupper() else char.strip()
-            for char in keyword.name
+        kw_name = "".join(
+            f" {char}" if char.isupper() else char.strip() for char in keyword.name
         ).strip()
         par_index, secret = filtered_keywords[kw_name]
     censored_args = list(keyword.args)
-    if secret == 'hint':
-        censored_args[par_index] = 'SECRET'
+    if secret == "hint":
+        censored_args[par_index] = "SECRET"
     else:
         censored_args[par_index] = "*" * 5
 
     return censored_args
 
 
 def _filtered_start_keyword(keyword: Keyword) -> None:
@@ -99,15 +99,15 @@
     for start_logger in LOGGER.start_loggers:
         start_logger.start_keyword(keyword)
 
     if apply_filter:
         _replace_keyword_args(keyword, tuple(original_args))
         b = BuiltIn()
         # Disable logging and store previous log level
-        if 'INFO' not in b.get_variables()['${LOG_LEVEL}']:
+        if "INFO" not in b.get_variables()["${LOG_LEVEL}"]:
             log_level = b.set_log_level("INFO")
         if debugfile_log:
             LOGGER._other_loggers[0].log_message = lambda x: None
 
 
 def _filtered_start_library_keyword(data: Keyword, implementation: Keyword, result: Keyword):
     """Modify Robot FW 7+ internal function "start_library_keyword".
@@ -132,15 +132,15 @@
     for start_logger in LOGGER.start_loggers:
         start_logger.start_library_keyword(data, implementation, result)
 
     if apply_filter:
         _replace_keyword_args(data, tuple(original_args))
         b = BuiltIn()
         # Disable logging and store previous log level
-        if 'INFO' not in b.get_variables()['${LOG_LEVEL}']:
+        if "INFO" not in b.get_variables()["${LOG_LEVEL}"]:
             log_level = b.set_log_level("INFO")
         if debugfile_log:
             LOGGER._other_loggers[0].log_message = lambda x: None
 
 
 def _filtered_end_keyword(keyword: Keyword) -> None:
     """Modify Robot FW internal function "end_keyword".
@@ -220,15 +220,15 @@
 
 try:
     debugfile_log = LOGGER._other_loggers[0].log_message  # pylint: disable=protected-access
 except IndexError:
     debugfile_log = False
 
 # Monkey patch Robot FW methods
-rfw_major_version, *_ = BuiltIn.ROBOT_LIBRARY_VERSION.split('.', maxsplit=1)
+rfw_major_version, *_ = BuiltIn.ROBOT_LIBRARY_VERSION.split(".", maxsplit=1)
 rfw_major_version = int(rfw_major_version)
 if rfw_major_version < 7:
     LOGGER.start_keyword = _filtered_start_keyword
     LOGGER.end_keyword = _filtered_end_keyword
 else:
     LOGGER.start_library_keyword = _filtered_start_library_keyword
     LOGGER.end_library_keyword = _filtered_end_library_keyword
```

### Comparing `QWeb-3.2.1/QWeb/internal/table.py` & `QWeb-3.3.0/QWeb/internal/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,43 +25,46 @@
 from selenium.common.exceptions import StaleElementReferenceException, NoSuchElementException
 from QWeb.internal.exceptions import QWebElementNotFoundError, QWebValueError
 from QWeb.internal import element, text, javascript, frame, util
 from QWeb.internal.config_defaults import CONFIG
 
 
 class Table:
-
     ACTIVE_TABLE: Table = None  # type: ignore[assignment]
 
-    def __init__(self,
-                 table: WebElement,
-                 locator: str,
-                 anchor: str,
-                 parent: bool = False,
-                 child: bool = False,
-                 level: int = 1,
-                 index: int = 1) -> None:
+    def __init__(
+        self,
+        table: WebElement,
+        locator: str,
+        anchor: str,
+        parent: bool = False,
+        child: bool = False,
+        level: int = 1,
+        index: int = 1,
+    ) -> None:
         self.table = table
         self.locator = locator
         self.anchor = anchor
         self.parent = parent
         self.child = child
         self.level = level
         self.index = index
         Table.ACTIVE_TABLE = self
 
     @classmethod
     @frame.all_frames
-    def from_table_instance(cls,
-                            locator: str,
-                            anchor: str,
-                            parent: bool = False,
-                            child: bool = False,
-                            level: int = 1,
-                            index: int = 1) -> Table:
+    def from_table_instance(
+        cls,
+        locator: str,
+        anchor: str,
+        parent: bool = False,
+        child: bool = False,
+        level: int = 1,
+        index: int = 1,
+    ) -> Table:
         """Create table instance by finding table based on locator
 
         Parameters
         ----------
         locator : str
             Text that locates the table. The table that is closest
             to the text is selected. Also one can use xpath by adding xpath= prefix
@@ -75,46 +78,50 @@
         if CONFIG["CssSelectors"] and not util.xpath_validator(locator):
             table_element = cls.get_table_element_by_css(locator, anchor)
         else:
             table_element = cls.get_table_element(cls, locator, index)  # type: ignore[arg-type]
         if table_element is None:
             raise QWebElementNotFoundError("Could not find Table Element!")
         if not parent and not child:
-            if CONFIG['SearchMode']:
+            if CONFIG["SearchMode"]:
                 element.draw_borders(table_element)
             return Table(table_element, locator, anchor, parent, child, level, index)
         table_element = cls.get_table_by_locator_table(table_element, parent, child, level, index)
-        if CONFIG['SearchMode']:
+        if CONFIG["SearchMode"]:
             element.draw_borders(table_element)
         return Table(table_element, locator, anchor, parent, child, level, index)
 
     @staticmethod
-    def get_table_by_locator_table(locator: WebElement,
-                                   parent: bool = False,
-                                   child: bool = False,
-                                   level: int = 1,
-                                   index: int = 1) -> WebElement:
+    def get_table_by_locator_table(
+        locator: WebElement,
+        parent: bool = False,
+        child: bool = False,
+        level: int = 1,
+        index: int = 1,
+    ) -> WebElement:
         if parent:
             script = ".parentElement.closest('table')" * int(level)
-            parent_table = javascript.execute_javascript("return arguments[0]{}".format(script),
-                                                         locator)
+            parent_table = javascript.execute_javascript(
+                "return arguments[0]{}".format(script), locator
+            )
             if parent_table:
                 if not child:
                     return parent_table
                 locator = parent_table
             else:
-                raise QWebElementNotFoundError('No parent table found')
+                raise QWebElementNotFoundError("No parent table found")
         if child:
             script = ".querySelectorAll('table')[{}]".format(int(index) - 1)
-            child_table = javascript.execute_javascript("return arguments[0]{}".format(script),
-                                                        locator)
+            child_table = javascript.execute_javascript(
+                "return arguments[0]{}".format(script), locator
+            )
             if child_table:
                 return child_table
-            raise QWebElementNotFoundError('No child table found')
-        raise QWebElementNotFoundError('Sub/parent table not found')
+            raise QWebElementNotFoundError("No child table found")
+        raise QWebElementNotFoundError("Sub/parent table not found")
 
     def get_table_element(self, locator: str, anchor: str) -> WebElement:
         if util.xpath_validator(locator):
             index = util.anchor_to_index(anchor)
             table_element = element.get_unique_element_by_xpath(locator, index=index)
         else:  # Search using text
             table_xpath = "//*[text()= '{0}']/ancestor::table".format(locator)
@@ -125,230 +132,237 @@
                 locator_element = text.get_text_using_anchor(locator, anchor)
                 table_elements = self._get_all_table_elements()
                 table_element = element.get_closest_element(locator_element, table_elements)
             else:  # Found many
                 table_element = text.get_element_using_anchor(table_elements, anchor)
         if table_element:
             return table_element
-        raise QWebElementNotFoundError(f'Table element not found by locator {locator}')
+        raise QWebElementNotFoundError(f"Table element not found by locator {locator}")
 
     def get_table_cell(self, coordinates: str, anchor: str, **kwargs) -> WebElement:  # pylint: disable=unused-argument
         cell = None
         try:
-            if '/' in coordinates:
+            if "/" in coordinates:
                 cell = self.get_using_text_in_coordinates(coordinates, anchor, **kwargs)
             else:
                 row, column = self._convert_coordinates(coordinates)
                 try:
-                    cell = self.table.find_element(By.XPATH,
-                                                   './/tr[{0}]//td[{1}]'.format(row, column))
+                    cell = self.table.find_element(
+                        By.XPATH, ".//tr[{0}]//td[{1}]".format(row, column)
+                    )
                 except AttributeError as e:
-                    logger.debug(f'exception {e}')
+                    logger.debug(f"exception {e}")
                     self.update_table()
             if cell:
-                if CONFIG['SearchMode']:
+                if CONFIG["SearchMode"]:
                     element.draw_borders(cell)
                 return cell
         except (StaleElementReferenceException, NoSuchElementException) as e:
-            logger.debug(f'exception {e}')
+            logger.debug(f"exception {e}")
             self.update_table()
-        raise QWebElementNotFoundError(
-            f'Cell for coords {coordinates} not found after'
-        )
+        raise QWebElementNotFoundError(f"Cell for coords {coordinates} not found after")
 
-    def get_using_text_in_coordinates(self,
-                                      coordinates: str,
-                                      anchor: str,
-                                      **kwargs) -> WebElement:
+    def get_using_text_in_coordinates(self, coordinates: str, anchor: str, **kwargs) -> WebElement:
         row: Optional[int]
         column: Optional[int]
         row_elem = None
         cell = None
-        locator = coordinates.split('/')
-        if locator[0].startswith('r?'):
+        locator = coordinates.split("/")
+        if locator[0].startswith("r?"):
             row_elem = self.get_row(locator[0][2:], anchor)
         else:
             row, _ = self._convert_coordinates(locator[0])
-        if locator[1].startswith('c?'):
+        if locator[1].startswith("c?"):
             column = self.get_cell_by_locator(locator[1][2:], **kwargs)
         else:
             _, column = self._convert_coordinates(locator[1])
         if row_elem:
             cell = javascript.execute_javascript(
-                'return arguments[0].cells[{}]'.format(column - 1),  # type:ignore[operator]
-                row_elem)
+                "return arguments[0].cells[{}]".format(column - 1),  # type:ignore[operator]
+                row_elem,
+            )
         else:
-            cell = javascript.execute_javascript('return arguments[0].rows[{}].cells[{}]'.format(
-                row - 1, column - 1), self.table)  # type:ignore[operator]
+            cell = javascript.execute_javascript(
+                "return arguments[0].rows[{}].cells[{}]".format(row - 1, column - 1),  # type:ignore[operator] # pylint: disable=C0301
+                self.table,
+            )
         return cell
 
-    def get_clickable_cell(self,
-                           coordinates: str,
-                           anchor: str,
-                           index: int = 1,
-                           **kwargs) -> WebElement:
+    def get_clickable_cell(
+        self, coordinates: str, anchor: str, index: int = 1, **kwargs
+    ) -> WebElement:
         if int(index) < 1:
-            raise QWebValueError('Index should be greater than 0.')
+            raise QWebValueError("Index should be greater than 0.")
         table_cell = self.get_table_cell(coordinates, anchor, **kwargs)
-        if 'tag' in kwargs:
-            clickable_child = element.get_element_from_childnodes(table_cell,
-                                                                  str(kwargs.get('tag')),
-                                                                  dom_traversing=False)
+        if "tag" in kwargs:
+            clickable_child = element.get_element_from_childnodes(
+                table_cell, str(kwargs.get("tag")), dom_traversing=False
+            )
             if int(index) > len(clickable_child):
-                raise QWebValueError('Index exceeds the number of clickable elements in cell.')
+                raise QWebValueError("Index exceeds the number of clickable elements in cell.")
             return clickable_child[int(index) - 1]
         return table_cell
 
     def get_cell_by_locator(self, locator: str, **kwargs) -> int:
-        partial_match = util.par2bool(kwargs.get('partial_match', CONFIG['PartialMatch']))
+        partial_match = util.par2bool(kwargs.get("partial_match", CONFIG["PartialMatch"]))
         rows = self.get_all_rows()
         for i, r in enumerate(rows):  # pylint: disable=unused-variable
             cells = self.get_cells_from_row(r)
             for index, c in enumerate(cells):
                 cell_text = ""
                 if c.text:
                     cell_text += c.text
                 elif javascript.execute_javascript(
-                        'return arguments[0].querySelector("input, textarea")', c):
-                    value = javascript.execute_javascript('return arguments[0].value', c)
+                    'return arguments[0].querySelector("input, textarea")', c
+                ):
+                    value = javascript.execute_javascript("return arguments[0].value", c)
                     if value:
                         cell_text += str(value)
                 if partial_match:
                     if locator in cell_text:
                         return index + 1
                 else:
                     if locator == cell_text:
                         return index + 1
-        raise QWebValueError(f'Matching table cell not found for locator {locator}.')
+        raise QWebValueError(f"Matching table cell not found for locator {locator}.")
 
-    def get_row(self, locator: str, anchor: str, row_index: bool = False, **kwargs
-                ) -> Union[WebElement, int]:
-        skip_header = util.par2bool(kwargs.get('skip_header', False))
+    def get_row(
+        self, locator: str, anchor: str, row_index: bool = False, **kwargs
+    ) -> Union[WebElement, int]:
+        skip_header = util.par2bool(kwargs.get("skip_header", False))
         rows = self.get_all_rows()
-        if locator.startswith('//last'):
+        if locator.startswith("//last"):
             if skip_header:
                 return len(rows) - 1
             return len(rows)
         matches, index = self._get_row_by_locator_text(rows, locator, anchor)
         if row_index:
             if skip_header:
                 return index
             return index + 1
         if matches:
             return matches
-        raise QWebValueError(f'Matching table row not found for locator {locator}.')
+        raise QWebValueError(f"Matching table row not found for locator {locator}.")
 
     def get_all_rows(self) -> list[WebElement]:
-        return javascript.execute_javascript('return arguments[0].rows', self.table)
+        return javascript.execute_javascript("return arguments[0].rows", self.table)
 
     @staticmethod
     def get_cells_from_row(row: WebElement) -> list[WebElement]:
-        return javascript.execute_javascript('return arguments[0].cells', row)
+        return javascript.execute_javascript("return arguments[0].cells", row)
 
     @staticmethod
-    def _get_row_by_locator_text(rows: list[WebElement], locator: str,
-                                 anchor: Union[str, int]) -> tuple[WebElement, int]:
+    def _get_row_by_locator_text(
+        rows: list[WebElement], locator: str, anchor: Union[str, int]
+    ) -> tuple[WebElement, int]:
         matches = []
         input_elements = []
         row_index = []
         anchor_text = ""
         try:
             anchor = int(anchor) - 1
         except ValueError:
             anchor_text = str(anchor)
         for index, row in enumerate(rows):
             row_content = row.text
-            if locator == 'EMPTY' and row_content.strip() == '':
+            if locator == "EMPTY" and row_content.strip() == "":
                 return row, index
             input_elements = javascript.execute_javascript(
-                'return arguments[0].querySelectorAll("input, textarea")', row)
+                'return arguments[0].querySelectorAll("input, textarea")', row
+            )
             for elem in input_elements:
-                row_content += str(javascript.execute_javascript('return arguments[0].value', elem))
+                row_content += str(javascript.execute_javascript("return arguments[0].value", elem))
             if locator in row_content:
                 if anchor_text and anchor_text in row_content:
                     return row, index
                 row_index.append(index)
                 matches.append(row)
         if matches and not anchor_text:
             return matches[int(anchor)], row_index[int(anchor)]
         raise QWebElementNotFoundError(
-            f'Row that includes texts {locator} and {anchor_text} not found'
+            f"Row that includes texts {locator} and {anchor_text} not found"
         )
 
     def _convert_coordinates(self, coordinate_str: str) -> tuple[Optional[int], Optional[int]]:
         """Return row and column from coordinate string."""
         try:
-            row = int(re.findall('r([+-]?[0-9]+)', coordinate_str)[0])
+            row = int(re.findall("r([+-]?[0-9]+)", coordinate_str)[0])
             if row < 0:
-                last_row = self.get_row('//last', self.anchor)
+                last_row = self.get_row("//last", self.anchor)
                 if isinstance(last_row, int):
                     row = last_row + (row + 1)
         except IndexError:
             row = None
         try:
-            col = int(re.findall('c([+-]?[0-9]+)', coordinate_str)[0])
+            col = int(re.findall("c([+-]?[0-9]+)", coordinate_str)[0])
             if col < 0:
                 row_index = row - 1  # type: ignore[operator]
                 col = int(
                     javascript.execute_javascript(
-                        ' return arguments[0].rows[{0}].cells.length'.format(row_index),
-                        self.table)) + (col + 1)
+                        " return arguments[0].rows[{0}].cells.length".format(row_index), self.table
+                    )
+                ) + (col + 1)
         except IndexError:
             col = None
         return row, col
 
     @staticmethod
     def get_table_element_by_css(locator: str, anchor: Union[str, int]) -> Optional[WebElement]:
         table_element = javascript.execute_javascript(
             'return document.querySelectorAll(\'table[summary^="{0}"], '
             'table[name^="{0}"], table[title^="{0}"], th[title^="{0}"], '
-            'tr[title^="{0}"], td[title^="{0}"]\')'.format(locator))
+            'tr[title^="{0}"], td[title^="{0}"]\')'.format(locator)
+        )
         if table_element:
             try:
                 anchor = int(anchor) - 1
-                if table_element[int(anchor)].tag_name == 'table':
+                if table_element[int(anchor)].tag_name == "table":
                     return table_element[int(anchor)]
                 table_element = javascript.execute_javascript(
-                    'return arguments[0].closest("table")', table_element[anchor])
+                    'return arguments[0].closest("table")', table_element[anchor]
+                )
                 return table_element
             except (ValueError, TypeError):
                 raise IndexError(  # pylint: disable=W0707
-                    'Element found by it\'s attribute. When using CSS Selectors'
-                    ' for finding table, anchor has to be index when anchor is not '
-                    'related to separate locator element')
+                    "Element found by it's attribute. When using CSS Selectors"
+                    " for finding table, anchor has to be index when anchor is not "
+                    "related to separate locator element"
+                )
             except StaleElementReferenceException:
-                logger.debug('Staling element..Retrying')
+                logger.debug("Staling element..Retrying")
                 return None
         try:
             locator_element = text.get_text_using_anchor(locator, str(anchor))
-            table_element = javascript.execute_javascript('return arguments[0].closest("table")',
-                                                          locator_element)
+            table_element = javascript.execute_javascript(
+                'return arguments[0].closest("table")', locator_element
+            )
         except (ValueError, NoSuchElementException, StaleElementReferenceException):
             return None
         if table_element:
             return table_element
         return None
 
     @staticmethod
     def _get_all_table_elements() -> list[WebElement]:
-        return element.get_webelements_in_active_area('//table')
+        return element.get_webelements_in_active_area("//table")
 
     @staticmethod
     def is_table_coordinates(locator: str) -> bool:
-        if '/' in locator:
-            parts = locator.split('/')
-            if parts[0].startswith('r') and parts[1].startswith('c'):
+        if "/" in locator:
+            parts = locator.split("/")
+            if parts[0].startswith("r") and parts[1].startswith("c"):
                 return True
         elif fnmatch.fnmatch(locator, "r[-0-9]*c[-0-9]*"):
             return True
         return False
 
     def update_table(self) -> Table:
-        table = self.from_table_instance(self.locator, self.anchor, self.parent, self.child,
-                                         self.level, self.index)
+        table = self.from_table_instance(
+            self.locator, self.anchor, self.parent, self.child, self.level, self.index
+        )
         return table
 
     def get_columns(self) -> list[WebElement]:
         js = """var columns = function(tableRef){
                     var columnCount = 0;
                     var headers = [];
```

### Comparing `QWeb-3.2.1/QWeb/internal/text.py` & `QWeb-3.3.0/QWeb/internal/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,94 +15,106 @@
 # limitations under the License.
 # ---------------------------
 from __future__ import annotations
 from typing import Optional, Union
 from selenium.webdriver.remote.webelement import WebElement
 
 from selenium.webdriver.common.by import By
-from selenium.common.exceptions import InvalidSelectorException, JavascriptException, \
-    WebDriverException, NoSuchFrameException, NoSuchElementException
+from selenium.common.exceptions import (
+    InvalidSelectorException,
+    JavascriptException,
+    WebDriverException,
+    NoSuchFrameException,
+    NoSuchElementException,
+)
 from robot.api import logger
 from QWeb.internal import element, javascript, frame, util, browser
-from QWeb.internal.exceptions import QWebElementNotFoundError, QWebValueError, \
-    QWebInstanceDoesNotExistError, QWebStalingElementError
+from QWeb.internal.exceptions import (
+    QWebElementNotFoundError,
+    QWebValueError,
+    QWebInstanceDoesNotExistError,
+    QWebStalingElementError,
+)
 from QWeb.internal.config_defaults import CONFIG
 from QWeb.internal.search_strategy import SearchStrategies
 
 
-def get_element_by_locator_text(locator: str,
-                                anchor: str = "1",
-                                index: Union[int, str] = 1,
-                                **kwargs) -> Optional[WebElement]:
+def get_element_by_locator_text(
+    locator: str, anchor: str = "1", index: Union[int, str] = 1, **kwargs
+) -> Optional[WebElement]:
     """Find element by it's visible text.
 
     Accepted kwargs:
         parent(tagName):Can be used when target element is some of the locators parent.
         child(tagName): Find clickable target from locator's child elements.
         allow_non_existent = True: Function returns immediately if element is not found
         css=False: Use this to bypass css search when finding elements by visible text
     """
     index = int(index) - 1
     try:
         web_element = get_text_using_anchor(locator, anchor, **kwargs)
-    except (QWebElementNotFoundError, InvalidSelectorException, JavascriptException,
-            WebDriverException):
+    except (
+        QWebElementNotFoundError,
+        InvalidSelectorException,
+        JavascriptException,
+        WebDriverException,
+    ):
         try:
             web_element = element.get_unique_element_by_xpath(locator, index=index)
         except (QWebElementNotFoundError, InvalidSelectorException, NoSuchFrameException) as e:
-            no_raise = util.par2bool(kwargs.get('allow_non_existent', False))
+            no_raise = util.par2bool(kwargs.get("allow_non_existent", False))
             if no_raise:
                 return None
             raise QWebElementNotFoundError(e) from e
     if web_element:
-        if 'parent' in kwargs and kwargs['parent']:
-            tag_name = kwargs['parent']
+        if "parent" in kwargs and kwargs["parent"]:
+            tag_name = kwargs["parent"]
             web_element = element.get_parent_element(web_element, tag_name)
-        elif 'child' in kwargs and kwargs['child']:
-            tag_name = kwargs['child']
-            web_element = element.get_element_from_childnodes(web_element,
-                                                              tag_name,
-                                                              dom_traversing=False)[int(index)]
-        if CONFIG['SearchMode']:
+        elif "child" in kwargs and kwargs["child"]:
+            tag_name = kwargs["child"]
+            web_element = element.get_element_from_childnodes(
+                web_element, tag_name, dom_traversing=False
+            )[int(index)]
+        if CONFIG["SearchMode"]:
             element.draw_borders(web_element)
         return web_element
-    raise QWebElementNotFoundError('Element not found')
+    raise QWebElementNotFoundError("Element not found")
 
 
 @frame.all_frames
 def find_text(text: str) -> bool:
     try:
-        if javascript.execute_javascript("return window.find('{}')".format(text.replace(
-                "\'", "\\'"))):
+        if javascript.execute_javascript(
+            "return window.find('{}')".format(text.replace("'", "\\'"))
+        ):
             return True
     except WebDriverException as e:
-        logger.debug('Got webdriver exception from find text func: {}'.format(e))
-    raise QWebElementNotFoundError('Text not found')
+        logger.debug("Got webdriver exception from find text func: {}".format(e))
+    raise QWebElementNotFoundError("Text not found")
 
 
 def get_text_elements(text: str, **kwargs) -> Optional[list[WebElement]]:
     web_elements: Optional[list[WebElement]]
     try:
         web_elements = _get_exact_text_element(text, **kwargs)
     except NoSuchFrameException:
-        logger.debug('Got no such frame from get exact text')
-    partial = util.par2bool(kwargs.get('partial_match', CONFIG['PartialMatch']))
+        logger.debug("Got no such frame from get exact text")
+    partial = util.par2bool(kwargs.get("partial_match", CONFIG["PartialMatch"]))
     if partial:
         try:
             web_elements = _get_contains_text_element(text, **kwargs)
         except NoSuchFrameException:
-            logger.debug('Got no such frame from contains text')
-    shadow_dom = CONFIG['ShadowDOM']
+            logger.debug("Got no such frame from contains text")
+    shadow_dom = CONFIG["ShadowDOM"]
     if shadow_dom:
         shadow_elements = get_texts_including_shadow_dom(text, partial, **kwargs)
         # remove possible stale elements
         web_elements = util.remove_stale_elements(web_elements)  # type: ignore
         # remove duplicates
-        web_elements = util.remove_duplicates_from_list(shadow_elements,
-                                                        web_elements)  # type: ignore
+        web_elements = util.remove_duplicates_from_list(shadow_elements, web_elements)  # type: ignore # pylint: disable=C0301
     return web_elements
 
 
 def get_unique_text_element(text: str, **kwargs) -> WebElement:
     """Get element with text that is unique.
 
     First tries to find exact match and if not found then search as a
@@ -126,46 +138,56 @@
         Found many elements with the given text.
     """
     web_elements = get_text_elements(text, **kwargs)
     if not web_elements:
         raise QWebValueError('Text "{}" did not match any elements'.format(text))
     if len(web_elements) == 1:
         return web_elements[0]  # pylint: disable=unsubscriptable-object
-    raise QWebValueError('Text "{}" matched {} elements. Needs to be unique'.format(
-        text, len(web_elements)))
+    raise QWebValueError(
+        'Text "{}" matched {} elements. Needs to be unique'.format(text, len(web_elements))
+    )
 
 
 @frame.all_frames
 def check_all_nodes(text: str, **kwargs) -> Optional[list[WebElement]]:
     try:
         return element.get_visible_elements_from_elements(
-            javascript.find_text_from_textnodes(text, **kwargs))
-    except (WebDriverException, NoSuchFrameException, JavascriptException,
-            QWebStalingElementError) as e:
-        logger.info('Got {} from check all nodes'.format(e))
+            javascript.find_text_from_textnodes(text, **kwargs)
+        )
+    except (
+        WebDriverException,
+        NoSuchFrameException,
+        JavascriptException,
+        QWebStalingElementError,
+    ) as e:
+        logger.info("Got {} from check all nodes".format(e))
         return None
 
 
 def get_all_text_elements(text: str, **kwargs) -> list[WebElement]:
     """Get all webelements found by text"""
     web_elements: list[WebElement] = []
-    shadow_dom = CONFIG['ShadowDOM']
-    all_text_nodes = util.par2bool(kwargs.get('all_text_nodes', CONFIG['AllTextNodes']))
-    kwargs['partial_match'] = kwargs.get('partial_match', CONFIG['PartialMatch'])
+    shadow_dom = CONFIG["ShadowDOM"]
+    all_text_nodes = util.par2bool(kwargs.get("all_text_nodes", CONFIG["AllTextNodes"]))
+    kwargs["partial_match"] = kwargs.get("partial_match", CONFIG["PartialMatch"])
     if all_text_nodes:
         web_elements = check_all_nodes(text, **kwargs)
         if web_elements:
             return web_elements
 
-    if 'css' not in kwargs:
+    if "css" not in kwargs:
         try:
             web_elements = get_clickable_element_by_js(text, shadow_dom=shadow_dom, **kwargs)
-        except (JavascriptException, WebDriverException, NoSuchFrameException,
-                QWebStalingElementError) as e:
-            logger.debug('got {}. Syntax might be invalid'.format(e))
+        except (
+            JavascriptException,
+            WebDriverException,
+            NoSuchFrameException,
+            QWebStalingElementError,
+        ) as e:
+            logger.debug("got {}. Syntax might be invalid".format(e))
     if not web_elements:
         # shadow dom search for all texts is done inside get_text_elements
         web_elements = get_text_elements(text, **kwargs)  # type: ignore[assignment]
     if not web_elements:
         raise QWebElementNotFoundError('Webpage did not contain text "{}"'.format(text))
     return web_elements
 
@@ -206,31 +228,31 @@
         return web_elements[0]
     # Found many elements, use anchors to determine correct element
     correct_element = get_element_using_anchor(web_elements, anchor, **kwargs)
     return correct_element
 
 
 def _get_exact_text_element(text: str, **kwargs) -> Optional[list[WebElement]]:
-    xpath = (CONFIG["TextMatch"].replace('"{0}"', util.escape_xpath_quotes(text)))
+    xpath = CONFIG["TextMatch"].replace('"{0}"', util.escape_xpath_quotes(text))
     return element.get_webelements_in_active_area(xpath, **kwargs)
 
 
 def _get_contains_text_element(text: str, **kwargs) -> list[WebElement]:
-    xpath = (CONFIG["ContainingTextMatch"].replace('"{0}"', util.escape_xpath_quotes(text)))
+    xpath = CONFIG["ContainingTextMatch"].replace('"{0}"', util.escape_xpath_quotes(text))
     return element.get_webelements_in_active_area(xpath, **kwargs)
 
 
 def filter_by_modal_ancestor(elements: list[WebElement]) -> list[WebElement]:
     xpath = CONFIG["IsModalXpath"]
     if xpath.startswith("xpath="):
         xpath = xpath.split("=", 1)[1]
     if xpath.startswith("//"):
         xpath = xpath[2:]
 
-    modal_xpath = CONFIG['IsModalXpath']
+    modal_xpath = CONFIG["IsModalXpath"]
     driver = browser.get_current_browser()
     # no filtering if modal setting is the default one
     if modal_xpath == SearchStrategies.IS_MODAL_XPATH:
         return elements
 
     # filter elements by modal (dialog etc)
     logger.debug("IsModalXpath filtering on, filtering...")
@@ -250,105 +272,112 @@
             logger.debug("Filtering out element, modal open but not under modal")
             continue
 
     logger.debug(f"length after filtering: {len(elems_in_modal)}")
     return elems_in_modal
 
 
-def get_element_using_anchor(elements: list[WebElement], anchor: Optional[Union[str, int]],
-                             **kwargs) -> WebElement:
+def get_element_using_anchor(
+    elements: list[WebElement], anchor: Optional[Union[str, int]], **kwargs
+) -> WebElement:
     """Determine correct element from list of elements using anchor.
 
     Parameters
     ----------
     elements : :obj:`list` of :obj:`WebElement`
     anchor
 
     Returns
     -------
     WebElement
     """
     if anchor is None:
         # Element was not unique and anchor was not used.
-        raise QWebValueError('Found {} elements. Use anchor to determine which is wanted'.format(
-            len(elements)))
+        raise QWebValueError(
+            "Found {} elements. Use anchor to determine which is wanted".format(len(elements))
+        )
     # Select by index unless anchor type is text
     if str(anchor).isdigit() and kwargs.get("anchor_type", "auto").lower() != "text":
         anchor_int = int(anchor) - 1
         if anchor_int < len(elements):
             return elements[anchor_int]
-        raise QWebInstanceDoesNotExistError('Found {} elements. Given anchor was {}'.format(
-            len(elements), anchor_int + 1))
+        raise QWebInstanceDoesNotExistError(
+            "Found {} elements. Given anchor was {}".format(len(elements), anchor_int + 1)
+        )
     if isinstance(anchor, str):  # Get closest element to anchor
-        kwargs['stay_in_current_frame'] = True
+        kwargs["stay_in_current_frame"] = True
         anchor_element: Optional[WebElement]
-        if CONFIG['MultipleAnchors']:
+        if CONFIG["MultipleAnchors"]:
             anchor_elements: list[WebElement] = []
-            logger.debug('Multiple anchors enabled, trying to find first exact match')
+            logger.debug("Multiple anchors enabled, trying to find first exact match")
             try:
                 anchor_elements = _get_exact_text_element(  # type: ignore[assignment]
-                    anchor, **kwargs)
+                    anchor, **kwargs
+                )
             except NoSuchFrameException:
-                logger.debug('Got no such frame from get exact text')
+                logger.debug("Got no such frame from get exact text")
             if len(anchor_elements) > 0:
                 # Using first exact match as anchor
 
                 # We need to return the element that has the text, not parent
-                anchor_element = _get_anchor_with_inner_text(anchor_elements,
-                                                             anchor,
-                                                             exact_match=True)
+                anchor_element = _get_anchor_with_inner_text(
+                    anchor_elements, anchor, exact_match=True
+                )
                 anchor_element = anchor_element or anchor_elements[0]
             else:
                 # No exact matches found, trying to find partial
                 anchor_elements = get_text_elements(  # type: ignore[assignment]
-                    anchor, **kwargs)
+                    anchor, **kwargs
+                )
                 if len(anchor_elements) > 0:
-                    logger.debug('No exact match found, using first partial match')
+                    logger.debug("No exact match found, using first partial match")
                     # We need to return the element that includes the text, not parent
-                    anchor_element = _get_anchor_with_inner_text(anchor_elements,
-                                                                 anchor,
-                                                                 exact_match=False)
+                    anchor_element = _get_anchor_with_inner_text(
+                        anchor_elements, anchor, exact_match=False
+                    )
 
                     anchor_element = anchor_element or anchor_elements[0]
                 else:
                     raise QWebElementNotFoundError(f"Could not find elements for anchor: {anchor}")
         else:
             anchor_element = get_unique_text_element(anchor, **kwargs)
         return element.get_closest_element(anchor_element, elements)
     raise TypeError("Unknown argument type {}".format(type(anchor)))
 
 
 def get_item_using_anchor(text: str, anchor: str, **kwargs) -> Optional[WebElement]:
-    xpath = '//*[@title="{0}" or @alt="{0}" or @data-tooltip="{0}" or ' \
-            '@tooltip="{0}" or @aria-label="{0}" or @data-icon="{0}"]'.format(text)
+    xpath = (
+        '//*[@title="{0}" or @alt="{0}" or @data-tooltip="{0}" or '
+        '@tooltip="{0}" or @aria-label="{0}" or @data-icon="{0}"]'.format(text)
+    )
     if CONFIG["CssSelectors"]:
         web_elements = _get_item_by_css(text, **kwargs)
     else:
         web_elements = element.get_webelements(xpath, **kwargs)
     # extend search to Shadow DOM
-    shadow_dom = CONFIG['ShadowDOM']
+    shadow_dom = CONFIG["ShadowDOM"]
     if shadow_dom:
-        tag = kwargs.get('tag', None)
+        tag = kwargs.get("tag", None)
         elements = get_items_including_shadow_dom(text, tag)
 
         if web_elements:
             for el in elements:
                 if el not in list(web_elements):
                     web_elements.append(el)
         else:
             web_elements = elements
     if web_elements:
         correct = _get_correct_element(web_elements, str(anchor), **kwargs)
-        if CONFIG['SearchMode']:
+        if CONFIG["SearchMode"]:
             element.draw_borders(correct)
         return correct
-    no_raise = util.par2bool(kwargs.get('allow_non_existent', False))
+    no_raise = util.par2bool(kwargs.get("allow_non_existent", False))
     if no_raise:
         return None
-    raise QWebElementNotFoundError('Cannot find item for locator {}'.format(text))
+    raise QWebElementNotFoundError("Cannot find item for locator {}".format(text))
 
 
 def _get_correct_element(web_elements: list[WebElement], anchor: str, **kwargs) -> WebElement:
     if len(web_elements) == 1:
         return web_elements[0]
     correct_element = get_element_using_anchor(web_elements, anchor, **kwargs)
     return correct_element
@@ -358,28 +387,30 @@
     """
     Allows partial match. Anchor has to be number.
     :param text: str
         Attribute value of the element
     :return:
         webelement that containing attribute with given value
     """
-    if 'partial_match' not in kwargs:
-        kwargs['partial_match'] = True
-    css = 'a, span, img, li, h1, h2, h3, h4, h5, h6, div, svg, p, button, input' \
-          ':not([type="text"]):not([type="password"]):not([type="email"])'
+    if "partial_match" not in kwargs:
+        kwargs["partial_match"] = True
+    css = (
+        "a, span, img, li, h1, h2, h3, h4, h5, h6, div, svg, p, button, input"
+        ':not([type="text"]):not([type="password"]):not([type="email"])'
+    )
     full, partial = element.get_elements_by_attributes(css, text, **kwargs)
     web_elements = element.get_visible_elements_from_elements(full + partial, **kwargs)
     if web_elements:
         return web_elements
     return None
 
 
-def _get_anchor_with_inner_text(anchor_elements: list[WebElement],
-                                anchor: str,
-                                exact_match: bool = True) -> Optional[WebElement]:
+def _get_anchor_with_inner_text(
+    anchor_elements: list[WebElement], anchor: str, exact_match: bool = True
+) -> Optional[WebElement]:
     """
     Finds the appropriate anchor element containing the given text in innertext based on
     whether we are searching for an exact match or partial match.
 
     Parameters:
     - anchor_elements: List[WebElement], a list of WebElement objects to search through.
     - anchor: str, the text to match against the element's innerText.
@@ -393,43 +424,47 @@
         inner_text = el.get_attribute("innerText") or ""
         if (exact_match and anchor == inner_text) or (not exact_match and anchor in inner_text):
             return el
     return None
 
 
 @frame.all_frames
-def get_clickable_element_by_js(locator: str,
-                                shadow_dom: bool = False,
-                                **kwargs) -> Optional[list[WebElement]]:
-    partial = kwargs['partial_match']
+def get_clickable_element_by_js(
+    locator: str, shadow_dom: bool = False, **kwargs
+) -> Optional[list[WebElement]]:
+    partial = kwargs["partial_match"]
     if shadow_dom:
         web_elements = element.get_visible_elements_from_elements(
-                       javascript.get_clickable_from_shadow_dom(locator, partial))
+            javascript.get_clickable_from_shadow_dom(locator, partial)
+        )
     else:
-        web_elements = element.get_visible_elements_from_elements(javascript.get_clickable(
-                                                                  locator), **kwargs)
+        web_elements = element.get_visible_elements_from_elements(
+            javascript.get_clickable(locator), **kwargs
+        )
     if web_elements:
-        logger.debug('Found elements by js: {}'.format(web_elements))
+        logger.debug("Found elements by js: {}".format(web_elements))
         return web_elements
     return None
 
 
 @frame.all_frames
 def get_texts_including_shadow_dom(locator: str, partial: bool, **kwargs) -> list[WebElement]:
     web_elements = element.get_visible_elements_from_elements(
-        javascript.get_text_elements_from_shadow_dom(locator, partial), **kwargs)
+        javascript.get_text_elements_from_shadow_dom(locator, partial), **kwargs
+    )
     if web_elements:
-        logger.debug('Found elements from shadow dom: {}'.format(web_elements))
+        logger.debug("Found elements from shadow dom: {}".format(web_elements))
     return web_elements
 
 
 @frame.all_frames
 def get_items_including_shadow_dom(text: str, tag: str, **kwargs) -> list[WebElement]:
     web_elements = element.get_visible_elements_from_elements(
-        javascript.get_item_elements_from_shadow_dom(tag), **kwargs)
+        javascript.get_item_elements_from_shadow_dom(tag), **kwargs
+    )
 
     matches = javascript.get_by_attributes(web_elements, text, False)
-    full, partial = matches.get('full', []), matches.get('partial', [])
+    full, partial = matches.get("full", []), matches.get("partial", [])
     shadow_elements = full + partial
     if shadow_elements:
-        logger.debug(f'Found {len(shadow_elements)} items when extending search to shadow dom')
+        logger.debug(f"Found {len(shadow_elements)} items when extending search to shadow dom")
     return shadow_elements
```

### Comparing `QWeb-3.2.1/QWeb/internal/user.py` & `QWeb-3.3.0/QWeb/internal/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,12 +28,13 @@
     # User id 0 is reserved for superuser aka root
     if uid == 0:
         return True
     return False
 
 
 def is_docker() -> bool:
-    path = '/proc/self/cgroup'
-    return (os.path.exists('/.dockerenv')
-            or os.path.isfile(path) and any('docker' in line
-                                            for line in open(path))  # noqa: W503,W1514
-            )
+    path = "/proc/self/cgroup"
+    return (
+        os.path.exists("/.dockerenv")
+        or os.path.isfile(path)
+        and any("docker" in line for line in open(path))  # noqa: W503,W1514
+    )
```

### Comparing `QWeb-3.2.1/QWeb/internal/util.py` & `QWeb-3.3.0/QWeb/internal/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,34 +38,33 @@
     """
     if isinstance(s, str):
         s = s.lower()
     return s in ["true", "1", "on", True, 1]
 
 
 def xpath_validator(locator: str) -> bool:
-    """Checks if given locator is an xpath and returns boolean (True, False)
-    """
+    """Checks if given locator is an xpath and returns boolean (True, False)"""
     # TODO: Make this more reliable
-    if locator.lower().startswith(('xpath=', '/html', '//')):
+    if locator.lower().startswith(("xpath=", "/html", "//")):
         return True
     return False
 
 
 def url_validator(url: str) -> bool:
-    """Checks if given url is valid and returns boolean (True, False)
-    """
+    """Checks if given url is valid and returns boolean (True, False)"""
     regex = re.compile(
         # Django url validation regex
-        r'^(?:http|ftp)s?://'
-        r'(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|'
-        r'localhost|'
-        r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'
-        r'(?::\d+)?'
-        r'(?:/?|[/?]\S+)$',
-        re.IGNORECASE)
+        r"^(?:http|ftp)s?://"
+        r"(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|"
+        r"localhost|"
+        r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"
+        r"(?::\d+)?"
+        r"(?:/?|[/?]\S+)$",
+        re.IGNORECASE,
+    )
     return re.match(regex, url) is not None
 
 
 def calculate_interval(timeout_int: int) -> float:
     """Calculates interval based on timeout.
 
     Some customers require long timeouts and polling every 0.1s results
@@ -85,108 +84,122 @@
     width = int(width_str)
     height = int(height_str)
     driver = browser.get_current_browser()
     driver.set_window_size(width, height)
     return width, height
 
 
-def _parse_pixels(pixels: str, split: str = 'x') -> tuple[str, str]:
+def _parse_pixels(pixels: str, split: str = "x") -> tuple[str, str]:
     pixel_list = pixels.lower().split(split)
     if len(pixel_list) == 1:
         raise ValueError("Pixels needs to be given with '1920x1080' syntax")
     return pixel_list[0], pixel_list[1]
 
 
 def set_input_handler(input_method: str) -> str:
     input_handler.input_method = input_method.lower()
     return input_method.lower()
 
 
 def get_emulation_pref(device_or_dimension: str) -> dict[str, Any]:
     """Sets correct mobile emulation option string based on given input
-     (existing device profile name or screen dimensions).
+    (existing device profile name or screen dimensions).
     """
     try:
         width_str, height_str = _parse_pixels(device_or_dimension)
         return {"deviceMetrics": {"width": int(width_str), "height": int(height_str)}}
     except ValueError:
         return {"deviceName": device_or_dimension}
 
 
 def set_line_break(key: str) -> str:
-    if key == '\ue000':
-        current_browser = browser.get_current_browser().capabilities['browserName']
-        if current_browser == 'firefox':
-            key = ''
+    if key == "\ue000":
+        current_browser = browser.get_current_browser().capabilities["browserName"]
+        if current_browser == "firefox":
+            key = ""
             input_handler.line_break_key = key
-            logger.info('\n\\ue000 line break does not work with Firefox, using empty string'
-                        ' instead. It is recommended to use None instead of \\ue000.')
+            logger.info(
+                "\n\\ue000 line break does not work with Firefox, using empty string"
+                " instead. It is recommended to use None instead of \\ue000."
+            )
         else:
             input_handler.line_break_key = key
-    elif key.lower() in ('none', 'empty', 'null'):
-        key = ''
+    elif key.lower() in ("none", "empty", "null"):
+        key = ""
         input_handler.line_break_key = key
     else:
         input_handler.line_break_key = key
     return key
 
 
 def set_clear_key(key: str) -> Optional[str]:
-    if key.lower() == 'none':
+    if key.lower() == "none":
         input_handler.clear_key = None
     else:
         input_handler.clear_key = key
     return input_handler.clear_key
 
 
 def highlight_validation(color: str) -> str:
-    """ Validates the given highligh color is among supported basic colors """
-    if not color.lower() in [
-            "red", "green", "blue", "black", "orange", "yellow", "fuchsia", "lime", "olive", "teal",
-            "purple", "navy", "aqua"
+    """Validates the given highligh color is among supported basic colors"""
+    if color.lower() not in [
+        "red",
+        "green",
+        "blue",
+        "black",
+        "orange",
+        "yellow",
+        "fuchsia",
+        "lime",
+        "olive",
+        "teal",
+        "purple",
+        "navy",
+        "aqua",
     ]:
-        raise ValueError("Not a supported highligt color")
+        raise ValueError("Not a supported highlight color")
     return color
 
 
-def get_substring(text: str, **kwargs) -> Union[int, float, str]:
-    if '\xa0' in text:
-        text = text.replace('\xa0', ' ')
-    start, end = kwargs.get('between', '{}???{}').format(0, len(text)).split('???')
-    include_start = kwargs.get('include_locator', False)
-    exclude_end = kwargs.get('exclude_post', True)
+def get_substring(text: str, remove_newlines: bool = True, **kwargs) -> Union[int, float, str]:
+    if "\xa0" in text:
+        text = text.replace("\xa0", " ")
+    start, end = kwargs.get("between", "{}???{}").format(0, len(text)).split("???")
+    include_start = kwargs.get("include_locator", False)
+    exclude_end = kwargs.get("exclude_post", True)
     start = get_index_of(text, start, include_start)
     end = get_index_of(text, end, exclude_end)
     if end == 0:
         end = len(text)
-    if 'from_start' in kwargs:
-        end = start + int(kwargs.get('from_start'))  # type: ignore[arg-type]
-    if 'from_end' in kwargs:
-        start = end - int(kwargs.get('from_end'))  # type: ignore[arg-type]
-    logger.debug('substring start: {}'.format(start))
-    logger.debug('substring end: {}'.format(end))
-    text = str(text[start:end]).strip().replace('\n', "")
-    text = text.replace('\r', "")
+    if "from_start" in kwargs:
+        end = start + int(kwargs.get("from_start"))  # type: ignore[arg-type]
+    if "from_end" in kwargs:
+        start = end - int(kwargs.get("from_end"))  # type: ignore[arg-type]
+    logger.debug("substring start: {}".format(start))
+    logger.debug("substring end: {}".format(end))
+    if remove_newlines:
+        text = str(text[start:end]).strip().replace("\n", "")
+        text = text.replace("\r", "")
     try:
-        if 'int' in kwargs:
-            num = float(text.replace(' ', '').replace(',', '.'))
+        if "int" in kwargs:
+            num = float(text.replace(" ", "").replace(",", "."))
             return int(num)
-        if 'float' in kwargs:
-            return float(text.replace(' ', '').replace(',', '.'))
+        if "float" in kwargs:
+            return float(text.replace(" ", "").replace(",", "."))
     except ValueError as e:
-        raise QWebValueMismatchError('Unable to convert. Got exception: {}'.format(e)) from e
+        raise QWebValueMismatchError("Unable to convert. Got exception: {}".format(e)) from e
     return text
 
 
 def get_index_of(text: str, locator: str, condition: Union[bool, int, str]) -> int:
     try:
         return int(locator.strip())
     except ValueError:
-        if locator.startswith('\\'):
-            locator.replace('\\', "")
+        if locator.startswith("\\"):
+            locator.replace("\\", "")
     index = text.find(locator.strip())
     if index > -1:
         if par2bool(condition) is False:
             index += len(locator)
         return index
     raise QWebValueMismatchError('File did not contain the text "{}"'.format(locator))
 
@@ -196,25 +209,30 @@
 
 
 def is_retina() -> bool:
     if platform.system().lower() == "darwin":
         if "arm" in platform.machine().lower():
             return True
 
-        if subprocess.call("system_profiler SPDisplaysDataType | grep -i 'retina'",
-                           shell=True,
-                           stdout=subprocess.DEVNULL,
-                           stderr=subprocess.DEVNULL) == 0:
+        if (
+            subprocess.call(
+                "system_profiler SPDisplaysDataType | grep -i 'retina'",
+                shell=True,
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
+            == 0
+        ):
             return True
     return False
 
 
 def is_safari() -> bool:
     driver = browser.get_current_browser()
-    return driver.capabilities['browserName'].lower() in SAFARINAMES
+    return driver.capabilities["browserName"].lower() in SAFARINAMES
 
 
 def get_browser_width() -> int:
     driver = browser.get_current_browser()
     size = driver.get_window_size()
     return size["width"]
 
@@ -231,37 +249,38 @@
         try:
             d = json.loads(prefs_j)
         except json.decoder.JSONDecodeError:
             try:
                 d = _handle_old_style_prefs(prefs)
             except QWebUnexpectedConditionError as e:
                 raise QWebUnexpectedConditionError(
-                    'Invalid argument! Experimental opts should given in robot dict '
-                    'or string in format: key1:value1, key2:value2') from e
+                    "Invalid argument! Experimental opts should given in robot dict "
+                    "or string in format: key1:value1, key2:value2"
+                ) from e
     # handle booleans in string format
     for key, value in list(d.items()):
         if isinstance(value, str):  # Check if the value is a string
             value_lower = value.lower()
             if value_lower == "true":
                 d[key] = True
             elif value_lower == "false":
                 d[key] = False
     return d
 
 
 def _handle_old_style_prefs(prefs: str) -> dict:
     d = {}
     val: Union[bool, str]
-    separated = prefs.split(',')
+    separated = prefs.split(",")
     for s in separated:
-        splitted = s.split(':', maxsplit=1)
+        splitted = s.split(":", maxsplit=1)
         if len(splitted) == 2:
-            logger.warn('Prefs keys and values without quotes is deprecated.')
+            logger.warn("Prefs keys and values without quotes is deprecated.")
             key = splitted[0].strip()
-            if 'true' in splitted[1].lower() or 'false' in splitted[1].lower():
+            if "true" in splitted[1].lower() or "false" in splitted[1].lower():
                 val = par2bool(splitted[1].strip())
             else:
                 val = splitted[1].strip()
             d[key] = val
         else:
             raise QWebUnexpectedConditionError
     return d
@@ -275,82 +294,86 @@
 
 
 def validate_run_before(value: Union[list[str], str]) -> Optional[Union[list[str], str]]:
     if isinstance(value, list):
         if value[0].lower().startswith("verify"):
             return value
     elif is_py_func(value):
-        valid = ['verify_', 'verify_no']
+        valid = ["verify_", "verify_no"]
         if any(x in value for x in valid):
             return value
     elif value.lower().startswith("verify"):
         return value
-    logger.warn('Invalid value. Only Verify* keywords are accepted.')
+    logger.warn("Invalid value. Only Verify* keywords are accepted.")
     return None
 
 
 def initial_logging(capabilities: dict[str, Any]) -> None:
     """Log version numbers at the start of test runs."""
     logger.debug(f"{capabilities}")
     try:
-        b_n, b_v = capabilities['browserName'], capabilities['browserVersion']
-        logger.info('Browser: {}'.format(b_n), also_console=True)
-        logger.info('Browser version: {}'.format(b_v), also_console=True)
-        if b_n == 'firefox':
-            logger.info('Geckodriver version: {}'.format(capabilities['moz:geckodriverVersion']),
-                        also_console=True)
-        if b_n == 'chrome':
-            logger.info('Chromedriver version: {}'.format(
-                capabilities['chrome']['chromedriverVersion']),
-                        also_console=True)
-        if b_n == 'msedge':
-            logger.info('Edgedriver version: {}'.format(
-                capabilities['msedge']['msedgedriverVersion']),
-                        also_console=True)
+        b_n, b_v = capabilities["browserName"], capabilities["browserVersion"]
+        logger.info("Browser: {}".format(b_n), also_console=True)
+        logger.info("Browser version: {}".format(b_v), also_console=True)
+        if b_n == "firefox":
+            logger.info(
+                "Geckodriver version: {}".format(capabilities["moz:geckodriverVersion"]),
+                also_console=True,
+            )
+        if b_n == "chrome":
+            logger.info(
+                "Chromedriver version: {}".format(capabilities["chrome"]["chromedriverVersion"]),
+                also_console=True,
+            )
+        if b_n == "msedge":
+            logger.info(
+                "Edgedriver version: {}".format(capabilities["msedge"]["msedgedriverVersion"]),
+                also_console=True,
+            )
     except KeyError:
-        logger.debug('Could not get browser/driver version data.')
+        logger.debug("Could not get browser/driver version data.")
 
 
 def option_handler(options: Optional[str]) -> list[str]:
     options2 = []
     if options:
-        options2 += options.split(',')
+        options2 += options.split(",")
 
-    if get_rfw_variable_value('${BROWSER_OPTIONS}'):
-        options2 += get_rfw_variable_value('${BROWSER_OPTIONS}').split(',')
+    if get_rfw_variable_value("${BROWSER_OPTIONS}"):
+        options2 += get_rfw_variable_value("${BROWSER_OPTIONS}").split(",")
 
     return options2
 
 
 def get_rfw_variable_value(key: str, default_value=None) -> Any:
-    """ Return robot fw variable value if robot is running.
-        Returns default value if robot is not running."""
+    """Return robot fw variable value if robot is running.
+    Returns default value if robot is not running."""
     try:
         return BuiltIn().get_variable_value(key)
     except RobotNotRunningError:
         return default_value
 
 
 def get_callable(pw: str) -> Callable[..., Any]:
     """Return function by Paceword name if exists."""
-    lib = BuiltIn().get_library_instance('QWeb')
+    lib = BuiltIn().get_library_instance("QWeb")
     pacewords = dir(lib)
     for paceword in pacewords:
-        if not paceword.startswith('__'):
-            if str(pw).replace(' ', '').lower() == paceword.replace('_', ''):
+        if not paceword.startswith("__"):
+            if str(pw).replace(" ", "").lower() == paceword.replace("_", ""):
                 fn = getattr(lib, paceword)
                 return fn
-    raise QWebUnexpectedConditionError('Paceword {} not found'.format(pw))
+    raise QWebUnexpectedConditionError("Paceword {} not found".format(pw))
 
 
 def escape_xpath_quotes(text: str) -> str:
     """Return xpath text with proper quotes"""
     # both single and double quotes in text
     if '"' in text and "'" in text:
-        return 'concat(%s)' % ", '\"',".join('"%s"' % x for x in text.split('"'))
+        return "concat(%s)" % ", '\"',".join('"%s"' % x for x in text.split('"'))
     # only double
     if '"' in text:
         return f"'{text}'"
     return f'"{text}"'
 
 
 def anchor_to_index(anchor: str) -> int:
```

### Comparing `QWeb-3.2.1/QWeb/internal/window.py` & `QWeb-3.3.0/QWeb/internal/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,86 +24,84 @@
 from robot.api import logger
 import time
 
 
 def get_window_handles() -> list[str]:
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     return open_windows if util.is_safari() else driver.window_handles
 
 
 def get_current_window_handle() -> str:
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     return driver.current_window_handle
 
 
 def append_new_windows_safari() -> None:
-    """ Safari returns window handles in random order.
-        We must keep track of opened windows in safari.
-        This function will append new open windows to global list."""
+    """Safari returns window handles in random order.
+    We must keep track of opened windows in safari.
+    This function will append new open windows to global list."""
     driver = browser.get_current_browser()
     all_handles = driver.window_handles
     for i in all_handles:
         if i not in open_windows:
             open_windows.append(i)
 
 
 def get_url() -> str:
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     return driver.current_url
 
 
 def switch_to_window(handle) -> None:
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     driver.switch_to.window(handle)
 
 
-def swipe(direction: str, times: Union[str, int] = '1', start: Optional[str] = None) -> None:
+def swipe(direction: str, times: Union[str, int] = "1", start: Optional[str] = None) -> None:
     """
     Internal swipe function used by the swipe keywords. Uses the arrow keys to "swipe",
     unless a starting point is given. If a starting point is given, drag and drop is used.
     Functionality isn't 100% same as in QMobile, but this should work in most cases.
     """
-    logger.info('Even though the keyword is called swipe, '
-                'it actually uses arrow keys or drag and drop to "swipe".')
+    logger.info(
+        "Even though the keyword is called swipe, "
+        'it actually uses arrow keys or drag and drop to "swipe".'
+    )
     directions = {
-        'down': (Keys.ARROW_DOWN, 0, 500),
-        'up': (Keys.ARROW_UP, 0, -500),
-        'left': (Keys.ARROW_LEFT, -500, 0),
-        'right': (Keys.ARROW_RIGHT, 500, 0)
+        "down": (Keys.ARROW_DOWN, 0, 500),
+        "up": (Keys.ARROW_UP, 0, -500),
+        "left": (Keys.ARROW_LEFT, -500, 0),
+        "right": (Keys.ARROW_RIGHT, 500, 0),
     }
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     action_chains = ActionChains(driver)
     try:
         times = int(times)
     except ValueError as e:
-        raise ValueError('Amount of times swiped needs to be an integer.') from e
+        raise ValueError("Amount of times swiped needs to be an integer.") from e
     if not start:
         default_swipe_length = 20
         times = default_swipe_length * times
         for _ in range(int(times)):
             action_chains.send_keys(directions[direction][0])
             action_chains.pause(0.05)
         action_chains.perform()
-        time.sleep(.5)
+        time.sleep(0.5)
     else:
         start_element = text.get_unique_text_element(start)
         action_chains.click(start_element)
-        action_chains.pause(.5)
-        action_chains.drag_and_drop_by_offset(start_element, directions[direction][1] * times,
-                                              directions[direction][2] * times)
+        action_chains.pause(0.5)
+        action_chains.drag_and_drop_by_offset(
+            start_element, directions[direction][1] * times, directions[direction][2] * times
+        )
         action_chains.perform()
-        time.sleep(.5)
+        time.sleep(0.5)
```

### Comparing `QWeb-3.2.1/QWeb/internal/xhr.py` & `QWeb-3.3.0/QWeb/internal/xhr.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,45 +49,44 @@
 
     except (WebDriverException, JavascriptException) as e:
         raise QWebDriverError(e)  # pylint: disable=W0707
 
 
 def get_ready_state() -> bool:
     ready_state = javascript.execute_javascript('return document.readyState === "complete"')
-    logger.debug('Readystate = {}'.format(ready_state))
+    logger.debug("Readystate = {}".format(ready_state))
     return ready_state
 
 
 def get_jquery_ready() -> bool:
-    jqueries_ready = javascript.execute_javascript('return window.jQuery.active === 0;')
+    jqueries_ready = javascript.execute_javascript("return window.jQuery.active === 0;")
     return jqueries_ready
 
 
 def wait_xhr(timeout: float = 0.0) -> None:
     """Uses jQuery.active to check if page is ready
 
     if jQuery is not available, calls setup_xhr_monitor
     which injects it to the page.
     jQuery.active returns 0 when page and js are ready and
     AJAX is done.
 
     """
     start = time.time()
     while time.time() < timeout + start:
-        logger.debug('Timeout for xhr:s = {}'.format(timeout))
+        logger.debug("Timeout for xhr:s = {}".format(timeout))
         ready_state = get_ready_state()
         logger.debug("ready_state {}".format(ready_state))
         if ready_state:
             jquery = setup_xhr_monitor()
             if jquery:
                 jquery_ready = get_jquery_ready()
                 if jquery_ready:
                     return
-                logger.debug('There are still pending AJAX requests..')
+                logger.debug("There are still pending AJAX requests..")
             else:
-                logger.debug('Unable to inject jQuery..')
+                logger.debug("Unable to inject jQuery..")
                 return
         else:
-            logger.debug('Page is not loaded yet..')
+            logger.debug("Page is not loaded yet..")
 
-    logger.debug('Page was not ready after {} seconds.'
-                 'Trying to continue..'.format(timeout))
+    logger.debug("Page was not ready after {} seconds." "Trying to continue..".format(timeout))
```

### Comparing `QWeb-3.2.1/QWeb/keywords/ajax.py` & `QWeb-3.3.0/QWeb/keywords/ajax.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,120 @@
-# -*- coding: utf-8 -*-
-# --------------------------
-# Copyright © 2014 -            Qentinel Group.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ---------------------------
-from __future__ import annotations
-from typing import Union, Optional
-
-from QWeb.internal import decorators, ajax, util
-from robot.api.deco import keyword
-
-
-@keyword(tags=["Logging"])
-@decorators.timeout_decorator
-def save_file(
-        locator: str,
-        filename: Optional[str] = None,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        path: Optional[str] = None,
-        **kwargs) -> None:
-    r"""Save file using http-request.
-
-    Needs url of the downloadable content which usually is in element's href attribute.
-    Text or tooltip can be used as a locator (Works as ClickText or ClickItem).
-    If locator element is not the one with href-attribute, tries to get href from closest
-    parent with <a> tag in it.
-
-    url can be used as a locator too.
-
-    Available element types without using tag attribute:
-    *a, span, img, li, h1, h2, h3, h4, h5, h6, div, svg, p, button, input\*
-    (\*submit buttons only).*
-
-    Examples
-    --------
-    .. code-block:: robotframework
-
-        SaveFile      ClickMe       filename.pdf
-        SaveFile      tooltip       filename.xml
-
-        # Locators parent or child element is the one with href:
-        SaveFile      ClickMe       filename.pdf    child=a
-        SaveFile      tooltip       filename.xml    parent=div
-
-        # Create folder for downloadable files:
-        SaveFile      ClickMe       pdf/filename.pdf
-        SaveFile      tooltip       xml/filename.xml
-        SaveFile      Robot         pics/filename.png
-
-        # Using url as locator
-        SaveFile      https://www.robot.fi/robot.xml  filename.xml
-
-        # Get html content of given url
-        SaveFile      https://www.qentinel.com      qentinel.html
-
-    Parameters
-    ----------
-    locator : str
-        Text or item to be "clicked".
-    filename: str
-        Wanted filename
-    anchor : str
-        Text near the element to be clicked or index. If the page contains many
-        places where the text argument is then anchor is used to get the
-        one that is closest to it.  (default 1)
-    timeout : str | int
-        How long we wait for element to be ready for click
-    path : str
-        Wanted path for files. Default path is users download folder.
-    kwargs :
-        |  Accepted kwargs:
-        |       tag : html tag of preferred element -
-        |           If tag is used then element is found
-        |           by some of it's attribute
-        |       parent : str: tag name for clickable parent
-        |       child : str: tag name for clickable child.
-        |       index : str: use index if there is multiple
-        |       childs with same tag name
-        |       headers : dict -Pass headers to http request
-
-    Related keywords
-    ----------------
-    \`ExpectFileDownload\`, \`UploadFile\`, \`UseFile\`,
-    \`VerifyFile\`, \`VerifyFileDownload\`
-    """
-    if locator.startswith('http'):
-        url = locator
-    else:
-        url = ajax.get_url_for_http_request(locator, anchor, **kwargs)
-    response = ajax.http_request_with_browser_cookies(url)
-    if not filename:
-        filename = str(
-            util.get_substring(
-                response.headers.get(
-                    'Content-Disposition',
-                    'filename=unnamed.{}'.format(
-                        response.headers.get(  # type: ignore[union-attr]
-                            'Content-Type').split('/')[1].split(';')[0])),
-                between='filename=???'))
-    ajax.save_response_as_file(response, str(filename), path)
+# -*- coding: utf-8 -*-
+# --------------------------
+# Copyright © 2014 -            Qentinel Group.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ---------------------------
+from __future__ import annotations
+from typing import Union, Optional
+
+from QWeb.internal import decorators, ajax, util
+from robot.api.deco import keyword
+
+
+@keyword(tags=["Logging"])
+@decorators.timeout_decorator
+def save_file(
+    locator: str,
+    filename: Optional[str] = None,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    path: Optional[str] = None,
+    **kwargs,
+) -> None:
+    r"""Save file using http-request.
+
+    Needs url of the downloadable content which usually is in element's href attribute.
+    Text or tooltip can be used as a locator (Works as ClickText or ClickItem).
+    If locator element is not the one with href-attribute, tries to get href from closest
+    parent with <a> tag in it.
+
+    url can be used as a locator too.
+
+    Available element types without using tag attribute:
+    *a, span, img, li, h1, h2, h3, h4, h5, h6, div, svg, p, button, input\*
+    (\*submit buttons only).*
+
+    Examples
+    --------
+    .. code-block:: robotframework
+
+        SaveFile      ClickMe       filename.pdf
+        SaveFile      tooltip       filename.xml
+
+        # Locators parent or child element is the one with href:
+        SaveFile      ClickMe       filename.pdf    child=a
+        SaveFile      tooltip       filename.xml    parent=div
+
+        # Create folder for downloadable files:
+        SaveFile      ClickMe       pdf/filename.pdf
+        SaveFile      tooltip       xml/filename.xml
+        SaveFile      Robot         pics/filename.png
+
+        # Using url as locator
+        SaveFile      https://www.robot.fi/robot.xml  filename.xml
+
+        # Get html content of given url
+        SaveFile      https://www.qentinel.com      qentinel.html
+
+    Parameters
+    ----------
+    locator : str
+        Text or item to be "clicked".
+    filename: str
+        Wanted filename
+    anchor : str
+        Text near the element to be clicked or index. If the page contains many
+        places where the text argument is then anchor is used to get the
+        one that is closest to it.  (default 1)
+    timeout : str | int
+        How long we wait for element to be ready for click
+    path : str
+        Wanted path for files. Default path is users download folder.
+    kwargs :
+        |  Accepted kwargs:
+        |       tag : html tag of preferred element -
+        |           If tag is used then element is found
+        |           by some of it's attribute
+        |       parent : str: tag name for clickable parent
+        |       child : str: tag name for clickable child.
+        |       index : str: use index if there is multiple
+        |       childs with same tag name
+        |       headers : dict -Pass headers to http request
+
+    Related keywords
+    ----------------
+    \`ExpectFileDownload\`, \`UploadFile\`, \`UseFile\`,
+    \`VerifyFile\`, \`VerifyFileDownload\`
+    """
+    if locator.startswith("http"):
+        url = locator
+    else:
+        url = ajax.get_url_for_http_request(locator, anchor, **kwargs)
+    response = ajax.http_request_with_browser_cookies(url)
+    if not filename:
+        filename = str(
+            util.get_substring(
+                response.headers.get(
+                    "Content-Disposition",
+                    "filename=unnamed.{}".format(
+                        response.headers.get(  # type: ignore[union-attr]
+                            "Content-Type"
+                        )
+                        .split("/")[1]
+                        .split(";")[0]
+                    ),
+                ),
+                between="filename=???",
+            )
+        )
+    ajax.save_response_as_file(response, str(filename), path)
```

### Comparing `QWeb-3.2.1/QWeb/keywords/alert.py` & `QWeb-3.3.0/QWeb/keywords/alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,8 +159,8 @@
     Related keywords
     ----------------
     \`CloseAlert\`, \`GetAlertText\`, \`IsAlert\`, \`TypeAlert\`
     """
     alert_ = alert.wait_alert(timeout=timeout)
     if text in alert_.text:
         return
-    raise QWebValueError('Text {} is not presented in Alert'.format(text))
+    raise QWebValueError("Text {} is not presented in Alert".format(text))
```

### Comparing `QWeb-3.2.1/QWeb/keywords/blocks.py` & `QWeb-3.3.0/QWeb/keywords/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         |       defined, this will be executed after every failed try
         |       before retrying
 
     Related keywords
     ----------------
     \`Appstate\`, \`SetConfig\`
     """
-    step = [{'paceword': block, 'args': args, 'kwargs': {}}]
+    step = [{"paceword": block, "args": args, "kwargs": {}}]
     try:
         _execute_block(step, timeout=timeout, **kwargs)
     except QWebElementNotFoundError as e:
         raise QWebUnexpectedConditionError(f"Runblock did not succeed in {timeout} seconds") from e
 
 
 @keyword(tags=("Config", "Error handling"))
@@ -129,30 +129,31 @@
         Possible args for block
 
     Related keywords
     ----------------
     \`RunBlock\`, \`SetConfig\`
     """
     status, res = BuiltIn().run_keyword_and_ignore_error(block, *args)
-    if status == 'FAIL':
+    if status == "FAIL":
         raise QWebUnexpectedConditionError(
-            'Unable to set correct pre-condition for test due error: {}'.format(res))
+            "Unable to set correct pre-condition for test due error: {}".format(res)
+        )
 
 
 @decorators.timeout_decorator
 def _execute_block(steps: list[dict[str, Any]], timeout: Union[int, float, str] = 0, **kwargs):  # pylint: disable=unused-argument
-    logger.trace(f'Timeout for block: {timeout}')
+    logger.trace(f"Timeout for block: {timeout}")
     logger.trace(f"{steps=}")
     for step in steps:
-        fn = step.get('paceword')
-        var_name = step.get('variable', None)
-        args = blocks.set_robot_args(*step.get('args', []), **step.get('kwargs', {}))
+        fn = step.get("paceword")
+        var_name = step.get("variable", None)
+        args = blocks.set_robot_args(*step.get("args", []), **step.get("kwargs", {}))
         status, res = BuiltIn().run_keyword_and_ignore_error(fn, *args)
-        logger.trace(f'status: {status}, res: {res}')
-        if status == 'FAIL':
-            teardown = kwargs.get('exp_handler', None)
+        logger.trace(f"status: {status}, res: {res}")
+        if status == "FAIL":
+            teardown = kwargs.get("exp_handler", None)
             if teardown:
                 BuiltIn().run_keyword_and_ignore_error(teardown)
 
-            raise QWebElementNotFoundError(f'Err from block {res}')
+            raise QWebElementNotFoundError(f"Err from block {res}")
         if var_name:
-            BuiltIn().set_suite_variable(f'{var_name}', res)
+            BuiltIn().set_suite_variable(f"{var_name}", res)
```

### Comparing `QWeb-3.2.1/QWeb/keywords/browser.py` & `QWeb-3.3.0/QWeb/keywords/browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # ---------------------------
 from __future__ import annotations
 from typing import Union, Optional
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.common.by import By
 
 import os
-import pkg_resources
 import requests
+from importlib.metadata import version, PackageNotFoundError
 from robot.api import logger
 from robot.api.deco import keyword
 from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
 from QWeb.keywords import window
 from QWeb.internal import browser, xhr, exceptions, util
 from QWeb.internal.config_defaults import CONFIG
 from QWeb.internal.decorators import get_timeout
@@ -122,26 +122,34 @@
         # Mobile emulation
         OpenBrowser    http://google.com     chrome    emulation=iPhone SE
         OpenBrowser    http://google.com     chrome    emulation=375x812
 
     Selenium Manager
     ----------------
 
-    If browser driver(s) can be found in path, they will be used. If not, Selenium
+    Selenium Manager's automatic browser and driver management is available for Chrome, Firefox
+    and Edge. To use specific browser version, add `browser_version` keyword argument.
+    If matching browser & driver(s) can be found in path, they will be used. If not, Selenium
     Manager tries to download and install them. With Chrome also specific version of
     browser ("Chrome for Testing") can be used.
+    Note that for Edge in Windows local admin rights are required!
+
+    More info:
+    https://www.selenium.dev/documentation/selenium_manager/#automated-browser-management
 
     **NOTE**: if you are using QWeb in some cloud service,
     it's best to use their method of setting browser version.
 
     .. code-block:: robotframework
 
-        # If Chrome 117 is already installed, it will be used.
-        # If not, Chrome for Testing v117 will be downloaded and used.
-        OpenBrowser   https://www.google.com    chrome    browser_version=117
+        # If Chrome 124 is already installed, it will be used.
+        # If not, Chrome for Testing v124 will be downloaded and used.
+        OpenBrowser   https://www.google.com    chrome    browser_version=124
+        OpenBrowser   https://www.google.com    firefox   browser_version=124
+        OpenBrowser   https://www.google.com    edge      browser_version=124
 
     BrowserStack usage
     ------------------
     QWeb can be directly used with BrowserStack for desktop and mobile browser
     testing. Your own Browserstack credentials are required.
 
     .. code-block:: robotframework
@@ -289,27 +297,21 @@
     Related keywords
     ----------------
     \`Back\`, \`CloseAllBrowsers\`, \`CloseBrowser\`, \`GetTitle\`,
     \`GetUrl\`, \`GoTo\`, \`RefreshPage\`, \`ReturnBrowser\`,
     \`SwitchWindow\`, \`VerifyTitle\`, \`VerifyUrl\`
     """
     try:
-        logger.info(
-            "\nQWeb version number: {}".format(
-                pkg_resources.get_distribution("QWeb").version
-            ),
-            also_console=True,
-        )
-    except pkg_resources.DistributionNotFound:
+        qweb_version = version("QWeb")
+        logger.info(f"QWeb version number: {qweb_version}", also_console=True)
+    except PackageNotFoundError:
         logger.info("Could not find QWeb version number.")
     number_of_open_sessions = _sessions_open()
     if number_of_open_sessions > 0:
-        logger.warn(
-            "You have {} browser sessions already open".format(number_of_open_sessions)
-        )
+        logger.warn("You have {} browser sessions already open".format(number_of_open_sessions))
     option_list = util.option_handler(options)
     b_lower = browser_alias.lower()
 
     if os.getenv("QWEB_HEADLESS"):
         kwargs = {"headless": True}
     if os.getenv("CHROME_ARGS") is not None:
         if option_list is None:
@@ -321,35 +323,27 @@
     bs_project_name = util.get_rfw_variable_value("${PROJECTNAME}") or ""
     bs_run_id = util.get_rfw_variable_value("${RUNID}") or ""
     provider = util.get_rfw_variable_value("${PROVIDER}")
 
     if provider in ("bs", "browserstack"):
         bs_device = util.get_rfw_variable_value("${DEVICE}")
         if not bs_device and b_lower in bs_desktop.NAMES:
-            driver = bs_desktop.open_browser(
-                b_lower, bs_project_name, bs_run_id, **kwargs
-            )
+            driver = bs_desktop.open_browser(b_lower, bs_project_name, bs_run_id, **kwargs)
         elif bs_device:
-            driver = bs_mobile.open_browser(
-                bs_device, bs_project_name, bs_run_id, **kwargs
-            )
+            driver = bs_mobile.open_browser(bs_device, bs_project_name, bs_run_id, **kwargs)
         else:
-            raise exceptions.QWebException(
-                "Unknown browserstack browser {}".format(browser_alias)
-            )
+            raise exceptions.QWebException("Unknown browserstack browser {}".format(browser_alias))
     else:
         driver = _browser_checker(b_lower, option_list, **kwargs)
     util.initial_logging(driver.capabilities)
 
     # If user wants to re-use Chrome browser then he/she has to give
     # variable BROWSER_REUSE=True. In that case no URL loaded needed as
     # user wants to continue with the existing browser session
-    is_browser_reused = (
-        util.par2bool(util.get_rfw_variable_value("${BROWSER_REUSE}")) or False
-    )
+    is_browser_reused = util.par2bool(util.get_rfw_variable_value("${BROWSER_REUSE}")) or False
     if not (is_browser_reused and b_lower == "chrome"):
         driver.get(url)
     xhr.setup_xhr_monitor()
 
 
 @keyword(tags=("Browser", "Interaction"))
 def switch_browser(index: Union[int, str]) -> None:
```

### Comparing `QWeb-3.2.1/QWeb/keywords/checkbox.py` & `QWeb-3.3.0/QWeb/keywords/checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 """Keywords for checkbox elements.
 
 Checkboxes are those that can be checked/selected and unchecked/unselected.
 """
+
 from __future__ import annotations
 from typing import Union
 
 from robot.api.deco import keyword
 from QWeb.internal import checkbox, actions, decorators
 import QWeb.internal.element
 from QWeb.internal.exceptions import QWebValueError
 
 
 @keyword(tags=("Checkbox", "Interaction"))
 @decorators.timeout_decorator
-def click_checkbox(locator: str,
-                   value: str,
-                   anchor: str = "1",
-                   timeout: Union[int, float, str] = 0,
-                   index: int = 1,
-                   **kwargs) -> None:
+def click_checkbox(
+    locator: str,
+    value: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Check or uncheck a checkbox.
 
     Examples
     --------
     .. code-block:: robotframework
 
         ClickCheckbox    I am not a robot    on
@@ -90,31 +93,33 @@
         CheckBox element not found
 
     Related keywords
     ----------------
     \`VerifyCheckbox\`, \`VerifyCheckboxStatus\`, \`VerifyCheckboxValue\`
     """
     checkbox_element, locator_element = checkbox.get_checkbox_elements_from_all_documents(
-        locator, anchor=anchor, index=index, **kwargs)
+        locator, anchor=anchor, index=index, **kwargs
+    )
     if checkbox_element:
         if value.lower() == "on":
             actions.checkbox_set(checkbox_element, locator_element, value=True, timeout=timeout)
         else:
             actions.checkbox_set(checkbox_element, locator_element, value=False, timeout=timeout)
 
 
 @keyword(tags=("Checkbox", "Verification"))
 @decorators.timeout_decorator
 def verify_checkbox_status(
-        locator: str,
-        status: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        index=1,
-        **kwargs) -> None:
+    locator: str,
+    status: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    index=1,
+    **kwargs,
+) -> None:
     r"""Verify checkbox is enabled or disabled.
 
     In other words verify can user interact with a checkbox or not.
 
     Examples
     --------
     .. code-block:: robotframework
@@ -164,38 +169,38 @@
     ValueError
         Checkbox interaction with the checkbox was not the same
 
     Related keywords
     ----------------
     \`ClickCheckbox\`, \`VerifyCheckbox\`, \`VerifyCheckboxValue\`
     """
-    checkbox_element, _ = checkbox.get_checkbox_elements_from_all_documents(locator,
-                                                                            anchor=anchor,
-                                                                            index=index,
-                                                                            **kwargs)
+    checkbox_element, _ = checkbox.get_checkbox_elements_from_all_documents(
+        locator, anchor=anchor, index=index, **kwargs
+    )
     status = status.lower()
     if status.lower() == "enabled":
         if not QWeb.internal.element.is_enabled(checkbox_element):
-            raise QWebValueError('The checkbox was disabled')
+            raise QWebValueError("The checkbox was disabled")
     elif status.lower() == "disabled":
         if QWeb.internal.element.is_enabled(checkbox_element):
-            raise QWebValueError('The checkbox was enabled')
+            raise QWebValueError("The checkbox was enabled")
     else:
         raise QWebValueError('Unkown status: "{}"'.format(status))
 
 
 @keyword(tags=("Checkbox", "Verification"))
 @decorators.timeout_decorator
 def verify_checkbox_value(
-        locator: str,
-        value: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        index: int = 1,
-        **kwargs) -> None:
+    locator: str,
+    value: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Verify checkbox is on (checked) or off (unchecked).
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyCheckboxValue    Mercedes           on
@@ -243,37 +248,37 @@
     ------
     ValueError : The checkbox value is not the same
 
     Related keywords
     ----------------
     \`ClickCheckbox\`, \`VerifyCheckbox\`, \`VerifyCheckboxStatus\`
     """
-    checkbox_element, _ = checkbox.get_checkbox_elements_from_all_documents(locator,
-                                                                            anchor=anchor,
-                                                                            index=index,
-                                                                            **kwargs)
+    checkbox_element, _ = checkbox.get_checkbox_elements_from_all_documents(
+        locator, anchor=anchor, index=index, **kwargs
+    )
     value = value.lower()
     if value.lower() == "on":
         if not checkbox.is_checked(checkbox_element):
-            raise QWebValueError('The checkbox was not checked.')
+            raise QWebValueError("The checkbox was not checked.")
     elif value.lower() == "off":
         if checkbox.is_checked(checkbox_element):
-            raise QWebValueError('The checkbox was checked')
+            raise QWebValueError("The checkbox was checked")
     else:
         raise QWebValueError('Unkown value: "{}"'.format(value))
 
 
 @keyword(tags=("Checkbox", "Verification"))
 @decorators.timeout_decorator
 def verify_checkbox(
-        locator: str,
-        anchor: str = '1',
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        index: int = 1,
-        **kwargs) -> None:
+    locator: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Verify that checkbox element exist.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyCheckbox    Mercedes
@@ -312,13 +317,12 @@
     ------
     NoSuchElementException: Checkbox element not found
 
     Related keywords
     ----------------
     \`ClickCheckbox\`, \`VerifyCheckboxStatus\`, \`VerifyCheckboxValue\`
     """
-    checkbox_element, _ = checkbox.get_checkbox_elements_from_all_documents(locator,
-                                                                            anchor=anchor,
-                                                                            index=index,
-                                                                            **kwargs)
+    checkbox_element, _ = checkbox.get_checkbox_elements_from_all_documents(
+        locator, anchor=anchor, index=index, **kwargs
+    )
     if checkbox_element:
         return
```

### Comparing `QWeb-3.2.1/QWeb/keywords/config.py` & `QWeb-3.3.0/QWeb/keywords/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1084,12 +1084,14 @@
     return current_config
 
 
 def _set_case_insensitivity(val: str) -> None:
     check = util.par2bool(val)
 
     if check:
-        CONFIG.set_value("ContainingTextMatch",
-                         SearchStrategies.CONTAINING_TEXT_MATCH_CASE_INSENSITIVE)
+        CONFIG.set_value(
+            "ContainingTextMatch", SearchStrategies.CONTAINING_TEXT_MATCH_CASE_INSENSITIVE
+        )
     else:
-        CONFIG.set_value("ContainingTextMatch",
-                         SearchStrategies.CONTAINING_TEXT_MATCH_CASE_SENSITIVE)
+        CONFIG.set_value(
+            "ContainingTextMatch", SearchStrategies.CONTAINING_TEXT_MATCH_CASE_SENSITIVE
+        )
```

### Comparing `QWeb-3.2.1/QWeb/keywords/cookies.py` & `QWeb-3.3.0/QWeb/keywords/cookies.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # limitations under the License.
 # ---------------------------
 """Keywords for browser cookie handling.
 
 When Selenium gets cookies from browser, it return them as dictionaries
 in a list. This list can be searched for key - value pairs.
 """
+
 from __future__ import annotations
 from typing import Any
 from robot.api import logger
 from robot.api.deco import keyword
 from QWeb.internal import cookies
```

### Comparing `QWeb-3.2.1/QWeb/keywords/debug.py` & `QWeb-3.3.0/QWeb/keywords/debug.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 """Keywords for controlling debugger."""
+
 import pyautogui
 from DebugLibrary import DebugLibrary
 from robot.api.deco import keyword
 from QWeb.internal.config_defaults import CONFIG
 
 cur_timeout = 0
 cur_mode = None
 
 
 @keyword(tags=("Debug", "Error handling"))
-def debug_on(mode: str = 'draw') -> None:
+def debug_on(mode: str = "draw") -> None:
     r"""Start debugger with drawing mode and set default timeout down to 2 sec.
 
     Examples
     --------
     .. code-block:: robotframework
 
        debugon    #Start debugger and set timeout to 2sec.
@@ -44,22 +45,23 @@
     Related keywords
     ----------------
     \`DebugOff\`
     """
     dbg = DebugLibrary()
     global cur_mode  # pylint: disable=global-statement
     global cur_timeout  # pylint: disable=global-statement
-    cur_mode = CONFIG.get_value('SearchMode')
+    cur_mode = CONFIG.get_value("SearchMode")
     cur_timeout = CONFIG.get_value(  # type: ignore[assignment]
-        'DefaultTimeout')
-    CONFIG.set_value('SearchMode', mode)
-    CONFIG.set_value('DefaultTimeout', 2)
-    CONFIG.set_value('Debug_Run', True)
+        "DefaultTimeout"
+    )
+    CONFIG.set_value("SearchMode", mode)
+    CONFIG.set_value("DefaultTimeout", 2)
+    CONFIG.set_value("Debug_Run", True)
     dbg.debug()
-    CONFIG.set_value('DefaultTimeout', cur_timeout)
+    CONFIG.set_value("DefaultTimeout", cur_timeout)
 
 
 @keyword(tags=("Debug", "Error handling"))
 def debug_off() -> None:
     r"""Exit debugger. Set timeout and SearchMode back to default.
 
     Examples
@@ -68,11 +70,11 @@
 
        debugoff
 
     Related keywords
     ----------------
     \`DebugOn\`
     """
-    CONFIG.set_value('SearchMode', cur_mode)
-    CONFIG.set_value('DefaultTimeout', cur_timeout)
-    CONFIG.set_value('Debug_Run', False)
-    pyautogui.hotkey('ctrl', 'D')
+    CONFIG.set_value("SearchMode", cur_mode)
+    CONFIG.set_value("DefaultTimeout", cur_timeout)
+    CONFIG.set_value("Debug_Run", False)
+    pyautogui.hotkey("ctrl", "D")
```

### Comparing `QWeb-3.2.1/QWeb/keywords/download.py` & `QWeb-3.3.0/QWeb/keywords/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,30 +65,30 @@
     start = time.time()
     previous_message = None
     while time.time() < start + timeout_int:
         modified_files = download.get_modified_files(download_dir, download.start_epoch)
         modified_files = download.remove_win_temp(modified_files)
         if len(modified_files) == 1:
             if not download.is_tmp_file(modified_files[0]):
-                logger.info('Found downloaded file {}'.format(modified_files[0]))
+                logger.info("Found downloaded file {}".format(modified_files[0]))
                 return modified_files[0]
         elif not modified_files:
-            message = 'Could not find any modified files'
+            message = "Could not find any modified files"
             if previous_message != message:
                 logger.info(message)
                 previous_message = message
         else:
-            message = 'Modified files\n{}'.format('\n'.join(modified_files))
+            message = "Modified files\n{}".format("\n".join(modified_files))
             if previous_message != message:
                 logger.info(message)
                 previous_message = message
             if all(not download.is_tmp_file(modified_file) for modified_file in modified_files):
-                raise ValueError('Found more than one file that was modified')
+                raise ValueError("Found more than one file that was modified")
         time.sleep(SHORT_DELAY)
-    raise ValueError('Could not find any modified files after {}s'.format(timeout_int))
+    raise ValueError("Could not find any modified files after {}s".format(timeout_int))
 
 
 @keyword(tags=("Browser", "Verification"))
 def expect_file_download() -> None:
     r"""Turns on polling for time after which file download should happen.
 
     Run this keyword everytime before \`VerifyFileDownload\` and the action that
@@ -103,10 +103,13 @@
         VerifyFileDownload      timeout=20s     # file should be downloaded in 20 seconds
 
     Related keywords
     ----------------
     \`SaveFile\`, \`UploadFile\`, \`VerifyFileDownload\`
     """
     now = time.time()
-    logger.info('The time has been set to {}'.format(
-        time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(now))))
+    logger.info(
+        "The time has been set to {}".format(
+            time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(now))
+        )
+    )
     download.start_epoch = now
```

### Comparing `QWeb-3.2.1/QWeb/keywords/dragdrop.py` & `QWeb-3.3.0/QWeb/keywords/dragdrop.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 """Keywords for draggable elements."""
+
 from __future__ import annotations
 from typing import Union
 from selenium.webdriver.remote.webelement import WebElement
 
 import pyautogui
 from robot.api import logger
 from robot.api.deco import keyword
@@ -26,29 +27,31 @@
 from QWeb.internal import element, decorators, dragdrop
 from QWeb.internal import text as internal_text
 from QWeb.internal import javascript
 
 
 @keyword(tags=["Interaction"])
 @decorators.timeout_decorator
-def drag_drop(locator: str,
-              target_locator: str,
-              index: int = 1,
-              anchor: str = "1",
-              target_anchor: str = "1",
-              timeout: Union[int, float, str] = 0,
-              dragtime: Union[int, str] = '0.5s',
-              left: int = 0,
-              right: int = 0,
-              above: int = 0,
-              below: int = 0,
-              loc_left: int = 0,
-              loc_right: int = 0,
-              loc_above: int = 0,
-              loc_below: int = 0) -> None:
+def drag_drop(
+    locator: str,
+    target_locator: str,
+    index: int = 1,
+    anchor: str = "1",
+    target_anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    dragtime: Union[int, str] = "0.5s",
+    left: int = 0,
+    right: int = 0,
+    above: int = 0,
+    below: int = 0,
+    loc_left: int = 0,
+    loc_right: int = 0,
+    loc_above: int = 0,
+    loc_below: int = 0,
+) -> None:
     # pylint: disable=unused-argument
     r"""Drag and drop element.
 
     Finds draggable element by it's visible text, tooltip attribute, index
     or xpath.
     Target element is found by it's visible text or xpath.
 
@@ -114,37 +117,39 @@
 
     Related keywords
     ----------------
     \`SwipeDown\`, \`SwipeLeft\`, \`SwipeRight\`, \`SwipeUp\`
     """
     pyautogui.FAILSAFE = False
     draggable = dragdrop.get_draggable_element(locator, index, anchor)
-    if target_locator.startswith('xpath=') or target_locator.startswith('//'):
+    if target_locator.startswith("xpath=") or target_locator.startswith("//"):
         target_elem = element.get_unique_element_by_xpath(target_locator, index=int(index - 1))
     else:
         target_elem = internal_text.get_text_using_anchor(target_locator, target_anchor)
     x, y = _get_coordinates(draggable)
     x = x + int(loc_right) - int(loc_left)
     y = y - int(loc_above) + int(loc_below)
-    logger.debug('draggable x is {} and y is {}'.format(x, y))
+    logger.debug("draggable x is {} and y is {}".format(x, y))
     pyautogui.moveTo(x, y)
     x, y = _get_coordinates(target_elem)
     x = x + int(right) - int(left)
     y = y - int(above) + int(below)
-    logger.debug('target x is {} and y is {}'.format(x, y))
+    logger.debug("target x is {} and y is {}".format(x, y))
     dragtime = _timestr_to_secs(dragtime)
-    pyautogui.dragTo(x, y, dragtime, button='left')
+    pyautogui.dragTo(x, y, dragtime, button="left")
     pyautogui.FAILSAFE = True
 
 
 def _get_coordinates(web_element: WebElement) -> tuple[int, int]:
     x_diff = javascript.execute_javascript(
-        'return window.outerWidth-window.innerWidth+screen.availLeft')
+        "return window.outerWidth-window.innerWidth+screen.availLeft"
+    )
     y_diff = javascript.execute_javascript(
-        'return window.outerHeight-window.innerHeight+screen.availTop')
+        "return window.outerHeight-window.innerHeight+screen.availTop"
+    )
     elem = javascript.execute_javascript("return arguments[0].getBoundingClientRect()", web_element)
     logger.debug("coords: {0}".format(elem))
-    y = elem['y']
+    y = elem["y"]
 
-    x_coord = web_element.location['x'] + x_diff + web_element.size['width'] / 2
-    y_coord = y + y_diff + web_element.size['height'] / 2
+    x_coord = web_element.location["x"] + x_diff + web_element.size["width"] / 2
+    y_coord = y + y_diff + web_element.size["height"] / 2
     return int(x_coord), int(y_coord)
```

### Comparing `QWeb-3.2.1/QWeb/keywords/dropdown.py` & `QWeb-3.3.0/QWeb/keywords/dropdown.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,33 +14,39 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 """Keywords for dropdown elements.
 
 Dropdown elements are considered to be any <select> tagged element.
 """
+
 from __future__ import annotations
 from typing import Union
 
 from robot.api.deco import keyword
 from QWeb.internal import decorators, actions
 from QWeb.internal.dropdown import get_dd_elements_from_all_documents as _get_dd_elements
 
 
 @keyword(tags=("Dropdown", "Interaction"))
 @decorators.timeout_decorator
-def drop_down(locator: str,
-              option: str,
-              anchor: str = '1',
-              timeout: Union[int, float, str] = 0,
-              index: int = 1,
-              unselect: bool = False,
-              **kwargs) -> None:
+def drop_down(
+    locator: str,
+    option: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    unselect: bool = False,
+    **kwargs,
+) -> None:
     r"""Select an option from dropdown menu/list.
 
+    **NOTE:** This keyword is designed to function exclusively with actual dropdowns
+    that contain **<select>** and **<option>** tags.
+
     Examples
     --------
     .. code-block:: robotframework
 
         DropDown        Canis   Collie
 
     In the above example the DropDown keyword will select from a dropdown
@@ -118,23 +124,28 @@
     select = _get_dd_elements(locator, anchor, index=index, **kwargs)
     if actions.select_option(select, option, timeout=timeout, unselect=unselect):
         return
 
 
 @keyword(tags=("Dropdown", "Verification"))
 @decorators.timeout_decorator
-def verify_selected_option(locator: str,
-                           expected_option: str,
-                           anchor: str = '1',
-                           timeout: Union[int, float, str] = 0,
-                           index: int = 1,
-                           **kwargs) -> None:
+def verify_selected_option(
+    locator: str,
+    expected_option: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Verify that an option is selected from dropdown menu/list.
     Note: with multiselection dropdown verify each option individually.
 
+    **NOTE:** This keyword is designed to function exclusively with actual dropdowns
+    that contain **<select>** and **<option>** tags.
+
     Examples
     --------
     .. code-block:: robotframework
 
         VerifySelectedOption    Canis   Collie
 
     In the above example the VerifySelectedOption keyword verifies from a dropdown
@@ -174,21 +185,22 @@
     select = _get_dd_elements(locator, anchor=anchor, index=index, **kwargs)
     if actions.get_selected_value(select, expected_option, timeout=timeout):
         return
 
 
 @keyword(tags=("Dropdown", "Getters"))
 @decorators.timeout_decorator
-def get_selected(locator: str,
-                 anchor: str = '1',
-                 timeout: Union[int, float, str] = 0,
-                 index: int = 1,
-                 **kwargs) -> None:
+def get_selected(
+    locator: str, anchor: str = "1", timeout: Union[int, float, str] = 0, index: int = 1, **kwargs
+) -> None:
     r"""Get selected option to variable from dropdown menu/list.
 
+    **NOTE:** This keyword is designed to function exclusively with actual dropdowns
+    that contain **<select>** and **<option>** tags.
+
     Examples
     --------
     .. code-block:: robotframework
 
         ${VALUE}    GetSelected    Canis
 
     In the above example we get selected value from dropdown Canis.
@@ -231,22 +243,27 @@
     """
     select = _get_dd_elements(locator, anchor=anchor, index=index, **kwargs)
     return actions.get_selected_value(select, timeout=timeout)
 
 
 @keyword(tags=("Dropdown", "Verification"))
 @decorators.timeout_decorator
-def verify_option(locator: str,
-                  expected_option: str,
-                  anchor: str = '1',
-                  timeout: Union[int, float, str] = 0,
-                  index: int = 1,
-                  **kwargs) -> None:
+def verify_option(
+    locator: str,
+    expected_option: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Verify that option exist in dropdown menu/list.
 
+    **NOTE:** This keyword is designed to function exclusively with actual dropdowns
+    that contain **<select>** and **<option>** tags.
+
     Examples
     --------
     .. code-block:: robotframework
 
        VerifyOption    Canis   Collie
 
     In the above example the VerifyOption keyword verifies from a dropdown
@@ -285,21 +302,22 @@
     select = _get_dd_elements(locator, anchor=anchor, index=index, **kwargs)
     if actions.get_select_options(select, expected_option, timeout=timeout):
         return
 
 
 @keyword(tags=("Dropdown", "Getters"))
 @decorators.timeout_decorator
-def get_drop_down_values(locator: str,
-                         anchor: str = '1',
-                         timeout: Union[int, float, str] = 0,
-                         index: int = 1,
-                         **kwargs) -> None:
+def get_drop_down_values(
+    locator: str, anchor: str = "1", timeout: Union[int, float, str] = 0, index: int = 1, **kwargs
+) -> None:
     r"""Return all options from a dropdown menu/list.
 
+    **NOTE:** This keyword is designed to function exclusively with actual dropdowns
+    that contain **<select>** and **<option>** tags.
+
     Examples
     --------
     .. code-block:: robotframework
 
         ${all_options}=     GetDropDownValues     Canis     Collie
         log     ${all_options}
 
@@ -332,22 +350,27 @@
     """
     select = _get_dd_elements(locator, anchor, index=index, **kwargs)
     return actions.get_select_options(select, timeout=timeout)
 
 
 @keyword(tags=("Dropdown", "Verification"))
 @decorators.timeout_decorator
-def verify_no_option(locator: str,
-                     option: str,
-                     anchor: str = '1',
-                     timeout: Union[int, float, str] = 0,
-                     index: int = 1,
-                     **kwargs) -> None:
+def verify_no_option(
+    locator: str,
+    option: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Verify that a given option is not in a dropdown menu/list.
 
+    **NOTE:** This keyword is designed to function exclusively with actual dropdowns
+    that contain **<select>** and **<option>** tags.
+
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyNoOption     Foobar    Cat
 
     In the above example VerifyNoOption keyword checks that the option "Cat" is not found
```

### Comparing `QWeb-3.2.1/QWeb/keywords/element.py` & `QWeb-3.3.0/QWeb/keywords/element.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 """Keywords for general elements that are retrieved using XPaths."""
+
 from __future__ import annotations
 from typing import Union, Optional
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.select import Select
 
 from robot.api.deco import keyword
 from QWeb.internal.exceptions import QWebValueError, QWebElementNotFoundError
-from QWeb.internal import element, decorators, actions, text, input_, \
-    dropdown, checkbox
+from QWeb.internal import element, decorators, actions, text, input_, dropdown, checkbox
 
 
 @keyword(tags=["Interaction"])
 @decorators.timeout_decorator
-def click_element(xpath: Union[WebElement, str],
-                  timeout: Union[int, float, str] = 0,
-                  js: bool = False,
-                  index: int = 1,
-                  **kwargs) -> None:
+def click_element(
+    xpath: Union[WebElement, str],
+    timeout: Union[int, float, str] = 0,
+    js: bool = False,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Click element specified by xpath.
 
     Examples
     --------
     .. code-block:: robotframework
 
         ClickElement          click_me      tag=button
@@ -84,31 +86,33 @@
     \`ClickCell\`, \`ClickCheckbox\`, \`ClickIcon\`, \`ClickItem\`, \`ClickList\`,
     \`ClickText\`, \`ClickUntil\`, \`ClickWhile\`, \`RightClick\`, \`VerifyElement\`
     """
     if isinstance(xpath, WebElement):
         web_element = xpath
     else:
         index = int(index) - 1
-        kwargs['element_kw'] = True
-        if 'tag' in kwargs:
-            web_element = element.get_elements_by_attributes(kwargs.get('tag'), xpath,
-                                                             **kwargs)[index]
+        kwargs["element_kw"] = True
+        if "tag" in kwargs:
+            web_element = element.get_elements_by_attributes(kwargs.get("tag"), xpath, **kwargs)[
+                index
+            ]
         else:
             web_element = element.get_unique_element_by_xpath(xpath, index=index)
     if actions.execute_click_and_verify_condition(web_element, timeout=timeout, js=js, **kwargs):
         return
 
 
 @keyword(tags=["Interaction"])
 @decorators.timeout_decorator
 def right_click(
-        xpath: str,
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        index: int = 1,
-        **kwargs) -> None:
+    xpath: str,
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Right clicks the element.
 
     Examples
     --------
     .. code-block:: robotframework
 
         RightClick          click_me      tag=button
@@ -133,29 +137,30 @@
         |       to True to allow partial match
 
     Related keywords
     ----------------
     \`ClickElement\`, \`ClickItem\`, \`ClickText\`
     """
     index = int(index) - 1
-    kwargs['element_kw'] = True
-    if 'tag' in kwargs:
-        web_element = element.get_elements_by_attributes(kwargs.get('tag'), xpath, **kwargs)[index]
+    kwargs["element_kw"] = True
+    if "tag" in kwargs:
+        web_element = element.get_elements_by_attributes(kwargs.get("tag"), xpath, **kwargs)[index]
     else:
         web_element = element.get_unique_element_by_xpath(xpath, index=index)
     actions.right_click(web_element)
 
 
 @keyword(tags=["Interaction"])
 @decorators.timeout_decorator
 def hover_element(
-        xpath: Union[WebElement, str],
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        index: int = 1,
-        **kwargs) -> None:
+    xpath: Union[WebElement, str],
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Hover the element specified by the xpath selector.
 
     Examples
     --------
     .. code-block:: robotframework
 
         HoverElement          //*[@id\="hover_me"]
@@ -184,30 +189,32 @@
     \`HoverItem\`, \`HoverText\`, \`HoverTo\`, \`Scroll\`,
     \`ScrollText\`, \`ScrollTo\`
     """
     if isinstance(xpath, WebElement):
         web_element = xpath
     else:
         index = int(index) - 1
-        kwargs['element_kw'] = True
-        if 'tag' in kwargs:
-            web_element = element.get_elements_by_attributes(kwargs.get('tag'), xpath,
-                                                             **kwargs)[index]
+        kwargs["element_kw"] = True
+        if "tag" in kwargs:
+            web_element = element.get_elements_by_attributes(kwargs.get("tag"), xpath, **kwargs)[
+                index
+            ]
         else:
             web_element = element.get_unique_element_by_xpath(xpath, index=index)
 
     actions.hover_to(web_element, timeout=timeout)
 
 
 @keyword(tags=["Getters"])
 @decorators.timeout_decorator
 def get_element_count(
-        locator: str,
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        **kwargs) -> int:
+    locator: str,
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    **kwargs,
+) -> int:
     r"""Get count of appearances for certain web element.
 
     Keyword waits until timeout has passed. If timeout is not specified, it
     uses default timeout that can be adjusted with DefaultTimeout keyword.
 
     GetElementCount does not require for the text to be unique.
 
@@ -228,30 +235,31 @@
     Accepted kwargs:
         tag=tagname: Needed when attribute value is used as a locator
 
     Related keywords
     ----------------
     \`GetTextCount\`, \`GetWebElement\`
     """
-    kwargs['element_kw'] = True
-    if 'tag' in kwargs:
-        web_elements = element.get_elements_by_attributes(kwargs.get('tag'), locator, **kwargs)
+    kwargs["element_kw"] = True
+    if "tag" in kwargs:
+        web_elements = element.get_elements_by_attributes(kwargs.get("tag"), locator, **kwargs)
     else:
         web_elements = element.get_webelements(locator, **kwargs)
     if web_elements:
         return len(web_elements)
-    raise QWebElementNotFoundError('Webelements not found')
+    raise QWebElementNotFoundError("Webelements not found")
 
 
 @keyword(tags=["Verification"])
 def is_element(
-        xpath: str,
-        timeout: Union[int, float, str] = '0.1s',
-        index: int = 1,  # pylint: disable=unused-argument
-        **kwargs) -> bool:
+    xpath: str,
+    timeout: Union[int, float, str] = "0.1s",
+    index: int = 1,  # pylint: disable=unused-argument
+    **kwargs,
+) -> bool:
     r"""Return True if element is visible.
 
     Examples
     --------
     .. code-block:: robotframework
 
         $note_visible=  IsElement        Paused
@@ -331,31 +339,33 @@
         Page did not contain element
 
     Related keywords
     ----------------
     \`ClickElement\`, \`GetAttribute\`, \`GetWebElement\`, \`GetElementCount\`,
     \`VerifyItem\`, \`VerifyText\`
     """
-    kwargs['element_kw'] = True
-    if 'tag' in kwargs:
+    kwargs["element_kw"] = True
+    if "tag" in kwargs:
         web_elements = element.get_visible_elements_from_elements(
-            element.get_elements_by_attributes(kwargs.get('tag'), xpath, **kwargs))
+            element.get_elements_by_attributes(kwargs.get("tag"), xpath, **kwargs)
+        )
     else:
         web_elements = element.get_webelements(xpath, **kwargs)
     if web_elements:
         return
-    raise QWebElementNotFoundError('No matching element found')
+    raise QWebElementNotFoundError("No matching element found")
 
 
 @keyword(tags=["Verification"])
 @decorators.timeout_decorator
 def verify_no_element(
-        xpath: str,
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        **kwargs) -> None:
+    xpath: str,
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    **kwargs,
+) -> None:
     r"""Wait element can not be found on the page.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyNoElement          //*[@id\="do_not_wait_me"]
@@ -389,32 +399,36 @@
     NoSuchElementException
         Page did contain the element
 
     Related keywords
     ----------------
     \`VerifyElement\`
     """
-    kwargs['element_kw'] = True
-    if 'tag' in kwargs:
+    kwargs["element_kw"] = True
+    if "tag" in kwargs:
         web_elements = element.get_visible_elements_from_elements(
-            element.get_elements_by_attributes(kwargs.get('tag'), xpath, **kwargs))
+            element.get_elements_by_attributes(kwargs.get("tag"), xpath, **kwargs)
+        )
     else:
         web_elements = element.get_webelements(xpath)
     if not web_elements:
         return
     raise QWebValueError('Page contained element with XPath "{}" after timeout'.format(xpath))
 
 
 @keyword(tags=["Getters"])
 @decorators.timeout_decorator
-def get_webelement(locator: str,
-                   anchor: str = '1',
-                   element_type: Optional[str] = None,
-                   timeout: Union[int, float, str] = 0,
-                   **kwargs) -> Union[Select, Optional[WebElement], list[WebElement]]:
+def get_webelement(
+    locator: str,
+    anchor: str = "1",
+    element_type: Optional[str] = None,
+    timeout: Union[int, float, str] = 0,
+    **kwargs,
+) -> Union[Select, Optional[WebElement], list[WebElement]]:
+    # pylint: disable=too-many-branches
     r"""Get Webelement using any Qword -stylish locator.
 
     Examples
     --------
     Using attributes or xpaths like with ClickElement etc. kw:s without specified
     element_type. Result is a type of list unless **index** or **element_type** is given:
 
@@ -470,56 +484,66 @@
         |       documentation
 
     Related keywords
     ----------------
     \`ClickElement\`, \`HoverElement\`, \`TypeText\`
     """
     web_elements: Union[Select, Optional[WebElement], list[WebElement]]
-    elem_index = kwargs.get('index', None)
-    kwargs['index'] = kwargs.get('index', 1)
-    kwargs['timeout'] = timeout
+    elem_index = kwargs.get("index", None)
+    kwargs["index"] = kwargs.get("index", 1)
+    kwargs["timeout"] = timeout
     if element_type:
-        if element_type.lower() == 'text':
+        if element_type.lower() == "text":
             web_elements = text.get_element_by_locator_text(locator, anchor, **kwargs)
-        if element_type.lower() == 'item':
+        elif element_type.lower() == "item":
             web_elements = text.get_item_using_anchor(locator, anchor, **kwargs)
-        if element_type.lower() == "dropdown":
+        elif element_type.lower() == "dropdown":
             web_elements = dropdown.get_dd_elements_from_all_documents(locator, anchor, **kwargs)
-        if element_type.lower() == "input":
+        elif element_type.lower() == "input":
             web_elements = input_.get_input_elements_from_all_documents(locator, anchor, **kwargs)
-        if element_type.lower() == "checkbox":
+        elif element_type.lower() == "checkbox":
             web_elements = checkbox.get_checkbox_elements_from_all_documents(
-                locator, anchor, **kwargs)[0]
-        if element_type.lower() == "css":
+                locator, anchor, **kwargs
+            )[0]
+        elif element_type.lower() == "css":
             web_elements = element.get_webelement_by_css(locator, **kwargs)
+        else:
+            msg = (
+                f"Invalid 'element_type':'{element_type}'!\n"
+                "\tValid types: 'text', 'item', 'dropdown', 'input', 'checkbox', 'css'"
+            )
+            raise QWebValueError(msg)
         return web_elements
 
-    kwargs['element_kw'] = True
-    if 'tag' in kwargs:
+    kwargs["element_kw"] = True
+    if "tag" in kwargs:
         web_elements = element.get_visible_elements_from_elements(
-            element.get_elements_by_attributes(kwargs.get('tag'), locator, **kwargs))
+            element.get_elements_by_attributes(kwargs.get("tag"), locator, **kwargs)
+        )
     else:
         web_element_list = element.get_webelements(locator, **kwargs)
         if elem_index:
             web_elements = element.get_element_by_index(web_element_list, elem_index)  # type: ignore # pylint: disable=line-too-long
         else:
             web_elements = web_element_list
     if web_elements:
         return web_elements
-    raise QWebElementNotFoundError('No matching element found')
+    raise QWebElementNotFoundError("No matching element found")
 
 
 @keyword(tags=["Getters"])
 @decorators.timeout_decorator
-def get_attribute(locator: str,
-                  attribute: str,
-                  anchor: str = '1',
-                  element_type: Optional[str] = None,
-                  timeout: Union[int, float, str] = 0,
-                  **kwargs) -> str:
+def get_attribute(
+    locator: str,
+    attribute: str,
+    anchor: str = "1",
+    element_type: Optional[str] = None,
+    timeout: Union[int, float, str] = 0,
+    **kwargs,
+) -> str:
     r"""Get attribute value of an element.
 
     Examples
     --------
     Using xpaths like with ClickElement etc. kw:s without specified
     element_type. Index must be given if element is not unique:
 
@@ -586,36 +610,40 @@
     Related keywords
     ----------------
     \`VerifyAttribute\`, \`VerifyElement\`
     """
     webelement = get_webelement(locator, anchor, element_type, timeout, **kwargs)
 
     if not webelement:
-        raise QWebElementNotFoundError('Could not find element {} with attribute {}'.format(
-            locator, attribute))
+        raise QWebElementNotFoundError(
+            "Could not find element {} with attribute {}".format(locator, attribute)
+        )
     if not isinstance(webelement, list):
         return webelement.get_attribute(attribute)
 
     if len(webelement) == 1:
         return webelement[0].get_attribute(attribute)
 
-    raise QWebValueError('Found {} occurences of locator {}. '
-                         'Use index etc. to uniquely identify the element'.format(
-                             len(webelement), locator))
+    raise QWebValueError(
+        "Found {} occurences of locator {}. "
+        "Use index etc. to uniquely identify the element".format(len(webelement), locator)
+    )
 
 
 @keyword(tags=["Verification"])
 @decorators.timeout_decorator
-def verify_attribute(locator: str,
-                     attribute: str,
-                     value: str,
-                     anchor: str = '1',
-                     element_type: Optional[str] = None,
-                     timeout: Union[int, float, str] = 0,
-                     **kwargs) -> None:
+def verify_attribute(
+    locator: str,
+    attribute: str,
+    value: str,
+    anchor: str = "1",
+    element_type: Optional[str] = None,
+    timeout: Union[int, float, str] = 0,
+    **kwargs,
+) -> None:
     r"""Verify attribute value of an element.
 
     Examples
     --------
     Using attributes or xpaths like with ClickElement etc. kw:s without specified
     element_type. If element_type is not specified end result is a type of list:
 
@@ -708,13 +736,13 @@
 
 
     Related keywords
     ----------------
     \`GetAttribute\`, \`VerifyElement\`
     """
     attr_val = get_attribute(locator, attribute, anchor, element_type, timeout, **kwargs)
-    operator = kwargs.get('operator', "equals")
+    operator = kwargs.get("operator", "equals")
 
     try:
         element.operator_verify(attr_val, value, operator)
     except QWebValueError as e:
         raise e
```

### Comparing `QWeb-3.2.1/QWeb/keywords/file.py` & `QWeb-3.3.0/QWeb/keywords/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,32 @@
 # limitations under the License.
 # ---------------------------
 from typing import Optional
 from pathlib import Path
 
 from QWeb.internal.file import File
 from QWeb.internal import download
-from QWeb.internal.exceptions import QWebInstanceDoesNotExistError, QWebValueMismatchError, \
-    QWebUnexpectedConditionError, QWebValueError, QWebFileNotFoundError
+from QWeb.internal.exceptions import (
+    QWebInstanceDoesNotExistError,
+    QWebValueMismatchError,
+    QWebUnexpectedConditionError,
+    QWebValueError,
+    QWebFileNotFoundError,
+)
 from zipfile import ZipFile
 from os.path import basename as _basename
 import os
 import shutil
 from robot.api import logger
 from robot.api.deco import keyword
 
 ACTIVE_FILE: File = None  # type: ignore[assignment]
 
 
-@keyword(tags=["File"])
+@keyword(tags=["PDF", "File"])
 def use_pdf(filename: str) -> None:
     r"""Define pdf file for all other pdf keywords.
 
     Sets active file for other keywords.
 
     Examples
     --------
@@ -82,85 +87,123 @@
     \`GetFileText\`, \`RemoveFile\`, \`SaveFile\`, \`UploadFile\`,
     \`VerifyAll\`, \`VerifyFileDownload\`, \`VerifyFileText\`
     """
     global ACTIVE_FILE  # pylint:disable=global-statement
     ACTIVE_FILE = File.create_text_file_instance(filename)
 
 
-@keyword(tags=("File", "Getters"))
+@keyword(tags=("PDF", "File", "Getters"))
 def get_pdf_text(**kwargs) -> str:
-    r"""Get text from pdf file.
+    r"""Get text content from pdf file.
 
     Examples
     --------
     .. code-block:: robotframework
 
-        ${text}    GetPdfText    #returns whole content
-        ${text}    GetPdfText    locator=xyz   chars=10  #returns 10 chars, starting from text xyz.
+        UsePdf     dummy.pdf
+        # returns whole PDF content
+        ${text}    GetPdfText
+
+        # returns whole PDF content, but remove newlines (\n)
+        ${text}    GetPdfText    remove_newlines=True
+
+        # returns 6 characters from the beginning
+        ${text}    GetPdfText    from_start=6
+
+        # returns 6 characters from the end
+        ${text}    GetPdfText    from_end=6
+
+        # returns all chars between Simple and File
+        ${text}    GetPdfText    between=Simple???File
+
+        # matches to text between Simple and end of file.
+        ${text}    GetPdfText    between=Simple???
+
+        # Returns 6 characters from the beginning of match.
+        ${text}    GetPdfText    between=Simple???       from_start=6
 
     Parameters
     ----------
-    locator : str
-        Starting point for substring (Locator text is returned by default)
-    post_text : str
-        Ending point for substring (post_text is not returned by default)
-    chars : int
-        length of wanted string
-    include_locator : bool
-        if set to False returns chars after locator text.
-    exclude_post : bool
-        if set to False returned string includes post_text
+    kwargs :
+        |  Accepted kwargs:
+        |       between : str/int - Start???End - Return all chars between texts Start and End.
+        |       from_start : int - Return x amount of chars. Starting from first char
+        |       from_end : int - Return x amount of chars. Starting from last char
+        |       include_locator : True - Starting text is part of returned string
+        |       exclude_post : False - Ending text is part of returned string
+        |       int : True - Return integer instead of string
+        |       float : int - Return float instead of string
+        |       remove_newlines : bool - Remove newlines (\\n) from returned text (True/False)
 
     Note that you must use named arguments with this keyword, i.e. use
     ``argument_name=value`` format!
 
     Related keywords
     ----------------
     \`RemovePdf\`, \`UsePdf\`, \`VerifyPdfText\`
     """
     _file_exists()
     return str(ACTIVE_FILE.get(**kwargs))
 
 
 @keyword(tags=("File", "Getters"))
 def get_file_text(**kwargs) -> str:
-    r"""Get text from pdf file.
+    r"""Get text content from a plain text file.
 
     Examples
     --------
     .. code-block:: robotframework
 
-        ${text}    GetFileText    #returns whole content
-        ${text}    GetFileText    xyz   10  #returns 10 chars, starting from text xyz.
+        UseFile    text.txt
+        # returns whole text content
+        ${text}    GetFileText
+
+        # returns whole text content, but remove newlines (\n)
+        ${text}    GetFileText   remove_newlines=True
+
+        # returns 6 characters from the beginning
+        ${text}    GetFileText   from_start=6
+
+        # returns 6 characters from the end
+        ${text}    GetFileText   from_end=6
+
+        # returns all chars between Simple and File
+        ${text}    GetFileText   between=Simple???File
+
+        # matches to text between Simple and end of file.
+        ${text}    GetFileText   between=Simple???File
+
+        # Returns 6 characters from the beginning of match.
+        ${text}    GetFileText   between=Simple???       from_start=6
 
     Parameters
     ----------
-    locator : str
-        Starting point for substring (Locator text is returned by default)
-    post_text : str
-        Ending point for substring (post_text is not returned by default)
-    chars : int
-        length of wanted string
-    include_locator : bool
-        if set to False returns chars after locator text.
-    exclude_post : bool
-        if set to False returned string includes post_text
+    kwargs :
+        |  Accepted kwargs:
+        |       between : str/int - Start???End - Return all chars between texts Start and End.
+        |       from_start : int - Return x amount of chars. Starting from first char
+        |       from_end : int - Return x amount of chars. Starting from last char
+        |       include_locator : True - Starting text is part of returned string
+        |       exclude_post : False - Ending text is part of returned string
+        |       int : True - Return integer instead of string
+        |       float : int - Return float instead of string
+        |       remove_newlines : bool - Remove newlines (\\n) from returned text (True/False)
 
     Note that you must use named arguments with this keyword, i.e. use
     ``argument_name=value`` format!
 
     Related keywords
     ----------------
     \`RemoveFile\`, \`UseFile\`, \`VerifyFileText\`
     """
     _file_exists()
     return str(ACTIVE_FILE.get(**kwargs))
 
 
-@keyword(tags=("File", "Verification"))
+@keyword(tags=("PDF", "File", "Verification"))
 def verify_pdf_text(text: str, normalize: bool = False) -> None:
     r"""Verify text from pdf file.
 
     Examples
     --------
     .. code-block:: robotframework
 
@@ -180,15 +223,15 @@
     """
     _file_exists()
     ACTIVE_FILE.verify(text, normalize)
 
 
 @keyword(tags=("File", "Verification"))
 def verify_file_text(text: str, normalize: bool = False) -> None:
-    r"""Verify text from pdf file.
+    r"""Verify text from plain text file.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyFileText     Test Automation
 
@@ -203,17 +246,17 @@
     ----------------
     \`GetFileText\`,\`RemoveFile\`, \`UseFile\`
     """
     _file_exists()
     ACTIVE_FILE.verify(text, normalize)
 
 
-@keyword(tags=("File", "Verification"))
+@keyword(tags=("PDF", "File", "Verification"))
 def verify_no_pdf_text(text: str, normalize: bool = False) -> None:
-    r"""Verify text not exists in pdf-file.
+    r"""Check that the text does not exist in the PDF file.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyNoPdfText     Robot
 
@@ -227,22 +270,22 @@
     Related keywords
     ----------------
     \`VerifyPdfText\`,\`VerifyFileText\`
     """
     _file_exists()
     try:
         if ACTIVE_FILE.verify(text, normalize) is True:
-            raise QWebUnexpectedConditionError('Text {} exists in pdf file'.format(text))
+            raise QWebUnexpectedConditionError("Text {} exists in pdf file".format(text))
     except QWebValueMismatchError:
         return
 
 
 @keyword(tags=("File", "Verification"))
 def verify_no_file_text(text: str, normalize: bool = False) -> None:
-    r"""Verify text not exists in pdf-file.
+    r"""Check that the text does not exist in the plain text file.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyNoFileText     Robot
 
@@ -256,15 +299,15 @@
     Related keywords
     ----------------
     \`VerifyFileText\`, \`VerifyPdfText\`
     """
     _file_exists()
     try:
         if ACTIVE_FILE.verify(text, normalize) is True:
-            raise QWebUnexpectedConditionError('Text {} exists in file'.format(text))
+            raise QWebUnexpectedConditionError("Text {} exists in file".format(text))
     except QWebValueMismatchError:
         return
 
 
 @keyword(tags=("File", "Interaction"))
 def remove_file(file: Optional[str] = None) -> None:
     r"""Remove a file.
@@ -286,15 +329,15 @@
         _file_exists()
         ACTIVE_FILE.remove()
     else:
         if os.path.isfile(file):
             os.remove(file)
 
 
-@keyword(tags=("File", "Interaction"))
+@keyword(tags=("PDF", "File", "Interaction"))
 def remove_pdf() -> None:
     r"""Remove a file.
 
     Examples
     --------
     .. code-block:: robotframework
 
@@ -310,18 +353,18 @@
     _file_exists()
     ACTIVE_FILE.remove()
 
 
 def _file_exists(file_path: Optional[File] = None) -> bool:
     if not file_path:
         if isinstance(ACTIVE_FILE, File) is False:
-            raise QWebInstanceDoesNotExistError('File has not been defined with UsePdf keyword')
+            raise QWebInstanceDoesNotExistError("File has not been defined with UsePdf keyword")
         return True
     if isinstance(file_path, File) is False:
-        raise QWebInstanceDoesNotExistError('Could not locate file {}'.format(file_path))
+        raise QWebInstanceDoesNotExistError("Could not locate file {}".format(file_path))
     return True
 
 
 @keyword(tags=("File", "Interaction"))
 def zip_files(name_of_zip: str, files_to_zip: str) -> None:
     """Zip files.
 
@@ -338,32 +381,36 @@
     Parameters
     ----------
     name_of_zip : str
         Name of the zip file created.
     files_to_zip : str
         Files to be zipped, separated by "," in case of multiple files.
     """
-    if not name_of_zip.endswith('.zip'):
-        name_of_zip += '.zip'
-    files = files_to_zip.split(',')
+    if not name_of_zip.endswith(".zip"):
+        name_of_zip += ".zip"
+    files = files_to_zip.split(",")
     try:
-        with ZipFile(name_of_zip, 'w') as zipped:
+        with ZipFile(name_of_zip, "w") as zipped:
             for file in files:
                 file = str(download.get_path(file.strip()))
                 if os.path.isdir(file):
                     for root, _, files2 in os.walk(file):
                         for file2 in files2:
                             zipped.write(os.path.join(root, file2))
                 else:
                     zipped.write(file, _basename(file))
     except OSError as e:
-        raise QWebValueError('\nFile name "{}" contained illegal characters.'
-                             '\nError message: {}'.format(name_of_zip, str(e))) from e
-    logger.info('Zipped files {} into the file {}'.format(str(files), name_of_zip),
-                also_console=True)
+        raise QWebValueError(
+            '\nFile name "{}" contained illegal characters.' "\nError message: {}".format(
+                name_of_zip, str(e)
+            )
+        ) from e
+    logger.info(
+        "Zipped files {} into the file {}".format(str(files), name_of_zip), also_console=True
+    )
 
 
 @keyword(tags=("File", "Interaction"))
 def move_files(files_to_move: str, destination_folder: str) -> None:
     r"""Move files.
 
     Examples
@@ -381,16 +428,16 @@
         Destination folder of the moved files.
 
     Related keywords
     ----------------
     \`RemoveFile\`, \`SaveFile\`, \`UploadFile\`, \`VerifyFile\`
     """
     if not os.path.isdir(destination_folder):
-        raise QWebValueError('Destination folder does not exist.')
-    files = files_to_move.split(',')
+        raise QWebValueError("Destination folder does not exist.")
+    files = files_to_move.split(",")
     for file in files:
         file = str(download.get_path(file.strip()))
         shutil.move(file, destination_folder)
 
 
 @keyword(tags=("File", "Verification"))
 def verify_file(filename: str) -> Path:
@@ -410,12 +457,13 @@
     Parameters
     ----------
     filename : str
         Filename or path to find.
     """
     try:
         path = download.get_path(filename)
-        logger.info('File found. Filepath is {}'.format(path))
+        logger.info("File found. Filepath is {}".format(path))
         return path
     except QWebFileNotFoundError as e:
-        raise QWebFileNotFoundError('File not found from default folders. '
-                                    'It may not exists or you may need a full path.') from e
+        raise QWebFileNotFoundError(
+            "File not found from default folders. It may not exists or you may need a full path."
+        ) from e
```

### Comparing `QWeb-3.2.1/QWeb/keywords/frame.py` & `QWeb-3.3.0/QWeb/keywords/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # limitations under the License.
 # ---------------------------
 """Keywords for webpage and frame elements.
 
 Frame is considered to be an element in a webapage which can contain another
 webpage. Usually these elements have iframe -tag.
 """
+
 from __future__ import print_function
 
 from selenium.common.exceptions import NoSuchFrameException
 
 from robot.api.deco import keyword
 
 from QWeb.internal import browser, element, frame, javascript
@@ -48,22 +49,23 @@
     NoSuchFrameException
         If the frame is not found
     """
     frame.wait_page_loaded()
     try:
         index = int(locator) - 1
         webelement = javascript.execute_javascript(
-            'document.querySelectorAll("iframe, frame")[{}]'.format(index))
+            'document.querySelectorAll("iframe, frame")[{}]'.format(index)
+        )
     except ValueError:
         webelement = element.get_unique_element_by_xpath(locator)
     driver = browser.get_current_browser()
     try:
         driver.switch_to.frame(webelement)
     except NoSuchFrameException as e:
-        raise NoSuchFrameException('No frame wound with xpath: {0}'.format(locator)) from e
+        raise NoSuchFrameException("No frame wound with xpath: {0}".format(locator)) from e
 
 
 @keyword(tags=["Config"])
 def use_page() -> None:
     """Make following keywords to use the page and not a frame on a page.
 
     Examples
```

### Comparing `QWeb-3.2.1/QWeb/keywords/input_.py` & `QWeb-3.3.0/QWeb/keywords/input_.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------
 """Keywords for input elements.
 
 Input elements are those in which one can input text in.
 """
+
 from __future__ import annotations
 from typing import Union
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.remote.webelement import WebElement
 from robot.api import logger
 from robot.api.deco import keyword
 from pyautogui import hotkey
@@ -71,20 +72,22 @@
     input_handler.line_break_key = key
     return old_line_break_key
 
 
 secrets.add_filter("Type Secret3", 1, "hint")
 
 
-def type_secret3(locator: str,
-                 input_text: str,
-                 anchor: str = "1",
-                 timeout: Union[int, float, str] = 0,
-                 index: int = 1,
-                 **kwargs) -> None:
+def type_secret3(
+    locator: str,
+    input_text: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     """Type sensitive information such as personal data.
 
     the first 1 or 3 digits of the secret value are displayed
     in the logfile, otherwise functionality is the same as Type Secret.
 
     Generally all secret credentials in Robot FW scripts should
     be provided as external variables. Secrets must not be
@@ -99,31 +102,33 @@
         # Provide this to Robot FW as follows:
         # robot --variable NAME:janedoe test.robot
         TypeSecret3      name    ${NAME}
         TypeSecret3      r1c1    ${NAME} #table
     """
     length = len(input_text)
     if length > 4:
-        logger.info('SECRET: {}'.format(input_text[:3]) + (length - 3) * '*')
+        logger.info("SECRET: {}".format(input_text[:3]) + (length - 3) * "*")
     else:
-        logger.info('SECRET: {}'.format(input_text[:1]) + (length - 1) * '*')
+        logger.info("SECRET: {}".format(input_text[:1]) + (length - 1) * "*")
     type_text(locator, input_text, anchor, timeout=timeout, index=index, **kwargs)
 
 
 # Filter out input_text parameter in type_secret
 secrets.add_filter("Type Secret", 1, None)
 
 
 @keyword(tags=("Input", "Interaction"))
-def type_secret(locator: str,
-                input_text: str,
-                anchor: str = "1",
-                timeout: Union[int, float, str] = 0,
-                index: int = 1,
-                **kwargs) -> None:
+def type_secret(
+    locator: str,
+    input_text: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Type secret information such as password.
 
     Logging in start_keyword and end_keyword is filtered,
     otherwise functionality is the same as TypeText.
 
     Generally all secret credentials in Robot FW scripts should
     be provided as external variables. Secrets must not be
@@ -145,20 +150,22 @@
     \`TypeText\`
     """
     type_text(locator, input_text, anchor, timeout=timeout, index=index, **kwargs)
 
 
 @keyword(tags=("Input", "Interaction"))
 @decorators.timeout_decorator
-def type_text(locator: Union[WebElement, str],
-              input_text: str,
-              anchor: str = "1",
-              timeout: Union[int, float, str] = 0,
-              index: int = 1,
-              **kwargs) -> None:
+def type_text(
+    locator: Union[WebElement, str],
+    input_text: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Type given text to a text field.
 
     First look through if there are any input fields that have the
     locator as a placeholder. If not then locates the input field by
     which is closest to the locator text.
 
     When input field is found, it is first cleared of all text and after
@@ -265,26 +272,25 @@
     Related keywords
     ----------------
     \`PressKey\`, \`TypeSecret\`, \`TypeTexts\`, \`WriteText\`
     """
     if isinstance(locator, WebElement):
         input_element = locator
     else:
-        input_element = input_.get_input_elements_from_all_documents(locator,
-                                                                     anchor,
-                                                                     timeout=timeout,
-                                                                     index=index,
-                                                                     **kwargs)
+        input_element = input_.get_input_elements_from_all_documents(
+            locator, anchor, timeout=timeout, index=index, **kwargs
+        )
     actions.write(input_element, str(input_text), timeout=timeout, **kwargs)
 
 
 @keyword(tags=("File", "Input", "Interaction"))
 @decorators.timeout_decorator
-def type_texts(input_texts: Union[dict[str, str], str],
-               timeout: Union[int, float, str] = '0') -> None:
+def type_texts(
+    input_texts: Union[dict[str, str], str], timeout: Union[int, float, str] = "0"
+) -> None:
     r"""Type text to multiple fields.
 
     Accepts a .txt file or Robot FW dictionary as a parameter. If using a text file, the locator
     and the text should be separated with a comma on each row.
 
     Examples
     --------
@@ -301,35 +307,37 @@
     ----------------
     \`PressKey\`, \`TypeSecret\`, \`TypeText\`, \`WriteText\`
     """
     if isinstance(input_texts, dict):
         for locator in input_texts:
             logger.info('Typing "{}", locator "{}"'.format(locator, input_texts[locator]))
             type_text(locator, input_texts[locator])
-    elif input_texts.endswith('.txt') or input_texts.endswith('.csv'):
+    elif input_texts.endswith(".txt") or input_texts.endswith(".csv"):
         file = download.get_path(input_texts)
-        with open(file, 'rb') as txt_file:
+        with open(file, "rb") as txt_file:
             params = [line.rstrip() for line in txt_file]
             for x_bytes in params:
-                x_str_list = x_bytes.decode('utf-8').split(',')
+                x_str_list = x_bytes.decode("utf-8").split(",")
                 locator, text = x_str_list[0].strip(), x_str_list[1].strip()
                 logger.info('Typing "{}", locator "{}"'.format(text, locator))
                 type_text(locator, text, timeout=timeout)
     else:
-        raise QWebValueError('Unknown input value. Text file or dictionary required.')
+        raise QWebValueError("Unknown input value. Text file or dictionary required.")
 
 
 @keyword(tags=("Input", "Verification"))
 @decorators.timeout_decorator
-def verify_input_value(locator: Union[WebElement, str],
-                       expected_value: str,
-                       anchor: str = "1",
-                       timeout: Union[int, float, str] = 0,
-                       index: int = 1,
-                       **kwargs) -> None:
+def verify_input_value(
+    locator: Union[WebElement, str],
+    expected_value: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Verify input field has given value.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyInputValue    Username          Qentinel
@@ -378,26 +386,25 @@
     Related keywords
     ----------------
     \`GetInputValue\`, \`VerifyInputElement\`, \`VerifyInputStatus\`, \`VerifyInputValues\`
     """
     if isinstance(locator, WebElement):
         input_element = locator
     else:
-        input_element = input_.get_input_elements_from_all_documents(locator,
-                                                                     anchor,
-                                                                     timeout=timeout,
-                                                                     index=index,
-                                                                     **kwargs)
+        input_element = input_.get_input_elements_from_all_documents(
+            locator, anchor, timeout=timeout, index=index, **kwargs
+        )
     actions.compare_input_values(input_element, expected_value, timeout=timeout)
 
 
 @keyword(tags=("Input", "Verification"))
 @decorators.timeout_decorator
-def verify_input_values(input_values: Union[dict[str, str], str],
-                        timeout: Union[int, float, str] = '0') -> None:
+def verify_input_values(
+    input_values: Union[dict[str, str], str], timeout: Union[int, float, str] = "0"
+) -> None:
     r"""Verify input fields have given values.
 
     Accepts a .txt file or Robot FW dictionary as a parameter. If using a text file, the locator
     and the expected value should be separated with a comma on each row.
 
     Examples
     --------
@@ -412,39 +419,44 @@
 
     Related keywords
     ----------------
     \`VerifyInputValue\`
     """
     if isinstance(input_values, dict):
         for locator in input_values:
-            logger.info('Locator: {}, Expected value: {}'.format(locator, input_values[locator]),
-                        also_console=True)
+            logger.info(
+                "Locator: {}, Expected value: {}".format(locator, input_values[locator]),
+                also_console=True,
+            )
             verify_input_value(locator, input_values[locator])
-    elif input_values.endswith('.txt') or input_values.endswith('.csv'):
+    elif input_values.endswith(".txt") or input_values.endswith(".csv"):
         file = download.get_path(input_values)
-        with open(file, 'rb') as txt_file:
+        with open(file, "rb") as txt_file:
             params = [line.rstrip() for line in txt_file]
             for x_bytes in params:
-                x_str_list = x_bytes.decode('utf-8').split(',')
+                x_str_list = x_bytes.decode("utf-8").split(",")
                 locator, value = x_str_list[0].strip(), x_str_list[1].strip()
-                logger.info('Locator: {}, Expected value: {}'.format(locator, value),
-                            also_console=True)
+                logger.info(
+                    "Locator: {}, Expected value: {}".format(locator, value), also_console=True
+                )
                 verify_input_value(locator, value, timeout=timeout)
     else:
-        raise QWebValueError('Unknown input value. Text file or dictionary required.')
+        raise QWebValueError("Unknown input value. Text file or dictionary required.")
 
 
 @keyword(tags=("Input", "Verification"))
 @decorators.timeout_decorator
-def verify_input_status(locator: str,
-                        status: str,
-                        anchor: str = "1",
-                        timeout: Union[int, float, str] = 0,
-                        index: int = 1,
-                        **kwargs) -> None:
+def verify_input_status(
+    locator: str,
+    status: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Verify input field is enabled or disabled.
 
     In other words verify can user interact with an input field or not.
     Element is considered to be disabled if disabled or readonly attribute exists
 
 
     Examples
@@ -494,40 +506,35 @@
     QWebValueError
         If the field interaction is not the same
 
     Related keywords
     ----------------
     \`GetInputValue\`, \`VerifyInputElement\`, \`VerifyInputValue\`, \`VerifyInputValues\`
     """
-    input_element = input_.get_input_elements_from_all_documents(locator,
-                                                                 anchor,
-                                                                 timeout=timeout,
-                                                                 index=index,
-                                                                 enable_check=True,
-                                                                 **kwargs)
+    input_element = input_.get_input_elements_from_all_documents(
+        locator, anchor, timeout=timeout, index=index, enable_check=True, **kwargs
+    )
     if status.lower() == "enabled":
         if not element.is_enabled(input_element) or element.is_readonly(input_element):
-            raise QWebValueError('The input field was disabled')
+            raise QWebValueError("The input field was disabled")
     elif status.lower() == "disabled":
         if element.is_enabled(input_element):
-            raise QWebValueError('The input field was enabled')
+            raise QWebValueError("The input field was enabled")
     elif status.lower() == "readonly":
         if not element.is_readonly(input_element):
-            raise QWebValueError('readonly attr not found')
+            raise QWebValueError("readonly attr not found")
     else:
         raise QWebValueError('Unkown status: "{}"'.format(status))
 
 
 @keyword(tags=("Input", "Verification"))
 @decorators.timeout_decorator
-def verify_input_element(locator: str,
-                         anchor: str = "1",
-                         timeout: Union[int, float, str] = 0,
-                         index: int = 1,
-                         **kwargs) -> None:
+def verify_input_element(
+    locator: str, anchor: str = "1", timeout: Union[int, float, str] = 0, index: int = 1, **kwargs
+) -> None:
     r"""Verify that input element exist.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyInputElement   Username
@@ -569,30 +576,31 @@
     ------
     NoSuchElementException: Checkbox element not found
 
     Related keywords
     ----------------
     \`GetInputValue\`, \`VerifyInputStatus\`, \`VerifyInputValue\`, \`VerifyInputValues\`
     """
-    input_element = input_.get_input_elements_from_all_documents(locator,
-                                                                 anchor,
-                                                                 timeout=timeout,
-                                                                 index=index,
-                                                                 **kwargs)
+    input_element = input_.get_input_elements_from_all_documents(
+        locator, anchor, timeout=timeout, index=index, **kwargs
+    )
     if input_element:
         return
 
 
 @keyword(tags=("Input", "Getters"))
 @decorators.timeout_decorator
-def get_input_value(locator: str,
-                    anchor: str = "1",
-                    timeout: Union[int, float, str] = 0,
-                    index: int = 1,
-                    **kwargs) -> Union[int, float, str]:
+def get_input_value(
+    locator: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    remove_newlines: bool = True,
+    **kwargs,
+) -> Union[int, float, str]:
     r"""Get input value from input field.
 
     Examples
     --------
     .. code-block:: robotframework
 
        ${value}=    GetInputValue    OrderNro
@@ -622,14 +630,16 @@
         of matching entries starting with 1. Text selects the entry with the closest
         distance.
     timeout : str | int
         How long we find element before failing. Default 10 (seconds)
     index : int
         If table cell contains more than one input elements or if there is some kind of
         nested structure inside of given input index may needed. Default = 1 (first)
+    remove_newlines : bool
+        Removes new lines (\n)from string, especially from multirow text areas. Default = True
     kwargs :
         |  Accepted kwargs:
         |       limit_traverse : False. If limit traverse is set to false we are heading up to
         |       fifth parent element if needed when finding relative input element for some label.
         |       between : str/int - Start???End - Return all chars between texts Start and End.
         |       from_start : int - Return x amount of chars. Starting from first char
         |       from_end : int - Return x amount of chars. Starting from last char
@@ -641,31 +651,31 @@
         |       to True to allow partial match
         |       blind : True - Return empty instead of error if input element is empty
 
     Related keywords
     ----------------
     \`VerifyInputElement\`, \`VerifyInputStatus\`, \`VerifyInputValue\`, \`VerifyInputValues\`
     """
-    input_element = input_.get_input_elements_from_all_documents(locator,
-                                                                 anchor,
-                                                                 timeout=timeout,
-                                                                 index=index,
-                                                                 **kwargs)
+    input_element = input_.get_input_elements_from_all_documents(
+        locator, anchor, timeout=timeout, index=index, **kwargs
+    )
     val = actions.input_value(input_element, timeout=timeout, **kwargs)
-    return util.get_substring(val, **kwargs)
+    return util.get_substring(val, remove_newlines=remove_newlines, **kwargs)
 
 
 @keyword(tags=("File", "Input", "Interaction"))
 @decorators.timeout_decorator
-def upload_file(locator: str,
-                filename: str,
-                anchor: str = "1",
-                timeout: Union[int, float, str] = 0,
-                index: int = 1,
-                **kwargs) -> None:
+def upload_file(
+    locator: str,
+    filename: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Upload file.
 
     Examples
     --------
     .. code-block:: robotframework
 
        UploadFile   Upload      text.txt
@@ -704,36 +714,33 @@
     ------
     ValueError: File not found
 
     Related keywords
     ----------------
     \`SaveFile\`
     """
-    kwargs['css'] = kwargs.get('css', '[type="file"]')
-    kwargs['upload'] = util.par2bool(kwargs.get('upload', True))
+    kwargs["css"] = kwargs.get("css", '[type="file"]')
+    kwargs["upload"] = util.par2bool(kwargs.get("upload", True))
     filepath = download.get_path(filename)
     if filepath:
-        input_element = input_.get_input_elements_from_all_documents(locator,
-                                                                     anchor,
-                                                                     timeout=timeout,
-                                                                     index=index,
-                                                                     **kwargs)
+        input_element = input_.get_input_elements_from_all_documents(
+            locator, anchor, timeout=timeout, index=index, **kwargs
+        )
         input_element.send_keys(str(filepath.resolve()))
         return
     raise QWebFileNotFoundError(
-        'Unable to find file {}. Tried from project/files and users/downloads'.format(filename))
+        "Unable to find file {}. Tried from project/files and users/downloads".format(filename)
+    )
 
 
 @keyword(tags=("Input", "Interaction"))
 @decorators.timeout_decorator
-def press_key(locator: str,
-              key: str,
-              anchor: str = "1",
-              timeout: Union[int, float, str] = 0,
-              **kwargs) -> None:
+def press_key(
+    locator: str, key: str, anchor: str = "1", timeout: Union[int, float, str] = 0, **kwargs
+) -> None:
     r"""Simulate user pressing keyboard key on element identified by "locator".
 
     The parameter "key" is either a single character or a keyboard key combination
     surrounded by '{ }'.
 
     If ${EMPTY} is given as a locator, "global" hotkey combination is sent and handled by the OS.
 
@@ -793,47 +800,43 @@
     """
     # no locator given, "global" hotkey
     if not locator:
         try:
             checked_key = input_handler.check_key_pyautogui(key)
         except AttributeError as e:
             logger.console(str(e))
-            raise QWebValueError(f'Could not find key: {key}') from e
+            raise QWebValueError(f"Could not find key: {key}") from e
         return hotkey(*checked_key) if isinstance(checked_key, list) else hotkey(checked_key)
 
     driver = browser.return_browser()
     action = ActionChains(driver)
     try:
-        input_element = input_.get_input_elements_from_all_documents(locator,
-                                                                     anchor,
-                                                                     timeout=timeout,
-                                                                     index=1,
-                                                                     **kwargs)
+        input_element = input_.get_input_elements_from_all_documents(
+            locator, anchor, timeout=timeout, index=1, **kwargs
+        )
         key = input_handler.check_key(key)  # type: ignore[assignment]
 
         # COMMAND key workaround on safari
         # supports normal text field CMD operations only
         # (i.e. CMD+C, CMD+A, CMD+V etc.)
-        if len(key) == 2 and key[0] == '\ue03d' and util.is_safari():
+        if len(key) == 2 and key[0] == "\ue03d" and util.is_safari():
             javascript.execute_javascript("arguments[0].focus();", input_element)
-            action.key_down(key[0]) \
-                  .send_keys(key[1]) \
-                  .key_up(key[0]).perform()
+            action.key_down(key[0]).send_keys(key[1]).key_up(key[0]).perform()
         else:
             input_element.send_keys(key)
     except AttributeError as e:
         logger.console(str(e))
         raise QWebValueError(f'Could not find key "{key}"') from e
     return None
 
 
 @keyword(tags=("Browser", "Interaction"))
-def scroll(locator: str,
-           direction: str = 'pagedown',
-           timeout: Union[int, float, str] = 0, **kwargs) -> None:
+def scroll(
+    locator: str, direction: str = "pagedown", timeout: Union[int, float, str] = 0, **kwargs
+) -> None:
     r"""Scrolls the page/element to given direction.
 
     Examples
     --------
     .. code-block:: robotframework
 
         # Scroll page down default value (one page)
@@ -874,22 +877,24 @@
         If the given scrollable element is not found.
 
     Related keywords
     ----------------
     \`ScrollTo\`, \`ScrollText\`
     """
 
-    keys = {"pagedown": "{PAGE_DOWN}",
-            "pageup": "{PAGE_UP}",
-            "top": "{HOME}",
-            "bottom": "{END}",
-            "up": "{ARROW_UP}",
-            "down": "{ARROW_DOWN}",
-            "left": "{ARROW_LEFT}",
-            "right": "{ARROW_RIGHT}"}
+    keys = {
+        "pagedown": "{PAGE_DOWN}",
+        "pageup": "{PAGE_UP}",
+        "top": "{HOME}",
+        "bottom": "{END}",
+        "up": "{ARROW_UP}",
+        "down": "{ARROW_DOWN}",
+        "left": "{ARROW_LEFT}",
+        "right": "{ARROW_RIGHT}",
+    }
 
     try:
         key = keys[direction.lower().replace("_", "")]
     except KeyError as e:
         raise QWebValueError("""Unknown 'direction'. Valid values are: page_down,
                              page_up, down, up, left, right, top, bottom""") from e
     press_key(locator, key, timeout=timeout, **kwargs)
```

### Comparing `QWeb-3.2.1/QWeb/keywords/javascript.py` & `QWeb-3.3.0/QWeb/keywords/javascript.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,14 @@
     ----------
     script : str
         Javascript code.
     variable_name : str
         Robot framework variable name without {}. (Default None)
     """
     output = javascript.execute_javascript(script)
-    logger.info(f'Output of execution:\n{output}')
+    logger.info(f"Output of execution:\n{output}")
     if variable_name:
         try:
             BuiltIn().set_suite_variable(variable_name, output)
         except Exception as e:
             logger.warn(str(e))
             raise QWebValueError(f"Invalid variable syntax '{variable_name}'.") from e
```

### Comparing `QWeb-3.2.1/QWeb/keywords/lists.py` & `QWeb-3.3.0/QWeb/keywords/lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,37 +16,43 @@
 # ---------------------------
 """Keywords for table elements.
 
 List elements are used to show many kinds of data. Lists have cells in
 contain rows and columns. Cells can contain all kinds of elements. Cells
 are usually referenced by coordinates or unique neighboring values.
 """
+
 from __future__ import annotations
 from typing import Union, Optional
 
 from robot.api.deco import keyword
-from QWeb.internal.exceptions import QWebInstanceDoesNotExistError, QWebValueMismatchError, \
-    QWebValueError
-from QWeb.internal.actions import execute_click_and_verify_condition \
-    as _execute_click_and_verify_condition
+from QWeb.internal.exceptions import (
+    QWebInstanceDoesNotExistError,
+    QWebValueMismatchError,
+    QWebValueError,
+)
+from QWeb.internal.actions import (
+    execute_click_and_verify_condition as _execute_click_and_verify_condition,
+)
 from QWeb.internal import decorators, util, element
 from QWeb.internal.lists import List
 
 ACTIVE_LIST: List = None  # type: ignore[assignment]
 
 
 @keyword(tags=("Config", "Lists"))
 @decorators.timeout_decorator
 def use_list(
-        locator: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        parent: Optional[str] = None,
-        child: Optional[str] = None,
-        **kwargs) -> None:
+    locator: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    parent: Optional[str] = None,
+    child: Optional[str] = None,
+    **kwargs,
+) -> None:
     r"""Define list for all other list keywords.
 
     Sets active table for other keywords.
 
     Examples
     --------
     .. code-block:: robotframework
@@ -90,22 +96,26 @@
     if _list_exists():
         active = ACTIVE_LIST.update_list()
         list_length = len(active.web_list)
         if int(expected_length) == list_length:
             return
         raise QWebValueMismatchError(
             'Expected length "{}" didn\'t match to list length "{}".'.format(
-                expected_length, list_length))
+                expected_length, list_length
+            )
+        )
 
 
 @keyword(tags=("Lists", "Verification"))
 @decorators.timeout_decorator
-def verify_list(text: str,
-                index: Optional[Union[int, str]] = None,
-                timeout: Union[int, float, str] = 0) -> None:  # pylint: disable=unused-argument
+def verify_list(
+    text: str,
+    index: Optional[Union[int, str]] = None,
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+) -> None:
     r"""Verify list contains given text.
 
     Examples
     --------
     .. code-block:: robotframework
 
         UseList         Qentinel
@@ -124,18 +134,17 @@
         if active.contains(text, idx):
             return
         raise QWebValueError('List didn\'t contain text "{}"'.format(text))
 
 
 @keyword(tags=("Lists", "Interaction"))
 @decorators.timeout_decorator
-def click_list(index: Union[int, str],
-               timeout: Union[int, float, str] = 0,
-               js: bool = True,
-               **kwargs) -> None:
+def click_list(
+    index: Union[int, str], timeout: Union[int, float, str] = 0, js: bool = True, **kwargs
+) -> None:
     r"""Click list element with in given index.
 
     Examples
     --------
     .. code-block:: robotframework
 
         ClickList       1
@@ -145,16 +154,17 @@
     ----------------
     \`GetList\`, \`UseList\`, \`VerifyList\`
     """
     if _list_exists():
         active = ACTIVE_LIST.update_list()
         if index:
             index = _check_index(index)
-            web_element = element.get_element_to_click_from_list(active.web_element_list, index,
-                                                                 **kwargs)
+            web_element = element.get_element_to_click_from_list(
+                active.web_element_list, index, **kwargs
+            )
             if _execute_click_and_verify_condition(web_element, timeout=timeout, js=js, **kwargs):
                 return
 
 
 @keyword(tags=("Lists", "Verification"))
 def verify_no_list(text: str, index: Optional[Union[int, str]] = None) -> None:
     r"""Verify that text is not in the list.
@@ -178,16 +188,17 @@
             idx = _check_index(index)
         if not active.contains(text, idx):
             return
         raise QWebValueMismatchError('List contains text "{}"'.format(text))
 
 
 @keyword(tags=("Lists", "Getters"))
-def get_list(index: Optional[Union[int, str]] = None,
-             **kwargs) -> Union[str, int, float, list[str]]:
+def get_list(
+    index: Optional[Union[int, str]] = None, **kwargs
+) -> Union[str, int, float, list[str]]:
     r"""Get value(s) from a list.
 
     Examples
     --------
     .. code-block:: robotframework
 
         UseList         Qentinel
@@ -220,18 +231,18 @@
         text = active.web_list[index]
         return util.get_substring(text, **kwargs)
     return active.web_list
 
 
 def _list_exists() -> bool:
     if isinstance(ACTIVE_LIST, List) is False:
-        raise QWebInstanceDoesNotExistError('List has not been defined with UseList keyword')
+        raise QWebInstanceDoesNotExistError("List has not been defined with UseList keyword")
     return True
 
 
 def _check_index(index: Union[int, str]) -> int:
     try:
         if int(index) - 1 < len(ACTIVE_LIST.web_list):
             return int(index) - 1
-        raise QWebValueError('Index can\'t be bigger than length of the list')
+        raise QWebValueError("Index can't be bigger than length of the list")
     except TypeError as e:
-        raise QWebValueError('Index has to be number') from e
+        raise QWebValueError("Index has to be number") from e
```

### Comparing `QWeb-3.2.1/QWeb/keywords/screenshot.py` & `QWeb-3.3.0/QWeb/keywords/screenshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     """Compare image to a known good one.
 
     :param imagename:
     :return:
     """
     status = screenshot.compare_screenshots(imagename, CONFIG["VerifyAppAccuracy"])
     if status is False:
-        raise ValueError('Images differ')
+        raise ValueError("Images differ")
 
 
 @keyword(tags=["Logging"])
-def log_screenshot(filename: str = 'screenshot_{}.png', fullpage: bool = False) -> Optional[str]:
+def log_screenshot(filename: str = "screenshot_{}.png", fullpage: bool = False) -> Optional[str]:
     r"""Log screenshot to Robot Framework log.
 
     Examples
     --------
     .. code-block:: robotframework
 
        LogScreenshot
@@ -64,22 +64,22 @@
     Related keywords
     ----------------
     \`LogPage\`
     """
     filepath: Optional[str] = None
     if CONFIG["LogScreenshot"]:
         screenshot_type = CONFIG["ScreenshotType"]
-        if screenshot_type == 'screenshot':
+        if screenshot_type == "screenshot":
             filepath = screenshot.save_screenshot(filename, fullpage=fullpage)
             screenshot.log_screenshot_file(filepath)
-        elif screenshot_type == 'html':
+        elif screenshot_type == "html":
             screenshot.log_html()
-        elif screenshot_type == 'all':
+        elif screenshot_type == "all":
             filepath = screenshot.save_screenshot(filename, fullpage=fullpage)
             screenshot.log_screenshot_file(filepath)
             screenshot.log_html()
         else:
-            raise ValueError('Unknown screenshot type: {}'.format(screenshot_type))
+            raise ValueError("Unknown screenshot type: {}".format(screenshot_type))
     else:
-        logger.info('Screenshots have been disabled with the SetConfig keyword.')
+        logger.info("Screenshots have been disabled with the SetConfig keyword.")
 
     return filepath
```

### Comparing `QWeb-3.2.1/QWeb/keywords/search_strategy.py` & `QWeb-3.3.0/QWeb/keywords/search_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,19 @@
     ValueError
         Wrong strategy type
     """
     if strategy_type == "all input elements":
         previous = config.set_config("AllInputElements", xpath)
     elif strategy_type == "matching input element":
         previous = config.set_config("MatchingInputElement", xpath)
-    elif strategy_type == 'active area xpath':
+    elif strategy_type == "active area xpath":
         previous = config.set_config("ActiveAreaXpath", xpath)
-    elif strategy_type == 'text':
+    elif strategy_type == "text":
         previous = config.set_config("TextMatch", xpath)
-    elif strategy_type == 'containing text':
+    elif strategy_type == "containing text":
         previous = config.set_config("ContainingTextMatch", xpath)
     else:
         raise ValueError("Wrong strategy type")
     return previous
 
 
 def default_timeout(timeout: Union[int, float, str]) -> Union[int, str]:
@@ -250,13 +250,15 @@
 
         CaseInsensitive    True
         CaseInsensitive    False
 
     """
     case_state = config.set_config("CaseInsensitive", state)
     if case_state:
-        config.set_config("ContainingTextMatch",
-                          SearchStrategies.CONTAINING_TEXT_MATCH_CASE_INSENSITIVE)
+        config.set_config(
+            "ContainingTextMatch", SearchStrategies.CONTAINING_TEXT_MATCH_CASE_INSENSITIVE
+        )
     else:
-        config.set_config("ContainingTextMatch",
-                          SearchStrategies.CONTAINING_TEXT_MATCH_CASE_SENSITIVE)
+        config.set_config(
+            "ContainingTextMatch", SearchStrategies.CONTAINING_TEXT_MATCH_CASE_SENSITIVE
+        )
     return case_state
```

### Comparing `QWeb-3.2.1/QWeb/keywords/table.py` & `QWeb-3.3.0/QWeb/keywords/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,37 +16,43 @@
 # ---------------------------
 """Keywords for table elements.
 
 Table elements are used to show many kinds of data. Tables have cells in
 contain rows and columns. Cells can contain all kinds of elements. Cells
 are usually refenced by coordinates or unique neighbouring values.
 """
+
 from typing import Union, List, Optional
 
 from selenium.webdriver.remote.webelement import WebElement
 from robot.api.deco import keyword
 from QWeb.internal import decorators, actions, util
-from QWeb.internal.exceptions import QWebInstanceDoesNotExistError, \
-    QWebTimeoutError, QWebValueError, QWebElementNotFoundError
+from QWeb.internal.exceptions import (
+    QWebInstanceDoesNotExistError,
+    QWebTimeoutError,
+    QWebValueError,
+    QWebElementNotFoundError,
+)
 from QWeb.internal.table import Table
 from QWeb.internal.config_defaults import CONFIG
 
 ACTIVE_TABLE: Table = None  # type: ignore[assignment]
 
 
 @keyword(tags=["Tables"])
 @decorators.timeout_decorator
 def use_table(
-        locator: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        parent: bool = False,
-        child: bool = False,
-        level: int = 1,
-        index: int = 1) -> None:
+    locator: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    parent: bool = False,
+    child: bool = False,
+    level: int = 1,
+    index: int = 1,
+) -> None:
     r"""Define table for all other table keywords.
 
     Sets active table for other keywords.
 
     Examples
     --------
     .. code-block:: robotframework
@@ -87,19 +93,21 @@
     """
     global ACTIVE_TABLE  # pylint:disable=global-statement
     ACTIVE_TABLE = Table.from_table_instance(locator, anchor, parent, child, level, index)
 
 
 @keyword(tags=("Tables", "Verification"))
 @decorators.timeout_decorator
-def verify_table(coordinates: str,
-                 expected: str,
-                 anchor: str = "1",
-                 timeout: Union[int, float, str] = 0,
-                 **kwargs) -> None:
+def verify_table(
+    coordinates: str,
+    expected: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    **kwargs,
+) -> None:
     r"""Verify text in table coordinates.
 
     Reads cell value from coordinates in active table and verifies it
     against expected value.
 
     Examples
     --------
@@ -141,29 +149,30 @@
         If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`ClickCell\`, \`GetCellText\`, \`GetTableRow\`, \`UseTable\`
     """
     if not isinstance(ACTIVE_TABLE, Table):
-        raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
     table = Table.ACTIVE_TABLE.update_table()
 
     table_cell = table.ACTIVE_TABLE.get_table_cell(coordinates, anchor, **kwargs)
-    partial_match = util.par2bool(kwargs.get('partial_match', CONFIG['PartialMatch']))
-    expected = f"{expected}*" if partial_match else expected
-    actions.get_element_text(table_cell, expected=expected, timeout=timeout)
+    partial_match = util.par2bool(kwargs.get("partial_match", CONFIG["PartialMatch"]))
+
+    actions.get_element_text(
+        table_cell, expected=expected, timeout=timeout, partial_match=partial_match
+    )
 
 
 @keyword(tags=("Tables", "Getters"))
 @decorators.timeout_decorator
-def get_cell_text(coordinates: str,
-                  anchor: str = "1",
-                  timeout: Union[int, float, str] = 0,
-                  **kwargs) -> Union[str, int, float]:
+def get_cell_text(
+    coordinates: str, anchor: str = "1", timeout: Union[int, float, str] = 0, **kwargs
+) -> Union[str, int, float]:
     r"""Get cell text to variable.
 
     Locates cell by coordinates from active table and return value
 
     Examples
     --------
     .. code-block:: robotframework
@@ -199,33 +208,34 @@
         If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`ClickCell\`, \`GetTableRow\`, \`UseTable\`, \`VerifyTable\`
     """
     if not isinstance(ACTIVE_TABLE, Table):
-        raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
     table = Table.ACTIVE_TABLE.update_table()
 
     table_cell = table.get_table_cell(coordinates, anchor)
     try:
         text = actions.get_element_text(table_cell, timeout=timeout)
         return util.get_substring(text, **kwargs)
     except QWebTimeoutError:
         return ""
 
 
 @keyword(tags=("Tables", "Interaction"))
 @decorators.timeout_decorator
 def click_cell(
-        coordinates: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        index: int = 1,
-        **kwargs) -> None:
+    coordinates: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    index: int = 1,
+    **kwargs,
+) -> None:
     r"""Click table cell.
 
     Locates cell by coordinates or text from active table and clicks it
 
     Examples
     --------
     .. code-block:: robotframework
@@ -268,28 +278,29 @@
        If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`GetCellText\`, \`GetTableRow\`, \`UseTable\`, \`VerifyTable\`
     """
     if not isinstance(ACTIVE_TABLE, Table):
-        raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
     table = Table.ACTIVE_TABLE.update_table()
 
     table_cell = table.get_clickable_cell(coordinates, anchor, index, **kwargs)
     actions.execute_click_and_verify_condition(table_cell, **kwargs)
 
 
 @keyword(tags=("Tables", "Getters"))
 @decorators.timeout_decorator
 def get_table_row(
-        locator: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        **kwargs) -> Union[WebElement, int]:
+    locator: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    **kwargs,
+) -> Union[WebElement, int]:
     r"""Get row (index) from current table.
 
     Get table row by some visible text or value.
 
     Examples
     --------
     .. code-block:: robotframework
@@ -316,15 +327,15 @@
        If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`ClickCell\`, \`GetCellText\`, \`UseTable\`, \`VerifyTable\`
     """
     if not isinstance(ACTIVE_TABLE, Table):
-        raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
     table = Table.ACTIVE_TABLE.update_table()
 
     return table.get_row(locator, anchor, row_index=True, **kwargs)
 
 
 @keyword(tags=("Tables", "Getters"))
 def get_col_header_count() -> int:
@@ -345,15 +356,15 @@
        If the table is not defined by UseTable keyword
 
     Related keywords
     ----------------
     \`GetColHeader\`, \`VerifyColHeader\`, \`UseTable\`, \`VerifyTable\`
     """
     if not isinstance(ACTIVE_TABLE, Table):
-        raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
     table = Table.ACTIVE_TABLE.update_table()
     return len(table.get_columns())
 
 
 @keyword(tags=("Tables", "Getters"))
 def get_col_header(index: Optional[int] = None) -> Union[str, List[str]]:
     r"""Get column header names/text as a list.
@@ -395,36 +406,34 @@
         Index argument is not an integer.
 
     Related keywords
     ----------------
     \`GetColHeaderCount\`, \`VerifyColHeader\`, \`GetColHeader\`, \`UseTable\`, \`VerifyTable\`
     """
     if not isinstance(ACTIVE_TABLE, Table):
-        raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
     table = Table.ACTIVE_TABLE.update_table()
     columns = table.get_columns()
 
     column_texts = _get_column_header_texts(columns)
 
     if not index:
         return column_texts
 
     if not str(index).isdigit():
-        raise QWebValueError('Column index should be a positive integer')
+        raise QWebValueError("Column index should be a positive integer")
 
     if len(columns) < index:
-        raise QWebValueError(f'Column index out of range: {index=}, {len(columns)=}')
+        raise QWebValueError(f"Column index out of range: {index=}, {len(columns)=}")
 
     return column_texts[index - 1]
 
 
 @keyword(tags=("Tables", "Verification"))
-def verify_col_header(expected: str,
-                      index: Optional[int] = None,
-                      **kwargs) -> bool:
+def verify_col_header(expected: str, index: Optional[int] = None, **kwargs) -> bool:
     r"""Verifies that a column header with given index matches the expected text.
 
     Note: only visible columns may be counted in some dynamic tables.
 
     Note2: If column header has attribute 'aria-label', it's value is considered as expected value.
     If not and 'title' attribute exists, then title is considered as expected value.
     If neither aria-label or title exists, then column text is considered as expected value.
@@ -469,19 +478,19 @@
 
 
     Related keywords
     ----------------
     \`GetColHeaderCount\`, \`GetColHeader\`, \`UseTable\`, \`VerifyTable\`
     """
     if not isinstance(ACTIVE_TABLE, Table):
-        raise QWebInstanceDoesNotExistError('Table has not been defined with UseTable keyword')
+        raise QWebInstanceDoesNotExistError("Table has not been defined with UseTable keyword")
     table = Table.ACTIVE_TABLE.update_table()
     columns = table.get_columns()
     column_texts = _get_column_header_texts(columns)
-    partial = kwargs.get('partial_match', CONFIG['PartialMatch'])
+    partial = kwargs.get("partial_match", CONFIG["PartialMatch"])
 
     # If index is not specified, verify that the expected text is in any column
     if not index:
         # accept partial match
         if util.par2bool(partial):
             found = found = any(expected in c for c in column_texts)
         # full match
@@ -489,18 +498,18 @@
             found = expected in column_texts
         if found:
             return True
 
         raise QWebElementNotFoundError(f'Column text "{expected}" does not exist.')
 
     if not str(index).isdigit():
-        raise QWebValueError('Column index should be a positive integer')
+        raise QWebValueError("Column index should be a positive integer")
 
     if len(columns) < index:
-        raise QWebValueError(f'Column index out of range: {index=}, {len(columns)=}')
+        raise QWebValueError(f"Column index out of range: {index=}, {len(columns)=}")
 
     actual = column_texts[index - 1]
     # accept partial match
     if util.par2bool(partial) and expected in actual:
         return True
 
     # full match
@@ -509,14 +518,11 @@
 
     raise QWebElementNotFoundError(f'Column "{index}" "{actual}" does not match "{expected}".')
 
 
 def _get_column_header_texts(columns: List[WebElement]) -> List[str]:
     # prefer using title, then aria-label, then text
     column_texts = [
-        c.get_attribute("aria-label")
-        or c.get_attribute("title")
-        or c.text
-        for c in columns
+        c.get_attribute("aria-label") or c.get_attribute("title") or c.text for c in columns
     ]
 
     return column_texts
```

### Comparing `QWeb-3.2.1/QWeb/keywords/text.py` & `QWeb-3.3.0/QWeb/keywords/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,39 +18,50 @@
 # ---------------------------
 """Keywords for text elements.
 
 Text elements are considered to be elements that have visible text. Input
 elements are not considered text elements even though they might have visible
 text.
 """
+
 from __future__ import annotations
 from typing import Union, Optional
 from pynput.keyboard import Controller
 import pyperclip
-from QWeb.internal.actions import scroll as _scroll, \
-    execute_click_and_verify_condition as _execute_click_and_verify_condition, \
-    hover_to as _hover_to, text_appearance as _text_appearance, \
-    scroll_dynamic_web_page as _scroll_dynamic_web_page, \
-    scroll_first_scrollable_parent_element as _scroll_first_scrollable_parent_element
+from QWeb.internal.actions import (
+    scroll as _scroll,
+    execute_click_and_verify_condition as _execute_click_and_verify_condition,
+    hover_to as _hover_to,
+    text_appearance as _text_appearance,
+    scroll_dynamic_web_page as _scroll_dynamic_web_page,
+    scroll_first_scrollable_parent_element as _scroll_first_scrollable_parent_element,
+)
 from QWeb.internal import element, decorators, util, download, text as internal_text
 from QWeb.internal.config_defaults import CONFIG
-from QWeb.internal.exceptions import QWebValueError, QWebEnvironmentError, QWebTimeoutError, \
-    QWebElementNotFoundError, QWebDriverError, QWebInstanceDoesNotExistError
+from QWeb.internal.exceptions import (
+    QWebValueError,
+    QWebEnvironmentError,
+    QWebTimeoutError,
+    QWebElementNotFoundError,
+    QWebDriverError,
+    QWebInstanceDoesNotExistError,
+)
 from robot.api import logger
 from robot.api.deco import keyword
 import os
 
 
 @keyword(tags=("Text", "Verification"))
 @decorators.timeout_decorator
 def verify_text(
-        text: str,
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        anchor: str = "1",
-        **kwargs) -> None:
+    text: str,
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    anchor: str = "1",
+    **kwargs,
+) -> None:
     r"""Verify page contains given text.
 
     Keyword waits until timeout has passed. If timeout is not specified, it
     uses default timeout that can be adjusted with DefaultTimeout keyword.
 
     VerifyText does not require for the text to be unique.
 
@@ -126,16 +137,16 @@
     Related keywords
     ----------------
     \`VerifyAlertText\`, \`VerifyAll\`, \`VerifyAny\`, \`VerifyAttribute\`, \`VerifyCheckbox\`,
     \`VerifyElement\`, \`VerifyIcon\`, \`VerifyInputValue\`, \`VerifyItem\`, \`VerifyLinks\`,
     \`VerifyNoText\`, \`VerifyOption\`, \`VerifyPdfText\`, \`VerifySelectedOption\`,
     \`VerifyTable\`, \`VerifyTitle\`, \`VerifyUrl\`
     """
-    kwargs['css'] = False
-    window_find = util.par2bool(kwargs.get('window_find', CONFIG['WindowFind']))
+    kwargs["css"] = False
+    window_find = util.par2bool(kwargs.get("window_find", CONFIG["WindowFind"]))
     if window_find:
         web_elements = internal_text.find_text(text)
     else:
         web_elements = internal_text.get_element_by_locator_text(text, anchor, **kwargs)
     if web_elements:
         return
 
@@ -192,30 +203,31 @@
     instead of text() since text() does not handle cases where the text is
     in both the a parent node and in its child node.
 
     Related keywords
     ----------------
     \`VerifyText\`
     """
-    kwargs['css'] = False
-    web_elements = internal_text.get_element_by_locator_text(text,
-                                                             allow_non_existent=True,
-                                                             **kwargs)
+    kwargs["css"] = False
+    web_elements = internal_text.get_element_by_locator_text(
+        text, allow_non_existent=True, **kwargs
+    )
     if not web_elements:
         return
     raise QWebValueError('Page contained the text "{}" after timeout'.format(text))
 
 
 @keyword(tags=("Text", "Verification"))
 @decorators.timeout_decorator
 def verify_text_count(
-        text: str,
-        expected_count: Union[int, str],
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        **kwargs) -> None:
+    text: str,
+    expected_count: Union[int, str],
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    **kwargs,
+) -> None:
     r"""Verify page contains given text given times.
 
     Keyword waits until timeout has passed. If timeout is not specified, it
     uses default timeout that can be adjusted with DefaultTimeout keyword.
 
     VerifyTextCount does not require for the text to be unique.
 
@@ -263,26 +275,29 @@
     in both the a parent node and in its child node.
 
     Related keywords
     ----------------
     \`GetElementCount\`, \`GetTextCount\`
     """
     expected_count = int(expected_count)
-    kwargs['css'] = False
+    kwargs["css"] = False
     try:
         webelements = internal_text.get_all_text_elements(text, **kwargs)
         element_count = len(webelements)
     except QWebElementNotFoundError:
         element_count = 0
 
     if element_count == expected_count:
         return
 
-    raise QWebValueError('Page contained {0} texts instead of {1} after timeout'.format(
-        element_count, expected_count))
+    raise QWebValueError(
+        "Page contained {0} texts instead of {1} after timeout".format(
+            element_count, expected_count
+        )
+    )
 
 
 @keyword(tags=("Text", "Getters"))
 @decorators.timeout_decorator
 def get_text_count(text: str, timeout: Union[int, float, str] = 0, **kwargs) -> int:  # pylint: disable=unused-argument
     r"""Get count of appearances for given text.
 
@@ -317,28 +332,30 @@
         css=False/off: Use this to bypass css search when finding elements
         by visible text
 
     Related keywords
     ----------------
     \`GetElementCount\`, \`VerifyTextCount\`
     """
-    kwargs['css'] = False
+    kwargs["css"] = False
     web_elements = internal_text.get_all_text_elements(text, **kwargs)
     return len(web_elements)
 
 
 @keyword(tags=("Text", "Interaction"))
 @decorators.timeout_decorator
-def click_text(text: str,
-               anchor: str = "1",
-               timeout: Union[int, float, str] = 0,
-               parent: Optional[str] = None,
-               child: Optional[str] = None,
-               js: bool = False,
-               **kwargs) -> None:
+def click_text(
+    text: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    parent: Optional[str] = None,
+    child: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     r"""Click text on web page.
 
     Keyword looks for an exact match and if not found uses xpath defined in
     Search Strategy. If the given text corresponds to multiple elements, it
     clicks the first element.
 
     If you want to click other element than the first one found, you need to
@@ -436,33 +453,32 @@
 
     Related keywords
     ----------------
     \`ClickElement\`, \`ClickItem\`, \`GetText\`, \`RightClick\`, \`VerifyText\`
     """
     anchor = str(anchor)
 
-    web_element = internal_text.get_element_by_locator_text(text,
-                                                            anchor,
-                                                            parent=parent,
-                                                            child=child,
-                                                            **kwargs)
+    web_element = internal_text.get_element_by_locator_text(
+        text, anchor, parent=parent, child=child, **kwargs
+    )
     if _execute_click_and_verify_condition(web_element, timeout=timeout, js=js, **kwargs):
         return
 
 
 def scan_click(
-        text: str,
-        text_to_appear: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,
-        interval: Optional[str] = None,
-        parent: Optional[str] = None,  # pylint: disable=unused-argument
-        child: Optional[str] = None,  # pylint: disable=unused-argument
-        js: bool = False,  # pylint: disable=unused-argument
-        **kwargs) -> None:
+    text: str,
+    text_to_appear: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    interval: Optional[str] = None,
+    parent: Optional[str] = None,  # pylint: disable=unused-argument
+    child: Optional[str] = None,  # pylint: disable=unused-argument
+    js: bool = False,  # pylint: disable=unused-argument
+    **kwargs,
+) -> None:
     """*DEPRECATED!!* Use keyword `ClickUntil` instead.
 
     Click text until a text appears.
 
     This keyword is required on slow pages where it takes time for a button
     listener to start. This clicks button and waits until text appears.
 
@@ -496,38 +512,42 @@
         If set to true, uses javascript instead of selenium to click element.
     Accepted kwargs:
         css=False/off: Use this to bypass css search when finding elements
         by visible text.
         el_type=item
         text(default) = find element by visible text | item = find item type element
     """
-    el_type = kwargs.get('el_type', 'text')
-    if el_type.lower() != 'text':
+    el_type = kwargs.get("el_type", "text")
+    if el_type.lower() != "text":
         click_item_until(text_to_appear, text, anchor, timeout, interval, js=False, **kwargs)
     else:
-        click_until(text_to_appear,
-                    text,
-                    anchor,
-                    timeout,
-                    interval,
-                    parent=None,
-                    child=None,
-                    js=False,
-                    **kwargs)
-
-
-def skim_click(text: str,
-               text_to_disappear: str = '',
-               anchor: str = "1",
-               timeout: Union[int, float, str] = 0,
-               interval: Optional[str] = None,
-               parent: Optional[str] = None,
-               child: Optional[str] = None,
-               js: bool = False,
-               **kwargs) -> None:
+        click_until(
+            text_to_appear,
+            text,
+            anchor,
+            timeout,
+            interval,
+            parent=None,
+            child=None,
+            js=False,
+            **kwargs,
+        )
+
+
+def skim_click(
+    text: str,
+    text_to_disappear: str = "",
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    interval: Optional[str] = None,
+    parent: Optional[str] = None,
+    child: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     """*DEPRECATED!!* Use keyword `ClickWhile` instead.
 
     Click text until a text disappears.
 
     This keyword is required on slow pages where it takes time for a button
     listener to start. This clicks button and waits until text disappears.
 
@@ -566,29 +586,28 @@
         If set to true, uses javascript instead of selenium to click element.
     Accepted kwargs:
         css=False/off: Use this to bypass css search when finding elements
         by visible text
         el_type = 'item':
         text(default) = find element by visible text | item = find item type element
     """
-    el_type = kwargs.get('el_type', 'text')
-    if text_to_disappear == '':
+    el_type = kwargs.get("el_type", "text")
+    if text_to_disappear == "":
         text_to_disappear = text
-    if el_type.lower() != 'text':
+    if el_type.lower() != "text":
         click_item_while(text_to_disappear, text, anchor, timeout, interval, js=js, **kwargs)
     else:
         click_while(text_to_disappear, text, anchor, timeout, interval, parent, child, js, **kwargs)
 
 
 @keyword(tags=("Text", "Interaction"))
 @decorators.timeout_decorator
-def hover_text(text: str,
-               anchor: str = "1",
-               timeout: Union[int, float, str] = "0",
-               **kwargs) -> None:
+def hover_text(
+    text: str, anchor: str = "1", timeout: Union[int, float, str] = "0", **kwargs
+) -> None:
     r"""Hover over text.
 
     Keyword will fail if text is not visible. You should use VerifyText before HoverText
     if you are not sure text is already visible.
 
     Examples
     --------
@@ -619,18 +638,17 @@
     """
     web_element = internal_text.get_element_by_locator_text(text, anchor, **kwargs)
     _hover_to(web_element, timeout=timeout)
 
 
 @keyword(tags=("Item", "Verification"))
 @decorators.timeout_decorator
-def hover_item(locator: str,
-               anchor: str = "1",
-               timeout: Union[int, float, str] = "0",
-               **kwargs) -> None:
+def hover_item(
+    locator: str, anchor: str = "1", timeout: Union[int, float, str] = "0", **kwargs
+) -> None:
     r"""Hover over item.
 
     Hover over web element.
 
     Examples
     --------
     .. code-block:: robotframework
@@ -745,19 +763,21 @@
         return _text_appearance(text, text_appear=False, timeout=timeout, **kwargs)
     except (QWebValueError, QWebTimeoutError):
         return False
 
 
 @keyword(tags=("Text", "Verification"))
 @decorators.timeout_decorator
-def verify_element_text(locator: str,
-                        text_to_find: str,
-                        timeout: Union[int, float, str] = 0,
-                        anchor: str = "1",
-                        **kwargs) -> None:
+def verify_element_text(
+    locator: str,
+    text_to_find: str,
+    timeout: Union[int, float, str] = 0,
+    anchor: str = "1",
+    **kwargs,
+) -> None:
     r"""Verify that element contains specified text.
 
     Examples
     --------
     .. code-block:: robotframework
 
         VerifyElementText       //input[@value\="Button3"]      ButtonText
@@ -779,31 +799,32 @@
         |       strict : bool - Verify that the texts are an exact match.
 
     Related keywords
     ----------------
     \`GetText\`, \`IsText\`, \`VerifyText\`
     """
     locator_text = get_text(locator, timeout, anchor, **kwargs)
-    strict = util.par2bool(kwargs.get('strict', False))
+    strict = util.par2bool(kwargs.get("strict", False))
     if strict:  # exact match
         if text_to_find == locator_text:
             return
         raise QWebValueError(f'"{text_to_find}" != "{locator_text}"')
     if text_to_find in locator_text:
         return
     raise QWebValueError(f'"{text_to_find}" not in "{locator_text}"')
 
 
 @keyword(tags=("Text", "Getters"))
 @decorators.timeout_decorator
 def get_text(
-        locator: str,
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        anchor: str = "1",
-        **kwargs) -> Union[str, int, float]:
+    locator: str,
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    anchor: str = "1",
+    **kwargs,
+) -> Union[str, int, float]:
     r"""Get text from element specified by xpath.
 
     Examples
     --------
     .. code-block:: robotframework
 
         GetText          //*[@id\="click_me"]
@@ -858,50 +879,49 @@
     text : Xpath value text
 
     Related keywords
     ----------------
     \`Is Text\`, \`VerifyText\`
     """
     anchor_int = util.anchor_to_index(anchor)
-    tag = kwargs.pop('tag', None)
+    tag = kwargs.pop("tag", None)
     if tag:
         try:
-            kwargs['element_kw'] = True
-            shadow_dom = CONFIG['ShadowDOM']
+            kwargs["element_kw"] = True
+            shadow_dom = CONFIG["ShadowDOM"]
             if shadow_dom:
-                web_element = internal_text.get_items_including_shadow_dom(locator,
-                                                                           tag,
-                                                                           **kwargs)[anchor_int]
+                web_element = internal_text.get_items_including_shadow_dom(locator, tag, **kwargs)[
+                    anchor_int
+                ]
             else:
                 web_element = element.get_elements_by_attributes(tag, locator, **kwargs)[anchor_int]
         except ValueError as e:
             raise QWebValueError(
-                'Only index is allowed anchor when searching element by it\'s attribute') from e
-    elif '//' not in locator:
+                "Only index is allowed anchor when searching element by it's attribute"
+            ) from e
+    elif "//" not in locator:
         # css=False means we include non-clickable texts
         web_element = internal_text.get_text_using_anchor(locator, anchor, css=False, **kwargs)
     else:
         web_element = element.get_unique_element_by_xpath(locator, index=anchor_int, **kwargs)
     # selenium's .text does not see all texts directly under slots
     # use innerText as a backup
     # note that "" at the end is important so that we don't get None instead of empty string
     # if there is no text.
-    text = web_element.text or web_element.get_attribute('innerText') or ""
-    if CONFIG['SearchMode']:
+    text = web_element.text or web_element.get_attribute("innerText") or ""
+    if CONFIG["SearchMode"]:
         element.draw_borders(web_element)
     return util.get_substring(text, **kwargs)
 
 
 @keyword(tags=("Item", "Interaction"))
 @decorators.timeout_decorator
-def click_item(text: str,
-               anchor: str = "1",
-               timeout: Union[int, float, str] = 0,
-               js: bool = False,
-               **kwargs) -> None:
+def click_item(
+    text: str, anchor: str = "1", timeout: Union[int, float, str] = 0, js: bool = False, **kwargs
+) -> None:
     r"""Click item (usually icon or picture) on webpage.
 
     Finds webelement by it's tooltip text (title or alt) or some another
     attribute.
     Available attributes: any
     Available element types without using tag attribute:
     *a, span, img, li, h1, h2, h3, h4, h5, h6, div, svg, p, button, input\*
@@ -970,18 +990,19 @@
     if _execute_click_and_verify_condition(web_element, timeout=timeout, js=js, **kwargs):
         return
 
 
 @keyword(tags=("Item", "Verification"))
 @decorators.timeout_decorator
 def verify_item(
-        text: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        **kwargs) -> None:
+    text: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    **kwargs,
+) -> None:
     r"""Verify Item (usually icon or picture) exist.
 
     Finds webelement by it's tooltip text (title or alt) or some another
     attribute.
     Available attributes: any
     Available element types without using tag attribute:
     *a, span, img, li, h1, h2, h3, h4, h5, h6, div, svg, p, button, input\*
@@ -1042,18 +1063,19 @@
     if web_element:
         return
 
 
 @keyword(tags=("Item", "Verification"))
 @decorators.timeout_decorator
 def verify_no_item(
-        text: str,
-        anchor: str = "1",
-        timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
-        **kwargs) -> None:
+    text: str,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,  # pylint: disable=unused-argument
+    **kwargs,
+) -> None:
     r"""Verify Item (usually icon or picture) is not exist.
 
     Finds webelement by it's tooltip text (title or alt) or some another
     attribute.
     Available attributes: any
     Available element types without using tag attribute:
     *a, span, img, li, h1, h2, h3, h4, h5, h6, div, svg, p, button, input\*
@@ -1089,19 +1111,19 @@
         |       partial_match: False. If only full match is accepted set
         |       partial_match to False.
 
     Related keywords
     ----------------
     \`ClickItem\`, \`VerifyItem\`
     """
-    kwargs['allow_non_existent'] = True
+    kwargs["allow_non_existent"] = True
     web_element = internal_text.get_item_using_anchor(text, anchor, **kwargs)
     if not web_element:
         return
-    raise QWebValueError('Element with attribute value {} still exists'.format(text))
+    raise QWebValueError("Element with attribute value {} still exists".format(text))
 
 
 @keyword(tags=("Item", "Verification"))
 @decorators.timeout_decorator
 def is_item(text: str, anchor: str = "1", timeout: Union[int, float, str] = 0.1, **kwargs) -> bool:
     r"""Check if Item (usually icon or picture) exists.
 
@@ -1206,18 +1228,17 @@
         return True
     except QWebValueError:
         return False
 
 
 @keyword(tags=("Text", "Interaction"))
 @decorators.timeout_decorator
-def scroll_text(text: str,
-                anchor: str = "1",
-                timeout: Union[int, float, str] = 0,
-                **kwargs) -> None:
+def scroll_text(
+    text: str, anchor: str = "1", timeout: Union[int, float, str] = 0, **kwargs
+) -> None:
     r"""Scroll page until text is on top.
 
     Finds text on page and scrolls until it is on top. This is used with visual testing
     tools to align page properly.
 
     Keyword tries to scroll to element until it succeeds or timeout has passed.
     If timeout is not specified, it uses default timeout that can be adjusted
@@ -1256,39 +1277,40 @@
 
         WriteText    Hello World!
 
     Related keywords
     ----------------
     \`PressKey\`, \`TypeText\`
     """
-    if CONFIG.get_value("Headless") or os.getenv('QWEB_HEADLESS', None):
-        raise QWebEnvironmentError('Running in headless environment. Pynput is unavailable.')
+    if CONFIG.get_value("Headless") or os.getenv("QWEB_HEADLESS", None):
+        raise QWebEnvironmentError("Running in headless environment. Pynput is unavailable.")
     keyboard = Controller()
     keyboard.type(text)
 
 
 @decorators.timeout_decorator
-def verify_texts(texts_to_verify: Union[list[str], str],
-                 timeout: Union[int, float, str] = 0) -> None:
+def verify_texts(
+    texts_to_verify: Union[list[str], str], timeout: Union[int, float, str] = 0
+) -> None:
     r"""*DEPRECATED!!* Use keyword `VerifyAll` instead."""
     logger.warn(r"""*DEPRECATED!!* Use keyword `VerifyAll` instead.""")
     if isinstance(texts_to_verify, list):
         for text in texts_to_verify:
             logger.info('Verifying text "{}".'.format(text), also_console=True)
             verify_text(text, timeout)
-    elif texts_to_verify.endswith('.txt'):
+    elif texts_to_verify.endswith(".txt"):
         file = download.get_path(texts_to_verify)
-        with open(file, 'rb') as txt_file:
+        with open(file, "rb") as txt_file:
             clean_data = [line.rstrip() for line in txt_file]
             for x in clean_data:
-                x_str = x.decode('utf-8')
+                x_str = x.decode("utf-8")
                 logger.info('Verifying text "{}".'.format(x_str), also_console=True)
                 verify_text(x_str, timeout)
     else:
-        texts = texts_to_verify.split(',')
+        texts = texts_to_verify.split(",")
         for text in texts:
             clean_text = text.strip()
             logger.info('Verifying text "{}".'.format(clean_text), also_console=True)
             verify_text(clean_text, timeout)
 
 
 @keyword(tags=("File", "Text", "Verification"))
@@ -1326,39 +1348,36 @@
     """
     if isinstance(texts_to_verify, list):
         for text in texts_to_verify:
             logger.info('Verifying text "{}".'.format(text), also_console=True)
             if is_text(text, timeout):
                 return text
 
-        raise QWebValueError('Could not find any of the texts: '
-                             f'{texts_to_verify}')
+        raise QWebValueError("Could not find any of the texts: " f"{texts_to_verify}")
 
-    if texts_to_verify.endswith('.txt'):
+    if texts_to_verify.endswith(".txt"):
         file = download.get_path(texts_to_verify)
-        with open(file, 'rb') as txt_file:
+        with open(file, "rb") as txt_file:
             clean_data = [line.rstrip() for line in txt_file]
             for x in clean_data:
-                x_str = x.decode('utf-8')
+                x_str = x.decode("utf-8")
                 if is_text(x_str, timeout):
                     return x_str
 
-            raise QWebValueError('Could not find any of the texts: '
-                                 f'{clean_data}')
+            raise QWebValueError("Could not find any of the texts: " f"{clean_data}")
 
     else:
-        texts = texts_to_verify.split(',')
+        texts = texts_to_verify.split(",")
         for text in texts:
             clean_text = text.strip()
             logger.info('Verifying text "{}".'.format(clean_text), also_console=True)
             if is_text(clean_text, timeout):
                 return clean_text
 
-        raise QWebValueError('Could not find any of the texts: '
-                             f'{texts}')
+        raise QWebValueError("Could not find any of the texts: " f"{texts}")
 
 
 @keyword(tags=("File", "Text", "Verification"))
 @decorators.timeout_decorator
 def verify_all(texts_to_verify: Union[list[str], str], timeout: Union[int, float, str] = 0) -> None:
     r"""Verify page contains given texts.
 
@@ -1367,54 +1386,56 @@
     Also accepts a .txt file or Robot FW list as a parameter. Each row in the text file will be
     verified, or each item in the Robot FW list.
 
     Examples
     --------
     .. code-block:: robotframework
 
-        VerifyTexts      Cat, Mouse, Dog, Lion, iddqd66402
-        VerifyTexts      list_of_cats.txt
-        VerifyTexts      C:/Users/pace/Desktop/textfile.txt
+        VerifyAll      Cat, Mouse, Dog, Lion, iddqd66402
+        VerifyAll      list_of_cats.txt
+        VerifyAll      C:/Users/pace/Desktop/textfile.txt
 
         ${cool_list}=    Create List    Cat    Mouse    Dog    Lion    iddqd66402
-        VerifyTexts      ${cool_list}
+        VerifyAll      ${cool_list}
 
     Related keywords
     ----------------
     \`VerifyAny\`, \`VerifyFile\`, \`VerifyFileText\`,
     \`VerifyPdfText\`, \`VerifyText\`
     """
     if isinstance(texts_to_verify, list):
         for text in texts_to_verify:
             logger.info('Verifying text "{}".'.format(text), also_console=True)
             verify_text(text, timeout)
-    elif texts_to_verify.endswith('.txt'):
+    elif texts_to_verify.endswith(".txt"):
         file = download.get_path(texts_to_verify)
-        with open(file, 'rb') as txt_file:
+        with open(file, "rb") as txt_file:
             clean_data = [line.rstrip() for line in txt_file]
             for x in clean_data:
-                x_str = x.decode('utf-8')
+                x_str = x.decode("utf-8")
                 logger.info('Verifying text "{}".'.format(x_str), also_console=True)
                 verify_text(x_str, timeout)
     else:
-        texts = texts_to_verify.split(',')
+        texts = texts_to_verify.split(",")
         for text in texts:
             clean_text = text.strip()
             logger.info('Verifying text "{}".'.format(clean_text), also_console=True)
             verify_text(clean_text, timeout)
 
 
 @keyword(tags=("Text", "Interaction"))
 @decorators.timeout_decorator
-def scroll_to(text_to_find: str,
-              locator: Optional[str] = None,
-              anchor: str = '1',
-              scroll_length: Optional[str] = None,
-              timeout: Union[int, float, str] = 120,
-              **kwargs) -> None:
+def scroll_to(
+    text_to_find: str,
+    locator: Optional[str] = None,
+    anchor: str = "1",
+    scroll_length: Optional[str] = None,
+    timeout: Union[int, float, str] = 120,
+    **kwargs,
+) -> None:
     r"""Scroll a dynamic web page or scrollbar.
 
     Parameters
     ----------
     text_to_find : str
         Text to find by scrolling a page or an element.
     locator : str
@@ -1460,18 +1481,19 @@
     \`HoverElement\`, \`HoverItem\`, \`HoverText\`,
     \`HoverTo\`, \`ScrollText\`
     """
     visible = is_text(text_to_find)
     if visible:
         scroll_text(text_to_find, anchor)
         return
-    slow_mode = util.par2bool(kwargs.get('slow_mode', False))
+    slow_mode = util.par2bool(kwargs.get("slow_mode", False))
     if locator:  # If we are trying to scroll a specific element
-        _scroll_first_scrollable_parent_element(locator, anchor, text_to_find, scroll_length,
-                                                slow_mode, timeout)
+        _scroll_first_scrollable_parent_element(
+            locator, anchor, text_to_find, scroll_length, slow_mode, timeout
+        )
     else:  # if we are just scrolling the web page
         _scroll_dynamic_web_page(text_to_find, scroll_length, slow_mode, timeout)
 
 
 @keyword(tags=("Text", "Interaction"))
 def copy_text(text: str) -> None:
     """Perform a copy.
@@ -1492,23 +1514,25 @@
         CopyText        text to clipboard
 
     """
     pyperclip.copy(text)
 
 
 @keyword(tags=("Text", "Interaction"))
-def click_while(text_to_disappear: str,
-                text_to_click: Optional[str] = None,
-                anchor: str = "1",
-                timeout: Union[int, float, str] = 0,
-                interval: Optional[str] = None,
-                parent: Optional[str] = None,
-                child: Optional[str] = None,
-                js: bool = False,
-                **kwargs) -> None:
+def click_while(
+    text_to_disappear: str,
+    text_to_click: Optional[str] = None,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    interval: Optional[str] = None,
+    parent: Optional[str] = None,
+    child: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     r"""Click text until a text or element disappears.
 
     This keyword is required on slow pages where it takes time for a button
     listener to start. This clicks button and waits until certain text or
     element disappears.
 
     If text_to_disappear is not entered, keyword will wait until clicked text disappears.
@@ -1553,45 +1577,48 @@
         tag=html tag: Use this if element to disappear is not default type of item element.
         force_click=True: Use this to bypass checks (istext/isnotext) before click.
 
     Related keywords
     ----------------
     \`ClickItemUntil\`, \`ClickItemWhile\`, \`ClickUntil\`
     """
-    el = util.par2bool(kwargs.get('element', False))
-    forced = util.par2bool(kwargs.get('force_click', False))
+    el = util.par2bool(kwargs.get("element", False))
+    forced = util.par2bool(kwargs.get("force_click", False))
     if not forced:
         if not text_to_click:
             text_to_click = text_to_disappear
         if el:
             try:
                 verify_item(text_to_disappear, timeout=timeout, **kwargs)
             except QWebElementNotFoundError as e:
-                raise QWebValueError('Element to disappear is not visible before click.') from e
+                raise QWebValueError("Element to disappear is not visible before click.") from e
         elif not is_text(text_to_disappear, timeout):
-            raise QWebValueError('Text to disappear is not visible before click.')
+            raise QWebValueError("Text to disappear is not visible before click.")
     try:
-        _retry_while(text_to_click, text_to_disappear, anchor, timeout, interval, parent, child, js,
-                     **kwargs)
+        _retry_while(
+            text_to_click, text_to_disappear, anchor, timeout, interval, parent, child, js, **kwargs
+        )
     except QWebElementNotFoundError as orig_err:
-        err = CONFIG.get_value('RetryError')
-        CONFIG.reset_value('RetryError')
+        err = CONFIG.get_value("RetryError")
+        CONFIG.reset_value("RetryError")
         raise err or orig_err
 
 
 @keyword(tags=("Text", "Interaction"))
-def click_until(text_to_appear: str,
-                text_to_click: Optional[str] = None,
-                anchor: str = "1",
-                timeout: Union[int, float, str] = 0,
-                interval: Optional[str] = None,
-                parent: Optional[str] = None,
-                child: Optional[str] = None,
-                js: bool = False,
-                **kwargs) -> None:
+def click_until(
+    text_to_appear: str,
+    text_to_click: Optional[str] = None,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    interval: Optional[str] = None,
+    parent: Optional[str] = None,
+    child: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     r"""Click text until a text appears.
 
     This keyword is required on slow pages where it takes time for a button
     listener to start. This clicks button and waits until text appears.
     Keyword is also handful in situations where we are waiting for some process
     to be ready and there is some button to press for getting results
 
@@ -1637,41 +1664,44 @@
         tag=html tag: Use this if element to disappear is not default type of item element.
         force_click=True: Use this to bypass checks (istext/isnotext) before click.
 
     Related keywords
     ----------------
     \`ClickItemUntil\`, \`ClickItemWhile\`, \`ClickWhile\`
     """
-    el = util.par2bool(kwargs.get('element', False))
-    forced = util.par2bool(kwargs.get('force_click', False))
+    el = util.par2bool(kwargs.get("element", False))
+    forced = util.par2bool(kwargs.get("force_click", False))
     if not forced:
         if el:
             try:
                 verify_no_item(text_to_appear, **kwargs)
             except QWebValueError as e:
-                raise QWebValueError('Element to appear is already visible.') from e
+                raise QWebValueError("Element to appear is already visible.") from e
         elif not is_no_text(text_to_appear):
-            raise QWebValueError('Text to appear is already visible.')
+            raise QWebValueError("Text to appear is already visible.")
     try:
-        _retry_until(text_to_click, text_to_appear, anchor, timeout, interval, parent, child, js,
-                     **kwargs)
+        _retry_until(
+            text_to_click, text_to_appear, anchor, timeout, interval, parent, child, js, **kwargs
+        )
     except QWebElementNotFoundError as orig_err:
-        err = CONFIG.get_value('RetryError')
-        CONFIG.reset_value('RetryError')
+        err = CONFIG.get_value("RetryError")
+        CONFIG.reset_value("RetryError")
         raise err or orig_err
 
 
 @keyword(tags=("Item", "Interaction"))
-def click_item_while(text_to_disappear: str,
-                     locator: Optional[str] = None,
-                     anchor: str = "1",
-                     timeout: Union[int, float, str] = 0,
-                     interval: Optional[str] = None,
-                     js: bool = False,
-                     **kwargs) -> None:
+def click_item_while(
+    text_to_disappear: str,
+    locator: Optional[str] = None,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    interval: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     r"""Click Item until a text or element disappears.
 
     This keyword is required on slow pages where it takes time for a button
     listener to start. This clicks button and waits until certain text or
     element disappears.
 
     If text_to_disappear is not entered, keyword will wait until clicked element disappears.
@@ -1713,43 +1743,45 @@
         tag=html tag: Use this if element to disappear is not default type of item element.
         force_click=True: Use this to bypass checks (istext/isnotext) before click.
 
     Related keywords
     ----------------
     \`ClickItemUntil\`, \`ClickUntil\`, \`ClickWhile\`
     """
-    kwargs['item'] = True
-    el = kwargs.get('element', False)
-    forced = util.par2bool(kwargs.get('force_click', False))
+    kwargs["item"] = True
+    el = kwargs.get("element", False)
+    forced = util.par2bool(kwargs.get("force_click", False))
     if not forced:
         if not locator:
             locator = text_to_disappear
         if el:
             try:
                 verify_item(text_to_disappear, timeout=timeout, **kwargs)
             except QWebElementNotFoundError as e:
-                raise QWebValueError('Element to disappear is not visible before click.') from e
+                raise QWebValueError("Element to disappear is not visible before click.") from e
         elif not is_text(text_to_disappear, timeout):
-            raise QWebValueError('Text to disappear is not visible before click.')
+            raise QWebValueError("Text to disappear is not visible before click.")
     try:
         _retry_while(locator, text_to_disappear, anchor, timeout, interval, js=js, **kwargs)
     except QWebElementNotFoundError as orig_err:
-        err = CONFIG.get_value('RetryError')
-        CONFIG.reset_value('RetryError')
+        err = CONFIG.get_value("RetryError")
+        CONFIG.reset_value("RetryError")
         raise err or orig_err
 
 
 @keyword(tags=("Item", "Interaction"))
-def click_item_until(text_to_appear: str,
-                     locator: Optional[str] = None,
-                     anchor: str = "1",
-                     timeout: Union[int, float, str] = 0,
-                     interval: Optional[str] = None,
-                     js: bool = False,
-                     **kwargs) -> None:
+def click_item_until(
+    text_to_appear: str,
+    locator: Optional[str] = None,
+    anchor: str = "1",
+    timeout: Union[int, float, str] = 0,
+    interval: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     r"""Click text until a text appears.
 
     This keyword is required on slow pages where it takes time for a button
     listener to start. This clicks button and waits until text appears.
     Keyword is also handful in situations where we are waiting for some process
     to be ready and there is some button to press for getting results
 
@@ -1789,92 +1821,94 @@
         tag=html tag: Use this if element to disappear is not default type of item element.
         force_click=True: Use this to bypass checks (istext/isnotext) before click.
 
     Related keywords
     ----------------
     \`ClickItemWhile\`, \`ClickUntil\`, \`ClickWhile\`
     """
-    kwargs['item'] = True
-    el = kwargs.get('element', False)
-    forced = util.par2bool(kwargs.get('force_click', False))
+    kwargs["item"] = True
+    el = kwargs.get("element", False)
+    forced = util.par2bool(kwargs.get("force_click", False))
     if not forced:
         if el:
             try:
                 verify_no_item(text_to_appear, **kwargs)
             except QWebValueError as e:
-                raise QWebValueError('Element to appear is already visible.') from e
+                raise QWebValueError("Element to appear is already visible.") from e
         elif not is_no_text(text_to_appear):
-            raise QWebValueError('Text to appear is already visible.')
+            raise QWebValueError("Text to appear is already visible.")
     try:
         _retry_until(locator, text_to_appear, anchor, timeout, interval, js=js, **kwargs)
     except QWebElementNotFoundError as orig_err:
-        err = CONFIG.get_value('RetryError')
-        CONFIG.reset_value('RetryError')
+        err = CONFIG.get_value("RetryError")
+        CONFIG.reset_value("RetryError")
         raise err or orig_err
 
 
 @decorators.timeout_decorator
 def _retry_while(
-        text: str,
-        text_to_disappear: str,
-        anchor: str,
-        timeout: Union[int, float, str],  # pylint: disable=unused-argument
-        interval: Optional[str],
-        parent: Optional[str] = None,
-        child: Optional[str] = None,
-        js: bool = False,
-        **kwargs) -> None:
+    text: str,
+    text_to_disappear: str,
+    anchor: str,
+    timeout: Union[int, float, str],  # pylint: disable=unused-argument
+    interval: Optional[str],
+    parent: Optional[str] = None,
+    child: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     if not interval:
-        interval = CONFIG['RetryInterval']
-    item = kwargs.get('item', False)
-    el = kwargs.get('element', False)
+        interval = CONFIG["RetryInterval"]
+    item = kwargs.get("item", False)
+    el = kwargs.get("element", False)
     try:
         if item:
             click_item(text, anchor, interval, js, **kwargs)
         else:
             click_text(text, anchor, interval, parent, child, js, **kwargs)
     except (QWebElementNotFoundError, QWebDriverError, QWebValueError) as e:
-        CONFIG.set_value('RetryError', e)
-        logger.info('Got {} from click part. Action probably triggered'.format(e))
+        CONFIG.set_value("RetryError", e)
+        logger.info("Got {} from click part. Action probably triggered".format(e))
     try:
         if el:
             verify_no_item(text_to_disappear, timeout=interval, **kwargs)
         else:
             verify_no_text(text_to_disappear, timeout=interval)
     except QWebValueError as e:
-        logger.info('Got {} from verify part.'.format(e))
-        CONFIG.set_value('RetryError', e)
+        logger.info("Got {} from verify part.".format(e))
+        CONFIG.set_value("RetryError", e)
         raise e
 
 
 @decorators.timeout_decorator
 def _retry_until(
-        text: str,
-        text_to_appear: str,
-        anchor: str,
-        timeout: Union[int, float, str],  # pylint: disable=unused-argument
-        interval: Optional[str],
-        parent: Optional[str] = None,
-        child: Optional[str] = None,
-        js: bool = False,
-        **kwargs) -> None:
+    text: str,
+    text_to_appear: str,
+    anchor: str,
+    timeout: Union[int, float, str],  # pylint: disable=unused-argument
+    interval: Optional[str],
+    parent: Optional[str] = None,
+    child: Optional[str] = None,
+    js: bool = False,
+    **kwargs,
+) -> None:
     if not interval:
-        interval = CONFIG['RetryInterval']
-    item = kwargs.get('item', False)
-    el = kwargs.get('element', False)
+        interval = CONFIG["RetryInterval"]
+    item = kwargs.get("item", False)
+    el = kwargs.get("element", False)
     try:
         if item:
             click_item(text, anchor, interval, js, **kwargs)
         else:
             click_text(text, anchor, interval, parent, child, js, **kwargs)
     except (QWebElementNotFoundError, QWebDriverError, QWebValueError) as e:
-        CONFIG.set_value('RetryError', e)
-        logger.info('Got {} from click part. Action probably triggered'.format(e))
+        CONFIG.set_value("RetryError", e)
+        logger.info("Got {} from click part. Action probably triggered".format(e))
     try:
         if el:
             verify_item(text_to_appear, timeout=interval, **kwargs)
         else:
             verify_text(text_to_appear, timeout=interval)
     except QWebElementNotFoundError as e:
-        logger.info('Got {} from verify part.'.format(e))
-        CONFIG.set_value('RetryError', e)
+        logger.info("Got {} from verify part.".format(e))
+        CONFIG.set_value("RetryError", e)
         raise e
```

### Comparing `QWeb-3.2.1/QWeb/keywords/window.py` & `QWeb-3.3.0/QWeb/keywords/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,15 @@
 
     Related keywords
     ----------------
     \`CloseAllBrowsers\`, \`CloseBrowser\`, \`OpenBrowser\`, \`OpenWindow\`, \`SwitchWindow\`
     """
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     driver.get(url)
 
 
 @keyword(tags=("Browser", "Interaction", "Window"))
 def open_window() -> None:
     r"""Open new tab.
 
@@ -71,18 +70,18 @@
         OpenWindow
 
     Related keywords
     ----------------
     \`CloseAllBrowsers\`, \`CloseBrowser\`, \`CloseOthers\`, \`GoTo\`,
     \`OpenBrowser\`, \`SwitchWindow\`
     """
-    script = 'window.open()'
+    script = "window.open()"
     javascript.execute_javascript(script)
     window_handles = window.get_window_handles()
-    logger.debug(f'available handles: {len(window_handles)}')
+    logger.debug(f"available handles: {len(window_handles)}")
 
     current_window_handle = window.get_current_window_handle()
 
     # make ordered list for safari
     if util.is_safari():
         # refresh all windows, not just the ones we have tracked as open
         window.append_new_windows_safari()
@@ -92,15 +91,15 @@
     new_window_index = index + 1
 
     window.switch_to_window(window_handles[new_window_index])
 
     try:
         xhr.setup_xhr_monitor()
     except QWebDriverError:
-        logger.debug('XHR monitor threw exception. Bypassing jQuery injection')
+        logger.debug("XHR monitor threw exception. Bypassing jQuery injection")
 
 
 @keyword(tags=("Browser", "Interaction", "Window"))
 def close_others() -> None:
     r"""Close all windows except the first window.
 
     If you have a test that may open new windows, this keyword closes them
@@ -128,22 +127,21 @@
     driver = browser.get_current_browser()
     while len(window_handles) > 1:
         try:
             window_handle = window_handles.pop()
             window.switch_to_window(window_handle)
             driver.close()
         except NoSuchWindowException:
-            logger.info('Failed to close window')
-    first_window_handle = window_handles[0] if util.is_safari() \
-        else window_handles.pop()
+            logger.info("Failed to close window")
+    first_window_handle = window_handles[0] if util.is_safari() else window_handles.pop()
     window.switch_to_window(first_window_handle)
 
     number_of_handles = len(window.get_window_handles())
     if number_of_handles != 1:
-        raise ValueError(f'Expected 1 window open, found {number_of_handles}')
+        raise ValueError(f"Expected 1 window open, found {number_of_handles}")
 
 
 @keyword(tags=("Browser", "Interaction", "Window"))
 def close_window() -> None:
     r"""Close current tab and switch context to another window handle.
 
     If you need to change to specific tab, use switch window keyword.
@@ -221,30 +219,35 @@
     # safari specific, refresh windows not open by keywords
     if util.is_safari():
         window.append_new_windows_safari()
     window_handles = window.get_window_handles()
     logger.info("Current browser contains {} tabs".format(len(window_handles)))
     if index.isdigit():
         if int(index) == 0:
-            raise QWebValueError('SwitchWindow index starts at 1.')
+            raise QWebValueError("SwitchWindow index starts at 1.")
         i = int(index) - 1
         if i < len(window_handles):
             correct_window_handle = window_handles[i]
             window.switch_to_window(correct_window_handle)
             return
-        logger.debug('Tried to select tab with index {} but there'
-                     ' are only {} tabs open'.format(index, len(window_handles)))
+        logger.debug(
+            "Tried to select tab with index {} but there" " are only {} tabs open".format(
+                index, len(window_handles)
+            )
+        )
     elif index == "NEW":
         window.switch_to_window(window_handles[-1])
         return
     else:
         raise QWebValueError('Given argument "{}" is not a digit or NEW'.format(index))
     raise QWebDriverError(
-        'Tried to select tab with index {} but there are only {} tabs open'.format(
-            index, len(window_handles)))
+        "Tried to select tab with index {} but there are only {} tabs open".format(
+            index, len(window_handles)
+        )
+    )
 
 
 def set_window_size(width: int, height: int) -> None:
     """*DEPRECATED!!* Use keyword `SetConfig` instead.
 
     Set current window size.
 
@@ -288,18 +291,17 @@
 
     Related keywords
     ----------------
     \`Back\`,\`RefreshPage\`, \`OpenWindow\`, \`SwitchWindow\`
     """
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
 
-    if CONFIG.get_value('Headless') is True:
+    if CONFIG.get_value("Headless") is True:
         logger.debug("Maximizing browser in headless mode")
         screen_width_js = driver.execute_script("return screen.width")
         screen_height_js = driver.execute_script("return screen.height")
 
         driver.set_window_size(screen_width_js, screen_height_js)
 
     else:
@@ -360,16 +362,15 @@
 
     Related keywords
     ----------------
     \`GetTitle\`, \`GetUrl\`, \`VerifyTitle\`
     """
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     current = driver.current_url
 
     if current.lower() != url.lower():
         raise QWebValueError(f"Current url '{current}'' does not match expected url '{url}'")
 
 
 @keyword(tags=("Browser", "Getters"))
@@ -390,16 +391,15 @@
 
     Related keywords
     ----------------
     \`GetUrl\`, \`VerifyTitle\`, \`VerifyUrl\`
     """
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     return driver.title
 
 
 @keyword(tags=("Browser", "Verification"))
 @decorators.timeout_decorator
 def verify_title(title: str, timeout: Union[int, float, str] = 0) -> None:  # pylint: disable=unused-argument
     r"""Verifies that current page's title matches expected title.
@@ -427,24 +427,23 @@
 
     Related keywords
     ----------------
     \`GetTitle\`, \`GetUrl\`, \`VerifyUrl\`
     """
     driver = browser.get_current_browser()
     if driver is None:
-        raise QWebDriverError("No browser open. Use OpenBrowser keyword"
-                              " to open browser first")
+        raise QWebDriverError("No browser open. Use OpenBrowser keyword to open browser first")
     actual = driver.title
 
     if actual != title:
         raise QWebValueError(f"Page title '{actual}'' does not match expected '{title}'")
 
 
 @keyword(tags=("Browser", "Interaction"))
-def swipe_down(times: str = '1', start: Optional[str] = None) -> None:
+def swipe_down(times: str = "1", start: Optional[str] = None) -> None:
     r"""Swipes down on the screen.
 
     Examples
     --------
     .. code-block:: robotframework
 
         SwipeDown   # Swipes down once
@@ -464,19 +463,19 @@
     ValueError
         If the swipe amount is not an integer.
 
     Related keywords
     ----------------
     \`SwipeLeft\`, \`SwipeRight\`, \`SwipeUp\`
     """
-    window.swipe('down', times, start)
+    window.swipe("down", times, start)
 
 
 @keyword(tags=("Browser", "Interaction"))
-def swipe_up(times: str = '1', start: Optional[str] = None) -> None:
+def swipe_up(times: str = "1", start: Optional[str] = None) -> None:
     r"""Swipes up on the screen.
 
     Examples
     --------
     .. code-block:: robotframework
 
         SwipeUp   # Swipes up once
@@ -496,19 +495,19 @@
     ValueError
         If the swipe amount is not an integer.
 
     Related keywords
     ----------------
     \`SwipeDown\`, \`SwipeLeft\`, \`SwipeRight\`
     """
-    window.swipe('up', times, start)
+    window.swipe("up", times, start)
 
 
 @keyword(tags=("Browser", "Interaction"))
-def swipe_left(times: str = '1', start: Optional[str] = None) -> None:
+def swipe_left(times: str = "1", start: Optional[str] = None) -> None:
     r"""Swipes left on the screen.
 
     Examples
     --------
     .. code-block:: robotframework
 
         SwipeLeft   # Swipes left once
@@ -528,19 +527,19 @@
     ValueError
         If the swipe amount is not an integer.
 
     Related keywords
     ----------------
     \`SwipeDown\`, \`SwipeRight\`, \`SwipeUp\`
     """
-    window.swipe('left', times, start)
+    window.swipe("left", times, start)
 
 
 @keyword(tags=("Browser", "Interaction"))
-def swipe_right(times: str = '1', start: Optional[str] = None) -> None:
+def swipe_right(times: str = "1", start: Optional[str] = None) -> None:
     r"""Swipes right on the screen.
 
     Examples
     --------
     .. code-block:: robotframework
 
         SwipeRight   # Swipes right once
@@ -560,8 +559,8 @@
     ValueError
         If the swipe amount is not an integer.
 
     Related keywords
     ----------------
     \`SwipeDown\`, \`SwipeLeft\`, \`SwipeUp\`
     """
-    window.swipe('right', times, start)
+    window.swipe("right", times, start)
```

### Comparing `QWeb-3.2.1/QWeb.egg-info/PKG-INFO` & `QWeb-3.3.0/QWeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QWeb
-Version: 3.2.1
+Version: 3.3.0
 Summary: Keyword driven automation for the web
 Home-page: https://github.com/qentinelqi/qweb/
 Author: Qentinel Group
 Author-email: libraries@qentinel.com
 License: Apache License 2.0
 Keywords: test automation robot framework
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `QWeb-3.2.1/QWeb.egg-info/SOURCES.txt` & `QWeb-3.3.0/QWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QWeb-3.2.1/README.md` & `QWeb-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `QWeb-3.2.1/setup.cfg` & `QWeb-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `QWeb-3.2.1/setup.py` & `QWeb-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `QWeb-3.2.1/versioneer.py` & `QWeb-3.3.0/versioneer.py`

 * *Files identical despite different names*

