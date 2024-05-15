# Comparing `tmp/pkrcomponents-1.5.0.tar.gz` & `tmp/pkrcomponents-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.5.0.tar", last modified: Wed May 15 13:01:58 2024, max compression
+gzip compressed data, was "pkrcomponents-1.5.1.tar", last modified: Wed May 15 16:09:02 2024, max compression
```

## Comparing `pkrcomponents-1.5.0.tar` & `pkrcomponents-1.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.418145 pkrcomponents-1.5.0/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:57.597410 pkrcomponents-1.5.0/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.5.0/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.5.0/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.5.0/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 13:01:58.413146 pkrcomponents-1.5.0/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.5.0/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:57.982489 pkrcomponents-1.5.0/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.5.0/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.5.0/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.016487 pkrcomponents-1.5.0/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.124479 pkrcomponents-1.5.0/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.5.0/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.5.0/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.5.0/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.5.0/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.233147 pkrcomponents-1.5.0/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.5.0/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.5.0/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.5.0/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.263364 pkrcomponents-1.5.0/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.5.0/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.5.0/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15520 2024-05-15 12:58:32.000000 pkrcomponents-1.5.0/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11948 2024-05-15 11:58:01.000000 pkrcomponents-1.5.0/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:57.491298 pkrcomponents-1.5.0/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.338900 pkrcomponents-1.5.0/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.376903 pkrcomponents-1.5.0/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.5.0/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.5.0/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.399150 pkrcomponents-1.5.0/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 13:01:56.000000 pkrcomponents-1.5.0/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 13:01:58.419148 pkrcomponents-1.5.0/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.5.0/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.917438 pkrcomponents-1.5.1/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:01.980407 pkrcomponents-1.5.1/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.5.1/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.5.1/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.5.1/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 16:09:02.911209 pkrcomponents-1.5.1/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.5.1/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/README.rst
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.417075 pkrcomponents-1.5.1/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.5.1/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.5.1/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.5.1/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.449868 pkrcomponents-1.5.1/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.557968 pkrcomponents-1.5.1/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.5.1/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.5.1/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.5.1/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.5.1/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.669863 pkrcomponents-1.5.1/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.5.1/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.5.1/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.5.1/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.706564 pkrcomponents-1.5.1/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.5.1/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.5.1/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.5.1/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15816 2024-05-15 15:52:00.000000 pkrcomponents-1.5.1/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11948 2024-05-15 11:58:01.000000 pkrcomponents-1.5.1/pkrcomponents/table_player.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:01.856114 pkrcomponents-1.5.1/pkrcomponents/tests/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.794202 pkrcomponents-1.5.1/pkrcomponents/tests/actions/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.863517 pkrcomponents-1.5.1/pkrcomponents/tests/actions/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.5.1/pkrcomponents/tests/actions/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.5.1/pkrcomponents/tests/actions/test_move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.5.1/pkrcomponents/tests/actions/test_street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.5.1/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 16:09:02.893137 pkrcomponents-1.5.1/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 16:09:00.000000 pkrcomponents-1.5.1/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.5.1/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 16:09:02.918432 pkrcomponents-1.5.1/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.5.1/setup.py
```

### Comparing `pkrcomponents-1.5.0/LICENSE.txt` & `pkrcomponents-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/MANIFEST.in` & `pkrcomponents-1.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/PKG-INFO` & `pkrcomponents-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.5.0/pkrcomponents/_common.py` & `pkrcomponents-1.5.1/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/action.py` & `pkrcomponents-1.5.1/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/bitcard.py` & `pkrcomponents-1.5.1/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/board.py` & `pkrcomponents-1.5.1/pkrcomponents/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,9 +129,16 @@
         """
         Boolean indicating if flop has a flushdraw
         """
         if len(self) < 3:
             return None
         return any(combo.first.suit == combo.second.suit for combo in self.flop_combinations)
 
+    def reset(self):
+        """
+        Reset the board
+        """
+        self.iloc[:] = np.nan
+
     def to_json(self):
         return self.astype(str).to_dict()
+
```

### Comparing `pkrcomponents-1.5.0/pkrcomponents/card.py` & `pkrcomponents-1.5.1/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/constants.py` & `pkrcomponents-1.5.1/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/evaluator.py` & `pkrcomponents-1.5.1/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/hand.py` & `pkrcomponents-1.5.1/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/listings.py` & `pkrcomponents-1.5.1/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/lookup_table.py` & `pkrcomponents-1.5.1/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.5.1/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.5.1/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/models/amount.py` & `pkrcomponents-1.5.1/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.5.1/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.5.1/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.5.1/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.5.1/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/players.py` & `pkrcomponents-1.5.1/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/pot.py` & `pkrcomponents-1.5.1/pkrcomponents/pot.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,7 +29,12 @@
         return self._highest_bet
 
     @highest_bet.setter
     def highest_bet(self, bet):
         """Setter for highest bet property"""
         self._highest_bet = bet
 
+    def reset(self):
+        """Reset the pot"""
+        self.value = 0
+        self.highest_bet = 0
+
```

### Comparing `pkrcomponents-1.5.0/pkrcomponents/table.py` & `pkrcomponents-1.5.1/pkrcomponents/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,7 +467,18 @@
         """Returns the preflop bet factors"""
         return self._preflop_bet_factors
 
     @property
     def postflop_bet_factors(self):
         """Returns the postflop bet factors"""
         return self._postflop_bet_factors
+
+    def advance_to_next_hand(self):
+        """Advance to the next hand"""
+        self.street = Street.PREFLOP
+        self.street_reset()
+        self.start_hand()
+        self.pot.reset()
+        self.board.reset()
+        self.deck.reset()
+        self._hand_has_started = False
+
```

### Comparing `pkrcomponents-1.5.0/pkrcomponents/table_player.py` & `pkrcomponents-1.5.1/pkrcomponents/table_player.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_move.py` & `pkrcomponents-1.5.1/pkrcomponents/tests/actions/test_move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_street.py` & `pkrcomponents-1.5.1/pkrcomponents/tests/actions/test_street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents/tournament.py` & `pkrcomponents-1.5.1/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.5.1/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.5.0/setup.py` & `pkrcomponents-1.5.1/setup.py`

 * *Files identical despite different names*

