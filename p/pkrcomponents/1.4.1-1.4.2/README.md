# Comparing `tmp/pkrcomponents-1.4.1.tar.gz` & `tmp/pkrcomponents-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.4.1.tar", last modified: Wed May 15 11:01:57 2024, max compression
+gzip compressed data, was "pkrcomponents-1.4.2.tar", last modified: Wed May 15 11:41:21 2024, max compression
```

## Comparing `pkrcomponents-1.4.1.tar` & `pkrcomponents-1.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:57.718417 pkrcomponents-1.4.1/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:56.226594 pkrcomponents-1.4.1/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.4.1/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.4.1/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.4.1/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 11:01:57.701596 pkrcomponents-1.4.1/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.4.1/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:56.928886 pkrcomponents-1.4.1/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5128 2023-11-10 18:03:03.000000 pkrcomponents-1.4.1/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.4.1/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:56.972551 pkrcomponents-1.4.1/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:57.147903 pkrcomponents-1.4.1/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.4.1/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.4.1/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.4.1/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.4.1/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:57.352912 pkrcomponents-1.4.1/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.4.1/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.4.1/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.4.1/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:57.416856 pkrcomponents-1.4.1/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.4.1/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.4.1/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15211 2024-05-15 10:56:45.000000 pkrcomponents-1.4.1/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11773 2024-05-15 10:08:13.000000 pkrcomponents-1.4.1/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:56.024013 pkrcomponents-1.4.1/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:57.544971 pkrcomponents-1.4.1/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:57.629046 pkrcomponents-1.4.1/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.4.1/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.4.1/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.4.1/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.4.1/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:01:57.682557 pkrcomponents-1.4.1/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 11:01:54.000000 pkrcomponents-1.4.1/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.4.1/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 11:01:57.719429 pkrcomponents-1.4.1/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.4.1/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.339413 pkrcomponents-1.4.2/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.646407 pkrcomponents-1.4.2/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.4.2/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.4.2/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.4.2/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 11:41:21.331421 pkrcomponents-1.4.2/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.4.2/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/README.rst
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.931045 pkrcomponents-1.4.2/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5128 2023-11-10 18:03:03.000000 pkrcomponents-1.4.2/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.4.2/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.950082 pkrcomponents-1.4.2/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.023763 pkrcomponents-1.4.2/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.4.2/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.4.2/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.4.2/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.4.2/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.098874 pkrcomponents-1.4.2/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.4.2/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.4.2/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.4.2/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.130004 pkrcomponents-1.4.2/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.4.2/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.4.2/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15433 2024-05-15 11:39:12.000000 pkrcomponents-1.4.2/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11773 2024-05-15 10:08:13.000000 pkrcomponents-1.4.2/pkrcomponents/table_player.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.561475 pkrcomponents-1.4.2/pkrcomponents/tests/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.218811 pkrcomponents-1.4.2/pkrcomponents/tests/actions/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.269947 pkrcomponents-1.4.2/pkrcomponents/tests/actions/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.4.2/pkrcomponents/tests/actions/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.4.2/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.304414 pkrcomponents-1.4.2/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 11:41:19.000000 pkrcomponents-1.4.2/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 11:41:21.342414 pkrcomponents-1.4.2/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.4.2/setup.py
```

### Comparing `pkrcomponents-1.4.1/LICENSE.txt` & `pkrcomponents-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/MANIFEST.in` & `pkrcomponents-1.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/PKG-INFO` & `pkrcomponents-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.4.1/pkrcomponents/_common.py` & `pkrcomponents-1.4.2/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/action.py` & `pkrcomponents-1.4.2/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/bitcard.py` & `pkrcomponents-1.4.2/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/board.py` & `pkrcomponents-1.4.2/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/card.py` & `pkrcomponents-1.4.2/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/constants.py` & `pkrcomponents-1.4.2/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/evaluator.py` & `pkrcomponents-1.4.2/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/hand.py` & `pkrcomponents-1.4.2/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/listings.py` & `pkrcomponents-1.4.2/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/lookup_table.py` & `pkrcomponents-1.4.2/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.4.2/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.4.2/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/models/amount.py` & `pkrcomponents-1.4.2/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.4.2/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.4.2/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.4.2/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.4.2/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/players.py` & `pkrcomponents-1.4.2/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/pot.py` & `pkrcomponents-1.4.2/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/table.py` & `pkrcomponents-1.4.2/pkrcomponents/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,16 @@
     def street_ended(self):
         """Returns True if the street has ended"""
         # First case: there is no player left in waiting_list
         # Second case: there is only one player left in waiting_list that can still play and he has nothing to call
         return len(self.players_waiting) == 0 or (
                 self.nb_waiting == 1
                 and self.nb_in_game == 1
-                and self.players_waiting[0].to_call == 0) or (
+                and self.players_waiting[0].to_call == 0
+                and self.street != Street.SHOWDOWN) or (
                 self.street == Street.SHOWDOWN and len(self.unrevealed_players) == 0
         )
 
 
     @property
     def players_in_game(self):
         """Returns the list of players on the table that are still in the game (they can make an action)"""
@@ -170,14 +171,19 @@
 
     @property
     def next_street_ready(self):
         """Returns True if the next street is ready to be played"""
         return self.street_ended and not self.hand_ended
 
     @property
+    def next_hand_ready(self):
+        """Returns True if the next hand is ready to be played"""
+        return self.hand_ended and self.street_ended
+
+    @property
     def seats_playing(self):
         """Returns the list of seats of players waiting to play"""
         return [pl.seat for pl in self.players_waiting]
 
     @property
     def nb_waiting(self):
         """Returns the number of players waiting to play"""
```

### Comparing `pkrcomponents-1.4.1/pkrcomponents/table_player.py` & `pkrcomponents-1.4.2/pkrcomponents/table_player.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/tests/actions/test_move.py` & `pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/tests/actions/test_street.py` & `pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents/tournament.py` & `pkrcomponents-1.4.2/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.4.2/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.1/setup.py` & `pkrcomponents-1.4.2/setup.py`

 * *Files identical despite different names*

