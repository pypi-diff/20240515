# Comparing `tmp/nonebot_plugin_tetris_stats-1.2.6.tar.gz` & `tmp/nonebot_plugin_tetris_stats-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-1.2.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-1.2.7.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-1.2.6.tar` & `nonebot_plugin_tetris_stats-1.2.7.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    34523 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/README.md
--rw-r--r--   0        0        0      791 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0      331 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/config.py
--rw-r--r--   0        0        0     1730 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
--rw-r--r--   0        0        0     1367 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
--rw-r--r--   0        0        0    14144 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py
--rw-r--r--   0        0        0     2052 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
--rw-r--r--   0        0        0     3026 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
--rw-r--r--   0        0        0     6279 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
--rw-r--r--   0        0        0     3256 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
--rw-r--r--   0        0        0     5458 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
--rw-r--r--   0        0        0        0 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/__init__.py
--rw-r--r--   0        0        0     3908 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
--rw-r--r--   0        0        0     1005 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
--rw-r--r--   0        0        0     4010 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/db/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-15 00:57:28.890992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/db/models.py
--rw-r--r--   0        0        0     1435 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0      208 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/constant.py
--rw-r--r--   0        0        0     2641 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0      323 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/__init__.py
--rw-r--r--   0        0        0     1294 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py
--rw-r--r--   0        0        0      771 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py
--rw-r--r--   0        0        0     4122 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py
--rw-r--r--   0        0        0      334 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/base.py
--rw-r--r--   0        0        0     1028 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py
--rw-r--r--   0        0        0      318 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0     3062 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py
--rw-r--r--   0        0        0     2219 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py
--rw-r--r--   0        0        0     1079 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py
--rw-r--r--   0        0        0      231 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/typing.py
--rw-r--r--   0        0        0     2917 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py
--rw-r--r--   0        0        0      536 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
--rw-r--r--   0        0        0     1122 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
--rw-r--r--   0        0        0    12720 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py
--rw-r--r--   0        0        0     7818 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py
--rw-r--r--   0        0        0      496 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
--rw-r--r--   0        0        0     2111 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
--rw-r--r--   0        0        0       49 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/__init__.py
--rw-r--r--   0        0        0      742 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py
--rw-r--r--   0        0        0     2824 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py
--rw-r--r--   0        0        0      319 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0      189 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user_profile.py
--rw-r--r--   0        0        0     2635 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py
--rw-r--r--   0        0        0      173 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
--rw-r--r--   0        0        0     2939 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py
--rw-r--r--   0        0        0     2548 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
--rw-r--r--   0        0        0       49 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/__init__.py
--rw-r--r--   0        0        0      851 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py
--rw-r--r--   0        0        0     5090 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py
--rw-r--r--   0        0        0      325 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0     3436 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py
--rw-r--r--   0        0        0      603 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py
--rw-r--r--   0        0        0     2712 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py
--rw-r--r--   0        0        0      463 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
--rw-r--r--   0        0        0     6463 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py
--rw-r--r--   0        0        0     1769 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/avatar.py
--rw-r--r--   0        0        0     3006 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/browser.py
--rw-r--r--   0        0        0      945 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/exception.py
--rw-r--r--   0        0        0     2097 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/host.py
--rw-r--r--   0        0        0     7337 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/metrics.py
--rw-r--r--   0        0        0      440 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/platform.py
--rw-r--r--   0        0        0      935 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/render/__init__.py
--rw-r--r--   0        0        0      197 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/render/schemas/base.py
--rw-r--r--   0        0        0      282 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/render/schemas/bind.py
--rw-r--r--   0        0        0     1521 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py
--rw-r--r--   0        0        0     6263 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/request.py
--rw-r--r--   0        0        0     1412 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/retry.py
--rw-r--r--   0        0        0      394 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/screenshot.py
--rw-r--r--   0        0        0     2594 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/templates.py
--rw-r--r--   0        0        0      922 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/typing.py
--rw-r--r--   0        0        0       93 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/version.py
--rw-r--r--   0        0        0     3615 2024-05-15 00:57:28.894992 nonebot_plugin_tetris_stats-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/README.md
+-rw-r--r--   0        0        0      791 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/config.py
+-rw-r--r--   0        0        0     1730 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
+-rw-r--r--   0        0        0     1367 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
+-rw-r--r--   0        0        0    14144 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py
+-rw-r--r--   0        0        0     2052 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
+-rw-r--r--   0        0        0     3026 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
+-rw-r--r--   0        0        0     6279 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
+-rw-r--r--   0        0        0     3256 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
+-rw-r--r--   0        0        0     5458 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
+-rw-r--r--   0        0        0        0 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/__init__.py
+-rw-r--r--   0        0        0     3908 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
+-rw-r--r--   0        0        0     1005 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
+-rw-r--r--   0        0        0     4010 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/db/__init__.py
+-rw-r--r--   0        0        0     3009 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/db/models.py
+-rw-r--r--   0        0        0     1435 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/constant.py
+-rw-r--r--   0        0        0     2641 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/__init__.py
+-rw-r--r--   0        0        0     1294 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py
+-rw-r--r--   0        0        0      771 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py
+-rw-r--r--   0        0        0     4122 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py
+-rw-r--r--   0        0        0      334 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/base.py
+-rw-r--r--   0        0        0     1028 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py
+-rw-r--r--   0        0        0      318 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0     3062 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py
+-rw-r--r--   0        0        0     2219 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py
+-rw-r--r--   0        0        0     1079 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py
+-rw-r--r--   0        0        0      231 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/typing.py
+-rw-r--r--   0        0        0     2917 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py
+-rw-r--r--   0        0        0      536 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
+-rw-r--r--   0        0        0     1122 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
+-rw-r--r--   0        0        0    16379 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py
+-rw-r--r--   0        0        0     7818 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py
+-rw-r--r--   0        0        0      496 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
+-rw-r--r--   0        0        0     2111 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py
+-rw-r--r--   0        0        0     2824 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py
+-rw-r--r--   0        0        0      319 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0      189 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2635 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py
+-rw-r--r--   0        0        0      173 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
+-rw-r--r--   0        0        0     2939 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py
+-rw-r--r--   0        0        0     2548 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py
+-rw-r--r--   0        0        0     5090 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py
+-rw-r--r--   0        0        0      325 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user.py
+-rw-r--r--   0        0        0     3436 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py
+-rw-r--r--   0        0        0      603 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2712 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py
+-rw-r--r--   0        0        0      463 2024-05-15 05:35:32.326433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
+-rw-r--r--   0        0        0     6463 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py
+-rw-r--r--   0        0        0     1769 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/avatar.py
+-rw-r--r--   0        0        0     3006 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/browser.py
+-rw-r--r--   0        0        0      945 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/exception.py
+-rw-r--r--   0        0        0     2097 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/host.py
+-rw-r--r--   0        0        0     7337 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/metrics.py
+-rw-r--r--   0        0        0      440 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/platform.py
+-rw-r--r--   0        0        0      935 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/render/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/render/schemas/base.py
+-rw-r--r--   0        0        0      282 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/render/schemas/bind.py
+-rw-r--r--   0        0        0     1521 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py
+-rw-r--r--   0        0        0     6263 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/request.py
+-rw-r--r--   0        0        0     1412 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/retry.py
+-rw-r--r--   0        0        0      394 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/screenshot.py
+-rw-r--r--   0        0        0     2594 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/templates.py
+-rw-r--r--   0        0        0      922 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/typing.py
+-rw-r--r--   0        0        0       93 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/version.py
+-rw-r--r--   0        0        0     3643 2024-05-15 05:35:32.330433 nonebot_plugin_tetris_stats-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-1.2.6/LICENSE` & `nonebot_plugin_tetris_stats-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/README.md` & `nonebot_plugin_tetris_stats-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/__init__.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/db/__init__.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/db/models.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/db/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 import contextlib
 from asyncio import gather
-from datetime import datetime, timedelta, timezone
+from collections import defaultdict
+from datetime import date, datetime, timedelta, timezone
 from hashlib import md5
 from math import ceil, floor
+from typing import ClassVar
 from urllib.parse import urlunparse
 from zoneinfo import ZoneInfo
 
+from aiofiles import open
+from nonebot import get_driver
 from nonebot.adapters import Bot, Event
+from nonebot.compat import type_validate_json
 from nonebot.matcher import Matcher
 from nonebot_plugin_alconna import At
 from nonebot_plugin_alconna.uniseg import UniMessage
+from nonebot_plugin_apscheduler import scheduler  # type: ignore[import-untyped]
+from nonebot_plugin_localstore import get_data_file  # type: ignore[import-untyped]
 from nonebot_plugin_orm import get_session
 from nonebot_plugin_session import EventSession  # type: ignore[import-untyped]
 from nonebot_plugin_session_orm import get_session_persist_id  # type: ignore[import-untyped]
 from sqlalchemy import select
+from zstandard import ZstdDecompressor
 
 from ...db import query_bind_info, trigger
 from ...utils.host import HostPage, get_self_netloc
 from ...utils.platform import get_platform
 from ...utils.render import TETRIOInfo, render
 from ...utils.render.schemas.base import Avatar
 from ...utils.render.schemas.tetrio_info import Data, Radar, Ranking, TetraLeague, TetraLeagueHistory
 from ...utils.render.schemas.tetrio_info import User as TemplateUser
 from ...utils.screenshot import screenshot
-from ...utils.typing import Me
+from ...utils.typing import Me, Number
 from ..constant import CANT_VERIFY_MESSAGE
 from . import alc
 from .api import Player, User, UserInfoSuccess
 from .api.models import TETRIOHistoricalData
+from .api.schemas.tetra_league import TetraLeagueSuccess
 from .api.schemas.user_info import NeverPlayedLeague, NeverRatedLeague, RatedLeague
 from .api.schemas.user_records import SoloModeRecord, SoloRecord
 from .constant import GAME_TYPE, TR_MAX, TR_MIN
+from .model import IORank
 
 UTC = timezone.utc
 
+driver = get_driver()
+
 
 @alc.assign('query')
 async def _(bot: Bot, event: Event, matcher: Matcher, target: At | Me, event_session: EventSession):
     async with trigger(
         session_persist_id=await get_session_persist_id(event_session),
         game_platform=GAME_TYPE,
         command_type='query',
@@ -53,17 +65,17 @@
         if bind is None:
             await matcher.finish('未查询到绑定信息')
         message = UniMessage(CANT_VERIFY_MESSAGE)
         player = Player(user_id=bind.game_account, trust=True)
         user, user_info, user_records = await gather(player.user, player.get_info(), player.get_records())
         sprint = user_records.data.records.sprint
         blitz = user_records.data.records.blitz
-        with contextlib.suppress(TypeError):
-            message += UniMessage.image(raw=await make_query_image(user, user_info, sprint.record, blitz.record))
-            await message.finish()
+        # with contextlib.suppress(TypeError):
+        message += UniMessage.image(raw=await make_query_image(user, user_info, sprint.record, blitz.record))
+        await message.finish()
         message += make_query_text(user_info, sprint, blitz)
         await message.finish()
 
 
 @alc.assign('query')
 async def _(account: Player, event_session: EventSession):
     async with trigger(
@@ -152,31 +164,31 @@
                     .where(TETRIOHistoricalData.id < min([i.id for i in historical_data]))
                     .limit(1)
                 )
             ).one_or_none()
             if extra is not None:
                 historical_data = list(historical_data)
                 historical_data.append(extra)
-    if not historical_data:
+    full_export_data = FullExport.get_data(user.unique_identifier)
+    if not historical_data and not full_export_data:
         return [
             Data(record_at=today - forward, tr=user_info.data.user.league.rating),
             Data(record_at=today.replace(microsecond=1000), tr=user_info.data.user.league.rating),
         ]
     histories = [
         Data(
             record_at=i.update_time.astimezone(ZoneInfo('Asia/Shanghai')),
             tr=i.data.data.user.league.rating,
         )
         for i in historical_data
         if isinstance(i.data, UserInfoSuccess) and isinstance(i.data.data.user.league, RatedLeague)
-    ]
+    ] + full_export_data
 
     # 按照时间排序
     histories = sorted(histories, key=lambda x: x.record_at)
-    print(histories)
     for index, value in enumerate(histories):
         # 在历史记录里找有没有今天0点后的数据, 并且至少要有两个数据点
         if value.record_at > today and len(histories) >= 2:  # noqa: PLR2004
             histories = histories[:index] + [
                 get_specified_point(histories[index - 1], histories[index], today.replace(microsecond=1000))
             ]
             break
@@ -291,7 +303,86 @@
     if sprint.record is not None:
         message += f'\n40L: {round(sprint.record.endcontext.final_time/1000,2)}s'
         message += f' ( #{sprint.rank} )' if sprint.rank is not None else ''
     if blitz.record is not None:
         message += f'\nBlitz: {blitz.record.endcontext.score}'
         message += f' ( #{blitz.rank} )' if blitz.rank is not None else ''
     return UniMessage(message)
+
+
+class FullExport:
+    cache: ClassVar[defaultdict[str, set[tuple[datetime, Number]]]] = defaultdict(set)
+    latest_update: ClassVar[date | None] = None
+
+    @classmethod
+    async def init(cls) -> None:
+        async with get_session() as session:
+            full_exports = (await session.scalars(select(IORank).where(IORank.update_time >= cls.start_time()))).all()
+        await gather(
+            *[
+                cls._load(update_time, file_hash)
+                for file_hash, update_time in {
+                    i.file_hash: i.update_time for i in full_exports if i.file_hash is not None
+                }.items()
+            ]
+        )
+
+    @classmethod
+    async def update(cls) -> None:
+        if cls.latest_update == datetime.now(tz=ZoneInfo('Asia/Shanghai')).date():
+            return
+        start_time = cls.start_time()
+        for i in cls.cache:
+            cls.cache[i] = {j for j in cls.cache[i] if j[0] >= start_time}
+        latest_time = max(cls.cache)
+        async with get_session() as session:
+            full_exports = (await session.scalars(select(IORank).where(IORank.update_time > latest_time))).all()
+        await gather(
+            *[
+                cls._load(update_time, file_hash)
+                for file_hash, update_time in {
+                    i.file_hash: i.update_time for i in full_exports if i.file_hash is not None
+                }.items()
+            ]
+        )
+        cls.latest_update = datetime.now(tz=ZoneInfo('Asia/Shanghai')).date()
+
+    @classmethod
+    def get_data(cls, unique_identifier: str) -> list[Data]:
+        return [Data(record_at=i[0], tr=i[1]) for i in cls.cache[unique_identifier]]
+
+    @classmethod
+    def start_time(cls) -> datetime:
+        return (
+            datetime.now(ZoneInfo('Asia/Shanghai')).replace(hour=0, minute=0, second=0, microsecond=0)
+            - timedelta(days=9)
+        ).astimezone(UTC)
+
+    @classmethod
+    async def _load(cls, update_time: datetime, file_hash: str) -> None:
+        try:
+            users = type_validate_json(TetraLeagueSuccess, await cls.decompress(file_hash)).data.users
+        except FileNotFoundError:
+            await cls.clear_invalid(file_hash)
+            return
+        update_time = update_time.astimezone(ZoneInfo('Asia/Shanghai'))
+        for i in users:
+            cls.cache[i.id].add((update_time, i.league.rating))
+
+    @classmethod
+    async def decompress(cls, file_hash: str) -> bytes:
+        async with open(get_data_file('nonebot_plugin_tetris_stats', f'{file_hash}.json.zst'), mode='rb') as file:
+            return ZstdDecompressor().decompress(await file.read())
+
+    @classmethod
+    async def clear_invalid(cls, file_hash: str) -> None:
+        async with get_session() as session:
+            full_exports = (await session.scalars(select(IORank).where(IORank.file_hash == file_hash))).all()
+            for i in full_exports:
+                i.file_hash = None
+            await session.commit()
+
+
+@driver.on_startup
+async def _():
+    await FullExport.init()
+    scheduler.add_job(FullExport.update, 'interval', hours=1)
```

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/avatar.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/browser.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/exception.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/host.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/host.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/metrics.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/render/__init__.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/render/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/request.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/retry.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/templates.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/templates.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/nonebot_plugin_tetris_stats/utils/typing.py` & `nonebot_plugin_tetris_stats-1.2.7/nonebot_plugin_tetris_stats/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.6/pyproject.toml` & `nonebot_plugin_tetris_stats-1.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'nonebot-plugin-tetris-stats'
-version = '1.2.6'
+version = '1.2.7'
 description = '一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件'
 authors = ['scdhh <wallfjjd@gmail.com>']
 readme = 'README.md'
 homepage = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 repository = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 license = 'AGPL-3.0'
 
@@ -42,14 +42,15 @@
 nonebot-adapter-discord = "^0.1.3"
 nonebot-adapter-kaiheila = "^0.3.4"
 nonebot-adapter-onebot = "^2.4.1"
 nonebot-adapter-qq = "^1.4.4"
 nonebot-adapter-satori = "^0.11.4"
 
 [tool.poetry.group.debug.dependencies]
+memory-profiler = "^0.61.0"
 objprint = '^0.2.2'
 viztracer = "^0.16.2"
 
 [build-system]
 requires = ['poetry-core>=1.0.0']
 build-backend = 'poetry.core.masonry.api'
```

### Comparing `nonebot_plugin_tetris_stats-1.2.6/PKG-INFO` & `nonebot_plugin_tetris_stats-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 1.2.6
+Version: 1.2.7
 Summary: 一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: AGPL-3.0
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.2.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.2.7 Summary:
 ä¸æ¬¾åºäº NoneBot2 çç¨äºæ¥è¯¢ Tetris ç¸å³æ¸¸ææ°æ®çæä»¶ Home-
 page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats License:
 AGPL-3.0 Author: scdhh Author-email: wallfjjd@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
```

