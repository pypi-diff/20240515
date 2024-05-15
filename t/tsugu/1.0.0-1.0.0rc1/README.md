# Comparing `tmp/tsugu-1.0.0.tar.gz` & `tmp/tsugu-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.0.0.tar", last modified: Wed May 15 05:58:20 2024, max compression
+gzip compressed data, was "tsugu-1.0.0rc1.tar", last modified: Wed May 15 04:13:23 2024, max compression
```

## Comparing `tsugu-1.0.0.tar` & `tsugu-1.0.0rc1.tar`

### file list

```diff
@@ -1,97 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.389553 tsugu-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 05:58:11.000000 tsugu-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 05:58:20.389553 tsugu-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 05:58:11.000000 tsugu-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 05:58:20.389553 tsugu-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-15 05:58:11.000000 tsugu-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.377553 tsugu-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-15 05:58:11.000000 tsugu-1.0.0/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.377553 tsugu-1.0.0/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.381554 tsugu-1.0.0/tsugu/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.381554 tsugu-1.0.0/tsugu/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.381554 tsugu-1.0.0/tsugu/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.381554 tsugu-1.0.0/tsugu/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.385553 tsugu-1.0.0/tsugu/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.385553 tsugu-1.0.0/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.377553 tsugu-1.0.0/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 05:58:20.000000 tsugu-1.0.0/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-15 05:58:20.000000 tsugu-1.0.0/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:58:20.000000 tsugu-1.0.0/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 05:58:20.000000 tsugu-1.0.0/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 05:58:20.000000 tsugu-1.0.0/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.385553 tsugu-1.0.0/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.385553 tsugu-1.0.0/tsugu_async/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.385553 tsugu-1.0.0/tsugu_async/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.385553 tsugu-1.0.0/tsugu_async/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.385553 tsugu-1.0.0/tsugu_async/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.389553 tsugu-1.0.0/tsugu_async/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:58:20.389553 tsugu-1.0.0/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-15 05:58:11.000000 tsugu-1.0.0/tsugu_async/utils/__init__.py
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

### Comparing `tsugu-1.0.0/LICENSE` & `tsugu-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/PKG-INFO` & `tsugu-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.0.0 Summary: Tsugu Python Frontend
-Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
-Author-email: zjr2992@outlook.com License: MIT Description:
+Metadata-Version: 2.1 Name: tsugu Version: 1.0.0rc1 Summary: Tsugu Python
+Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
+kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
 - `handler` ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
 ```python import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id
```

### Comparing `tsugu-1.0.0/README.md` & `tsugu-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/setup.py` & `tsugu-1.0.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.0.0',
+    version='1.0.0-rc1',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
@@ -17,13 +17,13 @@
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
             "loguru",
-            "tsugu-api-python>=1.1.2"
+            "tsugu-api-python>=1.0.4"
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-1.0.0/test/test_async.py` & `tsugu-1.0.0rc1/test/test_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,25 +20,24 @@
                     print(f"[图像大小: {len(i) / 1024:.2f}KB]")
 
         # tsugu.database('./user_data.db')
         # tsugu_async.config.reload_from_json('./config.json')
         # from tsugu_api_async import settings
         # settings.backend_url = 'http://127.0.0.1:8010'
         from tsugu_api_async import settings
+        settings.userdata_backend_url = 'http://127.0.0.1:14140'
 
-        # settings.backend_url = 'http://124.221.153.148:3000'
-        # settings.userdata_backend_url = 'http://127.0.0.1:3001'
-
-        msg1 = await tsugu_async.handler('玩家状态', '1528593481', 'red', '666808414')
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

### Comparing `tsugu-1.0.0/tsugu/command_matcher/__init__.py` & `tsugu-1.0.0rc1/tsugu/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/config.py` & `tsugu-1.0.0rc1/tsugu/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,32 +21,29 @@
             {"api": "search_song", "command_name": ["查歌曲", "查曲"]},
             {"api": "song_meta", "command_name": ["查询分数表", "查分数表"]},
             {"api": "search_character", "command_name": ["查角色"]},
             {"api": "song_chart", "command_name": ["查铺面", "查谱面"]},
             {"api": "ycx_all", "command_name": ["ycxall", "ycx all"]},
             {"api": "ycx", "command_name": ["ycx", "预测线"]},
             {"api": "lsycx", "command_name": ["lsycx"]},
+            {"api": "room_list", "command_name": ["ycm", "车来"]},
             {"api": "search_card", "command_name": ["查卡"]},
             {"api": "event_stage", "command_name": ["查试炼"]},
         ]
         self.user_commands = [
             {"api": "player_status", "command_name": ["玩家状态"]},
             {"api": "switch_car_forwarding_off", "command_name": ['关闭车牌转发', '关闭个人车牌转发']},
             {"api": "switch_car_forwarding_on", "command_name": ['开启车牌转发', '开启个人车牌转发']},
             {"api": "bind_player", "command_name": ["绑定玩家"]},
             {"api": "unbind_player", "command_name": ["解除绑定"]},
             {"api": "change_server_mode", "command_name": ["主服务器"]},
             {"api": "change_default_server", "command_name": ["设置默认服务器"]},
             {"api": "bind_player_verification_off", "command_name": ["验证解绑"]},
             {"api": "bind_player_verification_on", "command_name": ["验证绑定"]},
         ]
-        self.bandoristation_commands = [
-            {"api": "ycm", "command_name": ["ycm", "车来"]},
-            {"api": "rooms_forward", "command_name": ["上传车牌", ""]},  # 空字符串表示任何消息都会触发
-        ]
 
         self._user_database_path = None
         self._i_s = {0: "jp", 1: "en", 2: "tw", 3: "cn", 4: "kr"}
         self._s_i = {"jp": 0, "en": 1, "tw": 2, "cn": 3, "kr": 4}
         self._car_config = {
             "car": [
                 "q1",
```

### Comparing `tsugu-1.0.0/tsugu/handler.py` & `tsugu-1.0.0rc1/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/__init__.py` & `tsugu-1.0.0rc1/tsugu/router/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,46 @@
 from ..utils import server_exists, text_response, config, get_user
 from ..command_matcher import match_command
 from . import remote
 from . import universal
-from . import bandoristation
-from ..command_matcher import match_command, MC
+from .help import help_command
+from .rooms_forward import submit_rooms
 
 
 def handler(message: str, user_id: str, platform: str, channel_id: str):
     # 进行 api 命令匹配
-    result = universal_api_handler(user_id, message, platform, channel_id)
+    result = universal_api_handler(user_id, message, platform, channel_id, local=False)
     if result:
         return result
 
     # 远程命令
     result = remote_api_handler(user_id, message, platform, channel_id)
     if result:
         return result
 
-    result = bandoristation_api_handler(user_id, message, platform, channel_id)
-    if result:
-        return result
-
-    # 开始匹配 help
-    if res := match_command(message, commands=['help']):
-        return help_command(res)
 
-
-async def help_command(res: MC):
-    if not res.args:
-        command_list = list(config._help_doc_dict.keys())
-        command_list.sort()
-        return text_response(f'当前支持的命令有：\n{" ".join(command_list)}\n请使用"help 命令名"来查看命令的详细帮助')
-    if help_text := config.help_doc_dict.get(res.args[0], None):
-        return text_response(help_text)
-    return None
-
-
-def bandoristation_api_handler(user_id: str, message: str,  platform: str, channel_id: str):
-    for i in config.bandoristation_commands:
-        if res := match_command(message, commands=i['command_name']):
-            api = i['api']
-            user = get_user(user_id, platform)
-            return bandoristation.api_handler(user, res, api, platform, channel_id)
-    return None
-
-
-def universal_api_handler(user_id: str, message: str,  platform: str, channel_id: str):
+def universal_api_handler(user_id: str, message: str,  platform: str, channel_id: str, local=False):
     for i in config.commands:
         if res := match_command(message, commands=i['command_name']):
             api = i['api']
             user = get_user(user_id, platform)
             return universal.api_handler(user, res, api, platform, channel_id)
-        return None
+    # 开始匹配 help
+    if res := match_command(message, commands=['help']):
+        return help_command(res)
+        # 开始上传车牌
+    if res := match_command(message, commands=['上传车牌', '']):
+        submit_rooms(res, user_id, platform)
+    return None
 
 
 def remote_api_handler(user_id: str, message: str,  platform: str, channel_id: str):
     for i in config.user_commands:
         if res := match_command(message, commands=i['command_name']):
             api = i['api']
             user = get_user(user_id, platform)
             return remote.api_handler(user, res, api, platform, channel_id)
+
     return None
```

### Comparing `tsugu-1.0.0/tsugu/router/bandoristation/rooms_forward.py` & `tsugu-1.0.0rc1/tsugu_async/router/rooms_forward.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import tsugu_api
+import tsugu_api_async
 
-from ...utils import config
+from ..utils import config
 import re
-from ...utils import User, text_response
-from ...command_matcher import MC
+from ..utils import User, text_response
+from ..command_matcher import MC
 from loguru import logger
-from ...utils import get_user
+from ..utils import get_user
 
 
-def handler(user: User, res: MC, platform: str, channel_id: str):
+async def submit_rooms(res: MC, user_id, platform=None):
     message = res.text
     # 检查car_config['car']中的关键字
     for keyword in config._car_config["car"]:
         if str(keyword) in message:
             break
     else:
         return []
@@ -22,15 +22,15 @@
         if str(keyword) in message:
             return []
 
     pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
     if not re.match(pattern, message):
         return []
 
-    user = get_user(user.user_id, platform)
+    user = await get_user(user_id, platform)
 
     # 获取用户数据
     try:
         if platform:
             if not user.car:
                 return []
     except Exception as e:
@@ -38,18 +38,18 @@
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
         if user.user_id.isdigit():
-            car_user_id = user.user_id
-        else:
             car_user_id = '3889000770'
-        tsugu_api.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source=config.token_name, token=config.bandori_station_token)
+        else:
+            car_user_id = user.user_id
+        await tsugu_api_async.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source=config.token_name, token=config.bandori_station_token)
         return []
     except Exception as e:
         logger.error(f"[Tsugu] 发生异常: {e}")
         return []  # 虽然提交失败，但是确定了是车牌消息
```

### Comparing `tsugu-1.0.0/tsugu/router/remote/bind_player.py` & `tsugu-1.0.0rc1/tsugu/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/remote/bind_player_verification_off.py` & `tsugu-1.0.0rc1/tsugu/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/remote/bind_player_verification_on.py` & `tsugu-1.0.0rc1/tsugu/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/remote/change_default_server.py` & `tsugu-1.0.0rc1/tsugu/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/remote/change_server_mode.py` & `tsugu-1.0.0rc1/tsugu/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/remote/player_status.py` & `tsugu-1.0.0rc1/tsugu/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/remote/unbind_player.py` & `tsugu-1.0.0rc1/tsugu/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/__init__.py` & `tsugu-1.0.0rc1/tsugu/router/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/event_stage.py` & `tsugu-1.0.0rc1/tsugu/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/gacha_simulate.py` & `tsugu-1.0.0rc1/tsugu/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/lsycx.py` & `tsugu-1.0.0rc1/tsugu/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/search_player.py` & `tsugu-1.0.0rc1/tsugu/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/song_chart.py` & `tsugu-1.0.0rc1/tsugu/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/ycx.py` & `tsugu-1.0.0rc1/tsugu/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/router/universal/ycx_all.py` & `tsugu-1.0.0rc1/tsugu/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu/utils/__init__.py` & `tsugu-1.0.0rc1/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu.egg-info/PKG-INFO` & `tsugu-1.0.0rc1/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Chat Tsugu Py <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.0.0 Summary: Tsugu Python Frontend
-Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
-Author-email: zjr2992@outlook.com License: MIT Description:
+Metadata-Version: 2.1 Name: tsugu Version: 1.0.0rc1 Summary: Tsugu Python
+Frontend Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author:
+kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
 - `handler` ç¨äºç´æ¥å¤çç¨æ·è¾å¥çèªç¶è¯­è¨å¹¶è¿åæ¥è¯¢ç»æ:
 ```python import tsugu # åä¸ªåæ°ï¼åå«æå³ç æ¶æ¯åå®¹ ç¨æ·id
```

### Comparing `tsugu-1.0.0/tsugu.egg-info/SOURCES.txt` & `tsugu-1.0.0rc1/tsugu.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 tsugu.egg-info/PKG-INFO
 tsugu.egg-info/SOURCES.txt
 tsugu.egg-info/dependency_links.txt
 tsugu.egg-info/requires.txt
 tsugu.egg-info/top_level.txt
 tsugu/command_matcher/__init__.py
 tsugu/router/__init__.py
-tsugu/router/bandoristation/__init__.py
-tsugu/router/bandoristation/rooms_forward.py
-tsugu/router/bandoristation/ycm.py
+tsugu/router/help.py
+tsugu/router/rooms_forward.py
 tsugu/router/remote/__init__.py
 tsugu/router/remote/bind_player.py
 tsugu/router/remote/bind_player_verification_off.py
 tsugu/router/remote/bind_player_verification_on.py
 tsugu/router/remote/change_default_server.py
 tsugu/router/remote/change_server_mode.py
 tsugu/router/remote/player_status.py
@@ -43,17 +42,16 @@
 tsugu/router/universal/ycx_all.py
 tsugu/utils/__init__.py
 tsugu_async/__init__.py
 tsugu_async/config.py
 tsugu_async/handler.py
 tsugu_async/command_matcher/__init__.py
 tsugu_async/router/__init__.py
-tsugu_async/router/bandoristation/__init__.py
-tsugu_async/router/bandoristation/rooms_forward.py
-tsugu_async/router/bandoristation/ycm.py
+tsugu_async/router/help.py
+tsugu_async/router/rooms_forward.py
 tsugu_async/router/remote/__init__.py
 tsugu_async/router/remote/bind_player.py
 tsugu_async/router/remote/bind_player_verification_off.py
 tsugu_async/router/remote/bind_player_verification_on.py
 tsugu_async/router/remote/change_default_server.py
 tsugu_async/router/remote/change_server_mode.py
 tsugu_async/router/remote/player_status.py
@@ -61,14 +59,15 @@
 tsugu_async/router/remote/switch_car_forwarding_on.py
 tsugu_async/router/remote/unbind_player.py
 tsugu_async/router/universal/__init__.py
 tsugu_async/router/universal/event_stage.py
 tsugu_async/router/universal/gacha_simulate.py
 tsugu_async/router/universal/get_card_illustration.py
 tsugu_async/router/universal/lsycx.py
+tsugu_async/router/universal/room_list.py
 tsugu_async/router/universal/search_card.py
 tsugu_async/router/universal/search_character.py
 tsugu_async/router/universal/search_event.py
 tsugu_async/router/universal/search_gacha.py
 tsugu_async/router/universal/search_player.py
 tsugu_async/router/universal/search_song.py
 tsugu_async/router/universal/song_chart.py
```

### Comparing `tsugu-1.0.0/tsugu_async/command_matcher/__init__.py` & `tsugu-1.0.0rc1/tsugu_async/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/config.py` & `tsugu-1.0.0rc1/tsugu_async/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,32 +21,29 @@
             {"api": "search_song", "command_name": ["查歌曲", "查曲"]},
             {"api": "song_meta", "command_name": ["查询分数表", "查分数表"]},
             {"api": "search_character", "command_name": ["查角色"]},
             {"api": "song_chart", "command_name": ["查铺面", "查谱面"]},
             {"api": "ycx_all", "command_name": ["ycxall", "ycx all"]},
             {"api": "ycx", "command_name": ["ycx", "预测线"]},
             {"api": "lsycx", "command_name": ["lsycx"]},
+            {"api": "room_list", "command_name": ["ycm", "车来"]},
             {"api": "search_card", "command_name": ["查卡"]},
             {"api": "event_stage", "command_name": ["查试炼"]},
         ]
         self.user_commands = [
             {"api": "player_status", "command_name": ["玩家状态"]},
             {"api": "switch_car_forwarding_off", "command_name": ['关闭车牌转发', '关闭个人车牌转发']},
             {"api": "switch_car_forwarding_on", "command_name": ['开启车牌转发', '开启个人车牌转发']},
             {"api": "bind_player", "command_name": ["绑定玩家"]},
             {"api": "unbind_player", "command_name": ["解除绑定"]},
             {"api": "change_server_mode", "command_name": ["主服务器"]},
             {"api": "change_default_server", "command_name": ["设置默认服务器"]},
             {"api": "bind_player_verification_off", "command_name": ["验证解绑"]},
             {"api": "bind_player_verification_on", "command_name": ["验证绑定"]},
         ]
-        self.bandoristation_commands = [
-            {"api": "ycm", "command_name": ["ycm", "车来"]},
-            {"api": "rooms_forward", "command_name": ["上传车牌", ""]},  # 空字符串表示任何消息都会触发
-        ]
 
         self._user_database_path = None
         self._i_s = {0: "jp", 1: "en", 2: "tw", 3: "cn", 4: "kr"}
         self._s_i = {"jp": 0, "en": 1, "tw": 2, "cn": 3, "kr": 4}
         self._car_config = {
             "car": [
                 "q1",
```

### Comparing `tsugu-1.0.0/tsugu_async/handler.py` & `tsugu-1.0.0rc1/tsugu_async/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/bandoristation/rooms_forward.py` & `tsugu-1.0.0rc1/tsugu/router/rooms_forward.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-import tsugu_api_async
+import tsugu_api
 
-from ...utils import config
-import re
-from ...utils import User, text_response
-from ...command_matcher import MC
+from ..utils import config, get_user
 from loguru import logger
-from ...utils import get_user
+import httpx
+import re
+
+from ..utils import User, text_response
+from ..command_matcher import MC
 
 
-async def handler(user: User, res: MC, platform: str, channel_id: str):
+def submit_rooms(res: MC, user_id, platform=None):
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
 
-    user = await get_user(user.user_id, platform)
+    user = get_user(user_id, platform)
 
     # 获取用户数据
     try:
         if platform:
             if not user.car:
                 return []
     except Exception as e:
         # 默认不开启关闭车牌，继续提交
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
-        if user.user_id.isdigit():
-            car_user_id = user.user_id
-        else:
-            car_user_id = '3889000770'
-        await tsugu_api_async.submit_room_number(number=int(car_id), user_id=car_user_id, raw_message=message, source=config.token_name, token=config.bandori_station_token)
+
+        tsugu_api.submit_room_number(number=int(car_id), user_id=user.user_id, raw_message=message, source=config.token_name, token=config.bandori_station_token)
         return []
     except Exception as e:
         logger.error(f"[Tsugu] 发生异常: {e}")
         return []  # 虽然提交失败，但是确定了是车牌消息
```

### Comparing `tsugu-1.0.0/tsugu_async/router/remote/bind_player.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/remote/bind_player_verification_off.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/remote/bind_player_verification_on.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/remote/change_default_server.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/remote/change_server_mode.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/remote/player_status.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/remote/unbind_player.py` & `tsugu-1.0.0rc1/tsugu_async/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/__init__.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from . import search_song
 from . import song_meta
 from . import search_character
 from . import song_chart
 from . import ycx_all
 from . import ycx
 from . import lsycx
+from . import room_list
 from . import search_card
 from . import event_stage
 
 import asyncio
 
 
 async def api_handler(user, res, api, platform, channel_id):
```

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/event_stage.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/gacha_simulate.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/lsycx.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/search_player.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/song_chart.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/ycx.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/router/universal/ycx_all.py` & `tsugu-1.0.0rc1/tsugu_async/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.0/tsugu_async/utils/__init__.py` & `tsugu-1.0.0rc1/tsugu_async/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from ..config import config
 
 from tsugu_api._typing import _ServerId
 import tsugu_api_async
 import time
 from loguru import logger
 import asyncio
-from typing import Optional
 
 
 class User:
     def __init__(self, user_id: str, platform: str, server_mode: _ServerId, default_server: List[_ServerId], car: bool, server_list: list, game_ids: list, verify_code: str):
         self.user_id: str = user_id
         self.platform: str = platform
         self.server_mode: _ServerId = server_mode
@@ -47,52 +46,54 @@
     if server or server == 0:
         return True
     if not server:
         return False
     return False
 
 
-async def get_user(user_id: str, platform: str) -> Optional[User]:
+async def get_user(user_id: str, platform: str) -> User:
     for i in range(0, config.get_remote_user_data_max_retry):
         try:
             user_data_res = await tsugu_api_async.get_user_data(platform, user_id)
             if user_data_res.get('status') == 'failed':
-                return None
+                return text_response(user_data_res.get('data'))
             break
         except Exception as e:
             logger.error(f'Error: {e}')
-            time.sleep(0.5)
+            await asyncio.sleep(0.5)
             continue
     else:
-        return None
-
-    # 旧数据兼容
+        raise Exception('获取用户数据失败')
+    # 获取用户数据失败
+    if user_data_res.get('status') == 'failed':
+        return text_response(user_data_res.get('data'))
+    # 构建用户对象
     user_data = user_data_res.get('data')
+
     if user_data.get('game_ids') is None:
 
         user_data['game_ids'] = []
         for i in range(0, 5):
-            if user_data.get('server_list')[i]['playerId'] != 0:  # type: ignore
-                new_game_id = {"game_id": user_data.get('server_list')[i]['playerId'], "server": i}  # type: ignore
-                user_data['game_ids'].append(new_game_id)  # type: ignore
+            if user_data.get('server_list')[i]['playerId'] != 0:
+                new_game_id = {"game_id": user_data.get('server_list')[i]['playerId'], "server": i}
+                user_data['game_ids'].append(new_game_id)
         verify_code_all = []
         for i in range(0, 5):
             if user_data.get('server_list')[i].get('verifyCode') is not None:
                 verify_code_all.append(i)
         # 有一说一，下面这行没有实际意义
-        user_data['verify_code'] = '或'.join(
-            [str(user_data.get('server_list')[i].get('verifyCode')) for i in verify_code_all]) if len(
-            verify_code_all) > 1 else verify_code_all[0] if verify_code_all else ''
+        user_data['verify_code'] = '或'.join([str(user_data.get('server_list')[i].get('verifyCode')) for i in verify_code_all]) if len(verify_code_all) > 1 else verify_code_all[0] if verify_code_all else ''
 
-    # 构建用户对象
     user = User(user_id=user_id,
                 platform=platform,
-                server_mode=user_data.get('server_mode'),  # type: ignore
-                default_server=user_data.get('default_server'),  # type: ignore
-                car=user_data.get('car'),  # type: ignore
-                server_list=user_data.get('server_list', None),  # type: ignore
-                game_ids=user_data.get('game_ids', []),  # type: ignore
-                verify_code=user_data.get('verify_code'))  # type: ignore
+                server_mode=user_data.get('server_mode'),
+                default_server=user_data.get('default_server'),
+                car=user_data.get('car'),
+                server_list=user_data.get('server_list', None),
+                game_ids=user_data.get('game_ids', []),
+                verify_code=user_data.get('verify_code'))
     return user
 
 
 
+
+
```

