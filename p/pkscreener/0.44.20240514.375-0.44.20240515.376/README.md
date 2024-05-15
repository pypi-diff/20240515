# Comparing `tmp/pkscreener-0.44.20240514.375.tar.gz` & `tmp/pkscreener-0.44.20240515.376.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240514.375.tar", last modified: Tue May 14 19:09:24 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240515.376.tar", last modified: Wed May 15 10:24:08 2024, max compression
```

## Comparing `pkscreener-0.44.20240514.375.tar` & `pkscreener-0.44.20240515.376.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/
--rw-rw-rw-   0        0        0     1086 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.211229 pkscreener-0.44.20240514.375/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34202 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11409 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    40473 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12527 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   154876 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-14 19:09:15.000000 pkscreener-0.44.20240514.375/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   139571 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1041 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    32153 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.211229 pkscreener-0.44.20240514.375/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/
+-rw-rw-rw-   0        0        0     1086 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.662029 pkscreener-0.44.20240515.376/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34204 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11409 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    42096 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   154876 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83651 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-15 10:24:01.000000 pkscreener-0.44.20240515.376/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   140752 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1041 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    32153 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:24:08.662029 pkscreener-0.44.20240515.376/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-15 10:24:08.000000 pkscreener-0.44.20240515.376/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-15 10:24:08.678249 pkscreener-0.44.20240515.376/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-15 10:20:13.000000 pkscreener-0.44.20240515.376/setup.py
```

### Comparing `pkscreener-0.44.20240514.375/LICENSE` & `pkscreener-0.44.20240515.376/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/LICENSE-Others` & `pkscreener-0.44.20240515.376/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/PKG-INFO` & `pkscreener-0.44.20240515.376/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.375
+Version: 0.44.20240515.376
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.375.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.376.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.375/README.md` & `pkscreener-0.44.20240515.376/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.375/pkscreener/__init__.py` & `pkscreener-0.44.20240515.376/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,16 @@
         self.maxBacktestWindow = 30
         self.minVolume = 10000
         self.morninganalysiscandlenumber = 25 # 9:40am IST, since market opens at 9:15am IST
         self.morninganalysiscandleduration = '1m'
         self.logger = None
         self.showPastStrategyData = False
         self.atrTrailingStopSensitivity = 1
-        self.atrTrailingStopPeriod = 21
-        self.atrTrailingStopEMAPeriod = 9
+        self.atrTrailingStopPeriod = 10
+        self.atrTrailingStopEMAPeriod = 200
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 3
         self.maxNumResultRowsInMonitor = 2
         self.calculatersiintraday = False
```

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/MenuOptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -568,15 +568,15 @@
             level0MenuDict,
             renderExceptionKeys=["P", "T", "E", "U", "Z", "L", "D"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList,coloredValues=["X"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -640,34 +640,34 @@
                     ""
                 )
             return menuText
         
     def renderLevel1_T_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
+        defaultKey = 'L' if configManager.period == '280d' else 'S'
         menuText = self.fromDictionary(
             level1_T_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList,coloredValues=[defaultKey])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
                     + "[+] Select a configuration period for Screening:"
                     + colorText.END
                 )
-                defaultKey = 'L' if configManager.period == '280d' else 'S'
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
     Enter your choice > (default is """
                     + colorText.WARN
@@ -684,15 +684,15 @@
             level1_P_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["2"])
+        ).render(asList=asList, coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -719,15 +719,15 @@
             level2_P_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList,coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -754,15 +754,15 @@
             level1_X_MenuDict,
             renderExceptionKeys=["W", "0", "M", "15"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.THREE_PER_ROW,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["15"])
+        ).render(asList=asList, coloredValues=["15",str(configManager.defaultIndex)])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -789,15 +789,15 @@
             level2_T_MenuDict_L,
             renderExceptionKeys=["4","5","M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList, coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -805,31 +805,34 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
-                    + colorText.END
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("1").keyTextLabel()
+                    + ")  "
+                    "" + colorText.END
                 )
             return menuText
 
     def level2_T_MenuDict_S(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         menuText = self.fromDictionary(
             level2_T_MenuDict_S,
             renderExceptionKeys=["5", "M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList, coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -837,31 +840,34 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
-                    + colorText.END
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("1").keyTextLabel()
+                    + ")  "
+                    "" + colorText.END
                 )
             return menuText
         
     def renderLevel2_X_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
         menuText = self.fromDictionary(
             level2_X_MenuDict,
             renderExceptionKeys=["0", "42", "M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.TWO_PER_ROW,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList, coloredValues=["9"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -869,15 +875,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("9").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_Reversal_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
@@ -885,15 +893,15 @@
             level3_X_Reversal_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList,coloredValues=["3"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -901,15 +909,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("3").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_ChartPattern_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -917,15 +927,15 @@
             level3_X_ChartPattern_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList,coloredValues=["3"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -933,15 +943,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("3").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_PopularStocks_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -949,15 +961,15 @@
             level3_X_PopularStocks_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList, coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -965,15 +977,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("1").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel3_X_StockPerformance_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -981,15 +995,15 @@
             level3_X_StockPerformance_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList,coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -997,15 +1011,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("1").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
     def renderLevel4_X_Lorenzian_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
@@ -1013,15 +1029,15 @@
             level4_X_Lorenzian_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList, coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1029,15 +1045,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("1").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
 
     def renderLevel4_X_ChartPattern_BBands_SQZ_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
@@ -1046,15 +1064,15 @@
             level4_X_ChartPattern_BBands_SQZ_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList, coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1062,15 +1080,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("1").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
 
     def renderLevel4_X_ChartPattern_Confluence_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
@@ -1079,15 +1099,15 @@
             level4_X_ChartPattern_Confluence_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList)
+        ).render(asList=asList,coloredValues=["1"])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1095,15 +1115,17 @@
                     + colorText.END
                 )
                 OutputControls().printOutput(
                     colorText.BOLD
                     + menuText
                     + """
 
-            """
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + self.find("1").keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
         
 # Fundamentally good compnaies but nearing 52 week low
 # https://www.tickertape.in/screener/equity/prebuilt/SCR0005
```

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/OtaUpdater.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
                     action = input(
                             colorText.BOLD
                             + colorText.FAIL
                             + (
                                 f"\n[+] New {updateType} Software update (v%s) available. Download Now (Size: %dMB)? [Y/N]: "
                                 % (str(tag), size)
                             )
-                        )
+                        ) or "y"
                 except EOFError: # user pressed enter
                     action = "y"
                     pass
                 if action is not None and action.lower() == "y":
                     try:
                         if "Windows" in platform.system():
                             OTAUpdater.updateForWindows(OTAUpdater.checkForUpdate.url)
```

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/Utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1129,16 +1129,16 @@
         isSaved = False
         try:
             if defaultAnswer is None:
                 response = str(
                     input(
                         colorText.BOLD
                         + colorText.WARN
-                        + "[>] Do you want to save the results in excel file? [Y/N]: "
-                    )
+                        + "[>] Do you want to save the results in excel file? [Y/N](Default:Y): "
+                    ) or "Y"
                 ).upper()
             else:
                 response = defaultAnswer
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             response = "Y"
         if response is not None and response.upper() != "N":
@@ -1212,106 +1212,110 @@
             if defaultAnswer is None:
                 response = str(
                     input(
                         colorText.BOLD
                         + colorText.WARN
                         + "[>] "
                         + cache_file
-                        + " already exists. Do you want to replace this? [Y/N]: "
-                    )
-                ).upper()
+                        + " already exists. Do you want to replace this? [Y/N] (Default: Y): "
+                ) or "Y").upper()
             else:
                 response = defaultAnswer
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
         return "Y" if response != "N" else "N"
 
     # Prompt for asking RSI
     def promptRSIValues():
+        tools.clearScreen(forceTop=True)
         try:
             minRSI, maxRSI = int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
-                    + "\n[+] Enter Min RSI value: "
+                    + "\n[+] Enter Min RSI value (Default=55): "
                     + colorText.END
-                )
+                ) or 55
             ), int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
-                    + "[+] Enter Max RSI value: "
+                    + "[+] Enter Max RSI value (Default=68): "
                     + colorText.END
-                )
+                ) or "68"
             )
             if (
                 (minRSI >= 0 and minRSI <= 100)
                 and (maxRSI >= 0 and maxRSI <= 100)
                 and (minRSI <= maxRSI)
             ):
                 return (minRSI, maxRSI)
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             return (0, 0)
 
     # Prompt for asking CCI
     def promptCCIValues(minCCI=None, maxCCI=None):
+        tools.clearScreen(forceTop=True)
         if minCCI is not None and maxCCI is not None:
             return minCCI, maxCCI
         try:
             minCCI, maxCCI = int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
-                    + "\n[+] Enter Min CCI value: "
+                    + "\n[+] Enter Min CCI value (Default=110): "
                     + colorText.END
-                )
+                ) or "110"
             ), int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
-                    + "[+] Enter Max CCI value: "
+                    + "[+] Enter Max CCI value (Default=300): "
                     + colorText.END
-                )
+                ) or "300"
             )
             if minCCI <= maxCCI:
                 return (minCCI, maxCCI)
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             return (-100, 100)
 
     # Prompt for asking Volume ratio
     def promptVolumeMultiplier(volumeRatio=None):
+        tools.clearScreen(forceTop=True)
         if volumeRatio is not None:
             return volumeRatio
         try:
             volumeRatio = float(
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + "\n[+] Enter Min Volume ratio value (Default = 2.5): "
                     + colorText.END
-                )
+                ) or "2.5"
             )
             if volumeRatio > 0:
                 return volumeRatio
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             return 2
 
     def promptMenus(menu):
+        tools.clearScreen(forceTop=True)
         m = menus()
         m.level = menu.level if menu is not None else 0
         return m.renderForMenu(menu)
 
     def promptChartPatternSubMenu(menu,respChartPattern):
+        tools.clearScreen(forceTop=True)
         m3 = menus()
         m3.renderForMenu(menu,asList=True)
         lMenu =  m3.find(str(respChartPattern))
         maLength = tools.promptSubMenuOptions(lMenu)
         return maLength
     
     # Prompt for submenu options
@@ -1320,15 +1324,15 @@
             tools.promptMenus(menu=menu)
             resp = int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + """[+] Select Option:"""
                     + colorText.END
-                )
+                ) or "1"
             )
             if resp >= 0 and resp <= 10:
                 return resp
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             input(
@@ -1345,26 +1349,26 @@
             tools.promptMenus(menu=menu)
             resp = int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + """[+] Select Option:"""
                     + colorText.END
-                )
+                ) or "3"
             )
             if resp >= 0 and resp <= 10:
                 if resp == 4:
                     try:
                         maLength = int(
                             input(
                                 colorText.BOLD
                                 + colorText.WARN
-                                + "\n[+] Enter MA Length (E.g. 50 or 200): "
+                                + "\n[+] Enter MA Length (E.g. 50 or 200) (Default=50): "
                                 + colorText.END
-                            )
+                            ) or "50"
                         )
                         return resp, maLength
                     except ValueError as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
                         OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.FAIL
@@ -1374,17 +1378,17 @@
                         raise ValueError
                 elif resp == 6:
                     try:
                         maLength = int(
                             input(
                                 colorText.BOLD
                                 + colorText.WARN
-                                + "\n[+] Enter NR timeframe [Integer Number] (E.g. 4, 7, etc.): "
+                                + "\n[+] Enter NR timeframe [Integer Number] (E.g. 4, 7, etc.) (Default=4): "
                                 + colorText.END
-                            )
+                            ) or "4"
                         )
                         return resp, maLength
                     except ValueError as e:  # pragma: no cover
                         default_logger().debug(e, exc_info=True)
                         OutputControls().printOutput(
                             colorText.BOLD
                             + colorText.FAIL
@@ -1415,34 +1419,34 @@
             tools.promptMenus(menu=menu)
             resp = int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + """[+] Select Option:"""
                     + colorText.END
-                )
+                ) or "3"
             )
             if resp == 1 or resp == 2:
                 candles = int(
                     input(
                         colorText.BOLD
                         + colorText.WARN
-                        + "\n[+] How many candles (TimeFrame) to look back Inside Bar formation? : "
+                        + "\n[+] How many candles (TimeFrame) to look back Inside Bar formation? (Default=3): "
                         + colorText.END
-                    )
+                    ) or "3"
                 )
                 return (resp, candles)
             if resp == 3:
                 percent = float(
                     input(
                         colorText.BOLD
                         + colorText.WARN
-                        + "\n[+] Enter Percentage within which all MA/EMAs should be (Ideal: 1-2%)? : "
+                        + "\n[+] Enter Percentage within which all MA/EMAs should be (Ideal: 1-2%)? (Default=2): "
                         + colorText.END
-                    )
+                    ) or "2"
                 )
                 return (resp, percent / 100.0)
             if resp >= 0 and resp <= 7:
                 return resp, 0
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
```

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/classes/keys.py` & `pkscreener-0.44.20240515.376/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/courbd.ttf` & `pkscreener-0.44.20240515.376/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/globals.py` & `pkscreener-0.44.20240515.376/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,16 +356,16 @@
             else:
                 daysForLowestVolume = int(options[3])
         else:
             daysForLowestVolume = int(
                 input(
                     colorText.BOLD
                     + colorText.WARN
-                    + "\n[+] The Volume should be lowest since last how many candles? "
-                )
+                    + "\n[+] The Volume should be lowest since last how many candles? (Default = 5)"
+                ) or "5"
             )
     except ValueError as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         OutputControls().printOutput(colorText.END)
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
@@ -392,27 +392,29 @@
             input("Press <Enter> to continue...")
     elif menuOption == "T":
         if userPassedArgs is None or userPassedArgs.options is None:
             selectedMenu = m0.find(menuOption)
             m1.renderForMenu(selectedMenu=selectedMenu)
             periodOption = input(
                     colorText.BOLD + colorText.FAIL + "[+] Select option: "
-                )
+                ) or ('L' if configManager.period == '280d' else 'S')
             OutputControls().printOutput(colorText.END, end="")
             if periodOption is None or periodOption.upper() not in ["L","S"]:
                 return
+            Utility.tools.clearScreen(forceTop=True)
             if periodOption.upper() in ["L","S"]:
                 selectedMenu = m1.find(periodOption)
                 m2.renderForMenu(selectedMenu=selectedMenu)
                 durationOption = input(
                         colorText.BOLD + colorText.FAIL + "[+] Select option: "
-                    )
+                    ) or "1"
                 OutputControls().printOutput(colorText.END, end="")
                 if durationOption is None or durationOption.upper() not in ["1","2","3","4","5"]:
                     return
+                Utility.tools.clearScreen(forceTop=True)
                 if durationOption.upper() in ["1","2","3","4"]:
                     selectedMenu = m2.find(durationOption)
                     periodDurations = selectedMenu.menuText.split("(")[1].split(")")[0].split(", ")
                     configManager.period = periodDurations[0]
                     configManager.duration = periodDurations[1]
                     configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
                 elif durationOption.upper() in ["5"]:
@@ -571,15 +573,15 @@
             selectedMenu = m1.find(indexOption)
             m2.renderForMenu(selectedMenu=selectedMenu, skip=skip)
     try:
         if indexOption is not None and indexOption != "W":
             if executeOption is None:
                 executeOption = input(
                     colorText.BOLD + colorText.FAIL + "[+] Select option: "
-                )
+                ) or "9"
                 OutputControls().printOutput(colorText.END, end="")
             if executeOption == "":
                 executeOption = 1
             if not str(executeOption).isnumeric():
                 executeOption = executeOption.upper()
             else:
                 executeOption = int(executeOption)
@@ -1195,14 +1197,24 @@
             maLength = 1 # By default buy option
         else:
             maLength = Utility.tools.promptSubMenuOptions(selectedMenu)
         if maLength == 0:
             return None, None
         else:
             selectedChoice["3"] = str(maLength)
+        if userPassedArgs.options is None:
+            Utility.tools.clearScreen(forceTop=True)
+            atrSensitivity = input(colorText.WARN + f"Enter the ATR Trailing Stop Sensitivity (Multiplier) value (Optimal:1, Current={configManager.atrTrailingStopSensitivity}):") or configManager.atrTrailingStopSensitivity
+            configManager.atrTrailingStopSensitivity = atrSensitivity
+            atrPeriod = input(colorText.WARN + f"Enter the ATR Period value (Optimal:10, Current={configManager.atrTrailingStopPeriod}):") or configManager.atrTrailingStopPeriod
+            configManager.atrTrailingStopPeriod = atrPeriod
+            atrEma = input(colorText.WARN + f"Enter the ATR EMA period (Optimal:200, Current={configManager.atrTrailingStopEMAPeriod}):") or configManager.atrTrailingStopEMAPeriod
+            configManager.atrTrailingStopEMAPeriod = atrEma
+            configManager.setConfig(ConfigManager.parser,default=True,showFileCreatedText=False)
+
     if executeOption == 42:
         Utility.tools.getLastScreenedResults(defaultAnswer)
         return None, None
     if executeOption >= MAX_SUPPORTED_MENU_OPTION and executeOption <= MAX_MENU_OPTION:
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
@@ -1221,15 +1233,15 @@
         try:
             if indexOption == "W":
                 listStockCodes = fetcher.fetchWatchlist()
                 if listStockCodes is None:
                     input(
                         colorText.BOLD
                         + colorText.FAIL
-                        + f"[+] Create the watchlist.xlsx file in {os.getcwd()} and Restart the Program!"
+                        + f"[+] Please create the watchlist.xlsx file in {os.getcwd()} and Restart the Program!"
                         + colorText.END
                     )
                     sys.exit(0)
             elif indexOption == "N":
                 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
                 prediction, pText, sText = screener.getNiftyPrediction(
                     df=fetcher.fetchLatestNiftyDaily(proxyServer=fetcher.proxyServer)
```

### Comparing `pkscreener-0.44.20240514.375/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240515.376/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240515.376/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240515.376/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240515.376/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.375
+Version: 0.44.20240515.376
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.375.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240515.376.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.375/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.375/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240515.376/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.375/setup.py` & `pkscreener-0.44.20240515.376/setup.py`

 * *Files identical despite different names*

