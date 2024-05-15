# Comparing `tmp/pkrcomponents-1.6.1.tar.gz` & `tmp/pkrcomponents-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.6.1.tar", last modified: Wed May 15 18:31:32 2024, max compression
+gzip compressed data, was "pkrcomponents-1.6.2.tar", last modified: Wed May 15 18:40:27 2024, max compression
```

## Comparing `pkrcomponents-1.6.1.tar` & `pkrcomponents-1.6.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:32.330683 pkrcomponents-1.6.1/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:31.608377 pkrcomponents-1.6.1/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.6.1/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.6.1/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.6.1/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 18:31:32.326684 pkrcomponents-1.6.1/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.6.1/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:31.947945 pkrcomponents-1.6.1/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.6.1/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.6.1/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.6.1/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:31.976662 pkrcomponents-1.6.1/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:32.103823 pkrcomponents-1.6.1/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.6.1/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.6.1/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.6.1/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.6.1/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:32.178579 pkrcomponents-1.6.1/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.6.1/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.6.1/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.6.1/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:32.202992 pkrcomponents-1.6.1/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.6.1/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.6.1/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.6.1/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15943 2024-05-15 18:17:46.000000 pkrcomponents-1.6.1/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12138 2024-05-15 18:29:12.000000 pkrcomponents-1.6.1/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:31.525530 pkrcomponents-1.6.1/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:32.258067 pkrcomponents-1.6.1/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:32.295014 pkrcomponents-1.6.1/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.6.1/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.6.1/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.6.1/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.6.1/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:31:32.308066 pkrcomponents-1.6.1/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 18:31:30.000000 pkrcomponents-1.6.1/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.6.1/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 18:31:32.331683 pkrcomponents-1.6.1/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.6.1/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.628937 pkrcomponents-1.6.2/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.000335 pkrcomponents-1.6.2/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.6.2/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.6.2/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.6.2/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 18:40:27.628937 pkrcomponents-1.6.2/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.6.2/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/README.rst
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.268528 pkrcomponents-1.6.2/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.6.2/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.6.2/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.6.2/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.299069 pkrcomponents-1.6.2/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.393963 pkrcomponents-1.6.2/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.6.2/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.6.2/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.6.2/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.6.2/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.502349 pkrcomponents-1.6.2/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.6.2/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.6.2/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.6.2/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.517975 pkrcomponents-1.6.2/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.6.2/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.6.2/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      999 2024-05-15 15:52:00.000000 pkrcomponents-1.6.2/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15943 2024-05-15 18:17:46.000000 pkrcomponents-1.6.2/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12178 2024-05-15 18:33:59.000000 pkrcomponents-1.6.2/pkrcomponents/table_player.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:26.936700 pkrcomponents-1.6.2/pkrcomponents/tests/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.565265 pkrcomponents-1.6.2/pkrcomponents/tests/actions/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.596525 pkrcomponents-1.6.2/pkrcomponents/tests/actions/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.6.2/pkrcomponents/tests/actions/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.6.2/pkrcomponents/tests/actions/test_move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.6.2/pkrcomponents/tests/actions/test_street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7577 2024-05-15 07:44:35.000000 pkrcomponents-1.6.2/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 18:40:27.612757 pkrcomponents-1.6.2/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 18:40:26.000000 pkrcomponents-1.6.2/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.6.2/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 18:40:27.628937 pkrcomponents-1.6.2/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.6.2/setup.py
```

### Comparing `pkrcomponents-1.6.1/LICENSE.txt` & `pkrcomponents-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/MANIFEST.in` & `pkrcomponents-1.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/PKG-INFO` & `pkrcomponents-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.6.1/pkrcomponents/_common.py` & `pkrcomponents-1.6.2/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/action.py` & `pkrcomponents-1.6.2/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/bitcard.py` & `pkrcomponents-1.6.2/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/board.py` & `pkrcomponents-1.6.2/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/card.py` & `pkrcomponents-1.6.2/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/constants.py` & `pkrcomponents-1.6.2/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/evaluator.py` & `pkrcomponents-1.6.2/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/hand.py` & `pkrcomponents-1.6.2/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/listings.py` & `pkrcomponents-1.6.2/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/lookup_table.py` & `pkrcomponents-1.6.2/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.6.2/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.6.2/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/models/amount.py` & `pkrcomponents-1.6.2/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.6.2/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.6.2/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.6.2/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.6.2/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/players.py` & `pkrcomponents-1.6.2/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/pot.py` & `pkrcomponents-1.6.2/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/table.py` & `pkrcomponents-1.6.2/pkrcomponents/table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/table_player.py` & `pkrcomponents-1.6.2/pkrcomponents/table_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,18 @@
         combo = Combo(combo)
         self.table.deck.draw(combo.first)
         self.table.deck.draw(combo.second)
         self.combo = combo
 
     def delete_combo(self):
         """Deletes a player's combo"""
-        self.table.deck.replace(self.combo.first)
-        self.table.deck.replace(self.combo.second)
-        self._combo = None
+        if self.has_combo:
+            self.table.deck.replace(self.combo.first)
+            self.table.deck.replace(self.combo.second)
+            self._combo = None
 
     def reset_street_status(self):
         """Reset street status"""
         self.played = False
         self.current_bet = 0
 
     def reset_hand_status(self):
```

### Comparing `pkrcomponents-1.6.1/pkrcomponents/tests/actions/test_move.py` & `pkrcomponents-1.6.2/pkrcomponents/tests/actions/test_move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/tests/actions/test_street.py` & `pkrcomponents-1.6.2/pkrcomponents/tests/actions/test_street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents/tournament.py` & `pkrcomponents-1.6.2/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.6.2/pkrcomponents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.6.1/setup.py` & `pkrcomponents-1.6.2/setup.py`

 * *Files identical despite different names*

