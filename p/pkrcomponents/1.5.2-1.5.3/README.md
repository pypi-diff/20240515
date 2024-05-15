# Comparing `tmp/pkrcomponents-1.5.2.tar.gz` & `tmp/pkrcomponents-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.5.2.tar", last modified: Wed May 15 17:43:18 2024, max compression
+gzip compressed data, was "pkrcomponents-1.5.3.tar", last modified: Wed May 15 17:46:30 2024, max compression
```

## Comparing `pkrcomponents-1.5.2.tar` & `pkrcomponents-1.5.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.834325 pkrcomponents-1.5.2/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.111415 pkrcomponents-1.5.2/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.5.2/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.5.2/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.5.2/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 17:43:18.828359 pkrcomponents-1.5.2/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.5.2/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.456926 pkrcomponents-1.5.2/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.5.2/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.5.2/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.5.2/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.481958 pkrcomponents-1.5.2/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.566835 pkrcomponents-1.5.2/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.5.2/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.5.2/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.5.2/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.5.2/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.660044 pkrcomponents-1.5.2/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.5.2/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.5.2/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.5.2/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.684826 pkrcomponents-1.5.2/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.5.2/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.5.2/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.5.2/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15829 2024-05-15 17:40:32.000000 pkrcomponents-1.5.2/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11948 2024-05-15 11:58:01.000000 pkrcomponents-1.5.2/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:17.972182 pkrcomponents-1.5.2/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.750444 pkrcomponents-1.5.2/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.789740 pkrcomponents-1.5.2/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.5.2/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.5.2/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.5.2/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.5.2/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:43:18.810728 pkrcomponents-1.5.2/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 17:43:17.000000 pkrcomponents-1.5.2/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.5.2/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 17:43:18.836326 pkrcomponents-1.5.2/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.5.2/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.954321 pkrcomponents-1.5.3/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.313246 pkrcomponents-1.5.3/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.5.3/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.5.3/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.5.3/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 17:46:30.945300 pkrcomponents-1.5.3/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.5.3/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/README.rst
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.576536 pkrcomponents-1.5.3/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.5.3/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.5.3/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.5.3/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.598205 pkrcomponents-1.5.3/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.691407 pkrcomponents-1.5.3/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.5.3/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.5.3/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.5.3/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.5.3/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.782438 pkrcomponents-1.5.3/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.5.3/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.5.3/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.5.3/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.808530 pkrcomponents-1.5.3/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.5.3/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.5.3/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.5.3/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15829 2024-05-15 17:40:32.000000 pkrcomponents-1.5.3/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11977 2024-05-15 17:43:39.000000 pkrcomponents-1.5.3/pkrcomponents/table_player.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.241829 pkrcomponents-1.5.3/pkrcomponents/tests/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.873005 pkrcomponents-1.5.3/pkrcomponents/tests/actions/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.909074 pkrcomponents-1.5.3/pkrcomponents/tests/actions/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.5.3/pkrcomponents/tests/actions/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.5.3/pkrcomponents/tests/actions/test_move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.5.3/pkrcomponents/tests/actions/test_street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.5.3/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 17:46:30.932184 pkrcomponents-1.5.3/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 17:46:29.000000 pkrcomponents-1.5.3/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.5.3/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 17:46:30.955295 pkrcomponents-1.5.3/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.5.3/setup.py
```

### Comparing `pkrcomponents-1.5.2/LICENSE.txt` & `pkrcomponents-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/MANIFEST.in` & `pkrcomponents-1.5.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/PKG-INFO` & `pkrcomponents-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.5.2/pkrcomponents/_common.py` & `pkrcomponents-1.5.3/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/action.py` & `pkrcomponents-1.5.3/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/bitcard.py` & `pkrcomponents-1.5.3/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/board.py` & `pkrcomponents-1.5.3/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/card.py` & `pkrcomponents-1.5.3/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/constants.py` & `pkrcomponents-1.5.3/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/evaluator.py` & `pkrcomponents-1.5.3/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/hand.py` & `pkrcomponents-1.5.3/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/listings.py` & `pkrcomponents-1.5.3/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/lookup_table.py` & `pkrcomponents-1.5.3/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.5.3/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.5.3/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/models/amount.py` & `pkrcomponents-1.5.3/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.5.3/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.5.3/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.5.3/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.5.3/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/players.py` & `pkrcomponents-1.5.3/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/pot.py` & `pkrcomponents-1.5.3/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/table.py` & `pkrcomponents-1.5.3/pkrcomponents/table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/table_player.py` & `pkrcomponents-1.5.3/pkrcomponents/table_player.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         for card in self.combo:
             self.table.deck.replace(card)
         self._combo = None
 
     def reset_street_status(self):
         """Reset street status"""
         self.played = False
+        self.folded = False
         self.current_bet = 0
 
     @property
     def to_call(self):
         """float indicating the amount to call to continue on the table"""
         return min(self.table.pot.highest_bet-self.current_bet, self.stack)
```

### Comparing `pkrcomponents-1.5.2/pkrcomponents/tests/actions/test_move.py` & `pkrcomponents-1.5.3/pkrcomponents/tests/actions/test_move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/tests/actions/test_street.py` & `pkrcomponents-1.5.3/pkrcomponents/tests/actions/test_street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents/tournament.py` & `pkrcomponents-1.5.3/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.5.3/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.2/setup.py` & `pkrcomponents-1.5.3/setup.py`

 * *Files identical despite different names*

