# Comparing `tmp/pkrcomponents-1.4.2.tar.gz` & `tmp/pkrcomponents-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.4.2.tar", last modified: Wed May 15 11:41:21 2024, max compression
+gzip compressed data, was "pkrcomponents-1.5.0.tar", last modified: Wed May 15 13:01:58 2024, max compression
```

## Comparing `pkrcomponents-1.4.2.tar` & `pkrcomponents-1.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.339413 pkrcomponents-1.4.2/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.646407 pkrcomponents-1.4.2/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.4.2/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.4.2/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.4.2/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 11:41:21.331421 pkrcomponents-1.4.2/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.4.2/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.931045 pkrcomponents-1.4.2/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5128 2023-11-10 18:03:03.000000 pkrcomponents-1.4.2/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.4.2/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.950082 pkrcomponents-1.4.2/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.023763 pkrcomponents-1.4.2/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.4.2/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.4.2/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.4.2/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.4.2/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.098874 pkrcomponents-1.4.2/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.4.2/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.4.2/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.4.2/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.130004 pkrcomponents-1.4.2/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.4.2/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.4.2/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15433 2024-05-15 11:39:12.000000 pkrcomponents-1.4.2/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11773 2024-05-15 10:08:13.000000 pkrcomponents-1.4.2/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:20.561475 pkrcomponents-1.4.2/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.218811 pkrcomponents-1.4.2/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.269947 pkrcomponents-1.4.2/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.4.2/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.4.2/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 11:41:21.304414 pkrcomponents-1.4.2/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 11:41:19.000000 pkrcomponents-1.4.2/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.4.2/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 11:41:21.342414 pkrcomponents-1.4.2/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.4.2/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.418145 pkrcomponents-1.5.0/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:57.597410 pkrcomponents-1.5.0/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.5.0/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.5.0/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.5.0/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 13:01:58.413146 pkrcomponents-1.5.0/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.5.0/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/README.rst
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:57.982489 pkrcomponents-1.5.0/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.5.0/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.5.0/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.016487 pkrcomponents-1.5.0/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.124479 pkrcomponents-1.5.0/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.5.0/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.5.0/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.5.0/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.5.0/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.233147 pkrcomponents-1.5.0/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.5.0/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.5.0/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.5.0/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.263364 pkrcomponents-1.5.0/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.5.0/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4288 2024-05-15 10:53:41.000000 pkrcomponents-1.5.0/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15520 2024-05-15 12:58:32.000000 pkrcomponents-1.5.0/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11948 2024-05-15 11:58:01.000000 pkrcomponents-1.5.0/pkrcomponents/table_player.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:57.491298 pkrcomponents-1.5.0/pkrcomponents/tests/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.338900 pkrcomponents-1.5.0/pkrcomponents/tests/actions/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.376903 pkrcomponents-1.5.0/pkrcomponents/tests/actions/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.5.0/pkrcomponents/tests/actions/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.5.0/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 13:01:58.399150 pkrcomponents-1.5.0/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 13:01:56.000000 pkrcomponents-1.5.0/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.5.0/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 13:01:58.419148 pkrcomponents-1.5.0/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.5.0/setup.py
```

### Comparing `pkrcomponents-1.4.2/LICENSE.txt` & `pkrcomponents-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/MANIFEST.in` & `pkrcomponents-1.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/PKG-INFO` & `pkrcomponents-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.4.2
+Version: 1.5.0
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.4.2/pkrcomponents/_common.py` & `pkrcomponents-1.5.0/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/action.py` & `pkrcomponents-1.5.0/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/bitcard.py` & `pkrcomponents-1.5.0/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/board.py` & `pkrcomponents-1.5.0/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/card.py` & `pkrcomponents-1.5.0/pkrcomponents/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,21 @@
         if not cd:
             return self.cards.pop()
         else:
             cd = Card(cd)
             idx = self.cards.index(cd)
             return self.cards.pop(idx)
 
+    def replace(self, card):
+        """
+        Replaces a card in the deck
+        """
+        if card not in self.cards:
+            self.cards.append(card)
+
     @property
     def len(self):
         """
         Returns the number of cards currently in the deck
         """
         return self.__len__()
```

### Comparing `pkrcomponents-1.4.2/pkrcomponents/constants.py` & `pkrcomponents-1.5.0/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/evaluator.py` & `pkrcomponents-1.5.0/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/hand.py` & `pkrcomponents-1.5.0/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/listings.py` & `pkrcomponents-1.5.0/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/lookup_table.py` & `pkrcomponents-1.5.0/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.5.0/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.5.0/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/models/amount.py` & `pkrcomponents-1.5.0/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.5.0/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.5.0/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.5.0/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.5.0/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/players.py` & `pkrcomponents-1.5.0/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/pot.py` & `pkrcomponents-1.5.0/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/table.py` & `pkrcomponents-1.5.0/pkrcomponents/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,16 +414,18 @@
 
     @property
     def can_parse_winners(self) -> bool:
         """Returns True if the winners can be parsed"""
         return self.hand_ended and len(self.unrevealed_players) == 0
 
     @cached_property
-    def winners(self) -> dict[str, list]:
+    def winners(self) -> dict[int, list]:
         """Current status of winners with associated scores"""
+        if self.nb_involved == 1:
+            return {1: [self.players_involved[0]]}
         winners = {}
         for player in self.players_involved:
             pl_score = player.hand_score
             if not winners.get(pl_score):
                 winners[pl_score] = [player]
             else:
                 winners[pl_score].append(player)
```

### Comparing `pkrcomponents-1.4.2/pkrcomponents/table_player.py` & `pkrcomponents-1.5.0/pkrcomponents/table_player.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,20 @@
     def distribute(self, combo):
         """Distributes a combo to a player"""
         combo = Combo(combo)
         self.table.deck.draw(combo.first)
         self.table.deck.draw(combo.second)
         self.combo = combo
 
+    def delete_combo(self):
+        """Deletes a player's combo"""
+        for card in self.combo:
+            self.table.deck.replace(card)
+        self._combo = None
+
     def reset_street_status(self):
         """Reset street status"""
         self.played = False
         self.current_bet = 0
 
     @property
     def to_call(self):
```

### Comparing `pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_move.py` & `pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/tests/actions/test_street.py` & `pkrcomponents-1.5.0/pkrcomponents/tests/actions/test_street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents/tournament.py` & `pkrcomponents-1.5.0/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.5.0/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.4.2/setup.py` & `pkrcomponents-1.5.0/setup.py`

 * *Files identical despite different names*

