# Comparing `tmp/piqueserver-1.1.1.tar.gz` & `tmp/piqueserver-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqueserver-1.1.1.tar", last modified: Mon Jul  3 17:47:04 2023, max compression
+gzip compressed data, was "piqueserver-1.2.0.tar", last modified: Wed May 15 17:41:55 2024, max compression
```

## Comparing `piqueserver-1.1.1.tar` & `piqueserver-1.2.0.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.779773 piqueserver-1.1.1/
--rw-r--r--   0 nota      (1000) nota      (1000)    35147 2023-07-03 17:42:02.000000 piqueserver-1.1.1/COPYING.txt
--rw-r--r--   0 nota      (1000) nota      (1000)    35141 2023-07-03 17:42:02.000000 piqueserver-1.1.1/LICENSE
--rw-r--r--   0 nota      (1000) nota      (1000)      806 2023-07-03 17:42:02.000000 piqueserver-1.1.1/MANIFEST.in
--rw-r--r--   0 nota      (1000) nota      (1000)     7480 2023-07-03 17:47:04.780773 piqueserver-1.1.1/PKG-INFO
--rw-r--r--   0 nota      (1000) nota      (1000)     6187 2023-07-03 17:46:48.000000 piqueserver-1.1.1/README.rst
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.775773 piqueserver-1.1.1/piqueserver/
--rw-r--r--   0 nota      (1000) nota      (1000)       33 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)      194 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/__main__.py
--rw-r--r--   0 nota      (1000) nota      (1000)      326 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/auth.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1632 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/banpublish.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3145 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/bansubscribe.py
--rw-r--r--   0 nota      (1000) nota      (1000)    13204 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/commands.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.775773 piqueserver-1.1.1/piqueserver/config/
--rw-r--r--   0 nota      (1000) nota      (1000)     1116 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/README.md
--rw-r--r--   0 nota      (1000) nota      (1000)    11263 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/config.toml
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/config/game_modes/
--rw-r--r--   0 nota      (1000) nota      (1000)      297 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/game_modes/README.md
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/config/maps/
--rw-r--r--   0 nota      (1000) nota      (1000)      221 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/maps/classicgen.txt
--rw-r--r--   0 nota      (1000) nota      (1000)     5067 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/maps/random.txt
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/config/scripts/
--rw-r--r--   0 nota      (1000) nota      (1000)      128 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/scripts/README.md
--rw-r--r--   0 nota      (1000) nota      (1000)    10033 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3324 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/console.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/core_commands/
--rw-r--r--   0 nota      (1000) nota      (1000)      911 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     9210 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/game.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2249 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/info.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3497 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/map.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11857 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/moderation.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6367 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/movement.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2926 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/player.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2105 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/server.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2228 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/social.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5090 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/extensions.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/game_modes/
--rw-r--r--   0 nota      (1000) nota      (1000)        0 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)    22203 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/arena.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4285 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/babel.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5043 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/freeforall.py
--rw-r--r--   0 nota      (1000) nota      (1000)    10092 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/infiltration.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4532 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/onectf.py
--rw-r--r--   0 nota      (1000) nota      (1000)    17400 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/push.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5209 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/tdm.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5604 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/tow.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11452 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/irc.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5876 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/map.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2953 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/networkdict.py
--rw-r--r--   0 nota      (1000) nota      (1000)    16156 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/player.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1350 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/release.py
--rw-r--r--   0 nota      (1000) nota      (1000)     8537 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/run.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1666 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scheduler.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/scripts/
--rw-r--r--   0 nota      (1000) nota      (1000)        0 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4485 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/afk.py
--rw-r--r--   0 nota      (1000) nota      (1000)    19815 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/aimbot2.py
--rw-r--r--   0 nota      (1000) nota      (1000)    12194 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/airstrike2.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6238 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/analyze.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1602 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/antijerk.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1795 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/autohelp.py
--rw-r--r--   0 nota      (1000) nota      (1000)     9288 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/babel_script.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11601 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/badmin.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6554 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/blockinfo.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5448 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/daycycle.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1612 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/demolitionman.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1946 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/dirtnade.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2091 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/disco.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1617 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/flagreturn.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1734 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/geoip.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11241 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/grownade.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1582 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/map_extensions.py
--rw-r--r--   0 nota      (1000) nota      (1000)    13043 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/mapmakingtools.py
--rw-r--r--   0 nota      (1000) nota      (1000)    24491 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/markers.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5503 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/match.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1476 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/medkit.py
--rw-r--r--   0 nota      (1000) nota      (1000)      646 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/memcheck.py
--rw-r--r--   0 nota      (1000) nota      (1000)     9858 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/minefield.py
--rw-r--r--   0 nota      (1000) nota      (1000)      494 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/nointelonwalls.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1169 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/nospadingwalls.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2761 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/paint.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1033 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/passreload.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2431 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/protect.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6818 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rampage.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2635 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rangedamage.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3398 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rapid.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2904 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/ratio.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11023 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rollback.py
--rw-r--r--   0 nota      (1000) nota      (1000)     7644 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/runningman.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3250 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/savemap.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1255 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/smartnade.py
--rw-r--r--   0 nota      (1000) nota      (1000)      743 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/spadenadefix.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1430 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/spawn_protect.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4482 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/spectatorcontrol.py
--rw-r--r--   0 nota      (1000) nota      (1000)    10982 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/squad.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3441 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/strongblock.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2064 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/timedmute.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1585 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/trusted.py
--rw-r--r--   0 nota      (1000) nota      (1000)    12461 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/votekick.py
--rw-r--r--   0 nota      (1000) nota      (1000)     8869 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/votemap.py
--rw-r--r--   0 nota      (1000) nota      (1000)      662 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/welcome.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6215 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/zoc.py
--rw-r--r--   0 nota      (1000) nota      (1000)    37061 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/server.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2623 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/ssh.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5739 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/statistics.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5620 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/statusserver.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/utils/
--rw-r--r--   0 nota      (1000) nota      (1000)       86 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/utils/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1786 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/utils/_async.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6642 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/utils/_timeparse.py
--rw-r--r--   0 nota      (1000) nota      (1000)       51 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/version.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/web/
--rw-r--r--   0 nota      (1000) nota      (1000)        0 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/web/__init__.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/web/templates/
--rw-r--r--   0 nota      (1000) nota      (1000)    11833 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/web/templates/status.html
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.775773 piqueserver-1.1.1/piqueserver.egg-info/
--rw-r--r--   0 nota      (1000) nota      (1000)     7480 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/PKG-INFO
--rw-r--r--   0 nota      (1000) nota      (1000)     4176 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/SOURCES.txt
--rw-r--r--   0 nota      (1000) nota      (1000)        1 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/dependency_links.txt
--rw-r--r--   0 nota      (1000) nota      (1000)       53 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/entry_points.txt
--rw-r--r--   0 nota      (1000) nota      (1000)      204 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/requires.txt
--rw-r--r--   0 nota      (1000) nota      (1000)       21 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/top_level.txt
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.779773 piqueserver-1.1.1/pyspades/
--rw-r--r--   0 nota      (1000) nota      (1000)     1111 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1779 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/bytes.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)     9683 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/bytes.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     4510 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/bytes_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)     8890 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/classicgen_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)     1464 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/collision.py
--rw-r--r--   0 nota      (1000) nota      (1000)      977 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/color.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2409 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/common.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)    14662 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/common.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)      365 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/common_c.h
--rw-r--r--   0 nota      (1000) nota      (1000)     2682 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/constants.py
--rw-r--r--   0 nota      (1000) nota      (1000)      299 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/constants_c.h
--rw-r--r--   0 nota      (1000) nota      (1000)    28609 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/contained.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     4989 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/entities.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5316 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/gamemodes.py
--rw-r--r--   0 nota      (1000) nota      (1000)      886 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/loaders.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)     1400 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/loaders.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     3132 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/mapgenerator.py
--rw-r--r--   0 nota      (1000) nota      (1000)    20215 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/mapmaker.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     3352 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/master.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4943 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/packet.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)    53144 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/player.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5776 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/protocol.py
--rw-r--r--   0 nota      (1000) nota      (1000)    17863 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/server.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3117 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/team.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1654 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/tools.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2962 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/types.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1992 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)     9463 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)    15738 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)     2358 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl_c.h
--rw-r--r--   0 nota      (1000) nota      (1000)     4406 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/weapon.py
--rw-r--r--   0 nota      (1000) nota      (1000)    15029 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/world.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)    19626 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/world_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)       80 2023-07-03 17:47:04.780773 piqueserver-1.1.1/setup.cfg
--rw-r--r--   0 nota      (1000) nota      (1000)     4880 2023-07-03 17:42:02.000000 piqueserver-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.074001 piqueserver-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-15 17:41:51.000000 piqueserver-1.2.0/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-15 17:41:51.000000 piqueserver-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-15 17:41:51.000000 piqueserver-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-15 17:41:55.074001 piqueserver-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-15 17:41:51.000000 piqueserver-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.054001 piqueserver-1.2.0/piqueserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/banpublish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/bansubscribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.054001 piqueserver-1.2.0/piqueserver/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/config/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/config/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.054001 piqueserver-1.2.0/piqueserver/config/game_modes/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/config/game_modes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.054001 piqueserver-1.2.0/piqueserver/config/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/config/maps/classicgen.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/config/maps/random.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.054001 piqueserver-1.2.0/piqueserver/config/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/config/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.058001 piqueserver-1.2.0/piqueserver/core_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/core_commands/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.058001 piqueserver-1.2.0/piqueserver/game_modes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22203 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/arena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/babel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/freeforall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/infiltration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/onectf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17400 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/tdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/game_modes/tow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/irc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/networkdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16432 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.066001 piqueserver-1.2.0/piqueserver/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/afk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/aimbot2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/airstrike2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/antijerk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/autohelp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/babel_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/badmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/blockinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/daycycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/demolitionman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/dirtnade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/disco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/flagreturn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/geoip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/grownade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/map_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/mapmakingtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/medkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/memcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/minefield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/nointelonwalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/nospadingwalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/paint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/passreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/rampage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/rangedamage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/rapid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/rollback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/runningman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/savemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/smartnade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/spadenadefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/spawn_protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/spectatorcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/strongblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/timedmute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/trusted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/votekick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/votemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/scripts/zoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37717 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/statusserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.066001 piqueserver-1.2.0/piqueserver/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/utils/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/utils/_timeparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.066001 piqueserver-1.2.0/piqueserver/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.066001 piqueserver-1.2.0/piqueserver/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-15 17:41:51.000000 piqueserver-1.2.0/piqueserver/web/templates/status.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.074001 piqueserver-1.2.0/piqueserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-05-15 17:41:55.000000 piqueserver-1.2.0/piqueserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-15 17:41:55.000000 piqueserver-1.2.0/piqueserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:41:55.000000 piqueserver-1.2.0/piqueserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 17:41:55.000000 piqueserver-1.2.0/piqueserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 17:41:55.000000 piqueserver-1.2.0/piqueserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 17:41:55.000000 piqueserver-1.2.0/piqueserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:41:55.074001 piqueserver-1.2.0/pyspades/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/bytes.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/bytes.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/bytes_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/classicgen_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/common.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    14662 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/common.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/common_c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/constants_c.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28609 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/contained.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/gamemodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/loaders.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/loaders.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/mapgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20215 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/mapmaker.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/packet.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    53546 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/vxl.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/vxl.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/vxl_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/vxl_c.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/weapon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/world.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    19626 2024-05-15 17:41:51.000000 piqueserver-1.2.0/pyspades/world_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 17:41:55.074001 piqueserver-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-15 17:41:51.000000 piqueserver-1.2.0/setup.py
```

### Comparing `piqueserver-1.1.1/COPYING.txt` & `piqueserver-1.2.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/LICENSE` & `piqueserver-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/MANIFEST.in` & `piqueserver-1.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/PKG-INFO` & `piqueserver-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqueserver
-Version: 1.1.1
+Version: 1.2.0
 Summary: Open-Source server implementation for Ace of Spades 
 Home-page: https://github.com/piqueserver/piqueserver
 Author: Originally MatPow2 and PySnip contributors,now, StackOverflow and piqueserver authors
 Author-email: nate.shoffner@gmail.com
 Maintainer: noway421
 Maintainer-email: noway@2ch.hk
 License: GNU General Public License v3
@@ -23,18 +23,29 @@
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Twisted
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: First Person Shooters
 Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
-Provides-Extra: from
-Provides-Extra: ssh
 License-File: LICENSE
 License-File: COPYING.txt
+Requires-Dist: pypiwin32; platform_system == "Windows"
+Requires-Dist: Cython<1,>=0.27
+Requires-Dist: Twisted[tls]
+Requires-Dist: Jinja2<4,>=2
+Requires-Dist: Pillow<11,>=5.1.0
+Requires-Dist: aiohttp<3.8.0,>=3.3.0
+Requires-Dist: pyenet
+Requires-Dist: toml
+Requires-Dist: packaging>=19.0
+Provides-Extra: from
+Requires-Dist: geoip2<5.0,>=2.9; extra == "from"
+Provides-Extra: ssh
+Requires-Dist: Twisted[conch,tls]; extra == "ssh"
 
 piqueserver |Build Status| |Wheel Status| |Coverage Status|
 ===========================================================
 
 An Ace of Spades 0.75 server based on
 `PySnip <https://github.com/NateShoffner/PySnip>`__.
```

### Comparing `piqueserver-1.1.1/README.rst` & `piqueserver-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/banpublish.py` & `piqueserver-1.2.0/piqueserver/banpublish.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/bansubscribe.py` & `piqueserver-1.2.0/piqueserver/bansubscribe.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/commands.py` & `piqueserver-1.2.0/piqueserver/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,19 +399,24 @@
 
     Will log the command.
     """
     result = _handle_command(connection, command, parameters)
 
     if result == False:
         parameters = ['***'] * len(parameters)
-    log_message = '<{}> /{} {}'.format(connection.name, command,
-                                       ' '.join(parameters))
+
+    log_message = '<{name}> /{command} {parameters}'
     if result:
-        log_message += ' -> %s' % result
-    log.info(escape_control_codes(log_message))
+        log_message += ' -> {result}'
+
+    log.info(log_message,
+             name=escape_control_codes(connection.name),
+             command=escape_control_codes(command),
+             parameters=escape_control_codes(' '.join(parameters)),
+             result=escape_control_codes(result))
 
     return result
 
 def _handle_command(connection, command, parameters):
     command = command.lower()
     try:
         command_name = _alias_map.get(command, command)
```

### Comparing `piqueserver-1.1.1/piqueserver/config/README.md` & `piqueserver-1.2.0/piqueserver/config/README.md`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/config/config.toml` & `piqueserver-1.2.0/piqueserver/config/config.toml`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/config/maps/random.txt` & `piqueserver-1.2.0/piqueserver/config/maps/random.txt`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/config.py` & `piqueserver-1.2.0/piqueserver/config.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/console.py` & `piqueserver-1.2.0/piqueserver/console.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/__init__.py` & `piqueserver-1.2.0/piqueserver/core_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/game.py` & `piqueserver-1.2.0/piqueserver/core_commands/game.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/info.py` & `piqueserver-1.2.0/piqueserver/core_commands/info.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/map.py` & `piqueserver-1.2.0/piqueserver/core_commands/map.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/moderation.py` & `piqueserver-1.2.0/piqueserver/core_commands/moderation.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/movement.py` & `piqueserver-1.2.0/piqueserver/core_commands/movement.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/player.py` & `piqueserver-1.2.0/piqueserver/core_commands/player.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/server.py` & `piqueserver-1.2.0/piqueserver/core_commands/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """
     if not arg:
         raise ValueError("no argument given")
     name = join_arguments(arg)
     protocol = connection.protocol
     protocol.set_server_name(name)
     message = "%s changed servername to '%s'" % (connection.name, name)
-    log.info(message)
+    log.info("{message}", message=message)
     connection.protocol.irc_say("* " + message)
     if connection in connection.protocol.players.values():
         return message
     return None
 
 
 @command('server')
```

### Comparing `piqueserver-1.1.1/piqueserver/core_commands/social.py` & `piqueserver-1.2.0/piqueserver/core_commands/social.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/extensions.py` & `piqueserver-1.2.0/piqueserver/extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     dups = []
     for script in script_names:
         if script in seen:
             dups.append(script)
         else:
             seen.add(script)
     if dups:
-        log.warn("Scripts included multiple times: {}".format(dups))
+        log.warn("Scripts included multiple times: {dups}", dups=dups)
         return False
     return True
 
 
 def check_game_mode(game_mode_name):
     '''Validation for a game mode script.
 
@@ -65,30 +65,38 @@
     finder = importlib.machinery.PathFinder()
     for script in script_names:
         spec_scripts = finder.find_spec(script, [script_dir])
         spec_global = importlib.util.find_spec(script)
         spec = spec_scripts or spec_global
         if not spec:
             log.error(
-                "{} '{}' not found in either {} directory or global scope".format(
-                    script_type, script, script_dir))
+                ("{script_type} '{script}' not found in either {script_dir} "
+                 "directory or global scope"),
+                script_type=script_type,
+                script=script,
+                script_dir=script_dir
+            )
             continue
         # namespace module name to avoid shadowing global modules
         # TODO: figure out if there are any right or better ways.
         spec.name = 'piqueserver._{}_namespace.{}'.format(script_type, script)
         spec.loader.name = spec.name
         # load module
         try:
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
             script_objects.append(module)
             continue
         except Exception as e: # needs to be broad since we exec the module
-            log.failure("Error while loading {} {}: {!r}".format(
-                script_type, script, e))
+            log.failure(
+                "Error while loading {script_type} {script}: {exception!r}",
+                script_type=script_type,
+                script=script,
+                exception=e
+            )
 
     return script_objects
 
 
 def load_scripts_regular_extension(script_names, script_dir):
     ''' Wrapper for load function
```

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/arena.py` & `piqueserver-1.2.0/piqueserver/game_modes/arena.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/babel.py` & `piqueserver-1.2.0/piqueserver/game_modes/babel.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/freeforall.py` & `piqueserver-1.2.0/piqueserver/game_modes/freeforall.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/infiltration.py` & `piqueserver-1.2.0/piqueserver/game_modes/infiltration.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/onectf.py` & `piqueserver-1.2.0/piqueserver/game_modes/onectf.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/push.py` & `piqueserver-1.2.0/piqueserver/game_modes/push.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/tdm.py` & `piqueserver-1.2.0/piqueserver/game_modes/tdm.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/game_modes/tow.py` & `piqueserver-1.2.0/piqueserver/game_modes/tow.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/irc.py` & `piqueserver-1.2.0/piqueserver/irc.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def signedOn(self):
         self.join(self.factory.channel, self.factory.password)
 
     def joined(self, irc_channel):
         if irc_channel.lower() == self.factory.channel:
             self.ops = set()
             self.voices = set()
-        log.info("Joined channel %s" % irc_channel)
+        log.info("Joined channel {irc_channel}", irc_channel=irc_channel)
 
     def irc_NICK(self, prefix, params):
         user = prefix.split('!', 1)[0]
         new_user = params[0]
         if user in self.ops:
             self.ops.discard(user)
             self.ops.add(new_user)
@@ -146,15 +146,15 @@
         alias = self.factory.aliases.get(user, user)
 
         if msg.startswith(self.factory.chatprefix):
             max_len = MAX_IRC_CHAT_SIZE - \
                 len(self.protocol.server_prefix) - 1
             msg = msg[len(self.factory.chatprefix):].strip()
             message = ("[irc] <{}> {}".format(prefix + alias, msg))[:max_len]
-            log.info(escape_control_codes(message))
+            log.info('{message}', message=escape_control_codes(message))
             self.factory.server.broadcast_chat(message)
         elif msg.startswith(self.factory.commandprefix) and user in self.ops:
             self.unaliased_name = user
             self.name = prefix + alias
             user_input = msg[len(self.factory.commandprefix):]
             result = commands.handle_input(self, user_input)
             if result is not None:
@@ -218,21 +218,29 @@
         self.chatprefix = config.get('chatprefix', '')
         self.password = config.get('password', '') or None
 
     def startedConnecting(self, connector):
         log.info("Connecting to IRC server...")
 
     def clientConnectionLost(self, connector, reason):
-        log.info("Lost connection to IRC server ({}), reconnecting in {} seconds".format(
-            reason, self.lost_reconnect_delay))
+        log.info(
+            ("Lost connection to IRC server ({reason}), reconnecting in"
+             " {time} seconds"),
+            reason=reason,
+            lost_reconnect_delay=self.lost_reconnect_delay
+        )
         reactor.callLater(self.lost_reconnect_delay, connector.connect)
 
     def clientConnectionFailed(self, connector, reason):
-        log.info("Could not connect to IRC server ({}), retrying in {} seconds".format(
-            reason, self.failed_reconnect_delay))
+        log.info(
+            ("Could not connect to IRC server ({reason}), retrying in"
+             " {time} seconds"),
+            reason=reason,
+            time=self.failed_reconnect_delay
+        )
         reactor.callLater(self.failed_reconnect_delay, connector.connect)
 
     def buildProtocol(self, address):
         p = self.protocol()
         p.factory = self
         p.protocol = self.server
         self.bot = p
```

### Comparing `piqueserver-1.1.1/piqueserver/map.py` & `piqueserver-1.2.0/piqueserver/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,33 +71,34 @@
         if self.gen_script:
             seed = rot_info.get_seed()
             self.name = '{} #{}'.format(rot_info.name, seed)
             log.info("Generating map '{mapname}'...", mapname=self.name)
             random.seed(seed)
             self.data = self.gen_script(rot_info.name, seed)
         else:
-            log.info("Loading map '%s'..." % self.name)
+            log.info("Loading map '{mapname}'...", mapname=self.name)
             self.load_vxl(rot_info)
 
         log.info('Map loaded successfully. (took {duration:.2f}s)',
                  duration=time.monotonic() - start_time)
 
     def load_information(self, rot_info: 'RotationInfo', load_dir: str) -> None:
         path = rot_info.get_meta_filename(load_dir)
         namespace = 'piqueserver_internal_map_' + rot_info.name
         try:
             loader = importlib.machinery.SourceFileLoader(namespace, path)
             spec = importlib.util.spec_from_loader(loader.name, loader)
             info = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(info)
         except FileNotFoundError:
-            log.error("Map info file not found {}".format(path))
+            log.error("Map info file not found {path}", path=path)
             info = None
         except Exception as e:
-            log.error("Error while loading map info: {!r}".format(e))
+            log.error("Error while loading map info: {exception!r}",
+                      exception=e)
             info = None
 
         self.info = info
         self.load_dir = load_dir
         self.rot_info = rot_info
         self.gen_script = getattr(info, 'gen_script', None)
         if self.gen_script:
```

### Comparing `piqueserver-1.1.1/piqueserver/networkdict.py` & `piqueserver-1.2.0/piqueserver/networkdict.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/player.py` & `piqueserver-1.2.0/piqueserver/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,31 @@
         if client_ip in self.protocol.bans:
             name, reason, timestamp = self.protocol.bans[client_ip]
 
             if timestamp is not None and reactor.seconds() >= timestamp:
                 protocol.remove_ban(client_ip)
                 protocol.save_bans()
             else:
-                log.info('banned user {} ({}) attempted to join'
-                         .format(name, client_ip))
+                log.info('banned user {name} ({client_ip}) attempted to join',
+                         name=name,
+                         client_ip=client_ip)
                 self.disconnect(ERROR_BANNED)
                 return
 
         manager = self.protocol.ban_manager
 
         if manager is not None:
             reason = manager.get_ban(client_ip)
             if reason is not None:
-                log.info(('federated banned user (%s) attempted to join, '
-                          'banned for %r') % (client_ip, reason))
+                log.info(
+                    ('federated banned user ({client_ip}) attempted to join, '
+                     'banned for {reason}'),
+                    client_ip=client_ip,
+                    reason=reason
+                )
                 self.disconnect(ERROR_BANNED)
                 return
 
         ServerConnection.on_connect(self)
 
     def on_join(self) -> None:
         if self.protocol.motd is not None:
@@ -321,15 +326,15 @@
     def kick(self, reason=None, silent=False):
         if not silent:
             if reason is not None:
                 message = '{} was kicked: {}'.format(self.name, reason)
             else:
                 message = '%s was kicked' % self.name
             self.protocol.broadcast_chat(message, irc=True)
-            log.info(message)
+            log.info('{message}', message=message)
         # FIXME: Client should handle disconnect events the same way in both
         # main and initial loading network loops
         self.disconnect(ERROR_KICKED)
 
     def ban(self, reason=None, duration=None):
         reason = ': ' + reason if reason is not None else ''
         duration = duration or None
@@ -362,16 +367,19 @@
 
         # Detect if the send_lines key is already being sent to the player.
         # If the caller of this function forgot to specify a key (thus,
         # 'unknown' is used as per the default), we'll skip this detection.
         if key != 'unknown':
             if key in self.current_send_lines_types:
                 log.info(
-                    "Skipped sending lines to '{}': already being sent key "
-                    "'{}'".format(self.printable_name, key))
+                    ("Skipped sending lines to '{name}': already being sent "
+                     "key '{key}'"),
+                    name=self.printable_name,
+                    key=key
+                )
                 return
 
             self.current_send_lines_types.append(key)
 
         current_time = 0
         for line in lines:
             reactor.callLater(current_time, self.send_chat, line)
@@ -379,16 +387,17 @@
 
         reactor.callLater(current_time, self._completed_send_lines, key)
 
     def _completed_send_lines(self, type: str) -> None:
         self.current_send_lines_types.remove(type)
 
     def on_hack_attempt(self, reason):
-        log.warn('Hack attempt detected from {}: {}'
-                 .format(self.printable_name, reason))
+        log.warn('Hack attempt detected from {name}: {reason}',
+                 name=self.printable_name,
+                 reason=reason)
         self.kick(reason)
 
     def on_user_login(self, user_type, verbose=True):
         log.info("'{username}' logged in as {user_type}", username=self.name,
                  user_type=user_type)
 
         if user_type == 'admin':
@@ -408,9 +417,9 @@
         if verbose:
             message = ' logged in as %s' % (user_type)
             self.send_chat('You' + message)
             self.protocol.irc_say("* " + self.name + message)
 
     def timed_out(self):
         if self.name is not None:
-            log.info('%s timed out' % self.printable_name)
+            log.info('{name} timed out', name=self.printable_name)
         ServerConnection.timed_out(self)
```

### Comparing `piqueserver-1.1.1/piqueserver/release.py` & `piqueserver-1.2.0/piqueserver/release.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/run.py` & `piqueserver-1.2.0/piqueserver/run.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scheduler.py` & `piqueserver-1.2.0/piqueserver/scheduler.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/afk.py` & `piqueserver-1.2.0/piqueserver/scripts/afk.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/aimbot2.py` & `piqueserver-1.2.0/piqueserver/scripts/aimbot2.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/airstrike2.py` & `piqueserver-1.2.0/piqueserver/scripts/airstrike2.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/analyze.py` & `piqueserver-1.2.0/piqueserver/scripts/analyze.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/antijerk.py` & `piqueserver-1.2.0/piqueserver/scripts/antijerk.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/autohelp.py` & `piqueserver-1.2.0/piqueserver/scripts/autohelp.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/babel_script.py` & `piqueserver-1.2.0/piqueserver/scripts/babel_script.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/badmin.py` & `piqueserver-1.2.0/piqueserver/scripts/badmin.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/blockinfo.py` & `piqueserver-1.2.0/piqueserver/scripts/blockinfo.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/daycycle.py` & `piqueserver-1.2.0/piqueserver/scripts/daycycle.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/demolitionman.py` & `piqueserver-1.2.0/piqueserver/scripts/demolitionman.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/dirtnade.py` & `piqueserver-1.2.0/piqueserver/scripts/dirtnade.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/disco.py` & `piqueserver-1.2.0/piqueserver/scripts/disco.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/flagreturn.py` & `piqueserver-1.2.0/piqueserver/scripts/flagreturn.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/geoip.py` & `piqueserver-1.2.0/piqueserver/scripts/geoip.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/grownade.py` & `piqueserver-1.2.0/piqueserver/scripts/grownade.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/map_extensions.py` & `piqueserver-1.2.0/piqueserver/scripts/map_extensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Provides extensions to the map metadata (e.g. water damage).
 
-.. codeauthor:: ?
+.. codeauthor:: triplefox, mat^2
 """
 
 
 def apply_script(protocol, connection, config):
     class MapExtensionConnection(connection):
 
         def on_position_update(self):
```

### Comparing `piqueserver-1.1.1/piqueserver/scripts/mapmakingtools.py` & `piqueserver-1.2.0/piqueserver/scripts/mapmakingtools.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/markers.py` & `piqueserver-1.2.0/piqueserver/scripts/markers.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/match.py` & `piqueserver-1.2.0/piqueserver/scripts/match.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/medkit.py` & `piqueserver-1.2.0/piqueserver/scripts/medkit.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/memcheck.py` & `piqueserver-1.2.0/piqueserver/scripts/memcheck.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/minefield.py` & `piqueserver-1.2.0/piqueserver/scripts/minefield.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/nospadingwalls.py` & `piqueserver-1.2.0/piqueserver/scripts/nospadingwalls.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/paint.py` & `piqueserver-1.2.0/piqueserver/scripts/paint.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/passreload.py` & `piqueserver-1.2.0/piqueserver/scripts/passreload.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/protect.py` & `piqueserver-1.2.0/piqueserver/scripts/protect.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/rampage.py` & `piqueserver-1.2.0/piqueserver/scripts/rampage.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/rangedamage.py` & `piqueserver-1.2.0/piqueserver/scripts/rangedamage.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/rapid.py` & `piqueserver-1.2.0/piqueserver/scripts/rapid.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/ratio.py` & `piqueserver-1.2.0/piqueserver/scripts/ratio.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/rollback.py` & `piqueserver-1.2.0/piqueserver/scripts/rollback.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/runningman.py` & `piqueserver-1.2.0/piqueserver/scripts/runningman.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/savemap.py` & `piqueserver-1.2.0/piqueserver/scripts/savemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 
         async def set_map_name(self, rot_info: RotationInfo) -> None:
             if savemap_config.option('always_save_map', False).get():
                 if self.map is not None:
                     self.save_map()
             if savemap_config.option('load_saved_map', False).get():
                 if os.path.isfile(get_path(rot_info.name)):
-                    log.info("Saved version of '%s' found" % rot_info.name)
+                    log.info("Saved version of '{name}' found",
+                             name=rot_info.name)
                     rot_info.name += '.saved'
             await protocol.set_map_name(self, rot_info)
 
         def save_map(self, custom_name=None):
             if custom_name:
                 path = os.path.join(config_dir, 'maps', custom_name) + '.vxl'
             else:
```

### Comparing `piqueserver-1.1.1/piqueserver/scripts/smartnade.py` & `piqueserver-1.2.0/piqueserver/scripts/smartnade.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/spadenadefix.py` & `piqueserver-1.2.0/piqueserver/scripts/spadenadefix.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/spawn_protect.py` & `piqueserver-1.2.0/piqueserver/scripts/spawn_protect.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/spectatorcontrol.py` & `piqueserver-1.2.0/piqueserver/scripts/spectatorcontrol.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/squad.py` & `piqueserver-1.2.0/piqueserver/scripts/squad.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/strongblock.py` & `piqueserver-1.2.0/piqueserver/scripts/strongblock.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/timedmute.py` & `piqueserver-1.2.0/piqueserver/scripts/timedmute.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/trusted.py` & `piqueserver-1.2.0/piqueserver/scripts/trusted.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/votekick.py` & `piqueserver-1.2.0/piqueserver/scripts/votekick.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,21 +57,21 @@
 S_RESULT_BANNED = 'Banned by admin'
 S_RESULT_KICKED = 'Kicked by admin'
 S_RESULT_INSTIGATOR_KICKED = 'Instigator kicked by admin'
 S_RESULT_LEFT = '{victim} (#{victim_id}) left during votekick'
 S_RESULT_INSTIGATOR_LEFT = 'Instigator {instigator} (#{instigator_id}) left'
 S_RESULT_PASSED = 'Player kicked'
 S_ANNOUNCE_IRC = '* {instigator} (#{instigator_id}) started a votekick' \
-    'against player {victim} (#{victim_id}). Reason: {reason}'
+    ' against player {victim} (#{victim_id}). Reason: {reason}'
 S_ANNOUNCE = '{instigator} (#{instigator_id}) started a VOTEKICK against' \
-    '{victim} (#{victim_id}). Say /Y to agree'
+    ' {victim} (#{victim_id}). Say /Y to agree'
 S_ANNOUNCE_SELF = 'You started a votekick against {victim} ({victim_id}).'\
     ' Say /CANCEL to stop it'
 S_UPDATE = '{instigator} (#{instigator_id}) is votekicking' \
-    '{victim} (#{victim_id}). /Y to vote ({needed} left)'
+    ' {victim} (#{victim_id}). /Y to vote ({needed} left)'
 S_REASON = 'Reason: {reason}'
 
 # register options
 VOTEKICK_CONFIG = config.section('votekick')
 REQUIRED_PERCENTAGE_OPTION = VOTEKICK_CONFIG.option('percentage', 35.0)
 BAN_DURATION_OPTION = VOTEKICK_CONFIG.option(
     'ban_duration', default="30min", cast=cast_duration)
```

### Comparing `piqueserver-1.1.1/piqueserver/scripts/votemap.py` & `piqueserver-1.2.0/piqueserver/scripts/votemap.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/welcome.py` & `piqueserver-1.2.0/piqueserver/scripts/welcome.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/scripts/zoc.py` & `piqueserver-1.2.0/piqueserver/scripts/zoc.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/server.py` & `piqueserver-1.2.0/piqueserver/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from piqueserver.networkdict import NetworkDict
 from piqueserver.player import FeatureConnection
 from piqueserver.release import check_for_releases, format_release
 from piqueserver.scheduler import Scheduler
 from piqueserver.utils import as_deferred, EndCall
 from piqueserver.bansubscribe import bans_config_urls
 from pyspades.bytes import NoDataLeft
-from pyspades.constants import CTF_MODE, ERROR_SHUTDOWN, TC_MODE
+from pyspades.constants import CTF_MODE, ERROR_SHUTDOWN, TC_MODE, EXTENSION_CHATTYPE
 from pyspades.master import MAX_SERVER_NAME_SIZE
 from pyspades.server import ServerProtocol, Team
 from pyspades.tools import make_server_identifier
 from pyspades.vxl import VXLData
 
 log = Logger()
 
@@ -255,47 +255,53 @@
             observers = [
                 FilteringLogObserver(
                     textFileLogObserver(sys.stderr), [predicate]),
                 FilteringLogObserver(
                     textFileLogObserver(logging_file), [predicate])
             ]
             globalLogBeginner.beginLoggingTo(observers)
-            log.info('piqueserver started on %s' % time.strftime('%c'))
+            log.info('piqueserver started on {time}', time=time.strftime('%c'))
 
         self.config = config_dict
         if random_rotation.get():
             self.map_rotator_type = random_choice_cycle
         else:
             self.map_rotator_type = itertools.cycle
         self.default_time_limit = default_time_limit.get()
         self.default_cap_limit = cap_limit.get()
         self.advance_on_win = int(advance_on_win.get())
         self.win_count = itertools.count(1)
         self.bans = NetworkDict()
 
+        self.available_proto_extensions = [(EXTENSION_CHATTYPE, 1)]
+
         # attempt to load a saved bans list
         try:
             with open(os.path.join(config.config_dir, bans_file.get()), 'r') as f:
                 self.bans.read_list(json.load(f))
             log.debug("loaded {count} bans", count=len(self.bans))
         except FileNotFoundError:
             log.debug("skip loading bans: file unavailable",
                       count=len(self.bans))
         except IOError as e:
-            log.error('Could not read bans file ({}): {}'.format(
-                bans_file.get(), e))
+            log.error('Could not read bans file ({path}): {exception!r}',
+                      path=bans_file.get(),
+                      exception=e)
         except ValueError as e:
-            log.error('Could not parse bans file ({}): {}'.format(
-                bans_file.get(), e))
+            log.error('Could not parse bans file ({path}): {exception!r}',
+                      path=bans_file.get(),
+                      exception=e)
 
         self.hard_bans = set()  # possible DDoS'ers are added here
         self.player_memory = deque(maxlen=100)
         if len(self.name) > MAX_SERVER_NAME_SIZE:
-            log.warn('(server name too long; it will be truncated to "%s")' % (
-                self.name[:MAX_SERVER_NAME_SIZE]))
+            log.warn(
+                '(server name too long; it will be truncated to "{name}")',
+                name=self.name[:MAX_SERVER_NAME_SIZE]
+            )
         self.respawn_time = respawn_time_option.get()
         self.respawn_waves = respawn_waves.get()
 
         # since AoS only supports CTF and TC at a protocol level, we need to get
         # the base game mode if we are using a custom game mode.
         game_mode_name = game_mode.get()
         if game_mode_name == 'ctf':
@@ -374,15 +380,16 @@
         self.port = port_option.get()
         ServerProtocol.__init__(self, self.port, interface)
         self.host.intercept = self.receive_callback
 
         try:
             self.set_map_rotation(self.config['rotation'])
         except MapNotFound as e:
-            log.critical('Invalid map in map rotation (%s), exiting.' % e.map)
+            log.critical('Invalid map in map rotation ({name}), exiting.',
+                         name=e.map)
             raise SystemExit
 
         map_load_d = self.advance_rotation()
         # discard the result of the map advance for now
         map_load_d.addCallback(lambda x: self._post_init())
 
         ip_getter = ip_getter_option.get()
@@ -410,15 +417,19 @@
             reactor.callLater(self.tip_frequency * 60, self.send_tip)
 
         self.master = register_master_option.get()
         self.set_master()
 
     async def get_external_ip(self, ip_getter: str) -> Iterator[Deferred]:
         log.info(
-            'Retrieving external IP from {!r} to generate server identifier.'.format(ip_getter))
+            ('Retrieving external IP from {ip_getter} to generate server'
+             ' identifier.'),
+            ip_getter=ip_getter
+        )
+
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(ip_getter) as response:
                     ip = await response.text()
                     ip = IPv4Address(ip.strip())
         except AddressValueError as e:
             log.warn('External IP getter service returned invalid data.\n'
@@ -426,16 +437,20 @@
             return
         except Exception as e:  # pylint: disable=broad-except
             log.warn("Getting external IP failed: {reason}", reason=e)
             return
 
         self.ip = ip
         self.identifier = make_server_identifier(ip, self.port)
-        log.info('Server public ip address: {}:{}'.format(ip, self.port))
-        log.info('Public aos identifier: {}'.format(self.identifier))
+        log.info('Server public ip address: {ip}:{port}',
+                 ip=ip,
+                 port=self.port)
+
+        log.info('Public aos identifier: {identifier}',
+                 identifier=self.identifier)
 
     def set_time_limit(self, time_limit: Optional[int] = None, additive:
                        bool = False) -> Optional[int]:
         advance_call = self.advance_call
         add_time = 0.0
         if advance_call is not None:
             add_time = ((advance_call.getTime() - reactor.seconds()) / 60.0)
@@ -610,15 +625,16 @@
     def master_disconnected(self, client=None):
         ServerProtocol.master_disconnected(self, client)
         if self.master and self.master_reconnect_call is None:
             if client:
                 message = 'Master connection could not be established'
             else:
                 message = 'Master connection lost'
-            log.info('%s, reconnecting in 60 seconds...' % message)
+            log.info('{message}, reconnecting in 60 seconds...',
+                     message=message)
             self.master_reconnect_call = reactor.callLater(
                 60, self.reconnect_master)
 
     def reconnect_master(self):
         self.master_reconnect_call = None
         self.set_master()
 
@@ -685,15 +701,15 @@
 
     async def watch_for_releases(self):
         """Starts a loop for `check_for_releases` and updates `self.new_release`."""
         while True:
             self.new_release = await check_for_releases()
             if self.new_release:
                 log.info("#" * 60)
-                log.info(format_release(self.new_release))
+                log.info("{text}", text=format_release(self.new_release))
                 log.info("#" * 60)
             await asyncio.sleep(86400)  # 24 hrs
 
     def vacuum_bans(self):
         """remove any bans that might have expired. This takes a while, so it is
         split up over the event loop"""
 
@@ -765,15 +781,16 @@
                     map_name = "loading..."
                 entry = {
                     "name": self.name,
                     "players_current": self.get_player_count(),
                     "players_max": self.max_players,
                     "map": map_name,
                     "game_mode": self.get_mode_name(),
-                    "game_version": "0.75"
+                    "game_version": "0.75",
+                    "extensions": self.available_proto_extensions
                 }
                 payload = json.dumps(entry).encode()
                 self.host.socket.send(address, payload)
                 return 1
 
             # This drop the connection of any ip in hard_bans
             if address.host in self.hard_bans:
@@ -789,21 +806,25 @@
         current_time = reactor.seconds()
         try:
             ServerProtocol.data_received(self, peer, packet)
         except (NoDataLeft, ValueError):
             import traceback
             traceback.print_exc()
             log.info(
-                'IP %s was hardbanned for invalid data or possibly DDoS.' % ip)
+                'IP {ip} was hardbanned for invalid data or possibly DDoS.',
+                ip=ip
+            )
             self.hard_bans.add(ip)
             return
         dt = reactor.seconds() - current_time
         if dt > 1.0:
-            log.warn('processing {!r} from {} took {}'.format(
-                packet.data, ip, dt))
+            log.warn('processing {data!r} from {ip} took {time}',
+                     data=packet.data,
+                     ip=ip,
+                     time=dt)
 
     def irc_say(self, msg: str, me: bool = False) -> None:
         if self.irc_relay:
             if me:
                 self.irc_relay.me(msg, do_filter=True)
             else:
                 self.irc_relay.send(msg, do_filter=True)
@@ -835,22 +856,24 @@
 
     def update_world(self):
         last_time = self.last_time
         current_time = reactor.seconds()
         if last_time is not None:
             dt = current_time - last_time
             if dt > 1.0:
-                log.warn('high CPU usage detected - %s' % dt)
+                log.warn('high CPU usage detected - {dt}', dt=dt)
         self.last_time = current_time
         ServerProtocol.update_world(self)
         time_taken = reactor.seconds() - current_time
         if time_taken > 1.0:
             log.warn(
-                'World update iteration took %s, objects: %s' %
-                (time_taken, self.world.objects))
+                'World update iteration took {time}, objects: {objects!r}',
+                time=time_taken,
+                objects=self.world.objects
+            )
 
     # events
 
     def on_map_change(self, the_map: VXLData) -> None:
         self.set_fog_color(
             getattr(self.map_info.info, 'fog', self.default_fog)
         )
```

### Comparing `piqueserver-1.1.1/piqueserver/ssh.py` & `piqueserver-1.2.0/piqueserver/ssh.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/statistics.py` & `piqueserver-1.2.0/piqueserver/statistics.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/statusserver.py` & `piqueserver-1.2.0/piqueserver/statusserver.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/utils/_async.py` & `piqueserver-1.2.0/piqueserver/utils/_async.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/utils/_timeparse.py` & `piqueserver-1.2.0/piqueserver/utils/_timeparse.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver/web/templates/status.html` & `piqueserver-1.2.0/piqueserver/web/templates/status.html`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/piqueserver.egg-info/PKG-INFO` & `piqueserver-1.2.0/piqueserver.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqueserver
-Version: 1.1.1
+Version: 1.2.0
 Summary: Open-Source server implementation for Ace of Spades 
 Home-page: https://github.com/piqueserver/piqueserver
 Author: Originally MatPow2 and PySnip contributors,now, StackOverflow and piqueserver authors
 Author-email: nate.shoffner@gmail.com
 Maintainer: noway421
 Maintainer-email: noway@2ch.hk
 License: GNU General Public License v3
@@ -23,18 +23,29 @@
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Twisted
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: First Person Shooters
 Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
-Provides-Extra: from
-Provides-Extra: ssh
 License-File: LICENSE
 License-File: COPYING.txt
+Requires-Dist: pypiwin32; platform_system == "Windows"
+Requires-Dist: Cython<1,>=0.27
+Requires-Dist: Twisted[tls]
+Requires-Dist: Jinja2<4,>=2
+Requires-Dist: Pillow<11,>=5.1.0
+Requires-Dist: aiohttp<3.8.0,>=3.3.0
+Requires-Dist: pyenet
+Requires-Dist: toml
+Requires-Dist: packaging>=19.0
+Provides-Extra: from
+Requires-Dist: geoip2<5.0,>=2.9; extra == "from"
+Provides-Extra: ssh
+Requires-Dist: Twisted[conch,tls]; extra == "ssh"
 
 piqueserver |Build Status| |Wheel Status| |Coverage Status|
 ===========================================================
 
 An Ace of Spades 0.75 server based on
 `PySnip <https://github.com/NateShoffner/PySnip>`__.
```

### Comparing `piqueserver-1.1.1/piqueserver.egg-info/SOURCES.txt` & `piqueserver-1.2.0/piqueserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/__init__.py` & `piqueserver-1.2.0/pyspades/__init__.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/bytes.pxd` & `piqueserver-1.2.0/pyspades/bytes.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/bytes.pyx` & `piqueserver-1.2.0/pyspades/bytes.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/bytes_c.cpp` & `piqueserver-1.2.0/pyspades/bytes_c.cpp`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/classicgen_c.cpp` & `piqueserver-1.2.0/pyspades/classicgen_c.cpp`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/collision.py` & `piqueserver-1.2.0/pyspades/collision.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/color.py` & `piqueserver-1.2.0/pyspades/color.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/common.pxd` & `piqueserver-1.2.0/pyspades/common.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/common.pyx` & `piqueserver-1.2.0/pyspades/common.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/constants.py` & `piqueserver-1.2.0/pyspades/constants.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/contained.pyx` & `piqueserver-1.2.0/pyspades/contained.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/entities.py` & `piqueserver-1.2.0/pyspades/entities.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/gamemodes.py` & `piqueserver-1.2.0/pyspades/gamemodes.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/loaders.pxd` & `piqueserver-1.2.0/pyspades/loaders.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/loaders.pyx` & `piqueserver-1.2.0/pyspades/loaders.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/mapgenerator.py` & `piqueserver-1.2.0/pyspades/mapgenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The map generator is responsible for generating the map bytes that get sent
 to the client on connect
 """
 import zlib
 
-COMPRESSION_LEVEL = 9
+COMPRESSION_LEVEL = 5
 
 
 class ProgressiveMapGenerator:
     """
     Progressively generates the stream of bytes sent to the client for map
     downloads.
```

### Comparing `piqueserver-1.1.1/pyspades/mapmaker.pyx` & `piqueserver-1.2.0/pyspades/mapmaker.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/master.py` & `piqueserver-1.2.0/pyspades/master.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/packet.pyx` & `piqueserver-1.2.0/pyspades/packet.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/player.py` & `piqueserver-1.2.0/pyspades/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,19 @@
     @register_packet_handler(loaders.ShortPlayerData)
     def on_new_player_recieved(self, contained: loaders.ExistingPlayer) -> None:
         if self.team is not None and not self.team.spectator:
             # This player has already joined the game as a full player.
             # Existingplayer may only be sent if in the limbo or spectator
             # modes. Without this check, they could respawn themselves
             # instantly on any team they wanted.
-            log.debug("{} tried sending an ExistingPlayer packet while not in"
-                      " limbo or spectator mode".format(self))
+            log.debug(
+                ("{player!r} tried sending an ExistingPlayer packet while not"
+                 " in limbo or spectator mode"),
+                player=self
+            )
             return
 
         old_team = self.team
         team = self.protocol.teams[contained.team]
         log.debug("{user} wants to join {team}",
                   user=self, team=team, teamid=contained.team)
 
@@ -414,17 +417,21 @@
             return
         self.grenades -= 1
         if not self.check_speedhack(*contained.position):
             contained.position = self.world_object.position.get()
         if contained.value > 3.0:
             contained.value = 3.0
         velocity = Vertex3(*contained.velocity) - self.world_object.velocity
-        if velocity.length() > 2.0:  # cap at tested maximum
+        length = velocity.length()
+        if check_nan(length):
+            return
+        if length > 2.0:  # cap at tested maximum
             velocity = velocity.normal() * 2.0
         velocity += self.world_object.velocity
+        contained.velocity = (velocity.x, velocity.y, velocity.z)
         if self.on_grenade(contained.value) == False:
             return
         grenade = self.protocol.world.create_object(
             world.Grenade, contained.value,
             Vertex3(*contained.position), None,
             velocity, self.grenade_exploded)
         grenade.team = self.team
@@ -626,16 +633,18 @@
     @register_packet_handler(loaders.ChatMessage)
     def on_chat_message_recieved(self, contained: loaders.ChatMessage) -> None:
         if not self.name:
             return
 
         value = contained.value
         if len(value) > 108:
-            log.info("TOO LONG MESSAGE (%i chars) FROM %s (#%i)" %
-                     (len(value), self.name, self.player_id))
+            log.info("TOO LONG MESSAGE ({chars} chars) FROM {name} (#{id})",
+                     chars=len(value),
+                     name=self.name,
+                     id=self.player_id)
 
         value = value[:108]
         if value.startswith('/'):
             self.on_command(*parse_command(value[1:]))
         else:
             global_message = contained.chat_type == CHAT_ALL
             result = self.on_chat(value, global_message)
@@ -712,16 +721,17 @@
 
         # send extension info to clients that support this packet.
         # skip openspades <= 0.1.3 https://github.com/piqueserver/piqueserver/issues/504
         if contained.client == 'o' and contained.version <= (0, 1, 3):
             log.debug("not sending version request to OpenSpades <= 0.1.3")
         else:
             ext_info = loaders.ProtocolExtensionInfo()
-            ext_info.extensions = []
+            ext_info.extensions = self.protocol.available_proto_extensions
             self.send_contained(ext_info)
+        self.on_client_info()
 
     @property
     def client_string(self):
         client = self.client_info.get("client", "Unknown")
         os = self.client_info.get("os_info", "Unknown")
         version = self.client_info.get("version", None)
         version_string = "Unknown" if version is None else ".".join(
@@ -971,24 +981,25 @@
 
     def hit(self, value, by=None, kill_type=WEAPON_KILL):
         if self.hp is None:
             return
         if by is not None and self.team is by.team:
             friendly_fire = self.protocol.friendly_fire
             friendly_fire_on_grief = self.protocol.friendly_fire_on_grief
-            if friendly_fire_on_grief and not friendly_fire:
-                if (kill_type == MELEE_KILL and
-                        not self.protocol.spade_teamkills_on_grief):
-                    return
-                hit_time = self.protocol.friendly_fire_time
-                if (self.last_block_destroy is None
-                        or reactor.seconds() - self.last_block_destroy >= hit_time):
-                    return
             if not friendly_fire:
-                return
+                if friendly_fire_on_grief:
+                    if (kill_type == MELEE_KILL and
+                            not self.protocol.spade_teamkills_on_grief):
+                        return
+                    hit_time = self.protocol.friendly_fire_time
+                    if (self.last_block_destroy is None
+                            or reactor.seconds() - self.last_block_destroy >= hit_time):
+                        return
+                else:
+                    return
         self.set_hp(self.hp - value, by, kill_type=kill_type)
 
     def set_hp(self, value: Union[int, float], hit_by: Optional['ServerConnection'] = None, kill_type: int = WEAPON_KILL,
                hit_indicator: Optional[Tuple[float, float, float]] = None, grenade: Optional[world.Grenade] = None) -> None:
         value = int(value)
         self.hp = max(0, min(100, value))
         if self.hp <= 0:
@@ -1408,12 +1419,15 @@
 
     def on_walk_update(self, up: bool, down: bool, left: bool, right: bool) -> None:
         pass
 
     def on_animation_update(self, jump, crouch, sneak, sprint):
         pass
 
+    def on_client_info(self):
+        pass
+
     def __repr__(self):
         return "<{} player_id: {!r}, name: {!r}, address: {!r} at 0x{:x}>".format(
             self.__class__.__name__, self.player_id, self.name, self.address,
             id(self)
         )
```

### Comparing `piqueserver-1.1.1/pyspades/protocol.py` & `piqueserver-1.2.0/pyspades/protocol.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/server.py` & `piqueserver-1.2.0/pyspades/server.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/team.py` & `piqueserver-1.2.0/pyspades/team.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/tools.py` & `piqueserver-1.2.0/pyspades/tools.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/types.py` & `piqueserver-1.2.0/pyspades/types.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/vxl.pxd` & `piqueserver-1.2.0/pyspades/vxl.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/vxl.pyx` & `piqueserver-1.2.0/pyspades/vxl.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/vxl_c.cpp` & `piqueserver-1.2.0/pyspades/vxl_c.cpp`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/vxl_c.h` & `piqueserver-1.2.0/pyspades/vxl_c.h`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/weapon.py` & `piqueserver-1.2.0/pyspades/weapon.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/world.pyx` & `piqueserver-1.2.0/pyspades/world.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/pyspades/world_c.cpp` & `piqueserver-1.2.0/pyspades/world_c.cpp`

 * *Files identical despite different names*

### Comparing `piqueserver-1.1.1/setup.py` & `piqueserver-1.2.0/setup.py`

 * *Files identical despite different names*

