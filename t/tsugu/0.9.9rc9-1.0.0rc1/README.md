# Comparing `tmp/tsugu-0.9.9rc9.tar.gz` & `tmp/tsugu-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.9.9rc9.tar", last modified: Tue May 14 10:19:54 2024, max compression
+gzip compressed data, was "tsugu-1.0.0rc1.tar", last modified: Wed May 15 04:13:23 2024, max compression
```

## Comparing `tsugu-0.9.9rc9.tar` & `tsugu-1.0.0rc1.tar`

### file list

```diff
@@ -1,121 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.231572 tsugu-0.9.9rc9/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.231572 tsugu-0.9.9rc9/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/local/router/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/remote/router/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/storage/db/
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/storage/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/storage/remote_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/storage/remote_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/rooms_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/universal/router/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu_async/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/remote/router/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/storage/remote_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/storage/remote_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/rooms_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/tsugu_async/universal/router/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.935928 tsugu-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-15 04:13:23.935928 tsugu-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:13:23.935928 tsugu-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.927928 tsugu-1.0.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.927928 tsugu-1.0.0rc1/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.927928 tsugu-1.0.0rc1/tsugu/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.927928 tsugu-1.0.0rc1/tsugu/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.927928 tsugu-1.0.0rc1/tsugu/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/remote/unbind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.931928 tsugu-1.0.0rc1/tsugu/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.931928 tsugu-1.0.0rc1/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.927928 tsugu-1.0.0rc1/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-15 04:13:23.000000 tsugu-1.0.0rc1/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-15 04:13:23.000000 tsugu-1.0.0rc1/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:13:23.000000 tsugu-1.0.0rc1/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 04:13:23.000000 tsugu-1.0.0rc1/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 04:13:23.000000 tsugu-1.0.0rc1/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.931928 tsugu-1.0.0rc1/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.931928 tsugu-1.0.0rc1/tsugu_async/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.931928 tsugu-1.0.0rc1/tsugu_async/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.935928 tsugu-1.0.0rc1/tsugu_async/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/remote/unbind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.935928 tsugu-1.0.0rc1/tsugu_async/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:13:23.935928 tsugu-1.0.0rc1/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-15 04:13:12.000000 tsugu-1.0.0rc1/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-0.9.9rc9/LICENSE` & `tsugu-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/PKG-INFO` & `tsugu-1.0.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,123 +1,89 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.9.9rc9
+Version: 1.0.0rc1
 Summary: Tsugu Python Frontend
-Home-page: https://github.com/kumoSleeping/tsugu-bot-py
+Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
-        <h1 align="center"> Tsugu Bot Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
+        <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
         
         
-        <p align="center">
+        <div align="center">
+        
+        _✨ Python 编写的 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 自然语言交互库  ✨_
+        
+        </div>
         
+        <p align="center">
         <a href="https://github.com/Yamamoto-2/tsugu-bangdream-bot">
-            <img src="https://img.shields.io/badge/tsugubangdream bot - v2 api-yellow" alt="license">
+            <img src="https://img.shields.io/badge/tsugubangdream bot - api-yellow" alt="license">
           </a>
         
         <a href="https://github.com/kumoSleeping/tsugu-python-frontend?tab=MIT-1-ov-file">
             <img src="https://img.shields.io/github/license/kumoSleeping/tsugu-python-frontend" alt="license">
           </a>
         <a href="https://pypi.org/project/tsugu/">
             <img src="https://img.shields.io/pypi/v/tsugu.svg" alt="license">
           </a>
         </p>
         
-        
-        ***
-        
-        
-        - `tsugu`
-          - [x] 自然语言输入 -> 返回结果
-          - [x] 远程数据库 
-          - [x] 本地数据库 
-        
-        
-        - `tsugu.async`
-          - [x] 自然语言输入 -> 返回结果
-          - [x] 远程数据库 
-          - [ ] 本地数据库
-        
-        
-        
+        ---
         
         
         ```shell
         pip install tsugu
         ```
-        > Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
-        
         
-        ***
         
+        > Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
-        <h2 align="center"> 测试与调用 </h2>
+        ***
         
         ## handler
         
-        - `handler` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
+        - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
         import tsugu
         
-        # tsugu.database(path="./data.db")
-        
         # 四个参数，分别意味着 消息内容 用户id 平台 频道id
         for i in tsugu.handler(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414'):
             print('文本: ',i) if isinstance(i, str) else None
             print(f"[图片]") if isinstance(i, bytes) else None
         ```
         
         ```python
         import tsugu_async
-        
-        # tsugu_async.config.reload_from_json('./config.json')
-        
-        async def main():
-            res = await tsugu_async.handler(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414')
-            for i in res:
-                print('文本: ',i) if isinstance(i, str) else None
-                print(f"[图片]") if isinstance(i, bytes) else None
+        ...
         ```
         
         
         > 在常用的qqbot中，群号就是 `channel_id`。   
         > 当你使用QQ号作为 `user_id` 时，`platform` 可以填写 `red`。   
         
         ## handler_raw
         如果你方便使用 base64，`handler_raw` 方法或许会更好  
-        `tsugu` 后端本身返回此数据结构，如果你的bot可以直接发送 `base64` 类图片，这个方法会节省不必要的开销。
+        `tsugu` 后端本身返回此数据结构，这个方法可以节省不必要的开销。
         
         ```python
         import tsugu
         
         for i in tsugu.handler_raw(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414'):
             print('文本: ',i) if i['type'] == 'text' else None
             print(f"[图片]") if i['type'] == 'base64' else None
-        
-        
+        ```
+        ```python
         import tsugu_async
         ...
         ```
         
         
-        ## 使用本地数据库(不支持`tsugu_async`)
-        本地数据库由 `sqlite3` 提供，你可以使用 `tsugu.database` 来创建或使用本地数据库。
-        
-        ```py
-        import tsugu
-        
-        tsugu.database(path="./data.db")
-        ```
-        
-        > 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。  
-        > 远程数据库将不使用。
-        
         ## 配置
         
         
         > 随意更改配置项可能会导致不可预知的错误。
         
         ### tsugu_api settings
         
@@ -225,72 +191,25 @@
         ```
         
         
         
         ***
         
          <details>
-        <summary><b>客服ano酱指导(这里可以点击)</b></summary>
+        <summary><b>客服🐱指导(这里可以点击)</b></summary>
          
         **注意，如果你不知道什么是BanGDream，请不要随意加群**    
         **本群还是欢迎加群的（**    
         [BanGDreamBot开发聊天群](https://qm.qq.com/q/zjUPQkrdpm)   
         温馨的聊天环境～   
         
         </details>
         
         
-        下方已无内容。
-        
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
+        ---
         
-        🐱: 喵
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,42 +1,29 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.9.9rc9 Summary: Tsugu Python
-Frontend Home-page: https://github.com/kumoSleeping/tsugu-bot-py Author:
+Metadata-Version: 2.1 Name: tsugu Version: 1.0.0rc1 Summary: Tsugu Python
+Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
-                       ************ TTssuugguu BBoott PPyy[[ttmmrrnn]] ************
+                       ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
+_â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
+         bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
-*** - `tsugu` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [x] è¿ç¨æ°æ®åº -
-[x] æ¬å°æ°æ®åº - `tsugu.async` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ -
-[x] è¿ç¨æ°æ®åº - [ ] æ¬å°æ°æ®åº ```shell pip install tsugu ``` >
-Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n ***
-                          ********** ?æ?µ??è?¯??ä?¸??è?°??ç??¨ **********
-## handler - `handler` æ¯ `tsugu`
-çä¸ä¸ªåæ­¥å½æ°ï¼ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
-```python import tsugu # tsugu.database(path="./data.db") #
-åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å° é¢éid for i in
-tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481', platform='red',
-channel_id='666808414'): print('ææ¬: ',i) if isinstance(i, str) else None
-print(f"[å¾ç]") if isinstance(i, bytes) else None ``` ```python import
-tsugu_async # tsugu_async.config.reload_from_json('./config.json') async def
-main(): res = await tsugu_async.handler(message='æ¥å¡ ars 1x',
-user_id='1528593481', platform='red', channel_id='666808414') for i in res:
-print('ææ¬: ',i) if isinstance(i, str) else None print(f"[å¾ç]") if
-isinstance(i, bytes) else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
-`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
-å¯ä»¥å¡«å `red`ã ## handler_raw å¦æä½ æ¹ä¾¿ä½¿ç¨
-base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
-åç«¯æ¬èº«è¿åæ­¤æ°æ®ç»æï¼å¦æä½ çbotå¯ä»¥ç´æ¥åé `base64`
-ç±»å¾çï¼è¿ä¸ªæ¹æ³ä¼èçä¸å¿è¦çå¼éã ```python import tsugu
-for i in tsugu.handler_raw(message='æ¥å¡ ars 1x', user_id='1528593481',
-platform='red', channel_id='666808414'): print('ææ¬: ',i) if i['type'] ==
-'text' else None print(f"[å¾ç]") if i['type'] == 'base64' else None import
-tsugu_async ... ``` ## ä½¿ç¨æ¬å°æ°æ®åº(ä¸æ¯æ`tsugu_async`)
-æ¬å°æ°æ®åºç± `sqlite3` æä¾ï¼ä½ å¯ä»¥ä½¿ç¨ `tsugu.database`
-æ¥åå»ºæä½¿ç¨æ¬å°æ°æ®åºã ```py import tsugu tsugu.database(path="./
-data.db") ``` > æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
-æä¾ç¨æ·æ°æ®ã > è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã ## éç½® >
+--- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
+- `handler` ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
+```python import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id
+å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
+user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
+',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
+else None ``` ```python import tsugu_async ... ``` >
+å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º
+`user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã ## handler_raw
+å¦æä½ æ¹ä¾¿ä½¿ç¨ base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
+åç«¯æ¬èº«è¿åæ­¤æ°æ®ç»æï¼è¿ä¸ªæ¹æ³å¯ä»¥èçä¸å¿è¦çå¼éã
+```python import tsugu for i in tsugu.handler_raw(message='æ¥å¡ ars 1x',
+user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
+',i) if i['type'] == 'text' else None print(f"[å¾ç]") if i['type'] ==
+'base64' else None ``` ```python import tsugu_async ... ``` ## éç½® >
 éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api
 settings ```py from tsugu_api import settings settings.timeout = 10 '''
 è¯·æ±è¶æ¶æ¶é´ ''' settings.proxy = '' ''' ä»£çå°å '''
 settings.backend_url = 'http://tsugubot.com:8080' ''' åç«¯å°å é»è®¤ä¸º
 Tsugu å®æ¹åç«¯ï¼è¥æèªå»ºåç«¯æå¡å¨å¯è¿è¡ä¿®æ¹ã '''
 settings.backend_proxy = True ''' æ¯å¦ä½¿ç¨åç«¯ä»£ç
 å½è®¾ç½®ä»£çå°ååå¯ä¿®æ¹æ­¤é¡¹ä»¥å³å®æ¯å¦ä½¿ç¨ä»£çã é»è®¤ä¸º
@@ -61,60 +48,15 @@
 ''' config.allow_gap_less = True '''
 æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
 config.get_remote_user_data_max_retry = 3 '''
 è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ° ''' config.token_name = "Tsugu" '''
 bandori station token ''' config.bandori_station_token = "ZtV4EX2K9Onb" '''
 bandori station token ''' config.ban_gacha_simulate_group_data = [] '''
 éè¦å³é­æ¨¡ææ½å¡çç¾¤ ''' config.commands = ... config.user_commands =
-... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼
+... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼
 ((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
-qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ ä¸æ¹å·²æ åå®¹ã
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-ð±: åµ Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
-markdown
+qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ --- Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-0.9.9rc9/setup.py` & `tsugu-1.0.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.9.9-rc9',
+    version='1.0.0-rc1',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/kumoSleeping/tsugu-bot-py',
+    url='https://github.com/kumoSleeping/ChatTsuguPy',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
             "loguru",
-            "tsugu-api-python>=1.0.3"
+            "tsugu-api-python>=1.0.4"
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-0.9.9rc9/test/test_async.py` & `tsugu-1.0.0rc1/test/test_async.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,24 +19,25 @@
                     img.show()
                     print(f"[图像大小: {len(i) / 1024:.2f}KB]")
 
         # tsugu.database('./user_data.db')
         # tsugu_async.config.reload_from_json('./config.json')
         # from tsugu_api_async import settings
         # settings.backend_url = 'http://127.0.0.1:8010'
-        # from tsugu_async import config
-        # config.allow_gap_less = True
+        from tsugu_api_async import settings
+        settings.userdata_backend_url = 'http://127.0.0.1:14140'
 
-        msg1 = await tsugu_async.handler('查卡ksm', '1528593481', 'red', '666808414')
+        msg1 = await tsugu_async.handler('验证解绑 0', '1528593481', 'red', '666808414')
         await show_back_msg(msg1)
 
         # msg2 = await tsugu_async.handler('ycm', '1528593481', 'red', '666808414')
         # await show_back_msg(msg2)
 
         # msg3 = await tsugu_async.handler('12324 测q1试', '1528593481', 'red', '666808414')
         # await show_back_msg(msg3)
 
         # print(tsugu_api.get_user_data('red', '1528593481'))
 
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tsugu-0.9.9rc9/tsugu/command_matcher/__init__.py` & `tsugu-1.0.0rc1/tsugu/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/config.py` & `tsugu-1.0.0rc1/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/handler.py` & `tsugu-1.0.0rc1/tsugu_async/handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 import base64
 from typing import List, Union, Dict
 
 from .utils import *
-from .utils import text_response
-from . import remote
-from . import local
-from .utils import config
 from loguru import logger
 from tsugu_api import settings
+from . import router
 
-
-def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
+async def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Union[bytes, str]]
     '''
-    data = handler_raw(message, user_id, platform, channel_id)
-    response = []
-    if not data:
+    try:
+        data = await handler_raw(message, user_id, platform, channel_id)
+        response = []
+        if not data:
+            return response
+        for item in data:
+            response.append(item['string']) if item['type'] == 'string' else None
+            response.append(base64.b64decode(item['string'].encode('utf-8')) if item['type'] == 'base64' else None)
         return response
-    for item in data:
-        response.append(item['string']) if item['type'] == 'string' else None
-        response.append(base64.b64decode(item['string'].encode('utf-8')) if item['type'] == 'base64' else None)
-    return response
+    except Exception as e:
+        raise e
 
 
-def handler_raw(message: str, user_id: str, platform: str, channel_id: str) -> List[Dict[str, str]]:
+async def handler_raw(message: str, user_id: str, platform: str, channel_id: str) -> List[Dict[str, str]]:
     '''
     handler_raw 除了返回的数据类型不同外，其他与 handler 函数一致
     返回格式为 Tsugu 标准数据格式
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Dict[str, str]]
     '''
     try:
-        # 如果启用了本地数库
-        if config._user_database_path:
-            return r if (r := local.handler(message, user_id, platform, channel_id)) else None
-        # 否则使用远程服务器
-        return r if (r := remote.handler(message, user_id, platform, channel_id)) else None
+        # 使用远程服务器
+        res = await router.handler(message, user_id, platform, channel_id)
+        if not res:
+            return []
+        return res
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
```

### Comparing `tsugu-0.9.9rc9/tsugu/local/router/change_server_mode.py` & `tsugu-1.0.0rc1/tsugu/router/remote/change_server_mode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from ...config import config
-from ...utils import text_response, UserLocal
+from ...utils import text_response, User
 from ...command_matcher import MC
 import tsugu_api
 from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
 from tsugu_api._typing import _ServerId, _Update
-import typing
-from ...storage.db import db_manager
-import json
 
 
-def handler(user: UserLocal, res: MC, platform: str, channel_id: str):
-    server_mode: typing.Optional[_ServerId] = server_name_2_server_id(res.args[0]) if res.args else None
-    if not server_mode:
-        return text_response('未找到服务器，请输入正确的服务器名')
-    cursor = db_manager.conn.cursor()
-    cursor.execute("UPDATE users SET server_mode = ? WHERE user_id = ? AND platform = ?",
-                   (server_mode, user.user_id, platform))
-    db_manager.conn.commit()
-    return text_response(f'服务器模式设置为 {server_id_2_server_name(server_mode)}')
+def handler(user: User, res: MC, platform: str, channel_id: str):
+    if res.args:
+        server_mode = server_name_2_server_id(res.args[0])
+        if not server_exists(server_mode):
+            return text_response('未找到服务器，请输入正确的服务器名')
+        update: _Update = {'server_mode': server_mode, }
+        if r := tsugu_api.change_user_data(platform, user.user_id, update):
+            if r.get('status') == 'success':
+                return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
+            return text_response(r.get('data'))
```

### Comparing `tsugu-0.9.9rc9/tsugu/local/router/player_status.py` & `tsugu-1.0.0rc1/tsugu/router/remote/player_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from ...config import config
+from ...utils import text_response, User
+from ...command_matcher import MC
 import tsugu_api
 from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
 from tsugu_api._typing import _ServerId, _Update
 
-from ...utils import text_response, UserLocal
-from ...command_matcher import MC
-
-
 
-def handler(user: UserLocal, res: MC, platform: str, channel_id: str):
+def handler(user: User, res: MC, platform: str, channel_id: str):
     # 无参数
     if not res.args:
         # 默认情况1: 优先当前服务器
         for i in user.game_ids:
             if i.get("server") == user.server_mode:
                 player_id = str(i.get("game_id"))
                 server = int(i.get("server"))
@@ -21,18 +19,18 @@
                 return msg
         else:
             # 默认情况2: 优先第一个记录
             if len(user.game_ids) > 0:
                 player_id = str(user.game_ids[0].get("game_id"))
                 server = int(user.game_ids[0].get("server"))
                 text = f'已查找第一个记录 {player_id}'
-                msg = [text_response(text), tsugu_api.search_player(int(player_id), server)]
+                msg = tsugu_api.search_player(int(player_id), server) + text_response(text)
                 return msg
             else:
-                return text_response('未绑定任何记录')
+                return text_response('未绑定任何记录，可以使用 绑定玩家 进行绑定')
 
     # 查询指定服务器的玩家状态
     server: _ServerId = server_name_2_server_id(res.args[0])
     if server_exists(server):
         for i in user.game_ids:
             if i.get("server") == server:
                 player_id = str(i.get("game_id"))
@@ -50,10 +48,7 @@
         player_id = str(user.game_ids[int(res.args[0]) - 1].get("game_id"))
         server = int(user.game_ids[int(res.args[0]) - 1].get("server"))
         text = f'已查找第 {res.args[0]} 条记录'
         msg = tsugu_api.search_player(int(player_id), server) + text_response(text)
         return msg
 
     return text_response('请确保输入是 服务器名(字母缩写) 或者 记录(数字)')
-
-
-
```

### Comparing `tsugu-0.9.9rc9/tsugu/local/router/unbind_player.py` & `tsugu-1.0.0rc1/tsugu/router/remote/bind_player_verification_on.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,23 @@
+from ...utils import text_response, User
 from ...config import config
-from ...utils import text_response, UserLocal
 from ...command_matcher import MC
-import tsugu_api
-from ...utils import server_exists, server_name_2_server_id
+from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
 from tsugu_api._typing import _ServerId
+import tsugu_api
 
-from ...storage.db import db_manager, get_user
-
-
-def handler(user: UserLocal, res: MC, platform: str, channel_id: str):
-    if not res.args:
-        return text_response('请输入正确的记录(数字)\n例如: 解除绑定 1')
-
-    if not res.args[0].isdigit():
-        return text_response('请输入正确的记录(数字)')
-
-    now_game_ids = user.game_ids
-    # 检测是否存在该记录
-    if int(res.args[0]) > len(now_game_ids):
-        return text_response(f'未找到记录 {res.args[0]}')
-
-    exe_game_id = user.game_ids.pop(int(res.args[0]) - 1)
 
-    cursor = db_manager.conn.cursor()
-    cursor.execute("UPDATE users SET game_ids = ? WHERE user_id = ? AND platform = ?",
-                   (str(now_game_ids), user.user_id, platform))
-    db_manager.conn.commit()
+def handler(user: User, res: MC, platform: str, channel_id: str):
+    if not res.args or len(res.args) < 2:
+        return text_response('请输入正确的格式：验证绑定 你的玩家ID(数字) 服务器名(字母缩写)')
+    player_id = int(res.args[0])
+    server_pre = server_name_2_server_id(res.args[1])
+    if not server_exists(server_pre):
+        return text_response('未找到服务器，请输入正确的服务器名')
+    user.server_mode = server_pre
+
+    r = tsugu_api.bind_player_verification(platform, user.user_id, user.server_mode, player_id, True)
+    if r.get('status') != 'success':
+        return text_response(r.get('data'))
+    return text_response(f'绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
 
-    return text_response(f'已解除绑定 {exe_game_id.get("game_id")}')
```

### Comparing `tsugu-0.9.9rc9/tsugu/remote/__init__.py` & `tsugu-1.0.0rc1/tsugu_async/router/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,46 @@
-import time
-
-from ..utils import server_exists, text_response, config
+from ..utils import server_exists, text_response, config, get_user
 from ..command_matcher import match_command
-from ..universal import universal_api_handler
+from . import remote
+from . import universal
+from .help import help_command
+from .rooms_forward import submit_rooms
+
+
+async def universal_api_handler(user_id: str, message: str,  platform: str, channel_id: str):
+    for i in config.commands:
+        if res := match_command(message, commands=i['command_name']):
+            api = i['api']
+            user = await get_user(user_id, platform)
+            return await universal.api_handler(user, res, api, platform, channel_id)
 
-from . import router
-from ..storage import remote_db
+    # 开始匹配 help
+    if res := match_command(message, commands=['help']):
+        return await help_command(res)
+
+    # 开始上传车牌
+    if res := match_command(message, commands=['上传车牌', '']):
+        await submit_rooms(res, user_id, platform)
+    return None
 
 
-def remote_api_handler(user_id: str, message: str,  platform: str, channel_id: str):
+async def remote_api_handler(user_id: str, message: str,  platform: str, channel_id: str):
     for i in config.user_commands:
         if res := match_command(message, commands=i['command_name']):
             api = i['api']
-            user = remote_db.get_user(user_id, platform)
-            return router.api_handler(user, res, api, platform, channel_id)
+            user = await get_user(user_id, platform)
+            return await remote.api_handler(user, res, api, platform, channel_id)
 
     return None
 
 
-def handler(message: str, user_id: str, platform: str, channel_id: str):
+async def handler(message: str, user_id: str, platform: str, channel_id: str):
     # 进行 api 命令匹配
-    result = universal_api_handler(user_id, message, platform, channel_id, local=False)
+    result = await universal_api_handler(user_id, message, platform, channel_id)
     if result:
         return result
 
     # 远程命令
-    result = remote_api_handler(user_id, message, platform, channel_id)
+    result = await remote_api_handler(user_id, message, platform, channel_id)
     if result:
         return result
```

### Comparing `tsugu-0.9.9rc9/tsugu/remote/router/bind_player.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player_verification_on.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from ...config import config
 from ...utils import text_response, User
 from ...command_matcher import MC
-import tsugu_api
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
+import tsugu_api_async
+from ...utils import server_exists, server_name_2_server_id
 
 
-def handler(user: User, res: MC, platform: str, channel_id: str):
-    if res.args:
-        server_pre = server_name_2_server_id(res.args[0])
-        if not server_exists(server_pre):
-            return text_response('未找到服务器，请输入正确的服务器名')
-        user.server_mode = server_pre
-    # 获取绑定请求
-    r = tsugu_api.bind_player_request(platform, user.user_id, user.server_mode, True)
+async def handler(user: User, res: MC, platform: str, channel_id: str):
+    if not res.args or len(res.args) < 2:
+        return text_response('请输入正确的格式：验证绑定 你的玩家ID(数字) 服务器名(字母缩写)')
+    player_id = int(res.args[0])
+    server_pre = server_name_2_server_id(res.args[1])
+    if not server_exists(server_pre):
+        return text_response('未找到服务器，请输入正确的服务器名')
+    user.server_mode = server_pre
+
+    r = await tsugu_api_async.bind_player_verification(platform, user.user_id, user.server_mode, player_id, True)
     if r.get('status') != 'success':
         return text_response(r.get('data'))
-    return text_response(
-        f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 你的玩家ID(数字) {server_id_2_server_name(user.server_mode)}\n''')
+    return text_response(f'绑定成功！现在可以使用 玩家状态 {len(user.game_ids) + 1} 查看绑定的玩家状态')
+
+
```

### Comparing `tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_off.py` & `tsugu-1.0.0rc1/tsugu/router/remote/change_default_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from ...config import config
 from ...utils import text_response, User
 from ...command_matcher import MC
 import tsugu_api
-from ...utils import server_exists, server_name_2_server_id
+from ...utils import server_exists, server_names_2_server_ids
+from tsugu_api._typing import _Update
 
 
 def handler(user: User, res: MC, platform: str, channel_id: str):
-    if not res.args:
-        return text_response('请输入正确的服务器名参数')
-    server_pre = server_name_2_server_id(res.args[0])
-    if not server_exists(server_pre):
+    default_server = server_names_2_server_ids(res.args)
+    if not default_server:
         return text_response('未找到服务器，请输入正确的服务器名')
-    player_id = int(user.server_list[server_pre]['playerId'])
-
-    r = tsugu_api.bind_player_verification(platform, user.user_id, server_pre, player_id, False)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    return text_response('解绑成功')
-
-
+    change_data: _Update = {'default_server': default_server}
+    r = tsugu_api.change_user_data(platform, user.user_id, change_data)
+    if r.get('status') == 'success':
+        return text_response(f'默认服务器已设置为 {", ".join(res.args)}')
+    return text_response(r.get('data'))
```

### Comparing `tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_on.py` & `tsugu-1.0.0rc1/tsugu/router/remote/bind_player_verification_off.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 from ...utils import text_response, User
 from ...command_matcher import MC
 import tsugu_api
 from ...utils import server_exists, server_name_2_server_id
 
 
 def handler(user: User, res: MC, platform: str, channel_id: str):
-    if not res.args:
-        return text_response('请输入正确的玩家ID和服务器名参数(可选)')
+    if not res.args or len(res.args) > 1:
+        return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
     if not res.args[0].isdigit():
-        return text_response('请输入正确的玩家ID')
-    player_id = int(res.args[0])
-    if len(res.args) > 1:
-        server_pre = server_name_2_server_id(res.args[1])
-        if not server_exists(server_pre):
-            return text_response('未找到服务器，请输入正确的服务器名')
-        user.server_mode = server_pre
-
-    r = tsugu_api.bind_player_verification(platform, user.user_id, user.server_mode, player_id, True)
+        return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
+    if int(res.text) <= 0:
+        return text_response('请输入正确的格式：验证解绑 记录编号(数字)，编号从1开始')
+    if len(user.game_ids) < int(res.text):
+        return text_response('未找到记录')
+    player_id = user.game_ids[int(res.args[0]) - 1].get("game_id")
+    server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
+    r = tsugu_api.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
     if r.get('status') != 'success':
         return text_response(r.get('data'))
-    return text_response('绑定成功')
-
-    # 车牌转发控制
+    return text_response('解绑成功！')
```

### Comparing `tsugu-0.9.9rc9/tsugu/remote/router/change_default_server.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/change_default_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from ...config import config
 from ...utils import text_response, User
 from ...command_matcher import MC
-import tsugu_api
+import tsugu_api_async
 from ...utils import server_exists, server_names_2_server_ids
 from tsugu_api._typing import _Update
 
 
-def handler(user: User, res: MC, platform: str, channel_id: str):
+async def handler(user: User, res: MC, platform: str, channel_id: str):
     default_server = server_names_2_server_ids(res.args)
     if not default_server:
         return text_response('未找到服务器，请输入正确的服务器名')
     change_data: _Update = {'default_server': default_server}
-    r = tsugu_api.change_user_data(platform, user.user_id, change_data)
+    r = await tsugu_api_async.change_user_data(platform, user.user_id, change_data)
     if r.get('status') == 'success':
         return text_response(f'默认服务器已设置为 {", ".join(res.args)}')
-    return text_response(r.get('data'))
+    return text_response(r.get('data'))
```

### Comparing `tsugu-0.9.9rc9/tsugu/remote/router/change_server_mode.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/event_stage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from ...config import config
-from ...utils import text_response, User
+from ...utils import text_response, User, server_exists
 from ...command_matcher import MC
-import tsugu_api
-from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
-from tsugu_api._typing import _ServerId, _Update
-import typing
+import tsugu_api_async
 
+async def handler(user: User, res: MC, platform: str, channel_id: str):
+    if res.args:
+        #     最后一个参数
+        # if server_exists(name_2_index(res.args[-1])):
+        #     user.server_mode = name_2_index(res.args[-1])
+        event_id_pre: str = res.args[0]
+        # if event_id_pre.isdigit():
+        #     event_id = int(event_id_pre)
+        #     return tsugu_api.event_stage(user.server_mode, event_id=event_id, meta=False)
+        if res.text == '-m':
+            return await tsugu_api_async.event_stage(user.server_mode, meta=True)
 
-def handler(user: User, res: MC, platform: str, channel_id: str):
-    server_mode: typing.Optional[_ServerId] = server_name_2_server_id(res.args[0]) if res.args else None
-    if not server_mode:
-        return text_response('未找到服务器，请输入正确的服务器名')
-    update: _Update = {'server_mode': server_mode, }
-    if r := tsugu_api.change_user_data(platform, user.user_id, update):
-        if r.get('status') == 'success':
-            return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
-        return text_response(r.get('data'))
-    # 设置默认服务器列表
-
+    return await tsugu_api_async.event_stage(user.server_mode, meta=False)
```

### Comparing `tsugu-0.9.9rc9/tsugu/remote/router/unbind_player.py` & `tsugu-1.0.0rc1/tsugu/router/remote/unbind_player.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,23 +2,38 @@
 from ...utils import text_response, User
 from ...command_matcher import MC
 import tsugu_api
 from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
 from tsugu_api._typing import _ServerId
 
 
+def mask_data(game_id: str):
+    game_id = str(game_id)
+    if len(game_id) < 6:
+        return game_id[:3] + '*' * (len(game_id) - 3)
+    elif len(game_id) < 3:
+        return '*' * len(game_id)
+    else:
+        game_id = game_id[:3] + '*' * (len(game_id) - 6) + game_id[-3:]
+    return game_id
+
+
 def handler(user: User, res: MC, platform: str, channel_id: str):
-    if res.args:
-        server_pre = server_name_2_server_id(res.args[0])
-        if not server_exists(server_pre):
-            return text_response('未找到服务器，请输入正确的服务器名')
-        user.server_mode = server_pre
-        if not user.server_list[user.server_mode]['playerId']:
-            return text_response('未绑定玩家，请先绑定玩家')
-    r = tsugu_api.bind_player_request(platform, user.user_id, user.server_mode, False)
+    bind_record = '\n'.join(
+        [f'{i + 1}. {mask_data(x.get("game_id"))} {server_id_2_server_name(x.get("server"))}' for i, x in
+         enumerate(user.game_ids)])
+    if not res.args:
+        return text_response(f'请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n{bind_record}')
+
+    if not res.args[0].isdigit():
+        return text_response(f'请输入正确的记录(数字)\n例如: 解除绑定 1\n当前的绑定记录如下:\n{bind_record}')
+
+    if int(res.args[0]) > len(user.game_ids):
+        return text_response(f'未找到记录 {res.args[0]}，当前的绑定记录如下:\n{bind_record}')
+
+    server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
+    r = tsugu_api.bind_player_request(platform, user.user_id, server_mode, False)
     if r.get('status') != 'success':
         return text_response(r.get('data'))
     # 如果是200
     return text_response(
-        f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {server_id_2_server_name(user.server_mode)}\n来完成本次身份验证''')
-
-
+        f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {res.args[0]}\n来完成本次身份验证''')
```

### Comparing `tsugu-0.9.9rc9/tsugu/universal/__init__.py` & `tsugu-1.0.0rc1/tsugu/router/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,46 @@
-from ..utils import User, UserLocal
+from ..utils import server_exists, text_response, config, get_user
 from ..command_matcher import match_command
-from ..config import config
-from . import router
+from . import remote
+from . import universal
 from .help import help_command
-from ..storage import _get_user
 from .rooms_forward import submit_rooms
 
 
+def handler(message: str, user_id: str, platform: str, channel_id: str):
+    # 进行 api 命令匹配
+    result = universal_api_handler(user_id, message, platform, channel_id, local=False)
+    if result:
+        return result
+
+    # 远程命令
+    result = remote_api_handler(user_id, message, platform, channel_id)
+    if result:
+        return result
+
+
 def universal_api_handler(user_id: str, message: str,  platform: str, channel_id: str, local=False):
     for i in config.commands:
         if res := match_command(message, commands=i['command_name']):
             api = i['api']
-            user = _get_user(user_id, platform, local)
-            return router.api_handler(user, res, api, platform, channel_id)
+            user = get_user(user_id, platform)
+            return universal.api_handler(user, res, api, platform, channel_id)
     # 开始匹配 help
     if res := match_command(message, commands=['help']):
         return help_command(res)
         # 开始上传车牌
     if res := match_command(message, commands=['上传车牌', '']):
         submit_rooms(res, user_id, platform)
     return None
 
 
+def remote_api_handler(user_id: str, message: str,  platform: str, channel_id: str):
+    for i in config.user_commands:
+        if res := match_command(message, commands=i['command_name']):
+            api = i['api']
+            user = get_user(user_id, platform)
+            return remote.api_handler(user, res, api, platform, channel_id)
+
+    return None
+
+
+
```

### Comparing `tsugu-0.9.9rc9/tsugu/universal/help.py` & `tsugu-1.0.0rc1/tsugu/router/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/rooms_forward.py` & `tsugu-1.0.0rc1/tsugu/router/rooms_forward.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import tsugu_api
 
-from ..utils import config
+from ..utils import config, get_user
 from loguru import logger
 import httpx
 import re
 
 from ..utils import User, text_response
 from ..command_matcher import MC
-from ..storage import _get_user
 
 
 def submit_rooms(res: MC, user_id, platform=None):
     message = res.text
     # 检查car_config['car']中的关键字
     for keyword in config._car_config["car"]:
         if str(keyword) in message:
             break
     else:
         return []
-
     # 检查car_config['fake']中的关键字
     for keyword in config._car_config["fake"]:
         if str(keyword) in message:
             return []
-
     pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
     if not re.match(pattern, message):
         return []
 
-    user = _get_user(user_id, platform)
+    user = get_user(user_id, platform)
 
     # 获取用户数据
     try:
         if platform:
             if not user.car:
                 return []
     except Exception as e:
@@ -40,15 +37,15 @@
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
 
-        tsugu_api.submit_room_number(int(car_id), user.user_id, message, config.token_name, config.bandori_station_token)
+        tsugu_api.submit_room_number(number=int(car_id), user_id=user.user_id, raw_message=message, source=config.token_name, token=config.bandori_station_token)
         return []
     except Exception as e:
         logger.error(f"[Tsugu] 发生异常: {e}")
         return []  # 虽然提交失败，但是确定了是车牌消息
```

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/__init__.py` & `tsugu-1.0.0rc1/tsugu/router/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/event_stage.py` & `tsugu-1.0.0rc1/tsugu/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/gacha_simulate.py` & `tsugu-1.0.0rc1/tsugu/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/lsycx.py` & `tsugu-1.0.0rc1/tsugu/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/search_player.py` & `tsugu-1.0.0rc1/tsugu/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/song_chart.py` & `tsugu-1.0.0rc1/tsugu/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/ycx.py` & `tsugu-1.0.0rc1/tsugu/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu/universal/router/ycx_all.py` & `tsugu-1.0.0rc1/tsugu/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu.egg-info/PKG-INFO` & `tsugu-1.0.0rc1/tsugu.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,123 +1,89 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.9.9rc9
+Version: 1.0.0rc1
 Summary: Tsugu Python Frontend
-Home-page: https://github.com/kumoSleeping/tsugu-bot-py
+Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
-        <h1 align="center"> Tsugu Bot Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
+        <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
         
         
-        <p align="center">
+        <div align="center">
+        
+        _✨ Python 编写的 [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-bot?tab=readme-ov-file) 自然语言交互库  ✨_
+        
+        </div>
         
+        <p align="center">
         <a href="https://github.com/Yamamoto-2/tsugu-bangdream-bot">
-            <img src="https://img.shields.io/badge/tsugubangdream bot - v2 api-yellow" alt="license">
+            <img src="https://img.shields.io/badge/tsugubangdream bot - api-yellow" alt="license">
           </a>
         
         <a href="https://github.com/kumoSleeping/tsugu-python-frontend?tab=MIT-1-ov-file">
             <img src="https://img.shields.io/github/license/kumoSleeping/tsugu-python-frontend" alt="license">
           </a>
         <a href="https://pypi.org/project/tsugu/">
             <img src="https://img.shields.io/pypi/v/tsugu.svg" alt="license">
           </a>
         </p>
         
-        
-        ***
-        
-        
-        - `tsugu`
-          - [x] 自然语言输入 -> 返回结果
-          - [x] 远程数据库 
-          - [x] 本地数据库 
-        
-        
-        - `tsugu.async`
-          - [x] 自然语言输入 -> 返回结果
-          - [x] 远程数据库 
-          - [ ] 本地数据库
-        
-        
-        
+        ---
         
         
         ```shell
         pip install tsugu
         ```
-        > Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
-        
         
-        ***
         
+        > Powered by  <a href="https://github.com/WindowsSov8forUs/tsugu-api-python?tab=readme-ov-file">tsugu-api-python</a>
         
-        <h2 align="center"> 测试与调用 </h2>
+        ***
         
         ## handler
         
-        - `handler` 是 `tsugu` 的一个同步函数，用于直接处理用户输入的自然语言并返回查询结果: 
+        - `handler` 用于直接处理用户输入的自然语言并返回查询结果: 
         
         ```python
         import tsugu
         
-        # tsugu.database(path="./data.db")
-        
         # 四个参数，分别意味着 消息内容 用户id 平台 频道id
         for i in tsugu.handler(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414'):
             print('文本: ',i) if isinstance(i, str) else None
             print(f"[图片]") if isinstance(i, bytes) else None
         ```
         
         ```python
         import tsugu_async
-        
-        # tsugu_async.config.reload_from_json('./config.json')
-        
-        async def main():
-            res = await tsugu_async.handler(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414')
-            for i in res:
-                print('文本: ',i) if isinstance(i, str) else None
-                print(f"[图片]") if isinstance(i, bytes) else None
+        ...
         ```
         
         
         > 在常用的qqbot中，群号就是 `channel_id`。   
         > 当你使用QQ号作为 `user_id` 时，`platform` 可以填写 `red`。   
         
         ## handler_raw
         如果你方便使用 base64，`handler_raw` 方法或许会更好  
-        `tsugu` 后端本身返回此数据结构，如果你的bot可以直接发送 `base64` 类图片，这个方法会节省不必要的开销。
+        `tsugu` 后端本身返回此数据结构，这个方法可以节省不必要的开销。
         
         ```python
         import tsugu
         
         for i in tsugu.handler_raw(message='查卡 ars 1x', user_id='1528593481', platform='red', channel_id='666808414'):
             print('文本: ',i) if i['type'] == 'text' else None
             print(f"[图片]") if i['type'] == 'base64' else None
-        
-        
+        ```
+        ```python
         import tsugu_async
         ...
         ```
         
         
-        ## 使用本地数据库(不支持`tsugu_async`)
-        本地数据库由 `sqlite3` 提供，你可以使用 `tsugu.database` 来创建或使用本地数据库。
-        
-        ```py
-        import tsugu
-        
-        tsugu.database(path="./data.db")
-        ```
-        
-        > 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。  
-        > 远程数据库将不使用。
-        
         ## 配置
         
         
         > 随意更改配置项可能会导致不可预知的错误。
         
         ### tsugu_api settings
         
@@ -225,72 +191,25 @@
         ```
         
         
         
         ***
         
          <details>
-        <summary><b>客服ano酱指导(这里可以点击)</b></summary>
+        <summary><b>客服🐱指导(这里可以点击)</b></summary>
          
         **注意，如果你不知道什么是BanGDream，请不要随意加群**    
         **本群还是欢迎加群的（**    
         [BanGDreamBot开发聊天群](https://qm.qq.com/q/zjUPQkrdpm)   
         温馨的聊天环境～   
         
         </details>
         
         
-        下方已无内容。
-        
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
-        <br/>
+        ---
         
-        🐱: 喵
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,42 +1,29 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.9.9rc9 Summary: Tsugu Python
-Frontend Home-page: https://github.com/kumoSleeping/tsugu-bot-py Author:
+Metadata-Version: 2.1 Name: tsugu Version: 1.0.0rc1 Summary: Tsugu Python
+Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
-                       ************ TTssuugguu BBoott PPyy[[ttmmrrnn]] ************
+                       ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
+_â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
+         bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
-*** - `tsugu` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ - [x] è¿ç¨æ°æ®åº -
-[x] æ¬å°æ°æ®åº - `tsugu.async` - [x] èªç¶è¯­è¨è¾å¥ -> è¿åç»æ -
-[x] è¿ç¨æ°æ®åº - [ ] æ¬å°æ°æ®åº ```shell pip install tsugu ``` >
-Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n ***
-                          ********** ?æ?µ??è?¯??ä?¸??è?°??ç??¨ **********
-## handler - `handler` æ¯ `tsugu`
-çä¸ä¸ªåæ­¥å½æ°ï¼ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
-```python import tsugu # tsugu.database(path="./data.db") #
-åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id å¹³å° é¢éid for i in
-tsugu.handler(message='æ¥å¡ ars 1x', user_id='1528593481', platform='red',
-channel_id='666808414'): print('ææ¬: ',i) if isinstance(i, str) else None
-print(f"[å¾ç]") if isinstance(i, bytes) else None ``` ```python import
-tsugu_async # tsugu_async.config.reload_from_json('./config.json') async def
-main(): res = await tsugu_async.handler(message='æ¥å¡ ars 1x',
-user_id='1528593481', platform='red', channel_id='666808414') for i in res:
-print('ææ¬: ',i) if isinstance(i, str) else None print(f"[å¾ç]") if
-isinstance(i, bytes) else None ``` > å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯
-`channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º `user_id` æ¶ï¼`platform`
-å¯ä»¥å¡«å `red`ã ## handler_raw å¦æä½ æ¹ä¾¿ä½¿ç¨
-base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
-åç«¯æ¬èº«è¿åæ­¤æ°æ®ç»æï¼å¦æä½ çbotå¯ä»¥ç´æ¥åé `base64`
-ç±»å¾çï¼è¿ä¸ªæ¹æ³ä¼èçä¸å¿è¦çå¼éã ```python import tsugu
-for i in tsugu.handler_raw(message='æ¥å¡ ars 1x', user_id='1528593481',
-platform='red', channel_id='666808414'): print('ææ¬: ',i) if i['type'] ==
-'text' else None print(f"[å¾ç]") if i['type'] == 'base64' else None import
-tsugu_async ... ``` ## ä½¿ç¨æ¬å°æ°æ®åº(ä¸æ¯æ`tsugu_async`)
-æ¬å°æ°æ®åºç± `sqlite3` æä¾ï¼ä½ å¯ä»¥ä½¿ç¨ `tsugu.database`
-æ¥åå»ºæä½¿ç¨æ¬å°æ°æ®åºã ```py import tsugu tsugu.database(path="./
-data.db") ``` > æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
-æä¾ç¨æ·æ°æ®ã > è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã ## éç½® >
+--- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
+- `handler` ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
+```python import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id
+å¹³å° é¢éid for i in tsugu.handler(message='æ¥å¡ ars 1x',
+user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
+',i) if isinstance(i, str) else None print(f"[å¾ç]") if isinstance(i, bytes)
+else None ``` ```python import tsugu_async ... ``` >
+å¨å¸¸ç¨çqqbotä¸­ï¼ç¾¤å·å°±æ¯ `channel_id`ã > å½ä½ ä½¿ç¨QQå·ä½ä¸º
+`user_id` æ¶ï¼`platform` å¯ä»¥å¡«å `red`ã ## handler_raw
+å¦æä½ æ¹ä¾¿ä½¿ç¨ base64ï¼`handler_raw` æ¹æ³æè®¸ä¼æ´å¥½ `tsugu`
+åç«¯æ¬èº«è¿åæ­¤æ°æ®ç»æï¼è¿ä¸ªæ¹æ³å¯ä»¥èçä¸å¿è¦çå¼éã
+```python import tsugu for i in tsugu.handler_raw(message='æ¥å¡ ars 1x',
+user_id='1528593481', platform='red', channel_id='666808414'): print('ææ¬:
+',i) if i['type'] == 'text' else None print(f"[å¾ç]") if i['type'] ==
+'base64' else None ``` ```python import tsugu_async ... ``` ## éç½® >
 éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api
 settings ```py from tsugu_api import settings settings.timeout = 10 '''
 è¯·æ±è¶æ¶æ¶é´ ''' settings.proxy = '' ''' ä»£çå°å '''
 settings.backend_url = 'http://tsugubot.com:8080' ''' åç«¯å°å é»è®¤ä¸º
 Tsugu å®æ¹åç«¯ï¼è¥æèªå»ºåç«¯æå¡å¨å¯è¿è¡ä¿®æ¹ã '''
 settings.backend_proxy = True ''' æ¯å¦ä½¿ç¨åç«¯ä»£ç
 å½è®¾ç½®ä»£çå°ååå¯ä¿®æ¹æ­¤é¡¹ä»¥å³å®æ¯å¦ä½¿ç¨ä»£çã é»è®¤ä¸º
@@ -61,60 +48,15 @@
 ''' config.allow_gap_less = True '''
 æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
 config.get_remote_user_data_max_retry = 3 '''
 è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ° ''' config.token_name = "Tsugu" '''
 bandori station token ''' config.bandori_station_token = "ZtV4EX2K9Onb" '''
 bandori station token ''' config.ban_gacha_simulate_group_data = [] '''
 éè¦å³é­æ¨¡ææ½å¡çç¾¤ ''' config.commands = ... config.user_commands =
-... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼
+... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ???ð???±?æ???å?¯?¼
 ((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
-qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ ä¸æ¹å·²æ åå®¹ã
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-ð±: åµ Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
-markdown
+qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ --- Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/command_matcher/__init__.py` & `tsugu-1.0.0rc1/tsugu_async/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu_async/config.py` & `tsugu-1.0.0rc1/tsugu_async/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu_async/handler.py` & `tsugu-1.0.0rc1/tsugu/handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 import base64
 from typing import List, Union, Dict
 
 from .utils import *
-from . import remote
 from loguru import logger
-from tsugu_api import settings
+from . import router
 
-
-async def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
+def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Union[bytes, str]]
     '''
-    data = await handler_raw(message, user_id, platform, channel_id)
-    response = []
-    if not data:
+    try:
+        data = handler_raw(message, user_id, platform, channel_id)
+        response = []
+        if not data:
+            return response
+        for item in data:
+            response.append(item['string']) if item['type'] == 'string' else None
+            response.append(base64.b64decode(item['string'].encode('utf-8')) if item['type'] == 'base64' else None)
         return response
-    for item in data:
-        response.append(item['string']) if item['type'] == 'string' else None
-        response.append(base64.b64decode(item['string'].encode('utf-8')) if item['type'] == 'base64' else None)
-    return response
+    except Exception as e:
+        raise e
 
 
-async def handler_raw(message: str, user_id: str, platform: str, channel_id: str) -> List[Dict[str, str]]:
+def handler_raw(message: str, user_id: str, platform: str, channel_id: str) -> List[Dict[str, str]]:
     '''
     handler_raw 除了返回的数据类型不同外，其他与 handler 函数一致
     返回格式为 Tsugu 标准数据格式
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Dict[str, str]]
     '''
     try:
-        # 使用远程服务器
-        res = await remote.handler(message, user_id, platform, channel_id)
-        if not res:
-            return []
-        return res
+        return r if (r := router.handler(message, user_id, platform, channel_id)) else None
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/change_server_mode.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from ...config import config
 from ...utils import text_response, User
 from ...command_matcher import MC
 import tsugu_api_async
 from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
+from tsugu_api._typing import _ServerId, _Update
+import typing
 
 
 async def handler(user: User, res: MC, platform: str, channel_id: str):
     if res.args:
-        server_pre = server_name_2_server_id(res.args[0])
-        if not server_exists(server_pre):
+        server_mode = server_name_2_server_id(res.args[0])
+        if not server_exists(server_mode):
             return text_response('未找到服务器，请输入正确的服务器名')
-        user.server_mode = server_pre
-    # 获取绑定请求
-    r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, True)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    return text_response(
-        f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 你的玩家ID(数字) {server_id_2_server_name(user.server_mode)}\n''')
+        update: _Update = {'server_mode': server_mode, }
+        r = await tsugu_api_async.change_user_data(platform, user.user_id, update)
+        if r:
+            if r.get('status') == 'success':
+                return text_response('主服务器已设置为 ' + server_id_2_server_name(server_mode))
+            return text_response(r.get('data'))
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_off.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player_verification_off.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 from ...command_matcher import MC
 import tsugu_api_async
 from ...utils import server_exists, server_name_2_server_id
 from loguru import logger
 
 
 async def handler(user: User, res: MC, platform: str, channel_id: str):
-    if not res.args:
-        return text_response('请输入正确的服务器名参数')
-    server_pre = server_name_2_server_id(res.args[0])
-    if not server_exists(server_pre):
-        return text_response('未找到服务器，请输入正确的服务器名')
-    player_id = int(user.server_list[server_pre]['playerId'])
-
-    r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server_pre, player_id, False)
+    if not res.args or len(res.args) > 1:
+        return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
+    if not res.args[0].isdigit():
+        return text_response('请输入正确的格式：验证解绑 记录编号(数字)')
+    if int(res.text) <= 0:
+        return text_response('请输入正确的格式：验证解绑 记录编号(数字)，编号从1开始')
+    if len(user.game_ids) < int(res.text):
+        return text_response('未找到记录')
+    player_id = user.game_ids[int(res.args[0]) - 1].get("game_id")
+    server_mode = user.game_ids[int(res.args[0]) - 1].get("server")
+    r = await tsugu_api_async.bind_player_verification(platform, user.user_id, server_mode, player_id, False)
     if r.get('status') != 'success':
-        logger.error(r.get('data'))
         return text_response(r.get('data'))
-    return text_response('解绑成功')
+    return text_response('解绑成功！')
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_on.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/ycx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 from ...config import config
-from ...utils import text_response, User
+from ...utils import text_response, User, server_exists, server_name_2_server_id
 from ...command_matcher import MC
 import tsugu_api_async
-from ...utils import server_exists, server_name_2_server_id
 
 
 async def handler(user: User, res: MC, platform: str, channel_id: str):
+    # 无参数
     if not res.args:
-        return text_response('请输入正确的玩家ID和服务器名参数(可选)')
-    if not res.args[0].isdigit():
-        return text_response('请输入正确的玩家ID')
-    player_id = int(res.args[0])
-    if len(res.args) > 1:
-        server_pre = server_name_2_server_id(res.args[1])
-        if not server_exists(server_pre):
-            return text_response('未找到服务器，请输入正确的服务器名')
-        user.server_mode = server_pre
-
-    r = await tsugu_api_async.bind_player_verification(platform, user.user_id, user.server_mode, player_id, True)
-    if r.get('status') != 'success':
-        return text_response(r.get('data'))
-    return text_response('绑定成功')
-
-    # 车牌转发控制
+        return text_response('请输入档位线')
 
+    # 一个参数
+    if res.args[0].isdigit():
+        tier: int = int(res.args[0])
+    else:
+        return text_response('请输入正确的档位线')
+
+    if len(res.args) == 1:
+        return await tsugu_api_async.ycx(user.server_mode, tier)
+
+    # 两个参数
+    if len(res.args) == 2:
+        # 两个参数都是数字
+        if res.args[1].isdigit():
+            if res.args[1].isdigit():
+                event_id: int = int(res.args[1])
+            else:
+                return text_response('请输入正确的活动ID')
+            return await tsugu_api_async.ycx(user.server_mode, tier, event_id)
+        elif server_exists(server_pre := server_name_2_server_id(res.args[1])):
+            user.server_mode = server_pre
+            return await tsugu_api_async.ycx(user.server_mode, tier)
+        else:
+            return text_response('请输入正确的活动ID或服务器名称字母简写')
+
+    if len(res.args) == 3:
+        # 三个参数是 tier event_id server_mode
+        if res.args[1].isdigit():
+            if res.args[1].isdigit():
+                event_id: int = int(res.args[1])
+            else:
+                return text_response('第二个参数请输入正确的活动ID')
+            if server_exists(server_pre := server_name_2_server_id(res.args[2])):
+                user.server_mode = server_pre
+                return await tsugu_api_async.ycx(user.server_mode, tier, event_id)
+            else:
+                return text_response('第三个参数请输入正确的服务器名称字母简写')
 
+    return text_response('参数过多(<=3)')
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/remote/router/change_default_server.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/song_chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from ...config import config
 from ...utils import text_response, User
 from ...command_matcher import MC
 import tsugu_api_async
-from ...utils import server_exists, server_names_2_server_ids
-from tsugu_api._typing import _Update
+
+from tsugu_api._typing import _DifficultyText
 
 
 async def handler(user: User, res: MC, platform: str, channel_id: str):
-    default_server = server_names_2_server_ids(res.args)
-    if not default_server:
-        return text_response('未找到服务器，请输入正确的服务器名')
-    change_data: _Update = {'default_server': default_server}
-    r = await tsugu_api_async.change_user_data(platform, user.user_id, change_data)
-    if r.get('status') == 'success':
-        return text_response(f'默认服务器已设置为 {", ".join(res.args)}')
-    return text_response(r.get('data'))
+    if not res.args:
+        return text_response('请输入查询参数: 歌曲ID')
+    if not res.args[0].isdigit():
+        return text_response('请输入正确的歌曲ID(数字)')
+    if len(res.args) > 1:
+        # 难度符合 _DifficultyText
+        if not res.args[1] in ['easy', 'normal', 'hard', 'expert', 'special']:
+            return text_response(f'请输入正确的难度(easy, normal, hard, expert, special)')
+        return await tsugu_api_async.song_chart(user.default_server, int(res.args[0]), res.args[1])
+    elif len(res.args) == 1:
+        difficulty: _DifficultyText = 'expert'
+        return await tsugu_api_async.song_chart(user.default_server, int(res.args[0]), difficulty)
+    return text_response('参数错误')
+
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/remote/router/unbind_player.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,15 @@
+from ...config import config
 from ...utils import text_response, User
 from ...command_matcher import MC
 import tsugu_api_async
 from ...utils import server_exists, server_name_2_server_id, server_id_2_server_name
 
 
 async def handler(user: User, res: MC, platform: str, channel_id: str):
-    if res.args:
-        server_pre = server_name_2_server_id(res.args[0])
-        if not server_exists(server_pre):
-            return text_response('未找到服务器，请输入正确的服务器名')
-        user.server_mode = server_pre
-        if not user.server_list[user.server_mode]['playerId']:
-            return text_response('未绑定玩家，请先绑定玩家')
-    r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, False)
+    # 获取绑定请求
+    r = await tsugu_api_async.bind_player_request(platform, user.user_id, user.server_mode, True)
     if r.get('status') != 'success':
         return text_response(r.get('data'))
-    # 如果是200
     return text_response(
-        f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {server_id_2_server_name(user.server_mode)}\n来完成本次身份验证''')
-
+        f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{r.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证绑定 你的玩家ID(数字) 服务器名(字母缩写)\n例如：验证绑定 114****514 cn''')
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/universal/help.py` & `tsugu-1.0.0rc1/tsugu_async/router/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu_async/universal/rooms_forward.py` & `tsugu-1.0.0rc1/tsugu_async/router/rooms_forward.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import tsugu_api_async
 
 from ..utils import config
 import re
 from ..utils import User, text_response
 from ..command_matcher import MC
 from loguru import logger
-
-
-from ..storage.remote_db import get_user
+from ..utils import get_user
 
 
 async def submit_rooms(res: MC, user_id, platform=None):
     message = res.text
     # 检查car_config['car']中的关键字
     for keyword in config._car_config["car"]:
         if str(keyword) in message:
@@ -39,16 +37,19 @@
         # 默认不开启关闭车牌，继续提交
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
-
-        await tsugu_api_async.submit_room_number(int(car_id), user.user_id, message, config.token_name, config.bandori_station_token)
+        if user.user_id.isdigit():
+            car_user_id = '3889000770'
+        else:
+            car_user_id = user.user_id
+        await tsugu_api_async.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source=config.token_name, token=config.bandori_station_token)
         return []
     except Exception as e:
         logger.error(f"[Tsugu] 发生异常: {e}")
         return []  # 虽然提交失败，但是确定了是车牌消息
```

### Comparing `tsugu-0.9.9rc9/tsugu_async/universal/router/__init__.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu_async/universal/router/gacha_simulate.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu_async/universal/router/lsycx.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu_async/universal/router/search_player.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc9/tsugu_async/universal/router/song_chart.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/ycx_all.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 from ...config import config
-from ...utils import text_response, User
+from ...utils import text_response, User, server_exists, server_name_2_server_id
 from ...command_matcher import MC
 import tsugu_api_async
 
-from tsugu_api._typing import _DifficultyText
-
 
 async def handler(user: User, res: MC, platform: str, channel_id: str):
+    # 无参数
     if not res.args:
-        return text_response('请输入查询参数: 歌曲ID')
-    if not res.args[0].isdigit():
-        return text_response('请输入正确的歌曲ID(数字)')
-    if len(res.args) > 1:
-        # 难度符合 _DifficultyText
-        if not res.args[1] in ['easy', 'normal', 'hard', 'expert', 'special']:
-            return text_response(f'请输入正确的难度(easy, normal, hard, expert, special)')
-        return await tsugu_api_async.song_chart(user.default_server, int(res.args[0]), res.args[1])
-    elif len(res.args) == 1:
-        difficulty: _DifficultyText = 'expert'
-        return await tsugu_api_async.song_chart(user.default_server, int(res.args[0]), difficulty)
-    return text_response('参数错误')
+        return await tsugu_api_async.ycx_all(user.server_mode)
+
+    # 一个参数
+    if len(res.args) == 1:
+        # 两个参数都是数字
+        if res.args[0].isdigit():
+            if res.args[0].isdigit():
+                event_id: int = int(res.args[0])
+            else:
+                return text_response('请输入正确的活动ID')
+            return await tsugu_api_async.ycx_all(user.server_mode, event_id)
+        elif server_exists(server_pre := server_name_2_server_id(res.args[0])):
+            user.server_mode = server_pre
+            return await tsugu_api_async.ycx_all(user.server_mode)
+        else:
+            return text_response('请输入正确的活动ID或服务器名称字母简写')
+
+    if len(res.args) == 2:
+        # 两个参数是 event_id server_mode
+        if res.args[0].isdigit():
+            event_id: int = int(res.args[0])
+        else:
+            return text_response('第一个参数请输入正确的活动ID')
+        if server_exists(server_pre := server_name_2_server_id(res.args[1])):
+            user.server_mode = server_pre
+            return await tsugu_api_async.ycx_all(user.server_mode, event_id)
+        else:
+            return text_response('第二个参数请输入正确的服务器名称字母简写')
 
+    return text_response('参数过多(<=2)')
```

