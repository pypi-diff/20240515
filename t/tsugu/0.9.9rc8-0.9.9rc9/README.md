# Comparing `tmp/tsugu-0.9.9rc8.tar.gz` & `tmp/tsugu-0.9.9rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.9.9rc8.tar", last modified: Tue May 14 08:53:12 2024, max compression
+gzip compressed data, was "tsugu-0.9.9rc9.tar", last modified: Tue May 14 10:19:54 2024, max compression
```

## Comparing `tsugu-0.9.9rc8.tar` & `tsugu-0.9.9rc9.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.862371 tsugu-0.9.9rc8/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-14 08:53:12.862371 tsugu-0.9.9rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:53:12.862371 tsugu-0.9.9rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.846371 tsugu-0.9.9rc8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.846371 tsugu-0.9.9rc8/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.846371 tsugu-0.9.9rc8/tsugu/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.846371 tsugu-0.9.9rc8/tsugu/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.850371 tsugu-0.9.9rc8/tsugu/local/router/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/local/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.850371 tsugu-0.9.9rc8/tsugu/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.850371 tsugu-0.9.9rc8/tsugu/remote/router/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/remote/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.850371 tsugu-0.9.9rc8/tsugu/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.850371 tsugu-0.9.9rc8/tsugu/storage/db/
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/storage/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.850371 tsugu-0.9.9rc8/tsugu/storage/remote_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/storage/remote_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.854371 tsugu-0.9.9rc8/tsugu/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/rooms_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.854371 tsugu-0.9.9rc8/tsugu/universal/router/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/universal/router/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.854371 tsugu-0.9.9rc8/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.846371 tsugu-0.9.9rc8/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-14 08:53:12.000000 tsugu-0.9.9rc8/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-14 08:53:12.000000 tsugu-0.9.9rc8/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:53:12.000000 tsugu-0.9.9rc8/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 08:53:12.000000 tsugu-0.9.9rc8/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 08:53:12.000000 tsugu-0.9.9rc8/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.854371 tsugu-0.9.9rc8/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.854371 tsugu-0.9.9rc8/tsugu_async/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.854371 tsugu-0.9.9rc8/tsugu_async/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.858371 tsugu-0.9.9rc8/tsugu_async/remote/router/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/remote/router/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.858371 tsugu-0.9.9rc8/tsugu_async/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.858371 tsugu-0.9.9rc8/tsugu_async/storage/remote_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/storage/remote_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.858371 tsugu-0.9.9rc8/tsugu_async/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/rooms_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.862371 tsugu-0.9.9rc8/tsugu_async/universal/router/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/universal/router/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:53:12.862371 tsugu-0.9.9rc8/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 08:53:01.000000 tsugu-0.9.9rc8/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.231572 tsugu-0.9.9rc9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.231572 tsugu-0.9.9rc9/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/local/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/local/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/remote/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/remote/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/storage/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/storage/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/storage/remote_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/storage/remote_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/universal/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/universal/router/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.235572 tsugu-0.9.9rc9/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 10:19:54.000000 tsugu-0.9.9rc9/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.239572 tsugu-0.9.9rc9/tsugu_async/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/remote/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/remote/router/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/storage/remote_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/storage/remote_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.243572 tsugu-0.9.9rc9/tsugu_async/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/rooms_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/tsugu_async/universal/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/universal/router/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:19:54.247572 tsugu-0.9.9rc9/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-14 10:19:46.000000 tsugu-0.9.9rc9/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-0.9.9rc8/LICENSE` & `tsugu-0.9.9rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/README.md` & `tsugu-0.9.9rc9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -104,37 +104,121 @@
 ```
 
 > 此操作会自动创建或使用本地数据库为 tsugu.bot 提供用户数据。  
 > 远程数据库将不使用。
 
 ## 配置
 
+
+> 随意更改配置项可能会导致不可预知的错误。
+
+### tsugu_api settings
+
 ```py
-import tsugu
+from tsugu_api import settings
 
-tsugu.config.reload_from_json('./config.json')
-```
-> 如果不存在，会创建默认配置文件。
+settings.timeout = 10
+'''
+请求超时时间
+'''
+
+settings.proxy = ''
+'''
+代理地址
+'''
+
+settings.backend_url = 'http://tsugubot.com:8080'
+'''
+后端地址
+默认为 Tsugu 官方后端，若有自建后端服务器可进行修改。
+'''
+
+settings.backend_proxy = True
+'''
+是否使用后端代理
+当设置代理地址后可修改此项以决定是否使用代理。
+默认为 True，即使用后端代理。若使用代理时后端服务器无法访问，可将此项设置为 False。
+'''
+
+settings.userdata_backend_url = 'http://tsugubot.com:8080'
+'''
+用户数据后端地址
+默认为 Tsugu 官方后端，若有自建后端服务器可进行修改。
+'''
+
+settings.userdata_backend_proxy = True
+'''
+是否使用用户数据后端代理
+当设置代理地址后可修改此项以决定是否使用代理。
+默认为 True，即使用后端代理。若使用代理时后端服务器无法访问，可将此项设置为 False。
+'''
+
+settings.use_easy_bg = True
+'''
+是否使用简易背景，使用可在降低背景质量的前提下加快响应速度。
+默认为 True，即使用简易背景。若不使用简易背景，可将此项设置为 False。
+'''
+
+settings.compress = True
+'''
+是否压缩返回数据，压缩可减少返回数据大小。
+默认为 True，即压缩返回数据。若不压缩返回数据，可将此项设置为 False。
+'''
 
-> 注意，不清楚的配置项请不要更改，更改配置项可能会导致不可预知的错误。
+```
 
+```py
+from tsugu_api_async import settings
+...
+```
 
-- 你也可以直接更改配置，但不推荐:   
+### tsugu_async config
 
 ```py
-import tsugu
+from tsugu import config
 
-# 更改的后端地址。
-tsugu.config.backend = "http://127.0.0.0.1:3000"
+config.prefix = ['/', '']
+'''
+命令前缀
+最后一个参数如果不是空字符串，则只有在命令前缀符合时才会触发命令。
+'''
+
+config.allow_gap_less = True
+'''
+是否允许命令与参数之间没有空格
+'''
+
+config.get_remote_user_data_max_retry = 3
+'''
+获取远程用户数据最大重试次数
+'''
+
+config.token_name = "Tsugu"
+'''
+bandori station token
+'''
+config.bandori_station_token = "ZtV4EX2K9Onb"
+'''
+bandori station token
+'''
+
+config.ban_gacha_simulate_group_data = []
+'''
+需要关闭模拟抽卡的群
+'''
 
-# 添加关闭抽卡模拟的群号。
-tsugu.config.ban_gacha_simulate_group_data = ["114514", "1919810"]
-```
+config.commands = ...
 
+config.user_commands = ...
+```
 
+```py
+from tsugu_async import config
+...
+```
 
 
 
 ***
 
  <details>
 <summary><b>客服ano酱指导(这里可以点击)</b></summary>
```

#### html2text {}

```diff
@@ -25,22 +25,49 @@
 for i in tsugu.handler_raw(message='æ¥å¡ ars 1x', user_id='1528593481',
 platform='red', channel_id='666808414'): print('ææ¬: ',i) if i['type'] ==
 'text' else None print(f"[å¾ç]") if i['type'] == 'base64' else None import
 tsugu_async ... ``` ## ä½¿ç¨æ¬å°æ°æ®åº(ä¸æ¯æ`tsugu_async`)
 æ¬å°æ°æ®åºç± `sqlite3` æä¾ï¼ä½ å¯ä»¥ä½¿ç¨ `tsugu.database`
 æ¥åå»ºæä½¿ç¨æ¬å°æ°æ®åºã ```py import tsugu tsugu.database(path="./
 data.db") ``` > æ­¤æä½ä¼èªå¨åå»ºæä½¿ç¨æ¬å°æ°æ®åºä¸º tsugu.bot
-æä¾ç¨æ·æ°æ®ã > è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã ## éç½® ```py import
-tsugu tsugu.config.reload_from_json('./config.json') ``` >
-å¦æä¸å­å¨ï¼ä¼åå»ºé»è®¤éç½®æä»¶ã >
-æ³¨æï¼ä¸æ¸æ¥çéç½®é¡¹è¯·ä¸è¦æ´æ¹ï¼æ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã
-- ä½ ä¹å¯ä»¥ç´æ¥æ´æ¹éç½®ï¼ä½ä¸æ¨è: ```py import tsugu #
-æ´æ¹çåç«¯å°åã tsugu.config.backend = "http://127.0.0.0.1:3000" #
-æ·»å å³é­æ½å¡æ¨¡æçç¾¤å·ã tsugu.config.ban_gacha_simulate_group_data
-= ["114514", "1919810"] ``` *** ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
+æä¾ç¨æ·æ°æ®ã > è¿ç¨æ°æ®åºå°ä¸ä½¿ç¨ã ## éç½® >
+éææ´æ¹éç½®é¡¹å¯è½ä¼å¯¼è´ä¸å¯é¢ç¥çéè¯¯ã ### tsugu_api
+settings ```py from tsugu_api import settings settings.timeout = 10 '''
+è¯·æ±è¶æ¶æ¶é´ ''' settings.proxy = '' ''' ä»£çå°å '''
+settings.backend_url = 'http://tsugubot.com:8080' ''' åç«¯å°å é»è®¤ä¸º
+Tsugu å®æ¹åç«¯ï¼è¥æèªå»ºåç«¯æå¡å¨å¯è¿è¡ä¿®æ¹ã '''
+settings.backend_proxy = True ''' æ¯å¦ä½¿ç¨åç«¯ä»£ç
+å½è®¾ç½®ä»£çå°ååå¯ä¿®æ¹æ­¤é¡¹ä»¥å³å®æ¯å¦ä½¿ç¨ä»£çã é»è®¤ä¸º
+Trueï¼å³ä½¿ç¨åç«¯ä»£çãè¥ä½¿ç¨ä»£çæ¶åç«¯æå¡å¨æ æ³è®¿é®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
+Falseã ''' settings.userdata_backend_url = 'http://tsugubot.com:8080' '''
+ç¨æ·æ°æ®åç«¯å°å é»è®¤ä¸º Tsugu
+å®æ¹åç«¯ï¼è¥æèªå»ºåç«¯æå¡å¨å¯è¿è¡ä¿®æ¹ã '''
+settings.userdata_backend_proxy = True ''' æ¯å¦ä½¿ç¨ç¨æ·æ°æ®åç«¯ä»£ç
+å½è®¾ç½®ä»£çå°ååå¯ä¿®æ¹æ­¤é¡¹ä»¥å³å®æ¯å¦ä½¿ç¨ä»£çã é»è®¤ä¸º
+Trueï¼å³ä½¿ç¨åç«¯ä»£çãè¥ä½¿ç¨ä»£çæ¶åç«¯æå¡å¨æ æ³è®¿é®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
+Falseã ''' settings.use_easy_bg = True '''
+æ¯å¦ä½¿ç¨ç®æèæ¯ï¼ä½¿ç¨å¯å¨éä½èæ¯è´¨éçåæä¸å å¿«ååºéåº¦ã
+é»è®¤ä¸º
+Trueï¼å³ä½¿ç¨ç®æèæ¯ãè¥ä¸ä½¿ç¨ç®æèæ¯ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
+Falseã ''' settings.compress = True '''
+æ¯å¦åç¼©è¿åæ°æ®ï¼åç¼©å¯åå°è¿åæ°æ®å¤§å°ã é»è®¤ä¸º
+Trueï¼å³åç¼©è¿åæ°æ®ãè¥ä¸åç¼©è¿åæ°æ®ï¼å¯å°æ­¤é¡¹è®¾ç½®ä¸º
+Falseã ''' ``` ```py from tsugu_api_async import settings ... ``` ###
+tsugu_async config ```py from tsugu import config config.prefix = ['/', ''] '''
+å½ä»¤åç¼
+æåä¸ä¸ªåæ°å¦æä¸æ¯ç©ºå­ç¬¦ä¸²ï¼ååªæå¨å½ä»¤åç¼ç¬¦åæ¶æä¼è§¦åå½ä»¤ã
+''' config.allow_gap_less = True '''
+æ¯å¦åè®¸å½ä»¤ä¸åæ°ä¹é´æ²¡æç©ºæ ¼ '''
+config.get_remote_user_data_max_retry = 3 '''
+è·åè¿ç¨ç¨æ·æ°æ®æå¤§éè¯æ¬¡æ° ''' config.token_name = "Tsugu" '''
+bandori station token ''' config.bandori_station_token = "ZtV4EX2K9Onb" '''
+bandori station token ''' config.ban_gacha_simulate_group_data = [] '''
+éè¦å³é­æ¨¡ææ½å¡çç¾¤ ''' config.commands = ... config.user_commands =
+... ``` ```py from tsugu_async import config ... ``` *** ?å?®?¢?æ??aannoo?é??±?æ???å?¯?¼
+((?è?¿??é???å??¯?ä?»?¥?ç??¹?å??»))
 **æ³¨æï¼å¦æä½ ä¸ç¥éä»ä¹æ¯BanGDreamï¼è¯·ä¸è¦éæå ç¾¤**
 **æ¬ç¾¤è¿æ¯æ¬¢è¿å ç¾¤çï¼** [BanGDreamBotå¼åèå¤©ç¾¤](https://
 qm.qq.com/q/zjUPQkrdpm) æ¸©é¦¨çèå¤©ç¯å¢ï½ ä¸æ¹å·²æ åå®¹ã
```

### Comparing `tsugu-0.9.9rc8/setup.py` & `tsugu-0.9.9rc9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.9.9-rc8',
+    version='0.9.9-rc9',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bot-py',
```

### Comparing `tsugu-0.9.9rc8/test/test_async.py` & `tsugu-0.9.9rc9/test/test_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,20 @@
                     print(f"[图片信息]")
                     img = Image.open(io.BytesIO(i))
                     img.show()
                     print(f"[图像大小: {len(i) / 1024:.2f}KB]")
 
         # tsugu.database('./user_data.db')
         # tsugu_async.config.reload_from_json('./config.json')
+        # from tsugu_api_async import settings
+        # settings.backend_url = 'http://127.0.0.1:8010'
+        # from tsugu_async import config
+        # config.allow_gap_less = True
 
-        msg1 = await tsugu_async.handler('wdf', '1528593481', 'red', '666808414')
+        msg1 = await tsugu_async.handler('查卡ksm', '1528593481', 'red', '666808414')
         await show_back_msg(msg1)
 
         # msg2 = await tsugu_async.handler('ycm', '1528593481', 'red', '666808414')
         # await show_back_msg(msg2)
 
         # msg3 = await tsugu_async.handler('12324 测q1试', '1528593481', 'red', '666808414')
         # await show_back_msg(msg3)
```

### Comparing `tsugu-0.9.9rc8/tsugu/command_matcher/__init__.py` & `tsugu-0.9.9rc9/tsugu/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/handler.py` & `tsugu-0.9.9rc9/tsugu/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from .utils import *
 from .utils import text_response
 from . import remote
 from . import local
 from .utils import config
 from loguru import logger
+from tsugu_api import settings
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
@@ -37,19 +38,21 @@
     :param message: 用户消息
     :param user_id: 用户ID
     :param platform: 平台名称 一般为 red
     :param channel_id: 频道ID / 群号
     :return: List[Dict[str, str]]
     '''
     try:
-        # 如果启用了本地数据库
+        # 如果启用了本地数库
         if config._user_database_path:
             return r if (r := local.handler(message, user_id, platform, channel_id)) else None
         # 否则使用远程服务器
         return r if (r := remote.handler(message, user_id, platform, channel_id)) else None
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
 
 
 
 
+
+
```

### Comparing `tsugu-0.9.9rc8/tsugu/local/__init__.py` & `tsugu-0.9.9rc9/tsugu/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/local/router/bind_player.py` & `tsugu-0.9.9rc9/tsugu/local/router/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/local/router/bind_player_verification_on.py` & `tsugu-0.9.9rc9/tsugu/local/router/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/local/router/change_default_server.py` & `tsugu-0.9.9rc9/tsugu/local/router/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/local/router/change_server_mode.py` & `tsugu-0.9.9rc9/tsugu/local/router/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/local/router/player_status.py` & `tsugu-0.9.9rc9/tsugu/local/router/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/local/router/unbind_player.py` & `tsugu-0.9.9rc9/tsugu/local/router/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/__init__.py` & `tsugu-0.9.9rc9/tsugu/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/router/bind_player.py` & `tsugu-0.9.9rc9/tsugu/remote/router/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/router/bind_player_verification_off.py` & `tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/router/bind_player_verification_on.py` & `tsugu-0.9.9rc9/tsugu/remote/router/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/router/change_default_server.py` & `tsugu-0.9.9rc9/tsugu/remote/router/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/router/change_server_mode.py` & `tsugu-0.9.9rc9/tsugu/remote/router/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/router/player_status.py` & `tsugu-0.9.9rc9/tsugu/remote/router/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/remote/router/unbind_player.py` & `tsugu-0.9.9rc9/tsugu/remote/router/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/storage/db/__init__.py` & `tsugu-0.9.9rc9/tsugu/storage/db/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/storage/remote_db/__init__.py` & `tsugu-0.9.9rc9/tsugu/storage/remote_db/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/__init__.py` & `tsugu-0.9.9rc9/tsugu/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/help.py` & `tsugu-0.9.9rc9/tsugu/universal/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/rooms_forward.py` & `tsugu-0.9.9rc9/tsugu/universal/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/__init__.py` & `tsugu-0.9.9rc9/tsugu/universal/router/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/event_stage.py` & `tsugu-0.9.9rc9/tsugu/universal/router/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/gacha_simulate.py` & `tsugu-0.9.9rc9/tsugu/universal/router/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/lsycx.py` & `tsugu-0.9.9rc9/tsugu/universal/router/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/search_player.py` & `tsugu-0.9.9rc9/tsugu/universal/router/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/song_chart.py` & `tsugu-0.9.9rc9/tsugu/universal/router/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/ycx.py` & `tsugu-0.9.9rc9/tsugu/universal/router/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/universal/router/ycx_all.py` & `tsugu-0.9.9rc9/tsugu/universal/router/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu/utils/__init__.py` & `tsugu-0.9.9rc9/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu.egg-info/SOURCES.txt` & `tsugu-0.9.9rc9/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/command_matcher/__init__.py` & `tsugu-0.9.9rc9/tsugu_async/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/handler.py` & `tsugu-0.9.9rc9/tsugu_async/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 from typing import List, Union, Dict
 
 from .utils import *
 from . import remote
 from loguru import logger
+from tsugu_api import settings
 
 
 async def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
     '''
     Tsugu Handler
     处理用户输入的自然语言，返回处理后的结果
 
@@ -46,7 +47,9 @@
     except Exception as e:
         logger.error(f'Error: {e}')
         raise e
 
 
 
 
+
+
```

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/__init__.py` & `tsugu-0.9.9rc9/tsugu_async/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/router/bind_player.py` & `tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/router/bind_player_verification_off.py` & `tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/router/bind_player_verification_on.py` & `tsugu-0.9.9rc9/tsugu_async/remote/router/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/router/change_default_server.py` & `tsugu-0.9.9rc9/tsugu_async/remote/router/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/router/change_server_mode.py` & `tsugu-0.9.9rc9/tsugu_async/remote/router/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/router/player_status.py` & `tsugu-0.9.9rc9/tsugu_async/remote/router/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/remote/router/unbind_player.py` & `tsugu-0.9.9rc9/tsugu_async/remote/router/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/storage/remote_db/__init__.py` & `tsugu-0.9.9rc9/tsugu_async/storage/remote_db/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/__init__.py` & `tsugu-0.9.9rc9/tsugu_async/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/help.py` & `tsugu-0.9.9rc9/tsugu_async/universal/help.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/rooms_forward.py` & `tsugu-0.9.9rc9/tsugu_async/universal/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/__init__.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/event_stage.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/event_stage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from ...config import config
 from ...utils import text_response, User, server_exists
 from ...command_matcher import MC
 import tsugu_api_async
 
-
 async def handler(user: User, res: MC, platform: str, channel_id: str):
     if res.args:
         #     最后一个参数
         # if server_exists(name_2_index(res.args[-1])):
         #     user.server_mode = name_2_index(res.args[-1])
         event_id_pre: str = res.args[0]
         # if event_id_pre.isdigit():
```

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/gacha_simulate.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/lsycx.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/search_player.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/song_chart.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/ycx.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/universal/router/ycx_all.py` & `tsugu-0.9.9rc9/tsugu_async/universal/router/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.9.9rc8/tsugu_async/utils/__init__.py` & `tsugu-0.9.9rc9/tsugu_async/utils/__init__.py`

 * *Files identical despite different names*

