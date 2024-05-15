# Comparing `tmp/botl-112.tar.gz` & `tmp/botl-120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botl-112.tar", last modified: Sun Apr 21 23:16:12 2024, max compression
+gzip compressed data, was "botl-120.tar", last modified: Wed May 15 03:21:44 2024, max compression
```

## Comparing `botl-112.tar` & `botl-120.tar`

### file list

```diff
@@ -1,54 +1,47 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 23:16:12.441841 botl-112/
--rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-21 23:16:12.441841 botl-112/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3438 2024-04-19 17:56:29.000000 botl-112/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 23:16:12.437841 botl-112/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     2261 2024-04-21 22:02:36.000000 botl-112/bin/botl
--rwxr-xr-x   0 bart      (1000) bart      (1000)     4654 2024-04-21 23:15:30.000000 botl-112/bin/botlbot
--rwxr-xr-x   0 bart      (1000) bart      (1000)     2384 2024-04-21 23:15:24.000000 botl-112/bin/botld
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 23:16:12.441841 botl-112/botl/
--rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-19 17:56:29.000000 botl-112/botl/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1364 2024-04-19 17:56:29.000000 botl-112/botl/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-20 23:22:28.000000 botl-112/botl/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1922 2024-04-19 17:56:29.000000 botl-112/botl/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-19 17:56:29.000000 botl-112/botl/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1089 2024-04-19 17:56:29.000000 botl-112/botl/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-19 17:56:29.000000 botl-112/botl/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1930 2024-04-19 17:56:29.000000 botl-112/botl/find.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1362 2024-04-19 17:56:29.000000 botl-112/botl/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 23:16:12.441841 botl-112/botl/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      493 2024-04-20 21:28:02.000000 botl-112/botl/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-04-19 17:56:29.000000 botl-112/botl/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      403 2024-04-19 17:56:29.000000 botl-112/botl/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-19 17:56:29.000000 botl-112/botl/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      819 2024-04-20 23:21:57.000000 botl-112/botl/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17621 2024-04-19 17:56:29.000000 botl-112/botl/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      776 2024-04-19 17:56:29.000000 botl-112/botl/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3552 2024-04-19 17:56:29.000000 botl-112/botl/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17081 2024-04-19 17:56:29.000000 botl-112/botl/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      240 2024-04-19 17:56:29.000000 botl-112/botl/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2400 2024-04-19 17:56:29.000000 botl-112/botl/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11001 2024-04-19 17:56:29.000000 botl-112/botl/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2761 2024-04-19 17:56:29.000000 botl-112/botl/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1184 2024-04-19 17:56:29.000000 botl-112/botl/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1038 2024-04-19 17:56:29.000000 botl-112/botl/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5130 2024-04-19 17:56:29.000000 botl-112/botl/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2933 2024-04-19 17:56:29.000000 botl-112/botl/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5799 2024-04-19 17:56:29.000000 botl-112/botl/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-19 17:56:29.000000 botl-112/botl/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-19 17:56:29.000000 botl-112/botl/parser.py
--rw-r--r--   0 bart      (1000) bart      (1000)      752 2024-04-19 17:56:29.000000 botl-112/botl/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-19 17:56:29.000000 botl-112/botl/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-20 21:23:50.000000 botl-112/botl/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-19 17:56:29.000000 botl-112/botl/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-19 17:56:29.000000 botl-112/botl/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-19 17:56:29.000000 botl-112/botl/utils.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1101 2024-04-19 17:56:29.000000 botl-112/botl/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 23:16:12.441841 botl-112/botl.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-21 23:16:12.000000 botl-112/botl.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      840 2024-04-21 23:16:12.000000 botl-112/botl.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-21 23:16:12.000000 botl-112/botl.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-21 23:16:12.000000 botl-112/botl.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-21 23:16:12.000000 botl-112/botl.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      857 2024-04-21 23:15:19.000000 botl-112/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-21 23:16:12.441841 botl-112/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      196 2024-04-19 17:56:29.000000 botl-112/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-15 03:21:44.501078 botl-120/
+-rw-r--r--   0 bart      (1000) bart      (1001)     3946 2024-05-15 03:21:44.501078 botl-120/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     3423 2024-05-15 03:13:13.000000 botl-120/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-15 03:21:44.497078 botl-120/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2492 2024-05-15 03:12:12.000000 botl-120/bin/botl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1938 2024-05-15 02:55:56.000000 botl-120/bin/botld
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-15 03:21:44.497078 botl-120/botl/
+-rw-r--r--   0 bart      (1000) bart      (1001)       73 2024-05-15 02:51:31.000000 botl-120/botl/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      795 2024-05-15 02:51:31.000000 botl-120/botl/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-15 02:51:31.000000 botl-120/botl/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-15 02:51:31.000000 botl-120/botl/disk.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1954 2024-05-15 02:51:31.000000 botl-120/botl/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-15 02:51:31.000000 botl-120/botl/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-15 02:51:31.000000 botl-120/botl/log.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-15 03:21:44.501078 botl-120/botl/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      527 2024-05-15 03:18:47.000000 botl-120/botl/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-15 02:53:41.000000 botl-120/botl/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-15 02:53:41.000000 botl-120/botl/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      372 2024-05-15 02:58:10.000000 botl-120/botl/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      726 2024-05-15 03:07:56.000000 botl-120/botl/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18833 2024-05-15 02:53:41.000000 botl-120/botl/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      694 2024-05-15 02:53:41.000000 botl-120/botl/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3542 2024-05-15 02:59:08.000000 botl-120/botl/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17332 2024-05-15 03:20:42.000000 botl-120/botl/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-15 02:53:41.000000 botl-120/botl/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2151 2024-05-15 02:53:41.000000 botl-120/botl/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    10762 2024-05-15 02:53:41.000000 botl-120/botl/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2786 2024-05-15 02:53:41.000000 botl-120/botl/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      465 2024-05-15 02:53:41.000000 botl-120/botl/modules/slg.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1123 2024-05-15 02:53:41.000000 botl-120/botl/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-15 02:53:41.000000 botl-120/botl/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5163 2024-05-15 02:53:41.000000 botl-120/botl/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2929 2024-05-15 02:53:41.000000 botl-120/botl/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5729 2024-05-15 02:49:21.000000 botl-120/botl/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-15 02:51:31.000000 botl-120/botl/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-15 02:51:31.000000 botl-120/botl/run.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-15 02:51:31.000000 botl-120/botl/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      333 2024-05-15 02:51:31.000000 botl-120/botl/utils.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-15 03:21:44.497078 botl-120/botl.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     3946 2024-05-15 03:21:44.000000 botl-120/botl.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      730 2024-05-15 03:21:44.000000 botl-120/botl.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-15 03:21:44.000000 botl-120/botl.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        5 2024-05-15 03:21:44.000000 botl-120/botl.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-15 03:21:44.000000 botl-120/botl.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)      838 2024-05-15 03:05:52.000000 botl-120/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-15 03:21:44.501078 botl-120/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      158 2024-05-15 03:05:15.000000 botl-120/setup.py
```

### Comparing `botl-112/PKG-INFO` & `botl-120/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 112
+Version: 120
 Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
@@ -21,26 +21,32 @@
     BOTL - bot library
 
 
 SYNOPSIS
 
 ::
 
-    botl <cmd> [key=val] [key==val]
-    botl [-a] [-c] [-d] [-h] [-v]
+    botl  <cmd> [key=val] [key==val]
+    botl  [-c] [-v]
+    botld 
 
     options are:
 
-    -a     load all modules
     -c     start console
-    -d     start daemon
-    -h     display help
     -v     use verbose
 
 
+INSTALL
+
+::
+
+    $ pipx install botl
+    $ pipx ensurepath
+
+
 DESCRIPTION
 
 ::
 
     BOTL contains all the python3 code to program objects in a functional
     way. It provides a base Object class that has only dunder methods, all
     methods are factored out into functions with the objects as the first
@@ -61,14 +67,41 @@
     BOTL has a demo bot, it can connect to IRC, fetch and display RSS
     feeds, take todo notes, keep a shopping list and log text. You can
     also copy/paste the service file and run it under systemd for 24/7
     presence in a IRC channel.
 
     BOTL is Public Domain.
 
+
+CONFIGURATION
+
+::
+
+    $ botl cfg 
+    channel=#botl commands=True nick=botl port=6667 server=localhost
+
+    irc
+
+    $ botl cfg server=<server>
+    $ botl cfg channel=<channel>
+    $ botl cfg nick=<nick>
+
+    sasl
+
+    $ botl pwd <nsvnick> <nspass>
+    $ botl cfg password=<frompwd>
+
+    rss
+
+    $ botl rss <url>
+    $ botl dpl <url> <item1,item2>
+    $ botl rem <url>
+    $ botl nme <url> <name>
+
+
 USAGE
 
 ::
 
     without any argument the program does nothing
 
     $ botl
@@ -96,39 +129,14 @@
     use -v for verbose
 
     $ botl -cv mod=irc
     BOTL started CV started Sat Dec 2 17:53:24 2023
     >
 
 
-CONFIGURATION
-
-::
-
-    $ botl cfg 
-    channel=#botl commands=True nick=botl port=6667 server=localhost
-
-    irc
-
-    $ botl cfg server=<server>
-    $ botl cfg channel=<channel>
-    $ botl cfg nick=<nick>
-
-    sasl
-
-    $ botl pwd <nsvnick> <nspass>
-    $ botl cfg password=<frompwd>
-
-    rss
-
-    $ botl rss <url>
-    $ botl dpl <url> <item1,item2>
-    $ botl rem <url>
-    $ botl nme <url> <name>
-
 COMMANDS
 
 ::
 
     cmd - commands
     cfg - irc configuration
     dlt - remove a user
```

### Comparing `botl-112/README.rst` & `botl-120/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,32 @@
     BOTL - bot library
 
 
 SYNOPSIS
 
 ::
 
-    botl <cmd> [key=val] [key==val]
-    botl [-a] [-c] [-d] [-h] [-v]
+    botl  <cmd> [key=val] [key==val]
+    botl  [-c] [-v]
+    botld 
 
     options are:
 
-    -a     load all modules
     -c     start console
-    -d     start daemon
-    -h     display help
     -v     use verbose
 
 
+INSTALL
+
+::
+
+    $ pipx install botl
+    $ pipx ensurepath
+
+
 DESCRIPTION
 
 ::
 
     BOTL contains all the python3 code to program objects in a functional
     way. It provides a base Object class that has only dunder methods, all
     methods are factored out into functions with the objects as the first
@@ -45,14 +51,41 @@
     BOTL has a demo bot, it can connect to IRC, fetch and display RSS
     feeds, take todo notes, keep a shopping list and log text. You can
     also copy/paste the service file and run it under systemd for 24/7
     presence in a IRC channel.
 
     BOTL is Public Domain.
 
+
+CONFIGURATION
+
+::
+
+    $ botl cfg 
+    channel=#botl commands=True nick=botl port=6667 server=localhost
+
+    irc
+
+    $ botl cfg server=<server>
+    $ botl cfg channel=<channel>
+    $ botl cfg nick=<nick>
+
+    sasl
+
+    $ botl pwd <nsvnick> <nspass>
+    $ botl cfg password=<frompwd>
+
+    rss
+
+    $ botl rss <url>
+    $ botl dpl <url> <item1,item2>
+    $ botl rem <url>
+    $ botl nme <url> <name>
+
+
 USAGE
 
 ::
 
     without any argument the program does nothing
 
     $ botl
@@ -80,39 +113,14 @@
     use -v for verbose
 
     $ botl -cv mod=irc
     BOTL started CV started Sat Dec 2 17:53:24 2023
     >
 
 
-CONFIGURATION
-
-::
-
-    $ botl cfg 
-    channel=#botl commands=True nick=botl port=6667 server=localhost
-
-    irc
-
-    $ botl cfg server=<server>
-    $ botl cfg channel=<channel>
-    $ botl cfg nick=<nick>
-
-    sasl
-
-    $ botl pwd <nsvnick> <nspass>
-    $ botl cfg password=<frompwd>
-
-    rss
-
-    $ botl rss <url>
-    $ botl dpl <url> <item1,item2>
-    $ botl rem <url>
-    $ botl nme <url> <name>
-
 COMMANDS
 
 ::
 
     cmd - commands
     cfg - irc configuration
     dlt - remove a user
```

### Comparing `botl-112/bin/botl` & `botl-120/bin/botl`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,115 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,E0401
-# ruff: noqa: E402
+# pylint: disable=C0413
 
 
-"""botl <cmd> [key=val] [key==val]
+"main"
 
-use the cmd command to see a list of comands."""
 
-
-"cli"
-
-
-import getpass
 import os
-import pwd
-import readline # pylint: disable=W0611
+import readline
 import sys
+import termios
 import time
 
 
 sys.path.insert(0, os.getcwd())
 
 
-from botl.client  import Client, cmnd, parse_cmd, spl
-from botl.command import Command
-from botl.default import Default
-from botl.errors  import debug, enable, errors
-from botl.runtime import broker
-from botl.workdir import Workdir, skel
+from botl.client  import Client, cmnd, parse
+from botl.disk    import Workdir, skel
+from botl.handler import Event
+from botl.log     import debug, enable
+from botl.object  import Default
+from botl.run     import broker, init, scan
+from botl.thread  import errors, setout
 
 
 from botl import modules
 
 
-if os.path.exists("mods"):
-    import mods
-else:
-    mods = None
-
-
 Cfg             = Default()
-Cfg.mod         = "cmd,mod"
+Cfg.dis         = ""
+Cfg.mod         = "cmd,err,log,mod,tdo,thr,tmr"
 Cfg.opts        = ""
-Cfg.name        = "botl"
-Cfg.version     = "111"
-Cfg.user        = getpass.getuser()
-Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.workdir = Cfg.wd
+Cfg.name        = __file__.rsplit(os.sep, maxsplit=1)[-1]
+Cfg.version     = "120"
+Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
+
 
+Workdir.workdir = Cfg.wdr
 
-dte = time.ctime(time.time()).replace("  ", " ")
 
+class Console(Client):
 
-class CLI(Client):
+    "Console"
 
     def __init__(self):
         Client.__init__(self)
         broker.add(self)
 
     def announce(self, txt):
-        pass
+        "disable announce."
+
+    def callback(self, evt):
+        "wait for callback."
+        Client.callback(self, evt)
+        evt.wait()
+
+    def poll(self):
+        "poll console and create event."
+        evt = Event()
+        evt.orig = object.__repr__(self)
+        evt.txt = input("> ")
+        evt.type = "command"
+        return evt
 
     def say(self, _channel, txt):
+        "print to console"
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
-def init(pkg, modstr):
-    mds = []
-    for modname in spl(modstr):
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        if "init" in dir(module):
-            module.init()
-            mds.append(module)
-    return mds
-
-
-def privileges(username):
-    pwnam = pwd.getpwnam(username)
-    os.setgid(pwnam.pw_gid)
-    os.setuid(pwnam.pw_uid)
-
-
-def ver(event):
-    event.reply(f"{Cfg.name.upper()} {Cfg.version}")
+def wrap(func):
+    "restore console."
+    old2 = None
+    try:
+        old2 = termios.tcgetattr(sys.stdin.fileno())
+    except termios.error:
+        pass
+    try:
+        func()
+    except (KeyboardInterrupt, EOFError):
+        print("")
+    finally:
+        if old2:
+            termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
 def main():
-    Command.add(ver)
-    enable(print)
-    privileges(Cfg.user)
+    "main"
+    setout(print)
+    parse(Cfg, " ".join(sys.argv[1:]))
     skel()
-    parse_cmd(Cfg, " ".join(sys.argv[1:]))
-    if 'a' in Cfg.opts:
-        Cfg.mod = ",".join(modules.__dir__())
-        if mods:
-            Cfg.mod += "," + ",".join(mods.__dir__())
+    Cfg.mod = ",".join(modules.__dir__())
     if "v" in Cfg.opts:
-        debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
-    if "h" in Cfg.opts:
-        print(__doc__)
-        return
-    return cmnd(Cfg.otxt, print)
+        enable(print)
+        dte = " ".join(time.ctime(time.time()).replace("  ", " ").split()[1:])
+        debug(f'{dte} {Cfg.name.upper()} {Cfg.opts.upper()} {Cfg.mod.upper()}')
+    scan(modules, Cfg.mod, Cfg.sets.dis)
+    if "c" in Cfg.opts:
+        init(modules, Cfg.mod, Cfg.sets.dis)
+        csl = Console()
+        csl.start()
+        while 1:
+            time.sleep(1.0)
+    elif Cfg.otxt:
+        cmnd(Cfg.otxt, print)
 
 
 if __name__ == "__main__":
-    main()
+    readline.redisplay()
+    wrap(main)
     errors()
```

### Comparing `botl-112/bin/botld` & `botl-120/bin/botld`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,E0611
-# ruff: noqa: E402
+# pylint: disable=C0413,W0212
 
 
 "daemon"
 
 
 import getpass
 import os
+import pathlib
 import pwd
-import readline # pylint: disable=W0611
 import sys
 import time
 
 
-from botl.client  import spl
-from botl.command import Command
-from botl.default import Default
-from botl.errors  import enable, errors
-from botl.object  import cdir
-from botl.workdir import Workdir, skel
+from botl.disk   import Workdir, skel
+from botl.object import Default
+from botl.run    import init, scan
+from botl.thread import errors
+
+
+from botl import modules
 
 
 Cfg             = Default()
-Cfg.mod         = "cmd,irc,mod,rss"
-Cfg.opts        = ""
+Cfg.dis         = ""
 Cfg.name        = "botl"
-Cfg.version     = "112"
-Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.workdir = Cfg.wd
+Cfg.mod         = "cmd,mod"
+Cfg.version     = "16"
+Cfg.opts        = ""
+Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
 
 
-from botl import modules
+Workdir.workdir = Cfg.wdr
 
 
 def daemon(pidfile, verbose=False):
+    "switch to background."
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
         os._exit(0)
@@ -52,51 +53,35 @@
             os.dup2(sos.fileno(), sys.stdout.fileno())
         with open('/dev/null', 'a+', encoding="utf-8") as ses:
             os.dup2(ses.fileno(), sys.stderr.fileno())
     os.umask(0)
     os.chdir("/")
     if os.path.exists(pidfile):
         os.unlink(pidfile)
-    cdir(os.path.dirname(pidfile))
+    path = pathlib.Path(pidfile)
+    path.parent.mkdir(parents=True, exist_ok=True)
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
-def init(pkg, modstr, disable=""):
-    mds = []
-    for modname in spl(modstr):
-        if modname in spl(disable):
-            continue
-        module = getattr(pkg, modname, None)
-        if not module:
-            continue
-        if "init" in dir(module):
-            module.init()
-            mds.append(module)
-    return mds
-
-
 def privileges(username):
+    "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
-def ver(event):
-    event.reply(f"{Cfg.name.upper()} {Cfg.version}")
-
-
 def main():
-    Command.add(ver)
-    enable(print)
+    "main"
     skel()
-    Cfg.mod = "," + ",".join(modules.__dir__())
+    Cfg.mod  = ",".join(dir(modules))
     Cfg.user = getpass.getuser()
     daemon(Cfg.pidfile, "-v" in sys.argv)
     privileges(Cfg.user)
+    scan(modules, Cfg.mod)
     init(modules, Cfg.mod)
     while 1:
         time.sleep(1.0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `botl-112/botl/client.py` & `botl-120/botl/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0718
 
 
 "client"
 
 
-from .command import Command
-from .default import Default
-from .errors  import later
-from .event   import Event
-from .handler import Handler
+import inspect
+
+
+from .handler import Event, Handler
+from .object  import Default, Object
+from .thread  import later
 
 
 class Client(Handler):
 
     "Client"
 
     def __init__(self):
@@ -34,39 +33,51 @@
 
     def show(self, evt):
         "show results into a channel."
         for txt in evt.result:
             self.say(evt.channel, txt)
 
 
-def cmnd(txt, out):
-    "do a command using the provided output function."
-    clt = Client()
-    clt.raw = out
-    evn = Event()
-    evn.orig = object.__repr__(clt)
-    evn.txt = txt
-    command(clt, evn)
-    evn.wait()
-    return evn
+class Command(Object): # pylint: disable=R0903
+
+    "Command"
+
+    cmds = Object()
+
+
+def add(func):
+    "add command."
+    setattr(Command.cmds, func.__name__, func)
 
 
 def command(bot, evt):
     "check for and run a command."
-    parse_cmd(evt)
+    parse(evt)
     func = getattr(Command.cmds, evt.cmd, None)
     if func:
         try:
             func(evt)
-        except Exception as exc:
+        except Exception as exc: # pylint: disable=W0718
             later(exc)
     bot.show(evt)
     evt.ready()
 
 
+def cmnd(txt, outer):
+    "do a command using the provided output function."
+    clt = Client()
+    clt.raw = outer
+    evn = Event()
+    evn.orig = object.__repr__(clt)
+    evn.txt = txt
+    command(clt, evn)
+    evn.wait()
+    return evn
+
+
 def laps(seconds, short=True):
     "show elapsed time."
     txt = ""
     nsec = float(seconds)
     if nsec < 1:
         return f"{nsec:.2f}s"
     yea = 365*24*60*60
@@ -99,15 +110,15 @@
         txt += f"{minutes}m"
     if sec:
         txt += f"{sec}s"
     txt = txt.strip()
     return txt
 
 
-def parse_cmd(obj, txt=None):
+def parse(obj, txt=None):
     "parse a string for a command."
     args = []
     obj.args    = obj.args or []
     obj.cmd     = obj.cmd or ""
     obj.gets    = obj.gets or Default()
     obj.hasmods = obj.hasmod or False
     obj.index   = None
@@ -153,14 +164,26 @@
         obj.txt  = obj.cmd or ""
         obj.rest = " ".join(obj.args)
         obj.txt  = obj.cmd + " " + obj.rest
     else:
         obj.txt = obj.cmd or ""
 
 
-def spl(txt):
-    "split comma separated string into a list."
-    try:
-        res = txt.split(',')
-    except (TypeError, ValueError):
-        res = txt
-    return [x for x in res if x]
+def scancmd(mod) -> None:
+    "scan module for commands."
+    for key, cmd in inspect.getmembers(mod, inspect.isfunction):
+        if key.startswith("cb"):
+            continue
+        if 'event' in cmd.__code__.co_varnames:
+            add(cmd)
+
+
+def __dir__():
+    return (
+        'Client',
+        'Commands',
+        'add',
+        'command',
+        'laps',
+        'parse',
+        'scancmd'
+    )
```

### Comparing `botl-112/botl/find.py` & `botl-120/botl/find.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
-"locate"
+"find"
 
 
 import os
 import time
 
 
-from .default import Default
-from .object  import fqn, search, update
-from .persist import long
-from .workdir import fetch, store, strip
+from .disk import fetch, long, store, strip
+from .object import Default, fqn, search, update
 
 
 def fns(mtc=""):
     "show list of files."
     dname = ''
     pth = store(mtc)
     for rootdir, dirs, _files in os.walk(pth, topdown=False):
@@ -71,7 +67,16 @@
                    )
     res = None
     if result:
         inp = result[-1]
         update(obj, inp[-1])
         res = inp[0]
     return res
+
+
+def __dir__():
+    return (
+        'fns',
+        'fntime',
+        'find',
+        'last'
+    )
```

### Comparing `botl-112/botl/handler.py` & `botl-120/botl/handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0212
 
 
 "handler"
 
 
 import queue
 import threading
 import _thread
 
 
-from .object import Object
+from .object import Default, Object
 from .thread import launch
 
 
+rpr = object.__repr__
+
+
 class Handler:
 
     "Handler"
 
     def __init__(self):
         self.cbs      = Object()
         self.queue    = queue.Queue()
@@ -27,15 +28,15 @@
 
     def callback(self, evt):
         "call callback based on event type."
         func = getattr(self.cbs, evt.type, None)
         if not func:
             evt.ready()
             return
-        evt._thr = launch(func, self, evt)
+        evt._thr = launch(func, self, evt) # pylint: disable=W0212
 
     def loop(self):
         "proces events until interrupted."
         while not self.stopped.is_set():
             try:
                 evt = self.poll()
                 self.callback(evt)
@@ -57,7 +58,44 @@
     def start(self):
         "start the event loop."
         launch(self.loop)
 
     def stop(self):
         "stop the event loop."
         self.stopped.set()
+
+
+class Event(Default): # pylint: disable=R0902
+
+    "Event"
+
+    def __init__(self):
+        Default.__init__(self)
+        self._thr    = None
+        self._ready  = threading.Event()
+        self.done    = False
+        self.orig    = None
+        self.result  = []
+        self.txt     = ""
+        self.type    = "event"
+
+    def ready(self):
+        "event is ready."
+        self._ready.set()
+
+    def reply(self, txt):
+        "add text to the result"
+        self.result.append(txt)
+
+    def wait(self):
+        "wait for event to be ready."
+        if self._thr:
+            self._thr.join()
+        self._ready.wait()
+        return self.result
+
+
+def __dir__():
+    return (
+        'Event',
+        'Handler'
+    )
```

### Comparing `botl-112/botl/modules/fnd.py` & `botl-120/botl/modules/fnd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0611,E0402
 
 
 "locate"
 
 
-from ..command import Command
-from ..find    import find
-from ..object  import fmt
-from ..persist import long
-from ..workdir import liststore, skel
+from ..find   import find
+from ..object import fmt
+from ..disk   import lsstore, long, skel
 
 
 def fnd(event):
+    "locate objects."
     skel()
     if not event.rest:
-        res = sorted([x.split('.')[-1].lower() for x in liststore()])
+        res = sorted([x.split('.')[-1].lower() for x in lsstore()])
         if res:
             event.reply(",".join(res))
         return
     otype = event.args[0]
     clz = long(otype)
     if "." not in clz:
-        for fnm in liststore():
+        for fnm in lsstore():
             claz = fnm.split(".")[-1]
             if otype == claz.lower():
                 clz = fnm
     nmr = 0
     for fnm, obj in find(clz, event.gets):
         event.reply(f"{nmr} {fmt(obj)}")
         nmr += 1
     if not nmr:
         event.reply("no result")
-
-
-#Command.add(fnd)
```

### Comparing `botl-112/botl/modules/irc.py` & `botl-120/botl/modules/irc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105,W0612,W0718,E0402,W0201,W0603
-# ruff: noqa: F841
 
 
 "internet relay chat"
 
 
 import base64
 import os
@@ -15,59 +12,54 @@
 import textwrap
 import threading
 import time
 import _thread
 
 
 from ..client  import Client, command
-from ..command import Command
-from ..default import Default
-from ..errors  import debug, later
-from ..event   import Event
+from ..disk    import sync, whitelist
 from ..find    import last
-from ..object  import Object, edit, fmt, keys
-from ..persist import whitelist
-from ..runtime import broker
-from ..thread  import launch
-from ..workdir import sync
+from ..handler import Event
+from ..log     import Logging, debug
+from ..object  import Default, Object, edit, fmt, keys, values
+from ..run     import broker
+from ..thread  import later, launch
 
 
-NAME       = __file__.split(os.sep)[-3]
-filterlist = ["PING", "PONG", "PRIVMSG"]
-saylock    = _thread.allocate_lock()
+NAME    = __file__.split(os.sep)[-3]
+saylock = _thread.allocate_lock()
 
 
-myirc = None
+Logging.filter = ["PING", "PONG", "PRIVMSG"]
 
 
-def dbg(txt):
-    for flt in filterlist:
-        if flt in txt:
-            return
-    debug(txt)
-
 def init():
-    global myirc
+    "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
-    myirc = irc
+    debug(f'started irc {fmt(Config,skip="password")}')
     return irc
 
 
 def shutdown():
-    dbg(f"IRC stopping {myirc}")
-    if myirc:
-        myirc.state.pongcheck = True
-        myirc.state.keeprunning = False
-        myirc.events.connected.clear()
-        myirc.stop()
+    "shutdown irc bot."
+    for bot in values(broker.objs):
+        if "irc" not in str(type(bot)).lower():
+            continue
+        debug(f"IRC stopping {repr(bot)}")
+        bot.state.pongcheck = True
+        bot.state.keeprunning = False
+        bot.events.connected.clear()
+        bot.stop()
+
 
+class Config(Default): # pylint: disable=R0902,R0903
 
-class Config(Default):
+    "Config"
 
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
@@ -92,14 +84,16 @@
 
 
 whitelist(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
+    "TextWrap"
+
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -107,47 +101,54 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
+    "Output"
+
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
+        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
+        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
         chanlist = getattr(Output.cache, channel)
         chanlist.extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
+        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
+        "put text to output queue."
         if channel and channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
+        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -162,21 +163,24 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
+        "return size of channel cache."
         if chan in Output.cache:
             return len(getattr(Output.cache, chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
+    "IRC"
+
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
         self.channels = []
         self.events = Default()
@@ -202,18 +206,20 @@
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
         broker.add(self)
 
     def announce(self, txt):
+        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
     def docommand(self, cmd, *args):
+        "send command to server."
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -222,18 +228,19 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
+        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
-            dbg("using SASL")
+            debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.options |= ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1
             ctx.minimum_version = ssl.TLSVersion.TLSv1_2
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
@@ -248,47 +255,51 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
+        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
+        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as ex:
+               ) as _ex:
             pass
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0718
             later(ex)
 
     def doconnect(self, server, nck, port=6667):
+        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
                 self.state.error = str(ex)
-                dbg(str(ex))
-            dbg(f"sleeping {self.cfg.sleep} seconds")
+                debug(str(ex))
+            debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
+        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.docommand('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
@@ -307,49 +318,54 @@
         elif cmd == '433':
             self.state.error = txt
             nck = self.cfg.nick + '_'
             self.docommand('NICK', nck)
         return evt
 
     def joinall(self):
+        "join all channels."
         for channel in self.channels:
             self.docommand('JOIN', channel)
 
     def keep(self):
+        "keep alive."
         while not self.stopped.is_set():
             if self.state.stopkeep:
                 self.state.stopkeep = False
                 break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.docommand('PING', self.cfg.server)
             if self.state.pongcheck:
-                dbg("failed pongcheck, restarting")
+                debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
+        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
+        "parse text into an event."
+        # pylint: disable=R0912,R0915
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
-        dbg(txt)
+        debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
@@ -399,14 +415,15 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
+        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -416,26 +433,27 @@
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
                 later(ex)
                 self.stop()
-                dbg("handler stopped")
+                debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
+        "send raw text."
         txt = txt.rstrip()
-        dbg(txt)
+        debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
@@ -448,47 +466,52 @@
                 later(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        dbg(f"reconnecting to {self.cfg.server}")
+        "reconnect to server."
+        debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
+        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.docommand('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
+        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
+        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
+        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
         launch(Client.start, self)
@@ -498,101 +521,111 @@
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
+        "stop bot."
         self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
+        "wait for ready."
         self.events.ready.wait()
 
 
 def cb_auth(bot, evt):
+    "auth callback."
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
 def cb_cap(bot, evt):
+    "capabilities callback."
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
 def cb_error(bot, evt):
+    "error callback."
     if not bot.state.nrerror:
         bot.state.nrerror = 0
     bot.state.nrerror += 1
     bot.state.error = evt.txt
-    dbg(evt.txt)
+    debug(evt.txt)
 
 
 def cb_h903(bot, evt):
+    "auth succeded callback."
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_h904(bot, evt):
+    "auth succeded callback."
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
 def cb_kill(bot, evt):
-    pass
+    "got killed callback."
 
 
 def cb_log(bot, evt):
-    pass
+    "log callback."
 
 
 def cb_ready(bot, evt):
+    "bot is ready callback."
     bot.events.ready.set()
 
 
 def cb_001(bot, evt):
+    "first line received callback."
     bot.logon()
 
 
 def cb_notice(bot, evt):
+    "notice callback."
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
         bot.docommand('NOTICE', evt.channel, txt)
 
 
 def cb_privmsg(bot, evt):
+    "privmsg callback."
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
-        dbg(f"command from {evt.origin}: {evt.txt}")
+        debug(f"command from {evt.origin}: {evt.txt}")
         command(bot, evt)
 
 
 def cb_quit(bot, evt):
-    dbg(f"quit from {bot.cfg.server}")
+    "quit callback."
+    debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
-"commands"
-
-
 def cfg(event):
+    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
@@ -601,18 +634,16 @@
                    )
     else:
         edit(config, event.sets)
         sync(config, path)
         event.reply('ok')
 
 
-Command.add(cfg)
-
-
 def mre(event):
+    "show from output cache."
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = broker.get(event.orig)
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
@@ -623,24 +654,19 @@
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
     event.reply(f'{size} more in cache')
 
 
-Command.add(mre)
-
-
 def pwd(event):
+    "create a base64 password."
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
     arg1 = event.args[0]
     arg2 = event.args[1]
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
-
-
-Command.add(pwd)
```

### Comparing `botl-112/botl/modules/log.py` & `botl-120/botl/modules/log.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=R,C,E0402
 
 
 "log text"
 
 
 import time
 
 
-from ..client  import laps
-from ..command import Command
-from ..object  import Object
-from ..find    import find, fntime
-from ..workdir import  sync
-from ..persist import whitelist
+from ..client import laps
+from ..disk   import sync
+from ..find   import find, fntime
+from ..object import Object
 
 
-class Log(Object):
+class Log(Object): # pylint: disable=R0903
+
+    "Log"
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
-whitelist(Log)
-
-
 def log(event):
+    "log text."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
-
-
-Command.add(log)
```

### Comparing `botl-112/botl/modules/mbx.py` & `botl-120/botl/modules/mbx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0212,E0402
+# pylint: disable=C,R
 
 
 "mailbox"
 
 
 import mailbox
 import os
 import time
 
 
-from ..object  import Object, fmt, update
-from ..client  import laps
-from ..command import Command
-from ..find    import find, fntime
-from ..persist import whitelist
-from ..workdir import sync
+from ..disk   import sync, whitelist
+from ..object import Object, fmt, update
+from ..client import laps
+from ..find   import find, fntime
 
 
 MONTH = {
     'Jan': 1,
     'Feb': 2,
     'Mar': 3,
     'Apr': 4,
@@ -33,23 +31,26 @@
     'Nov': 11,
     'Dec': 12
 }
 
 
 class Email(Object):
 
+    "Email"
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.text = ""
 
 
 whitelist(Email)
 
 
 def to_date(date):
+    "match date in string." 
     date = date.replace("_", ":")
     res = date.split()
     ddd = ""
     try:
         if "+" in res[3]:
             raise ValueError
         if "-" in res[3]:
@@ -78,46 +79,43 @@
                             ddd = "{:4}".format(res[2])
                         except (IndexError, KeyError):
                             ddd = ""
     return ddd
 
 
 def cor(event):
+    "correspondence"
     if not event.args:
         event.reply("cor <email>")
         return
     nr = -1
     for _fn, email in find("email", {"From": event.args[0]}):
         nr += 1
         txt = ""
         if len(event.args) > 1:
             txt = ",".join(event.args[1:])
         else:
             txt = "From,Subject"
         event.reply("%s %s %s" % (nr, fmt(email, txt, plain=True), laps(time.time() - fntime(email.__stp__))))
 
 
-Command.add(cor)
-
-
 def eml(event):
+    "emnail"
     if not event.args:
         event.reply("eml <searchtxtinemail>")
         return
     nr = -1
     for fn, o in find("email"):
         if event.rest in o.text:
             nr += 1
             event.reply("%s %s %s" % (nr, fmt(o, "From,Subject"), laps(time.time() - fntime(fn))))
 
 
-Command.add(eml)
-
-
 def mbx(event):
+    "mailbox"
     if not event.args:
         return
     fn = os.path.expanduser(event.args[0])
     event.reply("reading from %s" % fn)
     nr = 0
     if os.path.isdir(fn):
         thing = mailbox.Maildir(fn, create=False)
@@ -127,20 +125,17 @@
         return
     try:
         thing.lock()
     except FileNotFoundError:
         pass
     for m in thing:
         o = Email()
-        update(o, m._headers)
+        update(o, m._headers) # pylint: disable=W0212
         o.text = ""
         for payload in m.walk():
             if payload.get_content_type() == 'text/plain':
                 o.text += payload.get_payload()
         o.text = o.text.replace("\\n", "\n")
         sync(o)
         nr += 1
     if nr:
         event.reply("ok %s" % nr)
-
-
-Command.add(mbx)
```

### Comparing `botl-112/botl/modules/mdl.py` & `botl-120/botl/modules/mdl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0613,E0402,W0105
+# pylint: disable=C0209
 
 
-"genocide model of the netherlands"
+"genocide model of the netherlands since 01-01-2020"
 
 
 import datetime
 import time
 
 
-from ..client   import laps
-from ..command  import Command
-from ..event    import Event
-from ..object   import Object, construct, keys, values
-from ..repeater import Repeater
-from ..runtime  import broker
-from ..thread   import launch
+from ..client  import laps
+from ..handler import Event
+from ..object  import Object, construct, keys, values
+from ..run     import broker
+from ..thread  import Repeater, launch
 
 
 DAY = 24*60*60
 YEAR = 365*DAY
-SOURCE = "https://github.com/bthate/genocide"
+SOURCE = "https://github.com/xobjectz/otpcr"
 STARTDATE = "2020-01-01 00:00:00"
 STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
 
 def init():
+    "start repeaters"
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
             repeater = Repeater(sec, cbstats, evt, thrname=aliases.get(key))
             repeater.start()
     launch(daily, name="daily")
-    
 
 
 oor = """"Totaal onderliggende doodsoorzaken (aantal)";
          "1 Infectieuze en parasitaire ziekten/Totaal infectieuze en parasitaire zktn (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.1 Tuberculose (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.2 Meningokokkeninfecties (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.3 Virale hepatitis (aantal)";
@@ -273,76 +271,87 @@
 
 oorzaak = Object()
 construct(oorzaak, zip(oor, aantal))
 oorzaken = Object()
 
 
 def getalias(txt):
+    "return value of alias."
+    result = None
     for key, value in aliases.items():
         if txt.lower() in key.lower():
-            return value
-
+            result = value
+            break
+    return result
 
 def getday():
+    "timestamp of current day."
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
+    "fetch mortality number."
     for k in keys(oorzaken):
         if name.lower() in k.lower():
             return int(getattr(oorzaken, k))
     return 0
 
 
 def seconds(nrs):
+    "convert nr/years to seconds."
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
 
 def iswanted(k, line):
+    "see whether filtered or not."
     for word in line:
         if word in k:
             return True
     return False
 
 
 def daily():
+    "daily job"
     while 1:
         time.sleep(24*60*60)
         evt = Event()
         cbnow(evt)
 
 
 def hourly():
+    "hourly job"
     while 1:
         time.sleep(60*60)
         evt = Event()
         cbnow(evt)
 
 
-def cbnow(evt):
+def cbnow(_evt):
+    "now callback"
     delta = time.time() - STARTTIME
     txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
-        txt += "%s: %s " % (getalias(name), nrtimes)
+        txt += f"{getalias(name)} {nrtimes} |"
     txt += " http://genocide.rtfd.io"
     for bot in values(broker.objs):
         if "announce" in dir(bot):
             bot.announce(txt)
 
 
 def cbstats(evt):
+    "stats callback."
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
         nrday = int(DAY/needed)
@@ -357,14 +366,15 @@
                                                                nryear,
                                                               )
         for bot in values(broker.objs):
             bot.announce(txt)
 
 
 def now(event):
+    "now command."
     name = event.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         txt = laps(delta) + " "
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
@@ -379,28 +389,16 @@
                                                                  laps(needed)
                                                                 )
         event.reply(txt)
     else:
         event.reply("not needed")
 
 
-Command.add(now)
-
-
-"interface"
-
-
-def __dir__():
-    return (
-            'init',
-            'now'
-           ) 
-
-
 def boot():
+    "construct model"
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
         if _nr == 0:
             continue
         if key.startswith('"'):
             key = key[1:]
@@ -422,8 +420,15 @@
         atl = atl.replace(", bevalling en kraambed. ", "")
         atl = atl.replace("Aandoeningen v.d. ", "")
         nms = " ".join(atl.split()[1:]).capitalize()
         nms = nms.strip()
         setattr(oorzaken, nms, aantal[_nr])
 
 
+def __dir__():
+    return (
+            'init',
+            'now'
+           )
+
+
 boot()
```

### Comparing `botl-112/botl/modules/req.py` & `botl-120/botl/modules/req.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C0115,C0116
 
 
-"""| **Information and Evidence Unit**
-| **Office of the Prosecutor**
-| **Post Office Box 19519**
-| **2500 CM The Hague**
-| **The Netherlands**
-|
+"""OTP-CR-117/19
 
-Hello Office of the Prosecutor,
+By law, with the use of poison, killing, torturing, castrating, destroying in whole or in part, 
+
+
+Information and Evidence Unit
+Office of the Prosecutor
+Post Office Box 19519
+2500 CM The Hague
+The Netherlands
+
+
+Hello Office of the Prosecutor, 
 
 i write you in the context of communications and claims under art.15 of
 the Rome Statute. i want to inform the prosecutor that the king of the
 netherlands and his government are commiting 3 of the 5 crimes defined
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
@@ -61,29 +64,13 @@
 (4) criminelen (criminials)
 (5) gehandicapten (handicapped)
 
 Since the members of the chamber and the king were aware that these
 medicine are poison at the time they voted for this law and the day the
 Wfz law took effect (1-1-2019), i ask the prosecutor to prosecute the
 king for making the commiting of the above mentioned crimes (killing,
-torture and impotent making) possible here in the netherlands in the
-hope that it stops the mass torture with poison the king of the
-netherlands and his government are doing.
-
-Bart Thate
-
-p.s.
-
-
-(1) provided are the confirmation letters of both the chamber and the king.
-(2) your reference: OTP-CR-117/19
-"""
-
-
-from ..command import Command
+torture and impotent making) possible."""
 
 
 def req(event):
+    "reconsider"
     event.reply(__doc__)
-
-
-Command.add(req)
```

### Comparing `botl-112/botl/modules/rss.py` & `botl-120/botl/modules/rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -14,24 +12,20 @@
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..client   import laps, spl
-from ..command  import Command
-from ..default  import Default
-from ..find     import find, fntime, last
-from ..object   import Object, fmt, update, values
-from ..persist  import whitelist
-from ..repeater import Repeater
-from ..runtime  import broker
-from ..thread   import launch
-from ..workdir  import sync
+from ..client import laps
+from ..disk   import sync
+from ..find   import find, fntime, last
+from ..object import Default, Object, fmt, update, values
+from ..run    import broker, spl
+from ..thread import Repeater, launch
 
 
 def init():
     "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
@@ -47,30 +41,30 @@
     <head>
         <title>rssbot opml</title>
     </head>
     <body>
         <outline title="rssbot opml" text="24/7 feed fetcher">"""
 
 
-class Feed(Default):
+class Feed(Default): # pylint: disable=R0903
 
     "Feed"
 
 
-class Rss(Default):
+class Rss(Default): # pylint: disable=R0903
 
     "Rss"
 
     def __init__(self):
         Default.__init__(self)
         self.display_list = 'title,link,author'
         self.rss          = ''
 
 
-class Seen(Default):
+class Seen(Default): # pylint: disable=R0903
 
     "Seen"
 
     def __init__(self):
         Default.__init__(self)
         self.urls = []
 
@@ -320,17 +314,14 @@
 
 
 def useragent(txt):
     "return useragent."
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
-"commands"
-
-
 def dpl(event):
     "set display items."
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
     for _fn, feed in find('rss', {'rss': event.args[0]}):
@@ -413,20 +404,7 @@
         if result:
             event.reply(f'already got {url}')
             return
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
-
-
-"register"
-
-
-Command.add(dpl)
-Command.add(exp)
-Command.add(nme)
-Command.add(rem)
-Command.add(res)
-Command.add(rss)
-whitelist(Rss)
-whitelist(Seen)
```

### Comparing `botl-112/botl/modules/rst.py` & `botl-120/botl/modules/rst.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,25 @@
 import sys
 import time
 
 
 from http.server import HTTPServer, BaseHTTPRequestHandler
 
 
-from ..default import Default
-from ..errors  import debug, later
-from ..find    import fns
-from ..object  import Object
-from ..thread  import launch
-from ..workdir import Workdir
+from ..find   import fns
+from ..log    import debug
+from ..object import Default, Object, fmt
+from ..thread import later, launch
+from ..disk   import Workdir
 
 
 def init():
-    try:
-        rest = REST((Config.hostname, int(Config.port)), RESTHandler)
-    except OSError:
-        return
+    rest = REST((Config.hostname, int(Config.port)), RESTHandler)
     launch(rest.start)
+    debug(f"started {fmt(Config)}")
     return rest
 
 
 def html(txt):
     return """<!doctype html>
 <html>
    %s
@@ -91,19 +88,21 @@
     def write_header(self, htype='text/plain'):
         self.send_response(200)
         self.send_header('Content-type', '%s; charset=%s ' % (htype, "utf-8"))
         self.send_header('Server', "1")
         self.end_headers()
 
     def do_GET(self):
+        if "favicon" in self.path:
+            return
         if self.path == "/":
             self.write_header("text/html")
             txt = ""
             for fnm in fns():
-                txt += f'<a href="http://{Config.hostname}:{Config.port}/{fnm}">{fnm}</a>\n'
+                txt += f'<a href="http://{Config.hostname}:{Config.port}/{fnm}">{fnm}</a><br>\n'
             self.send(html(txt.strip()))
             return
         fnm = Workdir.workdir + os.sep + "store" + os.sep + self.path
         try:
             f = open(fnm, "r", encoding="utf-8")
             txt = f.read()
             f.close()
```

### Comparing `botl-112/botl/modules/tdo.py` & `botl-120/botl/modules/tdo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,E0402
 
 
 "todo list"
 
 
 import time
 
 
-from ..client  import laps
-from ..object  import Object
-from ..command import Command
-from ..find    import fntime, find
-from ..persist import whitelist
-from ..workdir import sync
+from ..client import laps
+from ..disk   import sync
+from ..find   import fntime, find
+from ..object import Object
 
 
 class NoDate(Exception):
 
-    pass
+    "no matching date"
 
 
-class Todo(Object):
+class Todo(Object): # pylint: disable=R0903
+
+    "Todo"
 
     def __init__(self):
         Object.__init__(self)
         self.txt = ''
 
 
-whitelist(Todo)
-
-
 def dne(event):
+    "flag todo as done."
     if not event.args:
         event.reply("dne <txt>")
         return
     selector = {'txt': event.args[0]}
     nmr = 0
     for fnm, obj in find('todo', selector):
         nmr += 1
@@ -44,27 +40,22 @@
         sync(obj, fnm)
         event.reply('ok')
         break
     if not nmr:
         event.reply("nothing todo")
 
 
-Command.add(dne)
-
-
 def tdo(event):
+    "add todo."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('todo'):
             lap = laps(time.time()-fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply("no todo")
         return
     obj = Todo()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
-
-
-Command.add(tdo)
```

### Comparing `botl-112/botl/modules/thr.py` & `botl-120/botl/modules/thr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C0116,W0105,E0402,E0401,E0611
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
-from ..client import Command, laps
+from ..client    import laps
 from ..object import Object, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
+    "show running threads."
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
@@ -35,10 +34,7 @@
     for uptime, txt in sorted(result, key=lambda x: x[1]):
         lap = laps(uptime)
         res.append(f'{txt}/{lap}')
     if res:
         event.reply(' '.join(res))
     else:
         event.reply('no threads')
-
-
-Command.add(thr)
```

### Comparing `botl-112/botl/modules/tmr.py` & `botl-120/botl/modules/tmr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0612,W0105,W0702,E0402
 
 
 "timer"
 
 
 import datetime
 import re
 import time as ttime
 
 
 from ..client  import laps
-from ..command import Command
-from ..event   import Event
+from ..disk    import sync
 from ..find    import find
-from ..runtime import broker
-from ..timer   import Timer
-from ..thread  import launch
-from ..persist import whitelist
 from ..object  import update
-from ..workdir import sync
+from ..handler import Event
+from ..run     import broker
+from ..thread  import Timer, launch
 
 
 def init():
-    for fnm, obj in find("timer"):
+    "start timers."
+    for _fn, obj in find("timer"):
         if "time" not in obj:
             continue
         diff = float(obj.time) - ttime.time()
         if diff > 0:
             bot = broker.first()
             evt = Event()
             update(evt, obj)
@@ -60,56 +56,57 @@
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    pass
-
-
-whitelist(Timer)
+    "NoDate"
 
 
 def extract_date(daystr):
+    "extract date from string."
+    res = None
     for fmt in FORMATS:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
+            break
         except ValueError:
             res = None
-        if res:
-            return res
+    return res
 
 
 def get_day(daystr):
+    "return day from string."
     day = None
     month = None
     yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
         if ymdre:
             (day, month, yea) = ymdre.groups()
     except ValueError:
         try:
             ymre = re.search(r'(\d+)-(\d+)', daystr)
             if ymre:
                 (day, month) = ymre.groups()
                 yea = ttime.strftime("%Y", ttime.localtime())
-        except Exception as ex:
+        except Exception as ex: # pylint: disable=W0212
             raise NoDate(daystr) from ex
     if day:
         day = int(day)
         month = int(month)
         yea = int(yea)
-        date = "%s %s %s" % (day, MONTHS[month], yea)
+        date = f"{day} {MONTHS[month]} {yea}"
         return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
     raise NoDate(daystr)
 
 
 def get_hour(daystr):
+    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -123,25 +120,27 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
+    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
 def parse_time(txt):
+    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -156,78 +155,74 @@
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
 def to_day(daystr):
+    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
+    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
+            break
         except ValueError:
             res = None
-        if res:
-            return res
         line = ""
+    return res
 
 
 def today():
+    "return date."
     return str(datetime.datetime.today()).split()[0]
 
 
-"commands"
-
-
 def tmr(event):
+    "add a timer."
+    result = ""
     if not event.rest:
         nmr = 0
-        for fnm, obj in find('timer'):
-            if "time" not in obj:
-                continue
+        for _fn, obj in find('timer'):
             lap = float(obj.time) - ttime.time()
             if lap > 0:
                 event.reply(f'{nmr} {obj.txt} {laps(lap)}')
                 nmr += 1
-        if not nmr:
-            event.reply("no timers")
-        return
+        return result
     seconds = 0
     line = ""
     for word in event.args:
         if word.startswith("+"):
             try:
                 seconds = int(word[1:])
             except (ValueError, IndexError):
-                event.reply("%s is not an integer" % seconds)
-                return
+                event.reply(f"{seconds} is not an integer")
+                return result
         else:
             line += word + " "
     if seconds:
         target = ttime.time() + seconds
     else:
         try:
             target = get_day(event.rest)
         except NoDate:
             target = to_day(today())
         hour =  get_hour(event.rest)
         if hour:
             target += hour
     if not target or ttime.time() > target:
         event.reply("already passed given time.")
-        return
+        return result
     event.time = target
     diff = target - ttime.time()
     event.reply("ok " +  laps(diff))
     event.result = []
     event.result.append(event.rest)
     timer = Timer(diff, event.show, thrname=event.cmd)
     update(timer, event)
     sync(timer)
     launch(timer.start)
-
-
-Command.add(tmr)
+    return result
```

### Comparing `botl-112/botl/modules/udp.py` & `botl-120/botl/modules/udp.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 import select
 import socket
 import sys
 import threading
 import time
 
 
-from ..object  import Object, values
-from ..command import Command
-from ..runtime import broker
-from ..thread  import launch
+from ..log    import debug
+from ..object import Object, fmt
+from ..run    import broker
+from ..thread import launch
 
 
 def init():
     udpd = UDP()
     udpd.start()
+    debug(f"started udp {fmt(Cfg)}")
     return udpd
 
 
 class Cfg(Object):
 
     addr = ""
     host = "localhost"
@@ -43,15 +44,15 @@
         self._sock.setblocking(1)
         self._starttime = time.time()
         self.ready = threading.Event()
 
     def output(self, txt, addr=None):
         if addr:
             Cfg.addr = addr
-        for bot in values(broker.objs):
+        for bot in broker.all():
             bot.announce(txt.replace("\00", ""))
 
     def loop(self):
         try:
             self._sock.bind((Cfg.host, Cfg.port))
         except socket.gaierror:
             return
@@ -81,15 +82,15 @@
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.sendto(bytes(txt.strip(), "utf-8"), (host, port))
 
 
 def udp(event):
     if event.rest:
         toudp(Cfg.host, Cfg.port, event.rest)
-        event.reply(f"{len(event.rest)} characters sent")
+        debug(f"{len(event.rest)} characters sent")
         return
     if not select.select(
                          [sys.stdin, ],
                          [],
                          [],
                          0.0
                         )[0]:
@@ -112,10 +113,7 @@
             if not txt:
                 stop = True
                 break
             size += len(txt)
             toudp(Cfg.host, Cfg.port, txt)
         if stop:
             break
-
-
-Command.add(udp)
```

### Comparing `botl-112/botl/modules/wsd.py` & `botl-120/botl/modules/wsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,I,R,E0401,W0105
 
 
 """| wijsheid, wijs !
 
 | OVERDRACHT
 | ==========
 
@@ -185,18 +183,13 @@
 | coding
 """
 
 
 from random import SystemRandom
 
 
-from ..command import Command
-
-
 rand = SystemRandom()
 
 
 def wsd(event):
+    "show wisdom."
     event.reply(rand.choice(__doc__.split("\n")).strip()[2:])
-
-
-Command.add(wsd)
```

### Comparing `botl-112/botl/object.py` & `botl-120/botl/object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # This file is placed in the Public Domain.
-#
-# pylint: disable=C,R,W0105
 
 
-"objects"
+"clean namespace"
 
 
 import json
-import os
 import pathlib
 import _thread
 
 
-disklock = _thread.allocate_lock()
+lock = _thread.allocate_lock()
 
 
-class Object:
+class Object: # pylint: disable=R0902
 
     "Object"
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
@@ -28,14 +25,22 @@
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
         return str(self.__dict__)
 
 
+class Default(Object): # pylint: disable=R0902,R0903
+
+    "Default"
+
+    def __getattr__(self, key):
+        return self.__dict__.get(key, "")
+
+
 def construct(obj, *args, **kwargs):
     "construct an object from provided arguments."
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
@@ -113,15 +118,15 @@
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
 def read(obj, pth):
     "read an object from file path."
-    with disklock:
+    with lock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             update(obj, load(ofile))
 
 
 def search(obj, selector):
     "check if object matches provided values."
     res = False
@@ -148,16 +153,17 @@
 def values(obj):
     "return values of an object."
     return obj.__dict__.values()
 
 
 def write(obj, pth):
     "write an object to disk."
-    with disklock:
-        cdir(os.path.dirname(pth))
+    with lock:
+        path = pathlib.Path(pth)
+        path.parent.mkdir(parents=True, exist_ok=True)
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile, indent=4)
 
 
 class ObjectDecoder(json.JSONDecoder):
 
     "ObjectDecoder"
@@ -240,28 +246,18 @@
 
 def dumps(*args, **kw):
     "dump object to string."
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
 
 
-def cdir(pth):
-    "create directory."
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
-
-
-"interface"
-
-
 def __dir__():
     return (
         'Object',
+        'Default',
         'construct',
         'dump',
         'dumps',
         'edit',
         'fmt',
         'fqn',
         'hook',
@@ -271,10 +267,7 @@
         'loads',
         'read',
         'search',
         'update',
         'values',
         'write'
     )
-
-
-__all__ = __dir__()
```

### Comparing `botl-112/botl.egg-info/PKG-INFO` & `botl-120/botl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 112
+Version: 120
 Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
@@ -21,26 +21,32 @@
     BOTL - bot library
 
 
 SYNOPSIS
 
 ::
 
-    botl <cmd> [key=val] [key==val]
-    botl [-a] [-c] [-d] [-h] [-v]
+    botl  <cmd> [key=val] [key==val]
+    botl  [-c] [-v]
+    botld 
 
     options are:
 
-    -a     load all modules
     -c     start console
-    -d     start daemon
-    -h     display help
     -v     use verbose
 
 
+INSTALL
+
+::
+
+    $ pipx install botl
+    $ pipx ensurepath
+
+
 DESCRIPTION
 
 ::
 
     BOTL contains all the python3 code to program objects in a functional
     way. It provides a base Object class that has only dunder methods, all
     methods are factored out into functions with the objects as the first
@@ -61,14 +67,41 @@
     BOTL has a demo bot, it can connect to IRC, fetch and display RSS
     feeds, take todo notes, keep a shopping list and log text. You can
     also copy/paste the service file and run it under systemd for 24/7
     presence in a IRC channel.
 
     BOTL is Public Domain.
 
+
+CONFIGURATION
+
+::
+
+    $ botl cfg 
+    channel=#botl commands=True nick=botl port=6667 server=localhost
+
+    irc
+
+    $ botl cfg server=<server>
+    $ botl cfg channel=<channel>
+    $ botl cfg nick=<nick>
+
+    sasl
+
+    $ botl pwd <nsvnick> <nspass>
+    $ botl cfg password=<frompwd>
+
+    rss
+
+    $ botl rss <url>
+    $ botl dpl <url> <item1,item2>
+    $ botl rem <url>
+    $ botl nme <url> <name>
+
+
 USAGE
 
 ::
 
     without any argument the program does nothing
 
     $ botl
@@ -96,39 +129,14 @@
     use -v for verbose
 
     $ botl -cv mod=irc
     BOTL started CV started Sat Dec 2 17:53:24 2023
     >
 
 
-CONFIGURATION
-
-::
-
-    $ botl cfg 
-    channel=#botl commands=True nick=botl port=6667 server=localhost
-
-    irc
-
-    $ botl cfg server=<server>
-    $ botl cfg channel=<channel>
-    $ botl cfg nick=<nick>
-
-    sasl
-
-    $ botl pwd <nsvnick> <nspass>
-    $ botl cfg password=<frompwd>
-
-    rss
-
-    $ botl rss <url>
-    $ botl dpl <url> <item1,item2>
-    $ botl rem <url>
-    $ botl nme <url> <name>
-
 COMMANDS
 
 ::
 
     cmd - commands
     cfg - irc configuration
     dlt - remove a user
```

### Comparing `botl-112/pyproject.toml` & `botl-120/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "botl"
 description = "bot library"
-version = "112"
+version = "120"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
@@ -27,16 +27,15 @@
 "bugs" = "https://github.com/xobjectz/botl/issues"
 "source" = "https://github.com/xobjectz/botl"
 
 
 [tool.setuptools]
 script-files = [
     "bin/botl",
-    "bin/botld",
-    "bin/botlbot"
+    "bin/botld"
 ]
 packages = [
     "botl",
     "botl.modules"
 ]
 zip-safe=true
```

