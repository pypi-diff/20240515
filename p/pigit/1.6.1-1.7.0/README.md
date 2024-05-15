# Comparing `tmp/pigit-1.6.1.tar.gz` & `tmp/pigit-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigit-1.6.1.tar", last modified: Wed Jan 25 00:09:26 2023, max compression
+gzip compressed data, was "pigit-1.7.0.tar", last modified: Wed May 15 02:55:25 2024, max compression
```

## Comparing `pigit-1.6.1.tar` & `pigit-1.7.0.tar`

### file list

```diff
@@ -1,67 +1,76 @@
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.998003 pigit-1.6.1/
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1064 2022-01-11 07:04:24.000000 pigit-1.6.1/LICENSE
--rw-r--r--   0 lijunzhang   (501) staff       (20)     9915 2023-01-25 00:09:26.997737 pigit-1.6.1/PKG-INFO
--rw-r--r--   0 lijunzhang   (501) staff       (20)     9095 2023-01-25 00:06:37.000000 pigit-1.6.1/README.md
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.986104 pigit-1.6.1/pigit/
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1102 2022-03-24 15:37:11.000000 pigit-1.6.1/pigit/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      379 2022-03-20 13:41:30.000000 pigit-1.6.1/pigit/__main__.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.987312 pigit-1.6.1/pigit/cmdparse/
--rw-r--r--   0 lijunzhang   (501) staff       (20)        0 2022-03-27 12:44:56.000000 pigit-1.6.1/pigit/cmdparse/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    17325 2022-08-22 09:17:32.000000 pigit-1.6.1/pigit/cmdparse/parser.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.989016 pigit-1.6.1/pigit/cmdparse/shellcompletion/
--rw-r--r--   0 lijunzhang   (501) staff       (20)     2674 2022-04-02 13:33:03.000000 pigit-1.6.1/pigit/cmdparse/shellcompletion/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     5831 2022-04-09 16:52:30.000000 pigit-1.6.1/pigit/cmdparse/shellcompletion/base.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1360 2022-03-26 18:15:37.000000 pigit-1.6.1/pigit/cmdparse/shellcompletion/bash.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1905 2022-03-26 18:15:46.000000 pigit-1.6.1/pigit/cmdparse/shellcompletion/fish.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     5180 2022-04-01 14:17:00.000000 pigit-1.6.1/pigit/cmdparse/shellcompletion/zsh.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    19890 2022-08-22 09:43:33.000000 pigit-1.6.1/pigit/codecounter.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.990127 pigit-1.6.1/pigit/common/
--rw-r--r--   0 lijunzhang   (501) staff       (20)       23 2022-03-19 16:57:13.000000 pigit-1.6.1/pigit/common/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1972 2022-04-26 15:28:01.000000 pigit-1.6.1/pigit/common/func.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      250 2022-01-11 07:04:24.000000 pigit-1.6.1/pigit/common/singleton.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     8905 2022-04-26 15:23:09.000000 pigit-1.6.1/pigit/common/utils.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    10524 2023-01-24 23:44:03.000000 pigit-1.6.1/pigit/config.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1365 2023-01-25 00:02:23.000000 pigit-1.6.1/pigit/const.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    10878 2023-01-24 23:56:25.000000 pigit-1.6.1/pigit/entry.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.991717 pigit-1.6.1/pigit/gitlib/
--rw-r--r--   0 lijunzhang   (501) staff       (20)        0 2022-04-04 10:47:59.000000 pigit-1.6.1/pigit/gitlib/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     2357 2022-08-22 09:32:21.000000 pigit-1.6.1/pigit/gitlib/_cmd_func.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.992423 pigit-1.6.1/pigit/gitlib/ignore/
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1419 2022-04-09 18:38:13.000000 pigit-1.6.1/pigit/gitlib/ignore/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    26245 2022-04-09 19:02:08.000000 pigit-1.6.1/pigit/gitlib/ignore/template.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1744 2022-03-20 16:35:17.000000 pigit-1.6.1/pigit/gitlib/model.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    25635 2023-01-24 23:31:50.000000 pigit-1.6.1/pigit/gitlib/options.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     8651 2022-08-22 09:32:37.000000 pigit-1.6.1/pigit/gitlib/processor.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    21295 2022-04-10 08:38:02.000000 pigit-1.6.1/pigit/gitlib/shortcmds.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     4163 2022-08-22 09:39:36.000000 pigit-1.6.1/pigit/info.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     7985 2023-01-25 00:00:25.000000 pigit-1.6.1/pigit/interaction.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1249 2022-04-26 15:49:50.000000 pigit-1.6.1/pigit/log.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     2892 2022-08-22 09:39:52.000000 pigit-1.6.1/pigit/shellmode.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.994395 pigit-1.6.1/pigit/tui/
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1284 2022-01-11 07:04:24.000000 pigit-1.6.1/pigit/tui/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1771 2022-01-11 07:04:24.000000 pigit-1.6.1/pigit/tui/console.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     2115 2022-03-26 11:19:45.000000 pigit-1.6.1/pigit/tui/event_loop.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)    34974 2022-04-02 13:03:12.000000 pigit-1.6.1/pigit/tui/input.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1484 2022-01-11 07:04:24.000000 pigit-1.6.1/pigit/tui/screen.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     8671 2022-08-22 09:53:24.000000 pigit-1.6.1/pigit/tui/widgets.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.987058 pigit-1.6.1/pigit.egg-info/
--rw-r--r--   0 lijunzhang   (501) staff       (20)     9915 2023-01-25 00:09:26.000000 pigit-1.6.1/pigit.egg-info/PKG-INFO
--rw-r--r--   0 lijunzhang   (501) staff       (20)     1265 2023-01-25 00:09:26.000000 pigit-1.6.1/pigit.egg-info/SOURCES.txt
--rw-r--r--   0 lijunzhang   (501) staff       (20)        1 2023-01-25 00:09:26.000000 pigit-1.6.1/pigit.egg-info/dependency_links.txt
--rw-r--r--   0 lijunzhang   (501) staff       (20)       43 2023-01-25 00:09:26.000000 pigit-1.6.1/pigit.egg-info/entry_points.txt
--rw-r--r--   0 lijunzhang   (501) staff       (20)       14 2023-01-25 00:09:26.000000 pigit-1.6.1/pigit.egg-info/requires.txt
--rw-r--r--   0 lijunzhang   (501) staff       (20)       12 2023-01-25 00:09:26.000000 pigit-1.6.1/pigit.egg-info/top_level.txt
--rw-r--r--   0 lijunzhang   (501) staff       (20)       38 2023-01-25 00:09:26.998052 pigit-1.6.1/setup.cfg
--rw-r--r--   0 lijunzhang   (501) staff       (20)     2032 2022-08-22 10:29:11.000000 pigit-1.6.1/setup.py
-drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2023-01-25 00:09:26.997442 pigit-1.6.1/tests/
--rw-r--r--   0 lijunzhang   (501) staff       (20)        0 2022-01-11 07:04:24.000000 pigit-1.6.1/tests/__init__.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      247 2022-04-02 14:19:30.000000 pigit-1.6.1/tests/conftest.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      174 2022-03-20 13:41:30.000000 pigit-1.6.1/tests/run.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     4323 2022-04-08 16:19:00.000000 pigit-1.6.1/tests/test_cmdparser.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     2182 2022-04-09 17:00:54.000000 pigit-1.6.1/tests/test_common.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      615 2022-08-22 09:21:20.000000 pigit-1.6.1/tests/test_counter.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)     5003 2022-08-22 09:24:12.000000 pigit-1.6.1/tests/test_gitlib.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      524 2022-08-22 09:21:46.000000 pigit-1.6.1/tests/test_info.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      524 2022-04-02 10:25:41.000000 pigit-1.6.1/tests/test_pigit.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      305 2022-03-26 15:26:10.000000 pigit-1.6.1/tests/test_tui.py
--rw-r--r--   0 lijunzhang   (501) staff       (20)      327 2022-01-11 07:04:24.000000 pigit-1.6.1/tests/utils.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.208860 pigit-1.7.0/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1064 2023-12-14 03:22:21.000000 pigit-1.7.0/LICENSE
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    11287 2024-05-15 02:55:25.208594 pigit-1.7.0/PKG-INFO
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    10438 2023-12-07 06:46:42.000000 pigit-1.7.0/README.md
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.193738 pigit-1.7.0/pigit/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1102 2022-03-24 15:37:11.000000 pigit-1.7.0/pigit/__init__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      381 2024-02-19 07:40:14.000000 pigit-1.7.0/pigit/__main__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     6051 2024-05-11 09:30:25.000000 pigit-1.7.0/pigit/app.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.195235 pigit-1.7.0/pigit/cmdparse/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)        0 2023-07-16 12:55:54.000000 pigit-1.7.0/pigit/cmdparse/__init__.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.196956 pigit-1.7.0/pigit/cmdparse/completion/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1839 2023-07-26 07:02:49.000000 pigit-1.7.0/pigit/cmdparse/completion/__init__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     5333 2023-07-26 07:03:02.000000 pigit-1.7.0/pigit/cmdparse/completion/base.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      552 2023-07-26 07:03:13.000000 pigit-1.7.0/pigit/cmdparse/completion/bash.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1080 2023-07-26 07:03:20.000000 pigit-1.7.0/pigit/cmdparse/completion/fish.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     5154 2023-07-26 07:03:26.000000 pigit-1.7.0/pigit/cmdparse/completion/zsh.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    17992 2023-07-26 09:21:40.000000 pigit-1.7.0/pigit/cmdparse/parser.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    10697 2023-11-27 02:48:06.000000 pigit-1.7.0/pigit/config.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      524 2024-05-11 06:21:21.000000 pigit-1.7.0/pigit/console_scripts.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1378 2024-05-15 02:54:32.000000 pigit-1.7.0/pigit/const.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    13241 2023-12-07 06:46:42.000000 pigit-1.7.0/pigit/entry.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.198888 pigit-1.7.0/pigit/ext/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)       23 2022-03-19 16:57:13.000000 pigit-1.7.0/pigit/ext/__init__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     8469 2023-12-11 02:32:12.000000 pigit-1.7.0/pigit/ext/executor.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1974 2023-07-25 16:25:30.000000 pigit-1.7.0/pigit/ext/func.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    14041 2023-07-29 16:31:21.000000 pigit-1.7.0/pigit/ext/lcstat.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1715 2023-07-26 12:26:01.000000 pigit-1.7.0/pigit/ext/log.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      250 2022-01-11 07:04:24.000000 pigit-1.7.0/pigit/ext/singleton.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     7589 2024-02-19 07:44:25.000000 pigit-1.7.0/pigit/ext/utils.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.200756 pigit-1.7.0/pigit/git/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      740 2023-11-29 03:13:38.000000 pigit-1.7.0/pigit/git/__init__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     2417 2023-11-29 03:13:38.000000 pigit-1.7.0/pigit/git/_cmd_func.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    22092 2023-11-29 03:13:38.000000 pigit-1.7.0/pigit/git/_cmds.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.201576 pigit-1.7.0/pigit/git/ignore/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1505 2023-07-16 12:57:39.000000 pigit-1.7.0/pigit/git/ignore/__init__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    31082 2023-12-11 02:32:12.000000 pigit-1.7.0/pigit/git/ignore/template.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1939 2023-12-06 03:18:46.000000 pigit-1.7.0/pigit/git/model.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     8839 2023-11-29 03:13:38.000000 pigit-1.7.0/pigit/git/proxy.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    29546 2024-05-14 08:23:30.000000 pigit-1.7.0/pigit/git/repo.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     2925 2023-07-29 16:31:08.000000 pigit-1.7.0/pigit/info.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     2992 2023-11-29 03:13:38.000000 pigit-1.7.0/pigit/shellmode.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.203800 pigit-1.7.0/pigit/tui/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1284 2022-01-11 07:04:24.000000 pigit-1.7.0/pigit/tui/__init__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     9322 2024-05-13 09:59:37.000000 pigit-1.7.0/pigit/tui/components.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     3088 2024-05-11 07:15:29.000000 pigit-1.7.0/pigit/tui/console.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     3281 2024-05-11 08:42:25.000000 pigit-1.7.0/pigit/tui/event_loop.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    35454 2024-05-11 03:59:27.000000 pigit-1.7.0/pigit/tui/input.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1132 2023-08-03 03:34:42.000000 pigit-1.7.0/pigit/tui/utils.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.194801 pigit-1.7.0/pigit.egg-info/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    11287 2024-05-15 02:55:25.000000 pigit-1.7.0/pigit.egg-info/PKG-INFO
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1428 2024-05-15 02:55:25.000000 pigit-1.7.0/pigit.egg-info/SOURCES.txt
+-rw-r--r--   0 lijunzhang   (501) staff       (20)        1 2024-05-15 02:55:25.000000 pigit-1.7.0/pigit.egg-info/dependency_links.txt
+-rw-r--r--   0 lijunzhang   (501) staff       (20)       81 2024-05-15 02:55:25.000000 pigit-1.7.0/pigit.egg-info/entry_points.txt
+-rw-r--r--   0 lijunzhang   (501) staff       (20)       14 2024-05-15 02:55:25.000000 pigit-1.7.0/pigit.egg-info/requires.txt
+-rw-r--r--   0 lijunzhang   (501) staff       (20)       12 2024-05-15 02:55:25.000000 pigit-1.7.0/pigit.egg-info/top_level.txt
+-rw-r--r--   0 lijunzhang   (501) staff       (20)       38 2024-05-15 02:55:25.208908 pigit-1.7.0/setup.cfg
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     2099 2024-05-11 06:20:50.000000 pigit-1.7.0/setup.py
+drwxr-xr-x   0 lijunzhang   (501) staff       (20)        0 2024-05-15 02:55:25.208192 pigit-1.7.0/tests/
+-rw-r--r--   0 lijunzhang   (501) staff       (20)        0 2022-01-11 07:04:24.000000 pigit-1.7.0/tests/__init__.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      547 2023-12-11 02:32:12.000000 pigit-1.7.0/tests/conftest.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      497 2023-07-26 17:00:16.000000 pigit-1.7.0/tests/test_all_pigit.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     4613 2023-11-29 03:13:38.000000 pigit-1.7.0/tests/test_cmdparse.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      517 2023-07-26 16:44:50.000000 pigit-1.7.0/tests/test_config.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     2330 2024-05-14 03:44:08.000000 pigit-1.7.0/tests/test_ext.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     4639 2024-05-14 07:57:32.000000 pigit-1.7.0/tests/test_ext_executor.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     1011 2023-12-11 02:32:12.000000 pigit-1.7.0/tests/test_ext_lcstat.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     3891 2023-12-11 02:32:12.000000 pigit-1.7.0/tests/test_git.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     2044 2023-11-29 03:13:38.000000 pigit-1.7.0/tests/test_git_cmd.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      735 2024-05-14 06:49:13.000000 pigit-1.7.0/tests/test_git_ignore.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      482 2023-07-29 16:21:01.000000 pigit-1.7.0/tests/test_info.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     2380 2023-10-30 09:36:31.000000 pigit-1.7.0/tests/test_shell.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     8587 2024-05-14 07:54:44.000000 pigit-1.7.0/tests/test_tui_components.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     5030 2023-10-30 07:18:45.000000 pigit-1.7.0/tests/test_tui_console.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)     3678 2024-05-14 03:00:15.000000 pigit-1.7.0/tests/test_tui_eventloop.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)    18026 2024-05-14 07:09:20.000000 pigit-1.7.0/tests/test_tui_input.py
+-rw-r--r--   0 lijunzhang   (501) staff       (20)      327 2022-01-11 07:04:24.000000 pigit-1.7.0/tests/utils.py
```

### Comparing `pigit-1.6.1/LICENSE` & `pigit-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pigit-1.6.1/PKG-INFO` & `pigit-1.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pigit
-Version: 1.6.1
-Summary: Simple terminal tool of Git.
-Home-page: https://github.com/zlj-zz/pigit.git
-Author: Zachary Zhang
-Author-email: zlj19971222@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: System :: Shells
-Classifier: Topic :: Software Development
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PIGIT
 
 ![Python 3](https://img.shields.io/badge/Python-v3.8%5E-green?logo=python)
 [![pypi_version](https://img.shields.io/pypi/v/pigit?label=pypi)](https://pypi.org/project/pigit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A terminal tool for git. Read as [Pi Git], meaning to use git like pig it. When we use git, do you feel very uncomfortable with too long commands. For example: `git status --short`, this project can help you improve it. This project is written in Python. Now most UNIX like systems come with Python. So you can easily install and use it.
@@ -32,52 +9,56 @@
 ## Usage
 
 If you want to use it, you must first know what it can do.
 
 The command of `pigit -h` or `pigit --help` to get the help message with usage. Like this:
 
 ```bash
-usage: pigit [-h] [-v] [-r] [-f] [-i] [-c [PATH]] [-C] [--create-ignore TYPE]
-             [--create-config]
-             {cmd,repo} ...
+usage: pigit [-h] [-i] [-f] [-r] [-v] [-c [PATH]] [--create-ignore TYPE]
+             [--complete [SHELL]] [--create-config]
+             {cmd,repo,open} ...
 
 Pigit TUI is called automatically if no parameters are followed.
 
+
 positional arguments:
-  {cmd,repo}
+  {cmd,repo,open}
     cmd                 git short command.
-    repo                repo options.
+    repo                repos options.
     open                open remote repository in web browser.
 
-optional arguments:
+
+options:
   -h, --help            show this help message and exit
-  -v, --version         Show version and exit.
-  -r, --report          Report the pigit desc and exit.
-  -f, --config          Display the config of current git repository and exit.
   -i, --information     Show some information about the current git repository.
+  -f, --config          Display the config of current git repository and exit.
+  -r, --report          Report the pigit desc and exit.
+  -v, --version         Show version and exit.
+
 
 tools arguments:
   Auxiliary type commands.
 
   -c [PATH], --count [PATH]
-                        Count the number of codes and output them in tabular form.A given path can be
-                        accepted, and the default is the current directory.
-  -C, --complete        Add shell prompt script and exit.(Supported bash, zsh, fish)
-  --create-ignore TYPE  Create a demo .gitignore file. Need one argument, support: [android, c++, cpp, c,
-                        dart, elisp, gitbook, go, java, kotlin, lua, maven, node, python, qt, r, ros, ruby,
-                        rust, sass, swift, unity]
-  --create-config       Create a pre-configured file of PIGIT.(If a profile exists, the values available in it
-                        are used)
+                        Count the number of codes and output them in tabular form.
+                        A given path can be accepted, and the default is the
+                        current directory.
+  --create-ignore TYPE  Create a demo .gitignore file. Need one argument, the type
+                        of gitignore.
+  --complete [SHELL]    Add shell prompt script and exit. (Supported bash, zsh,
+                        fish)
+  --create-config       Create a pre-configured file of PIGIT.(If a profile
+                        exists, the values available in it are used)
 ```
 
 ### `cmd`
 
 The command of `cmd` support some short sub-command to replace the long git original command.
 
-![demo display](./docs//demo.gif)
+![demo display](./docs/resources/demo.gif)
 
 Use `pigit cmd -s` to check what short command it supported, it will display the corresponding help information and the git original command, like this:
 
 ```
 These are short commands that can replace git operations:
     b        lists, creates, renames, and deletes branches.
              git branch
@@ -100,27 +81,50 @@
 ......
 ```
 
 ### `repo`
 
 The command of `repo` support operate multiple repos at the same time.
 
-![demo display](./docs/demo_repo_1.png)
-![demo display](./docs/demo_repo_2.png)
-![demo display](./docs/demo_repo_3.png)
+![demo display](./docs/resources/demo_repo_1.png)
+![demo display](./docs/resources/demo_repo_2.png)
+![demo display](./docs/resources/demo_repo_3.png)
 
 Use `pigit repo -h` to get more help.
 
+```
+usage: pigit
+
+ repo [-h] {add,rm,rename,ll,clear,cd,fetch,pull,push} ...
+
+
+positional arguments:
+  {add,rm,rename,ll,clear,cd,fetch,pull,push}
+    add                 add repo(s).
+    rm                  remove repo(s).
+    rename              rename a repo.
+    ll                  display summary of all repos.
+    clear               clear the all repos.
+    cd                  jump to a repo dir.
+    fetch               fetch remote update for repo(s).
+    pull                pull remote updates for repo(s).
+    push                push the local updates for repo(s).
+
+
+options:
+  -h, --help            show this help message and exit
+```
+
 ### Interaction
 
 Even if you can use short commands instead of long commands of git, there are still some cases where simple commands can be very bad. For example: `git add a/b/1.txt b/c/1.txt c/d/1.txt`.
 
 Therefore, we need a TUI to help us, so Pigit provides a simple command-line interactive TUI. When you use `pigit` without following any parameters, you will enter it.
 
-![interaction demo](./docs/demo_interaction.gif)
+![interaction demo](./docs/resources/demo_interaction.gif)
 
 And in the interaction mode, you can use `?` or `h` to see the help message.
 
 ## Installation
 
 ### Pip
 
@@ -134,52 +138,81 @@
 git clone https://github.com/zlj-zz/pigit.git --depth=1
 cd pigit
 make install
 # or
 python setup.py install  # On windows
 ```
 
+## Completion
+
+Provides a friendly command-line completion capability, injecting completion through the following methods.
+
+Write it to your shell configuration file：
+
+```sh
+# ~/.zshrc
+
+eval "$(pigit --complete zsh)"
+```
+
+Currently supports `bash`, `zsh` and `fish`.
+
+If no shell is specified, it will try to automatically detect what shell you are using.
+
+```sh
+eval "$(pigit --complete)"
+```
+
 ## Alias
 
 Alias is good way to help you use _pigit_ faster . Open your shell profile and append:
 
 ```bash
 if type pigit >/dev/null 2>&1; then
     alias pg="pigit"
-    alias g="pigit cmd"
     alias gr="pigit repo"
 fi
 ```
 
-Then, you can use `pg` to call `pigit` and use `g` to call `pigit cmd`.
+Then, you can use `pg` to call `pigit`.
+
+**Windows**
+
+Check your *PowerShell* config, like this: `echo $profile`. Create it if the path not exist. Then open it, and input:
+
+```ps
+set-alias pg pigit
+```
+
+After completing the above preparations, restart your terminal. If it prompts that you cannot run the configuration, you can refer to the [official website address](https://learn.microsoft.com/zh-cn/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.4).
 
 ## Configuration
 
 You can use `pigit --create-config` to create a template configuration at **pigit** home path.
 
 On Linux or MacOS: `~/.config/pigit`
 
 On windows should be: `C:\\User\\<your username>`
 
 [here](./docs/pigit.conf) is a configuration template.
 
-| config key                  | type  | default                     | desc                                                                                                                        |
-| --------------------------- | ----- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
-| cmd_show_original           | bool  | True                        | Show original git command.                                                                                                  |
-| cmd_recommend               | bool  | True                        | Is it recommended to correct when entering wrong commands.                                                                  |
-| tui_help_showtime           | float | 1.5                         | Display time of help information in interactive mode.                                                                       |
-| counter_use_gitignore       | bool  | True                        | Whether to use the ignore configuration of the `.gitignore` file.                                                           |
-| counter_show_invalid        | bool  | False                       | Whether show files that cannot be counted.                                                                                  |
-| counter_show_icon           | bool  | True                        | Whether show files icons. Font support required, like: 'Nerd Font'.                                                         |
-| counter_format              | str   | table                       | Output format of statistical results. Supported: [table, simple]                                                            |
-| git_config_format           | str   | table                       | Git local config print format. Supported: [table, normal]                                                                   |
-| repo_info_include           | list  | ["remote", "branch", "log"] | Control which parts need to be displayed when viewing git repository information. Support: (path,remote,branch,log,summary) |
-| repo_auto_append            | bool  | False                       | Whether auto append path to repos.                                                                                          |
-| debug_open                  | bool  | False                       | Whether run PIGIT in debug mode.                                                                                            |
-| log_output                  | bool  | False                       | Whether output log in terminal.                                                                                             |
+| config key            | type  | default                     | desc                                                                                                                        |
+| --------------------- | ----- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
+| cmd_display           | bool  | True                        | Show original git command.                                                                                                  |
+| cmd_recommend         | bool  | True                        | Is it recommended to correct when entering wrong commands.                                                                  |
+| tui_help_showtime     | float | 1.5                         | Display time of help information in interactive mode.                                                                       |
+| counter_use_gitignore | bool  | True                        | Whether to use the ignore configuration of the `.gitignore` file.                                                           |
+| counter_show_invalid  | bool  | False                       | Whether show files that cannot be counted.                                                                                  |
+| counter_show_icon     | bool  | True                        | Whether show files icons. Font support required, like: 'Nerd Font'.                                                         |
+| counter_format        | str   | table                       | Output format of statistical results. Supported: [table, simple]                                                            |
+| git_config_format     | str   | table                       | Git local config print format. Supported: [table, normal]                                                                   |
+| repo_info_include     | list  | ["remote", "branch", "log"] | Control which parts need to be displayed when viewing git repository information. Support: (path,remote,branch,log,summary) |
+| repo_auto_append      | bool  | False                       | Whether auto append path to repos.                                                                                          |
+| log_debug             | bool  | False                       | Whether run PIGIT in debug mode.                                                                                            |
+| log_output            | bool  | False                       | Whether output log in terminal.                                                                                             |
 
 ## Extra cmds
 
 You can setting your custom cmds. It need create a `extra_cmds.py` file at the **pigit** home. And writing like this:
 
 ```python
 import os
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pigit-1.6.1/README.md` & `pigit-1.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: pigit
+Version: 1.7.0
+Summary: Simple terminal tool of Git.
+Home-page: https://github.com/zlj-zz/pigit.git
+Author: Zachary Zhang
+Author-email: zlj19971222@outlook.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Software Development
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: plenty==1.0.2
+
 # PIGIT
 
 ![Python 3](https://img.shields.io/badge/Python-v3.8%5E-green?logo=python)
 [![pypi_version](https://img.shields.io/pypi/v/pigit?label=pypi)](https://pypi.org/project/pigit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A terminal tool for git. Read as [Pi Git], meaning to use git like pig it. When we use git, do you feel very uncomfortable with too long commands. For example: `git status --short`, this project can help you improve it. This project is written in Python. Now most UNIX like systems come with Python. So you can easily install and use it.
@@ -9,52 +33,56 @@
 ## Usage
 
 If you want to use it, you must first know what it can do.
 
 The command of `pigit -h` or `pigit --help` to get the help message with usage. Like this:
 
 ```bash
-usage: pigit [-h] [-v] [-r] [-f] [-i] [-c [PATH]] [-C] [--create-ignore TYPE]
-             [--create-config]
-             {cmd,repo} ...
+usage: pigit [-h] [-i] [-f] [-r] [-v] [-c [PATH]] [--create-ignore TYPE]
+             [--complete [SHELL]] [--create-config]
+             {cmd,repo,open} ...
 
 Pigit TUI is called automatically if no parameters are followed.
 
+
 positional arguments:
-  {cmd,repo}
+  {cmd,repo,open}
     cmd                 git short command.
-    repo                repo options.
+    repo                repos options.
     open                open remote repository in web browser.
 
-optional arguments:
+
+options:
   -h, --help            show this help message and exit
-  -v, --version         Show version and exit.
-  -r, --report          Report the pigit desc and exit.
-  -f, --config          Display the config of current git repository and exit.
   -i, --information     Show some information about the current git repository.
+  -f, --config          Display the config of current git repository and exit.
+  -r, --report          Report the pigit desc and exit.
+  -v, --version         Show version and exit.
+
 
 tools arguments:
   Auxiliary type commands.
 
   -c [PATH], --count [PATH]
-                        Count the number of codes and output them in tabular form.A given path can be
-                        accepted, and the default is the current directory.
-  -C, --complete        Add shell prompt script and exit.(Supported bash, zsh, fish)
-  --create-ignore TYPE  Create a demo .gitignore file. Need one argument, support: [android, c++, cpp, c,
-                        dart, elisp, gitbook, go, java, kotlin, lua, maven, node, python, qt, r, ros, ruby,
-                        rust, sass, swift, unity]
-  --create-config       Create a pre-configured file of PIGIT.(If a profile exists, the values available in it
-                        are used)
+                        Count the number of codes and output them in tabular form.
+                        A given path can be accepted, and the default is the
+                        current directory.
+  --create-ignore TYPE  Create a demo .gitignore file. Need one argument, the type
+                        of gitignore.
+  --complete [SHELL]    Add shell prompt script and exit. (Supported bash, zsh,
+                        fish)
+  --create-config       Create a pre-configured file of PIGIT.(If a profile
+                        exists, the values available in it are used)
 ```
 
 ### `cmd`
 
 The command of `cmd` support some short sub-command to replace the long git original command.
 
-![demo display](./docs//demo.gif)
+![demo display](./docs/resources/demo.gif)
 
 Use `pigit cmd -s` to check what short command it supported, it will display the corresponding help information and the git original command, like this:
 
 ```
 These are short commands that can replace git operations:
     b        lists, creates, renames, and deletes branches.
              git branch
@@ -77,27 +105,50 @@
 ......
 ```
 
 ### `repo`
 
 The command of `repo` support operate multiple repos at the same time.
 
-![demo display](./docs/demo_repo_1.png)
-![demo display](./docs/demo_repo_2.png)
-![demo display](./docs/demo_repo_3.png)
+![demo display](./docs/resources/demo_repo_1.png)
+![demo display](./docs/resources/demo_repo_2.png)
+![demo display](./docs/resources/demo_repo_3.png)
 
 Use `pigit repo -h` to get more help.
 
+```
+usage: pigit
+
+ repo [-h] {add,rm,rename,ll,clear,cd,fetch,pull,push} ...
+
+
+positional arguments:
+  {add,rm,rename,ll,clear,cd,fetch,pull,push}
+    add                 add repo(s).
+    rm                  remove repo(s).
+    rename              rename a repo.
+    ll                  display summary of all repos.
+    clear               clear the all repos.
+    cd                  jump to a repo dir.
+    fetch               fetch remote update for repo(s).
+    pull                pull remote updates for repo(s).
+    push                push the local updates for repo(s).
+
+
+options:
+  -h, --help            show this help message and exit
+```
+
 ### Interaction
 
 Even if you can use short commands instead of long commands of git, there are still some cases where simple commands can be very bad. For example: `git add a/b/1.txt b/c/1.txt c/d/1.txt`.
 
 Therefore, we need a TUI to help us, so Pigit provides a simple command-line interactive TUI. When you use `pigit` without following any parameters, you will enter it.
 
-![interaction demo](./docs/demo_interaction.gif)
+![interaction demo](./docs/resources/demo_interaction.gif)
 
 And in the interaction mode, you can use `?` or `h` to see the help message.
 
 ## Installation
 
 ### Pip
 
@@ -111,52 +162,81 @@
 git clone https://github.com/zlj-zz/pigit.git --depth=1
 cd pigit
 make install
 # or
 python setup.py install  # On windows
 ```
 
+## Completion
+
+Provides a friendly command-line completion capability, injecting completion through the following methods.
+
+Write it to your shell configuration file：
+
+```sh
+# ~/.zshrc
+
+eval "$(pigit --complete zsh)"
+```
+
+Currently supports `bash`, `zsh` and `fish`.
+
+If no shell is specified, it will try to automatically detect what shell you are using.
+
+```sh
+eval "$(pigit --complete)"
+```
+
 ## Alias
 
 Alias is good way to help you use _pigit_ faster . Open your shell profile and append:
 
 ```bash
 if type pigit >/dev/null 2>&1; then
     alias pg="pigit"
-    alias g="pigit cmd"
     alias gr="pigit repo"
 fi
 ```
 
-Then, you can use `pg` to call `pigit` and use `g` to call `pigit cmd`.
+Then, you can use `pg` to call `pigit`.
+
+**Windows**
+
+Check your *PowerShell* config, like this: `echo $profile`. Create it if the path not exist. Then open it, and input:
+
+```ps
+set-alias pg pigit
+```
+
+After completing the above preparations, restart your terminal. If it prompts that you cannot run the configuration, you can refer to the [official website address](https://learn.microsoft.com/zh-cn/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.4).
 
 ## Configuration
 
 You can use `pigit --create-config` to create a template configuration at **pigit** home path.
 
 On Linux or MacOS: `~/.config/pigit`
 
 On windows should be: `C:\\User\\<your username>`
 
 [here](./docs/pigit.conf) is a configuration template.
 
-| config key                  | type  | default                     | desc                                                                                                                        |
-| --------------------------- | ----- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
-| cmd_show_original           | bool  | True                        | Show original git command.                                                                                                  |
-| cmd_recommend               | bool  | True                        | Is it recommended to correct when entering wrong commands.                                                                  |
-| tui_help_showtime           | float | 1.5                         | Display time of help information in interactive mode.                                                                       |
-| counter_use_gitignore       | bool  | True                        | Whether to use the ignore configuration of the `.gitignore` file.                                                           |
-| counter_show_invalid        | bool  | False                       | Whether show files that cannot be counted.                                                                                  |
-| counter_show_icon           | bool  | True                        | Whether show files icons. Font support required, like: 'Nerd Font'.                                                         |
-| counter_format              | str   | table                       | Output format of statistical results. Supported: [table, simple]                                                            |
-| git_config_format           | str   | table                       | Git local config print format. Supported: [table, normal]                                                                   |
-| repo_info_include           | list  | ["remote", "branch", "log"] | Control which parts need to be displayed when viewing git repository information. Support: (path,remote,branch,log,summary) |
-| repo_auto_append            | bool  | False                       | Whether auto append path to repos.                                                                                          |
-| debug_open                  | bool  | False                       | Whether run PIGIT in debug mode.                                                                                            |
-| log_output                  | bool  | False                       | Whether output log in terminal.                                                                                             |
+| config key            | type  | default                     | desc                                                                                                                        |
+| --------------------- | ----- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
+| cmd_display           | bool  | True                        | Show original git command.                                                                                                  |
+| cmd_recommend         | bool  | True                        | Is it recommended to correct when entering wrong commands.                                                                  |
+| tui_help_showtime     | float | 1.5                         | Display time of help information in interactive mode.                                                                       |
+| counter_use_gitignore | bool  | True                        | Whether to use the ignore configuration of the `.gitignore` file.                                                           |
+| counter_show_invalid  | bool  | False                       | Whether show files that cannot be counted.                                                                                  |
+| counter_show_icon     | bool  | True                        | Whether show files icons. Font support required, like: 'Nerd Font'.                                                         |
+| counter_format        | str   | table                       | Output format of statistical results. Supported: [table, simple]                                                            |
+| git_config_format     | str   | table                       | Git local config print format. Supported: [table, normal]                                                                   |
+| repo_info_include     | list  | ["remote", "branch", "log"] | Control which parts need to be displayed when viewing git repository information. Support: (path,remote,branch,log,summary) |
+| repo_auto_append      | bool  | False                       | Whether auto append path to repos.                                                                                          |
+| log_debug             | bool  | False                       | Whether run PIGIT in debug mode.                                                                                            |
+| log_output            | bool  | False                       | Whether output log in terminal.                                                                                             |
 
 ## Extra cmds
 
 You can setting your custom cmds. It need create a `extra_cmds.py` file at the **pigit** home. And writing like this:
 
 ```python
 import os
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pigit-1.6.1/pigit/__init__.py` & `pigit-1.7.0/pigit/__init__.py`

 * *Files identical despite different names*

### Comparing `pigit-1.6.1/pigit/cmdparse/parser.py` & `pigit-1.7.0/pigit/cmdparse/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,62 @@
 # -*- coding:utf-8 -*-
 
+from argparse import (
+    ArgumentParser,
+    HelpFormatter,
+    Namespace,
+    _SubParsersAction,
+)
+from functools import wraps
+from shutil import get_terminal_size
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Sequence,
     Tuple,
+    Type,
+    TypedDict,
     Union,
     overload,
 )
-from argparse import (
-    Namespace,
-    ArgumentParser,
-    HelpFormatter,
-    _SubParsersAction,
-)
-from shutil import get_terminal_size
-from plenty.style import Style
 
+from plenty.style import Style
 
 if TYPE_CHECKING:
     from argparse import Action, FileType, _ArgumentGroup
 
-FormatterStyle = Union[Style, str, None]
+
+class ParserOptions(TypedDict, total=False):
+    title: Optional[str]
+    description: Optional[str]
+    parser_class: Optional["Parser"]
+    action: Optional["Action"]
+    option_string: Optional[str]
+    dest: Optional[str]
+    required: bool
+    help: Optional[str]
+    metavar: Optional[str]
 
 
 class ColorHelpFormatter(HelpFormatter):
     """Formatter for generating usage messages and argument help strings.
     This class inherits `argparse.HelpFormatter` and rewrites some methods
     to complete customization.
     """
 
-    usage_style: FormatterStyle = "bold"
-    text_style: FormatterStyle = "i sky_blue"
-    command_style: FormatterStyle = "ok"
-    help_style: FormatterStyle = "i yellow"
+    usage_style: str = "bold"
+    text_style: str = "i sky_blue"
+    command_style: str = "ok"
+    help_style: str = "i yellow"
 
     def __init__(
         self,
         prog: str,
         indent_increment: int = 2,
         max_help_position: int = 24,
         width: Optional[int] = None,
@@ -56,15 +69,15 @@
 
         super().__init__(prog, indent_increment, max_help_position, width)
 
     def _format_usage(
         self,
         usage: str,
         actions: Iterable["Action"],
-        groups: Iterable["_ArgumentGroup"],
+        groups: Iterable,
         prefix: Optional[str],
     ) -> str:
         return Style.parse(self.usage_style).render(
             super()._format_usage(usage, actions, groups, prefix)
         )
 
     def _format_text(self, text: str) -> str:
@@ -77,14 +90,15 @@
         action_width = help_position - self._current_indent - 2
         action_header = self._format_action_invocation(action)
 
         # no help; start on same line and add a final newline
         if not action.help:
             tup = self._current_indent, "", action_header
             action_header = "%*s%s\n" % tup
+            indent_first = 0
 
         # short action name; start on the same line and pad two spaces
         elif len(action_header) <= action_width:
             tup = self._current_indent, "", action_width, action_header
             action_header = "%*s%-*s  " % tup
             indent_first = 0
 
@@ -111,16 +125,16 @@
             )
 
         elif not action_header.endswith("\n"):
             parts.append("\n")
 
         # if there are any sub-actions, add their help as well
         parts.extend(
-            self._format_action(subaction)
-            for subaction in self._iter_indented_subactions(action)
+            self._format_action(sub_action)
+            for sub_action in self._iter_indented_subactions(action)
         )
 
         # return a single string
         return self._join_parts(parts)
 
 
 class ParserError(Exception):
@@ -130,16 +144,16 @@
 class Parser(ArgumentParser):
     def __init__(
         self,
         prog: Optional[str] = None,
         usage: Optional[str] = None,
         description: Optional[str] = None,
         epilog: Optional[str] = None,
-        parents: Sequence[ArgumentParser] = None,
-        formatter_class: Sequence[HelpFormatter] = ColorHelpFormatter,
+        parents: Optional[Sequence[ArgumentParser]] = None,
+        formatter_class: Type[HelpFormatter] = ColorHelpFormatter,
         prefix_chars: str = "-",
         fromfile_prefix_chars: Optional[str] = None,
         argument_default: Any = None,
         conflict_handler: str = "error",
         add_help: bool = True,
         allow_abbrev: bool = True,
         # exit_on_error: bool = True,  # python3.9 feature
@@ -164,16 +178,18 @@
 
         self.subparsers_action: Optional["_SubParsersAction"] = None
         self.default_callback = callback
 
     # ================================
     # overload ~ArgumentParser method
     # ================================
-    def add_subparsers(self, **kwargs):
-        self.subparsers_action = super().add_subparsers(**kwargs)
+    def add_subparsers(self, **kwargs) -> "_SubParsersAction":
+        # cannot have multiple subparser arguments
+        if self.subparsers_action is None:
+            self.subparsers_action = super().add_subparsers(**kwargs)
         return self.subparsers_action
 
     # ============
     # call method
     # ============
     def main(self, args: Optional[List[str]] = None, **kwargs):
         known_args: Namespace
@@ -191,15 +207,15 @@
         self.main(args, **kwds)
 
     # ===============================
     # tools methods of serialization
     # ===============================
     @classmethod
     def from_dict(cls, parser_dict: Dict) -> "Parser":
-        """Parse a `dict` to genrate a ~Parser."""
+        """Parse a `dict` to generate a ~Parser."""
         from copy import deepcopy
 
         # Use `deepcopy` to ensure that the original dict will not be changed.
         parser_dict = deepcopy(parser_dict)
 
         def add_command(
             handle: Union["Parser", "_ArgumentGroup"],
@@ -208,15 +224,15 @@
         ) -> None:
             """Add command to ~Parser or ~Group object."""
 
             names: List[str] = name.split(" ")
             handle.add_argument(*names, **args)
 
         def parse_args(handle: "Parser", args: Dict) -> None:
-            sub_parsers: Optional["Parser"] = None
+            sub_parsers: Optional["_SubParsersAction"] = None
 
             for name, prop in args.items():
                 # Get command type.
                 prop_type = prop.pop("type", "")
 
                 # If the type is 'groups', it's mean that need create a new custom
                 # group. The command of the group in 'args', so we should iterative
@@ -237,21 +253,19 @@
                 elif prop_type == "sub":
                     #
                     if not sub_parsers:
                         sub_parsers = handle.add_subparsers()
 
                     sub_args: Dict = prop.pop("args", None)
 
-                    sub_handle: Sequence["Parser"] = sub_parsers.add_parser(
-                        name, **prop
-                    )
+                    sub_handle: "Parser" = sub_parsers.add_parser(name, **prop)
 
                     # If `set_defaults` in args, special treatment is required.
-                    set_defaults: Dict = sub_args.get("set_defaults", None)
-                    if set_defaults:
+                    set_defaults = sub_args.get("set_defaults")
+                    if set_defaults is not None:
                         del sub_args["set_defaults"]
                         sub_handle.set_defaults(**set_defaults)
 
                     parse_args(sub_handle, sub_args)
 
                 # Other types will be ignored, and it is considered that the current is
                 # just an ordinary command to add.
@@ -282,15 +296,15 @@
             "dest",
             "default",
             "type",
             "metavar",
             "help",
         ]
 
-        def _process(parser: Sequence["Parser"], target_dict: Dict) -> Dict:
+        def _process(parser: "Parser", target_dict: Dict) -> Dict:
             # Set parser parameters.
             for name in cmd_names:
                 target_dict[name] = getattr(parser, name, None)
 
             # Init `args`.
             target_dict["args"] = args = {}
 
@@ -326,27 +340,32 @@
     # ===============================
     # quick add sub-parser decorator
     # ===============================
     @overload
     def sub_parser(
         self,
         prog: str,
+        *,
         title: Optional[str] = None,
         description: Optional[str] = None,
         parser_class: Optional["Parser"] = None,
         action: Optional["Action"] = None,
         option_string: Optional[str] = None,
         dest: Optional[str] = None,
         required: bool = False,
         help: Optional[str] = None,
         metavar: Optional[str] = None,
-    ) -> "Parser":
+    ) -> Callable[..., "Parser"]:
         ...
 
-    def sub_parser(self, prog: str, **kwargs) -> "Parser":
+    @overload
+    def sub_parser(self, prog: str, **kwargs) -> Callable[..., "Parser"]:
+        ...
+
+    def sub_parser(self, prog: str, **kwargs) -> Callable[..., "Parser"]:
         """Create a new ~Parser of subparser and use the decorator use callback.
         This will also automatically attach all decorated :func:`argument` as
         parameters to the parser.
 
         Args:
             prog (str): the prog name of subparser.
 
@@ -358,17 +377,14 @@
         """
 
         if not isinstance(prog, str):
             raise ParserError(
                 f"The name of sub_parser must be str, but given a {type(prog).__name__}."
             ) from None
 
-        if self.subparsers_action is None:
-            self.add_subparsers()
-
         def decorator(fn: Callable[..., Any]) -> "Parser":
             nonlocal kwargs
             attr_params = kwargs.pop("params", None)
             params = attr_params if attr_params is not None else []
 
             try:
                 decorator_params = fn.__parser_params__
@@ -377,15 +393,16 @@
             else:
                 del fn.__parser_params__
                 params.extend(decorator_params)
 
             if "description" not in kwargs:
                 kwargs["description"] = fn.__doc__
 
-            parser = self.subparsers_action.add_parser(prog, **kwargs)
+            parser = self.add_subparsers().add_parser(prog, **kwargs)
+
             for args, kwargs in params:
                 parser.add_argument(*args, **kwargs)
 
             parser.set_defaults(sub_callback=fn)
 
             return parser
 
@@ -393,36 +410,48 @@
 
 
 # ====================================
 # decorator method of creating parser
 # ====================================
 @overload
 def command(
-    prog: Union[str, Callable, None] = None,
-    cls: Sequence[Parser] = None,
+    prog: Optional[str] = None,
+    cls: Optional[Type[Parser]] = None,
+    *,
     usage: Optional[str] = None,
     description: Optional[str] = None,
     epilog: Optional[str] = None,
-    parents: Sequence[Parser] = None,
-    formatter_class: HelpFormatter = HelpFormatter,
+    parents: Optional[Sequence[Parser]] = None,
+    formatter_class: Type[HelpFormatter] = HelpFormatter,
     prefix_chars: str = "-",
     fromfile_prefix_chars: Optional[str] = None,
     argument_default: Any = None,
     conflict_handler: str = "error",
     add_help: bool = True,
     allow_abbrev: bool = True,
     exit_on_error: bool = True,
     callback: Optional[Callable] = None,
-) -> Parser:
+) -> Callable[..., Parser]:
+    ...
+
+
+@overload
+def command(
+    prog: Optional[str] = None,
+    cls: Optional[Type[Parser]] = None,
+    **attrs,
+) -> Callable[..., Parser]:
     ...
 
 
 def command(
-    prog: Union[str, Callable, None] = None, cls: Sequence[Parser] = None, **attrs
-) -> Parser:
+    prog: Optional[str] = None,
+    cls: Optional[Type[Parser]] = None,
+    **attrs,
+) -> Callable[..., Parser]:
     """Creates a new ~Parser and uses the decorated function as callback.
     This will also automatically attach all decorated :func:`argument` as
     parameters to the parser.
 
     The name of the command defaults to the name of the function with
     underscores replaced by dashes. If you want to change that, you can
     pass the intended name as the first argument.
@@ -459,30 +488,28 @@
         )
 
         for args, kwargs in params:
             cmd.add_argument(*args, **kwargs)
 
         return cmd
 
-    if fn is not None:
-        return decorator(fn)
-
-    return decorator
+    return decorator(fn) if fn is not None else decorator
 
 
 def _param_memo(fn: Callable[..., Any], params) -> None:
     if not hasattr(fn, "__parser_params__"):
         fn.__parser_params__ = []
 
     fn.__parser_params__.append(params)
 
 
 @overload
 def argument(
     name: str,
+    *,
     action: Union[
         Literal[
             "store",
             "store_const",
             "store_true",
             "store_false",
             "append",
@@ -508,14 +535,19 @@
     dest: Optional[str] = None,
     version: Optional[str] = None,
     **kwargs: Any,
 ) -> Callable:
     ...
 
 
+@overload
+def argument(name: str, **kwargs) -> Callable:
+    ...
+
+
 def argument(name: str, **kwargs) -> Callable:
     """Attaches an argument to the parser, allow position or option."""
 
     if not isinstance(name, str):
         raise TypeError(
             f"The type of 'name' must be str, but receive {type(name).__name__}."
         ) from None
```

### Comparing `pigit-1.6.1/pigit/cmdparse/shellcompletion/__init__.py` & `pigit-1.7.0/pigit/cmdparse/completion/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,93 +1,72 @@
 # -*- coding:utf-8 -*-
 
-from typing import Dict, Optional
+from typing import Dict, Optional, Type
 
+from .base import ShellCompletion
 from .bash import BashCompletion
 from .zsh import ZshCompletion
 from .fish import FishCompletion
 
 
-supported_shell = {
+_Supported_Shell: Dict[str, Type[ShellCompletion]] = {
     "bash": BashCompletion,
     "zsh": ZshCompletion,
     "fish": FishCompletion,
 }
 
 
 def shell_complete(
     complete_vars: Dict,
-    script_dir: Optional[str] = None,
     shell: Optional[str] = None,
     prog: Optional[str] = None,
+    script_dir: Optional[str] = None,
     script_name: Optional[str] = None,
-    inject_path: Optional[str] = None,
-    inject: bool = True,
 ) -> None:
-    """Generate completion script source and try to injecting.
+    """Generate completion script source and print.
 
     Args:
         complete_vars (Dict): a dict of ~Parser serialization.
-        script_dir (Optional[str], optional): where the script saved. Defaults to None.
         shell (Optional[str], optional): shell name. Defaults to None.
         prog (Optional[str], optional): cmd prog. Defaults to None.
+        script_dir (Optional[str], optional): where the script saved. Defaults to None.
         script_name (Optional[str], optional): completion script name. Defaults to None.
-        inject_path (Optional[str], optional): where the script injecting. Defaults to None.
-        inject (bool, optional): whether inject script. Defaults to True.
     """
 
-    # check shell validable.
-    shell = get_shell() if shell is None else shell.lower().strip()
+    # check shell effectiveness
+    shell = (
+        get_shell()
+        if shell is None or shell not in _Supported_Shell
+        else shell.lower().strip()
+    )
+
     if not shell:
-        print("No shell be found!")
+        # No shell be found!
+        print("")
         return
 
-    if shell not in supported_shell:
-        print(
-            "shell name '{0}' is not supported, see {1}".format(
-                shell, supported_shell.keys()
-            )
-        )
+    if shell not in _Supported_Shell:
+        # not support shell
+        print("")
         return
 
-    print("\n===Try to add completion ...")
-    print(f":: Completion shell: {repr(shell)}")
-
-    complete_handle = supported_shell[shell](
-        prog, complete_vars, script_dir, script_name, inject_path
+    complete_handle = _Supported_Shell[shell](
+        prog, complete_vars, script_dir, script_name
     )
 
     # try create completion file.
     completion_src = complete_handle.generate_resource()
-    if not inject or not script_dir:
-        print(completion_src)
-        return
-
-    if not complete_handle.write_completion(completion_src):
-        print(":: Write completion script failed!")
-        return None
-    else:
-        print(":: Write completion script success.")
-
-    # try inject to shell config.
-    try:
-        injected = complete_handle.inject_into_shell()
-        if injected:
-            print(":: Source your shell configuration.")
-        else:
-            print(":: Command already exist.")
-    except Exception as e:
-        print(e)
+    print(completion_src)
 
 
 def get_shell() -> str:
     """Gets the currently used shell.
 
     Returns:
-            (str): Current shell string.
+        (str): Current shell string.
     """
     import os
 
     try:
         shell_string = os.environ["SHELL"]
         return shell_string.split("/")[-1].strip()
     except KeyError:
```

### Comparing `pigit-1.6.1/pigit/cmdparse/shellcompletion/base.py` & `pigit-1.7.0/pigit/cmdparse/completion/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 # -*- coding:utf-8 -*-
 
+import os
+import re
 from typing import Dict, Optional, Tuple
-import os, re
 
 
 class ShellCompletionError(Exception):
     """ShellCompletion error class."""
 
     pass
 
 
-class ShellCompletion(object):
+class ShellCompletion:
     """Implement and inject help classes for completion scripts."""
 
-    _SHELL: str  # shell name.
-    _INJECT_PATH: str  # script inject path.
-    _template_source: str  # script tempelate string.
+    SHELL: str  # shell name.
+    TEMPLATE_SRC: str  # script template string.
 
     def __init__(
         self,
         prog_name: Optional[str] = None,
-        complete_vars: Dict = None,
+        complete_vars: Optional[Dict] = None,
         script_dir: Optional[str] = None,
         script_name: Optional[str] = None,
-        inject_path: Optional[str] = None,
     ) -> None:
         """Initialization.
 
         Args:
             prop (str): completion trigger command.
             complete_var (dict): complete arguments dict.
                 >>> complete_vars = {
                 ...     '-h': 'Display help messages',
                 ...     '-v': 'Show version and exit',
                 ... }
             script_dir (str): where is the completion file save.
             script_name (str, optional): completion file name. Defaults to None.
-            inject_path (str, optional): script inject path.
 
         Raises:
             TypeError: when `complete_var` is not dict.
         """
-        super(ShellCompletion, self).__init__()
 
         if not isinstance(complete_vars, dict):
             raise TypeError("complete_var muse be dict.")
         self.complete_vars = complete_vars
 
         if prog_name is not None:
             self.prog_name = prog_name
         elif inner_prog_name := complete_vars.get("prog"):
             self.prog_name = inner_prog_name
         else:
             raise ShellCompletionError("Can't get prog name anywhere.") from None
 
         self.script_dir = script_dir or "."
         self.script_name = script_name or "{0}_{1}_comp".format(
-            self.prog_name, self._SHELL
+            self.prog_name, self.SHELL
         )
-        self.inject_path = inject_path or self._INJECT_PATH
 
     @property
     def func_name(self) -> str:
         """The name of the shell function defined by the completion
         script.
         """
 
@@ -95,90 +91,81 @@
             elif name.startswith("-"):
                 _arguments.append((name, prop.get("help", "_").replace("\n", "")))
             else:
                 _positions.append((name, prop.get("help", "_").replace("\n", "")))
 
         return _arguments, _positions, _sub_opts
 
-    def generate(self):
+    def generate_content(self):
         """Generate script content.
 
         Process self.complete_var to generate completion script content part.
         Due to different shells, the generated formats are different, which
         are finally implemented by subclasses.
+        If this method is not overridden, a string of all commands will be generated.
+        Like: '-h --help cmd repo'.
         """
 
-        raise NotImplementedError()
+        comp_keys = set()
+
+        _arguments, _, _sub_opts = self._parse(self.complete_vars["args"])
+
+        for _argument in _arguments:
+            for handle in _argument[0].split():
+                comp_keys.add(handle)
+
+        sub_q = [_sub_opts]
+        while sub_q:
+            temp: Dict = sub_q.pop(0)
+            for opt_name, p in temp.items():
+                comp_keys.add(opt_name)
+
+                if _arguments := p.get("_arguments"):
+                    for _argument in _arguments:
+                        for handle in _argument[0].split():
+                            comp_keys.add(handle)
+
+                if _opts := p.get("_sub_opts"):
+                    sub_q.insert(-1, _opts)
+
+        return " ".join(comp_keys)
 
     def generate_resource(self) -> str:
-        """Generate completion scirpt.
+        """Generate completion script.
 
         Generate the completion script of the corresponding shell according to
         the template.
 
         Returns:
-            (str): completion source.
+            (str): completion script source.
         """
 
-        complete_content = self.generate()
-        return self._template_source % {
+        complete_content = self.generate_content()
+        return self.TEMPLATE_SRC % {
             "func_name": self.func_name,
             "prop": self.prog_name,
             "complete_vars": complete_content,
         }
 
     def write_completion(self, complete_src: str) -> bool:
-        """Save completion to config path.
+        """Save completion to target path.
 
         Args:
-            complete_src (str): completion source.
+            complete_src (str): completion script source.
 
         Returns:
-            (str): completion full path.
+            (bool): whether saved.
         """
 
         if not os.path.isdir(self.script_dir):
             os.makedirs(self.script_dir, exist_ok=True)
 
         full_path = os.path.join(self.script_dir, self.script_name)
 
         try:
             with open(full_path, "w" if os.path.isfile(full_path) else "x") as f:
                 for line in complete_src:
                     f.write(line)
-        except Exception as e:
+        except Exception:
             return False
         else:
             return True
-
-    def inject_into_shell(self) -> bool:
-        """Try using completion script.
-
-        Inject the load of completion script into the configuration of shell.
-        If it exists in the configuration, the injection will not be repeated.
-        """
-
-        full_script_path = os.path.join(self.script_dir, self.script_name)
-
-        # Check whether already exist.
-        try:
-            with open(self.inject_path, "r") as f:
-                shell_conf = f.read()
-        except Exception as e:
-            raise ShellCompletionError(
-                "Read shell config error: {0}".format(e)
-            ) from None
-        else:
-            _re = re.compile(f"{full_script_path}[^\\s]*")
-            files = _re.findall(shell_conf)
-
-        injected = bool(files)
-        if injected:
-            return False
-
-        try:
-            # Inject.
-            with open(self.inject_path, "a") as f:
-                f.write(f"source {full_script_path}")
-        except Exception as e:
-            raise ShellCompletionError(f"Inject error: {str(e)}") from None
-        return True
```

### Comparing `pigit-1.6.1/pigit/cmdparse/shellcompletion/zsh.py` & `pigit-1.7.0/pigit/cmdparse/completion/zsh.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding:utf-8 -*-
 
-from typing import Dict, List
-import os
 import textwrap
+from typing import Dict, List
 
 from .base import ShellCompletion
 
 _TEMPLATE_ZSH: str = """\
 #compdef %(prog)s
 
 #--------------------------------------------------------------------
@@ -49,25 +48,19 @@
 %s
   && ret=0
 }
 """
 
 
 class ZshCompletion(ShellCompletion):
+    SHELL: str = "zsh"
 
-    _SHELL: str = "zsh"
-
-    try:
-        _INJECT_PATH: str = os.environ["HOME"] + "/.zshrc"
-    except:
-        _INJECT_PATH: str = ""
+    TEMPLATE_SRC: str = _TEMPLATE_ZSH
 
-    _template_source: str = _TEMPLATE_ZSH
-
-    def _process_arguments(self, _arguments) -> str:
+    def _process_arguments(self, _arguments) -> List[str]:
         res = []
 
         for one in _arguments:
             names = one[0].split()
             # help msg not allow include `[]`
             help_str = one[1].replace("[", "`").replace("]", "`")
 
@@ -138,23 +131,27 @@
 
         if _sub_opts:
             _subs = [
                 f"'{opt_name}[{opt_args['help']}]' \\"
                 for opt_name, opt_args in _sub_opts.items()
             ]
 
-            _sub_opt_str = textwrap.dedent(
-                """
-                ######################
-                # sub-commands helper
-                ######################
-                """
-            ) + _TEMP_V % (
-                "sub_opt",
-                textwrap.indent("\n".join(_subs), "    "),
+            _sub_opt_str = (
+                textwrap.dedent(
+                    """
+                    ######################
+                    # sub-commands helper
+                    ######################
+                    """
+                )
+                + _TEMP_V
+                % (
+                    "sub_opt",
+                    textwrap.indent("\n".join(_subs), "    "),
+                )
             )
 
             self._process_sub_commands(
                 _sub_opts, _sub_sub_opt_comps, _sub_relationship, idx=1
             )
 
         _opt_case_str = ""
@@ -174,15 +171,15 @@
             _opt_case_str += textwrap.indent("\n".join(_sub_relationship), " " * 4)
 
         if _opt_case_str:
             _opt_case_str += "esac"
 
         arguments_str = _TEMP_A % textwrap.indent("\n".join(_arguments), " " * 2)
 
-        return self._template_source % {
+        return self.TEMPLATE_SRC % {
             "func_name": self.func_name,
             "prog": self.prog_name,
             "tools": "\n".join([*_sub_sub_opt_comps, _sub_opt_str]),
             "arguments": textwrap.indent(arguments_str, " " * 2),
             "cases": textwrap.indent(_opt_case_str, " " * 2),
         }
```

### Comparing `pigit-1.6.1/pigit/codecounter.py` & `pigit-1.7.0/pigit/ext/lcstat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,146 @@
-# -*- coding:utf-8 -*-
-
-from typing import Dict, List, Literal, Optional, Tuple, Union, Any
-import os, re, json, stat
-import logging
+import contextlib
+import copy
+import json
+import os
+import re
+import stat
 import threading
-import concurrent.futures
-from shutil import get_terminal_size
-
-from plenty.table import Table
-from plenty import get_console
+from concurrent.futures import ProcessPoolExecutor
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple
 
-from .common.utils import confirm, get_file_icon, adjudgment_type
+from .log import logger
+from .utils import adjudgment_type, confirm
 
+if TYPE_CHECKING:
+    from concurrent.futures import Future
 
-Logger = logging.getLogger(__name__)
 
+FILES_NUM = "1"
+LINES_NUM = "2"
+FILES_CHANGE = "3"
+LINES_CHANGE = "4"
+
+Absolute_Rules: List[Dict] = [
+    # Exclude `.git` folder.
+    {"pattern": re.compile(r"\.git$|\.git\/"), "include": False},
+    {
+        # Exclude all picture formats.
+        "pattern": re.compile(
+            r"\.xbm$|\.tif$|\.pjp$|\.svgz$|\.jpg$|\.jpeg$|\.ico$|\.icns$|\.tiff$|\.gif$|\.svg$|\.jfif$|\.webp$|\.png$|\.bmp$|\.jpeg$|\.avif$",
+            re.I,
+        ),
+        "include": False,
+    },
+    {
+        # Exclude all video formats.
+        "pattern": re.compile(
+            r"\.avi$|\.rmvb$|\.rm$|\.asf$|\.divx$|\.mpg$|\.mpeg$|\.mpe$|\.wmv$|\.mp4$|\.mkv$|\.vob$",
+            re.I,
+        ),
+        "include": False,
+    },
+    {
+        # Exclude all audio frequency formats.
+        "pattern": re.compile(
+            r"\.mp3$|\.wma$|\.mid[i]?$|\.mpeg$|\.cda$|\.wav$|\.ape$|\.flac$|\.aiff$|\.au$",
+            re.I,
+        ),
+        "include": False,
+    },
+    {
+        # Exclude all font formats.
+        "pattern": re.compile(
+            r"\.otf$|\.woff$|\.woff2$|\.ttf$|\.eot$",
+            re.I,
+        ),
+        "include": False,
+    },
+    {
+        # Exclude some binary file.
+        "pattern": re.compile(
+            r"\.exe$|\.bin$",
+            re.I,
+        ),
+        "include": False,
+    },
+]
 
-CounterFormatType = Literal["simple", "table"]
+_Lock_Cache = {}
 
 
-class CodeCounter(object):
-    """Class of statistical code.
+def default_walk_err_callback(e):
+    """Default callback when has error on `walk`.
 
-    Attributes:
-        Absolute_Rules (dict): Precompiled rules.
-        Suffix_Type (dict): Supported file suffix dictionary.
-        Special_Name (dict): Type dict of special file name.
-            subscript, and the codes of different levels are colored
-            when the results are output.
-        symbol (dict):
+    Args:
+        e (_type_): _description_
     """
 
-    # The default rule is to count only files. Ignore all video, audio, fonts, binaries.
-    Absolute_Rules: List[Dict] = [
-        # Exclude `.git` folder.
-        {"pattern": re.compile(r"\.git$|\.git\/"), "include": False},
-        {
-            # Exclude all picture formats.
-            "pattern": re.compile(
-                r"\.xbm$|\.tif$|\.pjp$|\.svgz$|\.jpg$|\.jpeg$|\.ico$|\.icns$|\.tiff$|\.gif$|\.svg$|\.jfif$|\.webp$|\.png$|\.bmp$|\.jpeg$|\.avif$",
-                re.I,
-            ),
-            "include": False,
-        },
-        {
-            # Exclude all video formats.
-            "pattern": re.compile(
-                r"\.avi$|\.rmvb$|\.rm$|\.asf$|\.divx$|\.mpg$|\.mpeg$|\.mpe$|\.wmv$|\.mp4$|\.mkv$|\.vob$",
-                re.I,
-            ),
-            "include": False,
-        },
-        {
-            # Exclude all audio frequency formats.
-            "pattern": re.compile(
-                r"\.mp3$|\.wma$|\.mid[i]?$|\.mpeg$|\.cda$|\.wav$|\.ape$|\.flac$|\.aiff$|\.au$",
-                re.I,
-            ),
-            "include": False,
-        },
-        {
-            # Exclude all font formats.
-            "pattern": re.compile(
-                r"\.otf$|\.woff$|\.woff2$|\.ttf$|\.eot$",
-                re.I,
-            ),
-            "include": False,
-        },
-        {
-            # Exclude some binary file.
-            "pattern": re.compile(
-                r"\.exe$|\.bin$",
-                re.I,
-            ),
-            "include": False,
-        },
-    ]
+    print("Walk error: {0}".format(e))
+
+
+class CounterLockManageError(Exception):
+    """Error class for ~CounterLockManage"""
+
 
-    _Lock = threading.Lock()
+class CounterLockManage:
+    """Generate lock with multi ~Counter"""
+
+    def __init__(self, obj: "Counter") -> None:
+        self.id: int = id(obj)
+
+    def __enter__(self):
+        _Lock_Cache[self.id] = threading.Lock()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        del _Lock_Cache[self.id]
+
+    @classmethod
+    def get(cls, obj: "Counter"):
+        lock = _Lock_Cache.get(id(obj))
+        if lock is None:
+            raise CounterLockManageError(f"Can not find lock with '{obj}'")
 
+        return lock
+
+
+class Counter:
     def __init__(
         self,
-        *,
-        count_path: Optional[str] = None,
-        format_type: CounterFormatType = "table",
-        use_ignore: bool = True,
-        use_icon: bool = True,
-        result_saved_path: str = "",
-        whether_save: bool = True,
-        color: bool = True,
+        walk_err_cb: Optional[Callable] = None,
+        saved_dir: Optional[str] = None,
         show_invalid: bool = False,
     ) -> None:
         """
         Args:
-            count_path (str, optional): The path of needed count. Defaults to os.getcwd().
-            use_ignore (bool, optional): Whether detect `.gitignore` file. Defaults to True.
-            result_saved_path (str, optional): Result save path. Defaults to "".
-            result_format (str, optional): Output format string. Defaults to "table".
-            use_icon (bool, optional): Whether output with icon. Defaults to False.
-
+            walk_err_cb (Optional[Callable], optional): Callback function when
+                has walk error. Defaults to None.
+            show_invalid (bool, optional): Whether show invalid files. Defaults to False.
         """
-        # Store the rules obtained after processing.
-        self.Rules: List = []
+        self.rules = []
+
+        self.walk_err_cb = (
+            walk_err_cb if walk_err_cb is not None else default_walk_err_callback
+        )
 
-        self.count_path = count_path or os.getcwd()
-        self.format_type = format_type
-        self.use_ignore = use_ignore
-        self.use_icon = use_icon
-        self.result_saved_path = result_saved_path
-        self.whether_save = whether_save
-        self.color = color
+        self.saved_dir = saved_dir or ""
         self.show_invalid = show_invalid
 
+        with contextlib.suppress(Exception):
+            os.makedirs(self.saved_dir, exist_ok=True)
+
     def parse_gitignore2rule(self, root: str) -> None:
         """Process `.gitignore` files and add matching rules.
 
         Args:
             root (str): Absolute or relative path to the directory.
-            files (list): The list of all file names under the `root` path.
         """
-
         root = root.replace("\\", "/")  # Unified symbol.
         ignore_path = os.path.join(root, ".gitignore")
+
         try:
             with open(ignore_path) as f:
                 ignore_content = filter(
                     # Filter out comment lines.
                     lambda x: x and not x.startswith("#"),
                     map(
                         # Filter out white space lines.
@@ -160,144 +175,154 @@
                 item = re.sub(r"(^|[^\\])\?", ".", item)
                 item = re.sub(r"\/\*\*", "([\\\\/][^\\\\/]+)?", item)  # /**
                 item = re.sub(r"\*\*\/", "([^\\\\/]+[\\\\/])?", item)  # **/
                 item = re.sub(r"\*", "([^\\\\/]+)", item)  # for `*`
                 item = re.sub(r"\?", "*", item)  # for `?``
                 item = re.sub(r"([^\/])$", r"\1(([\\\\/].*)|$)", item)
                 item = re.sub(r"\/$", "(([\\\\/].*)|$)", item)  # for trialing with `/`
-                self.Rules.append({"pattern": re.compile(item), "include": is_negative})
+                self.rules.append({"pattern": re.compile(item), "include": is_negative})
 
     def matching_rules(self, full_path: str) -> bool:
         """Matching rules.
 
         Judge whether it is the required file according to the rule matching path.
         Returns `True` if the file not needs to be ignored, or `False` if needs.
 
         Args:
             full_path (str): File full path for matching.
+
+        Returns:
+            (bool): Whether the file is valid or not needs to be counted.
         """
 
         # Precompiled rules have the highest priority.
-        if list(
-            filter(lambda rule: rule["pattern"].search(full_path), self.Absolute_Rules)
-        ):
+        if list(filter(lambda rule: rule["pattern"].search(full_path), Absolute_Rules)):
             return False
 
         # Matching the generated rules.
-        res = list(filter(lambda rule: rule["pattern"].search(full_path), self.Rules))
-        if not res:
-            return True
+        res = list(filter(lambda rule: rule["pattern"].search(full_path), self.rules))
 
         # If multiple rules match successfully, we think the last rule added has
         # the highest priority. Or if just one, this no problem also.
-        return res[-1]["include"]
+        return res[-1]["include"] if res else True
         # selected_rule = max(res, key=lambda rule: len(str(rule["pattern"])))
 
-    def _sub_count(self, root: str, files: List) -> tuple:
-        """Process handle use by `self.count`."""
-        show_invailed = self.show_invalid
-
-        result: dict[str[dict[str, int]]] = {}  # type: dict[str,dict]
-        valid_counter = invalid_counter = 0
-        invalid_list: list[str] = []
-        total_size: int = 0
+    def count_files(
+        self, root: str, files: List[str]
+    ) -> Tuple[int, Dict[str, Dict[str, int]], List[str], int, int]:
+        """Statistics files.
+
+        Args:
+            root (str): Absolute or relative path to the directory.
+            files (List[str]): The list of all file names under the `root` path.
+
+        Returns:
+            Tuple[int, Dict, List[str], int, int]: total size of file,
+                result dict, invalid file list, invalid file num, valid file num.
+        """
+        total_size = 0
+        result = {}
+        invalids = []
+        invalid_num = 0
+        valid_num = 0
 
         for file in files:
             full_path = os.path.join(root, file)
-            is_effective = self.matching_rules(full_path)
-            if is_effective:
+
+            if is_effective := self.matching_rules(full_path):
                 try:
                     # Try read size of the valid file. Then do sum calc.
                     file_size = os.path.getsize(full_path)
-                    total_size += file_size
-                except:
-                    Logger.warn(f"Can't read size of '{full_path}'")
+                except Exception:
+                    file_size = 0
+                    logger(__name__).warn(f"Can't read size of '{full_path}'")
 
-                # Get file type.
+                total_size += file_size
                 file_type = adjudgment_type(file, original=True)
                 try:
                     with open(full_path) as f:
-                        count = len(f.read().split("\n"))
+                        count = sum(1 for _ in f)
+
+                        # Superposition.
+                        if result.get(file_type) is None:
+                            result[file_type] = {FILES_NUM: 1, LINES_NUM: count}
+                        else:
+                            result[file_type][FILES_NUM] += 1
+                            result[file_type][LINES_NUM] += count
+
+                        valid_num += 1
                 except Exception:
-                    if show_invailed:
-                        invalid_list.append(file)
-                    invalid_counter += 1
+                    invalid_num += 1
+
+                    if self.show_invalid:
+                        invalids.append(file)
+
                     continue
-                else:
-                    # Superposition.
-                    if result.get(file_type) is None:
-                        result[file_type] = {"files": 1, "lines": count}
-                    else:
-                        result[file_type]["files"] += 1
-                        result[file_type]["lines"] += count
-                    valid_counter += 1
-
-        return result, total_size, valid_counter, invalid_counter, invalid_list
-
-    @staticmethod
-    def _walk_err_callback(e):
-        """Handle of processing walk error."""
-        print("Walk error: {0}".format(e))
-        return
 
-    def count(self) -> Tuple[Dict, List, List]:
-        """Statistics file and returns the result dictionary for Python3.
+        return total_size, result, invalids, invalid_num, valid_num
 
-        Args:
-            root_path (str): The path is walk needed.
-            use_ignore (bool): Whether ignore files in `.gitignore`. Defaults to True.
-            progress (bool): Whether show processing. Defaults to True.
+    def update_dfd(self, src_d: Dict, d: Dict):
+        if not d:
+            return
+
+        for k, v in d.items():
+            if src_d.get(k) is None:
+                src_d[k] = v
+            else:
+                v_type = type(v)
 
-        Return:
-            result (dict): Dictionary containing statistical results.
-            invalid_list (list): invalid file list.
-            total_size (int): the sum size of all valid files.
-
-            result = {
-                'Python': {
-                    'files': 5,
-                    'lines': 2124,
-                }
-            }
+                if v_type == int:
+                    src_d[k] += v
+                elif v_type == list:
+                    src_d[k].extend(v)
+                elif v_type == dict:
+                    self.update_dfd(src_d[k], v)
+
+    def count_with_multiprocessing(
+        self, root_path: str, use_ignore: bool
+    ) -> Tuple[int, Dict[str, Dict[str, int]], List[str]]:
         """
-        root_path = self.count_path
-        use_ignore = self.use_ignore
-
-        result = {}  # type: dict[str,dict]
-        data_count = [0, 0, 0]  # [total_size, valid_count, invalid_count]
-        invalid_list = []  # Invalid file list.
+        Args:
+            root_path (str): The directory path to be counted.
+            use_ignore (bool): Whether gitignore files in convenience
+                directories need to be recognized, and rules generated.
+
+        Returns:
+            Tuple[int, Dict[str, Dict[str, int]], List]: total size,
+                result dict, invalid file list.
+        """
+        total_size: int = 0
+        result: Dict[str, Dict[str, int]] = {}
+        invalids: List[str] = []
+        invalid_num: int = 0
+        valid_num: int = 0
 
-        def _callback(r):
+        def _cb(r: "Future"):
+            nonlocal total_size, result, invalids, invalid_num, valid_num
             (
-                _result,
-                _total_size,
-                _valid_counter,
-                _invalid_counter,
-                _invalid_list,
+                sub_total_size,
+                sub_result,
+                sub_invalids,
+                sub_invalid_num,
+                sub_valid_num,
             ) = r.result()
 
-            with self._Lock:
-                for key, values in _result.items():
-                    if result.get(key) is None:
-                        result[key] = values
-                    else:
-                        result[key]["files"] += _result[key]["files"]
-                        result[key]["lines"] += _result[key]["lines"]
-
-                data_count[0] += _total_size
-                data_count[1] += _valid_counter
-                data_count[2] += _invalid_counter
-                invalid_list.extend(_invalid_list)
-
-        cpu: int = os.cpu_count() or 1
-        max_queue: int = cpu * 200
-        print("Detect CPU count: {0}, start record ...".format(cpu))
-
-        with concurrent.futures.ProcessPoolExecutor() as pool:
-            for root, _, files in os.walk(root_path, onerror=self._walk_err_callback):
+            with CounterLockManage.get(self):
+                total_size += sub_total_size
+                self.update_dfd(result, sub_result)
+                invalids.extend(sub_invalids)
+                invalid_num += sub_invalid_num
+                valid_num += sub_valid_num
+
+        max_queue: int = (os.cpu_count() or 1) * 50
+
+        with CounterLockManage(self), ProcessPoolExecutor(
+            max_workers=(os.cpu_count() or 1) + 4
+        ) as pool:
+            for root, _, files in os.walk(root_path, onerror=self.walk_err_cb):
                 if not files:
                     continue
 
                 # Judge whether the directory is valid. Invalid directories
                 # do not traverse files.
                 is_effective_dir = self.matching_rules(root)
                 if not is_effective_dir:
@@ -306,245 +331,85 @@
                 # Process ``.gitignore`` file, add custom rules.
                 if use_ignore and ".gitignore" in files:
                     self.parse_gitignore2rule(root)
 
                 # If the number of files(exclude sub dir) in the directory is greater
                 # than 15 and the number of enabled processes does not exceed the upper
                 # limit, enable process traversal.
-                if len(files) >= 15 and pool._queue_count < max_queue:
-                    # Calling process.
-                    future_result = pool.submit(self._sub_count, root, files)
-                    future_result.add_done_callback(_callback)
+                # The `add_done_callback` method will execute the callback function in
+                # a multi-threaded environment in the main process.
+                if len(files) >= 15 or pool._queue_count < max_queue:
+                    future_res = pool.submit(self.count_files, root, files)
+                    future_res.add_done_callback(_cb)
                 else:
-                    (
-                        _result,
-                        _total_size,
-                        _valid_counter,
-                        _invalid_counter,
-                        _invalid_list,
-                    ) = self._sub_count(root, files)
-
-                    with self._Lock:
-                        for key, values in _result.items():
-                            if result.get(key, None) is None:
-                                result[key] = values
-                            else:
-                                result[key]["files"] += _result[key]["files"]
-                                result[key]["lines"] += _result[key]["lines"]
-
-                        data_count[0] += _total_size
-                        data_count[1] += _valid_counter
-                        data_count[2] += _invalid_counter
-                        invalid_list.extend(_invalid_list)
-
-        # Some processes may not be finished after synchronization.
-        print("\nPlease wait calculate ...")
-
-        return result, invalid_list, data_count[0]
-
-    def _get_saved_path(self, root_path: str) -> str:
-        file_name: str = (
-            root_path.replace("/", "_").replace("\\", "_").replace(".", "_")
-        )
-        return os.path.join(self.result_saved_path, file_name)
+                    self.count_files(root, files)
+
+        return total_size, result, invalids
 
-    def load_recorded_result(self, root_path: str) -> Optional[Dict]:
+    def count(self, root_path: str, use_ignore: bool):
+        return self.count_with_multiprocessing(root_path, use_ignore)
+
+    def _saved_path(self, root_path: str) -> str:
+        """Generate saved path."""
+        file_name = root_path.replace("/", "_").replace("\\", "_").replace(".", "_")
+        return os.path.join(self.saved_dir, file_name)
+
+    def load(self, root_path: str) -> Dict[str, Dict[str, int]]:
         """Load count result."""
-        file_path = self._get_saved_path(root_path)
+        file_path = self._saved_path(root_path)
+
         try:
-            with open(file_path, "r") as rf:
-                res = json.load(rf)
+            with open(file_path, "r") as f:
+                res: Dict = json.load(f)
+                return res
         except Exception:
-            return None
-        else:
-            return res
+            return {}
 
-    def save_result(self, result: Dict, root_path: str) -> bool:
+    def dump(self, root_path: str, result: Dict) -> bool:
         """Save count result.
 
-        Generate name according to `root_path`, then try save the record
-        result to [`TOOLS_HOME`/Counter].
-
         Args:
-            result (dict): Statistical results.
             root_path (str): Traversal directory.
+            result (dict): Statistical result.
 
         Return:
             (bool): Whether saving successful.
         """
+        file_path = self._saved_path(root_path)
 
-        file_path = self._get_saved_path(root_path)
         try:
-            with open(file_path, "w" if os.path.isfile(file_path) else "x") as wf:
-                json.dump(result, wf, indent=2)
-        except Exception:
+            with open(file_path, "w" if os.path.isfile(file_path) else "x") as f:
+                json.dump(result, f, indent=2)
+                return True
+        except Exception as e:
+            logger(__name__).warning(f"Dump counter result with error: {e}")
             return False
-        else:
-            return True
-
-    def simple_output(self, result: Dict) -> str:
-        gen = []
-        for key, value in result.items():
-            line = f"::{key}  (files:{value['files']:,} | lines:{value['lines']:,})"
-            gen.append(line)
-
-        return "\n".join(gen)
-
-    def table_output(self, new: Dict, old: Dict) -> Table:
-        use_icon = self.use_icon
-        color = self.color
-
-        tb = Table(title="[Code Counter Result]", title_style="bold")
-        tb.add_column("Language")
-        tb.add_column("Files")
-        tb.add_column("Code lines")
-
-        # Diff
-        sum_lines = 0
-        for key, value in new.items():
-            files = value["files"]
-            lines = value["lines"]
-            # Calc sum code line.
-            sum_lines += lines
-
-            file_type_str = (
-                "{0} {1}".format(get_file_icon(key), key) if use_icon else key
-            )
-            files_str = f"{files:,}"
-            lines_str = f"{lines:,}"
-
-            if color:
-                file_type_str = f"`{file_type_str}`<cyan>"
-                files_str = f"`{files_str}`<{self.color_index(files)}>"
-                lines_str = f"`{lines_str}`<{self.color_index(lines)}>"
-
-            # Compare change.
-            if isinstance(old, dict) and old.get(key) is not None:
-                old_files = old.get(key).get("files", None)
-                old_lines = old.get(key).get("lines", None)
-
-                if old_files and old_files != files:
-                    files_change = "{:+}".format(files - old_files)
-                else:
-                    files_change = ""
-
-                if old_lines and old_lines != lines:
-                    lines_change = "{:+}".format(lines - old_lines)
-                else:
-                    lines_change = ""
 
+    def diff_count(
+        self, root_path: str, use_ignore: bool
+    ) -> Tuple[str, Dict[str, Dict[str, int]], List[str]]:
+        total_size, result, invalids = self.count(root_path, use_ignore)
+        result_old = self.load(root_path)
+
+        diff_result = {}
+        for k, info in result.items():
+            temp = diff_result[k] = copy.deepcopy(info)
+
+            info_old = result_old.get(k)
+            if info_old is not None:
+                temp[FILES_CHANGE] = temp.get(FILES_NUM, 0) - info_old.get(FILES_NUM, 0)
+                temp[LINES_CHANGE] = temp.get(LINES_NUM, 0) - info_old.get(LINES_NUM, 0)
+
+        # update saved result.
+        self.dump(root_path, result)
+
+        # optimize size unit.
+        size_unit = ["byte", "KB", "MB", "GB"]
+        for i in range(3):
+            if total_size >= 1024:
+                total_size /= 1024
             else:
-                files_change = lines_change = ""
-
-            if color:
-                files_change_str = f"`{files_change}`<{'#98fb98' if files_change.startswith('+') else '#ff6347'}>"
-                lines_change_str = f"`{lines_change}`<{'#98fb98' if lines_change.startswith('+') else '#ff6347'}>"
-            else:
-                files_change_str = files_change
-                lines_change_str = lines_change
-
-            tb.add_row(
-                file_type_str,
-                f"{files_str} {files_change_str}",
-                f"{lines_str} {lines_change_str}",
-            )
-
-        # Print total and change graph.
-        tb.caption = " Total: {0} lines".format(sum_lines)
-        return tb
-
-    @classmethod
-    def color_index(
-        cls, count: int, level_color: Union[List, Tuple, None] = None
-    ) -> int:
-        # Colors displayed for different code quantities.
-        if level_color is None:
-            level_color = (
-                "green",
-                "#EBCB8C",  # yellow
-                "#FF6347",  # tomato
-                "#C71585",  # middle violet red
-                "#87CEFA",  # skyblue
-            )
-        index = len(str(count // 1000))
-        return level_color[-1] if index > len(level_color) else level_color[index - 1]
-
-    def generate_format_output(self, new: Dict, old: Optional[Dict] = None) -> Any:
-        """Print result with color and diff.
-
-        If the console width is not enough, the output is simple.
-
-        Args:
-            new (dict): Current statistical results.
-            old (dict|None): The results saved in the past may not exist.
-        """
-
-        result_format = self.format_type
-
-        needed_width: int = 67
-        width, _ = get_terminal_size()
-        if result_format == "simple" or width < needed_width:
-            return self.simple_output(new)
-
-        elif result_format == "table":
-            return self.table_output(new, old)
-
-    def run(
-        self,
-        whether_output: bool = True,
-        *,
-        count_path: Optional[str] = None,
-        format_type: Optional[CounterFormatType] = None,
-        use_ignore: Optional[bool] = None,
-        use_icon: Optional[bool] = None,
-        result_saved_path: Optional[str] = None,
-        whether_save: Optional[bool] = None,
-        color: Optional[bool] = None,
-        show_invalid: Optional[bool] = None,
-    ) -> None:
-        if count_path is not None:
-            self.count_path = count_path
-        if format_type is not None:
-            self.format_type = format_type
-        if use_ignore is not None:
-            self.use_ignore = use_ignore
-        if use_icon is not None:
-            self.use_icon = use_icon
-        if result_saved_path is not None:
-            self.result_saved_path = result_saved_path
-        if whether_save is not None:
-            self.whether_save = whether_save
-        if color is not None:
-            self.color = color
-        if show_invalid is not None:
-            self.show_invalid = show_invalid
-
-        result, invalid_list, total_size = self.count()
-
-        old_result = self.load_recorded_result(self.count_path)
-
-        # diff print.
-        if whether_output:
-            output = self.generate_format_output(result, old_result)
-            get_console().echo(output)
-
-            if self.whether_save:
-                self.save_result(result, self.count_path)
-            if (
-                self.show_invalid
-                and invalid_list
-                and confirm("Whether print invalid file list?[y/n]", default=False)
-            ):
-                print(invalid_list)
-
-            # optimize size unit.
-            size_unit = ["byte", "KB", "MB", "GB"]
-            for i in range(3):
-                if total_size >= 1024:
-                    total_size /= 1024
-                else:
-                    break
-            else:
-                i = 3
-            print("Files total size: {0:.2f}{1}".format(total_size, size_unit[i]))
+                break
+        else:
+            i = 3
 
-        return result
+        return "{0:.2f}{1}".format(total_size, size_unit[i]), diff_result, invalids
```

### Comparing `pigit-1.6.1/pigit/common/func.py` & `pigit-1.7.0/pigit/ext/func.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def time_it(fn: Callable) -> Callable:
     """Print the overall running time.
     When recursive calls exist, only the outermost layer is printed.
     """
     time_it.deep = 0  # Mark recursion levels.
-    time_unit = ["second", "mintue", "hour"]
+    time_unit = ["second", "minute", "hour"]
 
     @wraps(fn)
     def wrap(*args, **kwargs):
         time_it.deep += 1
         start_time = time.time()
         res = None
         with contextlib.suppress(SystemExit, EOFError):
@@ -27,15 +27,15 @@
             for i in range(2):
                 if used_time >= 60:
                     used_time /= 60
                 else:
                     break
             else:
                 i = 2
-            print("\nruntime: {0:.2f} {1}".format(used_time, time_unit[i]))
+            print("\n# runtime: {0:.2f} {1}".format(used_time, time_unit[i]))
         return res
 
     return wrap
 
 
 def dynamic_default_attrs(fn: Callable, **kwds: Any) -> Callable:
     """Set default parameters dynamically.
```

### Comparing `pigit-1.6.1/pigit/common/utils.py` & `pigit-1.7.0/pigit/ext/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,77 @@
 # -*- coding:utf-8 -*-
 
-from typing import Callable, Dict, Iterable, List, Optional, Tuple, ByteString, Union
-import sys, subprocess, asyncio
-from math import sqrt
+import sys
 from collections import Counter
+from math import sqrt
+from typing import Iterable, Tuple, Dict
+
+
+def strtobool(s: str) -> bool:
+    """Convert a string representation of truth to true (1) or false (0).
+
+    Raises:
+        ValueError: if val is anything else.
+
+    Returns:
+        bool
+
+    Docs Test:
+        >>> strtobool('y')
+        True
+        >>> strtobool('Y')
+        True
+        >>> strtobool('n')
+        False
+        >>> strtobool('N')
+        False
+    """
+    s = s.lower()
+
+    if s in {"y", "yes", 't', 'true', "on", "1"}:
+        return True
+    elif s in {"n", "no", "f", "false", "off", "0"}:
+        return False
+    else:
+        raise ValueError('Not support string.')
 
 
 def traceback_info(extra_msg: str = "null") -> str:
-    """Get traceback infomation.
+    """Get traceback information.
 
     Args:
         extra_msg (str, optional): extra custom message. Defaults to "null".
 
     Returns:
-        str: formated traceback infomation.
+        str: formatted traceback information.
     """
-
     exc_type, exc_value, exc_obj = sys.exc_info()
     if exc_type is None or exc_value is None or exc_obj is None:
         return ""
 
     err_value = exc_type.__name__
     lineno = exc_obj.tb_lineno
     filename = exc_obj.tb_frame.f_code.co_filename
 
     return (
         f"File {filename}, line {lineno}, {err_value}:{exc_value}, remark:[{extra_msg}]"
     )
 
 
-def exec_cmd(
-    *args, cwd: Optional[str] = None, reply: bool = True, decoding: bool = True
-) -> Tuple[Union[str, ByteString, None], ...]:
-    """Run system shell command.
-
-    Args:
-        reply (bool): whether return execute result. Default is True.
-        decoding (bool): whether decode the return. Default is True.
-    """
-    _stderr: Optional[int] = subprocess.PIPE if reply else None
-    _stdout: Optional[int] = subprocess.PIPE if reply else None
-
-    _err: Union[str, ByteString, None] = None
-    _rlt: Union[str, ByteString, None] = None
-
-    try:
-        # Take over the input stream and get the return information.
-        with subprocess.Popen(
-            " ".join(args), stderr=_stderr, stdout=_stdout, shell=True, cwd=cwd
-        ) as proc:
-            outres, errres = proc.communicate()
-    except FileNotFoundError as e:
-        _err = str(e).encode()
-    else:
-        _err, _rlt = errres, outres
-
-    if not decoding:
-        return _err, _rlt
-
-    # decode
-    if _err is not None:
-        _err = _err.decode()
-    if _rlt is not None:
-        _rlt = _rlt.decode()
-    return _err, _rlt
-
-
-async def async_run_cmd(
-    *args, cwd: Optional[str] = None, msg: Optional[str] = None, output: bool = True
-):
-
-    # receive (program, *args, ...), so must split the full cmd,
-    # and unpack incoming.
-    proc = await asyncio.create_subprocess_exec(
-        *args,
-        stderr=subprocess.PIPE,
-        stdout=subprocess.PIPE,
-        start_new_session=True,
-        cwd=cwd,
-    )
-    res, err = await proc.communicate()
-
-    if output:
-        msg and print(msg)
-        res and print(res.decode())
-        err and print(err.decode())
-
-    if proc.returncode != 0:
-        return proc.returncode, args, cwd
-    else:
-        return proc.returncode, err.decode(), res.decode()
-
-
-def exec_async_tasks(tasks: List[Callable]) -> List[str]:
-    """Execute tasks asynchronously."""
-
-    # The loop argument is deprecated since Python 3.8
-    # and scheduled for removal in Python 3.10
-    async def main():
-        L = await asyncio.gather(*tasks)
-        return L
-
-    return asyncio.run(main())
-
-
 def confirm(text: str = "", default: bool = True) -> bool:
     """Obtain confirmation results.
     Args:
         text (str): Confirmation prompt.
         default (bool): Result returned when unexpected input.
 
     Returns:
         (bool): Confirm result.
     """
-
     input_command: str = input(text).strip().lower()
+
     if input_command in {"n", "no", "N", "No"}:
         return False
     elif input_command in {"y", "yes", "Y", "Yes"}:
         return True
     else:
         return default
 
@@ -141,15 +94,14 @@
         >>> similar_command('br', commands)
         'branch'
         >>> similar_command('wo', commands)
         'working tree'
         >>> similar_command('com', commands)
         'commit'
     """
-
     #  The dictionary of letter frequency of all commands.
     words: dict = {word: dict(Counter(word)) for word in all_commands}
     # Letter frequency of command.
     fre = dict(Counter(command))
     # The distance between the frequency of each letter in the command
     # to be tested and all candidate commands, that is the difference
     # between the frequency of letters.
@@ -157,15 +109,15 @@
         word: [fre[ch] - words[word].get(ch, 0) for ch in command]
         + [words[word][ch] - fre.get(ch, 0) for ch in word]
         for word in words
     }
     # Square of sum of squares of word frequency difference.
     frequency_sum_square: list[Tuple[str, int]] = list(
         map(
-            lambda item: (item[0], int(sqrt(sum(map(lambda i: i ** 2, item[1]))))),
+            lambda item: (item[0], int(sqrt(sum(map(lambda i: i**2, item[1]))))),
             frequency_difference.items(),
         )
     )
 
     # The value of `frequency_sum_square` is multiplied by the weight to find
     # the minimum.
     # Distance weight: compensate for the effect of length difference.
@@ -217,15 +169,15 @@
     "m": "Object-C",
     "mm": "Object-C++",
     "markdown": "Markdown",
     "md": "Markdown",
     "msg": "ROS Message",
     "php": "PHP",
     "plist": "XML",
-    "properties": "Propertie",
+    "properties": "Properties",
     "py": "Python",
     "r": "R",
     "rb": "Ruby",
     "rc": "Properties",
     "rs": "Rust",
     "rst": "reStructuredText",
     "ts": "Type Script",
@@ -234,28 +186,28 @@
     "scss": "CSS",
     "sh": "Shell",
     "sql": "SQL",
     "srv": "ROS Message",
     "swift": "Swift",
     "toml": "Properties",
     "vb": "Visual Basic",
-    "vim": "Vim Scirpt",
+    "vim": "Vim Script",
     "vue": "Vue",
     "xhtml": "HTML",
     "xml": "XML",
     "yaml": "YAML",
     "yml": "YAML",
     "zsh": "Shell",
 }
 
 # Mark the type of some special files.
 SPECIAL_NAMES: Dict[str, str] = {
     "license": "LICENSE",
     "requirements.txt": "Pip requirement",
-    "vimrc": "Vim Scirpt",
+    "vimrc": "Vim Script",
     "dockerfile": "Docker",
 }
 
 
 def adjudgment_type(file: str, original: bool = False) -> str:
     """Get file type.
 
@@ -264,21 +216,28 @@
 
     Args:
         file (str): file name string.
         original (bool, option): whether return origin when match failed.
 
     Returns:
         (str): file type.
-    """
 
-    if pre_type := SPECIAL_NAMES.get(file.lower(), None):
+    Docs test
+        >>> adjudgment_type('py')
+        'Python'
+        >>> adjudgment_type('xx')
+        'unknown'
+        >>> adjudgment_type('xx', True)
+        'xx'
+    """
+    if pre_type := SPECIAL_NAMES.get(file.lower()):
         return pre_type
 
     suffix = file.split(".")[-1]
-    if suffix_type := SUFFIX_TYPE.get(suffix.lower(), None):
+    if suffix_type := SUFFIX_TYPE.get(suffix.lower()):
         return suffix_type
     else:
         return suffix if original else "unknown"
 
 
 FILE_ICONS: Dict[str, str] = {
     "": "",
@@ -288,49 +247,54 @@
     "C++": "",
     "CSS": "",
     "Dart": "",
     "Groovy": "",
     "Go": "",
     "HTML": "",
     "Java": "",
-    "Java Scirpt": "",
+    "Java Script": "",
     "Lua": "",
     "Kotlin": "",
     "Markdown": "",
     "PHP": "",
-    "Propertie": "",
+    "Properties": "",
     "Python": "",
     "R": "ﳒ",
     "React": "",
     "Ruby": "",
     "Rust": "",
     "ROS Message": "",
     "reStructuredText": "",
     "Shell": "",
     "Swift": "",
     "SQL": "",
     "snippets": "",
-    "Type Scirpt": "",
-    "Vim Scirpt": "",
+    "Type Script": "",
+    "Vim Script": "",
     "Vue": "﵂",
     "YAML": "",
     "XML": "",
 }
 
 
 def get_file_icon(file_type: str) -> str:
     """According file type return icon.
 
     Args:
         file_type (str): type string.
 
     Returns:
         str: icon.
-    """
 
+    Docs test
+        >>> get_file_icon('Python')
+        ''
+        >>> get_file_icon('xx')
+        ''
+    """
     #     
     return FILE_ICONS.get(file_type, "")
 
 
 if __name__ == "__main__":
     import doctest
```

### Comparing `pigit-1.6.1/pigit/config.py` & `pigit-1.7.0/pigit/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # -*- coding:utf-8 -*-
 
-from typing import Dict, List
-import os, re, textwrap, logging
-from distutils.util import strtobool
+import os
+import re
+import textwrap
+from typing import Any, List, Literal, Dict
+
+from .ext.log import logger
+from .ext.singleton import Singleton
+from .ext.utils import confirm, strtobool ,traceback_info
 
-from plenty.style import Color
-
-from .common.utils import confirm, traceback_info
-from .common.singleton import Singleton
-
-Logger = logging.getLogger(__name__)
 
 CONF_ERROR = "==error=="
 
 
 class ConfigError(Exception):
     """Config error. Using by `Config`."""
 
-    pass
-
 
 class Config(metaclass=Singleton):
     """PIGIT configuration class."""
 
     CONFIG_TEMPLATE: str = textwrap.dedent(
         """\
         #? Config file for pigit v. {version}
@@ -32,15 +29,15 @@
         # | |_) | | |  _ | |  | |_____ _____ / __/ _ \\| '_ \\| |_| |/ _` |
         # |  __/| | |_| || |  | |_____|_____| (_| (_) | | | |  _| | (_| |
         # |_|  |___\\____|___| |_|            \\___\\___/|_| |_|_| |_|\\__, |
         #                                     {version:>20} |___/
         # Git-tools -- pigit configuration.
 
         # (bool) Show original git command.
-        cmd_show_original={cmd_show_original}
+        cmd_display={cmd_display}
 
         # (bool) Is it recommended to correct when entering wrong commands.
         cmd_recommend={cmd_recommend}
 
         # (float) Display time of help information in interactive mode.
         tui_help_showtime={tui_help_showtime}
 
@@ -68,244 +65,254 @@
         # Support: (path,remote,branch,log,summary)
         repo_info_include={repo_info_include}
 
         # (bool) Whether auto append path to repos.
         repo_auto_append={repo_auto_append}
 
         # (bool) Whether run PIGIT in debug mode.
-        debug_open={debug_open}
+        log_debug={log_debug}
 
         # (bool) Whether output log in terminal.
         log_output={log_output}
 
         """
     )
 
-    _keys: List[str] = [
-        "cmd_show_original",
+    _KEYS: List[str] = [
+        "cmd_display",
         "cmd_recommend",
         "tui_help_showtime",
         "tui_files_icon",
         "counter_use_gitignore",
         "counter_show_invalid",
         "counter_show_icon",
         "counter_format",
         "git_config_format",
         "repo_info_include",
         "repo_auto_append",
-        "debug_open",
+        "log_debug",
         "log_output",
     ]
 
     # ======================
     # config default values.
     # ======================
 
     # cmd processor conf
-    cmd_show_original: bool = True
+    cmd_display: bool = True
     cmd_recommend: bool = True
 
     # tui conf
     tui_help_showtime: float = 1.5
     tui_files_icon: bool = False
 
     # code counter conf
     counter_use_gitignore: bool = True
     counter_show_invalid: bool = False
     counter_show_icon: bool = False
-    counter_format: str = "table"  # table, simple
-    _supported_result_format: List = ["table", "simple"]
+    counter_format: Literal["table", "simple"] = "table"
+    _counter_format_candidate: List = ["table", "simple"]
 
     # info conf
-    git_config_format: str = "table"
-    _supported_git_config_format: List = ["normal", "table"]
+    git_config_format: Literal["normal", "table"] = "table"
+    _git_config_format_candidate: List = ["normal", "table"]
 
     repo_info_include: List[str] = ["remote", "branch", "log"]
 
     # repo conf
     repo_auto_append: bool = False
 
     # setting conf
-    debug_open: bool = False
+    log_debug: bool = False
     log_output: bool = False
 
     # Store warning messages.
-    warnings: List = []
+    _warnings: List = []
 
     def __init__(
         self, path: str, version: str = "unknown", auto_load: bool = True
     ) -> None:
         self.config_file_path: str = path
         self.current_version: str = version
-        self.conf: Dict = {}
+        self.conf: Dict[str, Any] = {}
 
         if auto_load:
             self.load_config()
 
-    def output_warnings(self) -> None:
+    def output_warnings(self) -> "Config":
         """Output config warning info and return self object.
 
         Returns:
             self (Config): single `Config` object.
         """
 
-        if self.warnings:
-            print("Config Warning Info")
-            print("=" * 30)
-            for warning in self.warnings:
-                print(warning)
-            print("=" * 30)
-            self.warnings = []
+        if self._warnings:
+            print("#", "::Config Warning Info::")
+            print("#", "=" * 30)
+            for warning in self._warnings:
+                print("#", warning)
+            print("#", "=" * 30)
+            self._warnings = []
 
         return self
 
-    def check_and_set_value(self, key: str, value: str, new_config: Dict) -> None:
-        if key not in self._keys:
-            self.warnings.append(f"'{key}' is not be supported!")
-        elif type(getattr(self, key)) == int:
+    def check_and_set_value(self, key: str, value: str, config: Dict) -> None:
+        if key not in self._KEYS:
+            self._warnings.append(f"'{key}' is not be supported!")
+            return
+
+        v_type = type(getattr(self, key))
+        if v_type == int:
             try:
-                new_config[key] = int(value)
+                config[key] = int(value)
             except ValueError:
-                self.warnings.append(f'Config key "{key}" should be an integer!')
-        elif type(getattr(self, key)) == float:
+                self._warnings.append(f'Config key "{key}" should be an integer!')
+        elif v_type == float:
             try:
-                new_config[key] = float(value)
+                config[key] = float(value)
             except ValueError:
-                self.warnings.append(f'Config key "{key}" should be a float!')
-        elif type(getattr(self, key)) == bool:
+                self._warnings.append(f'Config key "{key}" should be a float!')
+        elif v_type == bool:
             try:
                 # True values are y, yes, t, true, on and 1;
                 # false values are n, no, f, false, off and 0.
                 # Raises ValueError if val is anything else.
-                new_config[key] = bool(strtobool(value))
+                config[key] = bool(strtobool(value))
             except ValueError:
-                self.warnings.append(f'Config key "{key}" can only be True or False!')
-        elif type(getattr(self, key)) == str:
-            if "color" in key and not Color.is_color(value):
-                self.warnings.append(
+                self._warnings.append(f'Config key "{key}" can only be True or False!')
+        elif v_type == str:
+            if "color" in key and not re.match(r"^#[0-9a-fA-F]6$", value):
+                self._warnings.append(
                     f'Config key "{key}" should be RGB string, like: "#FF0000".'
                 )
             else:
-                new_config[key] = value
-        elif type(getattr(self, key)) == list:
+                config[key] = value
+        elif v_type == list:
             if re.match(r"^\[[\w\s0-9\'\"_]+,?([\s\w0-9\'\"_]+,?)*\]$", value):
-                new_config[key] = eval(value)
+                config[key] = eval(value)
             else:
-                self.warnings.append(f'Config key "{key}" not support `{value}`.')
+                self._warnings.append(f'Config key "{key}" not support `{value}`.')
 
     def read_config(self) -> None:
-        new_config = self.conf
+        config = self.conf
         config_file = self.config_file_path
 
+        if not os.path.isfile(config_file):
+            logger(__name__).info("Has no custom config file.")
+            return
+
         with open(config_file) as cf:
             for line in cf:
                 line = line.strip()
                 if line.startswith("#? Config"):
-                    new_config["version"] = line[line.find("v. ") + 3 :]
+                    config["version"] = line[line.find("v. ") + 3 :]
                     continue
                 if line.startswith("#"):
                     # comment line.
                     continue
                 if "=" not in line:
                     # invalid line.
                     continue
 
                 # remove line comment.
                 if line_comment_idx := line.find("#") > 0:
                     line = line[:line_comment_idx]
 
                 # processing.
-                key_string, value_string = line.split("=", maxsplit=1)
-                key_string = key_string.strip()
-                value_string = value_string.strip().strip('"')
+                key_str, value_str = line.split("=", maxsplit=1)
+                key_str = key_str.strip()
+                value_str = value_str.strip().strip('"')
 
                 # checking.
-                self.check_and_set_value(key_string, value_string, new_config)
+                self.check_and_set_value(key_str, value_str, config)
 
-    def parse_conf(self) -> None:
-        new_config = self.conf
+    def parse_config(self) -> None:
+        config = self.conf
 
-        if (  # check codecounter output format whether supported.
-            "codecounter_result_format" in new_config
-            and new_config["codecounter_result_format"]
-            not in self._supported_result_format
+        if (  # check code-counter output format whether supported.
+            "counter_format" in config
+            and config["counter_format"] not in self._counter_format_candidate
         ):
-            new_config["codecounter_result_format"] = CONF_ERROR
-            self.warnings.append(
+            config["counter_format"] = CONF_ERROR
+            self._warnings.append(
                 'Config key "{0}" support must in {1}'.format(
-                    "codecounter_result_format", self._supported_result_format
+                    "counter_format", self._counter_format_candidate
                 )
             )
 
         if (
-            "git_config_format" in new_config
-            and new_config["git_config_format"] not in self._supported_git_config_format
+            "git_config_format" in config
+            and config["git_config_format"] not in self._git_config_format_candidate
         ):
-            new_config["git_config_format"] = CONF_ERROR
-            self.warnings.append(
+            config["git_config_format"] = CONF_ERROR
+            self._warnings.append(
                 'Config key "{0}" support must in {1}'.format(
-                    "git_config_format", self._supported_git_config_format
+                    "git_config_format", self._git_config_format_candidate
                 )
             )
 
         version = self.current_version
-        if "version" in new_config and not (
+        if "version" in config and not (
             # If unknown current version or
             # If the version is right or
-            # If current version is a [beta, alpha, dev] verstion then will not tip.
+            # If current version is a [beta, alpha, dev] version then will not tip.
             # Else if version is not right will tip.
             version == "unknown"
-            or new_config["version"] == version
+            or config["version"] == version
             or "beta" in version
             or "alpha" in version
             or "dev" in version
         ):
-            print(new_config["version"])
-            self.warnings.append(
+            self._warnings.append(
                 "The current configuration file is not up-to-date."
                 "You'd better recreate it."
+                f"Config version is '{config['version']}', current version is '{version}'."
             )
 
     def load_config(self) -> None:
         try:
             self.read_config()
         except Exception:
-            Logger.error(traceback_info())
-            self.warnings.append(
+            logger(__name__).error(traceback_info())
+            self._warnings.append(
                 f"Can not load the config file. Path: {self.config_file_path}"
             )
 
-        self.parse_conf()
+        self.parse_config()
 
         # setting config.
-        for key in self._keys:
+        for key in self._KEYS:
             if key in self.conf.keys() and self.conf[key] != CONF_ERROR:
+                # update default for using.
                 setattr(self, key, self.conf[key])
             else:
+                # append default to conf for written.
                 self.conf[key] = getattr(self, key)
 
-    def create_config_template(self) -> None:
+    def create_config_template(self) -> bool:
         parent_dir = os.path.dirname(self.config_file_path)
         if not os.path.isdir(parent_dir):
             os.makedirs(parent_dir, exist_ok=True)
 
         if os.path.exists(self.config_file_path) and not confirm(
             "Configuration exists, overwrite? [y/n]"
         ):
-            return None
+            return False
 
         # Try to load already has config.
         self.load_config()
         self.conf["version"] = self.current_version
 
         # Write config with already exist custom settings.
         try:
             with open(
                 self.config_file_path,
                 "w" if os.path.isfile(self.config_file_path) else "x",
             ) as f:
                 f.write(self.CONFIG_TEMPLATE.format(**self.conf))
         except Exception:
-            Logger.error(traceback_info())
+            logger(__name__).error(traceback_info())
             print("Fail to create config.")
+            return False
         else:
             print("Successful.")
+            return True
```

### Comparing `pigit-1.6.1/pigit/const.py` & `pigit-1.7.0/pigit/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding:utf-8 -*-
 
-import os, platform, datetime
+import datetime
+import os
+import platform
+
 
 __project__ = "pigit"
-__version__ = "1.6.1"
+__version__ = "1.7.0"
 __url__ = "https://github.com/zlj-zz/pigit.git"
 __uri__ = __url__
 
 __author__ = "Zachary Zhang"
 __email__ = "zlj19971222@outlook.com"
 
 __license__ = "MIT"
```

### Comparing `pigit-1.6.1/pigit/entry.py` & `pigit-1.7.0/pigit/entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,290 @@
 # -*- coding:utf-8 -*-
 # The PIGIT terminal tool entry file.
 
-from typing import Dict, List
-import os, logging, textwrap
+import os
+import textwrap
+from typing import TYPE_CHECKING, Dict, List
 
 from plenty import get_console
+from plenty.table import Table
 
-from .log import setup_logging
 from .config import Config
-from .cmdparse.parser import command, argument, Namespace
 from .const import (
-    VERSION,
-    REPOS_PATH,
-    PIGIT_HOME,
-    LOG_FILE_PATH,
-    EXTRA_CMD_MODULE_NAME,
-    EXTRA_CMD_MODULE_PATH,
     CONFIG_FILE_PATH,
     COUNTER_DIR_PATH,
+    EXTRA_CMD_MODULE_NAME,
+    EXTRA_CMD_MODULE_PATH,
     IS_FIRST_RUN,
+    IS_WIN,
+    LOG_FILE_PATH,
+    PIGIT_HOME,
+    REPOS_PATH,
+    VERSION,
 )
-from .common.utils import confirm
-from .common.func import dynamic_default_attrs, time_it
-from .gitlib.processor import ShortGitter, GIT_CMDS, get_extra_cmds
-from .gitlib.options import GitOption
-from .gitlib.ignore import create_gitignore
-from .info import introduce, GitConfig
+from .cmdparse.parser import argument, command
+from .ext.lcstat import LINES_CHANGE, LINES_NUM, FILES_CHANGE, FILES_NUM, Counter
+from .ext.log import setup_logging
+from .ext.func import dynamic_default_attrs, time_it
+from .ext.utils import confirm, get_file_icon
+from .git import Git_Proxy_Cmds, GitProxy, Repo, create_gitignore, get_extra_cmds
+from .info import introduce, show_gitconfig
 
-
-Logger = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    from .cmdparse.parser import Namespace
 
 
 # ===============
 # Configuration.
 # ===============
-CONFIG = Config(
-    path=CONFIG_FILE_PATH, version=VERSION, auto_load=True
-).output_warnings()
+Conf = Config(path=CONFIG_FILE_PATH, version=VERSION, auto_load=True).output_warnings()
 
 setup_logging(
-    debug=CONFIG.debug_open,
-    log_file=None if CONFIG.log_output else LOG_FILE_PATH,
+    debug=Conf.log_debug,
+    log_file=None if Conf.log_output else LOG_FILE_PATH,
 )
 
 
 # ==============
 # Global handle
 # ==============
-git = GitOption(repo_json_path=REPOS_PATH)
+repo_handler = Repo(repo_json_path=REPOS_PATH)
 console = get_console()
 
 
 # =====================
 # main command `pigit`
 # yapf: disable
 # =====================
 @command("pigit", description="Pigit TUI is called automatically if no parameters are followed.")
 @argument("-r --report", action="store_true", help="Report the pigit desc and exit.")
 @argument("-f --config", action="store_true", help="Display the config of current git repository and exit.")
 @argument("-i --information", action="store_true", help="Show some information about the current git repository.")
-def pigit(args: Namespace, _) -> None:
+def pigit(args: "Namespace", _) -> None:
     if args.report:
         console.echo(introduce())
 
     elif args.create_config:
-        return CONFIG.create_config_template()
+        Conf.create_config_template()
+        return
 
     elif args.config:
-        console.echo(GitConfig(format_type=CONFIG.git_config_format).generate())
+        console.echo(show_gitconfig(format_type=Conf.git_config_format))
 
     elif args.information:
-        console.echo(git.get_repo_desc(include_part=CONFIG.repo_info_include))
+        console.echo(repo_handler.get_repo_desc(include_part=Conf.repo_info_include))
 
     elif args.complete:
-        # Generate competion vars dict.
+        # Generate completion vars dict.
         complete_vars = pigit.to_dict()
         complete_vars["args"]["cmd"]["args"].update(
-            {k: {"help": v["help"], "args": {}} for k, v in GIT_CMDS.items()}
+            {k: {"help": v["help"], "args": {}} for k, v in Git_Proxy_Cmds.items()}
         )
 
-        from .cmdparse.shellcompletion import shell_complete
+        from .cmdparse.completion import shell_complete
 
-        shell_complete(complete_vars, PIGIT_HOME, inject=True)
+        shell_complete(complete_vars, args.complete)
         return None
 
     elif args.ignore_type:
-        _, msg = create_gitignore(args.ignore_type,writting=True)
+        _, msg = create_gitignore(args.ignore_type, writing=True)
         console.echo(msg)
 
     elif args.count:
-        from .codecounter import CodeCounter
-
         path = os.path.abspath(args.count) if args.count != "." else os.getcwd()
-        CodeCounter(
-            count_path=path,
-            use_ignore=CONFIG.counter_use_gitignore,
-            result_saved_path=COUNTER_DIR_PATH,
-            format_type=CONFIG.counter_format,
-            use_icon=CONFIG.counter_show_icon,
-        ).run(
-            show_invalid=CONFIG.counter_show_invalid,
-        )
+        total_size, diff_result, invalids = Counter(
+            saved_dir=COUNTER_DIR_PATH, show_invalid=Conf.counter_show_invalid
+        ).diff_count(path, Conf.counter_use_gitignore)
+        if Conf.counter_format == "simple":
+            for k, v in diff_result.items():
+                print(f"::{k}  (files:{v[FILES_NUM]:,} | lines:{v[LINES_NUM]:,})")
+
+        elif Conf.counter_format == "table":
+
+            def color_index(
+                count: int,
+            ) -> str:
+                # Colors displayed for different code quantities.
+                level_color = (
+                    "green",
+                    "#EBCB8C",  # yellow
+                    "#FF6347",  # tomato
+                    "#C71585",  # middle violet red
+                    "#87CEFA",  # skyblue
+                )
+                index = len(str(count // 1000))
+                return (
+                    level_color[-1]
+                    if index > len(level_color)
+                    else level_color[index - 1]
+                )
+
+            tb = Table(title="[Code Counter Result]", title_style="bold")
+            tb.add_column("Language")
+            tb.add_column("Files")
+            tb.add_column("Code lines")
+
+            for k, v in diff_result.items():
+                f_type_str = (
+                    f"`{get_file_icon(k)} {k}`<cyan>" if Conf.counter_show_icon else k
+                )
+
+                f_num_str = f"`{v[FILES_NUM]}`<{color_index(v[FILES_NUM])}>"
+                l_num_str = f"`{v[LINES_NUM]}`<{color_index(v[LINES_NUM])}>"
+
+                f_change_str = (
+                    f"{v[FILES_CHANGE]:+}" if v.get(FILES_CHANGE, 0) != 0 else ""
+                )
+                l_change_str = (
+                    f"{v[LINES_CHANGE]:+}" if v.get(LINES_CHANGE, 0) != 0 else ""
+                )
+
+                tb.add_row(
+                    f_type_str,
+                    f"{f_num_str} `{f_change_str}`<{'#98fb98' if f_change_str.startswith('+') else '#ff6347'}>",
+                    f"{l_num_str} `{l_change_str}`<{'#98fb98' if l_change_str.startswith('+') else '#ff6347'}>",
+                )
+            tb.caption = " Total: {0}".format(total_size)
+            get_console().echo(tb)
+        else:
+            print("Invalid display format!")
+
         return None
 
     # Don't have invalid command list.
     # if not list(filter(lambda x: x, vars(known_args).values())):
     else:
-        from .interaction import tui_main
-
         if IS_FIRST_RUN:
             introduce()
             if not confirm("Input `enter` to continue:"):
                 return
 
-        tui_main(CONFIG)
+        if IS_WIN:
+            print("Not support windows now.")
+        else:
+            from .app import App
+
+            App().run()
 
 
-pigit.add_argument("-v", "--version", action="version", help="Show version and exit.", version=f"Version:{VERSION}")
+# yapf: enable
+pigit.add_argument(
+    "-v",
+    "--version",
+    action="version",
+    help="Show version and exit.",
+    version=f"Version:{VERSION}",
+)
 
-tools_group = pigit.add_argument_group(title="tools arguments", description="Auxiliary type commands.")
-tools_group.add_argument("-c", "--count", nargs="?", const=".", type=str, metavar="PATH",
+tools_group = pigit.add_argument_group(
+    title="tools arguments", description="Auxiliary type commands."
+)
+tools_group.add_argument(
+    "-c",
+    "--count",
+    nargs="?",
+    const=".",
+    type=str,
+    metavar="PATH",
     help="""Count the number of codes and output them in tabular form.
     A given path can be accepted, and the default is the current directory.
-    """,)
-tools_group.add_argument( "--create-ignore", type=str, metavar="TYPE", dest="ignore_type",
-    help="""Create a demo .gitignore file. Need one argument, the type of gitignore.""")
-tools_group.add_argument("-C", "--complete", action="store_true",
-    help="Add shell prompt script and exit. (Supported bash, zsh, fish)")
-tools_group.add_argument("--create-config", action="store_true",
+    """,
+)
+tools_group.add_argument(
+    "--create-ignore",
+    type=str,
+    metavar="TYPE",
+    dest="ignore_type",
+    help="""Create a demo .gitignore file. Need one argument, the type of gitignore.""",
+)
+tools_group.add_argument(
+    "--complete",
+    nargs="?",
+    const="nil",
+    type=str,
+    metavar="SHELL",
+    help="Add shell prompt script and exit. (Supported bash, zsh, fish)",
+)
+tools_group.add_argument(
+    "--create-config",
+    action="store_true",
     help="Create a pre-configured file of PIGIT."
-    "(If a profile exists, the values available in it are used)",)
+    "(If a profile exists, the values available in it are used)",
+)
+
 
 # =============================================
 # sub command `cmd`
 # =============================================
 @pigit.sub_parser("cmd", help="git short command.")
 @argument("--shell", action="store_true", help="Go to the pigit shell mode.")
 @argument("-t --types", action="store_true", help="List all command types and exit.")
-@argument("-p --show-part-command", type=str, metavar="TYPE", dest="command_type",
-    help='According to given type to list available short command and wealth and exit.')
-@argument("-s --show-commands", action="store_true", help="List all available short command and wealth and exit.")
+@argument(
+    "-p --show-part-command",
+    type=str,
+    metavar="TYPE",
+    dest="command_type",
+    help="According to given type to list available short command and wealth and exit.",
+)
+@argument(
+    "-s --show-commands",
+    action="store_true",
+    help="List all available short command and wealth and exit.",
+)
 @argument("args", nargs="*", type=str, help="Command parameter list.")
-@argument("command", nargs="?", type=str, default=None, help="Short git command or other.")
-def _cmd_func(args: Namespace, unknown: List):
+@argument(
+    "command", nargs="?", type=str, default=None, help="Short git command or other."
+)
+def _(args: "Namespace", unknown: List):
     """If you want to use some original git commands, please use -- to indicate."""
 
     # If you want to manipulate the current folder with git,
     # try adding it to repos automatically.
-    if CONFIG.repo_auto_append:
-        repo_path, repo_conf = git.get_repo_info()
-        git.add_repos([repo_path])
+    if Conf.repo_auto_append:
+        repo_path, repo_conf = repo_handler.confirm_repo()
+        repo_handler.add_repos([repo_path])
 
     # Init extra custom cmds.
     extra_cmd: Dict = {
         # "shell": {
         #     "command": lambda _: shell_mode(git_processor),
         #     "type": "func",
         #     "help": "Into PIGIT shell mode.",
         # },  # only for tips.
     }
     extra_cmd.update(get_extra_cmds(EXTRA_CMD_MODULE_NAME, EXTRA_CMD_MODULE_PATH))
 
-    git_processor = ShortGitter(
+    git_processor = GitProxy(
         extra_cmds=extra_cmd,
-        command_prompt=CONFIG.cmd_recommend,
-        show_original=CONFIG.cmd_show_original,
+        prompt=Conf.cmd_recommend,
+        display=Conf.cmd_display,
     )
 
     if args.shell:
         from .shellmode import PigitShell
+
         shell_ = PigitShell(git_processor)
         # print(shell_.__dir__())
         shell_.cmdloop()
         return
 
     if args.show_commands:
-        return git_processor.print_help()
+        # return git_processor.print_help()
+        return console.echo(git_processor.get_help())
 
     if args.command_type:
-        return git_processor.print_help_by_type(args.command_type)
+        return console.echo(git_processor.get_help_by_type(args.command_type))
 
     if args.types:
-        return git_processor.print_types()
+        return console.echo(git_processor.get_types())
 
     if args.command:
-        command = args.command
+        short_cmd = args.command
         args.args.extend(unknown)
-        git_processor.do(command, args.args)
+        console.echo(git_processor.do(short_cmd, args.args))
         return None
     else:
         console.echo("`pigit cmd -h`<ok> for help.")
 
 
 # =============================================
 # sub command `repo`
@@ -198,54 +292,54 @@
 repo = pigit.sub_parser("repo", help="repos options.")(lambda _, __: print("-h help"))
 
 
 @repo.sub_parser("add", help="add repo(s).")
 @argument("--dry-run", action="store_true", help="dry run.")
 @argument("paths", nargs="+", help="path of reps(s).")
 def repo_add(args, _):
-    if added := git.add_repos(args.paths, args.dry_run):
+    if added := repo_handler.add_repos(args.paths, args.dry_run):
         console.echo(f"Found {len(added)} new repo(s).")
         for path in added:
             console.echo(f"\t`{path}`<sky_blue>")
     else:
         console.echo("`No new repos found!`<tomato>")
 
 
 @repo.sub_parser("rm", help="remove repo(s).")
-@argument("--path", action="store_true", help="remove follow path, defult is name.")
+@argument("--path", action="store_true", help="remove follow path, default is name.")
 @argument("repos", nargs="+", help="name or path of repo(s).")
 def repo_rm(args, _):
-    res = git.rm_repos(args.repos, args.path)
+    res = repo_handler.rm_repos(args.repos, args.path)
     for one in res:
         console.echo(f"Deleted repo. name: '{one[0]}', path: {one[1]}")
 
 
 @repo.sub_parser("rename", help="rename a repo.")
 @argument("new_name", help="the new name of repo.")
 @argument("repo", help="the name of repo.")
 def repo_rename(args, _):
-    success, msg = git.rename_repo(args.repo, args.new_name)
+    success, msg = repo_handler.rename_repo(args.repo, args.new_name)
     console.echo(msg)
 
 
 @repo.sub_parser("ll", help="display summary of all repos.")
 @argument("--simple", action="store_true", help="display simple summary.")
-@argument("--revese", action="store_true", help="revese to display invalid repo.")
+@argument("--reverse", action="store_true", help="reverse to display invalid repo.")
 def repo_ll(args, _):
     simple = args.simple
-    revese = args.revese
+    reverse = args.reverse
 
-    for info in git.ll_repos(revese=revese):
+    for info in repo_handler.ll_repos(reverse=reverse):
         if simple:
-            if revese:
+            if reverse:
                 console.echo(f"{info[0][0]:<20} {info[1][1]:<15}")
             else:
                 console.echo(f"{info[0][0]:<20} {info[1][1]:<15} {info[5][1]}")
         else:
-            if revese:
+            if reverse:
                 summary_string = textwrap.dedent(
                     f"""\
                     b`{info[0][0]}`
                         {info[1][0]}: `{info[1][1]}`<sky_blue>
                     """
                 )
             else:
@@ -258,51 +352,52 @@
                         {info[4][0]}: `{info[4][1]}`<ok>
                         {info[5][0]}: `{info[5][1]}`<sky_blue>
                     """
                 )
             console.echo(summary_string)
 
 
-repo.sub_parser("clear", help="clear the all repos.")(lambda _, __: git.clear_repos())
+repo.sub_parser("clear", help="clear the all repos.")(
+    lambda _, __: repo_handler.clear_repos()
+)
+
+
+@repo.sub_parser("cd", help="jump to a repo dir.")
+@argument("repo", nargs="?", help="the name of repo.")
+def _(args, _):
+    repo_handler.cd_repo(args.repo)
 
 
 repo_options = {
     "fetch": {"cmd": "git fetch", "allow_all": True, "help": "fetch remote update"},
     "pull": {"cmd": "git pull", "allow_all": True, "help": "pull remote updates"},
     "push": {"cmd": "git push", "allow_all": True, "help": "push the local updates"},
 }
-for subcmd, prop in repo_options.items():
-    help_string = f'{h.strip()} for repo(s).' if (h:=prop.get("help")) else "NULL"
-    repo.sub_parser(subcmd, help=help_string)(
+for sub_cmd, prop in repo_options.items():
+    help_string = f"{h.strip()} for repo(s)." if (h := prop.get("help")) else "NULL"
+    repo.sub_parser(sub_cmd, help=help_string)(
         argument("repos", nargs="*", help="name of repo(s).")(
             dynamic_default_attrs(
-                lambda args, _, cmd: git.process_repo_option(args.repos, cmd),
-                cmd=prop['cmd']
+                lambda args, _, cmd: repo_handler.process_repos_option(args.repos, cmd),
+                cmd=prop["cmd"],
             )
         )
     )
 
 
 # =============================================
 # sub command `open`
+# yapf: disable
 # =============================================
 @pigit.sub_parser("open", help="open remote repository in web browser.")
 @argument("-p --print", action="store_true", help="only print the url at the terminal, but do not open it.")
 @argument("-c --commit", help="the current commit in the repo website.")
 @argument("-i --issue", help="the given issue of the repository.")
 @argument("branch", nargs="?", default=None, help="the branch of repository.")
-def _open_func(args: Namespace, _):
-    code, msg = git.open_repo_in_browser(
+def _(args: "Namespace", _):
+    code, msg = repo_handler.open_repo_in_browser(
         branch=args.branch, issue=args.issue, commit=args.commit, print=args.print
     )
     console.echo(msg)
 
+# yapf: enable
 
-# =============================================
-# terminal entry
-# =============================================
-@time_it
-def main():
-    try:
-        pigit()
-    except (KeyboardInterrupt, EOFError):
-        raise SystemExit(0) from None
```

### Comparing `pigit-1.6.1/pigit/gitlib/_cmd_func.py` & `pigit-1.7.0/pigit/git/_cmd_func.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,90 +2,88 @@
 
 """Command methods.
 
 This file encapsulates some methods corresponding to command.
 All methods are must and only accept an `args` parameter -- a list or tuple
 of parameters to be processed. If don't need will get a empty list or tuple.
 
-Like this:
->>> def func(args: Union[list, tuple]) -> None:
+Example:
+>>> def func(args: Union[list, tuple]) -> str:
 >>>     # your code.
 >>>     pass
+>>>     return "result msg."
 """
 
+import re
 from typing import List, Tuple, Union
 
-from plenty import echo
+from pigit.ext.executor import WAITING, Executor
 
-from ..common.utils import exec_cmd
 
-
-def add(args: Union[List, Tuple]) -> None:
+def add(args: Union[List, Tuple]) -> str:
     """git add option.
 
     Args:
         args (list): arguments list, maybe empty. need file string.
     """
 
     args_str = " ".join(args) if args else " ."
-    echo(
-        ":rainbow: Storage file: {0}".format(
-            "all" if args_str.strip() == "." else args_str
-        )
+    Executor().exec(f"git add {args_str}", flags=WAITING)
+
+    return ":rainbow: Storage file: {0}".format(
+        "all" if args_str.strip() == "." else args_str
     )
-    exec_cmd(f"git add {args_str}", reply=False)
 
 
-def fetch_remote_branch(args: Union[List, Tuple]) -> None:
+def fetch_remote_branch(args: Union[List, Tuple]) -> str:
     "Fetch a remote branch to local and with the same name."
 
     branch = args[0] if len(args) > 1 else None
 
     if branch:
-        exec_cmd("git fetch origin {0}:{0} ".format(branch), reply=False)
+        Executor().exec("git fetch origin {0}:{0} ".format(branch), flags=WAITING)
+        return ""
     else:
-        echo("`This option need a branch name.`<error>")
+        return "`This option need a branch name.`<error>"
 
 
-def set_email_and_username(args: Union[List, Tuple]) -> None:
+def set_email_and_username(args: Union[List, Tuple]) -> str:
     """Set git username and email with interaction.
 
     Args:
         args (list): arguments list, maybe empty.
     """
 
     print("Set the interactive environment of user name and email ...")
 
     is_global = next(
         (" --global " for i in args if i.strip() in ["-g", "--global"]), ""
     )
 
-    if is_global:
-        print("Now set for global.")
-    else:
-        print("Now set for local.")
+    print("Now set for global." if is_global else "Now set for local.")
 
     while True:
         name = input("Please input username:").strip()
 
         if name:
             break
         else:
-            echo("`Name is empty.`<error>")
-
-    import re
+            print("ERROR: Name is empty. continue ...")
 
     email_re = re.compile(r"^[0-9a-zA-Z_]{0,19}@[0-9a-zA-Z]{1,13}\.[com,cn,net]{1,3}$")
     while True:
         email = input("Please input email:")
 
         if email_re.match(email) is not None:
             break
         else:
-            echo("`Bad mailbox format.`<error>")
+            print("ERROR: Bad mailbox format. continue ...")
 
-    if exec_cmd(f"git config user.name {name} {is_global}", reply=False) and exec_cmd(
-        f"git config user.email {email} {is_global}", reply=False
-    ):
-        echo("`Successfully set.`<ok>")
+    executor = Executor()
+    if executor.exec(
+        f"git config user.name {name} {is_global}", flags=WAITING
+    ) and executor.exec(f"git config user.email {email} {is_global}", flags=WAITING):
+        print("Successfully set.")
     else:
-        echo("`Failed. Please check log.`<error>")
+        print("Failed. Please check log.")
+
+    return ""
```

### Comparing `pigit-1.6.1/pigit/gitlib/ignore/__init__.py` & `pigit-1.7.0/pigit/git/ignore/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from typing import Optional, Tuple
 from shutil import get_terminal_size
 from pathlib import Path
+
 from .template import IGNORE_TEMPLATE
 
 
 __all__ = ("get_ignore_source", "create_gitignore")
 
 
-def get_ignore_source(type_: str) -> Optional[str]:
+def get_ignore_source(t: str) -> Optional[str]:
     """Get gitignore source follow type."""
-    return IGNORE_TEMPLATE.get(type_)
+
+    return IGNORE_TEMPLATE.get(t)
 
 
 def create_gitignore(
-    type_: str,
+    t: str,
     file_name: str = ".gitignore",
     dir_path: Optional[str] = None,
-    writting: bool = True,
+    writing: bool = True,
 ) -> Tuple[int, str]:
     """Try to create a gitignore file.
 
     Args:
-        type_ (str): project type.
+        t (str): project type.
         file_name (str, optional): file name. Defaults to ".gitignore".
         dir_path (Optional[str], optional): dir path. Defaults to None.
-        writting (bool, optional): whether writting. Defaults to True.
+        writing (bool, optional): whether writing. Defaults to True.
 
     Returns:
         Tuple[int, str]: (code, message)
+            code:
+                0: successful
+                1: don't write
+                2: not supported
     """
 
-    source = IGNORE_TEMPLATE.get(type_.lower())
+    source = IGNORE_TEMPLATE.get(t.lower())
     path = Path(dir_path or ".").joinpath(file_name)
 
     if source is None:
 
         return 2, (
-            f"Unsupported type: {type_}\n"
+            f"Unsupported type: {t}\n"
             f'Supported type: [{" ".join(IGNORE_TEMPLATE)}]. Case insensitive.'
         )
 
-    if not (writting and path.parent.is_dir()):
+    if not (writing and path.parent.is_dir()):
         width, _ = get_terminal_size()
         return 1, "{sep}{source}{sep}".format(sep="=" * width, source=source)
 
     with path.open(mode="w+") as f:
         f.write(source)
 
     return 0, f"Write gitignore file successful. Path: {path}"
```

### Comparing `pigit-1.6.1/pigit/gitlib/ignore/template.py` & `pigit-1.7.0/pigit/git/ignore/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from typing import Dict
 
 # https://github.com/github/gitignore
+# Generate by script `gitignore.py`.
+
+from typing import Dict
+
 
 _android: str = r"""
 # Gradle files
 .gradle/
 build/
 
 # Local configuration file (sdk path, etc)
@@ -34,14 +37,15 @@
 # Google Services (e.g. APIs or Firebase)
 google-services.json
 
 # Android Profiling
 *.hprof
 """
 
+
 _cpp: str = r"""
 # Prerequisites
 *.d
 
 # Compiled Object files
 *.slo
 *.lo
@@ -69,14 +73,15 @@
 
 # Executables
 *.exe
 *.out
 *.app
 """
 
+
 _c: str = r"""
 # Prerequisites
 *.d
 
 # Object files
 *.o
 *.ko
@@ -124,28 +129,68 @@
 .tmp_versions/
 modules.order
 Module.symvers
 Mkfile.old
 dkms.conf
 """
 
+
 _cmake: str = r"""
 CMakeLists.txt.user
 CMakeCache.txt
 CMakeFiles
 CMakeScripts
 Testing
 Makefile
 cmake_install.cmake
 install_manifest.txt
 compile_commands.json
 CTestTestfile.cmake
 _deps
 """
 
+
+_cuda: str = r"""
+*.i
+*.ii
+*.gpu
+*.ptx
+*.cubin
+*.fatbin
+"""
+
+
+_d: str = r"""
+# Compiled Object files
+*.o
+*.obj
+
+# Compiled Dynamic libraries
+*.so
+*.dylib
+*.dll
+
+# Compiled Static libraries
+*.a
+*.lib
+
+# Executables
+*.exe
+
+# DUB
+.dub
+docs.json
+__dummy.html
+docs/
+
+# Code coverage
+*.lst
+"""
+
+
 _dart: str = r"""
 # See https://www.dartlang.org/guides/libraries/private-files
 
 # Files and directories created by pub
 .dart_tool/
 .packages
 build/
@@ -168,29 +213,52 @@
 *.js.deps
 *.js.map
 
 .flutter-plugins
 .flutter-plugins-dependencies
 """
 
+
 _elisp: str = r"""
 # Compiled
 *.elc
 
 # Packaging
 .cask
 
 # Backup files
 *~
 
 # Undo-tree save-files
 *.~undo-tree
 """
 
-_gitbook: str = r"""\
+
+_erlang: str = r"""
+.eunit
+*.o
+*.beam
+*.plt
+erl_crash.dump
+.concrete/DEV_MODE
+
+# rebar 2.x
+.rebar
+rel/example_project
+ebin/*.beam
+deps
+
+# rebar 3
+.rebar3
+_build/
+_checkouts/
+"""
+
+
+_gitbook: str = r"""
 # Node rules:
 ## Grunt intermediate storage (http://gruntjs.com/creating-plugins#storing-task-files)
 .grunt
 
 ## Dependency directory
 ## Commenting this out is preferred by some people, see
 ## https://docs.npmjs.com/misc/faq#should-i-check-my-node_modules-folder-into-git
@@ -201,14 +269,15 @@
 
 # eBook build output
 *.epub
 *.mobi
 *.pdf
 """
 
+
 _go: str = r"""
 # If you prefer the allow list template instead of the deny list, see community template:
 # https://github.com/github/gitignore/blob/main/community/Golang/Go.AllowList.gitignore
 #
 # Binaries for programs and plugins
 *.exe
 *.exe~
@@ -225,14 +294,15 @@
 # Dependency directories (remove the comment below to include it)
 # vendor/
 
 # Go workspace file
 go.work
 """
 
+
 _java: str = r"""
 # Compiled class file
 *.class
 
 # Log file
 *.log
 
@@ -252,14 +322,71 @@
 *.rar
 
 # virtual machine crash logs, see http://www.java.com/en/download/help/error_hotspot.xml
 hs_err_pid*
 replay_pid*
 """
 
+
+_julia: str = r"""
+# Files generated by invoking Julia with --code-coverage
+*.jl.cov
+*.jl.*.cov
+
+# Files generated by invoking Julia with --track-allocation
+*.jl.mem
+
+# System-specific files and directories generated by the BinaryProvider and BinDeps packages
+# They contain absolute paths specific to the host computer, and so should not be committed
+deps/deps.jl
+deps/build.log
+deps/downloads/
+deps/usr/
+deps/src/
+
+# Build artifacts for creating documentation generated by the Documenter package
+docs/build/
+docs/site/
+
+# File generated by Pkg, the package manager, based on a corresponding Project.toml
+# It records a fixed state of all packages used by the project. As such, it should not be
+# committed for packages, but should be committed for applications that require a static
+# environment.
+Manifest.toml
+"""
+
+
+_kotlin: str = r"""
+# Compiled class file
+*.class
+
+# Log file
+*.log
+
+# BlueJ files
+*.ctxt
+
+# Mobile Tools for Java (J2ME)
+.mtj.tmp/
+
+# Package Files #
+*.jar
+*.war
+*.nar
+*.ear
+*.zip
+*.tar.gz
+*.rar
+
+# virtual machine crash logs, see http://www.java.com/en/download/help/error_hotspot.xml
+hs_err_pid*
+replay_pid*
+"""
+
+
 _lua: str = r"""
 # Compiled Lua sources
 luac.out
 
 # luarocks build files
 *.src.rock
 *.zip
@@ -295,14 +422,15 @@
 *.out
 *.app
 *.i*86
 *.x86_64
 *.hex
 """
 
+
 _maven: str = r"""
 target/
 pom.xml.tag
 pom.xml.releaseBackup
 pom.xml.versionsBackup
 pom.xml.next
 release.properties
@@ -315,14 +443,15 @@
 # Eclipse m2e generated files
 # Eclipse Core
 .project
 # JDT-specific (Eclipse Java Development Tools)
 .classpath
 """
 
+
 _node: str = r"""
 # Logs
 logs
 *.log
 npm-debug.log*
 yarn-debug.log*
 yarn-error.log*
@@ -448,147 +577,126 @@
 .yarn/cache
 .yarn/unplugged
 .yarn/build-state.yml
 .yarn/install-state.gz
 .pnp.*
 """
 
-_object_c: str = r"""
-# Logs
-logs
-*.log
-npm-debug.log*
-yarn-debug.log*
-yarn-error.log*
-lerna-debug.log*
-.pnpm-debug.log*
-
-# Diagnostic reports (https://nodejs.org/api/report.html)
-report.[0-9]*.[0-9]*.[0-9]*.[0-9]*.json
-
-# Runtime data
-pids
-*.pid
-*.seed
-*.pid.lock
-
-# Directory for instrumented libs generated by jscoverage/JSCover
-lib-cov
-
-# Coverage directory used by tools like istanbul
-coverage
-*.lcov
-
-# nyc test coverage
-.nyc_output
-
-# Grunt intermediate storage (https://gruntjs.com/creating-plugins#storing-task-files)
-.grunt
-
-# Bower dependency directory (https://bower.io/)
-bower_components
-
-# node-waf configuration
-.lock-wscript
-
-# Compiled binary addons (https://nodejs.org/api/addons.html)
-build/Release
-
-# Dependency directories
-node_modules/
-jspm_packages/
-
-# Snowpack dependency directory (https://snowpack.dev/)
-web_modules/
-
-# TypeScript cache
-*.tsbuildinfo
-
-# Optional npm cache directory
-.npm
-
-# Optional eslint cache
-.eslintcache
-
-# Optional stylelint cache
-.stylelintcache
 
-# Microbundle cache
-.rpt2_cache/
-.rts2_cache_cjs/
-.rts2_cache_es/
-.rts2_cache_umd/
+_objective_c: str = r"""
+# Xcode
+#
+# gitignore contributors: remember to update Global/Xcode.gitignore, Objective-C.gitignore & Swift.gitignore
 
-# Optional REPL history
-.node_repl_history
+## User settings
+xcuserdata/
 
-# Output of 'npm pack'
-*.tgz
+## compatibility with Xcode 8 and earlier (ignoring not required starting Xcode 9)
+*.xcscmblueprint
+*.xccheckout
 
-# Yarn Integrity file
-.yarn-integrity
+## compatibility with Xcode 3 and earlier (ignoring not required starting Xcode 4)
+build/
+DerivedData/
+*.moved-aside
+*.pbxuser
+!default.pbxuser
+*.mode1v3
+!default.mode1v3
+*.mode2v3
+!default.mode2v3
+*.perspectivev3
+!default.perspectivev3
 
-# dotenv environment variable files
-.env
-.env.development.local
-.env.test.local
-.env.production.local
-.env.local
+## Obj-C/Swift specific
+*.hmap
 
-# parcel-bundler cache (https://parceljs.org/)
-.cache
-.parcel-cache
+## App packaging
+*.ipa
+*.dSYM.zip
+*.dSYM
 
-# Next.js build output
-.next
-out
+# CocoaPods
+#
+# We recommend against adding the Pods directory to your .gitignore. However
+# you should judge for yourself, the pros and cons are mentioned at:
+# https://guides.cocoapods.org/using/using-cocoapods.html#should-i-check-the-pods-directory-into-source-control
+#
+# Pods/
+#
+# Add this line if you want to avoid checking in source code from the Xcode workspace
+# *.xcworkspace
 
-# Nuxt.js build / generate output
-.nuxt
-dist
+# Carthage
+#
+# Add this line if you want to avoid checking in source code from Carthage dependencies.
+# Carthage/Checkouts
 
-# Gatsby files
-.cache/
-# Comment in the public line in if your project uses Gatsby and not Next.js
-# https://nextjs.org/blog/next-9-1#public-directory-support
-# public
+Carthage/Build/
 
-# vuepress build output
-.vuepress/dist
+# fastlane
+#
+# It is recommended to not store the screenshots in the git repo.
+# Instead, use fastlane to re-generate the screenshots whenever they are needed.
+# For more information about the recommended setup visit:
+# https://docs.fastlane.tools/best-practices/source-control/#source-control
 
-# vuepress v2.x temp and cache directory
-.temp
-.cache
+fastlane/report.xml
+fastlane/Preview.html
+fastlane/screenshots/**/*.png
+fastlane/test_output
 
-# Docusaurus cache and generated files
-.docusaurus
+# Code Injection
+#
+# After new code Injection tools there's a generated folder /iOSInjectionProject
+# https://github.com/johnno1962/injectionforxcode
 
-# Serverless directories
-.serverless/
+iOSInjectionProject/
+"""
 
-# FuseBox cache
-.fusebox/
 
-# DynamoDB Local files
-.dynamodb/
+_perl: str = r"""
+!Build/
+.last_cover_stats
+/META.yml
+/META.json
+/MYMETA.*
+*.o
+*.pm.tdy
+*.bs
 
-# TernJS port file
-.tern-port
+# Devel::Cover
+cover_db/
 
-# Stores VSCode versions used for testing VSCode extensions
-.vscode-test
+# Devel::NYTProf
+nytprof.out
 
-# yarn v2
-.yarn/cache
-.yarn/unplugged
-.yarn/build-state.yml
-.yarn/install-state.gz
-.pnp.*
+# Dist::Zilla
+/.build/
+
+# Module::Build
+_build/
+Build
+Build.bat
+
+# Module::Install
+inc/
+
+# ExtUtils::MakeMaker
+/blib/
+/_eumm/
+/*.gz
+/Makefile
+/Makefile.old
+/MANIFEST.bak
+/pm_to_blib
+/*.zip
 """
 
+
 _python: str = r"""
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
@@ -744,14 +852,15 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 """
 
+
 _qt: str = r"""
 # C++ objects and libs
 *.slo
 *.lo
 *.o
 *.a
 *.la
@@ -801,14 +910,15 @@
 
 # QtCreator local machine specific files for imported projects
 *creator.user*
 
 *_qmlcache.qrc
 """
 
+
 _r: str = r"""
 # History files
 .Rhistory
 .Rapp.history
 
 # Session Data files
 .RData
@@ -853,14 +963,15 @@
 # translation temp files
 po/*~
 
 # RStudio Connect folder
 rsconnect/
 """
 
+
 _ros: str = r"""
 devel/
 logs/
 build/
 bin/
 lib/
 msg_gen/
@@ -907,14 +1018,15 @@
 # Emacs
 .#*
 
 # Catkin custom files
 CATKIN_IGNORE
 """
 
+
 _ruby: str = r"""
 *.gem
 *.rbc
 /.config
 /coverage/
 /InstalledFiles
 /pkg/
@@ -966,14 +1078,15 @@
 # unless supporting rvm < 1.11.0 or doing something fancy, ignore this:
 .rvmrc
 
 # Used by RuboCop. Remote config files pulled in from inherit_from directive.
 # .rubocop-https?--*
 """
 
+
 _rust: str = r"""
 # Generated by Cargo
 # will have compiled files and executables
 debug/
 target/
 
 # Remove Cargo.lock from gitignore if creating an executable, leave it for libraries
@@ -983,29 +1096,32 @@
 # These are backup files generated by rustfmt
 **/*.rs.bk
 
 # MSVC Windows builds of rustc generate these, which store debugging information
 *.pdb
 """
 
+
 _sass: str = r"""
 .sass-cache/
 *.css.map
 *.sass.map
 *.scss.map
 """
 
-_scale: str = r"""
+
+_scala: str = r"""
 *.class
 *.log
 
 # virtual machine crash logs, see http://www.java.com/en/download/help/error_hotspot.xml
 hs_err_pid*
 """
 
+
 _swift: str = r"""
 # Xcode
 #
 # gitignore contributors: remember to update Global/Xcode.gitignore, Objective-C.gitignore & Swift.gitignore
 
 ## User settings
 xcuserdata/
@@ -1091,14 +1207,320 @@
 #
 # After new code Injection tools there's a generated folder /iOSInjectionProject
 # https://github.com/johnno1962/injectionforxcode
 
 iOSInjectionProject/
 """
 
+
+_tex: str = r"""
+## Core latex/pdflatex auxiliary files:
+*.aux
+*.lof
+*.log
+*.lot
+*.fls
+*.out
+*.toc
+*.fmt
+*.fot
+*.cb
+*.cb2
+.*.lb
+
+## Intermediate documents:
+*.dvi
+*.xdv
+*-converted-to.*
+# these rules might exclude image files for figures etc.
+# *.ps
+# *.eps
+# *.pdf
+
+## Generated if empty string is given at "Please type another file name for output:"
+.pdf
+
+## Bibliography auxiliary files (bibtex/biblatex/biber):
+*.bbl
+*.bcf
+*.blg
+*-blx.aux
+*-blx.bib
+*.run.xml
+
+## Build tool auxiliary files:
+*.fdb_latexmk
+*.synctex
+*.synctex(busy)
+*.synctex.gz
+*.synctex.gz(busy)
+*.pdfsync
+
+## Build tool directories for auxiliary files
+# latexrun
+latex.out/
+
+## Auxiliary and intermediate files from other packages:
+# algorithms
+*.alg
+*.loa
+
+# achemso
+acs-*.bib
+
+# amsthm
+*.thm
+
+# beamer
+*.nav
+*.pre
+*.snm
+*.vrb
+
+# changes
+*.soc
+
+# comment
+*.cut
+
+# cprotect
+*.cpt
+
+# elsarticle (documentclass of Elsevier journals)
+*.spl
+
+# endnotes
+*.ent
+
+# fixme
+*.lox
+
+# feynmf/feynmp
+*.mf
+*.mp
+*.t[1-9]
+*.t[1-9][0-9]
+*.tfm
+
+#(r)(e)ledmac/(r)(e)ledpar
+*.end
+*.?end
+*.[1-9]
+*.[1-9][0-9]
+*.[1-9][0-9][0-9]
+*.[1-9]R
+*.[1-9][0-9]R
+*.[1-9][0-9][0-9]R
+*.eledsec[1-9]
+*.eledsec[1-9]R
+*.eledsec[1-9][0-9]
+*.eledsec[1-9][0-9]R
+*.eledsec[1-9][0-9][0-9]
+*.eledsec[1-9][0-9][0-9]R
+
+# glossaries
+*.acn
+*.acr
+*.glg
+*.glo
+*.gls
+*.glsdefs
+*.lzo
+*.lzs
+*.slg
+*.slo
+*.sls
+
+# uncomment this for glossaries-extra (will ignore makeindex's style files!)
+# *.ist
+
+# gnuplot
+*.gnuplot
+*.table
+
+# gnuplottex
+*-gnuplottex-*
+
+# gregoriotex
+*.gaux
+*.glog
+*.gtex
+
+# htlatex
+*.4ct
+*.4tc
+*.idv
+*.lg
+*.trc
+*.xref
+
+# hyperref
+*.brf
+
+# knitr
+*-concordance.tex
+# TODO Uncomment the next line if you use knitr and want to ignore its generated tikz files
+# *.tikz
+*-tikzDictionary
+
+# listings
+*.lol
+
+# luatexja-ruby
+*.ltjruby
+
+# makeidx
+*.idx
+*.ilg
+*.ind
+
+# minitoc
+*.maf
+*.mlf
+*.mlt
+*.mtc[0-9]*
+*.slf[0-9]*
+*.slt[0-9]*
+*.stc[0-9]*
+
+# minted
+_minted*
+*.pyg
+
+# morewrites
+*.mw
+
+# newpax
+*.newpax
+
+# nomencl
+*.nlg
+*.nlo
+*.nls
+
+# pax
+*.pax
+
+# pdfpcnotes
+*.pdfpc
+
+# sagetex
+*.sagetex.sage
+*.sagetex.py
+*.sagetex.scmd
+
+# scrwfile
+*.wrt
+
+# svg
+svg-inkscape/
+
+# sympy
+*.sout
+*.sympy
+sympy-plots-for-*.tex/
+
+# pdfcomment
+*.upa
+*.upb
+
+# pythontex
+*.pytxcode
+pythontex-files-*/
+
+# tcolorbox
+*.listing
+
+# thmtools
+*.loe
+
+# TikZ & PGF
+*.dpth
+*.md5
+*.auxlock
+
+# titletoc
+*.ptc
+
+# todonotes
+*.tdo
+
+# vhistory
+*.hst
+*.ver
+
+# easy-todo
+*.lod
+
+# xcolor
+*.xcp
+
+# xmpincl
+*.xmpi
+
+# xindy
+*.xdy
+
+# xypic precompiled matrices and outlines
+*.xyc
+*.xyd
+
+# endfloat
+*.ttt
+*.fff
+
+# Latexian
+TSWLatexianTemp*
+
+## Editors:
+# WinEdt
+*.bak
+*.sav
+
+# Texpad
+.texpadtmp
+
+# LyX
+*.lyx~
+
+# Kile
+*.backup
+
+# gummi
+.*.swp
+
+# KBibTeX
+*~[0-9]*
+
+# TeXnicCenter
+*.tps
+
+# auto folder when using emacs and auctex
+./auto/*
+*.el
+
+# expex forward references with \gathertags
+*-tags.tex
+
+# standalone packages
+*.sta
+
+# Makeindex log files
+*.lpz
+
+# xwatermark package
+*.xwm
+
+# REVTeX puts footnotes in the bibliography by default, unless the nofootinbib
+# option is specified. Footnotes are the stored in a file with suffix Notes.bib.
+# Uncomment the next line to have this generated file ignored.
+#*Notes.bib
+"""
+
+
 _unity: str = r"""
 # This .gitignore file should be placed at the root of your Unity project directory
 #
 # Get latest from https://github.com/github/gitignore/blob/main/Unity.gitignore
 #
 /[Ll]ibrary/
 /[Tt]emp/
@@ -1166,15 +1588,16 @@
 /[Aa]ssets/[Aa]ddressable[Aa]ssets[Dd]ata/*/*.bin*
 
 # Temporary auto-generated Android Assets
 /[Aa]ssets/[Ss]treamingAssets/aa.meta
 /[Aa]ssets/[Ss]treamingAssets/aa/*
 """
 
-_visual_studio: str = r"""
+
+_visualstudio: str = r"""
 ## Ignore Visual Studio temporary files, build results, and
 ## files generated by popular Visual Studio add-ons.
 ##
 ## Get latest from https://github.com/github/gitignore/blob/main/VisualStudio.gitignore
 
 # User-specific files
 *.rsuser
@@ -1570,35 +1993,40 @@
 # JetBrains Rider
 *.sln.iml
 """
 
 
 IGNORE_TEMPLATE: Dict[str, str] = {
     "android": _android,
-    "c++": _cpp,
     "cpp": _cpp,
     "c": _c,
     "cmake": _cmake,
+    "cuda": _cuda,
+    "d": _d,
     "dart": _dart,
     "elisp": _elisp,
+    "erlang": _erlang,
     "gitbook": _gitbook,
     "go": _go,
     "java": _java,
-    "kotlin": _java,
+    "julia": _julia,
+    "kotlin": _kotlin,
     "lua": _lua,
     "maven": _maven,
     "node": _node,
-    "object-c": _object_c,
+    "objective-c": _objective_c,
+    "perl": _perl,
     "python": _python,
     "qt": _qt,
     "r": _r,
     "ros": _ros,
     "ruby": _ruby,
     "rust": _rust,
-    "scale": _scale,
     "sass": _sass,
+    "scala": _scala,
     "swift": _swift,
+    "tex": _tex,
     "unity": _unity,
-    "visualstudio": _visual_studio,
+    "visualstudio": _visualstudio,
 }
 
 __all__ = ("IGNORE_TEMPLATE",)
```

### Comparing `pigit-1.6.1/pigit/gitlib/model.py` & `pigit-1.7.0/pigit/git/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,22 @@
 
     # file whether has merged conflict.
     has_merged_conflicts: bool
 
     # file whether has inline merged conflict.
     has_inline_merged_conflicts: bool
 
+    def get_file_str(self) -> str:
+        """Get the right file path str."""
+        file_name = self.name
+
+        if "->" in file_name:
+            file_name = file_name.split("->")[-1].strip()
+
+        return file_name
 
 @dataclass
 class Commit:
     """Model class of a git commit."""
 
     # The commit sha value.
     sha: str
@@ -74,18 +82,18 @@
 @dataclass
 class Branch:
     """Model class of git branch."""
 
     # The branch name.
     name: str
 
-    # This should be `True` if the branch can be pushing.
-    pushables: str
+    # The ahead time ou upstream, default '?'.
+    ahead: str
 
-    # This should be `True` if the branch can be pulling.
-    pullables: str
+    # The behind time ou upstream, default '?'.
+    behind: str
 
     # This should be `True` if the branch is head.
     is_head: bool
 
     # The branch up-stream name. Default is "".
     upstream_name: str = ""
```

### Comparing `pigit-1.6.1/pigit/gitlib/options.py` & `pigit-1.7.0/pigit/git/repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 # -*- coding:utf-8 -*-
 
+import os
+import re
+import json
+import textwrap
 from typing import Dict, List, Optional, Tuple, Union, Generator
 from collections import Counter
 from pathlib import Path
-import os, re, textwrap, json
 
 from plenty.str_utils import shorten, byte_str2str
 from plenty.console import Console
 
-from pigit.common.utils import (
-    adjudgment_type,
-    async_run_cmd,
-    exec_async_tasks,
-    exec_cmd,
-    get_file_icon,
-)
-from pigit.gitlib.model import File, Commit, Branch
+from pigit.ext.executor import SILENT, WAITING, REPLY, DECODE, Executor
+from pigit.ext.log import logger
+from pigit.ext.utils import adjudgment_type, get_file_icon
+from .model import File, Commit, Branch
 
 
-class GitOptionError(Exception):
+class RepoError(Exception):
     """Error class of ~GitOption."""
 
 
-class GitOption:
+class Repo:
     """Git option class."""
 
     def __init__(
-        self, op_path: Optional[str] = None, repo_json_path: Optional[str] = None
+        self, path: Optional[str] = None, repo_json_path: Optional[str] = None
     ) -> None:
-        self.op_path = op_path
+        """
+        Args:
+            path (Optional[str], optional): repo path. Defaults to None.
+            repo_json_path (Optional[str], optional): repos info json path.
+                Defaults to None.
+        """
+        self.executor = Executor()
+
+        self.path = path
         self.repo_json_path = (
             Path("./repos.json") if repo_json_path is None else Path(repo_json_path)
         )
 
         # create repo path dir.
         self.repo_json_path.parent.mkdir(parents=True, exist_ok=True)
 
     def update_setting(
         self, *, op_path: Optional[str] = None, repo_info_path: Optional[str] = None
-    ) -> "GitOption":
+    ) -> "Repo":
         if op_path is not None:
-            self.op_path = op_path
+            self.path = op_path
         if repo_info_path is not None:
-            self.repo_json_path = repo_info_path
+            self.repo_json_path = Path(repo_info_path)
 
         return self
 
     # ==================
     # Basic info option
     # ==================
-    @property
-    def git_version(self) -> str:
-        """Get Git version."""
-
-        _, _version = exec_cmd("git --version")
-        return _version.strip() or ""
-
-    def get_repo_info(
+    def confirm_repo(
         self, given_path: Optional[str] = None, exclude_submodule: bool = False
     ) -> Tuple[str, str]:
-        """
+        """Confirm given path whether a git repo. And return repo path info.
         Get the current git repository path. If not, the path is empty.
         Get the local git config path. If not, the path is empty.
 
-        Return:
-                (tuple[str, str]): repository path, git config path.
+        Returns:
+            (tuple[str, str]): repository path, git config path.
         """
+        path = given_path or self.path or "."
+        path = os.path.abspath(path)
 
-        path = given_path or self.op_path or "."
         repo_path: str = ""
         git_conf_path: str = ""
 
-        path = os.path.abspath(path)
         if not os.path.isdir(path):
             return repo_path, git_conf_path
 
-        err, repo_path = exec_cmd("git rev-parse --git-dir", cwd=path)
+        _, err, repo_path = self.executor.exec(
+            "git rev-parse --git-dir", flags=REPLY | DECODE, cwd=path
+        )
         if err:
             return repo_path, git_conf_path
 
         # remove useless space.
         repo_path = repo_path.strip()
 
         if ".git/modules/" in repo_path and not exclude_submodule:
@@ -91,96 +93,149 @@
             git_conf_path = os.path.join(repo_path, ".git")
         else:
             git_conf_path = repo_path
             repo_path = repo_path[:-5]
 
         return repo_path, git_conf_path
 
+    def get_config(self, path: Optional[str] = None) -> Dict[str, Dict[str, str]]:
+        """Try to read git config and parse, return a config dict.
+
+        Args:
+            path (Optional[str], optional): repo path. Defaults to None.
+
+        Returns:
+            Dict[str, Dict[str, str]]: config dict.
+        """
+        path = path or self.path
+
+        _, config_path = self.confirm_repo(path)
+        try:
+            with open(f"{config_path}/config", "r") as cf:
+                context = cf.read()
+        except Exception as e:
+            logger(__name__).warning(f"Can not read config with: {e}")
+            return {}
+        else:
+            conf_dict: Dict[str, Dict[str, str]] = {}
+            conf_list = re.split(r"\r\n|\r|\n", context)
+            config_type: str = ""
+
+            for line in conf_list:
+                line = line.strip()
+
+                if not line:
+                    continue
+
+                elif line.startswith("["):
+                    config_type = line[1:-1].strip()
+                    conf_dict[config_type] = {}
+
+                elif "=" in line:
+                    key, value = line.split("=", 1)
+                    conf_dict[config_type][key.strip()] = value.strip()
+
+                else:
+                    continue
+
+            return conf_dict
+
     def get_head(self, path: Optional[str] = None) -> Optional[str]:
         """Get current repo head. Return a branch name or a commit sha string."""
+        path = path or self.path
 
-        path = path or self.op_path
-        _, res = exec_cmd(
+        _, _, head = self.executor.exec(
             "git symbolic-ref -q --short HEAD || git describe --tags --exact-match",
+            flags=REPLY | DECODE,
             cwd=path,
         )
-        if res is not None:
-            res = res.rstrip()
-        return res
+        if head is not None:
+            head = head.rstrip()
+        return head
+
+    def get_first_pushed_commit(
+        self, path: Optional[str] = None, branch_name: Optional[str] = None
+    ) -> str:
+        path = path or self.path
+
+        if branch_name is None:
+            if head := self.get_head(path):
+                branch_name = head
+            else:
+                return ""
+
+        command = "git merge-base %s %s@{u}" % (branch_name, branch_name)
+        _, _, commit_msg = self.executor.exec(command, flags=REPLY | DECODE, cwd=path)
+        return commit_msg.strip()
 
     def get_branches(
         self,
         path: Optional[str] = None,
         include_remote: bool = False,
         plain: bool = True,
     ) -> List[str]:
         """Get repo all branch."""
+        path = path or self.path
 
-        path = path or self.op_path
-        include_remote = "--all" if include_remote else ""
+        include_all = "--all" if include_remote else ""
         color = "never" if plain else "always"
 
-        err, res = exec_cmd(f"git branch {include_remote} --color={color}", cwd=path)
+        _, _, res = self.executor.exec(
+            f"git branch {include_all} --color={color}",
+            flags=REPLY | DECODE,
+            cwd=path,
+        )
 
         if res is None:
             return []
         return [branch[2:] for branch in res.rstrip().split("\n")]
 
-    def get_first_pushed_commit(
-        self, path: Optional[str] = None, branch_name: Optional[str] = None
-    ) -> str:
-        path = path or self.op_path
-
-        if branch_name is None:
-            if branches := self.get_branches(path):
-                branch_name = branches[0]
-            else:
-                return ""
-
-        command = "git merge-base %s %s@{u}" % (branch_name, branch_name)
-        _, resp = exec_cmd(command, cwd=path)
-        return resp.strip()
-
     def get_remotes(self, path: Optional[str] = None) -> List[str]:
         """Get repo remote url."""
 
         # Get remote name, exit when error.
-        path = path or self.op_path
-        err, res = exec_cmd("git remote show", cwd=path)
+        path = path or self.path
+        _, _, res = self.executor.exec(
+            "git remote show", flags=REPLY | DECODE, cwd=path
+        )
 
-        return [] if err else res.strip().split("\n")
+        return res.strip().split("\n") if res else []
 
     def get_remote_url(
         self, path: Optional[str] = None, remote_name: Optional[str] = None
     ) -> str:
         """Get repo remote url."""
+        path = path or self.path
 
-        path = path or self.op_path
         if remote_name is None:
             if remotes := self.get_remotes(path):
                 remote_name = remotes[0]
             else:
                 return ""
 
         # Get remote url, exit when error.
-        err, remote_url = exec_cmd(f"git ls-remote --get-url {remote_name}", cwd=path)
+        _, err, remote_url = self.executor.exec(
+            f"git ls-remote --get-url {remote_name}", flags=REPLY | DECODE, cwd=path
+        )
 
         if err:
             return ""
 
         remote_url = remote_url[:-5]
         return remote_url
 
     def get_summary(self, path: Optional[str] = None, plain: bool = True) -> str:
-        path = path or self.op_path
+        path = path or self.path
         color = "never" if plain else "always"
-        err, res = exec_cmd(
-            f"git shortlog --summary --numbered --color={color}", cwd=path
+        _, _, summary = self.executor.exec(
+            f"git shortlog --summary --numbered --color={color}",
+            flags=REPLY | DECODE,
+            cwd=path,
         )
-        return res
+        return summary
 
     def get_repo_desc(
         self,
         include_part: Optional[List] = None,
         path: Optional[str] = None,
         color: bool = True,
     ) -> str:
@@ -190,19 +245,18 @@
                 include_part (Optional[list], optional): should return info part: [path,remote,branch,log,summary]. Defaults to None.
                 path (Optional[str], optional): custom repo path. Defaults to None.
                 color (bool, optional): whether return with color. Defaults to True.
 
         Returns:
                 str: desc info.
         """
-
-        path = path or self.op_path
+        path = path or self.path
         error_str = "`Error getting.`<error>"
         gen = ["[b`Repository Information`]" if color else "[Repository Information]"]
-        repo_path, _ = self.get_repo_info(path)
+        repo_path, _ = self.confirm_repo(path)
 
         # Get content.
         if not include_part or "path" in include_part:
             gen.append(
                 f"Repository: \n\t`{repo_path}`<sky_blue>\n"
                 if color
                 else f"Repository: \n\t{repo_path}\n"
@@ -228,109 +282,118 @@
             branches_str = (
                 "\n".join(f"\t{branch}" for branch in branches)
                 if branches
                 else f"\t{error_str}"
             )
             gen.append("Branches: \n%s\n" % branches_str)
 
-        # Get the lastest log.
+        # Get the latest log.
         if not include_part or "log" in include_part:
-            err, res = exec_cmd(
+            _, err, res = self.executor.exec(
                 f"git log --stat --oneline --decorate -1 --color={'always' if color else 'never'}",
+                flags=REPLY | DECODE,
                 cwd=path,
             )
             git_log = "\t" + error_str if err else textwrap.indent(res, "\t")
-            gen.append("Lastest log:\n%s\n" % git_log)
+            gen.append("Latest log:\n%s\n" % git_log)
 
         # FIXME: will broken in a init repo.
         # Get git summary.
         # if not include_part or "summary" in include_part:
         #     summary = self.get_summary(path, not color)
         #     gen.append("Summary:\n%s\n" % summary or error_str)
 
         return "\n".join(gen)
 
     # =============
     # Special info
     # =============
     def load_branches(self, path: Optional[str] = None) -> List[Branch]:
-        path = path or self.op_path
-        command = (
-            "git branch --sort=-committerdate "
-            '--format="%(HEAD)|%(refname:short)|%(upstream:short)|%(upstream:track)" '
-        )
+        path = path or self.path
         branches = []
 
-        err, resp = exec_cmd(command, cwd=path)
+        _, _, resp = self.executor.exec(
+            "git branch --sort=-committerdate "
+            '--format="%(HEAD)|%(refname:short)|%(upstream:short)|%(upstream:track)" ',
+            flags=REPLY | DECODE,
+            cwd=path,
+        )
         resp = resp.strip()
         if not resp:
             return branches
 
         lines = resp.split("\n")
 
         for line in lines:
             items = line.split("|")
             branch = Branch(
-                name=items[1], pushables="?", pullables="?", is_head=items[0] == "*"
+                name=items[1], ahead="?", behind="?", is_head=items[0] == "*"
             )
 
             upstream_name = items[2]
 
             if not upstream_name:
                 branches.append(branch)
                 continue
 
             branch.upstream_name = upstream_name
 
             track = items[3]
             _re = re.compile(r"ahead (\d+)")
-            branch.pushables = str(match[1]) if (match := _re.search(track)) else "0"
+            branch.ahead = str(match[1]) if (match := _re.search(track)) else "0"
             _re = re.compile(r"behind (\d+)")
-            branch.pullables = str(match[1]) if (match := _re.search(track)) else "0"
+            branch.behind = str(match[1]) if (match := _re.search(track)) else "0"
             branches.append(branch)
 
         return branches
 
     def load_log(
         self,
         branch_name: str = "",
         limit: Optional[int] = None,
         filter_path: str = "",
         arg_str: str = '--oneline --pretty=format:"%H|%at|%aN|%d|%p|%s" --abbrev=20 --date=unix',
         path: Optional[str] = None,
     ) -> str:
-        path = path or self.op_path
+        path = path or self.path
+
         limit_flag = f"-{limit}" if limit else ""
         filter_flag = f"--follow -- {filter_path}" if filter_path else ""
 
-        command = f"git log {branch_name} {arg_str} {limit_flag}  {filter_flag}"
-        err, resp = exec_cmd(command, cwd=path)
+        _, _, resp = self.executor.exec(
+            f"git log {branch_name} {arg_str} {limit_flag} {filter_flag}",
+            flags=REPLY | DECODE,
+            cwd=path,
+        )
 
         return "" if resp is None else resp.strip()
 
     def load_status(
         self,
         max_width: int = 80,
         ident: int = 2,
         plain: bool = False,
         path: Optional[str] = None,
         icon: bool = False,
     ) -> List[File]:
         """Get the file tree status of GIT for processing and encapsulation.
+
         Args:
                 max_width (int): The max length of display string.
                 ident (int, option): Number of reserved blank characters in the header.
+
         Returns:
                 (List[File]): Processed file status list.
         """
-
-        path = path or self.op_path
+        path = path or self.path
         file_items = []
 
-        err, files = exec_cmd("git status -s -u --porcelain", cwd=path)
+        _, err, files = self.executor.exec(
+            "git status -s -u --porcelain", flags=REPLY | DECODE, cwd=path
+        )
         if err:
             return file_items
         for file in files.rstrip().split("\n"):
             if not file.strip():
                 # skip blank line.
                 continue
 
@@ -374,71 +437,70 @@
 
     def load_file_diff(
         self,
         file: str,
         tracked: bool = True,
         cached: bool = False,
         plain: bool = False,
-        path: str = None,
+        path: Optional[str] = None,
     ) -> str:
         """Gets the modification of the file.
+
         Args:
                 file (str): file path relative to git.
                 tracked (bool, optional): Defaults to True.
                 cached (bool, optional): Defaults to False.
                 plain (bool, optional): Whether need color. Defaults to False.
+
         Returns:
                 (str): change string.
         """
-
-        path = path or self.op_path
-        command = "git diff --submodule --no-ext-diff {plain} {cached} {tracked} {file}"
+        path = path or self.path
 
         _plain = "--color=never" if plain else "--color=always"
         _cached = "--cached" if cached else ""
         _tracked = "--" if tracked else "--no-index -- /dev/null"
 
         if "->" in file:  # rename status.
             file = file.split("->")[-1].strip()
 
-        err, res = exec_cmd(
-            command.format(plain=_plain, cached=_cached, tracked=_tracked, file=file),
+        _, err, res = self.executor.exec(
+            f"git diff --submodule --no-ext-diff {_plain} {_cached} {_tracked} {file}",
+            flags=REPLY | DECODE,
             cwd=path,
         )
         return "Can't get diff." if err else res.rstrip()
 
     def load_commits(
         self,
         branch_name: str,
         limit: bool = True,
         filter_path: str = "",
         path: Optional[str] = None,
     ) -> List[Commit]:
         """Get the all commit of a given branch.
+
         Args:
                 branch_name (str): want branch name.
                 limit (bool): Whether to get only the latest 300.
                 filter_path (str): filter dir path, default is empty.
         """
+        path = path or self.path
 
-        path = path or self.op_path
-        command = "git merge-base %s %s@{u}" % (branch_name, branch_name)
-
-        _, resp = exec_cmd(command, cwd=path)
-        first_pushed_commit = resp.strip()
-
+        first_pushed_commit = self.get_first_pushed_commit(path, branch_name)
         passed_first_pushed_commit = not first_pushed_commit
+
         commits: List[Commit] = []
 
         # Generate git command.
         limit_flag = "-300" if limit else ""
         filter_flag = f"--follow -- {filter_path}" if filter_path else ""
         command = f'git log {branch_name} --oneline --pretty=format:"%H|%at|%aN|%d|%p|%s" {limit_flag} --abbrev=20 --date=unix {filter_flag}'
 
-        err, resp = exec_cmd(command, cwd=path)
+        _, err, resp = self.executor.exec(command, flags=REPLY | DECODE, cwd=path)
         if err:
             return commits  # current is empty list.
 
         # Process data.
         for line in resp.split("\n"):
             split_ = line.split("|")
 
@@ -470,108 +532,112 @@
             )
             commits.append(commit_)
 
         return commits
 
     def load_commit_info(
         self,
-        commit_sha: str,
+        commit_sha: str = "",
         file_name: str = "",
         plain: bool = False,
         path: Optional[str] = None,
     ) -> str:
         """Gets the change of a file or all in a given commit.
         Args:
                 commit_sha: commit id.
                 file_name: file name(include full path).
                 plain: whether has color.
         """
-
-        path = path or self.op_path
+        path = path or self.path
         color_str = "never" if plain else "always"
 
-        command = f"git show --color={color_str} {commit_sha} {file_name}"
-        _, resp = exec_cmd(command, cwd=path)
+        _, _, resp = self.executor.exec(
+            f"git show --color={color_str} {commit_sha} {file_name}",
+            flags=REPLY | DECODE,
+            cwd=path,
+        )
         return resp.rstrip()
 
     # ===============
     # Options of git
     # ===============
-    def _get_file_str(self, file) -> str:
-        if isinstance(file, File):
-            file_name = file.name
-        elif isinstance(file, str):
-            file_name = file
-        else:
-            raise GitOptionError("`file` only allow 'str' or 'File'.") from None
+    def switch_file_status(self, file: File, path: Optional[str] = None):
+        """Change the file stage status.
 
-        if "->" in file_name:
-            file_name = file_name.split("->")[-1].strip()
-
-        return file_name
-
-    def switch_file_status(self, file: Union[File, str], path: Optional[str] = None):
-        path = path or self.op_path
-        file_name = self._get_file_str(file)
+        Args:
+            file (File): git file object.
+            path (Optional[str], optional): exec path. Defaults to None.
+        """
+        path = path or self.path
+        file_name = file.get_file_str()
 
         if file.has_merged_conflicts or file.has_inline_merged_conflicts:
             pass
         elif file.has_unstaged_change:
-            exec_cmd(f"git add -- '{file_name}'", cwd=path)
+            self.executor.exec(
+                f"git add -- '{file_name}'", flags=WAITING | SILENT, cwd=path
+            )
         elif file.has_staged_change:
             if file.tracked:
-                exec_cmd(f"git reset HEAD -- '{file_name}'", cwd=path)
+                self.executor.exec(
+                    f"git reset HEAD -- '{file_name}'",
+                    flags=WAITING | SILENT,
+                    cwd=path,
+                )
             else:
-                exec_cmd(f"git rm --cached --force -- '{file_name}'", cwd=path)
+                self.executor.exec(
+                    f"git rm --cached --force -- '{file_name}'",
+                    flags=WAITING | SILENT,
+                    cwd=path,
+                )
 
     def discard_file(
         self,
         file: Union[File, str],
         path: Optional[str] = None,
         tracked: Optional[bool] = None,
     ):
-        path = path or self.op_path
-        file_name = self._get_file_str(file)
+        path = path or self.path
+        file_name = file.get_file_str()
 
         if tracked is None:
             if isinstance(file, File):
                 tracked = file.tracked
             else:
-                raise GitOptionError("Please set `tracked` or give a 'File'.") from None
+                raise RepoError("Please set `tracked` or give a 'File'.") from None
 
         if tracked:
-            exec_cmd(f"git checkout -- {file_name}", cwd=path)
+            self.executor.exec(f"git checkout -- {file_name}", cwd=path)
         else:
-            repo_path, _ = self.get_repo_info(path)
-            os.remove(os.path.join(repo_path, file_name))
+            os.remove(os.path.join(path or "", file_name))
 
     def ignore_file(self, file: Union[File, str], path: Optional[str] = None):
         """Append file to `.gitignore` file."""
 
-        path = path or self.op_path
-        repo_path, _ = self.get_repo_info(path)
-        file_name = self._get_file_str(file)
+        path = path or self.path
+        repo_path, _ = self.confirm_repo(path)
+        file_name = file.get_file_str()
 
         with open(f"{repo_path}/.gitignore", "a+") as f:
             f.write(f"\n{file_name}")
 
     def checkout_branch(self, branch_name: str, path: Optional[str] = None) -> str:
-        path = path or self.op_path
-        err, _ = exec_cmd(f"git checkout {branch_name}", cwd=path)
+        path = path or self.path
+        _, err, _ = self.executor.exec(f"git checkout {branch_name}", cwd=path)
         return err or "ok"
 
     def open_repo_in_browser(
         self,
         path: Optional[str] = None,
         branch: str = "",
         issue: str = "",
         commit: str = "",
         print: bool = False,
-    ) -> bool:
-        path = path or self.op_path
+    ) -> Tuple[bool, str]:
+        path = path or self.path
         remote_url = self.get_remote_url(path=path)
 
         if branch:
             branch = f"/tree/{branch}"
             remote_url += branch
         elif issue:
             issue = f"/issues/{issue}"
@@ -589,18 +655,18 @@
             webbrowser.open(remote_url)
         except Exception as e:
             return False, f"Failed to open the repo; {e}"
         else:
             return True, "Successfully opened repo."
 
     # ====================
-    # custom repo options
+    # custom repos option
     # ====================
     @staticmethod
-    def _make_repo_name(path: str, repos: List[str], name_counts: Counter) -> str:
+    def _make_repo_name(path: str, repos: Dict[str, str], name_counts: Counter) -> str:
         """
         Given a new repo `path`, create a repo name. By default, basename is used.
         If name collision exists, further include parent path name.
 
         Args:
             path (str): repo path.
             repos (list[str]): path list of exist repos.
@@ -614,31 +680,88 @@
         if name in repos or name_counts[name] > 1:
             # path has no trailing /
             par_name = os.path.basename(os.path.dirname(path))
             return os.path.join(par_name, name)
         return name
 
     def load_repos(self) -> Dict:
+        """Load repos info from cache file."""
+
         if not self.repo_json_path.is_file():
             return {}
 
         with self.repo_json_path.open(mode="r") as fp:
             return json.load(fp)
 
-    def save_repos(self, repos: Dict) -> bool:
+    def dump_repos(self, repos: Dict) -> bool:
+        """Dump repos info to cache file, re-write mode."""
+
         try:
             with self.repo_json_path.open(mode="w+") as fp:
                 json.dump(repos, fp, indent=2)
                 return True
         except Exception:
             return False
 
     def clear_repos(self) -> None:
         self.repo_json_path.unlink(missing_ok=True)
 
+    def ll_repos(self, reverse: bool = False) -> Generator[List[Tuple], None, None]:
+        exist_repos = self.load_repos()
+
+        for repo_name, prop in exist_repos.items():
+            repo_path = prop["path"]
+            head = self.get_head(repo_path)
+
+            # jump invalid repo.
+            if head is None:
+                if reverse:
+                    yield [
+                        (repo_name, ""),
+                        ("Local Path", repo_path),
+                    ]
+
+            elif not reverse:
+                _, _, unstaged = self.executor.exec(
+                    "git diff --stat", flags=REPLY | DECODE, cwd=repo_path
+                )
+                _, _, staged = self.executor.exec(
+                    "git diff --stat --cached", flags=REPLY | DECODE, cwd=repo_path
+                )
+                _, _, untracked = self.executor.exec(
+                    "git ls-files -zo --exclude-standard",
+                    flags=REPLY | DECODE,
+                    cwd=repo_path,
+                )
+                commit_hash = self.get_first_pushed_commit(
+                    path=repo_path, branch_name=head
+                )
+                commit = self.load_log(
+                    limit=1,
+                    arg_str="--format='%s (%cd)||%C(auto)%d%n' --date=relative --color",
+                    path=repo_path,
+                )
+
+                commit_msg, branch_status = commit.strip().split("||")
+                unstaged_symbol = "*" if unstaged else " "
+                staged_symbol = "+" if staged else " "
+                untracked_symbol = "?" if untracked else " "
+
+                yield [
+                    (repo_name, ""),
+                    (
+                        "Branch",
+                        f"{head} {unstaged_symbol}{staged_symbol}{untracked_symbol}",
+                    ),
+                    ("Status", branch_status),
+                    ("Commit Hash", commit_hash),
+                    ("Commit Msg", commit_msg),
+                    ("Local Path", repo_path),
+                ]
+
     def add_repos(self, paths: List[str], dry_run: bool = False) -> List:
         """Traverse the incoming paths. If it is not saved and is a git
         directory, add it to repos.
 
         Args:
             paths (list[str]): incoming paths.
             dry_run (bool, optional): Show but not really execute. Defaults to False.
@@ -646,28 +769,28 @@
         """
 
         exist_repos = self.load_repos()
         exist_paths = [r["path"] for r in exist_repos.values()]
 
         new_git_paths = []
         for path in paths:
-            repo_path, _ = self.get_repo_info(path)
+            repo_path, _ = self.confirm_repo(path)
             if repo_path and repo_path not in exist_paths:
                 new_git_paths.append(repo_path)
 
         if new_git_paths and not dry_run:
             name_counts = Counter(
                 os.path.basename(os.path.normpath(p)) for p in new_git_paths
             )
             new_repos = {
                 self._make_repo_name(path, exist_repos, name_counts): {"path": path}
                 for path in new_git_paths
             }
 
-            self.save_repos({**exist_repos, **new_repos})
+            self.dump_repos({**exist_repos, **new_repos})
 
         return new_git_paths
 
     def rm_repos(self, repos: List[str], use_path: bool = False) -> List[Tuple]:
         exist_repos = self.load_repos()
 
         del_repos = []
@@ -679,87 +802,88 @@
         else:
             del_repos.extend(repo for repo in repos if exist_repos.get(repo))
 
         for repo in del_repos:
             del_paths.append(exist_repos[repo]["path"])
             del exist_repos[repo]
 
-        self.save_repos(exist_repos)
-        return zip(del_repos, del_paths)
+        self.dump_repos(exist_repos)
+        return list(zip(del_repos, del_paths))
 
     def rename_repo(self, repo: str, name: str) -> Tuple[bool, str]:
+        """Rename repo
+
+        Args:
+            repo (str): exist repo name
+            name (str): new name
+
+        Returns:
+            Tuple[bool, str]: whether rename successful, tip msg.
+        """
+
         exist_repos = self.load_repos()
 
-        if name in exist_repos:
+        if name == repo:
+            return False, "The same name do nothing!"
+        elif name in exist_repos:
             return False, f"'{name}' is already in use!"
         elif repo not in exist_repos:
             return False, f"'{repo}' is not a valid repo name!"
         else:
             prop = exist_repos[repo]
             del exist_repos[repo]
             exist_repos[name] = prop
 
-            self.save_repos(exist_repos)
+            self.dump_repos(exist_repos)
             return True, f"rename successful, `{repo}`->`{name}`."
 
-    def ll_repos(self, revese: bool = False) -> Generator[List[Tuple], None, None]:
-        exist_repos = self.load_repos()
+    def cd_repo(self, repo: Optional[str] = None):
+        """Quick jump to repo dir.
 
-        for repo_name, prop in exist_repos.items():
-            repo_path = prop["path"]
-            head = self.get_head(repo_path)
+        Args:
+            repo (Optional[str], optional): repo name. Defaults to None.
 
-            # jump invalid repo.
-            if head is None:
-                if revese:
-                    yield [
-                        (repo_name, ""),
-                        ("Local Path", repo_path),
-                    ]
+        Returns:
+            _type_: _description_
+        """
 
-            elif not revese:
-                _, unstaged = exec_cmd("git diff --stat", cwd=repo_path)
-                _, staged = exec_cmd("git diff --stat --cached", cwd=repo_path)
-                _, untracked = exec_cmd(
-                    "git ls-files -zo --exclude-standard", cwd=repo_path
-                )
-                commit_hash = self.get_first_pushed_commit(
-                    path=repo_path, branch_name=head
-                )
-                commit = self.load_log(
-                    limit=1,
-                    arg_str="--format='%s (%cd)||%C(auto)%d%n' --date=relative --color",
-                    path=repo_path,
-                )
+        command = "$SHELL -c 'cd {0} && exec $SHELL'"
+        exist_repos = self.load_repos()
 
-                commit_msg, branch_status = commit.strip().split("||")
-                unstaged_symbol = "*" if unstaged else " "
-                staged_symbol = "+" if staged else " "
-                untracked_symbol = "?" if untracked else " "
+        if repo in exist_repos:
+            path = exist_repos[repo]["path"]
+            self.executor.exec(command.format(path), flags=WAITING)
+        else:
+            cur_cache = []
+            print("Managed repos include the following:")
+            for i, r in enumerate(exist_repos, 0):
+                cur_cache.append(r)
+                print(".  ", i, r)
 
-                yield [
-                    (repo_name, ""),
-                    (
-                        "Branch",
-                        f"{head} {unstaged_symbol}{staged_symbol}{untracked_symbol}",
-                    ),
-                    ("Status", branch_status),
-                    ("Commit Hash", commit_hash),
-                    ("Commit Msg", commit_msg),
-                    ("Local Path", repo_path),
-                ]
+            try:
+                input_num = int(input("Please input the index:"))
+                if 0 <= input_num <= len(cur_cache):
+                    path = exist_repos[cur_cache[input_num]]["path"]
+                    print(self.executor.exec(command.format(path), cwd=".", flags=WAITING))
+                else:
+                    print("Error: index out of range.")
+            except Exception:
+                print("Error: index need input a number.")
 
-    def process_repo_option(self, repos: Optional[List[str]], cmd: str):
+    def process_repos_option(self, repos: Optional[List[str]], cmd: str):
         exist_repos = self.load_repos()
         print(f":: {cmd}\n")
 
         if repos:
             exist_repos = {k: v for k, v in exist_repos.items() if k in repos}
 
         if len(exist_repos) >= 1:
-            return exec_async_tasks(
-                async_run_cmd(*cmd.split(), cwd=prop["path"], msg=f":: {prop['path']}")
-                for name, prop in exist_repos.items()
-            )
+            cmds = []
+            orders = []
+            for _, prop in exist_repos.items():
+                cmds.append(cmd)
+                orders.append({"cwd": prop["path"]})
+
+            return self.executor.exec_parallel(*cmds, orders=orders, flags=WAITING)
 
         for _, prop in exist_repos.items():
-            exec_cmd(cmd, prop["path"])
+            self.executor.exec(cmd, flags=WAITING, cwd=prop["path"])
```

### Comparing `pigit-1.6.1/pigit/gitlib/processor.py` & `pigit-1.7.0/pigit/git/proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding:utf-8 -*-
 
+import os
+import re
+import random
+import textwrap
 from typing import Callable, Dict, List, Optional, Tuple, Union
-import os, re, textwrap, random, logging
 
-from plenty import get_console
-from plenty.str_utils import shorten
-
-from ..common.utils import exec_cmd, confirm, similar_command, traceback_info
-from ..common.singleton import Singleton
-from .shortcmds import GIT_CMDS, CommandType
-
-Log = logging.getLogger(__name__)
+from pigit.ext.log import logger
+from pigit.ext.utils import confirm, similar_command, traceback_info
+from pigit.ext.executor import Executor, WAITING
+from ._cmds import Git_Proxy_Cmds, GitCommandType
 
 
 def get_extra_cmds(name: str, path: str) -> Dict:
     """Get custom cmds.
 
     Load the `extra_cmds.py` file under PIGIT HOME, check whether `extra_cmds`
     exists, and return it. If not have, return a empty dict.
@@ -24,60 +23,71 @@
     """
     import importlib.util
 
     extra_cmds = {}
 
     if os.path.isfile(path):
         try:
-            # load a module form localtion.
+            # load a module form location.
             spec = importlib.util.spec_from_file_location(name, path)
+            if spec is None:
+                raise ValueError("spec is None")
+            if spec.loader is None:
+                raise ValueError("spec.loader is None")
+
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
         except Exception:
-            Log.error(traceback_info(f"Can't load file '{path}'."))
+            logger(__name__).error(traceback_info(f"Can't load file '{path}'."))
         else:
             try:
                 extra_cmds = module.extra_cmds  # type: ignore
             except AttributeError:
-                Log.error("Can't found dict name is 'extra_cmds'.")
+                logger(__name__).error("Can't found dict name is 'extra_cmds'.")
 
     return extra_cmds
 
 
-class ShortGitter(metaclass=Singleton):
-    """Git short command processor."""
+class GitProxy:
+    """Git short command proxy `handler."""
 
     def __init__(
         self,
         extra_cmds: Optional[dict] = None,
-        command_prompt: bool = True,
-        show_original: bool = True,
-        **kwargs,
+        prompt: bool = True,
+        display: bool = True,
     ) -> None:
+        self.prompt = prompt
+        self.display = display
 
-        self.use_recommend = command_prompt
-        self.show_original = show_original
+        self.executor = Executor()
 
         # Init commands.
-        self.cmds = GIT_CMDS
+        self.cmds = Git_Proxy_Cmds
         if extra_cmds:
             if not isinstance(extra_cmds, dict):
                 raise TypeError("Custom cmds must be a dict.") from None
             self.cmds.update(extra_cmds)
 
     @staticmethod
     def color_command(command: str) -> str:
         """Return the command string with color.
         prog      : green;
         command   : yellow;
         arguments : skyblue;
         values    : white.
-        """
 
+        Returns:
+            str: command with color tags.
+        """
         handle = re.match(r"(\w+)\s+(\w+)", command)
+        # Unable to match correctly.
+        if handle is None:
+            return f"Not valid command: '{command}'"
+
         prop = handle[1]
         cmd = handle[2]
         next_position = handle.span()[1]
 
         color_command = f"b`{prop}`<ok> b`{cmd}`<goldenrod> "
 
         arguments = re.findall(
@@ -85,82 +95,89 @@
         )
         for arg_handle, value, _, _ in arguments:
             color_command += f"`{arg_handle}`<sky_blue>{value} "
 
         return color_command
 
     def process_command(
-        self, command_string: str, args: Optional[Union[List, Tuple]] = None
+        self, short_cmd: str, args: Optional[Union[List, Tuple]] = None
     ) -> Tuple[int, str]:
         """Process command and arguments.
 
         Args:
             command_ (str): short command string
             args (list|None, optional): command arguments. Defaults to None.
-        """
 
-        option: Optional[Dict[str, Dict]] = self.cmds.get(command_string, None)
+        Returns:
+            Tuple[int, str]: (code, msg)
+                code:
+                    0: successful with msg.
+                    1: has no option item.
+                    2: has no cmd string.
+                    3: func cmd exec error.
+                    5: not supported cmd type.
+        """
+        msgs: List[str] = []
+        option = self.cmds.get(short_cmd)
 
         # Invalid, if need suggest.
         if option is None:
             return (
                 1,
-                f"Don't support this command: `{command_string}`<error>, "
+                f"Don't support this command: `{short_cmd}`<error>, "
                 "please try `--show-commands`<gold>",
             )
 
-        command: Optional[Union[str, Callable]] = option.get("command")
+        command = option.get("command")
+
         # Has no command can be executed.
         if not command:
             return 2, "`Invalid custom short command, nothing can to exec.`<error>"
 
+        # Invalid args need tip.
         if not option.get("has_arguments", False) and args:
-            get_console().echo(
+            args = []
+            msgs.append(
                 f"`The command does not accept parameters. Discard {args}.`<error>"
             )
-            args = []
 
         if isinstance(command, Callable):
             try:
-                command(args)
+                # exec func and return msg.
+                return 0, command(args)
             except Exception as e:
                 return 3, f"`{e}`<error>"
         elif isinstance(command, str):
             if args:
                 command = " ".join([command, *args])
-            if self.show_original:
-                get_console().echo(f":rainbow:  {self.color_command(command)}")
-            exec_cmd(command, reply=False)
+            if self.display:
+                msgs.append(f":rainbow:  {self.color_command(command)}")
+            self.executor.exec(command, flags=WAITING)
         else:
             return 5, "`The type of command not supported.`<error>"
 
-        return 0, ""
+        return 0, "\n".join(msgs)
 
-    def do(self, command_string: str, args: Optional[Union[List, Tuple]] = None):
+    def do(self, short_cmd: str, args: Optional[Union[List, Tuple]] = None) -> str:
         """Process command and arguments."""
 
-        code, msg = self.process_command(command_string, args)
-        if code == 0:
-            pass
-        elif code == 1 and self.use_recommend:  # check config.
-            predicted_command = similar_command(command_string, self.cmds.keys())
-            if confirm(
-                get_console().render_str(
-                    f":thinking: The wanted command is `{predicted_command}`<ok> ?[y/n]:"
-                )
-            ):
-                self.do(predicted_command, args=args)
-        else:
-            get_console().echo(msg)
+        code, msg = self.process_command(short_cmd, args)
+
+        if code == 1 and self.prompt:  # check config.
+            predicted_command = similar_command(short_cmd, self.cmds.keys())
+            if confirm(f":TIPS: The wanted command is `{predicted_command}`?[y/n]:"):
+                return self.do(predicted_command, args=args)
+
+        return msg
 
     # ============================
     # Print command help message.
     # ============================
-    def _generate_help_by_key(
-        self, _key: str, use_color: bool = True, max_width=90
+    def generate_help_by_key(
+        self, key: str, use_color: bool = True, max_width: int = 90
     ) -> str:
         """Generate one help by given key.
 
         Args:
             _key (str): Short command string.
             use_color (bool, optional): Whether color help message. Defaults to True.
 
@@ -168,92 +185,93 @@
             (str): Help message of one command.
         """
 
         help_position = 15
         msg_max_width = max_width - help_position
 
         # Get help message and command.
-        _help: str = self.cmds[_key].get("help", "").strip()
+        _help: str = self.cmds[key].get("help", "").strip()
         if _help:
-            _help = textwrap.wrap(_help, msg_max_width)
-            help_msg = _help[0] + "\n"
-            for line in _help[1:]:
+            _wraps = textwrap.wrap(_help, msg_max_width)
+            help_msg = _wraps[0] + "\n"
+            for line in _wraps[1:]:
                 help_msg += "%*s%s\n" % (help_position, "", line)
         else:
             help_msg = ""
 
-        _command = self.cmds[_key].get("command", "ERROR: empty command.")
+        _command = self.cmds[key].get("command", "ERROR: empty command.")
         if callable(_command):
             _command = f"Func: {_command.__name__}"
 
-        _command = shorten(_command, msg_max_width, placeholder="...")
         command_msg = "%*s%s" % (help_position, "", _command) if help_msg else _command
 
         if use_color:
-            return f"  `{_key:<13}`<ok>{help_msg}`{command_msg}`<gold>"
+            return f"  `{key:<13}`<ok>{help_msg}`{command_msg}`<gold>"
         else:
-            return f"  {_key:<12} {_help}{command_msg}"
+            return f"  {key:<12} {_help}{command_msg}"
+
+    def get_help(self) -> str:
+        """Get all help message."""
+
+        msgs = ["These are short commands that can replace git operations:"]
 
-    def print_help(self) -> None:
-        """Print help message."""
-        print("These are short commands that can replace git operations:")
         for key in self.cmds.keys():
-            msg = self._generate_help_by_key(key)
-            get_console().echo(msg)
+            msg = self.generate_help_by_key(key)
+            msgs.append(msg)
+
+        return "\n".join(msgs)
 
-    def print_help_by_type(self, command_type: str) -> None:
+    def get_help_by_type(self, t: str) -> str:
         """Print a part of help message.
 
         Print the help information of the corresponding part according to the
         incoming command type string. If there is no print error prompt for the
         type.
 
         Args:
             command_type (str): A command type of `TYPE`.
         """
 
         # Process received type.
-        command_type = command_type.capitalize().strip()
+        t = t.capitalize().strip()
 
         # Checking the type whether right.
-        if command_type not in CommandType.__members__:
-            get_console().echo(
-                "`There is no such type.`<error>\n"
-                "Please use `git --types`<ok> to view the supported types."
-            )
+        if t not in GitCommandType.__members__:
+            predicted_type = similar_command(t, GitCommandType.__members__.keys())
+            if self.prompt and confirm(
+                f":TIPS: The wanted type is `{predicted_type}`?[y/n]:"
+            ):
+                return self.get_help_by_type(predicted_type)
 
-            if self.use_recommend:
-                predicted_type = similar_command(
-                    command_type, CommandType.__members__.keys()
+            else:
+                return (
+                    "`There is no such type.`<error>\n"
+                    "Please use `--types`<ok> to view the supported types."
                 )
-                if confirm(
-                    get_console().render_str(
-                        f":thinking: The wanted type is `{predicted_type}`<ok> ?[y/n]:"
-                    )
-                ):
-                    self.print_help_by_type(predicted_type)
-            return None
 
-        # Print help.
-        print("These are the orders of {0}".format(command_type))
+        # Get help.
+        msgs = ["These are the orders of {0}".format(t)]
+
         for k, v in self.cmds.items():
-            belong = v.get("belong", CommandType.Extra)
+            belong = v.get("belong", GitCommandType.Extra)
             # Prevent the `belong` attribute from being set in the custom command.
-            if isinstance(belong, CommandType) and belong.value == command_type:
-                msg = self._generate_help_by_key(k)
-                get_console().echo(msg)
+            if isinstance(belong, GitCommandType) and belong.value == t:
+                msg = self.generate_help_by_key(k)
+                msgs.append(msg)
+
+        return "\n".join(msgs)
 
     @classmethod
-    def print_types(cls) -> None:
+    def get_types(cls) -> str:
         """Print all command types with random color."""
-        res = []
+        msgs = []
 
-        for member in CommandType:
+        for member in GitCommandType:
             color_str = "#{:02X}{:02X}{:02X}".format(
                 random.randint(70, 255),
                 random.randint(70, 255),
                 random.randint(70, 255),
             )
 
-            res.append(f"`{member.value}`<{color_str}>")
+            msgs.append(f"`{member.value}`<{color_str}>")
 
-        get_console().echo(" ".join(res))
+        return " ".join(msgs)
```

### Comparing `pigit-1.6.1/pigit/gitlib/shortcmds.py` & `pigit-1.7.0/pigit/git/_cmds.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,32 @@
 short command.
 
 [belong] is the type of command. The default is `Extra`.
 [command] is the execution content of the short command. It supports (method, command
           string). The default is command.
 [help] is help information, optional.
 [has_arguments] indicates whether the short command receives parameters. The default is False.
+
+Example:
+    "b": {
+        "belong": CommandType.Branch,
+        "command": "git branch",
+        "help": "lists, creates, renames, and deletes branches.",
+        "has_arguments": True,
+    }
 """
 
 import enum
+from typing import Callable, Dict, List, Union, Tuple, TypedDict
+
 from ._cmd_func import *
 
 
 @enum.unique
-class CommandType(enum.Enum):
+class GitCommandType(enum.Enum):
     Branch = "Branch"
     Commit = "Commit"
     Conflict = "Conflict"
     Fetch = "Fetch"
     Index = "Index"
     Log = "Log"
     Merge = "Merge"
@@ -31,632 +41,642 @@
     Tag = "Tag"
     WorkingTree = "Working tree"
     Submodule = "Submodule"
     Setting = "Setting"
     Extra = "Extra"  # default
 
 
+GitCommand = Union[str, Callable[[Union[List, Tuple]], None]]
+
+
+class GitProxyOptions(TypedDict):
+    belong: GitCommandType
+    command: GitCommand
+    help: str
+    has_arguments: bool
+
+
 # The custom git output format string.
 #   git ... --pretty={0}.format(GIT_PRINT_FORMAT)
 _GIT_PRINT_FORMAT = (
     'format:"%C(bold yellow)commit %H%C(auto)%d%n'
     "%C(bold)Author: %C(blue)%an <%ae> %C(reset)%C(cyan)%ai (%ar)%n"
     '%C(bold)Commit: %C(blue)%cn <%ce> %C(reset)%C(cyan)%ci (%cr)%C(reset)%n%+B"'
 )
 
 
-GIT_CMDS = {
+Git_Proxy_Cmds: Dict[str, GitProxyOptions] = {
     # Branch
     "b": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git branch",
         "help": "lists, creates, renames, and deletes branches.",
         "has_arguments": True,
     },
     "bc": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git checkout -b",
         "help": "creates a new branch.",
         "has_arguments": True,
     },
     "bl": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git branch -vv",
         "help": "lists branches and their commits.",
     },
     "bL": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git branch --all -vv",
         "help": "lists local and remote branches and their commits.",
     },
     "bs": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git show-branch",
         "help": "lists branches and their commits with ancestry graphs.",
     },
     "bS": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git show-branch --all",
         "help": "lists local and remote branches and their commits with "
         "ancestry graphs.",
     },
     "bm": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git branch --move",
         "help": "renames a branch.",
         "has_arguments": True,
     },
     "bM": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git branch --move --force",
         "help": "renames a branch even if the new branch name already exists.",
         "has_arguments": True,
     },
     "bd": {
-        "belong": CommandType.Branch,
+        "belong": GitCommandType.Branch,
         "command": "git branch -d",
         "help": "delete a local branch by name.",
         "has_arguments": True,
     },
     # Commit
     "c": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git commit --verbose",
         "help": "records changes to the repository.",
     },
     "ca": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git commit --verbose --all",
         "help": "commits all modified and deleted files.",
     },
     "cA": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git commit --verbose --patch",
         "help": "commits all modified and deleted files interactively",
     },
     "cm": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git commit --verbose --message",
         "help": "commits with the given message.",
     },
     "co": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git checkout",
         "help": "checks out a branch or paths to the working tree.",
         "has_arguments": True,
     },
     "cO": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git checkout --patch",
         "help": "checks out hunks from the index or the tree interactively.",
         "has_arguments": True,
     },
     "cf": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git commit --amend --reuse-message HEAD ",
         "help": "amends the tip of the current branch reusing the same log "
         "message as HEAD.",
     },
     "cF": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git commit --verbose --amend",
         "help": "amends the tip of the current branch.",
     },
     "cr": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": "git revert",
         "help": "reverts existing commits by reverting patches and recording "
         "new commits.",
         "has_arguments": True,
     },
     "cR": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": 'git reset "HEAD^"',
         "help": "removes the HEAD commit.",
     },
     "cs": {
-        "belong": CommandType.Commit,
+        "belong": GitCommandType.Commit,
         "command": f"git show --pretty={_GIT_PRINT_FORMAT}",
         "help": "shows one or more objects (blobs, trees, tags and commits).",
         "has_arguments": True,
     },
     # Conflict(C)
     "Cl": {
-        "belong": CommandType.Conflict,
+        "belong": GitCommandType.Conflict,
         "command": "git --no-pager diff --diff-filter=U --name-only",
         "help": "lists unmerged files.",
     },
     "Ca": {
-        "belong": CommandType.Conflict,
+        "belong": GitCommandType.Conflict,
         "command": "git add git --no-pager diff --diff-filter=U --name-only",
         "help": "adds unmerged file contents to the index.",
         "has_arguments": True,
     },
     "Ce": {
-        "belong": CommandType.Conflict,
+        "belong": GitCommandType.Conflict,
         "command": "git mergetool git --no-pager diff --diff-filter=U --name-only",
         "help": "executes merge-tool on all unmerged files.",
     },
     "Co": {
-        "belong": CommandType.Conflict,
+        "belong": GitCommandType.Conflict,
         "command": "git checkout --ours -- ",
         "help": "checks out our changes for unmerged paths.",
     },
     "CO": {
-        "belong": CommandType.Conflict,
+        "belong": GitCommandType.Conflict,
         "command": "git checkout --ours -- git --no-pager diff --diff-filter=U --name-only",
         "help": "checks out our changes for all unmerged paths.",
     },
     "Ct": {
-        "belong": CommandType.Conflict,
+        "belong": GitCommandType.Conflict,
         "command": "git checkout --theirs -- ",
         "help": "checks out their changes for unmerged paths.",
     },
     "CT": {
-        "belong": CommandType.Conflict,
+        "belong": GitCommandType.Conflict,
         "command": "git checkout --theirs -- git --no-pager diff --diff-filter=U --name-only",
         "help": "checks out their changes for all unmerged paths.",
     },
     # Fetch(f)
     "f": {
-        "belong": CommandType.Fetch,
+        "belong": GitCommandType.Fetch,
         "command": "git fetch",
         "help": "downloads objects and references from another repository.",
         "has_arguments": True,
     },
     "fc": {
-        "belong": CommandType.Fetch,
+        "belong": GitCommandType.Fetch,
         "command": "git clone",
         "help": "clones a repository into a new directory.",
         "has_arguments": True,
     },
     "fC": {
-        "belong": CommandType.Fetch,
+        "belong": GitCommandType.Fetch,
         "command": "git clone --depth=1",
         "help": "clones a repository into a new directory clearly(depth:1).",
         "has_arguments": True,
     },
     "fm": {
-        "belong": CommandType.Fetch,
+        "belong": GitCommandType.Fetch,
         "command": "git pull",
         "help": "fetches from and merges with another repository or local branch.",
         "has_arguments": True,
     },
     "fr": {
-        "belong": CommandType.Fetch,
+        "belong": GitCommandType.Fetch,
         "command": "git pull --rebase",
         "help": "fetches from and rebase on top of another repository or local branch.",
         "has_arguments": True,
     },
     "fu": {
-        "belong": CommandType.Fetch,
+        "belong": GitCommandType.Fetch,
         "command": "git fetch --all --prune && git merge --ff-only @{u}",
         "help": "removes un-existing remote-tracking references, fetches all remotes "
         "and merges.",
         "has_arguments": True,
     },
     "fb": {
-        "belong": CommandType.Fetch,
+        "belong": GitCommandType.Fetch,
         "command": fetch_remote_branch,
         "help": "fetch other branch to local as same name.",
     },
     # Index(i)
     "ia": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": add,
         "help": "adds file contents to the index(default: all files).",
         "has_arguments": True,
     },
     "iA": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git add --patch",
         "help": "adds file contents to the index interactively.",
         "has_arguments": True,
     },
     "iu": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git add --update",
         "help": "adds file contents to the index (updates only known files).",
         "has_arguments": True,
     },
     "id": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git diff --no-ext-diff --cached",
         "help": "displays changes between the index and a named commit (diff).",
         "has_arguments": True,
     },
     "iD": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git diff --no-ext-diff --cached --word-diff",
         "help": "displays changes between the index and a named commit (word diff).",
         "has_arguments": True,
     },
     "ir": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git reset",
         "help": "resets the current HEAD to the specified state.",
         "has_arguments": True,
     },
     "iR": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git reset --patch",
         "help": "resets the current index interactively.",
         "has_arguments": True,
     },
     "ix": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git rm --cached -r",
         "help": "removes files from the index (recursively).",
         "has_arguments": True,
     },
     "iX": {
-        "belong": CommandType.Index,
+        "belong": GitCommandType.Index,
         "command": "git rm --cached -rf",
         "help": "removes files from the index (recursively and forced).",
         "has_arguments": True,
     },
     # Log(l)
     "l": {
-        "belong": CommandType.Log,
+        "belong": GitCommandType.Log,
         "command": "git log --graph --all --decorate",
         "help": "display the log with good format.",
     },
     "l1": {
-        "belong": CommandType.Log,
+        "belong": GitCommandType.Log,
         "command": "git log --graph --all --decorate --oneline",
-        "help": "display the log with oneline.",
+        "help": "display the log with one-line.",
     },
     "ls": {
-        "belong": CommandType.Log,
+        "belong": GitCommandType.Log,
         "command": f"git log --topo-order --stat --pretty={_GIT_PRINT_FORMAT}",
         "help": "displays the stats log.",
     },
     "ld": {
-        "belong": CommandType.Log,
+        "belong": GitCommandType.Log,
         "command": f"git log --topo-order --stat --patch --pretty={_GIT_PRINT_FORMAT}",
         "help": "displays the diff log.",
     },
     "lv": {
-        "belong": CommandType.Log,
+        "belong": GitCommandType.Log,
         "command": f"git log --topo-order --show-signature --pretty={_GIT_PRINT_FORMAT}",
         "help": "displays the log, verifying the GPG signature of commits.",
     },
     "lc": {
-        "belong": CommandType.Log,
+        "belong": GitCommandType.Log,
         "command": "git shortlog --summary --numbered",
         "help": "displays the commit count for each contributor in descending order.",
     },
     "lr": {
-        "belong": CommandType.Log,
+        "belong": GitCommandType.Log,
         "command": "git reflog",
         "help": "manages reflog information.",
         "has_arguments": True,
     },
     # Merge(m)
     "m": {
-        "belong": CommandType.Merge,
+        "belong": GitCommandType.Merge,
         "command": "git merge",
         "help": "joins two or more development histories together.",
         "has_arguments": True,
     },
     "ma": {
-        "belong": CommandType.Merge,
+        "belong": GitCommandType.Merge,
         "command": "git merge --abort",
         "help": "aborts the conflict resolution, and reconstructs the pre-merge state.",
         "has_arguments": True,
     },
     "mC": {
-        "belong": CommandType.Merge,
+        "belong": GitCommandType.Merge,
         "command": "git merge --no-commit",
         "help": "performs the merge but does not commit.",
         "has_arguments": True,
     },
     "mF": {
-        "belong": CommandType.Merge,
+        "belong": GitCommandType.Merge,
         "command": "git merge --no-ff",
         "help": "creates a merge commit even if the merge could be resolved as a "
         "fast-forward.",
         "has_arguments": True,
     },
     "mS": {
-        "belong": CommandType.Merge,
+        "belong": GitCommandType.Merge,
         "command": "git merge -S",
         "help": "performs the merge and GPG-signs the resulting commit.",
         "has_arguments": True,
     },
     "mv": {
-        "belong": CommandType.Merge,
+        "belong": GitCommandType.Merge,
         "command": "git merge --verify-signatures",
         "help": "verifies the GPG signature of the tip commit of the side branch "
         "being merged.",
         "has_arguments": True,
     },
     "mt": {
-        "belong": CommandType.Merge,
+        "belong": GitCommandType.Merge,
         "command": "git mergetool",
         "help": "runs the merge conflict resolution tools to resolve conflicts.",
         "has_arguments": True,
     },
     # Push(p)
     "p": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": "git push",
         "help": "updates remote refs along with associated objects.",
         "has_arguments": True,
     },
     "pf": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": "git push --force-with-lease",
         "help": 'forces a push safely (with "lease").',
         "has_arguments": True,
     },
     "pF": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": "git push --force",
         "help": "forces a push.",
         "has_arguments": True,
     },
     "pa": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": "git push --all",
         "help": "pushes all branches.",
     },
     "pA": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": "git push --all && git push --tags",
         "help": "pushes all branches and tags.",
     },
     "pt": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": "git push --tags",
         "help": "pushes all tags.",
     },
     "pc": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": 'git push --set-upstream origin "$(git symbolic-ref -q --short HEAD 2> /dev/null)"',
         "help": "pushes the current branch and adds origin as an upstream reference for it.",
     },
     "pp": {
-        "belong": CommandType.Push,
+        "belong": GitCommandType.Push,
         "command": (
             'git pull origin "$(git symbolic-ref -q --short HEAD 2> /dev/null)" && '
             'git push origin "$(git symbolic-ref -q --short HEAD 2> /dev/null)"'
         ),
         "help": "pulls and pushes the current branch from origin to origin.",
     },
     # Remote(R)
     "R": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote",
         "help": "manages tracked repositories.",
         "has_arguments": True,
     },
     "Rl": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote --verbose",
         "help": "lists remote names and their URLs.",
         "has_arguments": True,
     },
     "Ra": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote add",
         "help": "adds a new remote.",
         "has_arguments": True,
     },
     "Rx": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote rm",
         "help": "removes a remote.",
         "has_arguments": True,
     },
     "Rm": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote rename",
         "help": "renames a remote.",
         "has_arguments": True,
     },
     "Ru": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote update",
         "help": "fetches remotes updates.",
         "has_arguments": True,
     },
     "Rp": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote prune",
         "help": "prunes all stale remote tracking branches.",
         "has_arguments": True,
     },
     "Rs": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote show",
         "help": "shows information about a given remote.",
         "has_arguments": True,
     },
     "RS": {
-        "belong": CommandType.Remote,
+        "belong": GitCommandType.Remote,
         "command": "git remote set-url",
         "help": "changes URLs for a remote.",
         "has_arguments": True,
     },
     # Stash(s)
     "s": {
-        "belong": CommandType.Stash,
+        "belong": GitCommandType.Stash,
         "command": "git stash",
         "help": "stashes the changes of the dirty working directory.",
         "has_arguments": True,
     },
     "sp": {
-        "belong": CommandType.Stash,
+        "belong": GitCommandType.Stash,
         "command": "git stash pop",
         "help": "removes and applies a single stashed state from the stash list.",
     },
     "sl": {
-        "belong": CommandType.Stash,
+        "belong": GitCommandType.Stash,
         "command": "git stash list",
         "help": "lists stashed states.",
     },
     "sd": {
-        "belong": CommandType.Stash,
+        "belong": GitCommandType.Stash,
         "command": "git stash show",
         "help": "display stash list.",
         "has_arguments": True,
     },
     "sD": {
-        "belong": CommandType.Stash,
+        "belong": GitCommandType.Stash,
         "command": "git stash show --patch --stat",
         "help": "display stash list with detail.",
         "has_arguments": True,
     },
     # Tag (t)
     "t": {
-        "belong": CommandType.Tag,
+        "belong": GitCommandType.Tag,
         "command": "git tag",
         "help": "creates, lists, deletes or verifies a tag object signed with GPG.",
         "has_arguments": True,
     },
     "ta": {
-        "belong": CommandType.Tag,
+        "belong": GitCommandType.Tag,
         "command": "git tag -a",
         "help": "create a new tag.",
         "has_arguments": True,
     },
     "tx": {
-        "belong": CommandType.Tag,
+        "belong": GitCommandType.Tag,
         "command": "git tag --delete",
         "help": "deletes tags with given names.",
         "has_arguments": True,
     },
     # Working tree(w)
     "ws": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git status --short",
         "help": "displays working-tree status in the short format.",
     },
     "wS": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git status",
         "help": "displays working-tree status.",
         "has_arguments": True,
     },
     "wd": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git diff --no-ext-diff",
         "help": "displays changes between the working tree and the index (diff).",
         "has_arguments": True,
     },
     "wD": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git diff --no-ext-diff --word-diff",
         "help": "displays changes between the working tree and the index (word diff).",
         "has_arguments": True,
     },
     "wr": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git reset --soft",
         "help": "resets the current HEAD to the specified state, does not touch the "
         "index nor the working tree.",
         "has_arguments": True,
     },
     "wR": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git reset --hard",
         "help": "resets the current HEAD, index and working tree to the specified state.",
         "has_arguments": True,
     },
     "wc": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git clean --dry-run",
         "help": "cleans untracked files from the working tree (dry-run).",
         "has_arguments": True,
     },
     "wC": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git clean -d --force",
         "help": "cleans untracked files from the working tree.",
         "has_arguments": True,
     },
     "wm": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git mv",
         "help": "moves or renames files.",
         "has_arguments": True,
     },
     "wM": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git mv -f",
         "help": "moves or renames files (forced).",
         "has_arguments": True,
     },
     "wx": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git rm -r",
         "help": "removes files from the working tree and from the index (recursively).",
         "has_arguments": True,
     },
     "wX": {
-        "belong": CommandType.WorkingTree,
+        "belong": GitCommandType.WorkingTree,
         "command": "git rm -rf",
         "help": "removes files from the working tree and from the index (recursively "
         "and forced).",
         "has_arguments": True,
     },
     # Submodule
     "Sc": {
-        "belong": CommandType.Submodule,
+        "belong": GitCommandType.Submodule,
         "command": "git clone --recursive",
         "help": "Clone a repository as a submodule.",
         "has_arguments": True,
     },
     "Si": {
-        "belong": CommandType.Submodule,
+        "belong": GitCommandType.Submodule,
         "command": "git submodule update --init --recursive",
         "help": "Pull the submodule for the first time.",
     },
     # For above git 1.8.2
     #   `git submodule update --recursive --remote`
     # For above git 1.7.3
     #   `git submodule update --recursive`
     #   `git pull --reccurse-submodules`
     "Su": {
-        "belong": CommandType.Submodule,
+        "belong": GitCommandType.Submodule,
         "command": "git submodule update --recursive --remote",
         "help": "Update git submodule.",
     },
     "Sd": {
-        "belong": CommandType.Submodule,
+        "belong": GitCommandType.Submodule,
         "command": "git rm --cached",
         "help": "Remove submodule from repository.",
         "has_arguments": True,
     },
     "SD": {
-        "belong": CommandType.Submodule,
+        "belong": GitCommandType.Submodule,
         "command": "git submodule deinit",
         "help": "Inverse initialization submodule, clear the dir.",
         "has_arguments": True,
     },
     # Setting
     "savepd": {
-        "belong": CommandType.Setting,
+        "belong": GitCommandType.Setting,
         "command": "git config credential.helper store",
         "help": "Remember your account and password.",
         "has_arguments": True,
     },
     "ue": {
-        "belong": CommandType.Setting,
+        "belong": GitCommandType.Setting,
         "command": set_email_and_username,
         "help": "set email and username interactively.",
         "has_arguments": True,
     },
     "user": {
-        "belong": CommandType.Setting,
+        "belong": GitCommandType.Setting,
         "command": "git config user.name",
         "help": "set username.",
         "has_arguments": True,
     },
     "email": {
-        "belong": CommandType.Setting,
+        "belong": GitCommandType.Setting,
         "command": "git config user.email",
         "help": "set user email.",
         "has_arguments": True,
     },
 }  # type: dict[str,dict]
```

### Comparing `pigit-1.6.1/pigit/log.py` & `pigit-1.7.0/pigit/ext/log.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 
-from typing import Optional
 import os
 import logging
 import logging.handlers
+from typing import Dict, Optional
 
 
 FMT_NORMAL = logging.Formatter(
     fmt="%(asctime)s %(levelname).4s %(message)s", datefmt="%H:%M:%S"
 )
 
 FMT_DEBUG = logging.Formatter(
@@ -42,7 +42,24 @@
             raise SystemExit(1) from None
 
     log_handle.setFormatter(formatter)
     log_handle.setLevel(log_level)
 
     root_logger.addHandler(log_handle)
     root_logger.setLevel(0)
+
+
+# cache logger, avoid creating loggers with the same name repeatedly.
+_logger_cache: Dict[str, "logging.Logger"] = {}
+
+
+def logger(name: Optional[str] = None) -> "logging.Logger":
+    # not cache no name logger
+    if name is None:
+        return logging.getLogger()
+
+    cache_logger = _logger_cache.get(name)
+    if cache_logger is not None:
+        return cache_logger
+
+    new_logger = _logger_cache[name] = logging.getLogger(name)
+    return new_logger
```

### Comparing `pigit-1.6.1/pigit/shellmode.py` & `pigit-1.7.0/pigit/shellmode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from typing import TYPE_CHECKING, Callable, List, Optional, IO
-import os, cmd
+import os
+import cmd
 import functools
 
 from plenty import get_console
 
 if TYPE_CHECKING:
-    from pigit.gitlib.processor import ShortGitter
+    from pigit.git.proxy import GitProxy
 
 
 class PigitShell(cmd.Cmd):
     intro: str = get_console().render_str(
         "b`Welcome come PIGIT shell.`<khaki>\n"
         "`You can use short commands directly. Input '?' to get help.`<khaki>\n"
     )
     prompt: str = "(pigit)> "
 
     def __init__(
         self,
-        short_gitter: "ShortGitter",
+        short_giter: "GitProxy",
         *,
         completekey: str = "tab",
         stdin: Optional[IO[str]] = None,
         stdout: Optional[IO[str]] = None,
     ) -> None:
         super().__init__(completekey, stdin, stdout)
 
         self.console = get_console()
-        self.short_gitter = short_gitter
+        self.short_giter = short_giter
 
-        for key, values in short_gitter.cmds.items():
+        for key, values in short_giter.cmds.items():
             func_name = f"do_{key}"
 
-            self.set_instance_method(self.make_fun(key, values.get("help")), func_name)
+            self.set_instance_method(
+                self.make_fun(key, values.get("help", "")), func_name
+            )
 
     # =================
     # cmd tools method
     # =================
     def make_fun(self, key: str, doc: str):
         _key = key
 
         def func(args: str):
-            self.short_gitter.process_command(_key, args.split())
+            _, msg = self.short_giter.process_command(_key, args.split())
+            get_console().echo(msg)
 
         func.__doc__ = doc
 
         return func
 
     @classmethod
     def set_instance_method(cls, func: Callable, func_name: Optional[str] = None):
@@ -56,37 +60,36 @@
             func_name = func.__name__
 
         setattr(cls, func_name, dummy)
 
     # ==================
     # print help method
     # ==================
-    def default(self, line):
+    def default(self, line: str):
         """Called on an input line when the command prefix is not recognized.
 
         If this method is not overridden, it prints an error message and
         returns.
-
         """
         self.stdout.write(
             get_console().render_str(
                 "`pigit shell: Invalid command '{0}', please select from`<error> "
                 "`[shell, quit] or git short command.`<error>\n".format(line.split()[0])
             )
         )
 
     def do_help(self, arg: str):
         """List available commands with "help" or detailed help with "help cmd"."""
         if not arg:
             return super().do_help(arg)
 
         args: List[str] = arg.split()
-        for a in args:
-            self.stdout.write(f"{a}: ")
-            super().do_help(a)
+        for value in args:
+            self.stdout.write(f"{value}: ")
+            super().do_help(value)
 
     # ================
     # support command
     # ================
     def do_shell(self, args: str):
         """Run a shell command.
 
@@ -95,8 +98,8 @@
         """
         os.system(args)
 
     do_sh = do_shell
 
     def do_all(self, args: str):
         """Show all short git cmds help."""
-        self.short_gitter.print_help()
+        get_console().echo(self.short_giter.get_help())
```

### Comparing `pigit-1.6.1/pigit/tui/__init__.py` & `pigit-1.7.0/pigit/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `pigit-1.6.1/pigit/tui/input.py` & `pigit-1.7.0/pigit/tui/input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,173 +1,116 @@
 # -*- coding:utf-8 -*-
-import os, sys
-import tty, termios, select, fcntl
+import contextlib
+import fcntl
+import os
+import select
+import sys
+import termios
+import tty
 import signal
 from subprocess import Popen, PIPE
+from typing import Callable, Dict, Final, List, Optional, Tuple, Union
 
 
 # ===========
 # Predefined
 # ===========
-ord2 = lambda x: x
 B = lambda x: x.encode("iso8859-1")  # noqa: E731
 
 # ==================
 # Terminal encoding
 # ==================
 _byte_encoding = None
 
 
-def set_byte_encoding(enc):
-    assert enc in ("utf8", "narrow", "wide")
+def set_byte_encoding(enc: str):
+    assert enc in {"utf8", "narrow", "wide"}
     global _byte_encoding
     _byte_encoding = enc
 
 
-def get_byte_encoding():
+def get_byte_encoding() -> str:
     return _byte_encoding
 
 
 def detect_encoding():
     # Try to determine if using a supported double-byte encoding
     import locale
 
     initial = locale.getlocale()
     try:
-        try:
+        with contextlib.suppress(locale.Error):
             locale.setlocale(locale.LC_ALL, "")
-        except locale.Error:
-            pass
         return locale.getlocale()[1] or ""
     except ValueError as e:
         # with invalid LANG value python will throw ValueError
         if e.args and e.args[0].startswith("unknown locale"):
             return ""
         else:
             raise
     finally:
-        try:
+        with contextlib.suppress(locale.Error):
             locale.setlocale(locale.LC_ALL, initial)
-        except locale.Error:
-            pass
 
 
 if "detected_encoding" not in locals():
     detected_encoding = detect_encoding()
 else:
     assert 0, "It worked!"
 
 _target_encoding = None
 _use_dec_special = True
 
 
-def set_encoding(encoding):
+def set_encoding(encoding: str):
     """
     Set the byte encoding to assume when processing strings and the
     encoding to use when converting unicode strings.
     """
     encoding = encoding.lower()
 
     global _target_encoding, _use_dec_special
 
-    if encoding in ("utf-8", "utf8", "utf"):
+    if encoding in {"utf-8", "utf8", "utf"}:
         set_byte_encoding("utf8")
-
         _use_dec_special = False
-    elif encoding in (
-        "euc-jp",  # JISX 0208 only
-        "euc-kr",
-        "euc-cn",
-        "euc-tw",  # CNS 11643 plain 1 only
-        "gb2312",
-        "gbk",
-        "big5",
-        "cn-gb",
-        "uhc"
-        # these shouldn't happen, should they?
-        ,
-        "eucjp",
-        "euckr",
-        "euccn",
-        "euctw",
-        "cncb",
-    ):
-        set_byte_encoding("wide")
 
-        _use_dec_special = True
     else:
         set_byte_encoding("narrow")
         _use_dec_special = True
 
     # if encoding is valid for conversion from unicode, remember it
     _target_encoding = "ascii"
-    try:
+    with contextlib.suppress(LookupError):
         if encoding:
-            u"".encode(encoding)
+            "".encode(encoding)
             _target_encoding = encoding
-    except LookupError:
-        pass
 
 
 # ==============
 # Util function
 # ==============
-def within_double_byte(text, line_start, pos):
-    """Return whether pos is within a double-byte encoded character.
-    text -- byte string in question
-    line_start -- offset of beginning of line (< pos)
-    pos -- offset in question
-    Return values:
-    0 -- not within dbe char, or double_byte_encoding == False
-    1 -- pos is on the 1st half of a dbe char
-    2 -- pos is on the 2nd half of a dbe char
-    """
-    assert isinstance(text, bytes)
-    v = ord2(text[pos])
-
-    if v >= 0x40 and v < 0x7F:
-        # might be second half of big5, uhc or gbk encoding
-        if pos == line_start:
-            return 0
-
-        if ord2(text[pos - 1]) >= 0x81:
-            if within_double_byte(text, line_start, pos - 1) == 1:
-                return 2
-        return 0
-
-    if v < 0x80:
-        return 0
-
-    i = pos - 1
-    while i >= line_start:
-        if ord2(text[i]) < 0x80:
-            break
-        i -= 1
-
-    if (pos - i) & 1:
-        return 1
-    return 2
-
-
 def is_mouse_event(ev):
     return type(ev) == tuple and len(ev) == 4 and ev[0].find("mouse") >= 0
 
 
 def is_mouse_press(ev):
     return ev.find("press") >= 0
 
 
 # =================
 ## Input sequences
 # =================
 class MoreInputRequired(Exception):
-    pass
+    """Exception of process input codes.
+    Throw this error to inform the caller that more input characters are needed.
+    """
 
 
-def escape_modifier(digit):
+def _escape_modifier(digit: int):
     mode = ord(digit) - ord("1")
     return (
         "shift " * (mode & 1)
         + "meta " * ((mode & 2) // 2)
         + "ctrl " * ((mode & 4) // 4)
     )
 
@@ -199,50 +142,50 @@
 
     ('[200~', 'begin paste'), ('[201~', 'end paste'),
 ] + [
     (prefix + letter, modifier + key)
     for prefix, modifier in zip('O[', ('meta ', 'shift '))
     for letter, key in zip('abcd', ('up', 'down', 'right', 'left'))
 ] + [
-    ("[" + digit + symbol, modifier + key)
+    (f"[{digit}{symbol}", modifier + key)
     for modifier, symbol in zip(('shift ', 'meta '), '$^')
     for digit, key in zip('235678',
         ('insert', 'delete', 'page up', 'page down', 'home', 'end'))
 ] + [
     ('O' + chr(ord('p')+n), str(n)) for n in range(10)
 ] + [
     # modified cursor keys + home, end, 5 -- [#X and [1;#X forms
-    (prefix+digit+letter, escape_modifier(digit) + key)
+    (prefix+digit+letter, _escape_modifier(digit) + key)
     for prefix in ("[", "[1;")
     for digit in "12345678"
     for letter,key in zip("ABCDEFGH",
         ('up','down','right','left','5','end','5','home'))
 ] + [
     # modified F1-F4 keys -- O#X form
-    ("O"+digit+letter, escape_modifier(digit) + key)
+    (f"O{digit}{letter}", _escape_modifier(digit) + key)
     for digit in "12345678"
     for letter,key in zip("PQRS",('f1','f2','f3','f4'))
 ] + [
     # modified F1-F13 keys -- [XX;#~ form
-    ("["+str(num)+";"+digit+"~", escape_modifier(digit) + key)
+    (f"[{num};{digit}~", _escape_modifier(digit) + key)
     for digit in "12345678"
     for num,key in zip(
         (3,5,6,11,12,13,14,15,17,18,19,20,21,23,24,25,26,28,29,31,32,33,34),
         ('delete', 'page up', 'page down',
         'f1','f2','f3','f4','f5','f6','f7','f8','f9','f10','f11',
         'f12','f13','f14','f15','f16','f17','f18','f19','f20'))
 ] + [
-    # mouse reporting (special handling done in KeyqueueTrie)
+    # mouse reporting (special handling done in KeyQueueTrie)
     ('[M', 'mouse'),
 
     # mouse reporting for SGR 1006
     ('[<', 'sgrmouse'),
 
     # report status response
-    ('[0n', 'status ok')
+    ('[0n', 'status ok'),
 ]
 # yapf: enable
 
 # This is added to button value to signal mouse release by curses_display
 # and raw_display when we know which button was released.  NON-STANDARD
 MOUSE_RELEASE_FLAG = 2048
 
@@ -256,76 +199,106 @@
 # triple release adds this times two.  NON-STANDARD
 MOUSE_MULTIPLE_CLICK_FLAG = 512
 
 # xterm adds this to the button value to signal a mouse drag event
 MOUSE_DRAG_FLAG = 32
 
 
-class KeyqueueTrie(object):
-    def __init__(self, sequences):
+class KeyQueueTrie:
+    def __init__(self, sequences: Dict):
         self.data = {}
         for s, result in sequences:
             assert type(result) != dict
             self.add(self.data, s, result)
 
-    def add(self, root, s, result):
+    def add(self, root: Dict, k: str, v: str) -> None:
+        """Add a pair of k-v mappings to the recursive mapping field.
+
+        Args:
+            root (Dict): The root dictionary.
+            k (str): The key.
+            v (str): The value.
+        """
         assert type(root) == dict, "trie conflict detected"
-        assert len(s) > 0, "trie conflict detected"
+        assert k != "", "trie conflict detected"
 
-        if ord(s[0]) in root:
-            return self.add(root[ord(s[0])], s[1:], result)
-        if len(s) > 1:
+        if ord(k[0]) in root:
+            return self.add(root[ord(k[0])], k[1:], v)
+        if len(k) > 1:
             d = {}
-            root[ord(s[0])] = d
-            return self.add(d, s[1:], result)
-        root[ord(s)] = result
+            root[ord(k[0])] = d
+            return self.add(d, k[1:], v)
+        root[ord(k)] = v
 
-    def get(self, keys, more_available):
-
-        result = self.get_recurse(self.data, keys, more_available)
+    def get(self, codes: List[int], more_available: bool):
+        result, remaining_codes = self.get_recurse(self.data, codes, more_available)
         if not result:
-            result = self.read_cursor_position(keys, more_available)
-        return result
+            result, remaining_codes = self.read_cursor_position(codes, more_available)
+        return result, remaining_codes
+
+    def get_recurse(
+        self, root: Union[Dict, str], codes: List[int], more_available: bool
+    ) -> Tuple[Optional[Union[str, Tuple]], List[int]]:
+        """Recursively get the result and remaining codes.
+
+        Args:
+            root: The root object.
+            codes (List[int]): The codes list.
+            more_available (bool): Indicates if more input is available.
 
-    def get_recurse(self, root, keys, more_available):
+        Returns:
+            Tuple[Optional[Union[str, Tuple]], List[int]]: The result and remaining codes.
+        """
         if type(root) != dict:
             if root == "mouse":
-                return self.read_mouse_info(keys, more_available)
+                return self.read_mouse_info(codes, more_available)
             elif root == "sgrmouse":
-                return self.read_sgrmouse_info(keys, more_available)
-            return (root, keys)
-        if not keys:
+                return self.read_sgrmouse_info(codes, more_available)
+            else:
+                return root, codes
+        if not codes:
             # get more keys
             if more_available:
                 raise MoreInputRequired()
-            return None
-        if keys[0] not in root:
-            return None
-        return self.get_recurse(root[keys[0]], keys[1:], more_available)
+            return None, codes
+        if codes[0] not in root:
+            return None, codes
+        return self.get_recurse(root[codes[0]], codes[1:], more_available)
+
+    def read_mouse_info(
+        self, codes: List[int], more_available: bool
+    ) -> Tuple[Optional[Tuple], List[int]]:
+        """Read mouse information after processing codes.
+
+        Args:
+            codes (List[int]): The codes list.
+            more_available (bool): Indicates if more input is available.
 
-    def read_mouse_info(self, keys, more_available):
-        if len(keys) < 3:
+        Returns:
+            Tuple[Optional[Tuple], List[int]]: The mouse information and remaining codes.
+        """
+        if len(codes) < 3:
             if more_available:
                 raise MoreInputRequired()
-            return None
+            return None, codes
 
-        b = keys[0] - 32
-        x, y = (keys[1] - 33) % 256, (keys[2] - 33) % 256  # supports 0-255
+        b = codes[0] - 32
+        x, y = (codes[1] - 33) % 256, (codes[2] - 33) % 256  # supports 0-255
 
         prefix = ""
         if b & 4:
-            prefix = prefix + "shift "
+            prefix += "shift "
         if b & 8:
-            prefix = prefix + "meta "
+            prefix += "meta "
         if b & 16:
-            prefix = prefix + "ctrl "
+            prefix += "ctrl "
         if (b & MOUSE_MULTIPLE_CLICK_MASK) >> 9 == 1:
-            prefix = prefix + "double "
+            prefix += "double "
         if (b & MOUSE_MULTIPLE_CLICK_MASK) >> 9 == 2:
-            prefix = prefix + "triple "
+            prefix += "triple "
 
         # 0->1, 1->2, 2->3, 64->4, 65->5
         button = ((b & 64) // 64 * 3) + (b & 3) + 1
 
         if b & 3 == 3:
             action = "release"
             button = 0
@@ -334,122 +307,133 @@
         elif b & MOUSE_DRAG_FLAG:
             action = "drag"
         elif b & MOUSE_MULTIPLE_CLICK_MASK:
             action = "click"
         else:
             action = "press"
 
-        return ((prefix + "mouse " + action, button, x, y), keys[3:])
+        return (f"{prefix}mouse {action}", button, x, y), codes[3:]
 
-    def read_sgrmouse_info(self, keys, more_available):
+    def read_sgrmouse_info(
+        self, codes: List[int], more_available: bool
+    ) -> Tuple[Optional[Tuple], List[int]]:
         # Helpful links:
         # https://stackoverflow.com/questions/5966903/how-to-get-mousemove-and-mouseclick-in-bash
         # http://invisible-island.net/xterm/ctlseqs/ctlseqs.pdf
 
-        if not keys:
+        if not codes:
             if more_available:
                 raise MoreInputRequired()
-            return None
+            return None, codes
 
         value = ""
         pos_m = 0
         found_m = False
-        for k in keys:
+        for k in codes:
             value = value + chr(k)
-            if (k is ord("M")) or (k is ord("m")):
+            if k in [ord("M"), ord("m")]:
                 found_m = True
                 break
             pos_m += 1
         if not found_m:
             if more_available:
                 raise MoreInputRequired()
-            return None
+            return None, codes
 
         (b, x, y) = value[:-1].split(";")
 
         # shift, meta, ctrl etc. is not communicated on my machine, so I
         # can't and won't be able to add support for it.
         # Double and triple clicks are not supported as well. They can be
         # implemented by using a timer. This timer can check if the last
         # registered click is below a certain threshold. This threshold
         # is normally set in the operating system itself, so setting one
-        # here will cause an inconsistent behaviour. I do not plan to use
+        # here will cause an inconsistent behavior. I do not plan to use
         # that feature, so I won't implement it.
 
         button = ((int(b) & 64) // 64 * 3) + (int(b) & 3) + 1
         x = int(x) - 1
         y = int(y) - 1
 
         if value[-1] == "M":
-            if int(b) & MOUSE_DRAG_FLAG:
-                action = "drag"
-            else:
-                action = "press"
+            action = "drag" if int(b) & MOUSE_DRAG_FLAG else "press"
         else:
             action = "release"
 
-        return (("mouse " + action, button, x, y), keys[pos_m + 1 :])
+        return (f"mouse {action}", button, x, y), codes[pos_m + 1 :]
 
-    def read_cursor_position(self, keys, more_available):
-        """
-        Interpret cursor position information being sent by the
-        user's terminal.  Returned as ('cursor position', x, y)
-        where (x, y) == (0, 0) is the top left of the screen.
+    def read_cursor_position(
+        self, codes: List[int], more_available: bool
+    ) -> Tuple[Optional[Tuple], List[int]]:
+        """Return the cursor position info.
+        Interpret cursor position information being sent by the user's terminal.
+        Returned as ('cursor position', x, y) where (x, y) == (0, 0) is the top
+        left of the screen.
+
+        Args:
+            codes (List[int]): The codes list.
+            more_available (bool): Indicates if more input is available.
+
+        Returns:
+            Tuple[Optional[Tuple], List[int]]: The cursor position information and remaining codes.
         """
-        if not keys:
+        # TODO: improve method.
+        default = (None, codes)
+
+        if not codes:
             if more_available:
                 raise MoreInputRequired()
-            return None
-        if keys[0] != ord("["):
-            return None
+            return default
+        if codes[0] != ord("["):
+            return default
         # read y value
         y = 0
         i = 1
-        for k in keys[i:]:
+        for k in codes[i:]:
             i += 1
             if k == ord(";"):
-                if not y:
-                    return None
-                else:
+                if y:
                     break
+                else:
+                    return default
             if k < ord("0") or k > ord("9"):
-                return None
+                return default
             if not y and k == ord("0"):
-                return None
+                return default
             y = y * 10 + k - ord("0")
-        if not keys[i:]:
+        if not codes[i:]:
             if more_available:
                 raise MoreInputRequired()
-            return None
+            return default
         # read x value
         x = 0
-        for k in keys[i:]:
+        for k in codes[i:]:
             i += 1
             if k == ord("R"):
-                return None if not x else (("cursor position", x - 1, y - 1), keys[i:])
+                return (("cursor position", x - 1, y - 1), codes[i:]) if x else None
             if k < ord("0") or k > ord("9"):
-                return None
+                return default
             if not x and k == ord("0"):
-                return None
+                return default
             x = x * 10 + k - ord("0")
-        if not keys[i:] and more_available:
+        if not codes[i:] and more_available:
             raise MoreInputRequired()
-        return None
+        return default
 
 
 # ===============================================
 # Build the input trie from input_sequences list
-input_trie = KeyqueueTrie(input_sequences)
+input_trie = KeyQueueTrie(input_sequences)
 # ===============================================
 
-ESC = "\x1b"
-MOUSE_TRACKING_ON = ESC + "[?1000h" + ESC + "[?1002h" + ESC + "[?1006h"
-MOUSE_TRACKING_OFF = ESC + "[?1006l" + ESC + "[?1002l" + ESC + "[?1000l"
+ESC: Final = "\x1b"
+MOUSE_TRACKING_ON: Final = f"{ESC}[?1000h{ESC}[?1002h{ESC}[?1006h"
+MOUSE_TRACKING_OFF: Final = f"{ESC}[?1006l{ESC}[?1002l{ESC}[?1000l"
 
-_keyconv = {
+_key_conv = {
     -1: None,
     8: "backspace",
     9: "tab",
     10: "enter",
     13: "enter",
     127: "backspace",
     # curses-only keycodes follow..  (XXX: are these used anymore?)
@@ -489,98 +473,119 @@
     339: "page up",
     343: "enter",  # on numpad
     350: "5",  # on numpad
     360: "end",
 }
 
 
-def process_keyqueue(codes, more_available):
+def process_one_code(code: int) -> Optional[str]:
+    """Process key code that less than 127 or code in `_key_conv`."""
+    # Using `_key_conv` as the first step. The code of 'enter' and 'ctrl+j' both 10.
+    if code in _key_conv:
+        return _key_conv[code]
+
+    # ctrl + a-z
+    if 0 < code < 27:
+        return f'ctrl {chr(ord("a") + code - 1)}'
+
+    # ctrl + [\]^
+    if 27 < code < 32:
+        return f'ctrl {chr(ord("A") + code - 1)}'
+
+    # (space)!"#$%&'()*+,-./ 0-9 :;<=>?@ A-Z [\]^_` a-z {|}~
+    return chr(code) if code >= 32 and code <= 126 else None
+
+
+def process_utf8_code(
+    codes: List[int], more_available: bool
+) -> Union[None, Tuple[List[str], List[int]]]:
+    """Process UTF-8 code."""
+    code = codes[0]
+    if not (127 < code < 256):
+        return None
+
+    if code & 0xE0 == 0xC0:  # 2-byte form
+        need_more = 1
+    elif code & 0xF0 == 0xE0:  # 3-byte form
+        need_more = 2
+    elif code & 0xF8 == 0xF0:  # 4-byte form
+        need_more = 3
+    else:
+        return ["<%d>" % code], codes[1:]
+
+    if len(codes) < need_more + 1:
+        if more_available:
+            raise MoreInputRequired()
+        else:
+            return ["<%d>" % code], codes[1:]
+
+    for i in range(need_more):
+        k = codes[i + 1]
+        if k > 256 or k & 0xC0 != 0x80:
+            return ["<%d>" % code], codes[1:]
+
+    s = bytes(codes[: need_more + 1])
+    try:
+        # Right process.
+        return [s.decode("utf-8")], codes[need_more + 1 :]
+    except UnicodeDecodeError:
+        return ["<%d>" % code], codes[1:]
+
+
+def process_key_queue(codes: List[int], more_available: bool) -> Tuple[List, List[int]]:
     """
     codes -- list of key codes
     more_available -- if True then raise MoreInputRequired when in the
         middle of a character sequence (escape/utf8/wide) and caller
         will attempt to send more key codes on the next call.
     returns (list of input, list of remaining key codes).
     """
-    code = codes[0]
-    if code >= 32 and code <= 126:
-        key = chr(code)
-        return [key], codes[1:]
-    if code in _keyconv:
-        return [_keyconv[code]], codes[1:]
-    if code > 0 and code < 27:
-        return ["ctrl %s" % chr(ord("a") + code - 1)], codes[1:]
-    if code > 27 and code < 32:
-        return ["ctrl %s" % chr(ord("A") + code - 1)], codes[1:]
+    if not codes:
+        return [], []
 
-    em = get_byte_encoding()
+    c = codes[0]
+    if s := process_one_code(c):
+        return [s], codes[1:]
 
-    if em == "wide" and code < 256 and within_double_byte(chr(code), 0, 0):
-        if not codes[1:]:
-            if more_available:
-                raise MoreInputRequired()
-        if codes[1:] and codes[1] < 256:
-            db = chr(code) + chr(codes[1])
-            if within_double_byte(db, 0, 1):
-                return [db], codes[2:]
-    if em == "utf8" and code > 127 and code < 256:
-        if code & 0xE0 == 0xC0:  # 2-byte form
-            need_more = 1
-        elif code & 0xF0 == 0xE0:  # 3-byte form
-            need_more = 2
-        elif code & 0xF8 == 0xF0:  # 4-byte form
-            need_more = 3
-        else:
-            return ["<%d>" % code], codes[1:]
-
-        for i in range(need_more):
-            if len(codes) - 1 <= i:
-                if more_available:
-                    raise MoreInputRequired()
-                else:
-                    return ["<%d>" % code], codes[1:]
-            k = codes[i + 1]
-            if k > 256 or k & 0xC0 != 0x80:
-                return ["<%d>" % code], codes[1:]
-
-        s = bytes(codes[: need_more + 1])
-
-        assert isinstance(s, bytes)
-        try:
-            return [s.decode("utf-8")], codes[need_more + 1 :]
-        except UnicodeDecodeError:
-            return ["<%d>" % code], codes[1:]
+    em = get_byte_encoding()
+    em_map = {
+        "utf8": process_utf8_code,
+    }
+    if em in em_map and (
+        result_and_remaining_codes := em_map[em](codes, more_available)
+    ):
+        return result_and_remaining_codes
 
-    if code > 127 and code < 256:
-        key = chr(code)
+    if c > 127 and c < 256:
+        key = chr(c)
         return [key], codes[1:]
-    if code != 27:
-        return ["<%d>" % code], codes[1:]
+    if c != 27:
+        return ["<%d>" % c], codes[1:]
 
-    result = input_trie.get(codes[1:], more_available)
+    # Try get from input trie
+    result, remaining_codes = input_trie.get(codes[1:], more_available)
 
     if result is not None:
-        result, remaining_codes = result
         return [result], remaining_codes
 
+    #  code -- ESC
     if codes[1:]:
         # Meta keys -- ESC+Key form
-        run, remaining_codes = process_keyqueue(codes[1:], more_available)
-        if is_mouse_event(run[0]):
-            return ["esc"] + run, remaining_codes
-        if run[0] == "esc" or run[0].find("meta ") >= 0:
-            return ["esc"] + run, remaining_codes
-        return ["meta " + run[0]] + run[1:], remaining_codes
+        result, remaining_codes = process_key_queue(codes[1:], more_available)
+        if is_mouse_event(result[0]):
+            return ["esc"] + result, remaining_codes
+        if result[0] == "esc" or result[0].find("meta ") >= 0:
+            return ["esc"] + result, remaining_codes
+        return [f"meta {result[0]}"] + result[1:], remaining_codes
 
     return ["esc"], codes[1:]
 
 
-class InputTerminal(object):
+class InputTerminal:
     def __init__(self):
-        super(InputTerminal, self).__init__()
         self._signal_keys_set = False
         self._old_signal_keys = None
 
     def tty_signal_keys(
         self, intr=None, quit=None, start=None, stop=None, susp=None, fileno=None
     ):
         """
@@ -644,46 +649,65 @@
         return skeys
 
 
 class PosixInput(InputTerminal):
     def __init__(self, input=sys.stdin, output=sys.stdout) -> None:
         super().__init__()
 
-        self._keyqueue = []
+        self._key_queue = []
         self.prev_input_resize = 0
-        self._partial_codes = None
-        self._input_timeout = None
+        self._partial_codes: Optional[List[int]] = None
+        self._input_timeout: Optional[float] = None
         self.set_input_timeouts()
-        self._next_timeout = None
-        self._resized = False
+        self._next_timeout: Optional[float] = None
+        self._resized: bool = False
 
         self.gpm_mev = None
         self.gpm_event_pending = False
         self._mouse_tracking_enabled = False
         self.signal_handler_setter = signal.signal
 
         # Our connections to the world
         self._term_output_file = output
         self._term_input_file = input
 
         # pipe for signalling external event loops about resize events
         self._resize_pipe_rd, self._resize_pipe_wr = os.pipe()
         fcntl.fcntl(self._resize_pipe_rd, fcntl.F_SETFL, os.O_NONBLOCK)
 
-    def _input_fileno(self):
+    def write(self, data) -> None:
+        """Write some data to the terminal.
+        You may wish to override this if you're using something other than
+        regular files for input and output.
         """
-        Returns the fileno of the input stream, or None if it doesn't have one.
-        A stream without a fileno can't participate in whatever.
+        self._term_output_file.write(data)
+
+    def flush(self) -> None:
+        """Flush the output buffer.
+        You may wish to override this if you're using something other than
+        regular files for input and output.
+        """
+        self._term_output_file.flush()
+
+    def _input_fileno(self) -> Optional[int]:
+        """Returns the fileno of the input stream.
+        Or None if it doesn't have one. A stream without a fileno can't
+        participate in whatever.
         """
         if hasattr(self._term_input_file, "fileno"):
             return self._term_input_file.fileno()
         else:
             return None
 
-    def set_input_timeouts(self, max_wait=None, complete_wait=0.125, resize_wait=0.125):
+    def set_input_timeouts(
+        self,
+        max_wait: Optional[float] = None,
+        complete_wait: float = 0.125,
+        resize_wait: float = 0.125,
+    ):
         """
         Set the get_input timeout values.  All values are in floating
         point numbers of seconds.
         max_wait -- amount of time in seconds to wait for input when
             there is no input pending, wait forever if None
         complete_wait -- amount of time in seconds to wait when
             get_input detects an incomplete escape sequence at the
@@ -694,15 +718,15 @@
             window resize operation
         """
         self.max_wait = max_wait
         if max_wait is not None:
             if self._next_timeout is None:
                 self._next_timeout = max_wait
             else:
-                self._next_timeout = min(self._next_timeout, self.max_wait)
+                self._next_timeout = min(self._next_timeout, max_wait)
         self.complete_wait = complete_wait
         self.resize_wait = resize_wait
 
     def _sigwinch_handler(self, signum, frame=None):
         """
         frame -- will always be None when the GLib event loop is being used.
         """
@@ -738,15 +762,15 @@
         enable = bool(enable)
         if enable == self._mouse_tracking_enabled:
             return
 
         self._mouse_tracking(enable)
         self._mouse_tracking_enabled = enable
 
-    def _mouse_tracking(self, enable):
+    def _mouse_tracking(self, enable: bool):
         if enable:
             self.write(MOUSE_TRACKING_ON)
             self._start_gpm_tracking()
         else:
             self.write(MOUSE_TRACKING_OFF)
             self._stop_gpm_tracking()
 
@@ -756,14 +780,16 @@
         if not os.environ.get("TERM", "").lower().startswith("linux"):
             return
         if not Popen:
             return
         m = Popen(
             ["/usr/bin/mev", "-e", "158"], stdin=PIPE, stdout=PIPE, close_fds=True
         )
+        if not m.stdout:
+            return
         fcntl.fcntl(m.stdout.fileno(), fcntl.F_SETFL, os.O_NONBLOCK)
         self.gpm_mev = m
 
     def _stop_gpm_tracking(self):
         if not self.gpm_mev:
             return
         os.kill(self.gpm_mev.pid, signal.SIGINT)
@@ -790,49 +816,53 @@
 
         fd = self._input_fileno()
         if fd is not None and os.isatty(fd):
             termios.tcsetattr(fd, termios.TCSADRAIN, self._old_termios_settings)
 
         self._mouse_tracking(False)
 
-    def _wait_for_input_ready(self, timeout):
-        ready = None
+    def _wait_input_ready(self, timeout: float) -> List[int]:
+        """Monitor input fileno until timeout, return a list of prepared input fileno."""
+        ready_fds: Optional[List] = None
+
         fd_list = []
         fd = self._input_fileno()
         if fd is not None:
             fd_list.append(fd)
         while True:
             try:
                 if timeout is None:
-                    ready, w, err = select.select(fd_list, [], fd_list)
+                    ready_fds, w, err = select.select(fd_list, [], fd_list)
                 else:
-                    ready, w, err = select.select(fd_list, [], fd_list, timeout)
+                    ready_fds, w, err = select.select(fd_list, [], fd_list, timeout)
                 break
             except select.error as e:
                 if e.args[0] != 4:
                     raise
                 if self._resized:
-                    ready = []
+                    ready_fds = []
                     break
-        return ready
+        return ready_fds
 
-    def _getch(self, timeout):
-        ready = self._wait_for_input_ready(timeout)
+    def _getch(self, timeout: float) -> int:
+        """Read one byte from fileno until timeout."""
+        ready = self._wait_input_ready(timeout)
         fd = self._input_fileno()
-        if fd is not None and fd in ready:
-            return ord(os.read(fd, 1))
-        return -1
 
-    def _getch_nodelay(self):
+        return ord(os.read(fd, 1)) if fd in ready else -1
+
+    def _getch_no_delay(self) -> int:
         return self._getch(0)
 
-    def _get_keyboard_codes(self):
-        codes = []
+    def _get_keyboard_codes(self) -> List[int]:
+        """Read byte code util there was no."""
+        codes: List[int] = []
+
         while True:
-            code = self._getch_nodelay()
+            code = self._getch_no_delay()
             if code < 0:
                 break
             codes.append(code)
         return codes
 
     def _encode_gpm_event(self):
         self.gpm_event_pending = False
@@ -862,15 +892,15 @@
         if m & 4:
             mod |= 16  # ctrl
 
         def append_button(b):
             b |= mod
             l.extend([27, ord("["), ord("M"), b + 32, x + 32, y + 32])
 
-        if ev == 20 or ev == 36 or ev == 52:  # press
+        if ev in {20, 36, 52}:  # press
             if b & 4 and last & 1 == 0:
                 append_button(0)
                 next |= 1
             if b & 2 and last & 2 == 0:
                 append_button(1)
                 next |= 2
             if b & 1 and last & 4 == 0:
@@ -931,93 +961,80 @@
 
         if self._partial_codes:
             codes = self._partial_codes + codes
             self._partial_codes = None
 
         # clean out the pipe used to signal external event loops
         # that a resize has occurred
-        try:
+        with contextlib.suppress(OSError):
             while True:
                 os.read(self._resize_pipe_rd, 1)
-        except OSError:
-            pass
 
         return codes
 
-    def parse_input(self, event_loop, callback, codes, wait_for_more=True):
+    def parse_input(
+        self, callback: Optional[Callable], codes: List[int], wait_for_more: bool = True
+    ) -> Optional[Tuple[List[str], List[int]]]:
         """
         Read any available input from get_available_raw_input, parses it into
         keys, and calls the given callback.
-        The current implementation tries to avoid any assumptions about what
-        the screen or event loop look like; it only deals with parsing keycodes
-        and setting a timeout when an incomplete one is detected.
-        `codes` should be a sequence of keycodes, i.e. bytes.  A bytearray is
+        `codes` should be a sequence of key-codes, i.e. bytes.  A bytearray is
         appropriate, but beware of using bytes, which only iterates as integers
         on Python 3.
         """
         # Note: event_loop may be None for 100% synchronous support, only used
         # by get_input.  Not documented because you shouldn't be doing it.
-        if self._input_timeout and event_loop:
-            event_loop.remove_alarm(self._input_timeout)
-            self._input_timeout = None
 
         original_codes = codes
         processed = []
         try:
             while codes:
-                run, codes = process_keyqueue(codes, wait_for_more)
+                # Here will update `codes`.
+                run, codes = process_key_queue(codes, wait_for_more)
                 processed.extend(run)
         except MoreInputRequired:
             # Set a timer to wait for the rest of the input; if it goes off
-            # without any new input having come in, use the partial input
-            k = len(original_codes) - len(codes)
-            processed_codes = original_codes[:k]
+            # without any new input having come in, use the partial input.
+            # sourcery skip: extract-method, inline-immediately-returned-variable
+            pos = len(original_codes) - len(codes)
+            processed_codes = original_codes[:pos]
             self._partial_codes = codes
 
-            def _parse_incomplete_input():
-                self._input_timeout = None
-                self._partial_codes = None
-                self.parse_input(event_loop, callback, codes, wait_for_more=False)
-
-            if event_loop:
-                self._input_timeout = event_loop.alarm(
-                    self.complete_wait, _parse_incomplete_input
-                )
-            else:
-                # When there is no `eventloop`, and turn on `wait more`.
-                run, codes = self.parse_input(
-                    event_loop, callback, codes, wait_for_more=False
-                )
-                processed.extend(run)
-                processed_codes = original_codes
+            # When there is no `event_loop`, and turn on `wait more`.
+            run, codes = self.parse_input(callback, codes, wait_for_more=False)
+            processed.extend(run)
+            processed_codes = original_codes
 
         else:
             processed_codes = original_codes
             self._partial_codes = None
 
+        # Check resize event.
         if self._resized:
             processed.append("window resize")
             self._resized = False
 
         if callback:
             callback(processed, processed_codes)
         else:
             # For get_input
             return processed, processed_codes
 
-    def get_input(self, raw_keys=False):
+    def get_input(
+        self, raw_keys: bool = False
+    ) -> Tuple[List[str], Optional[List[int]]]:
         """Return pending input as a list.
-        raw_keys -- return raw keycodes as well as translated versions
+        raw_keys -- return raw key-codes as well as translated versions
         This function will immediately return all the input since the
         last time it was called.  If there is no input pending it will
         wait before returning an empty list.  The wait time may be
         configured with the set_input_timeouts function.
         If raw_keys is False (default) this function will return a list
         of keys pressed.  If raw_keys is True this function will return
-        a ( keys pressed, raw keycodes ) tuple instead.
+        a ( keys pressed, raw key-codes ) tuple instead.
         Examples of keys returned:
         * ASCII printable characters:  " ", "a", "0", "A", "-", "/"
         * ASCII control characters:  "tab", "enter"
         * Escape sequences:  "up", "page up", "home", "insert", "f1"
         * Key combinations:  "shift f1", "meta a", "ctrl b"
         * Window events:  "window resize"
         When a narrow encoding is not enabled:
@@ -1032,24 +1049,22 @@
         * Mouse drag: ('mouse drag', 1, 16, 13),
                       ('mouse drag', 1, 17, 13),
                       ('ctrl mouse drag', 1, 18, 13)
         * Mouse button release: ('mouse release', 0, 18, 13),
                                 ('ctrl mouse release', 0, 17, 23)
         """
 
-        self._wait_for_input_ready(self._next_timeout)
-        keys, raw = self.parse_input(None, None, self.get_available_raw_input())
+        self._wait_input_ready(self._next_timeout)
+        keys, raw = self.parse_input(None, self.get_available_raw_input())
 
         # Avoid pegging CPU at 100% when slowly resizing
         if keys == ["window resize"] and self.prev_input_resize:
             while True:
-                self._wait_for_input_ready(self.resize_wait)
-                keys, raw2 = self.parse_input(
-                    None, None, self.get_available_raw_input()
-                )
+                self._wait_input_ready(self.resize_wait)
+                keys, raw2 = self.parse_input(None, self.get_available_raw_input())
                 raw += raw2
                 # if not keys:
                 #    keys, raw2 = self._get_input(
                 #        self.resize_wait)
                 #    raw += raw2
                 if keys != ["window resize"]:
                     break
@@ -1059,35 +1074,19 @@
         if keys == ["window resize"]:
             self.prev_input_resize = 2
         elif self.prev_input_resize == 2 and not keys:
             self.prev_input_resize = 1
         else:
             self.prev_input_resize = 0
 
-        if raw_keys:
-            return keys, raw
-        return keys
-
-    def write(self, data):
-        """Write some data to the terminal.
-        You may wish to override this if you're using something other than
-        regular files for input and output.
-        """
-        self._term_output_file.write(data)
-
-    def flush(self):
-        """Flush the output buffer.
-        You may wish to override this if you're using something other than
-        regular files for input and output.
-        """
-        self._term_output_file.flush()
+        return (keys, raw) if raw_keys else (keys, None)
 
 
 if __name__ == "__main__":
+    set_byte_encoding("utf8")
     handle = PosixInput()
-    # handle.set_input_timeouts(0.125)
     handle.start()
     handle.set_mouse_tracking()
     handle.set_input_timeouts(0.125)
     while True:
         res = handle.get_input(raw_keys=True)
         print(res)
```

### Comparing `pigit-1.6.1/pigit.egg-info/PKG-INFO` & `pigit-1.7.0/pigit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigit
-Version: 1.6.1
+Version: 1.7.0
 Summary: Simple terminal tool of Git.
 Home-page: https://github.com/zlj-zz/pigit.git
 Author: Zachary Zhang
 Author-email: zlj19971222@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: plenty==1.0.2
 
 # PIGIT
 
 ![Python 3](https://img.shields.io/badge/Python-v3.8%5E-green?logo=python)
 [![pypi_version](https://img.shields.io/pypi/v/pigit?label=pypi)](https://pypi.org/project/pigit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -32,52 +33,56 @@
 ## Usage
 
 If you want to use it, you must first know what it can do.
 
 The command of `pigit -h` or `pigit --help` to get the help message with usage. Like this:
 
 ```bash
-usage: pigit [-h] [-v] [-r] [-f] [-i] [-c [PATH]] [-C] [--create-ignore TYPE]
-             [--create-config]
-             {cmd,repo} ...
+usage: pigit [-h] [-i] [-f] [-r] [-v] [-c [PATH]] [--create-ignore TYPE]
+             [--complete [SHELL]] [--create-config]
+             {cmd,repo,open} ...
 
 Pigit TUI is called automatically if no parameters are followed.
 
+
 positional arguments:
-  {cmd,repo}
+  {cmd,repo,open}
     cmd                 git short command.
-    repo                repo options.
+    repo                repos options.
     open                open remote repository in web browser.
 
-optional arguments:
+
+options:
   -h, --help            show this help message and exit
-  -v, --version         Show version and exit.
-  -r, --report          Report the pigit desc and exit.
-  -f, --config          Display the config of current git repository and exit.
   -i, --information     Show some information about the current git repository.
+  -f, --config          Display the config of current git repository and exit.
+  -r, --report          Report the pigit desc and exit.
+  -v, --version         Show version and exit.
+
 
 tools arguments:
   Auxiliary type commands.
 
   -c [PATH], --count [PATH]
-                        Count the number of codes and output them in tabular form.A given path can be
-                        accepted, and the default is the current directory.
-  -C, --complete        Add shell prompt script and exit.(Supported bash, zsh, fish)
-  --create-ignore TYPE  Create a demo .gitignore file. Need one argument, support: [android, c++, cpp, c,
-                        dart, elisp, gitbook, go, java, kotlin, lua, maven, node, python, qt, r, ros, ruby,
-                        rust, sass, swift, unity]
-  --create-config       Create a pre-configured file of PIGIT.(If a profile exists, the values available in it
-                        are used)
+                        Count the number of codes and output them in tabular form.
+                        A given path can be accepted, and the default is the
+                        current directory.
+  --create-ignore TYPE  Create a demo .gitignore file. Need one argument, the type
+                        of gitignore.
+  --complete [SHELL]    Add shell prompt script and exit. (Supported bash, zsh,
+                        fish)
+  --create-config       Create a pre-configured file of PIGIT.(If a profile
+                        exists, the values available in it are used)
 ```
 
 ### `cmd`
 
 The command of `cmd` support some short sub-command to replace the long git original command.
 
-![demo display](./docs//demo.gif)
+![demo display](./docs/resources/demo.gif)
 
 Use `pigit cmd -s` to check what short command it supported, it will display the corresponding help information and the git original command, like this:
 
 ```
 These are short commands that can replace git operations:
     b        lists, creates, renames, and deletes branches.
              git branch
@@ -100,27 +105,50 @@
 ......
 ```
 
 ### `repo`
 
 The command of `repo` support operate multiple repos at the same time.
 
-![demo display](./docs/demo_repo_1.png)
-![demo display](./docs/demo_repo_2.png)
-![demo display](./docs/demo_repo_3.png)
+![demo display](./docs/resources/demo_repo_1.png)
+![demo display](./docs/resources/demo_repo_2.png)
+![demo display](./docs/resources/demo_repo_3.png)
 
 Use `pigit repo -h` to get more help.
 
+```
+usage: pigit
+
+ repo [-h] {add,rm,rename,ll,clear,cd,fetch,pull,push} ...
+
+
+positional arguments:
+  {add,rm,rename,ll,clear,cd,fetch,pull,push}
+    add                 add repo(s).
+    rm                  remove repo(s).
+    rename              rename a repo.
+    ll                  display summary of all repos.
+    clear               clear the all repos.
+    cd                  jump to a repo dir.
+    fetch               fetch remote update for repo(s).
+    pull                pull remote updates for repo(s).
+    push                push the local updates for repo(s).
+
+
+options:
+  -h, --help            show this help message and exit
+```
+
 ### Interaction
 
 Even if you can use short commands instead of long commands of git, there are still some cases where simple commands can be very bad. For example: `git add a/b/1.txt b/c/1.txt c/d/1.txt`.
 
 Therefore, we need a TUI to help us, so Pigit provides a simple command-line interactive TUI. When you use `pigit` without following any parameters, you will enter it.
 
-![interaction demo](./docs/demo_interaction.gif)
+![interaction demo](./docs/resources/demo_interaction.gif)
 
 And in the interaction mode, you can use `?` or `h` to see the help message.
 
 ## Installation
 
 ### Pip
 
@@ -134,52 +162,81 @@
 git clone https://github.com/zlj-zz/pigit.git --depth=1
 cd pigit
 make install
 # or
 python setup.py install  # On windows
 ```
 
+## Completion
+
+Provides a friendly command-line completion capability, injecting completion through the following methods.
+
+Write it to your shell configuration file：
+
+```sh
+# ~/.zshrc
+
+eval "$(pigit --complete zsh)"
+```
+
+Currently supports `bash`, `zsh` and `fish`.
+
+If no shell is specified, it will try to automatically detect what shell you are using.
+
+```sh
+eval "$(pigit --complete)"
+```
+
 ## Alias
 
 Alias is good way to help you use _pigit_ faster . Open your shell profile and append:
 
 ```bash
 if type pigit >/dev/null 2>&1; then
     alias pg="pigit"
-    alias g="pigit cmd"
     alias gr="pigit repo"
 fi
 ```
 
-Then, you can use `pg` to call `pigit` and use `g` to call `pigit cmd`.
+Then, you can use `pg` to call `pigit`.
+
+**Windows**
+
+Check your *PowerShell* config, like this: `echo $profile`. Create it if the path not exist. Then open it, and input:
+
+```ps
+set-alias pg pigit
+```
+
+After completing the above preparations, restart your terminal. If it prompts that you cannot run the configuration, you can refer to the [official website address](https://learn.microsoft.com/zh-cn/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.4).
 
 ## Configuration
 
 You can use `pigit --create-config` to create a template configuration at **pigit** home path.
 
 On Linux or MacOS: `~/.config/pigit`
 
 On windows should be: `C:\\User\\<your username>`
 
 [here](./docs/pigit.conf) is a configuration template.
 
-| config key                  | type  | default                     | desc                                                                                                                        |
-| --------------------------- | ----- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
-| cmd_show_original           | bool  | True                        | Show original git command.                                                                                                  |
-| cmd_recommend               | bool  | True                        | Is it recommended to correct when entering wrong commands.                                                                  |
-| tui_help_showtime           | float | 1.5                         | Display time of help information in interactive mode.                                                                       |
-| counter_use_gitignore       | bool  | True                        | Whether to use the ignore configuration of the `.gitignore` file.                                                           |
-| counter_show_invalid        | bool  | False                       | Whether show files that cannot be counted.                                                                                  |
-| counter_show_icon           | bool  | True                        | Whether show files icons. Font support required, like: 'Nerd Font'.                                                         |
-| counter_format              | str   | table                       | Output format of statistical results. Supported: [table, simple]                                                            |
-| git_config_format           | str   | table                       | Git local config print format. Supported: [table, normal]                                                                   |
-| repo_info_include           | list  | ["remote", "branch", "log"] | Control which parts need to be displayed when viewing git repository information. Support: (path,remote,branch,log,summary) |
-| repo_auto_append            | bool  | False                       | Whether auto append path to repos.                                                                                          |
-| debug_open                  | bool  | False                       | Whether run PIGIT in debug mode.                                                                                            |
-| log_output                  | bool  | False                       | Whether output log in terminal.                                                                                             |
+| config key            | type  | default                     | desc                                                                                                                        |
+| --------------------- | ----- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
+| cmd_display           | bool  | True                        | Show original git command.                                                                                                  |
+| cmd_recommend         | bool  | True                        | Is it recommended to correct when entering wrong commands.                                                                  |
+| tui_help_showtime     | float | 1.5                         | Display time of help information in interactive mode.                                                                       |
+| counter_use_gitignore | bool  | True                        | Whether to use the ignore configuration of the `.gitignore` file.                                                           |
+| counter_show_invalid  | bool  | False                       | Whether show files that cannot be counted.                                                                                  |
+| counter_show_icon     | bool  | True                        | Whether show files icons. Font support required, like: 'Nerd Font'.                                                         |
+| counter_format        | str   | table                       | Output format of statistical results. Supported: [table, simple]                                                            |
+| git_config_format     | str   | table                       | Git local config print format. Supported: [table, normal]                                                                   |
+| repo_info_include     | list  | ["remote", "branch", "log"] | Control which parts need to be displayed when viewing git repository information. Support: (path,remote,branch,log,summary) |
+| repo_auto_append      | bool  | False                       | Whether auto append path to repos.                                                                                          |
+| log_debug             | bool  | False                       | Whether run PIGIT in debug mode.                                                                                            |
+| log_output            | bool  | False                       | Whether output log in terminal.                                                                                             |
 
 ## Extra cmds
 
 You can setting your custom cmds. It need create a `extra_cmds.py` file at the **pigit** home. And writing like this:
 
 ```python
 import os
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pigit-1.6.1/pigit.egg-info/SOURCES.txt` & `pigit-1.7.0/pigit.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 LICENSE
 README.md
 setup.py
 pigit/__init__.py
 pigit/__main__.py
-pigit/codecounter.py
+pigit/app.py
 pigit/config.py
+pigit/console_scripts.py
 pigit/const.py
 pigit/entry.py
 pigit/info.py
-pigit/interaction.py
-pigit/log.py
 pigit/shellmode.py
 pigit.egg-info/PKG-INFO
 pigit.egg-info/SOURCES.txt
 pigit.egg-info/dependency_links.txt
 pigit.egg-info/entry_points.txt
 pigit.egg-info/requires.txt
 pigit.egg-info/top_level.txt
 pigit/cmdparse/__init__.py
 pigit/cmdparse/parser.py
-pigit/cmdparse/shellcompletion/__init__.py
-pigit/cmdparse/shellcompletion/base.py
-pigit/cmdparse/shellcompletion/bash.py
-pigit/cmdparse/shellcompletion/fish.py
-pigit/cmdparse/shellcompletion/zsh.py
-pigit/common/__init__.py
-pigit/common/func.py
-pigit/common/singleton.py
-pigit/common/utils.py
-pigit/gitlib/__init__.py
-pigit/gitlib/_cmd_func.py
-pigit/gitlib/model.py
-pigit/gitlib/options.py
-pigit/gitlib/processor.py
-pigit/gitlib/shortcmds.py
-pigit/gitlib/ignore/__init__.py
-pigit/gitlib/ignore/template.py
+pigit/cmdparse/completion/__init__.py
+pigit/cmdparse/completion/base.py
+pigit/cmdparse/completion/bash.py
+pigit/cmdparse/completion/fish.py
+pigit/cmdparse/completion/zsh.py
+pigit/ext/__init__.py
+pigit/ext/executor.py
+pigit/ext/func.py
+pigit/ext/lcstat.py
+pigit/ext/log.py
+pigit/ext/singleton.py
+pigit/ext/utils.py
+pigit/git/__init__.py
+pigit/git/_cmd_func.py
+pigit/git/_cmds.py
+pigit/git/model.py
+pigit/git/proxy.py
+pigit/git/repo.py
+pigit/git/ignore/__init__.py
+pigit/git/ignore/template.py
 pigit/tui/__init__.py
+pigit/tui/components.py
 pigit/tui/console.py
 pigit/tui/event_loop.py
 pigit/tui/input.py
-pigit/tui/screen.py
-pigit/tui/widgets.py
+pigit/tui/utils.py
 tests/__init__.py
 tests/conftest.py
-tests/run.py
-tests/test_cmdparser.py
-tests/test_common.py
-tests/test_counter.py
-tests/test_gitlib.py
+tests/test_all_pigit.py
+tests/test_cmdparse.py
+tests/test_config.py
+tests/test_ext.py
+tests/test_ext_executor.py
+tests/test_ext_lcstat.py
+tests/test_git.py
+tests/test_git_cmd.py
+tests/test_git_ignore.py
 tests/test_info.py
-tests/test_pigit.py
-tests/test_tui.py
+tests/test_shell.py
+tests/test_tui_components.py
+tests/test_tui_console.py
+tests/test_tui_eventloop.py
+tests/test_tui_input.py
 tests/utils.py
```

### Comparing `pigit-1.6.1/setup.py` & `pigit-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,13 +61,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
     ],
     install_requires=['plenty==1.0.2'],
-    entry_points="""
-        [console_scripts]
-        pigit=pigit.entry:main
-    """,
+    entry_points={
+        "console_scripts": [
+            "pigit=pigit.console_scripts:main",
+            "g=pigit.console_scripts:g",
+        ]
+    },
     python_requires=">=3.8",
 )
```

### Comparing `pigit-1.6.1/tests/test_cmdparser.py` & `pigit-1.7.0/tests/test_cmdparse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-import pytest, os, copy
+import pytest
+import os
+import copy
 from pprint import pprint
-from .utils import analyze_it
+
 from .conftest import _PIGIT_PATH
+from .utils import analyze_it
 
+from pigit.git._cmds import Git_Proxy_Cmds
 from pigit.cmdparse.parser import command, Parser
-from pigit.cmdparse.shellcompletion.base import ShellCompletion
-from pigit.cmdparse.shellcompletion import (
+from pigit.cmdparse.completion.base import ShellCompletion, ShellCompletionError
+from pigit.cmdparse.completion import (
     ZshCompletion,
     BashCompletion,
     FishCompletion,
     shell_complete,
     get_shell,
 )
-from pigit.gitlib.shortcmds import GIT_CMDS
+
 
 argparse_dict = {
     "prog": "pigit",
     "prefix_chars": "-",
     "description": "Pigit TUI is called automatically if no parameters are followed.",
     "args": {
         "-v --version": {
@@ -76,65 +80,71 @@
 }
 
 
 def test_generate_about_dict():
     parser = Parser.from_dict(argparse_dict)
     parser.print_help()
 
-    ShellCompletion._SHELL = ""
-    ShellCompletion._INJECT_PATH = ""
+    ShellCompletion.SHELL = ""
     args = parser.to_dict()["args"]
     pprint(ShellCompletion("", {})._parse(args))
 
 
 class TestCompletion:
-    real = True
-    prog = "pigit"
-    script_dir = os.path.join(_PIGIT_PATH, "docs")
-
-    if real:
-        from pigit.entry import pigit
-
-        complete_vars = pigit.to_dict()
-        complete_vars["args"]["cmd"]["args"].update(
-            {k: {"help": v["help"], "args": {}} for k, v in GIT_CMDS.items()}
-        )
-    else:
-        complete_vars = copy.deepcopy(argparse_dict)
-        cmd_temp = complete_vars["args"]["cmd"]["args"]
-        cmd_temp.update(
-            {k: {"help": v["help"], "args": {}} for k, v in GIT_CMDS.items()}
-        )
+    @classmethod
+    def setup_class(cls):
+        real = True
+
+        cls.prog = "pigit"
+        cls.script_dir = os.path.join(_PIGIT_PATH, "docs")
+
+        if real:
+            from pigit.entry import pigit
+
+            cls.complete_vars = pigit.to_dict()
+            cls.complete_vars["args"]["cmd"]["args"].update(
+                {k: {"help": v["help"], "args": {}} for k, v in Git_Proxy_Cmds.items()}
+            )
+        else:
+            cls.complete_vars = copy.deepcopy(argparse_dict)
+            cmd_temp = cls.complete_vars["args"]["cmd"]["args"]
+            cmd_temp.update(
+                {k: {"help": v["help"], "args": {}} for k, v in Git_Proxy_Cmds.items()}
+            )
 
-    def test_error_complete_vars(self):
+    def test_error(self):
+        # error complete_vars
         with pytest.raises(TypeError):
             BashCompletion("test", "xxx", ".")
 
-    def print(self, c):
-        print(c.prog_name)
-        print(c.script_name)
-        print(c.inject_path)
+        # error prog
+        with pytest.raises(ShellCompletionError):
+            BashCompletion(None, {}, ".")
+
+    def print(self, c: ShellCompletion):
+        assert c.prog_name == "pigit"
+
+        assert c.script_name == f"pigit_{c.SHELL}_comp"
 
         source = c.generate_resource()
-        print(source)
+        # print(source)
 
         c.write_completion(source)
 
-    @analyze_it
     def test_bash(self):
         c = BashCompletion(None, self.complete_vars, self.script_dir)
         self.print(c)
 
     @analyze_it
     def test_zsh(self):
-        c = ZshCompletion("pigit-dev", self.complete_vars, self.script_dir)
+        c = ZshCompletion("pigit", self.complete_vars, self.script_dir)
         self.print(c)
 
     def test_fish(self):
         c = FishCompletion(self.prog, self.complete_vars, self.script_dir)
         self.print(c)
 
     def test_get_shell(self):
-        print(get_shell())
+        assert get_shell() in ["bash", "zsh", "fish", ""]
 
     def test_action(self):
-        shell_complete(self.complete_vars, "bash", "xxx", ".", None, "./test.txt")
+        shell_complete(self.complete_vars, "bash", "xxx", ".", "./test.txt")
```

