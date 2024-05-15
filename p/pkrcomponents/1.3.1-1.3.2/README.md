# Comparing `tmp/pkrcomponents-1.3.1.tar.gz` & `tmp/pkrcomponents-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.3.1.tar", last modified: Tue May 14 20:20:50 2024, max compression
+gzip compressed data, was "pkrcomponents-1.3.2.tar", last modified: Wed May 15 05:22:39 2024, max compression
```

## Comparing `pkrcomponents-1.3.1.tar` & `pkrcomponents-1.3.2.tar`

### file list

```diff
@@ -1,92 +1,48 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.406609 pkrcomponents-1.3.1/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.011754 pkrcomponents-1.3.1/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.3.1/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.3.1/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       42 2024-05-14 20:14:27.000000 pkrcomponents-1.3.1/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-14 20:20:50.402598 pkrcomponents-1.3.1/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.3.1/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/README.rst
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:48.848450 pkrcomponents-1.3.1/Tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:48.912127 pkrcomponents-1.3.1/Tests/pkrcomponents/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.071510 pkrcomponents-1.3.1/Tests/pkrcomponents/_common/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      338 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/_common/test_common.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.095192 pkrcomponents-1.3.1/Tests/pkrcomponents/action/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2140 2023-09-25 10:39:52.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/action/test_action.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.133645 pkrcomponents-1.3.1/Tests/pkrcomponents/bitcard/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1388 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/bitcard/test_bitcard.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.188579 pkrcomponents-1.3.1/Tests/pkrcomponents/board/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6309 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/board/test_board.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.350117 pkrcomponents-1.3.1/Tests/pkrcomponents/card/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2017 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/card/test_card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1455 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/card/test_deck.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2995 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/card/test_rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1285 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/card/test_suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.391474 pkrcomponents-1.3.1/Tests/pkrcomponents/constants/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      555 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/constants/test_constants.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.431206 pkrcomponents-1.3.1/Tests/pkrcomponents/evaluator/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1649 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/evaluator/test_evaluator.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.516814 pkrcomponents-1.3.1/Tests/pkrcomponents/hand/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6271 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/hand/test_combo.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      250 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/hand/test_combo_range.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1041 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/hand/test_general.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     6753 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/hand/test_hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      808 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/hand/test_shape.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.531814 pkrcomponents-1.3.1/Tests/pkrcomponents/listings/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      659 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/listings/test_listings.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.549853 pkrcomponents-1.3.1/Tests/pkrcomponents/lookup_table/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      290 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/lookup_table/test_lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.566372 pkrcomponents-1.3.1/Tests/pkrcomponents/players/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2962 2024-05-08 12:10:46.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/players/test_players.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.583371 pkrcomponents-1.3.1/Tests/pkrcomponents/pot/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      513 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/pot/test_pot.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.598863 pkrcomponents-1.3.1/Tests/pkrcomponents/table/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    12988 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/table/test_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.616864 pkrcomponents-1.3.1/Tests/pkrcomponents/table_player/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4222 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/table_player/test_table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:49.650733 pkrcomponents-1.3.1/Tests/pkrcomponents/tournament/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1787 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/tournament/test_level.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2322 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/Tests/pkrcomponents/tournament/test_tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.002595 pkrcomponents-1.3.1/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5128 2023-11-10 18:03:03.000000 pkrcomponents-1.3.1/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.3.1/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.093318 pkrcomponents-1.3.1/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.167839 pkrcomponents-1.3.1/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.3.1/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.3.1/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.3.1/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.3.1/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.249671 pkrcomponents-1.3.1/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.3.1/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.3.1/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.3.1/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.272693 pkrcomponents-1.3.1/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.3.1/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4001 2024-05-14 19:44:00.000000 pkrcomponents-1.3.1/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15227 2024-05-14 19:01:45.000000 pkrcomponents-1.3.1/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11924 2024-05-14 19:44:00.000000 pkrcomponents-1.3.1/pkrcomponents/table_player.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:48.933139 pkrcomponents-1.3.1/pkrcomponents/tests/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.341758 pkrcomponents-1.3.1/pkrcomponents/tests/actions/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.377589 pkrcomponents-1.3.1/pkrcomponents/tests/actions/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.3.1/pkrcomponents/tests/actions/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.3.1/pkrcomponents/tests/actions/test_move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.3.1/pkrcomponents/tests/actions/test_street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3427 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-14 20:20:50.079057 pkrcomponents-1.3.1/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-14 20:19:24.000000 pkrcomponents-1.3.1/pkrcomponents.egg-info/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2092 2024-05-14 20:20:48.000000 pkrcomponents-1.3.1/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        1 2024-05-14 20:19:24.000000 pkrcomponents-1.3.1/pkrcomponents.egg-info/dependency_links.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       70 2024-05-14 20:19:24.000000 pkrcomponents-1.3.1/pkrcomponents.egg-info/requires.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       14 2024-05-14 20:19:24.000000 pkrcomponents-1.3.1/pkrcomponents.egg-info/top_level.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.3.1/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-14 20:20:50.407617 pkrcomponents-1.3.1/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.3.1/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.316573 pkrcomponents-1.3.2/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.553855 pkrcomponents-1.3.2/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.3.2/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.3.2/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-14 20:27:30.000000 pkrcomponents-1.3.2/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      704 2024-05-15 05:22:39.312296 pkrcomponents-1.3.2/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-04-16 08:43:13.000000 pkrcomponents-1.3.2/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/README.rst
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.898305 pkrcomponents-1.3.2/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1507 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7279 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3840 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5128 2023-11-10 18:03:03.000000 pkrcomponents-1.3.2/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3435 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13029 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1374 2024-05-10 23:42:15.000000 pkrcomponents-1.3.2/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/lookup_table.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.926643 pkrcomponents-1.3.2/pkrcomponents/models/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.011056 pkrcomponents-1.3.2/pkrcomponents/models/actions/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.3.2/pkrcomponents/models/actions/move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.3.2/pkrcomponents/models/actions/sequence.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.3.2/pkrcomponents/models/actions/street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.3.2/pkrcomponents/models/amount.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.105564 pkrcomponents-1.3.2/pkrcomponents/models/cards/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.3.2/pkrcomponents/models/cards/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.3.2/pkrcomponents/models/cards/rank.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.3.2/pkrcomponents/models/cards/suit.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.137079 pkrcomponents-1.3.2/pkrcomponents/models/pots/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.3.2/pkrcomponents/models/pots/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4001 2024-05-14 19:44:00.000000 pkrcomponents-1.3.2/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      892 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    15227 2024-05-14 19:01:45.000000 pkrcomponents-1.3.2/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    11543 2024-05-15 05:20:34.000000 pkrcomponents-1.3.2/pkrcomponents/table_player.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:38.440049 pkrcomponents-1.3.2/pkrcomponents/tests/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.251776 pkrcomponents-1.3.2/pkrcomponents/tests/actions/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.286743 pkrcomponents-1.3.2/pkrcomponents/tests/actions/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2023-11-10 19:00:33.000000 pkrcomponents-1.3.2/pkrcomponents/tests/actions/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3185 2023-11-10 19:03:11.000000 pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_move.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1970 2023-11-10 19:18:13.000000 pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_street.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3427 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-15 05:22:39.301936 pkrcomponents-1.3.2/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      920 2024-05-15 05:22:37.000000 pkrcomponents-1.3.2/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.3.2/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-15 05:22:39.316573 pkrcomponents-1.3.2/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1334 2024-05-12 18:14:33.000000 pkrcomponents-1.3.2/setup.py
```

### Comparing `pkrcomponents-1.3.1/LICENSE.txt` & `pkrcomponents-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/PKG-INFO` & `pkrcomponents-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.3.1/pkrcomponents/_common.py` & `pkrcomponents-1.3.2/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/action.py` & `pkrcomponents-1.3.2/pkrcomponents/action.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/bitcard.py` & `pkrcomponents-1.3.2/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/board.py` & `pkrcomponents-1.3.2/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/card.py` & `pkrcomponents-1.3.2/pkrcomponents/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/constants.py` & `pkrcomponents-1.3.2/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/evaluator.py` & `pkrcomponents-1.3.2/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/hand.py` & `pkrcomponents-1.3.2/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/listings.py` & `pkrcomponents-1.3.2/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/lookup_table.py` & `pkrcomponents-1.3.2/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/models/actions/move.py` & `pkrcomponents-1.3.2/pkrcomponents/models/actions/move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/models/actions/street.py` & `pkrcomponents-1.3.2/pkrcomponents/models/actions/street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/models/amount.py` & `pkrcomponents-1.3.2/pkrcomponents/models/amount.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/models/cards/card.py` & `pkrcomponents-1.3.2/pkrcomponents/models/cards/card.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/models/cards/rank.py` & `pkrcomponents-1.3.2/pkrcomponents/models/cards/rank.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.3.2/pkrcomponents/models/cards/suit.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/models/pots/pot.py` & `pkrcomponents-1.3.2/pkrcomponents/models/pots/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/players.py` & `pkrcomponents-1.3.2/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/pot.py` & `pkrcomponents-1.3.2/pkrcomponents/pot.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/table.py` & `pkrcomponents-1.3.2/pkrcomponents/table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/table_player.py` & `pkrcomponents-1.3.2/pkrcomponents/table_player.py`

 * *Files 7% similar despite different names*

```diff
@@ -255,38 +255,30 @@
 
     def pay(self, value):
         """Action of paying a value"""
         amount = self.max_bet(value)
         self.stack -= amount
         self.table.pot.add(amount)
 
-    # def do_bet(self, value):
-    #     """Action of betting a certain value"""
-    #     self.current_bet += self.max_bet(value)
-    #     self.pay(value)
-    #     if self.current_bet > self.table.pot.highest_bet:
-    #         self.table.pot.highest_bet = self.current_bet
-    #         self.table.cnt_bets += 1
-    #     self.played = True
-
     def do_bet(self, value):
         """Action of betting a certain value"""
-        self.current_bet += min(self.stack, value)
-        self.stack -= min(self.stack, value)
-        self.table.pot.highest_bet = max(self.current_bet, self.table.pot.highest_bet)
-        self.table.cnt_bets += self.current_bet > self.table.pot.highest_bet
+        self.current_bet += self.max_bet(value)
+        self.pay(value)
+        if self.current_bet > self.table.pot.highest_bet:
+            self.table.pot.highest_bet = self.current_bet
+            self.table.cnt_bets += 1
         self.played = True
 
     def bet(self, value):
         """Bet and step to next player"""
         if value >= self.table.min_bet:
             self.table.min_bet = 2*value - self.table.pot.highest_bet
             self.do_bet(value)
         elif self.table.min_bet > self.stack:
-            self.bet(self.stack)
+            self.bet(self.table.min_bet)
         else:
             raise ValueError(f"You cannot bet {value} if the minimum bet is {self.table.min_bet} "
                              f"and your stack is {self.stack}")
         self.table.advance_seat_playing()
 
     def do_call(self):
         """Action of calling"""
```

### Comparing `pkrcomponents-1.3.1/pkrcomponents/tests/actions/test_move.py` & `pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_move.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/tests/actions/test_street.py` & `pkrcomponents-1.3.2/pkrcomponents/tests/actions/test_street.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/pkrcomponents/tournament.py` & `pkrcomponents-1.3.2/pkrcomponents/tournament.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.3.1/setup.py` & `pkrcomponents-1.3.2/setup.py`

 * *Files identical despite different names*

