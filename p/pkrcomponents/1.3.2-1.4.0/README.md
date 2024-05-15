# Comparing `tmp/pkrcomponents-1.3.2.tar.gz` & `tmp/pkrcomponents-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.3.2.tar", last modified: Wed May 15 05:22:39 2024, max compression
+gzip compressed data, was "pkrcomponents-1.4.0.tar", last modified: Wed May 15 09:08:53 2024, max compression
```

## Comparing `pkrcomponents-1.3.2.tar` & `pkrcomponents-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.316573 pkrcomponents-1.3.2/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.553855 pkrcomponents-1.3.2/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.3.2/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.3.2/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.3.2/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 05:22:39.312296 pkrcomponents-1.3.2/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.3.2/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.898305 pkrcomponents-1.3.2/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5128 2023-11-10 18:03:03.000000 pkrcomponents-1.3.2/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.3.2/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.926643 pkrcomponents-1.3.2/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.011056 pkrcomponents-1.3.2/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.3.2/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.3.2/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.3.2/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.3.2/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.105564 pkrcomponents-1.3.2/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.3.2/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.3.2/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.3.2/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.137079 pkrcomponents-1.3.2/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.3.2/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4001 2024-05-14 19:44:00.000000 pkrcomponents-1.3.2/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15227 2024-05-14 19:01:45.000000 pkrcomponents-1.3.2/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11543 2024-05-15 05:20:34.000000 pkrcomponents-1.3.2/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.440049 pkrcomponents-1.3.2/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.251776 pkrcomponents-1.3.2/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.286743 pkrcomponents-1.3.2/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.3.2/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3427 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.301936 pkrcomponents-1.3.2/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 05:22:37.000000 pkrcomponents-1.3.2/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 05:22:39.316573 pkrcomponents-1.3.2/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.3.2/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.804547 pkrcomponents-1.4.0/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:52.680990 pkrcomponents-1.4.0/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.4.0/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.4.0/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.4.0/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 09:08:53.800432 pkrcomponents-1.4.0/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.4.0/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/README.rst
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.202799 pkrcomponents-1.4.0/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5128 2023-11-10 18:03:03.000000 pkrcomponents-1.4.0/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.4.0/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.237664 pkrcomponents-1.4.0/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.372729 pkrcomponents-1.4.0/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.4.0/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.4.0/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.4.0/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.4.0/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.538880 pkrcomponents-1.4.0/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.4.0/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.4.0/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.4.0/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.586402 pkrcomponents-1.4.0/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.4.0/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4001 2024-05-14 19:44:00.000000 pkrcomponents-1.4.0/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15227 2024-05-14 19:01:45.000000 pkrcomponents-1.4.0/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11543 2024-05-15 05:20:34.000000 pkrcomponents-1.4.0/pkrcomponents/table_player.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:52.582078 pkrcomponents-1.4.0/pkrcomponents/tests/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.715341 pkrcomponents-1.4.0/pkrcomponents/tests/actions/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.762432 pkrcomponents-1.4.0/pkrcomponents/tests/actions/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.4.0/pkrcomponents/tests/actions/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.4.0/pkrcomponents/tests/actions/test_move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.4.0/pkrcomponents/tests/actions/test_street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.4.0/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 09:08:53.788104 pkrcomponents-1.4.0/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 09:08:51.000000 pkrcomponents-1.4.0/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.4.0/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 09:08:53.805549 pkrcomponents-1.4.0/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.4.0/setup.py
```

### Comparing `pkrcomponents-1.3.2/LICENSE.txt` & `pkrcomponents-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/MANIFEST.in` & `pkrcomponents-1.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/PKG-INFO` & `pkrcomponents-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.3.2/pkrcomponents/_common.py` & `pkrcomponents-1.4.0/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/action.py` & `pkrcomponents-1.4.0/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/bitcard.py` & `pkrcomponents-1.4.0/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/board.py` & `pkrcomponents-1.4.0/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/card.py` & `pkrcomponents-1.4.0/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/constants.py` & `pkrcomponents-1.4.0/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/evaluator.py` & `pkrcomponents-1.4.0/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/hand.py` & `pkrcomponents-1.4.0/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/listings.py` & `pkrcomponents-1.4.0/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/lookup_table.py` & `pkrcomponents-1.4.0/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.4.0/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.4.0/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/models/amount.py` & `pkrcomponents-1.4.0/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.4.0/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.4.0/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.4.0/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.4.0/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/players.py` & `pkrcomponents-1.4.0/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/pot.py` & `pkrcomponents-1.4.0/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/table.py` & `pkrcomponents-1.4.0/pkrcomponents/table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/table_player.py` & `pkrcomponents-1.4.0/pkrcomponents/table_player.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_move.py` & `pkrcomponents-1.4.0/pkrcomponents/tests/actions/test_move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_street.py` & `pkrcomponents-1.4.0/pkrcomponents/tests/actions/test_street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.4.0/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.2/setup.py` & `pkrcomponents-1.4.0/setup.py`

 * *Files identical despite different names*

