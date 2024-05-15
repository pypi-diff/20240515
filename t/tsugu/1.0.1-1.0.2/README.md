# Comparing `tmp/tsugu-1.0.1.tar.gz` & `tmp/tsugu-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-1.0.1.tar", last modified: Wed May 15 06:42:32 2024, max compression
+gzip compressed data, was "tsugu-1.0.2.tar", last modified: Wed May 15 10:11:55 2024, max compression
```

## Comparing `tsugu-1.0.1.tar` & `tsugu-1.0.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.934220 tsugu-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 06:42:20.000000 tsugu-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 06:42:32.934220 tsugu-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 06:42:20.000000 tsugu-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 06:42:32.934220 tsugu-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-15 06:42:20.000000 tsugu-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.922220 tsugu-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-15 06:42:20.000000 tsugu-1.0.1/test/test_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.922220 tsugu-1.0.1/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.922220 tsugu-1.0.1/tsugu/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.922220 tsugu-1.0.1/tsugu/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.922220 tsugu-1.0.1/tsugu/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.926220 tsugu-1.0.1/tsugu/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.926220 tsugu-1.0.1/tsugu/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/room_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.926220 tsugu-1.0.1/tsugu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.922220 tsugu-1.0.1/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 06:42:32.000000 tsugu-1.0.1/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-15 06:42:32.000000 tsugu-1.0.1/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 06:42:32.000000 tsugu-1.0.1/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 06:42:32.000000 tsugu-1.0.1/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 06:42:32.000000 tsugu-1.0.1/tsugu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.926220 tsugu-1.0.1/tsugu_async/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.926220 tsugu-1.0.1/tsugu_async/command_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/command_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.926220 tsugu-1.0.1/tsugu_async/router/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.930220 tsugu-1.0.1/tsugu_async/router/bandoristation/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/bandoristation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/bandoristation/rooms_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/bandoristation/ycm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.930220 tsugu-1.0.1/tsugu_async/router/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/bind_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/bind_player_verification_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/bind_player_verification_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/change_default_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/change_server_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/switch_car_forwarding_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/switch_car_forwarding_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/remote/unbind_player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.930220 tsugu-1.0.1/tsugu_async/router/universal/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/event_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/gacha_simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/get_card_illustration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/lsycx.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/search_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/search_character.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/search_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/search_gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/search_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/search_song.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/song_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/song_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/ycx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/router/universal/ycx_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 06:42:32.930220 tsugu-1.0.1/tsugu_async/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-15 06:42:20.000000 tsugu-1.0.1/tsugu_async/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.801615 tsugu-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 10:11:42.000000 tsugu-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 10:11:55.801615 tsugu-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-15 10:11:42.000000 tsugu-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:11:55.801615 tsugu-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-15 10:11:42.000000 tsugu-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.789615 tsugu-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-15 10:11:42.000000 tsugu-1.0.2/test/test_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.793615 tsugu-1.0.2/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.793615 tsugu-1.0.2/tsugu/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.793615 tsugu-1.0.2/tsugu/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.793615 tsugu-1.0.2/tsugu/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.793615 tsugu-1.0.2/tsugu/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.797615 tsugu-1.0.2/tsugu/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/room_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.797615 tsugu-1.0.2/tsugu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.793615 tsugu-1.0.2/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-15 10:11:55.000000 tsugu-1.0.2/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-15 10:11:55.000000 tsugu-1.0.2/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:11:55.000000 tsugu-1.0.2/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 10:11:55.000000 tsugu-1.0.2/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 10:11:55.000000 tsugu-1.0.2/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.797615 tsugu-1.0.2/tsugu_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.797615 tsugu-1.0.2/tsugu_async/command_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/command_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.797615 tsugu-1.0.2/tsugu_async/router/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.797615 tsugu-1.0.2/tsugu_async/router/bandoristation/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/bandoristation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/bandoristation/rooms_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/bandoristation/ycm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.797615 tsugu-1.0.2/tsugu_async/router/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/bind_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/bind_player_verification_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/bind_player_verification_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/change_default_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/change_server_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/switch_car_forwarding_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/switch_car_forwarding_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/remote/unbind_player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.801615 tsugu-1.0.2/tsugu_async/router/universal/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/event_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/gacha_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/get_card_illustration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/lsycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/search_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/search_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/search_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/search_gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/search_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/search_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/song_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/song_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/ycx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/router/universal/ycx_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:11:55.801615 tsugu-1.0.2/tsugu_async/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-15 10:11:42.000000 tsugu-1.0.2/tsugu_async/utils/__init__.py
```

### Comparing `tsugu-1.0.1/LICENSE` & `tsugu-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/PKG-INFO` & `tsugu-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.0.1
+Version: 1.0.2
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.0.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 1.0.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
```

### Comparing `tsugu-1.0.1/README.md` & `tsugu-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/setup.py` & `tsugu-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='1.0.1',
+    version='1.0.2',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/ChatTsuguPy',
```

### Comparing `tsugu-1.0.1/test/test_async.py` & `tsugu-1.0.2/test/test_async.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/command_matcher/__init__.py` & `tsugu-1.0.2/tsugu/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/config.py` & `tsugu-1.0.2/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/handler.py` & `tsugu-1.0.2/tsugu/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/__init__.py` & `tsugu-1.0.2/tsugu/router/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return result
 
     # 开始匹配 help
     if res := match_command(message, commands=['help']):
         return help_command(res)
 
 
-async def help_command(res: MC):
+def help_command(res: MC):
     if not res.args:
         command_list = list(config._help_doc_dict.keys())
         command_list.sort()
         return text_response(f'当前支持的命令有：\n{" ".join(command_list)}\n请使用"help 命令名"来查看命令的详细帮助')
     if help_text := config.help_doc_dict.get(res.args[0], None):
         return text_response(help_text)
     return None
```

### Comparing `tsugu-1.0.1/tsugu/router/bandoristation/rooms_forward.py` & `tsugu-1.0.2/tsugu/router/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/bandoristation/ycm.py` & `tsugu-1.0.2/tsugu/router/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/remote/bind_player.py` & `tsugu-1.0.2/tsugu/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/remote/bind_player_verification_off.py` & `tsugu-1.0.2/tsugu/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/remote/bind_player_verification_on.py` & `tsugu-1.0.2/tsugu/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/remote/change_default_server.py` & `tsugu-1.0.2/tsugu/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/remote/change_server_mode.py` & `tsugu-1.0.2/tsugu/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/remote/player_status.py` & `tsugu-1.0.2/tsugu/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/remote/unbind_player.py` & `tsugu-1.0.2/tsugu/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/__init__.py` & `tsugu-1.0.2/tsugu/router/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/event_stage.py` & `tsugu-1.0.2/tsugu/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/gacha_simulate.py` & `tsugu-1.0.2/tsugu/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/lsycx.py` & `tsugu-1.0.2/tsugu/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/search_player.py` & `tsugu-1.0.2/tsugu/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/song_chart.py` & `tsugu-1.0.2/tsugu/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/ycx.py` & `tsugu-1.0.2/tsugu/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/router/universal/ycx_all.py` & `tsugu-1.0.2/tsugu/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu/utils/__init__.py` & `tsugu-1.0.2/tsugu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu.egg-info/PKG-INFO` & `tsugu-1.0.2/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 1.0.1
+Version: 1.0.2
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 1.0.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 1.0.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/ChatTsuguPy Author: kumoSleeping
 Author-email: zjr2992@outlook.com License: MIT Description:
                        ************ CChhaatt TTssuugguu PPyy[[ttmmrrnn]] ************
 _â¨ Python ç¼åç [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-
          bangdream-bot?tab=readme-ov-file) èªç¶è¯­è¨äº¤äºåº â¨_
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 --- ```shell pip install tsugu ``` > Powered by _t_s_u_g_u_-_a_p_i_-_p_y_t_h_o_n *** ## handler
```

### Comparing `tsugu-1.0.1/tsugu.egg-info/SOURCES.txt` & `tsugu-1.0.2/tsugu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/command_matcher/__init__.py` & `tsugu-1.0.2/tsugu_async/command_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/config.py` & `tsugu-1.0.2/tsugu_async/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/handler.py` & `tsugu-1.0.2/tsugu_async/handler.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/__init__.py` & `tsugu-1.0.2/tsugu_async/router/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/bandoristation/rooms_forward.py` & `tsugu-1.0.2/tsugu_async/router/bandoristation/rooms_forward.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/bandoristation/ycm.py` & `tsugu-1.0.2/tsugu_async/router/bandoristation/ycm.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/remote/bind_player.py` & `tsugu-1.0.2/tsugu_async/router/remote/bind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/remote/bind_player_verification_off.py` & `tsugu-1.0.2/tsugu_async/router/remote/bind_player_verification_off.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/remote/bind_player_verification_on.py` & `tsugu-1.0.2/tsugu_async/router/remote/bind_player_verification_on.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/remote/change_default_server.py` & `tsugu-1.0.2/tsugu_async/router/remote/change_default_server.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/remote/change_server_mode.py` & `tsugu-1.0.2/tsugu_async/router/remote/change_server_mode.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/remote/player_status.py` & `tsugu-1.0.2/tsugu_async/router/remote/player_status.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/remote/unbind_player.py` & `tsugu-1.0.2/tsugu_async/router/remote/unbind_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/__init__.py` & `tsugu-1.0.2/tsugu_async/router/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/event_stage.py` & `tsugu-1.0.2/tsugu_async/router/universal/event_stage.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/gacha_simulate.py` & `tsugu-1.0.2/tsugu_async/router/universal/gacha_simulate.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/lsycx.py` & `tsugu-1.0.2/tsugu_async/router/universal/lsycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/search_player.py` & `tsugu-1.0.2/tsugu_async/router/universal/search_player.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/song_chart.py` & `tsugu-1.0.2/tsugu_async/router/universal/song_chart.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/ycx.py` & `tsugu-1.0.2/tsugu_async/router/universal/ycx.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/router/universal/ycx_all.py` & `tsugu-1.0.2/tsugu_async/router/universal/ycx_all.py`

 * *Files identical despite different names*

### Comparing `tsugu-1.0.1/tsugu_async/utils/__init__.py` & `tsugu-1.0.2/tsugu_async/utils/__init__.py`

 * *Files identical despite different names*

