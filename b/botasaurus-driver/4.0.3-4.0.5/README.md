# Comparing `tmp/botasaurus_driver-4.0.3.tar.gz` & `tmp/botasaurus_driver-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_driver-4.0.3.tar", last modified: Wed Apr 24 07:22:59 2024, max compression
+gzip compressed data, was "botasaurus_driver-4.0.5.tar", last modified: Tue May 14 15:46:41 2024, max compression
```

## Comparing `botasaurus_driver-4.0.3.tar` & `botasaurus_driver-4.0.5.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 07:22:59.903247 botasaurus_driver-4.0.3/
--rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus_driver-4.0.3/LICENSE
--rw-rw-rw-   0        0        0      139 2024-04-24 09:55:31.000000 botasaurus_driver-4.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2855 2024-04-24 07:22:59.902157 botasaurus_driver-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-04-24 06:56:42.000000 botasaurus_driver-4.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 07:22:59.777073 botasaurus_driver-4.0.3/botasaurus_driver/
--rw-rw-rw-   0        0        0      743 2024-04-24 09:50:01.000000 botasaurus_driver-4.0.3/botasaurus_driver/__init__.py
--rw-rw-rw-   0        0        0     3673 2024-04-22 10:12:09.000000 botasaurus_driver-4.0.3/botasaurus_driver/base_data.py
--rw-rw-rw-   0        0        0     1305 2024-04-22 08:12:58.000000 botasaurus_driver-4.0.3/botasaurus_driver/beep_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:22:59.882635 botasaurus_driver-4.0.3/botasaurus_driver/cdp/
--rw-rw-rw-   0        0        0      172 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/README.md
--rw-rw-rw-   0        0        0     1011 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/__init__.py
--rw-rw-rw-   0        0        0    25019 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/accessibility.py
--rw-rw-rw-   0        0        0    11919 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/animation.py
--rw-rw-rw-   0        0        0    65075 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/audits.py
--rw-rw-rw-   0        0        0     8168 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/autofill.py
--rw-rw-rw-   0        0        0     6359 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/background_service.py
--rw-rw-rw-   0        0        0    22888 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/browser.py
--rw-rw-rw-   0        0        0     9549 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/cache_storage.py
--rw-rw-rw-   0        0        0     4565 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/cast.py
--rw-rw-rw-   0        0        0     3004 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/console.py
--rw-rw-rw-   0        0        0    80456 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/css.py
--rw-rw-rw-   0        0        0     4358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/database.py
--rw-rw-rw-   0        0        0    54782 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/debugger.py
--rw-rw-rw-   0        0        0     3497 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/device_access.py
--rw-rw-rw-   0        0        0     1187 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/device_orientation.py
--rw-rw-rw-   0        0        0    66246 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom.py
--rw-rw-rw-   0        0        0    10211 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom_debugger.py
--rw-rw-rw-   0        0        0    43435 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom_snapshot.py
--rw-rw-rw-   0        0        0     6124 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom_storage.py
--rw-rw-rw-   0        0        0    34831 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/emulation.py
--rw-rw-rw-   0        0        0     1501 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/event_breakpoints.py
--rw-rw-rw-   0        0        0     7347 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/fed_cm.py
--rw-rw-rw-   0        0        0    21611 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/fetch.py
--rw-rw-rw-   0        0        0     5219 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/headless_experimental.py
--rw-rw-rw-   0        0        0    14457 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/heap_profiler.py
--rw-rw-rw-   0        0        0    18362 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/indexed_db.py
--rw-rw-rw-   0        0        0    29314 2024-04-15 12:04:59.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/input_.py
--rw-rw-rw-   0        0        0     1743 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/inspector.py
--rw-rw-rw-   0        0        0     3120 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/io.py
--rw-rw-rw-   0        0        0    16878 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/layer_tree.py
--rw-rw-rw-   0        0        0     6092 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/log.py
--rw-rw-rw-   0        0        0     8215 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/media.py
--rw-rw-rw-   0        0        0     7279 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/memory.py
--rw-rw-rw-   0        0        0   147161 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/network.py
--rw-rw-rw-   0        0        0    60483 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/overlay.py
--rw-rw-rw-   0        0        0   117573 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/page.py
--rw-rw-rw-   0        0        0     3203 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/performance.py
--rw-rw-rw-   0        0        0     7587 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/performance_timeline.py
--rw-rw-rw-   0        0        0    22524 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/preload.py
--rw-rw-rw-   0        0        0    14302 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/profiler.py
--rw-rw-rw-   0        0        0        0 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/py.typed
--rw-rw-rw-   0        0        0    67631 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/runtime.py
--rw-rw-rw-   0        0        0     1196 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/schema.py
--rw-rw-rw-   0        0        0    18824 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/security.py
--rw-rw-rw-   0        0        0    12358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/service_worker.py
--rw-rw-rw-   0        0        0    61377 2024-04-17 07:20:04.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/storage.py
--rw-rw-rw-   0        0        0    12914 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/system_info.py
--rw-rw-rw-   0        0        0    25505 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/target.py
--rw-rw-rw-   0        0        0     1533 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/tethering.py
--rw-rw-rw-   0        0        0    14682 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/tracing.py
--rw-rw-rw-   0        0        0      470 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/util.py
--rw-rw-rw-   0        0        0    18513 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/web_audio.py
--rw-rw-rw-   0        0        0    18390 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.3/botasaurus_driver/cdp/web_authn.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:22:59.899142 botasaurus_driver-4.0.3/botasaurus_driver/core/
--rw-rw-rw-   0        0        0     3344 2024-04-19 06:25:12.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/_contradict.py
--rw-rw-rw-   0        0        0    17802 2024-04-24 07:21:50.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/browser.py
--rw-rw-rw-   0        0        0    10464 2024-04-23 11:13:07.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/config.py
--rw-rw-rw-   0        0        0    17386 2024-04-20 11:05:41.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/connection.py
--rw-rw-rw-   0        0        0     1445 2024-04-22 12:23:38.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/custom_storage_cdp.py
--rw-rw-rw-   0        0        0    33534 2024-04-22 07:27:39.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/element.py
--rw-rw-rw-   0        0        0      687 2024-04-22 12:49:02.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/env.py
--rw-rw-rw-   0        0        0     3185 2024-04-22 11:09:04.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/profiles.py
--rw-rw-rw-   0        0        0    40748 2024-04-22 10:32:44.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/tab.py
--rw-rw-rw-   0        0        0     4748 2024-04-22 11:57:20.000000 botasaurus_driver-4.0.3/botasaurus_driver/core/util.py
--rw-rw-rw-   0        0        0    35872 2024-04-24 07:16:14.000000 botasaurus_driver-4.0.3/botasaurus_driver/driver.py
--rw-rw-rw-   0        0        0     5041 2024-04-22 10:57:19.000000 botasaurus_driver-4.0.3/botasaurus_driver/driver_utils.py
--rw-rw-rw-   0        0        0     4841 2024-04-24 07:47:17.000000 botasaurus_driver-4.0.3/botasaurus_driver/exceptions.py
--rw-rw-rw-   0        0        0     3764 2024-04-22 13:03:42.000000 botasaurus_driver-4.0.3/botasaurus_driver/lang.py
--rw-rw-rw-   0        0        0     1710 2024-04-16 12:10:34.000000 botasaurus_driver-4.0.3/botasaurus_driver/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.000000 botasaurus_driver-4.0.3/botasaurus_driver/opponent.py
--rw-rw-rw-   0        0        0     3439 2024-04-20 07:11:23.000000 botasaurus_driver-4.0.3/botasaurus_driver/solve_cloudflare_captcha.py
--rw-rw-rw-   0        0        0     1160 2024-04-22 13:05:31.000000 botasaurus_driver-4.0.3/botasaurus_driver/tiny_profile.py
--rw-rw-rw-   0        0        0     7569 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.3/botasaurus_driver/user_agent.py
--rw-rw-rw-   0        0        0     1203 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.3/botasaurus_driver/window_size.py
-drwxrwxrwx   0        0        0        0 2024-04-24 07:22:59.900160 botasaurus_driver-4.0.3/botasaurus_driver.egg-info/
--rw-rw-rw-   0        0        0     2855 2024-04-24 07:22:59.000000 botasaurus_driver-4.0.3/botasaurus_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2923 2024-04-24 07:22:59.000000 botasaurus_driver-4.0.3/botasaurus_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 07:22:59.000000 botasaurus_driver-4.0.3/botasaurus_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2024-04-24 07:22:59.000000 botasaurus_driver-4.0.3/botasaurus_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-24 07:22:59.000000 botasaurus_driver-4.0.3/botasaurus_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1914 2024-04-24 07:22:58.000000 botasaurus_driver-4.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-04-24 07:22:59.905908 botasaurus_driver-4.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_driver-4.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:46:41.452640 botasaurus_driver-4.0.5/
+-rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus_driver-4.0.5/LICENSE
+-rw-rw-rw-   0        0        0      139 2024-04-24 09:55:31.000000 botasaurus_driver-4.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6818 2024-05-14 15:46:41.451438 botasaurus_driver-4.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3984 2024-05-14 14:16:36.000000 botasaurus_driver-4.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:46:41.209484 botasaurus_driver-4.0.5/botasaurus_driver/
+-rw-rw-rw-   0        0        0      638 2024-05-06 12:43:02.000000 botasaurus_driver-4.0.5/botasaurus_driver/__init__.py
+-rw-rw-rw-   0        0        0     3673 2024-04-22 10:12:09.000000 botasaurus_driver-4.0.5/botasaurus_driver/base_data.py
+-rw-rw-rw-   0        0        0     1305 2024-04-22 08:12:58.000000 botasaurus_driver-4.0.5/botasaurus_driver/beep_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:46:41.414314 botasaurus_driver-4.0.5/botasaurus_driver/cdp/
+-rw-rw-rw-   0        0        0      172 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/README.md
+-rw-rw-rw-   0        0        0     1011 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/__init__.py
+-rw-rw-rw-   0        0        0    25019 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/accessibility.py
+-rw-rw-rw-   0        0        0    11919 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/animation.py
+-rw-rw-rw-   0        0        0    65075 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/audits.py
+-rw-rw-rw-   0        0        0     8168 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/autofill.py
+-rw-rw-rw-   0        0        0     6359 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/background_service.py
+-rw-rw-rw-   0        0        0    22888 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/browser.py
+-rw-rw-rw-   0        0        0     9549 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/cache_storage.py
+-rw-rw-rw-   0        0        0     4565 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/cast.py
+-rw-rw-rw-   0        0        0     3004 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/console.py
+-rw-rw-rw-   0        0        0    80456 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/css.py
+-rw-rw-rw-   0        0        0     4358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/database.py
+-rw-rw-rw-   0        0        0    54782 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/debugger.py
+-rw-rw-rw-   0        0        0     3497 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/device_access.py
+-rw-rw-rw-   0        0        0     1187 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/device_orientation.py
+-rw-rw-rw-   0        0        0    66246 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom.py
+-rw-rw-rw-   0        0        0    10211 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom_debugger.py
+-rw-rw-rw-   0        0        0    43435 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom_snapshot.py
+-rw-rw-rw-   0        0        0     6124 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom_storage.py
+-rw-rw-rw-   0        0        0    34831 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/emulation.py
+-rw-rw-rw-   0        0        0     1501 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/event_breakpoints.py
+-rw-rw-rw-   0        0        0     7347 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/fed_cm.py
+-rw-rw-rw-   0        0        0    21611 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/fetch.py
+-rw-rw-rw-   0        0        0     5219 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/headless_experimental.py
+-rw-rw-rw-   0        0        0    14457 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/heap_profiler.py
+-rw-rw-rw-   0        0        0    18362 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/indexed_db.py
+-rw-rw-rw-   0        0        0    29314 2024-04-15 12:04:59.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/input_.py
+-rw-rw-rw-   0        0        0     1743 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/inspector.py
+-rw-rw-rw-   0        0        0     3120 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/io.py
+-rw-rw-rw-   0        0        0    16878 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/layer_tree.py
+-rw-rw-rw-   0        0        0     6092 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/log.py
+-rw-rw-rw-   0        0        0     8215 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/media.py
+-rw-rw-rw-   0        0        0     7279 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/memory.py
+-rw-rw-rw-   0        0        0   147161 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/network.py
+-rw-rw-rw-   0        0        0    60483 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/overlay.py
+-rw-rw-rw-   0        0        0   117573 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/page.py
+-rw-rw-rw-   0        0        0     3203 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/performance.py
+-rw-rw-rw-   0        0        0     7587 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/performance_timeline.py
+-rw-rw-rw-   0        0        0    22524 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/preload.py
+-rw-rw-rw-   0        0        0    14302 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/profiler.py
+-rw-rw-rw-   0        0        0        0 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/py.typed
+-rw-rw-rw-   0        0        0    67631 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/runtime.py
+-rw-rw-rw-   0        0        0     1196 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/schema.py
+-rw-rw-rw-   0        0        0    18824 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/security.py
+-rw-rw-rw-   0        0        0    12358 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/service_worker.py
+-rw-rw-rw-   0        0        0    61377 2024-04-17 07:20:04.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/storage.py
+-rw-rw-rw-   0        0        0    12914 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/system_info.py
+-rw-rw-rw-   0        0        0    25505 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/target.py
+-rw-rw-rw-   0        0        0     1533 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/tethering.py
+-rw-rw-rw-   0        0        0    14682 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/tracing.py
+-rw-rw-rw-   0        0        0      470 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/util.py
+-rw-rw-rw-   0        0        0    18513 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/web_audio.py
+-rw-rw-rw-   0        0        0    18390 2024-04-14 11:02:29.000000 botasaurus_driver-4.0.5/botasaurus_driver/cdp/web_authn.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:46:41.443239 botasaurus_driver-4.0.5/botasaurus_driver/core/
+-rw-rw-rw-   0        0        0     3344 2024-04-19 06:25:12.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/_contradict.py
+-rw-rw-rw-   0        0        0    17760 2024-05-10 15:05:54.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/browser.py
+-rw-rw-rw-   0        0        0    11687 2024-05-04 13:04:59.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/config.py
+-rw-rw-rw-   0        0        0    17622 2024-05-14 12:40:04.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/connection.py
+-rw-rw-rw-   0        0        0     1445 2024-04-22 12:23:38.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/custom_storage_cdp.py
+-rw-rw-rw-   0        0        0    33534 2024-04-22 07:27:39.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/element.py
+-rw-rw-rw-   0        0        0      687 2024-04-22 12:49:02.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/env.py
+-rw-rw-rw-   0        0        0     3185 2024-04-22 11:09:04.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/profiles.py
+-rw-rw-rw-   0        0        0    40672 2024-05-10 14:59:53.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/tab.py
+-rw-rw-rw-   0        0        0     4748 2024-04-22 11:57:20.000000 botasaurus_driver-4.0.5/botasaurus_driver/core/util.py
+-rw-rw-rw-   0        0        0    37106 2024-05-14 05:29:03.000000 botasaurus_driver-4.0.5/botasaurus_driver/driver.py
+-rw-rw-rw-   0        0        0     5041 2024-04-22 10:57:19.000000 botasaurus_driver-4.0.5/botasaurus_driver/driver_utils.py
+-rw-rw-rw-   0        0        0     4957 2024-05-02 11:54:25.000000 botasaurus_driver-4.0.5/botasaurus_driver/exceptions.py
+-rw-rw-rw-   0        0        0     3764 2024-04-22 13:03:42.000000 botasaurus_driver-4.0.5/botasaurus_driver/lang.py
+-rw-rw-rw-   0        0        0     1710 2024-04-16 12:10:34.000000 botasaurus_driver-4.0.5/botasaurus_driver/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.000000 botasaurus_driver-4.0.5/botasaurus_driver/opponent.py
+-rw-rw-rw-   0        0        0     4153 2024-05-02 11:56:26.000000 botasaurus_driver-4.0.5/botasaurus_driver/profile.py
+-rw-rw-rw-   0        0        0     4617 2024-05-12 10:41:42.000000 botasaurus_driver-4.0.5/botasaurus_driver/solve_cloudflare_captcha.py
+-rw-rw-rw-   0        0        0     1160 2024-04-22 13:05:31.000000 botasaurus_driver-4.0.5/botasaurus_driver/tiny_profile.py
+-rw-rw-rw-   0        0        0     7569 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.5/botasaurus_driver/user_agent.py
+-rw-rw-rw-   0        0        0     1203 2024-04-22 13:04:27.000000 botasaurus_driver-4.0.5/botasaurus_driver/window_size.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:46:41.446698 botasaurus_driver-4.0.5/botasaurus_driver.egg-info/
+-rw-rw-rw-   0        0        0     6818 2024-05-14 15:46:40.000000 botasaurus_driver-4.0.5/botasaurus_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2952 2024-05-14 15:46:40.000000 botasaurus_driver-4.0.5/botasaurus_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:46:40.000000 botasaurus_driver-4.0.5/botasaurus_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2024-05-14 15:46:40.000000 botasaurus_driver-4.0.5/botasaurus_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-14 15:46:40.000000 botasaurus_driver-4.0.5/botasaurus_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1914 2024-05-14 15:46:38.000000 botasaurus_driver-4.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-14 15:46:41.465424 botasaurus_driver-4.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_driver-4.0.5/setup.py
```

### Comparing `botasaurus_driver-4.0.3/LICENSE` & `botasaurus_driver-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/base_data.py` & `botasaurus_driver-4.0.5/botasaurus_driver/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/beep_utils.py` & `botasaurus_driver-4.0.5/botasaurus_driver/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/__init__.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/accessibility.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/accessibility.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/animation.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/animation.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/audits.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/audits.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/autofill.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/autofill.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/background_service.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/background_service.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/browser.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/browser.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/cache_storage.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/cache_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/cast.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/cast.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/console.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/console.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/css.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/css.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/database.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/database.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/debugger.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/debugger.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/device_access.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/device_access.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/device_orientation.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/device_orientation.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom_debugger.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom_debugger.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom_snapshot.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/dom_storage.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/dom_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/emulation.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/emulation.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/event_breakpoints.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/event_breakpoints.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/fed_cm.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/fed_cm.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/fetch.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/fetch.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/headless_experimental.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/headless_experimental.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/heap_profiler.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/heap_profiler.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/indexed_db.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/indexed_db.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/input_.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/input_.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/inspector.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/inspector.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/io.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/io.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/layer_tree.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/layer_tree.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/log.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/log.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/media.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/media.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/memory.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/memory.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/network.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/network.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/overlay.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/overlay.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/page.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/page.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/performance.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/performance.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/performance_timeline.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/performance_timeline.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/preload.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/preload.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/profiler.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/profiler.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/runtime.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/runtime.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/schema.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/schema.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/security.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/security.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/service_worker.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/service_worker.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/storage.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/system_info.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/system_info.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/target.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/target.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/tethering.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/tethering.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/tracing.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/tracing.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/web_audio.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/web_audio.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/cdp/web_authn.py` & `botasaurus_driver-4.0.5/botasaurus_driver/cdp/web_authn.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/_contradict.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/_contradict.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/browser.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 from . import util
 from . import tab
 from ._contradict import ContraDict
 from .config import PathLike, Config, free_port, is_posix
 from .connection import Connection
 from .custom_storage_cdp import  get_cookies, set_cookies
 
+import os
+import signal
+
+def kill_process(pid):
+    os.kill(pid, signal.SIGTERM)
+
 def get_folder_name_from_path(absolute_path):
     """
     Returns the folder name from an absolute path.
 
     Args:
         absolute_path (str): The absolute path to a directory or file.
 
@@ -150,17 +156,16 @@
         elif isinstance(event, cdp.target.TargetCreated):
             target_info: cdp.target.TargetInfo = event.target_info
             from .tab import Tab
 
             new_target = Tab(
                 (
                     f"ws://{self.config.host}:{self.config.port}"
-                    f"/devtools/{target_info.type_.lower()}"
-                    f"/{target_info.target_id}"
-                ),
+                    f"/devtools/page"  # all types are 'page' internally in chrome apparently
+                    f"/{target_info.target_id}"                ),
                 target=target_info,
                 browser=self,
             )
             self.targets.append(new_target)
 
 
         elif isinstance(event, cdp.target.TargetDestroyed):
@@ -219,26 +224,14 @@
             if self._process.returncode is not None:
                 return await self.create(config=self.config)
             print("ignored! this call has no effect when already running.")
             return
 
         self.config.host = self.config.host or "127.0.0.1"
         self.config.port = self.config.port or free_port()
-        if not os.path.exists(self.config.browser_executable_path):
-            raise DriverException(
-                (
-                    """
-                ---------------------
-                Could not determine browser executable.
-                ---------------------
-                Make sure your browser is installed in the default location (path).
-                If you are sure about the browser executable."""
-                )
-            )
-
         exe = self.config.browser_executable_path
         params = self.config()
         self._process: asyncio.subprocess.Process = (
             await asyncio.create_subprocess_exec(
                 # self.config.browser_executable_path,
                 # *cmdparams,
                 exe,
@@ -333,17 +326,17 @@
                     break
             else:
 
                 self.targets.append(
                     Connection(
                         (
                             f"ws://{self.config.host}:{self.config.port}"
-                            f"/devtools/{t.type_.lower()}"
+                            f"/devtools/page"  # all types are 'page' somehow
                             f"/{t.target_id}"
-                        ),
+                                                                            ),
                         target=t,
                         _owner=self,
                     )
                 )
 
         await asyncio.sleep(0)
 
@@ -373,33 +366,37 @@
                 if self._i != len(self.tabs):
                     self._i += 1
                 else:
                     del self._i
 
 
     def close(self):
-        try:
-            # asyncio.get_running_loop().create_task(self.connection.send(cdp.browser.close()))
-            asyncio.get_event_loop().create_task(self.connection.aclose())
-        except RuntimeError:
-            if self.connection:
-                try:
-                    # asyncio.run(self.connection.send(cdp.browser.close()))
-                    asyncio.run(self.connection.aclose())
-                except Exception:
-                    pass
+        # No need we are killing
+        # try:
+        #     # asyncio.get_running_loop().create_task(self.connection.send(cdp.browser.close()))
+        #     asyncio.get_event_loop().create_task(self.connection.aclose())
+        # except RuntimeError:
+        #     if self.connection:
+        #         try:
+        #             # asyncio.run(self.connection.send(cdp.browser.close()))
+        #             asyncio.run(self.connection.aclose())
+        #         except Exception:
+        #             pass
+        # except Exception:   
+        #     pass
+        
         for _ in range(3):
             try:
-                self._process.terminate()
-            
+                # print("killing browser")
+                kill_process(self._process_pid)
+                # print("killed browser")            
                 break
             except (Exception,):
                 try:
-                    self._process.kill()
-                
+                    kill_process(self._process_pid)
                     break
                 except (Exception,):
                     try:
                         if hasattr(self, "browser_process_pid"):
                             os.kill(self._process_pid, 15)
                             break
                     except (TypeError,):
@@ -512,15 +509,17 @@
         self.host, self.port = addr
         self.api = "http://%s:%d" % (self.host, self.port)
 
     async def get(self, endpoint: str):
         return await self._request(endpoint)
 
     async def _request(self, endpoint, method: str = "get", data: dict = None):
-        url = urllib.parse.urljoin(self.api, "/".join(["json", endpoint]))
+        url = urllib.parse.urljoin(
+            self.api, f"json/{endpoint}" if endpoint else "/json"
+        )
         if data and method.lower() == "get":
             raise DriverException("get requests cannot contain data")
         if not url:
             url = self.api + endpoint
         request = urllib.request.Request(url)
         request.method = method
         request.data = None
```

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/connection.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,17 +320,24 @@
             if not self.mapper:
                 self.__count__ = itertools.count(0)
             tx.id = next(self.__count__)
             self.mapper.update({tx.id: tx})
 
             if not _is_update:
                 await self._register_handlers()
-            await self.websocket.send(tx.message)
+            
+            maxtmt = 180
+            await asyncio.wait_for(self.websocket.send(tx.message), timeout=maxtmt)
             try:
-                return await tx
+                try:
+                  u =  await asyncio.wait_for(tx, timeout=maxtmt)
+                except asyncio.TimeoutError as e:
+                  raise e
+
+                return u
             except ProtocolException as e:
                 e.message += f"\ncommand:{tx.method}\nparams:{tx.params}"
                 raise e
 
         except Exception:
             await self.aclose()
```

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/custom_storage_cdp.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/custom_storage_cdp.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/element.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/element.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/env.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/env.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/profiles.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/profiles.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/tab.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/tab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import asyncio
 import json
 import typing
 from datetime import datetime
 from typing import List, Union, Optional
 
-from ..exceptions import ElementWithSelectorNotFoundException, JavascriptException, ProtocolException, InvalidFilenameException, JavascriptSyntaxException, ScreenshotException
+from ..exceptions import ElementWithSelectorNotFoundException, DriverException, JavascriptException, ProtocolException, InvalidFilenameException, JavascriptSyntaxException, ScreenshotException
 from ..driver_utils import create_screenshot_filename, get_download_directory, get_download_filename
 
 from . import element
 from . import util
 from .config import PathLike
 from .connection import Connection
 from .. import cdp
@@ -17,15 +17,20 @@
 
 bannedtextsearchresults = set(["title","meta", "script", "link", "style", "head"])
 def isbanned( node):
         return node.node_name.lower() in bannedtextsearchresults
 
 def issametype(node, type):
         return node.node_name.lower() ==type
-
+def append_safe(results, elem, text, exact_match):
+            if exact_match:
+                if text == elem.text:
+                    results.append(elem)
+            else:
+                results.append(elem)
 class Tab(Connection):
     """
     :ref:`tab` is the controlling mechanism/connection to a 'target',
     for most of us 'target' can be read as 'tab'. however it could also
     be an iframe, serviceworker or background script for example,
     although there isn't much to control for those.
 
@@ -160,15 +165,16 @@
 
     async def find(
         self,
         text: str,
         best_match: bool = False,
         return_enclosing_element=True,
         timeout: Union[int, float] = 10,
-        type=None
+        type=None, 
+        exact_match = False,
     ):
         """
         find single element by text
         can also be used to wait for such element to appear.
 
         :param text: text to search for. note: script contents are also considered text
         :type text: str
@@ -198,21 +204,21 @@
         :param timeout: raise timeout exception when after this many seconds nothing is found.
         :type timeout: float,int
         """
         loop = asyncio.get_running_loop()
         now = loop.time()
 
         item = await self.find_element_by_text(
-            text, best_match, return_enclosing_element, type=type
+            text, best_match, return_enclosing_element, type=type, exact_match=exact_match
         )
         if timeout:
             while not item:
                 await self
                 item = await self.find_element_by_text(
-                    text, best_match, return_enclosing_element, type=type
+                    text, best_match, return_enclosing_element, type=type, exact_match=exact_match
                 )
                 if loop.time() - now > timeout:
                     return None
                 await self.sleep(0.5)
         return item
 
     async def select(
@@ -245,34 +251,35 @@
                 await self.sleep(0.5)
         return item
     
     async def find_all(
         self,
         text: str,
         timeout: Union[int, float] = 10,
-        type=None
+        type=None,
+        exact_match = False,
     ):
         """
         find multiple elements by text
         can also be used to wait for such element to appear.
 
         :param text: text to search for. note: script contents are also considered text
         :type text: str
 
         :param timeout: raise timeout exception when after this many seconds nothing is found.
         :type timeout: float,int
         """
         loop = asyncio.get_running_loop()
         now = loop.time()
 
-        results = await self.find_elements_by_text(text, type=type)
+        results = await self.find_elements_by_text(text, type=type, exact_match=exact_match)
         if timeout:
             while not results:
                 await self
-                results = await self.find_elements_by_text(text, type=type)
+                results = await self.find_elements_by_text(text, type=type, exact_match=exact_match)
                 if loop.time() - now > timeout:
                     return []
                 await self.sleep(0.5)
         return results
 
     async def select_all(
         self,
@@ -388,15 +395,16 @@
         if not _node:
             doc: cdp.dom.Node = await self.send(cdp.dom.get_document(-1, True))
         else:
             doc = _node
             if _node.node_name == "IFRAME":
                 doc = _node.content_document
         node_id = None
-
+        if not doc:
+            raise DriverException("Failed to find Document")
         try:
             node_id = await self.send(cdp.dom.query_selector(doc.node_id, selector))
 
         except ProtocolException as e:
             if _node is not None:
                 if "could not find node" in e.message.lower():
                     if getattr(_node, "__last", None):
@@ -420,14 +428,15 @@
         return element.create(node, self, doc)
 
     async def find_elements_by_text(
         self,
         text: str,
         tag_hint: Optional[str] = None,
         type=None,
+        exact_match = False,
     ) -> List[element.Element]:
         """
         returns element which match the given text.
         please note: this may (or will) also return any other element (like inline scripts),
         which happen to contain that text.
 
         :param text:
@@ -458,15 +467,15 @@
                     continue
                 # remote_object = await self.send(cdp.dom.resolve_node(backend_node_id=node.backend_node_id))
                 # node_id = await self.send(cdp.dom.request_node(object_id=remote_object.object_id))
             try:
                 elem = element.create(node, self, doc)
             except:  # noqa
                 continue
-            await self.checktextnodeandappend(type, results, elem)  
+            await self.checktextnodeandappend(type, results, elem, text, exact_match)  
 
         # since we already fetched the entire doc, including shadow and frames
         # let's also search through the iframes
         # iframes = util.filter_recurse_all(doc, lambda node: node.node_name == "IFRAME")
         # if iframes:
             # iframes_elems = [
             #     element.create(iframe, self, iframe.content_document)
@@ -495,14 +504,15 @@
 
     async def find_element_by_text(
         self,
         text: str,
         best_match: Optional[bool] = False,
         return_enclosing_element: Optional[bool] = True,
         type=None,
+        exact_match= False,
     ) -> Union[element.Element, None]:
         """
         finds and returns the first element containing <text>, or best match
 
         :param text:
         :type text:
         :param best_match:  when True, which is MUCH more expensive (thus much slower),
@@ -532,15 +542,15 @@
               return results[0]
 
             node = util.filter_recurse(doc, lambda n: n.node_id == nid)
             try:
                 elem = element.create(node, self, doc)
             except:  # noqa
                 continue
-            await self.checktextnodeandappend(type, results, elem)  
+            await self.checktextnodeandappend(type, results, elem, text, exact_match)   
 
         # since we already fetched the entire doc, including shadow and frames
         # let's also search through the iframes
         # iframes = util.filter_recurse_all(doc, lambda node: node.node_name == "IFRAME")
         # if iframes:
         #     iframes_elems = [
         #         element.create(iframe, self, iframe.content_document)
@@ -557,52 +567,46 @@
                 #         element.create(text_node, self, iframe_elem.tree)
                 #         for text_node in iframe_text_nodes
                 #     ]
                 #     results.extend(text_node.parent for text_node in iframe_text_elems)
         try:
             if not results:
                 return
-            if best_match:
-                closest_by_length = min(
-                    results, key=lambda el: abs(len(text) - len(el.text_all))
-                )
-                elem = closest_by_length or results[0]
-
-                return elem
-            else:
                 # naively just return the first result
-                for elem in results:
-                    if elem:
-                        return elem
+            for elem in results:
+                if elem:
+                    return elem
         finally:
             await self.send(cdp.dom.disable())
 
-    async def checktextnodeandappend(self, type, results, elem):
+    async def checktextnodeandappend(self, type, results, elem, text, exact_match):
+        
+
         if elem.node_type == 3:
                 # if found element is a text node (which is plain text, and useless for our purpose),
                 # we return the parent element of the node (which is often a tag which can have text between their
                 # opening and closing tags (that is most tags, except for example "img" and "video", "br")
             if not elem.parent:
                     # check if parent actually has a parent and update it to be absolutely sure
                 await elem.update()
             final = elem.parent or elem
             if final:
                 if type:
                     if issametype(final.node, type):
-                        results.append(final)  
+                        append_safe(results, final, text, exact_match)
                 else:
                     if not isbanned(final.node):
-                        results.append(final)  
+                        append_safe(results, final, text, exact_match)
         else:
                 if type:
                     if issametype(elem.node, type):
-                        results.append(elem)
+                        append_safe(results, elem, text, exact_match)
                 else:
                     if not isbanned(elem.node):
-                        results.append(elem)
+                        append_safe(results, elem, text, exact_match)
 
 
     async def evaluate(
         self, expression: str, await_promise=False, return_by_value=True
     ):
         expression = r"""(() => {
 const resp = (() => { SCRIPT })()
@@ -625,34 +629,21 @@
 
         if not response:
             raise JavascriptSyntaxException()
 
         remote_object, errors = response
         if errors:
             raise JavascriptException(errors)
-            if not return_by_value:
-                return remote_object, errors
-            return errors.to_json()
         if remote_object:
             if return_by_value:
                 if remote_object.value:
                     return json.loads(util.get_remote_object_value(remote_object)).get("x")
 
             else:
                 return remote_object, errors
-            # if getattr(remote_object, "subtype", None) == "error":
-            #     val = remote_object.description
-            #     return {"error": val, "stack": errors}
-        #     try:
-        #         return json.loads(remote_object.value)
-        #     except:
-        #         return remote_object.value
-        # if exc:
-        #     return exc
-
     async def js_dumps(
         self, obj_name: str, return_by_value: Optional[bool] = True
     ) -> typing.Union[
         typing.Dict,
         typing.Tuple[cdp.runtime.RemoteObject, cdp.runtime.ExceptionDetails],
     ]:
         """
```

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/core/util.py` & `botasaurus_driver-4.0.5/botasaurus_driver/core/util.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/driver.py` & `botasaurus_driver-4.0.5/botasaurus_driver/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     create_video_filename,
     ensure_supports_file_upload,
     ensure_supports_multiple_upload,
     perform_accept_google_cookies_action,
     sleep_for_n_seconds,
     sleep_forever,
 )
-from .exceptions import CheckboxElementForLabelNotFoundException, ElementWithTextNotFoundException, IframeNotFoundException, InputElementForLabelNotFoundException,  PageNotFoundException
+from .exceptions import CheckboxElementForLabelNotFoundException, ElementWithTextNotFoundException, IframeNotFoundException, InputElementForLabelNotFoundException, NoProfileException,  PageNotFoundException
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
-from .solve_cloudflare_captcha import bypass_if_detected
+from .solve_cloudflare_captcha import bypass_if_detected,  wait_till_document_is_ready
 from .core.browser import Browser
 from .core.util import start
 from .core.tab import Tab
 from .core.element import Element as CoreElement
 
 class Wait:
     SHORT = 4
@@ -63,32 +63,21 @@
         if time.time() - start_time > timeout:
             internal_frame_id = str(internal_elem.frame_id)
             raise IframeNotFoundException(internal_frame_id)
 
         time.sleep(0.1)
         # time.sleep(2)
 
-def wait_till_document_is_ready(tab):
-    while True:
-        sleep(0.1)
-        try:
-            script = "return document.readyState === 'complete'"
-            response = tab._run(tab.evaluate(script, await_promise=True))
-            if response:
-                break
-        except Exception as e:
-            print("An exception occurred", e)
-
 def add_loop_to_tab(value, loop):
     value.loop = loop
 
 def wait_for_iframe_tab_load(driver, iframe_tab):
     add_loop_to_tab(iframe_tab, driver._loop)
     iframe_tab.websocket_url = iframe_tab.websocket_url.replace("iframe", "page")
-    wait_till_document_is_ready(iframe_tab)
+    # wait_till_document_is_ready(iframe_tab, True)
 
 def create_iframe_element(driver, internal_elem):
     iframe_tab = get_iframe_tab(driver, internal_elem)
     wait_for_iframe_tab_load(driver, iframe_tab)
     
     return IframeElement(driver.config, iframe_tab, driver._loop, driver._browser)
 
@@ -422,14 +411,20 @@
                     input_elem = label_elem.select(get_inside_input_selector(type), wait=None)
                 
                 if input_elem:
                     return input_elem
     
     return None
 
+def block_if_should(driver):
+        if driver.config.block_images_and_css:
+            driver.block_images_and_css()
+        elif driver.config.block_images:
+            driver.block_images()
+
 class DriverBase():
     def __init__(self, config,_tab_value, _loop, _browser):
             self.config = config
             self._tab_value = _tab_value
             self._loop = _loop
             self._browser = _browser
 
@@ -449,44 +444,64 @@
         add_loop_to_tab(value, self._loop)
         self._tab_value = value
 
     @property
     def current_url(self):
         return self.run_js("return window.location.href")
 
+
+    @property
+    def title(self):
+        el = self.select('title', None)
+        if el:
+            return el.text
+
     @property
     def page_text(self):
         return self.select("body").text
 
     @property
     def page_html(self):
         return self._run(self._tab.get_content())
 
     @property
     def local_storage(self):
         return LocalStorage(self)
+
+    @property
+    def profile(self):
+        from .profile import Profile
+        if self.config.profile:
+            return Profile(self.config.profile)
+        else: 
+            raise NoProfileException()
     
     def _update_targets(self):
         return self._run(self._browser.update_targets())
 
     def get(self, link: str, bypass_cloudflare=False, wait: Optional[int] = None):
         self._tab = self._run(self._browser.get(link))
         self.sleep(wait)
-        if self.config.wait_for_complete_page_load:
-            wait_till_document_is_ready(self._tab)
+        wait_till_document_is_ready(self._tab, self.config.wait_for_complete_page_load)
         if bypass_cloudflare:
             self.detect_and_bypass_cloudflare()
+        block_if_should(self)
 
-    def get_via(self, link: str, source_referrer: str, bypass_cloudflare=False, wait: Optional[int] = None):
-        self._tab = self._run(self._browser.get(link, referrer=source_referrer))
+    def get_via(self, link: str, referer: str, bypass_cloudflare=False, wait: Optional[int] = None):
+        
+        referer = referer.rstrip("/")  + "/"
+        self._tab = self._run(self._browser.get(link, referrer=referer))
+        
         self.sleep(wait)
-        if self.config.wait_for_complete_page_load:
-            wait_till_document_is_ready(self._tab)
+        
+        wait_till_document_is_ready(self._tab, self.config.wait_for_complete_page_load)
+        
         if bypass_cloudflare:
             self.detect_and_bypass_cloudflare()
+        block_if_should(self)
 
     def google_get(
         self, link: str, bypass_cloudflare=False, wait: Optional[int] = None, accept_google_cookies: bool = False
     ):
         if accept_google_cookies:
             # No need to accept cookies multiple times
             if hasattr(self, 'has_accepted_google_cookies') and self.has_accepted_google_cookies:
@@ -502,17 +517,22 @@
         self.run_js(f'window.location.href = "{link}";')
         if currenturl != link:
             while True:
                 if currenturl != self.current_url:
                     break
                 sleep(0.1)
         self.sleep(wait)
+
+        wait_till_document_is_ready(self._tab, self.config.wait_for_complete_page_load)
+
         if bypass_cloudflare:
             self.detect_and_bypass_cloudflare()
 
+        block_if_should(self)
+
     def run_js(self, script: str) -> Any:
         # Run it in IIFE for isloation
         return self._run(self._tab.evaluate(script, await_promise=True))
 
     def run_cdp_command(self, command) -> Any:
         return self._run(self._tab.run_cdp_command(command))
 
@@ -531,27 +551,42 @@
         elems = self._run(elems_coro)
         return [make_element(self, self._tab, e) for e in elems]
 
     def select_iframe(self, selector: str, wait: Optional[int] = Wait.SHORT) -> 'IframeElement':
         return self.select(selector, wait)
 
     def get_element_containing_text(
-        self, text: str, type: Optional[str] = None, wait: Optional[int] = Wait.SHORT
+        self, text: str, wait: Optional[int] = Wait.SHORT, type: Optional[str] = None, 
     ) -> Element:
         elem_coro = self._tab.find(text, type=type, timeout=wait)
         elem = self._run(elem_coro)
         return make_element(self, self._tab, elem) if elem else None
 
     def get_all_elements_containing_text(
-        self, text: str, type: Optional[str] = None, wait: Optional[int] = Wait.SHORT
+        self, text: str, wait: Optional[int] = Wait.SHORT, type: Optional[str] = None, 
     ) -> List[Element]:
         elems_coro = self._tab.find_all(text, type=type, timeout=wait)
         elems = self._run(elems_coro)
         return [make_element(self, self._tab, e) for e in elems]
 
+
+    def get_element_with_exact_text(
+        self, text: str,  wait: Optional[int] = Wait.SHORT,type: Optional[str] = None,
+    ) -> Element:
+        elem_coro = self._tab.find(text, type=type, timeout=wait, exact_match=True)
+        elem = self._run(elem_coro)
+        return make_element(self, self._tab, elem) if elem else None
+
+    def get_all_elements_with_exact_text(
+        self, text: str,  wait: Optional[int] = Wait.SHORT, type: Optional[str] = None,
+    ) -> List[Element]:
+        elems_coro = self._tab.find_all(text, type=type, timeout=wait, exact_match=True)
+        elems = self._run(elems_coro)
+        return [make_element(self, self._tab, e) for e in elems]
+
     def is_element_present(self, selector: str, wait: Optional[int] = None) -> bool:
         return self.select(selector, wait) is not None
 
     def click(self, selector: str, wait: Optional[int] = Wait.SHORT) -> None:
         elem = self.wait_for_element(selector, wait)
         elem.click()
 
@@ -677,15 +712,15 @@
             elems = [elem for elem in elems if url_contains_text in elem.src]
 
         if element_contains_text:
             elems = [elem for elem in elems if element_contains_text in elem.text]
 
         return [elem.src for elem in elems]
 
-    def get_element_text(self, selector: str, wait: Optional[int] = Wait.SHORT) -> str:
+    def get_text(self, selector: str, wait: Optional[int] = Wait.SHORT) -> str:
         elem = self.wait_for_element(selector, wait)
         return elem.text
 
     def wait_for_element(
         self, selector: str, wait: Optional[int] = Wait.SHORT
     ) -> Element:
         return make_element(self, self._tab, self._run(self._tab.wait_for(selector, timeout=wait)))
@@ -779,19 +814,19 @@
     def long_random_sleep(self) -> None:
         sleep_for_n_seconds(uniform(6, 9))
 
     def sleep_forever(self) -> None:
         sleep_forever()
 
     def get_bot_detected_by(self) -> str:
-        clf = self.select("#challenge-running", None)
-        if clf is not None:
+        clf = self.select("#challenge-running", wait=None)
+        if clf is not None or self.title == "Just a moment...":
             return Opponent.CLOUDFLARE
 
-        pmx = self.get_element_containing_text("Please verify you are a human", None)
+        pmx = self.get_element_containing_text("Please verify you are a human", wait=None)
 
         if pmx is not None:
             return Opponent.PERIMETER_X
 
         return None
 
     def is_bot_detected(self) -> bool:
@@ -877,21 +912,21 @@
                 for url in expected_url:
                     if url == driver.current_url:
                         return True
             return False
 
         if wait is None:
             if check_page(self, expected_url):
-                wait_till_document_is_ready(self._tab)
+                wait_till_document_is_ready(self._tab, True)
                 return True
         else:
             time = 0
             while time < wait:
                 if check_page(self, expected_url):
-                    wait_till_document_is_ready(self._tab)
+                    wait_till_document_is_ready(self._tab, True)
                     return True
                 sleep_time = 0.2
                 time += sleep_time
                 sleep(sleep_time)
 
             if raise_exception:
                 raise PageNotFoundException(expected_url, wait)
@@ -955,29 +990,32 @@
         
         self.config = Config(headless=headless,proxy=proxy,profile=profile,tiny_profile=tiny_profile,block_images=block_images,block_images_and_css=block_images_and_css,wait_for_complete_page_load=wait_for_complete_page_load,extensions=extensions,arguments=arguments,user_agent=user_agent,window_size=window_size,lang=lang,beep=beep)
         self._tab_value: Tab = None
 
         self._loop = asyncio.new_event_loop()
         asyncio.set_event_loop(self._loop)
         self._browser: Browser = self._run(start(self.config))
-
-        if self.config.block_images_and_css:
-            self.block_urls(['.css', '.jpg', '.jpeg', '.png', '.svg', '.gif', '.woff', '.pdf', '.zip'])            
-        elif self.config.block_images:
-            self.block_urls(['.jpg', '.jpeg', '.png', '.svg', '.gif', '.woff', '.pdf', '.zip'])
+    
+        block_if_should(self)
 
         if self.config.tiny_profile:
             load_cookies(self, self.config.profile)        
      
         super().__init__(self.config, self._tab_value, self._loop, self._browser)
 
     def block_urls(self, urls) -> None:
         # You usually don't need to close it because we automatically close it when script is cancelled (ctrl + c) or completed 
         self.run_cdp_command(enable_network())
         self.run_cdp_command(block_urls(urls))
 
+    def block_images_and_css(self) -> None:
+        self.block_urls(['.css', '.jpg', '.jpeg', '.png', '.svg', '.gif', '.woff', '.pdf', '.zip'])    
+
+    def block_images(self) -> None:
+        self.block_urls(['.jpg', '.jpeg', '.png', '.svg', '.gif', '.woff', '.pdf', '.zip'])
+
     def close(self) -> None:
         if self.config.tiny_profile:
             save_cookies(self, self.config.profile)        
 
         # You usually don't need to close it because we automatically close it when script is cancelled (ctrl + c) or completed 
         self._browser.close()
```

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/driver_utils.py` & `botasaurus_driver-4.0.5/botasaurus_driver/driver_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/exceptions.py` & `botasaurus_driver-4.0.5/botasaurus_driver/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,19 @@
         self.message = message
         super().__init__(self.message)
 
 class IframeNotFoundException(DriverException):
     def init(self, iframe_id):
         super().init(f"Iframe {iframe_id} does not exist in the targets.")
 
+
+class NoProfileException(DriverException):
+    def init(self):
+        super().init(f"No profile provided.")
+
 class ElementWithTextNotFoundException(DriverException):
     def __init__(self, text):
         super().__init__(f"Cannot find element containing text: '{text}'.")
 
 class ElementWithSelectorNotFoundException(DriverException):
     def __init__(self, selector):
         super().__init__(f"Cannot find element with selector: '{selector}'.")
```

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/lang.py` & `botasaurus_driver-4.0.5/botasaurus_driver/lang.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/local_storage_driver.py` & `botasaurus_driver-4.0.5/botasaurus_driver/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/tiny_profile.py` & `botasaurus_driver-4.0.5/botasaurus_driver/tiny_profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/user_agent.py` & `botasaurus_driver-4.0.5/botasaurus_driver/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver/window_size.py` & `botasaurus_driver-4.0.5/botasaurus_driver/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus_driver-4.0.3/botasaurus_driver.egg-info/SOURCES.txt` & `botasaurus_driver-4.0.5/botasaurus_driver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 botasaurus_driver/beep_utils.py
 botasaurus_driver/driver.py
 botasaurus_driver/driver_utils.py
 botasaurus_driver/exceptions.py
 botasaurus_driver/lang.py
 botasaurus_driver/local_storage_driver.py
 botasaurus_driver/opponent.py
+botasaurus_driver/profile.py
 botasaurus_driver/solve_cloudflare_captcha.py
 botasaurus_driver/tiny_profile.py
 botasaurus_driver/user_agent.py
 botasaurus_driver/window_size.py
 botasaurus_driver.egg-info/PKG-INFO
 botasaurus_driver.egg-info/SOURCES.txt
 botasaurus_driver.egg-info/dependency_links.txt
```

### Comparing `botasaurus_driver-4.0.3/pyproject.toml` & `botasaurus_driver-4.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botasaurus_driver" # Required
-version="4.0.3"  # Required
+version="4.0.5"  # Required
 description = "Super Fast, Super Anti-Detect, and Super Intuitive Web Driver"
 readme = {file = "README.md", content-type = "text/markdown"} # Optional
 requires-python = ">=3.5"
 license = {file = "LICENSE"}
 keywords = [
     "webdriver", "browser", "captcha", "web-scraping",
     "selenium", "navigator", "python3", "cloudflare",
```

