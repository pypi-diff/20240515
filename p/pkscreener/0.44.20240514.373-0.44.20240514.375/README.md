# Comparing `tmp/pkscreener-0.44.20240514.373.tar.gz` & `tmp/pkscreener-0.44.20240514.375.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240514.373.tar", last modified: Tue May 14 12:14:53 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240514.375.tar", last modified: Tue May 14 19:09:24 2024, max compression
```

## Comparing `pkscreener-0.44.20240514.373.tar` & `pkscreener-0.44.20240514.375.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/
--rw-rw-rw-   0        0        0     1086 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.751484 pkscreener-0.44.20240514.373/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34197 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11409 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    40469 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12432 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   154876 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56135 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-14 12:14:43.000000 pkscreener-0.44.20240514.373/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   139167 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1024 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53036 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    31996 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-14 12:14:53.751484 pkscreener-0.44.20240514.373/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-14 12:14:53.000000 pkscreener-0.44.20240514.373/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-14 12:14:53.767097 pkscreener-0.44.20240514.373/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-14 12:09:44.000000 pkscreener-0.44.20240514.373/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/
+-rw-rw-rw-   0        0        0     1086 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.211229 pkscreener-0.44.20240514.375/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34202 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11409 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    40473 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12527 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   154876 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56135 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-14 19:09:15.000000 pkscreener-0.44.20240514.375/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   139571 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1041 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    53036 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    32153 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:09:24.211229 pkscreener-0.44.20240514.375/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-14 19:09:24.000000 pkscreener-0.44.20240514.375/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-14 19:09:24.226858 pkscreener-0.44.20240514.375/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-14 19:03:37.000000 pkscreener-0.44.20240514.375/setup.py
```

### Comparing `pkscreener-0.44.20240514.373/LICENSE` & `pkscreener-0.44.20240514.375/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/LICENSE-Others` & `pkscreener-0.44.20240514.375/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/PKG-INFO` & `pkscreener-0.44.20240514.375/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.373
+Version: 0.44.20240514.375
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.373.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.375.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.373/README.md` & `pkscreener-0.44.20240514.375/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener/__init__.py` & `pkscreener-0.44.20240514.375/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 3
         self.maxNumResultRowsInMonitor = 2
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:40:i 1m,X:12:27,X:12:28,X:12:23,X:12:7:3:.01:1,|{1}X:0:29:,|{3}X:0:31:,X:12:6:3,X:12:6:8,X:12:6:7:1,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m"
+        self.defaultMonitorOptions = "X:12:9:2.5,|X:0:5:0:40:i 1m,|{1}X:12:27:,X:12:28,X:12:23,|{3}X:0:31:,X:12:7:3:.01:1,|{1}X:0:29:,X:12:6:3,X:12:6:8,X:12:6:7:1,X:12:6:9,X:12:6:10:1,X:12:7:3:.02:1,X:12:7:6:1,X:12:17,X:12:2,X:12:24,X:12:12:i 5m,X:12:13:i 1m"
         self.minimumChangePercentage = 0
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,16 @@
     "M": "Back to the Top/Main menu",
 }
 PIPED_SCANNERS = {"1": "-a y -e -o 'X:12:9:2.5:;|X:0:31:;|X:0:27:'",
                   "2": "-a y -e -o 'X:12:9:2.5:;|X:0:31:'",
                   "3": "-a y -e -o 'X:12:9:2.5:;|X:0:27:'",
                   "4": "-a y -e -o 'X:12:9:2.5:;|X:0:29:'",
                   "5": "-a y -e -o 'X:12:31:;|X:0:27:'",
-                  "6": "-a y -e -o 'X:12:31:;|X:0:30:'",
-                  "7": "-a y -e -o 'X:12:27:;|X:0:30:'",
+                  "6": "-a y -e -o 'X:12:31:;|X:0:30:1:'",
+                  "7": "-a y -e -o 'X:12:27:;|X:0:30:1:'",
                   }
 
 level1_T_MenuDict = {
     "L": "Long Term",
     "S": "Short Term (Intraday)",
     "M": "Back to the Top/Main menu",
 }
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/OtaUpdater.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,25 +156,27 @@
             size = int(resp.json()["assets"][0]["size"] / (1024 * 1024))
         return resp, size
 
     # Check for update and download if available
     def checkForUpdate(VERSION=VERSION, skipDownload=False):
         OTAUpdater.checkForUpdate.url = None
         resp = None
+        updateType = "minor"
         try:
             now_components = str(VERSION).split(".")
             now_major_minor = ".".join([now_components[0], now_components[1]])
             now = float(now_major_minor)
             resp, size = OTAUpdater.get_latest_release_info()
             tag = resp.json()["tag_name"]
             version_components = tag.split(".")
             major_minor = ".".join([version_components[0], version_components[1]])
             last_release = float(major_minor)
             prod_update = False
             if last_release > now:
+                updateType = "major"
                 prod_update = True
             elif last_release == now and (
                 len(now_components) < len(version_components)
             ):
                 # Must be the weekly update over the last major.minor update
                 prod_update = True
             elif last_release == now and (
@@ -186,15 +188,15 @@
                     if float(now_components[3]) < float(version_components[3]):
                         prod_update = True
             if prod_update:
                 if skipDownload:
                     OutputControls().printOutput(
                         colorText.BOLD
                         + colorText.GREEN
-                        + f"    [+] A software update (v{tag} [{size} MB]) is available. Check out with the menu option U."
+                        + f"    [+] A {updateType} software update (v{tag} [{size} MB]) is available. Check out with the menu option U."
                         + colorText.END
                     )
                     return
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
                     + "[+] What's New in this Update?\n"
@@ -204,15 +206,15 @@
                     + colorText.END
                 )
                 try:
                     action = input(
                             colorText.BOLD
                             + colorText.FAIL
                             + (
-                                "\n[+] New Software update (v%s) available. Download Now (Size: %dMB)? [Y/N]: "
+                                f"\n[+] New {updateType} Software update (v%s) available. Download Now (Size: %dMB)? [Y/N]: "
                                 % (str(tag), size)
                             )
                         )
                 except EOFError: # user pressed enter
                     action = "y"
                     pass
                 if action is not None and action.lower() == "y":
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/classes/keys.py` & `pkscreener-0.44.20240514.375/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/courbd.ttf` & `pkscreener-0.44.20240514.375/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/globals.py` & `pkscreener-0.44.20240514.375/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -774,27 +774,30 @@
             os.system(f"{launcher} -a Y -e -d -i 1m")
         elif menuOption in ["L"]:
             OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener to collect logs. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -l{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
             sleep(2)
             os.system(f"{launcher} -a Y -l")
         sys.exit(0)
     if menuOption in ["P"]:
+        Utility.tools.clearScreen(forceTop=True)
         selectedMenu = m0.find(menuOption)
         m1.renderForMenu(selectedMenu)
         predefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
         OutputControls().printOutput(colorText.END, end="")
         if predefinedOption not in ["1","2"]:
             return None, None
         if predefinedOption == "1":
+            Utility.tools.clearScreen(forceTop=True)
             selectedMenu = m1.find(predefinedOption)
             m2.renderForMenu(selectedMenu=selectedMenu)
             selPredefinedOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ") or "1"
             OutputControls().printOutput(colorText.END, end="")
             if selPredefinedOption in ["1","2","3","4","5","6","7"]:
                 scannerOption = PIPED_SCANNERS[selPredefinedOption]
+                Utility.tools.clearScreen(forceTop=True)
                 if userPassedArgs.pipedmenus is not None:
                     chosenOptions = scannerOption.split("-o ")[1]
                     userPassedArgs.options = chosenOptions.replace("'","")
                     return addOrRunPipedMenus()
                 launcher = sys.argv[0]
                 launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
                 OutputControls().printOutput(f"{colorText.GREEN}Launching PKScreener with piped scanners. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} {scannerOption}{colorText.END}")
@@ -1182,14 +1185,16 @@
     if executeOption == 30:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 4:
             if str(options[3]).isnumeric():
                 maLength = int(options[3])
             elif str(options[3]).upper() == "D":
                 maLength = 1
+            else:
+                maLength = 1
         elif len(options) >= 3:
             maLength = 1 # By default buy option
         else:
             maLength = Utility.tools.promptSubMenuOptions(selectedMenu)
         if maLength == 0:
             return None, None
         else:
@@ -1518,15 +1523,17 @@
             if optionalFinalOutcome_df is None:
                 optionalFinalOutcome_df = analysis_df
             else:
                 optionalFinalOutcome_df = pd.concat([optionalFinalOutcome_df, analysis_df], axis=0)
             return optionalFinalOutcome_df, saveResults
         else:
             existingTitle = f"{userPassedArgs.pipedtitle}|" if userPassedArgs.pipedtitle is not None else ""
-            userPassedArgs.pipedtitle = f'{existingTitle}{menuChoiceHierarchy.split(">")[-1]}'
+            choiceSegments = menuChoiceHierarchy.split(">")
+            choiceSegments = f"{choiceSegments[-2]} > {choiceSegments[-1]}" if len(choiceSegments)>=4 else f"{choiceSegments[-1]}"
+            userPassedArgs.pipedtitle = f'{existingTitle}{choiceSegments}[{len(saveResults)}]'
             return screenResults, saveResults
 
 def loadDatabaseOrFetch(downloadOnly, listStockCodes, menuOption, indexOption):
     global stockDictPrimary,stockDictSecondary, configManager, defaultAnswer, userPassedArgs, loadedStockData
     if menuOption not in ["C"]:
         stockDictPrimary = Utility.tools.loadStockData(
                     stockDictPrimary,
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240514.375/pkscreener/pkscreener.ini`

 * *Files 12% similar despite different names*

```diff
@@ -12,53 +12,55 @@
 000000b0: 6174 6572 7369 696e 7472 6164 6179 203d  atersiintraday =
 000000c0: 206e 0d0a 6461 7973 746f 6c6f 6f6b 6261   n..daystolookba
 000000d0: 636b 203d 2032 320d 0a64 6566 6175 6c74  ck = 22..default
 000000e0: 696e 6465 7820 3d20 3132 0d0a 6465 6661  index = 12..defa
 000000f0: 756c 746d 6f6e 6974 6f72 6f70 7469 6f6e  ultmonitoroption
 00000100: 7320 3d20 583a 3132 3a39 3a32 2e35 2c7c  s = X:12:9:2.5,|
 00000110: 583a 303a 353a 303a 3430 3a69 2031 6d2c  X:0:5:0:40:i 1m,
-00000120: 583a 3132 3a32 372c 583a 3132 3a32 382c  X:12:27,X:12:28,
-00000130: 583a 3132 3a32 332c 583a 3132 3a37 3a33  X:12:23,X:12:7:3
-00000140: 3a2e 3031 3a31 2c7c 7b31 7d58 3a30 3a32  :.01:1,|{1}X:0:2
-00000150: 393a 2c58 3a31 323a 363a 332c 583a 3132  9:,X:12:6:3,X:12
-00000160: 3a36 3a38 2c58 3a31 323a 363a 373a 312c  :6:8,X:12:6:7:1,
-00000170: 583a 3132 3a36 3a39 2c58 3a31 323a 363a  X:12:6:9,X:12:6:
-00000180: 3130 3a31 2c58 3a31 323a 373a 333a 2e30  10:1,X:12:7:3:.0
-00000190: 323a 312c 583a 3132 3a37 3a36 3a31 2c58  2:1,X:12:7:6:1,X
-000001a0: 3a31 323a 3137 2c58 3a31 323a 322c 583a  :12:17,X:12:2,X:
-000001b0: 3132 3a32 342c 583a 3132 3a31 323a 6920  12:24,X:12:12:i 
-000001c0: 356d 2c58 3a31 323a 3133 3a69 2031 6d0d  5m,X:12:13:i 1m.
-000001d0: 0a64 7572 6174 696f 6e20 3d20 3164 0d0a  .duration = 1d..
-000001e0: 656e 6162 6c65 706f 7274 666f 6c69 6f63  enableportfolioc
-000001f0: 616c 6375 6c61 7469 6f6e 7320 3d20 6e0d  alculations = n.
-00000200: 0a67 656e 6572 616c 7469 6d65 6f75 7420  .generaltimeout 
-00000210: 3d20 322e 300d 0a6c 6f67 7365 6e61 626c  = 2.0..logsenabl
-00000220: 6564 203d 206e 0d0a 6c6f 6e67 7469 6d65  ed = n..longtime
-00000230: 6f75 7420 3d20 342e 300d 0a6d 6178 6261  out = 4.0..maxba
-00000240: 636b 7465 7374 7769 6e64 6f77 203d 2033  cktestwindow = 3
-00000250: 300d 0a6d 6178 6461 7368 626f 6172 6477  0..maxdashboardw
-00000260: 6964 6765 7473 7065 7272 6f77 203d 2033  idgetsperrow = 3
-00000270: 0d0a 6d61 786e 6574 776f 726b 7265 7472  ..maxnetworkretr
-00000280: 7963 6f75 6e74 203d 2031 300d 0a6d 6178  ycount = 10..max
-00000290: 6e75 6d72 6573 756c 7472 6f77 7369 6e6d  numresultrowsinm
-000002a0: 6f6e 6974 6f72 203d 2032 0d0a 6d6f 726e  onitor = 2..morn
-000002b0: 696e 6761 6e61 6c79 7369 7363 616e 646c  inganalysiscandl
-000002c0: 656e 756d 6265 7220 3d20 3235 0d0a 6d6f  enumber = 25..mo
-000002d0: 726e 696e 6761 6e61 6c79 7369 7363 616e  rninganalysiscan
-000002e0: 646c 6564 7572 6174 696f 6e20 3d20 316d  dleduration = 1m
-000002f0: 0d0a 6f6e 6c79 7374 6167 6574 776f 7374  ..onlystagetwost
-00000300: 6f63 6b73 203d 2079 0d0a 7065 7269 6f64  ocks = y..period
-00000310: 203d 2032 3830 640d 0a73 686f 7770 6173   = 280d..showpas
-00000320: 7473 7472 6174 6567 7964 6174 6120 3d20  tstrategydata = 
-00000330: 6e0d 0a73 686f 7775 6e6b 6e6f 776e 7472  n..showunknowntr
-00000340: 656e 6473 203d 2079 0d0a 7368 7566 666c  ends = y..shuffl
-00000350: 6520 3d20 790d 0a75 7365 656d 6120 3d20  e = y..useema = 
-00000360: 6e0d 0a0d 0a5b 6669 6c74 6572 735d 0d0a  n....[filters]..
-00000370: 636f 6e73 6f6c 6964 6174 696f 6e70 6572  consolidationper
-00000380: 6365 6e74 6167 6520 3d20 3130 2e30 0d0a  centage = 10.0..
-00000390: 6d61 7870 7269 6365 203d 2035 3030 3030  maxprice = 50000
-000003a0: 2e30 0d0a 6d69 6e69 6d75 6d63 6861 6e67  .0..minimumchang
-000003b0: 6570 6572 6365 6e74 6167 6520 3d20 302e  epercentage = 0.
-000003c0: 300d 0a6d 696e 696d 756d 766f 6c75 6d65  0..minimumvolume
-000003d0: 203d 2031 3030 3030 0d0a 6d69 6e70 7269   = 10000..minpri
-000003e0: 6365 203d 2032 302e 300d 0a76 6f6c 756d  ce = 20.0..volum
-000003f0: 6572 6174 696f 203d 2032 2e35 0d0a 0d0a  eratio = 2.5....
+00000120: 7c7b 317d 583a 3132 3a32 373a 2c58 3a31  |{1}X:12:27:,X:1
+00000130: 323a 3238 2c58 3a31 323a 3233 2c7c 7b33  2:28,X:12:23,|{3
+00000140: 7d58 3a30 3a33 313a 2c58 3a31 323a 373a  }X:0:31:,X:12:7:
+00000150: 333a 2e30 313a 312c 7c7b 317d 583a 303a  3:.01:1,|{1}X:0:
+00000160: 3239 3a2c 583a 3132 3a36 3a33 2c58 3a31  29:,X:12:6:3,X:1
+00000170: 323a 363a 382c 583a 3132 3a36 3a37 3a31  2:6:8,X:12:6:7:1
+00000180: 2c58 3a31 323a 363a 392c 583a 3132 3a36  ,X:12:6:9,X:12:6
+00000190: 3a31 303a 312c 583a 3132 3a37 3a33 3a2e  :10:1,X:12:7:3:.
+000001a0: 3032 3a31 2c58 3a31 323a 373a 363a 312c  02:1,X:12:7:6:1,
+000001b0: 583a 3132 3a31 372c 583a 3132 3a32 2c58  X:12:17,X:12:2,X
+000001c0: 3a31 323a 3234 2c58 3a31 323a 3132 3a69  :12:24,X:12:12:i
+000001d0: 2035 6d2c 583a 3132 3a31 333a 6920 316d   5m,X:12:13:i 1m
+000001e0: 0d0a 6475 7261 7469 6f6e 203d 2031 640d  ..duration = 1d.
+000001f0: 0a65 6e61 626c 6570 6f72 7466 6f6c 696f  .enableportfolio
+00000200: 6361 6c63 756c 6174 696f 6e73 203d 206e  calculations = n
+00000210: 0d0a 6765 6e65 7261 6c74 696d 656f 7574  ..generaltimeout
+00000220: 203d 2032 2e30 0d0a 6c6f 6773 656e 6162   = 2.0..logsenab
+00000230: 6c65 6420 3d20 6e0d 0a6c 6f6e 6774 696d  led = n..longtim
+00000240: 656f 7574 203d 2034 2e30 0d0a 6d61 7862  eout = 4.0..maxb
+00000250: 6163 6b74 6573 7477 696e 646f 7720 3d20  acktestwindow = 
+00000260: 3330 0d0a 6d61 7864 6173 6862 6f61 7264  30..maxdashboard
+00000270: 7769 6467 6574 7370 6572 726f 7720 3d20  widgetsperrow = 
+00000280: 330d 0a6d 6178 6e65 7477 6f72 6b72 6574  3..maxnetworkret
+00000290: 7279 636f 756e 7420 3d20 3130 0d0a 6d61  rycount = 10..ma
+000002a0: 786e 756d 7265 7375 6c74 726f 7773 696e  xnumresultrowsin
+000002b0: 6d6f 6e69 746f 7220 3d20 320d 0a6d 6f72  monitor = 2..mor
+000002c0: 6e69 6e67 616e 616c 7973 6973 6361 6e64  ninganalysiscand
+000002d0: 6c65 6e75 6d62 6572 203d 2032 350d 0a6d  lenumber = 25..m
+000002e0: 6f72 6e69 6e67 616e 616c 7973 6973 6361  orninganalysisca
+000002f0: 6e64 6c65 6475 7261 7469 6f6e 203d 2031  ndleduration = 1
+00000300: 6d0d 0a6f 6e6c 7973 7461 6765 7477 6f73  m..onlystagetwos
+00000310: 746f 636b 7320 3d20 790d 0a70 6572 696f  tocks = y..perio
+00000320: 6420 3d20 3238 3064 0d0a 7368 6f77 7061  d = 280d..showpa
+00000330: 7374 7374 7261 7465 6779 6461 7461 203d  ststrategydata =
+00000340: 206e 0d0a 7368 6f77 756e 6b6e 6f77 6e74   n..showunknownt
+00000350: 7265 6e64 7320 3d20 790d 0a73 6875 6666  rends = y..shuff
+00000360: 6c65 203d 2079 0d0a 7573 6565 6d61 203d  le = y..useema =
+00000370: 206e 0d0a 0d0a 5b66 696c 7465 7273 5d0d   n....[filters].
+00000380: 0a63 6f6e 736f 6c69 6461 7469 6f6e 7065  .consolidationpe
+00000390: 7263 656e 7461 6765 203d 2031 302e 300d  rcentage = 10.0.
+000003a0: 0a6d 6178 7072 6963 6520 3d20 3530 3030  .maxprice = 5000
+000003b0: 302e 300d 0a6d 696e 696d 756d 6368 616e  0.0..minimumchan
+000003c0: 6765 7065 7263 656e 7461 6765 203d 2030  gepercentage = 0
+000003d0: 2e30 0d0a 6d69 6e69 6d75 6d76 6f6c 756d  .0..minimumvolum
+000003e0: 6520 3d20 3130 3030 300d 0a6d 696e 7072  e = 10000..minpr
+000003f0: 6963 6520 3d20 3230 2e30 0d0a 766f 6c75  ice = 20.0..volu
+00000400: 6d65 7261 7469 6f20 3d20 322e 350d 0a0d  meratio = 2.5...
+00000410: 0a                                       .
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240514.375/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240514.375/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,21 +475,22 @@
                     sys.exit(0)
                 runPipedScans = True
                 while runPipedScans:
                     runPipedScans = pipeResults(plainResults,args)
                     if runPipedScans:
                         results, plainResults = main(userArgs=args)
                     else:
-                        OutputControls().printOutput(
-                                colorText.GREEN
-                                + f"[+] Finished running all piped scanners! Try reducing number of piped scans if no stocks could be found eventually."
-                                + colorText.END
-                            )
-                        if args.answerdefault is None:
-                            input("Press <Enter> to continue...")
+                        if args is not None and args.pipedtitle is not None and "|" in args.pipedtitle:
+                            OutputControls().printOutput(
+                                    colorText.WARN
+                                    + f"[+] Pipe Results Found: {args.pipedtitle}. {'Reduce number of piped scans if no stocks could be found.' if '[0]' in args.pipedtitle else ''}"
+                                    + colorText.END
+                                )
+                            if args.answerdefault is None:
+                                input("Press <Enter> to continue...")
             except SystemExit:
                 closeWorkersAndExit()
                 removeMonitorFile()
                 sys.exit(0)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240514.375/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240514.373
+Version: 0.44.20240514.375
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.373.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240514.375.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.372/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240514.374/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240514.373/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240514.375/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240514.373/setup.py` & `pkscreener-0.44.20240514.375/setup.py`

 * *Files identical despite different names*

