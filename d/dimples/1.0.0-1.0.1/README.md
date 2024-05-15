# Comparing `tmp/dimples-1.0.0.tar.gz` & `tmp/dimples-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-1.0.0.tar", last modified: Fri May 10 15:58:45 2024, max compression
+gzip compressed data, was "dist/dimples-1.0.1.tar", last modified: Tue May 14 16:43:06 2024, max compression
```

## Comparing `dimples-1.0.0.tar` & `dimples-1.0.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-10 15:58:45.000000 dimples-1.0.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-1.0.0/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-1.0.0/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-1.0.0/dimples/client/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10946 2024-05-07 03:48:04.000000 dimples-1.0.0/dimples/client/archivist.py
--rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-1.0.0/dimples/client/checkpoint.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-1.0.0/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1952 2024-05-07 03:28:52.000000 dimples-1.0.0/dimples/client/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-1.0.0/dimples/client/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     9096 2024-05-07 16:12:33.000000 dimples-1.0.0/dimples/client/cpu/group.py
--rw-r--r--   0 moky       (501) staff       (20)     2173 2024-05-07 03:32:12.000000 dimples-1.0.0/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     5937 2024-05-07 03:34:38.000000 dimples-1.0.0/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3998 2024-05-07 03:35:17.000000 dimples-1.0.0/dimples/client/cpu/grp_join.py
--rw-r--r--   0 moky       (501) staff       (20)     4177 2024-05-07 03:35:53.000000 dimples-1.0.0/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     4388 2024-05-07 03:36:21.000000 dimples-1.0.0/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     5711 2024-05-07 03:36:56.000000 dimples-1.0.0/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     4086 2024-05-07 03:37:19.000000 dimples-1.0.0/dimples/client/cpu/grp_resign.py
--rw-r--r--   0 moky       (501) staff       (20)     5184 2024-05-07 03:50:13.000000 dimples-1.0.0/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     6404 2024-05-06 19:03:39.000000 dimples-1.0.0/dimples/client/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     9059 2024-05-07 03:49:36.000000 dimples-1.0.0/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-1.0.0/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7030 2024-05-09 20:14:55.000000 dimples-1.0.0/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     9331 2024-05-09 16:38:52.000000 dimples-1.0.0/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-1.0.0/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     9296 2024-05-07 03:57:08.000000 dimples-1.0.0/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6077 2024-05-07 04:00:01.000000 dimples-1.0.0/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5525 2024-05-09 19:49:02.000000 dimples-1.0.0/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-1.0.0/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-1.0.0/dimples/common/anonymous.py
--rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-1.0.0/dimples/common/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     7930 2024-05-06 18:08:29.000000 dimples-1.0.0/dimples/common/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/compat/
--rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-1.0.0/dimples/common/compat/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-1.0.0/dimples/common/compat/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-1.0.0/dimples/common/compat/compatible.py
--rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-1.0.0/dimples/common/compat/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-1.0.0/dimples/common/compat/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-1.0.0/dimples/common/compat/network.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-1.0.0/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7648 2024-05-06 18:49:56.000000 dimples-1.0.0/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2735 2024-05-06 18:36:11.000000 dimples-1.0.0/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     8007 2024-05-06 18:03:43.000000 dimples-1.0.0/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8591 2024-05-07 18:41:02.000000 dimples-1.0.0/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     9209 2024-05-07 18:48:04.000000 dimples-1.0.0/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     8616 2024-05-06 18:15:14.000000 dimples-1.0.0/dimples/common/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     2999 2024-05-07 18:46:08.000000 dimples-1.0.0/dimples/common/processer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-1.0.0/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-1.0.0/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-1.0.0/dimples/common/protocol/block.py
--rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-1.0.0/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-1.0.0/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-1.0.0/dimples/common/protocol/mute.py
--rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-1.0.0/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6346 2024-05-06 18:17:07.000000 dimples-1.0.0/dimples/common/register.py
--rw-r--r--   0 moky       (501) staff       (20)     4591 2024-05-07 18:47:41.000000 dimples-1.0.0/dimples/common/session.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-1.0.0/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10934 2024-05-07 17:49:30.000000 dimples-1.0.0/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)    12254 2024-05-10 05:26:49.000000 dimples-1.0.0/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10800 2024-05-07 16:01:10.000000 dimples-1.0.0/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7992 2024-05-07 16:02:25.000000 dimples-1.0.0/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-1.0.0/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-1.0.0/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     6444 2024-04-24 03:34:40.000000 dimples-1.0.0/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-1.0.0/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     4261 2024-05-07 18:47:41.000000 dimples-1.0.0/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     7910 2024-05-09 16:38:10.000000 dimples-1.0.0/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-1.0.0/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8179 2024-05-06 18:51:03.000000 dimples-1.0.0/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-1.0.0/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-1.0.0/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     6360 2024-05-06 18:30:09.000000 dimples-1.0.0/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5247 2024-05-06 18:21:39.000000 dimples-1.0.0/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     6045 2024-05-06 18:50:27.000000 dimples-1.0.0/dimples/database/dos/group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     2789 2024-05-06 18:39:54.000000 dimples-1.0.0/dimples/database/dos/group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     3101 2024-05-06 18:24:21.000000 dimples-1.0.0/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2646 2024-05-06 18:24:29.000000 dimples-1.0.0/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5553 2024-05-06 18:24:46.000000 dimples-1.0.0/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8045 2024-05-06 18:26:43.000000 dimples-1.0.0/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     2941 2024-05-06 18:27:02.000000 dimples-1.0.0/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3760 2024-05-06 18:51:40.000000 dimples-1.0.0/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4436 2024-05-06 18:53:13.000000 dimples-1.0.0/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     3132 2024-05-06 18:27:39.000000 dimples-1.0.0/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     4147 2024-05-06 18:30:39.000000 dimples-1.0.0/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6567 2024-05-06 18:31:50.000000 dimples-1.0.0/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     5809 2024-05-06 18:50:47.000000 dimples-1.0.0/dimples/database/t_group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     4295 2024-05-06 18:41:59.000000 dimples-1.0.0/dimples/database/t_group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4246 2024-05-06 18:41:59.000000 dimples-1.0.0/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     4405 2024-05-06 18:39:12.000000 dimples-1.0.0/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3756 2024-05-06 18:41:59.000000 dimples-1.0.0/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5909 2024-05-06 18:42:32.000000 dimples-1.0.0/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6845 2024-05-06 18:44:20.000000 dimples-1.0.0/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     3578 2024-05-06 18:45:26.000000 dimples-1.0.0/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    16034 2024-05-09 19:52:12.000000 dimples-1.0.0/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     6071 2024-05-07 17:55:00.000000 dimples-1.0.0/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2848 2024-05-10 14:43:14.000000 dimples-1.0.0/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/group/
--rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-1.0.0/dimples/group/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6217 2024-05-06 18:55:34.000000 dimples-1.0.0/dimples/group/admin.py
--rw-r--r--   0 moky       (501) staff       (20)     7191 2024-05-06 19:06:23.000000 dimples-1.0.0/dimples/group/builder.py
--rw-r--r--   0 moky       (501) staff       (20)     7337 2024-05-06 19:05:04.000000 dimples-1.0.0/dimples/group/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)    12302 2024-05-06 19:12:10.000000 dimples-1.0.0/dimples/group/emitter.py
--rw-r--r--   0 moky       (501) staff       (20)     5275 2024-05-06 18:58:53.000000 dimples-1.0.0/dimples/group/helper.py
--rw-r--r--   0 moky       (501) staff       (20)    16535 2024-05-06 19:16:50.000000 dimples-1.0.0/dimples/group/manager.py
--rw-r--r--   0 moky       (501) staff       (20)     5084 2024-05-06 19:10:38.000000 dimples-1.0.0/dimples/group/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-25 15:20:32.000000 dimples-1.0.0/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10595 2024-05-10 10:25:00.000000 dimples-1.0.0/dimples/register/base.py
--rw-r--r--   0 moky       (501) staff       (20)     8248 2024-05-10 10:25:44.000000 dimples-1.0.0/dimples/register/ext.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3910 2024-05-09 16:40:41.000000 dimples-1.0.0/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     4151 2024-05-07 17:52:52.000000 dimples-1.0.0/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-1.0.0/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7502 2024-05-07 17:25:09.000000 dimples-1.0.0/dimples/server/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-1.0.0/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2729 2024-05-07 04:03:19.000000 dimples-1.0.0/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4857 2024-05-07 04:03:27.000000 dimples-1.0.0/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4035 2024-05-07 04:22:27.000000 dimples-1.0.0/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4234 2024-05-07 04:22:59.000000 dimples-1.0.0/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3539 2024-05-07 04:23:05.000000 dimples-1.0.0/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    17669 2024-05-09 19:47:47.000000 dimples-1.0.0/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4574 2024-05-07 17:29:24.000000 dimples-1.0.0/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6584 2024-05-07 04:15:23.000000 dimples-1.0.0/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)    14023 2024-05-07 18:39:52.000000 dimples-1.0.0/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5453 2024-05-09 19:53:21.000000 dimples-1.0.0/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)    10034 2024-05-10 14:19:20.000000 dimples-1.0.0/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-1.0.0/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-1.0.0/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3029 2024-05-10 14:24:22.000000 dimples-1.0.0/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7433 2024-05-07 17:52:09.000000 dimples-1.0.0/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3755 2024-05-09 16:42:05.000000 dimples-1.0.0/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     4740 2024-05-09 19:46:27.000000 dimples-1.0.0/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6511 2024-05-10 05:25:44.000000 dimples-1.0.0/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-1.0.0/dimples/utils/config.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-1.0.0/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-1.0.0/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3982 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      104 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2024-05-10 15:58:45.000000 dimples-1.0.0/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:58:45.000000 dimples-1.0.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1671 2024-05-10 15:51:37.000000 dimples-1.0.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-14 16:43:06.000000 dimples-1.0.1/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-1.0.1/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-1.0.1/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-1.0.1/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10946 2024-05-07 03:48:04.000000 dimples-1.0.1/dimples/client/archivist.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-1.0.1/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-1.0.1/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1952 2024-05-07 03:28:52.000000 dimples-1.0.1/dimples/client/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-1.0.1/dimples/client/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     9096 2024-05-07 16:12:33.000000 dimples-1.0.1/dimples/client/cpu/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     2173 2024-05-07 03:32:12.000000 dimples-1.0.1/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     5937 2024-05-07 03:34:38.000000 dimples-1.0.1/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3998 2024-05-07 03:35:17.000000 dimples-1.0.1/dimples/client/cpu/grp_join.py
+-rw-r--r--   0 moky       (501) staff       (20)     4177 2024-05-07 03:35:53.000000 dimples-1.0.1/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     4388 2024-05-07 03:36:21.000000 dimples-1.0.1/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     5711 2024-05-07 03:36:56.000000 dimples-1.0.1/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     4086 2024-05-07 03:37:19.000000 dimples-1.0.1/dimples/client/cpu/grp_resign.py
+-rw-r--r--   0 moky       (501) staff       (20)     5184 2024-05-07 03:50:13.000000 dimples-1.0.1/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     6404 2024-05-06 19:03:39.000000 dimples-1.0.1/dimples/client/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9059 2024-05-07 03:49:36.000000 dimples-1.0.1/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-1.0.1/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7030 2024-05-09 20:14:55.000000 dimples-1.0.1/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     9331 2024-05-09 16:38:52.000000 dimples-1.0.1/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-1.0.1/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     9296 2024-05-07 03:57:08.000000 dimples-1.0.1/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6077 2024-05-07 04:00:01.000000 dimples-1.0.1/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5525 2024-05-09 19:49:02.000000 dimples-1.0.1/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-1.0.1/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-1.0.1/dimples/common/anonymous.py
+-rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-1.0.1/dimples/common/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     7930 2024-05-06 18:08:29.000000 dimples-1.0.1/dimples/common/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/common/compat/
+-rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-1.0.1/dimples/common/compat/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-1.0.1/dimples/common/compat/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-1.0.1/dimples/common/compat/compatible.py
+-rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-1.0.1/dimples/common/compat/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-1.0.1/dimples/common/compat/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-1.0.1/dimples/common/compat/network.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-1.0.1/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7648 2024-05-06 18:49:56.000000 dimples-1.0.1/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2735 2024-05-06 18:36:11.000000 dimples-1.0.1/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     8007 2024-05-06 18:03:43.000000 dimples-1.0.1/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8591 2024-05-07 18:41:02.000000 dimples-1.0.1/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     9209 2024-05-07 18:48:04.000000 dimples-1.0.1/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     8616 2024-05-06 18:15:14.000000 dimples-1.0.1/dimples/common/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     2999 2024-05-07 18:46:08.000000 dimples-1.0.1/dimples/common/processer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-1.0.1/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-1.0.1/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-1.0.1/dimples/common/protocol/block.py
+-rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-1.0.1/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-1.0.1/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-1.0.1/dimples/common/protocol/mute.py
+-rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-1.0.1/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     6346 2024-05-06 18:17:07.000000 dimples-1.0.1/dimples/common/register.py
+-rw-r--r--   0 moky       (501) staff       (20)     4591 2024-05-07 18:47:41.000000 dimples-1.0.1/dimples/common/session.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4508 2024-05-14 15:03:49.000000 dimples-1.0.1/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6270 2024-05-14 16:29:47.000000 dimples-1.0.1/dimples/conn/flexible.py
+-rw-r--r--   0 moky       (501) staff       (20)    10956 2024-05-14 15:09:23.000000 dimples-1.0.1/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12264 2024-05-14 15:17:10.000000 dimples-1.0.1/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10810 2024-05-14 15:15:47.000000 dimples-1.0.1/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8002 2024-05-14 15:15:53.000000 dimples-1.0.1/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1916 2024-05-14 15:15:34.000000 dimples-1.0.1/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-1.0.1/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8992 2024-05-14 15:42:00.000000 dimples-1.0.1/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     6444 2024-04-24 03:34:40.000000 dimples-1.0.1/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-1.0.1/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     4294 2024-05-14 15:17:10.000000 dimples-1.0.1/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     7920 2024-05-14 16:13:17.000000 dimples-1.0.1/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-1.0.1/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8179 2024-05-06 18:51:03.000000 dimples-1.0.1/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-1.0.1/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4692 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     6360 2024-05-06 18:30:09.000000 dimples-1.0.1/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5247 2024-05-06 18:21:39.000000 dimples-1.0.1/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     6045 2024-05-06 18:50:27.000000 dimples-1.0.1/dimples/database/dos/group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     2789 2024-05-06 18:39:54.000000 dimples-1.0.1/dimples/database/dos/group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     3101 2024-05-06 18:24:21.000000 dimples-1.0.1/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2646 2024-05-06 18:24:29.000000 dimples-1.0.1/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5553 2024-05-06 18:24:46.000000 dimples-1.0.1/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8045 2024-05-06 18:26:43.000000 dimples-1.0.1/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     2941 2024-05-06 18:27:02.000000 dimples-1.0.1/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3760 2024-05-06 18:51:40.000000 dimples-1.0.1/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4436 2024-05-06 18:53:13.000000 dimples-1.0.1/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     3132 2024-05-06 18:27:39.000000 dimples-1.0.1/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     4147 2024-05-06 18:30:39.000000 dimples-1.0.1/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     6567 2024-05-06 18:31:50.000000 dimples-1.0.1/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5809 2024-05-06 18:50:47.000000 dimples-1.0.1/dimples/database/t_group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4295 2024-05-06 18:41:59.000000 dimples-1.0.1/dimples/database/t_group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4246 2024-05-06 18:41:59.000000 dimples-1.0.1/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     4405 2024-05-06 18:39:12.000000 dimples-1.0.1/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3756 2024-05-06 18:41:59.000000 dimples-1.0.1/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5909 2024-05-06 18:42:32.000000 dimples-1.0.1/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6845 2024-05-06 18:44:20.000000 dimples-1.0.1/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     3578 2024-05-06 18:45:26.000000 dimples-1.0.1/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-1.0.1/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    16034 2024-05-10 16:30:30.000000 dimples-1.0.1/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     6062 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2848 2024-05-10 14:43:14.000000 dimples-1.0.1/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/group/
+-rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-1.0.1/dimples/group/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6217 2024-05-06 18:55:34.000000 dimples-1.0.1/dimples/group/admin.py
+-rw-r--r--   0 moky       (501) staff       (20)     7191 2024-05-06 19:06:23.000000 dimples-1.0.1/dimples/group/builder.py
+-rw-r--r--   0 moky       (501) staff       (20)     7337 2024-05-06 19:05:04.000000 dimples-1.0.1/dimples/group/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12302 2024-05-06 19:12:10.000000 dimples-1.0.1/dimples/group/emitter.py
+-rw-r--r--   0 moky       (501) staff       (20)     5275 2024-05-06 18:58:53.000000 dimples-1.0.1/dimples/group/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)    16535 2024-05-06 19:16:50.000000 dimples-1.0.1/dimples/group/manager.py
+-rw-r--r--   0 moky       (501) staff       (20)     5084 2024-05-06 19:10:38.000000 dimples-1.0.1/dimples/group/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2024-04-25 15:20:32.000000 dimples-1.0.1/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10595 2024-05-10 10:25:00.000000 dimples-1.0.1/dimples/register/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     8248 2024-05-10 10:25:44.000000 dimples-1.0.1/dimples/register/ext.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3901 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     4151 2024-05-07 17:52:52.000000 dimples-1.0.1/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-1.0.1/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7502 2024-05-07 17:25:09.000000 dimples-1.0.1/dimples/server/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-1.0.1/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2729 2024-05-07 04:03:19.000000 dimples-1.0.1/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4857 2024-05-07 04:03:27.000000 dimples-1.0.1/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4035 2024-05-07 04:22:27.000000 dimples-1.0.1/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4234 2024-05-07 04:22:59.000000 dimples-1.0.1/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3539 2024-05-07 04:23:05.000000 dimples-1.0.1/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    17669 2024-05-09 19:47:47.000000 dimples-1.0.1/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     4574 2024-05-07 17:29:24.000000 dimples-1.0.1/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6584 2024-05-07 04:15:23.000000 dimples-1.0.1/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)    14023 2024-05-07 18:39:52.000000 dimples-1.0.1/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5453 2024-05-09 19:53:21.000000 dimples-1.0.1/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     9591 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-1.0.1/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-1.0.1/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-1.0.1/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3029 2024-05-10 14:24:22.000000 dimples-1.0.1/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7424 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3755 2024-05-09 16:42:05.000000 dimples-1.0.1/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:06.000000 dimples-1.0.1/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     4742 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6512 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-1.0.1/dimples/utils/config.py
+-rw-r--r--   0 moky       (501) staff       (20)     7057 2024-05-14 14:54:42.000000 dimples-1.0.1/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-1.0.1/dimples/utils/log.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3980 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      104 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2024-05-14 16:43:05.000000 dimples-1.0.1/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-14 16:43:06.000000 dimples-1.0.1/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1671 2024-05-14 14:54:42.000000 dimples-1.0.1/setup.py
```

### Comparing `dimples-1.0.0/PKG-INFO` & `dimples-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 1.0.0
+Version: 1.0.1
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-1.0.0/README.md` & `dimples-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/__init__.py` & `dimples-1.0.1/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/__init__.py` & `dimples-1.0.1/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/archivist.py` & `dimples-1.0.1/dimples/client/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/checkpoint.py` & `dimples-1.0.1/dimples/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/__init__.py` & `dimples-1.0.1/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/commands.py` & `dimples-1.0.1/dimples/client/cpu/commands.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/creator.py` & `dimples-1.0.1/dimples/client/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/group.py` & `dimples-1.0.1/dimples/client/cpu/group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/grp_expel.py` & `dimples-1.0.1/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/grp_invite.py` & `dimples-1.0.1/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/grp_join.py` & `dimples-1.0.1/dimples/client/cpu/grp_join.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/grp_query.py` & `dimples-1.0.1/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/grp_quit.py` & `dimples-1.0.1/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/grp_reset.py` & `dimples-1.0.1/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/grp_resign.py` & `dimples-1.0.1/dimples/client/cpu/grp_resign.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/cpu/handshake.py` & `dimples-1.0.1/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/facebook.py` & `dimples-1.0.1/dimples/client/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/messenger.py` & `dimples-1.0.1/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/network/__init__.py` & `dimples-1.0.1/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/network/session.py` & `dimples-1.0.1/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/network/state.py` & `dimples-1.0.1/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/network/transition.py` & `dimples-1.0.1/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/packer.py` & `dimples-1.0.1/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/processor.py` & `dimples-1.0.1/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/client/terminal.py` & `dimples-1.0.1/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/__init__.py` & `dimples-1.0.1/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/anonymous.py` & `dimples-1.0.1/dimples/common/anonymous.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/ans.py` & `dimples-1.0.1/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/archivist.py` & `dimples-1.0.1/dimples/common/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/compat/__init__.py` & `dimples-1.0.1/dimples/common/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/compat/btc.py` & `dimples-1.0.1/dimples/common/compat/btc.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/compat/compatible.py` & `dimples-1.0.1/dimples/common/compat/compatible.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/compat/entity.py` & `dimples-1.0.1/dimples/common/compat/entity.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/compat/meta.py` & `dimples-1.0.1/dimples/common/compat/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/compat/network.py` & `dimples-1.0.1/dimples/common/compat/network.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/dbi/__init__.py` & `dimples-1.0.1/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/dbi/account.py` & `dimples-1.0.1/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/dbi/message.py` & `dimples-1.0.1/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/dbi/session.py` & `dimples-1.0.1/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/facebook.py` & `dimples-1.0.1/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/messenger.py` & `dimples-1.0.1/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/packer.py` & `dimples-1.0.1/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/processer.py` & `dimples-1.0.1/dimples/common/processer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/protocol/__init__.py` & `dimples-1.0.1/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/protocol/ans.py` & `dimples-1.0.1/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/protocol/block.py` & `dimples-1.0.1/dimples/common/protocol/block.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/protocol/handshake.py` & `dimples-1.0.1/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/protocol/login.py` & `dimples-1.0.1/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/protocol/mute.py` & `dimples-1.0.1/dimples/common/protocol/mute.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/protocol/report.py` & `dimples-1.0.1/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/register.py` & `dimples-1.0.1/dimples/common/register.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/common/session.py` & `dimples-1.0.1/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/conn/__init__.py` & `dimples-1.0.1/dimples/conn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from udp import ServerHub as UDPServerHub, ClientHub as UDPClientHub
 
 from .protocol import WebSocket, NetMsg, NetMsgHead, NetMsgSeq
 
 from .ws import WSArrival, WSDeparture, WSDocker
 from .mars import MarsStreamArrival, MarsStreamDeparture, MarsStreamDocker
 from .mtp import MTPStreamArrival, MTPStreamDeparture, MTPStreamDocker
+from .flexible import FlexibleDocker
 from .gate import CommonGate, TCPServerGate, TCPClientGate, UDPServerGate, UDPClientGate
 # from .gatekeeper import GateKeeper
 from .queue import MessageWrapper, MessageQueue
 from .session import BaseSession
 
 
 __all__ = [
@@ -103,12 +104,13 @@
 
     #
     #   Network
     #
     'WSArrival', 'WSDeparture', 'WSDocker',
     'MarsStreamArrival', 'MarsStreamDeparture', 'MarsStreamDocker',
     'MTPStreamArrival', 'MTPStreamDeparture', 'MTPStreamDocker',
+    'FlexibleDocker',
     'CommonGate', 'TCPServerGate', 'TCPClientGate', 'UDPServerGate', 'UDPClientGate',
     # 'GateKeeper',
     'MessageWrapper', 'MessageQueue',
     'BaseSession',
 ]
```

### Comparing `dimples-1.0.0/dimples/conn/gate.py` & `dimples-1.0.1/dimples/conn/gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from startrek import Arrival, StarDocker, StarGate
 
 from ..utils import Logging
 
 from .mtp import TransactionID, MTPStreamDocker, MTPHelper
 from .mars import MarsStreamArrival, MarsStreamDocker, MarsHelper
 from .ws import WSDocker
+from .flexible import FlexibleDocker
 
 
 H = TypeVar('H')
 
 
 # noinspection PyAbstractClass
 class CommonGate(StarGate, Logging, Generic[H], ABC):
@@ -108,15 +109,17 @@
                 # set connection for this docker
                 await worker.set_connection(conn)
         return worker
 
     async def send_response(self, payload: bytes, ship: Arrival,
                             remote: SocketAddress, local: Optional[SocketAddress]) -> bool:
         worker = self._get_docker(remote=remote, local=local)
-        if isinstance(worker, MTPStreamDocker):
+        if isinstance(worker, FlexibleDocker):
+            return await worker.send_data(payload=payload)
+        elif isinstance(worker, MTPStreamDocker):
             # sn = TransactionID.from_data(data=ship.sn)
             sn = TransactionID.generate()
             pack = MTPHelper.create_message(body=payload, sn=sn)
             return await worker.send_package(pack=pack)
         elif isinstance(worker, MarsStreamDocker):
             assert isinstance(ship, MarsStreamArrival), 'responding ship error: %s' % ship
             mars = MarsHelper.create_respond(head=ship.package.head, payload=payload)
@@ -200,24 +203,19 @@
 
 class TCPServerGate(CommonGate, Generic[H]):
 
     # Override
     def _create_docker(self, parties: List[bytes],
                        remote: SocketAddress, local: Optional[SocketAddress]) -> Docker:
         count = len(parties)
-        if count == 0:
-            # return MTPStreamDocker(remote=remote, local=local, gate=self)
-            assert False, 'data empty'
-        data = parties[0]
-        for i in range(1, count):
-            data = data + parties[i]
-        if len(data) == 0:
-            assert False, 'data empty'
+        data = b'' if count == 0 else parties[count - 1]
         # check data format before creating docker
-        if MTPStreamDocker.check(data=data):
+        if len(data) == 0:
+            docker = FlexibleDocker(remote=remote, local=local)
+        elif MTPStreamDocker.check(data=data):
             docker = MTPStreamDocker(remote=remote, local=local)
         elif MarsStreamDocker.check(data=data):
             docker = MarsStreamDocker(remote=remote, local=local)
         elif WSDocker.check(data=data):
             docker = WSDocker(remote=remote, local=local)
         else:
             raise LookupError('failed to create docker: %s' % data)
@@ -229,15 +227,15 @@
 
     # Override
     def _create_docker(self, parties: List[bytes],
                        remote: SocketAddress, local: Optional[SocketAddress]) -> Docker:
         count = len(parties)
         if count == 0:
             # return MTPStreamDocker(remote=remote, local=local, gate=self)
-            assert False, 'data empty'
+            assert False, 'data empty: %s -> %s' % (remote, local)
         data = parties[count - 1]
         # check data format before creating docker
         if MTPStreamDocker.check(data=data):
             docker = MTPStreamDocker(remote=remote, local=local)
         else:
             raise LookupError('failed to create docker: %s' % data)
         docker.delegate = self.delegate
```

### Comparing `dimples-1.0.0/dimples/conn/gatekeeper.py` & `dimples-1.0.1/dimples/conn/gatekeeper.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             return True
         # try to push
         ok = await gate.send_ship(ship=wrapper, remote=self.remote_address, local=None)
         if not ok:
             self.error(msg='gate error, failed to send data')
         return ok
 
-    async def _docker_pack(self, payload: bytes, priority: int = 0) -> Departure:
+    async def _docker_pack(self, payload: bytes, priority: int = 0) -> Optional[Departure]:
         docker = await self.gate.fetch_docker([], remote=self.remote_address, local=None)
         assert isinstance(docker, DeparturePacker), 'departure packer error: %s' % docker
         return docker.pack(payload=payload, priority=priority)
 
     def _queue_append(self, msg: ReliableMessage, ship: Departure) -> bool:
         return self.__queue.append(msg=msg, ship=ship)
```

### Comparing `dimples-1.0.0/dimples/conn/mars.py` & `dimples-1.0.1/dimples/conn/mars.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 
     # Override
     async def heartbeat(self):
         # heartbeat by client
         pass
 
     # Override
-    def pack(self, payload: bytes, priority: int = 0) -> Departure:
+    def pack(self, payload: bytes, priority: int = 0) -> Optional[Departure]:
         mars = MarsHelper.create_push(payload=payload)
         return self.create_departure(mars=mars, priority=priority)
 
     @classmethod
     def create_departure(cls, mars: NetMsg, priority: int = 0) -> Departure:
         cmd = mars.head.cmd
         if cmd == NetMsgHead.PUSH_MESSAGE:
```

### Comparing `dimples-1.0.0/dimples/conn/mtp.py` & `dimples-1.0.1/dimples/conn/mtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         return MTPHelper.respond_command(sn=sn, body=body)
 
     # Override
     def _create_message_response(self, sn: TransactionID, pages: int, index: int) -> Package:
         return MTPHelper.respond_message(sn=sn, pages=pages, index=index, body=OK)
 
     # Override
-    def pack(self, payload: bytes, priority: int = 0) -> Departure:
+    def pack(self, payload: bytes, priority: int = 0) -> Optional[Departure]:
         pkg = MTPHelper.create_message(body=payload)
         return self._create_departure(pack=pkg, priority=priority)
 
     @classmethod
     def check(cls, data: bytes) -> bool:
         head, offset = MTPHelper.seek_header(data=Data(buffer=data))
         return head is not None
```

### Comparing `dimples-1.0.0/dimples/conn/protocol/__init__.py` & `dimples-1.0.1/dimples/conn/protocol/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,25 +24,27 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from abc import ABC
+from abc import ABC, abstractmethod
+from typing import Optional
 
 from startrek import Departure
 
 from .ws import WebSocket
 from .mars import NetMsg, NetMsgHead, NetMsgSeq
 
 
 class DeparturePacker(ABC):
 
-    def pack(self, payload: bytes, priority: int = 0) -> Departure:
+    @abstractmethod
+    def pack(self, payload: bytes, priority: int = 0) -> Optional[Departure]:
         raise NotImplemented
 
 
 __all__ = [
 
     'DeparturePacker',
```

### Comparing `dimples-1.0.0/dimples/conn/protocol/mars.py` & `dimples-1.0.1/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/conn/protocol/ws.py` & `dimples-1.0.1/dimples/conn/protocol/ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
                     return None, stream
                 mask = stream[pos:pos+4]
                 pos += 4
             else:
                 mask = None
             # 4. get payload
             if stream_len < pos + msg_len:
-                Log.info(msg='incomplete ws package for payload: %d' % stream_len)
+                Log.info(msg='incomplete ws package for payload: %d, msg len: %d' % (stream_len, msg_len))
                 return None, stream
             payload = stream[pos:pos+msg_len]
             pos += msg_len
             if mask is None:
                 content = payload
             else:
                 content = bytearray()
```

### Comparing `dimples-1.0.0/dimples/conn/queue.py` & `dimples-1.0.1/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/conn/seeker.py` & `dimples-1.0.1/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/conn/session.py` & `dimples-1.0.1/dimples/conn/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,16 @@
     @messenger.setter
     def messenger(self, transceiver: CommonMessenger):
         self.__messenger = None if transceiver is None else weakref.ref(transceiver)
 
     # Override
     async def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
         ship = await self._docker_pack(payload=data, priority=priority)
-        return self._queue_append(msg=msg, ship=ship)
+        if ship is not None:
+            return self._queue_append(msg=msg, ship=ship)
 
     #
     #   Transmitter
     #
 
     # Override
     async def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
```

### Comparing `dimples-1.0.0/dimples/conn/ws.py` & `dimples-1.0.1/dimples/conn/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 
     # Override
     async def heartbeat(self):
         # heartbeat by client
         pass
 
     # Override
-    def pack(self, payload: bytes, priority: int = 0) -> Departure:
+    def pack(self, payload: bytes, priority: int = 0) -> Optional[Departure]:
         req_pack = WebSocket.pack(payload=payload)
         return WSDeparture(package=req_pack, payload=payload, priority=priority)
 
     @classmethod
     def check(cls, data: bytes) -> bool:
         return WebSocket.is_handshake(stream=data)
```

### Comparing `dimples-1.0.0/dimples/database/__init__.py` & `dimples-1.0.1/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/account.py` & `dimples-1.0.1/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/__init__.py` & `dimples-1.0.1/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/base.py` & `dimples-1.0.1/dimples/database/dos/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-import os
 from typing import Optional, Union
 
 from ...utils import template_replace
 from ...utils import Log
-from ...utils import File, TextFile, JSONFile
+from ...utils import Path
+from ...utils import TextFile, JSONFile
 
 
 """
     Root Directory
     ~~~~~~~~~~~~~~
     Directory for MKM database
 """
@@ -65,32 +65,28 @@
             # replace with tag
             return template_replace(template=template, key='PUBLIC', value=self._public)
         elif template.startswith('/') or template.find(':') > 0:
             # absolute path
             return template
         else:
             # relative path
-            return os.path.join(self._public, template)
+            return Path.join(self._public, template)
 
     def private_path(self, template: str):
         """ replace '{PRIVATE}' with private directory """
         tag = '{PRIVATE}'
         if template.startswith(tag):
             # replace with tag
             return template_replace(template=template, key='PRIVATE', value=self._private)
         elif template.startswith('/') or template.find(':') > 0:
             # absolute path
             return template
         else:
             # relative path
-            return os.path.join(self._public, template)
-
-    @classmethod
-    def exists(cls, path: str) -> bool:
-        return File(path=path).exists(path=path)
+            return Path.join(self._public, template)
 
     @classmethod
     def read_text(cls, path: str) -> Optional[str]:
         try:
             return TextFile(path=path).read()
         except Exception as error:
             Log.error(msg='Storage >\t%s' % error)
@@ -119,21 +115,14 @@
     @classmethod
     def append_text(cls, text: str, path: str) -> bool:
         try:
             return TextFile(path=path).append(text=text)
         except Exception as error:
             Log.error(msg='Storage >\t%s' % error)
 
-    @classmethod
-    def remove(cls, path: str) -> bool:
-        try:
-            return File(path=path).remove()
-        except Exception as error:
-            Log.error(msg='Storage >\t%s' % error)
-
     #
     #  Logging
     #
     def debug(self, msg: str):
         Log.debug(msg='[DB] %s >\t%s' % (self.__class__.__name__, msg))
 
     def info(self, msg: str):
```

### Comparing `dimples-1.0.0/dimples/database/dos/document.py` & `dimples-1.0.1/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/group.py` & `dimples-1.0.1/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/group_history.py` & `dimples-1.0.1/dimples/database/dos/group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/group_keys.py` & `dimples-1.0.1/dimples/database/dos/group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/login.py` & `dimples-1.0.1/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/meta.py` & `dimples-1.0.1/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/private.py` & `dimples-1.0.1/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/station.py` & `dimples-1.0.1/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/dos/user.py` & `dimples-1.0.1/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/message.py` & `dimples-1.0.1/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/session.py` & `dimples-1.0.1/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_cipherkey.py` & `dimples-1.0.1/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_document.py` & `dimples-1.0.1/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_group.py` & `dimples-1.0.1/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_group_history.py` & `dimples-1.0.1/dimples/database/t_group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_group_keys.py` & `dimples-1.0.1/dimples/database/t_group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_login.py` & `dimples-1.0.1/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_message.py` & `dimples-1.0.1/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_meta.py` & `dimples-1.0.1/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_private.py` & `dimples-1.0.1/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_station.py` & `dimples-1.0.1/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/database/t_user.py` & `dimples-1.0.1/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/edge/__init__.py` & `dimples-1.0.1/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/edge/octopus.py` & `dimples-1.0.1/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/edge/shared.py` & `dimples-1.0.1/dimples/edge/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 import sys
 import time
 from typing import Optional, Tuple
 
 from dimsdk import ID, Station
 
 from ..utils import Singleton, Config
+from ..utils import Path
 from ..common import AccountDBI, MessageDBI, SessionDBI
 from ..common import ProviderInfo
 from ..database import AccountDatabase, MessageDatabase, SessionDatabase
-from ..database import Storage
 from ..client import ClientSession, ClientFacebook, ClientArchivist
 
 
 @Singleton
 class GlobalVariable:
 
     def __init__(self):
@@ -81,15 +81,15 @@
             ini_file = arg
         else:
             show_help(cmd=cmd, app_name=app_name, default_config=default_config)
             sys.exit(0)
     # check config filepath
     if ini_file is None:
         ini_file = default_config
-    if not Storage.exists(path=ini_file):
+    if not Path.exists(path=ini_file):
         show_help(cmd=cmd, app_name=app_name, default_config=default_config)
         print('')
         print('!!! config file not exists: %s' % ini_file)
         print('')
         sys.exit(0)
     # load config from file
     config = Config.load(file=ini_file)
```

### Comparing `dimples-1.0.0/dimples/edge/start.py` & `dimples-1.0.1/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/__init__.py` & `dimples-1.0.1/dimples/group/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/admin.py` & `dimples-1.0.1/dimples/group/admin.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/builder.py` & `dimples-1.0.1/dimples/group/builder.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/delegate.py` & `dimples-1.0.1/dimples/group/delegate.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/emitter.py` & `dimples-1.0.1/dimples/group/emitter.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/helper.py` & `dimples-1.0.1/dimples/group/helper.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/manager.py` & `dimples-1.0.1/dimples/group/manager.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/group/packer.py` & `dimples-1.0.1/dimples/group/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/register/__init__.py` & `dimples-1.0.1/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/register/base.py` & `dimples-1.0.1/dimples/register/base.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/register/ext.py` & `dimples-1.0.1/dimples/register/ext.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/register/run.py` & `dimples-1.0.1/dimples/register/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 path = os.path.abspath(__file__)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 path = os.path.dirname(path)
 sys.path.insert(0, path)
 
 from dimples.utils import Log, Config
+from dimples.utils import Path
 from dimples.utils import Runner
-from dimples.database import Storage
 
 from dimples.register.shared import GlobalVariable
 from dimples.register.shared import create_database
 from dimples.register.shared import generate, modify
 
 
 #
@@ -89,15 +89,15 @@
             ini_file = arg
         else:
             show_help()
             sys.exit(0)
     # check config filepath
     if ini_file is None:
         ini_file = DEFAULT_CONFIG
-    if not Storage.exists(path=ini_file):
+    if not Path.exists(path=ini_file):
         show_help()
         print('')
         print('!!! config file not exists: %s' % ini_file)
         print('')
         sys.exit(0)
     # load config
     config = Config.load(file=ini_file)
```

### Comparing `dimples-1.0.0/dimples/register/shared.py` & `dimples-1.0.1/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/__init__.py` & `dimples-1.0.1/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/archivist.py` & `dimples-1.0.1/dimples/server/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/cpu/__init__.py` & `dimples-1.0.1/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/cpu/ans.py` & `dimples-1.0.1/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/cpu/document.py` & `dimples-1.0.1/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/cpu/handshake.py` & `dimples-1.0.1/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/cpu/login.py` & `dimples-1.0.1/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/cpu/report.py` & `dimples-1.0.1/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/dispatcher.py` & `dimples-1.0.1/dimples/server/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/messenger.py` & `dimples-1.0.1/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/packer.py` & `dimples-1.0.1/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/processor.py` & `dimples-1.0.1/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/push.py` & `dimples-1.0.1/dimples/server/push.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/session.py` & `dimples-1.0.1/dimples/server/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,23 +33,21 @@
     ~~~~~~~~~~~~~~
 
     for login user
 """
 
 import socket
 import traceback
-import weakref
 from typing import Optional, List, Tuple
 
 from dimsdk import ID, EntityType
 from dimsdk import ReliableMessage
 
 from startrek import Docker, DockerStatus
 from startrek import Arrival, Departure
-from startrek.net.channel import is_closed
 
 from ..utils import Log, Runner
 from ..utils import hex_encode, random_bytes
 from ..utils import get_msg_sig, get_msg_info
 from ..common import SessionDBI, MessageDBI, ReliableMessageDBI
 from ..conn import MessageWrapper
 from ..conn import BaseSession
@@ -81,15 +79,14 @@
                 After received 'offline' command, it will be set to False;
                 and when received 'online' it will be True again.
                 Only push message when it's True.
     """
 
     def __init__(self, remote: Tuple[str, int], sock: socket.socket, database: SessionDBI):
         super().__init__(remote=remote, sock=sock, database=database)
-        self.__sock = weakref.ref(sock)
         self.__key = generate_session_key()
 
     @property
     def key(self) -> str:
         return self.__key
 
     # Override
@@ -105,23 +102,14 @@
     def set_active(self, active: bool, when: float = None) -> bool:
         if super().set_active(active=active, when=when):
             session_change_active(session=self, active=active)
             # load cached message asynchronously
             Runner.async_run(coroutine=load_cached_messages(session=self))
             return True
 
-    @property  # Override
-    def running(self) -> bool:
-        if super().running:
-            # gate = self.gate
-            # conn = gate.get_channel(remote=self.remote_address, local=None)
-            # return not (conn is None or conn.closed)
-            sock = self.__sock()
-            return not (sock is None or is_closed(sock=sock))
-
     # Override
     async def start(self):
         await super().start()
         await self.run()
 
     #
     #   Docker Delegate
```

### Comparing `dimples-1.0.0/dimples/server/session_center.py` & `dimples-1.0.1/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/server/trace.py` & `dimples-1.0.1/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/station/__init__.py` & `dimples-1.0.1/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/station/handler.py` & `dimples-1.0.1/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/station/shared.py` & `dimples-1.0.1/dimples/station/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 import sys
 import time
 from typing import Optional, Tuple
 
 from dimsdk import ID
 
 from ..utils import Singleton, Config
+from ..utils import Path
 from ..common import AddressNameServer, ANSFactory
 from ..common import CommonFacebook, CommonMessenger
 from ..common import AccountDBI, MessageDBI, SessionDBI
 from ..common import ProviderInfo
 from ..database import AccountDatabase, MessageDatabase, SessionDatabase
-from ..database import Storage
 from ..server import ServerArchivist
 from ..server import ServerSession
 from ..server import ServerMessenger
 from ..server import ServerMessagePacker
 from ..server import ServerMessageProcessor
 from ..server import Dispatcher
 
@@ -89,15 +89,15 @@
             ini_file = arg
         else:
             show_help(cmd=cmd, app_name=app_name, default_config=default_config)
             sys.exit(0)
     # check config filepath
     if ini_file is None:
         ini_file = default_config
-    if not Storage.exists(path=ini_file):
+    if not Path.exists(path=ini_file):
         show_help(cmd=cmd, app_name=app_name, default_config=default_config)
         print('')
         print('!!! config file not exists: %s' % ini_file)
         print('')
         sys.exit(0)
     # load config from file
     config = Config.load(file=ini_file)
```

### Comparing `dimples-1.0.0/dimples/station/start.py` & `dimples-1.0.1/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/utils/__init__.py` & `dimples-1.0.1/dimples/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 from dimsdk import Converter
 from dimsdk import DateTime
 from dimsdk import ReliableMessage
 from dimsdk import DocumentHelper
 
 from dimplugins.crypto.aes import random_bytes
 
+from startrek.fsm import Singleton
 from startrek.fsm import Runnable, Runner, Daemon, DaemonRunner
 from startrek.fsm import Delegate as StateDelegate
 from startrek.net.channel import get_remote_address, get_local_address
 
 
-from .singleton import Singleton
 from .log import Log, Logging
 from .dos import Path, File, TextFile, JSONFile
 from .cache import CachePool, CacheHolder, CacheManager
 
 from .config import Config
```

### Comparing `dimples-1.0.0/dimples/utils/cache.py` & `dimples-1.0.1/dimples/utils/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,18 @@
     Database module
     ~~~~~~~~~~~~~~~
 
 """
 
 from typing import TypeVar, Generic, Optional, Dict, Set, Tuple
 
+from startrek.fsm import Singleton
 from startrek.fsm import Runnable, Runner, Daemon
 from dimsdk import DateTime
 
-from .singleton import Singleton
-
 
 K = TypeVar('K')
 V = TypeVar('V')
 
 
 class CacheHolder(Generic[V]):
```

### Comparing `dimples-1.0.0/dimples/utils/config.py` & `dimples-1.0.1/dimples/utils/config.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples/utils/dos.py` & `dimples-1.0.1/dimples/utils/dos.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ~~~~~~~~~~~~~~~~~~~~~
 
     File access
 """
 
 import os
 import sys
-from typing import Union, Optional, AnyStr
+from typing import Optional, Union, AnyStr, Dict, List
 import json
 
 
 class Path:
     """
         Paths for main script
         ~~~~~~~~~~~~~~~~~~~~~
@@ -58,119 +58,170 @@
     @classmethod
     def abs(cls, path: str) -> str:
         # 'file.txt' -> '/home/User/Documents/file.txt'
         return os.path.abspath(path)
 
     @classmethod
     def add(cls, path: str):
+        """ add system path """
         sys.path.insert(0, path)
 
+    """
+        Path Utils
+        ~~~~~~~~~~
+    """
 
-class File:
+    @classmethod
+    def join(cls, parent: str, *children: str) -> str:
+        return os.path.join(parent, *children)
 
-    def __init__(self, path: str):
-        super().__init__()
-        self.__path: str = path
-        self.__data: Optional[AnyStr] = None
+    @classmethod
+    def is_dir(cls, path: str) -> bool:
+        return os.path.isdir(path)
 
     @classmethod
-    def make_dirs(cls, directory: str) -> bool:
-        if os.path.exists(directory):
-            if os.path.isdir(directory):
-                # directory exists
-                return True
-            else:
-                raise IOError('%s exists but is not a directory!' % directory)
-        else:
-            os.makedirs(directory, exist_ok=True)
-            return True
+    def is_file(cls, path: str) -> bool:
+        return os.path.isfile(path)
 
-    def exists(self, path: str = None) -> bool:
-        # param 'path' deprecated
-        if path is None:
-            path = self.__path
+    @classmethod
+    def exists(cls, path: str) -> bool:
         return os.path.exists(path)
 
-    def remove(self, path: str = None) -> bool:
-        if path is None:
-            path = self.__path
+    @classmethod
+    def remove(cls, path: str) -> bool:
         if os.path.exists(path):
             os.remove(path)
             return True
 
-    def read(self, mode: str = 'rb', encoding=None) -> Optional[AnyStr]:
+    @classmethod
+    def make_dirs(cls, directory: str) -> bool:
+        if not os.path.exists(directory):
+            os.makedirs(directory, exist_ok=True)
+            return True
+        elif os.path.isdir(directory):
+            # directory exists
+            return True
+        else:
+            raise IOError('%s exists but is not a directory!' % directory)
+
+
+class File:
+    """ Base File """
+
+    def __init__(self, path: str):
+        super().__init__()
+        self.__path: str = path
+        self.__data: Optional[AnyStr] = None
+
+    @property
+    def path(self) -> str:
+        return self.__path
+
+    def read(self, mode: str = 'rb', encoding: str = None) -> Optional[AnyStr]:
         if self.__data is not None:
             # get data from cache
             return self.__data
-        if not os.path.exists(self.__path):
+        if not Path.exists(path=self.__path):
             # file not found
             return None
-        if not os.path.isfile(self.__path):
+        if not Path.is_file(path=self.__path):
             # the path is not a file
             raise IOError('%s is not a file' % self.__path)
         with open(self.__path, mode=mode, encoding=encoding) as file:
             self.__data = file.read()
         return self.__data
 
-    def write(self, data: AnyStr, mode: str = 'wb', encoding=None) -> bool:
-        directory = os.path.dirname(self.__path)
-        if not self.make_dirs(directory):
+    def write(self, data: AnyStr, mode: str = 'wb', encoding: str = None) -> bool:
+        directory = Path.dir(path=self.__path)
+        if not Path.make_dirs(directory=directory):
             return False
         with open(self.__path, mode=mode, encoding=encoding) as file:
             if len(data) == file.write(data):
                 # OK, update cache
                 self.__data = data
                 return True
 
-    def append(self, data: AnyStr, mode: str = 'ab', encoding=None) -> bool:
-        if not os.path.exists(self.__path):
+    def append(self, data: AnyStr, mode: str = 'ab', encoding: str = None) -> bool:
+        if not Path.exists(path=self.__path):
             # new file
+            if mode is not None:
+                mode = mode.replace('a', 'w')
             return self.write(data, mode=mode)
         # append to exists file
         with open(self.__path, mode=mode, encoding=encoding) as file:
             if len(data) == file.write(data):
                 # OK, erase cache for next update
                 self.__data = None
                 return True
 
 
-class TextFile(File):
+class BinaryFile:
+
+    def __init__(self, path: str):
+        super().__init__()
+        self.__file = File(path=path)
+
+    @property
+    def path(self) -> str:
+        return self.__file.path
+
+    def read(self) -> Optional[bytes]:
+        return self.__file.read(mode='rb')
+
+    def write(self, data: bytes) -> bool:
+        return self.__file.write(data=data, mode='wb')
+
+    def append(self, data: bytes) -> bool:
+        return self.__file.append(data=data, mode='ab')
+
+
+class TextFile:
+
+    def __init__(self, path: str):
+        super().__init__()
+        self.__file = File(path=path)
+
+    @property
+    def path(self) -> str:
+        return self.__file.path
 
-    def read(self, mode: str = 'r', encoding='utf-8') -> Optional[str]:
-        return super().read(mode=mode, encoding=encoding)
+    def read(self, encoding: str = 'utf-8') -> Optional[str]:
+        return self.__file.read(mode='r', encoding=encoding)
 
-    def write(self, text: str, mode: str = 'w', encoding='utf-8') -> bool:
-        return super().write(text, mode=mode, encoding=encoding)
+    def write(self, text: str, encoding: str = 'utf-8') -> bool:
+        return self.__file.write(data=text, mode='w', encoding=encoding)
 
-    def append(self, text: str, mode: str = 'a', encoding='utf-8') -> bool:
-        return super().append(text, mode=mode, encoding=encoding)
+    def append(self, text: str, encoding: str = 'utf-8') -> bool:
+        return self.__file.append(data=text, mode='a', encoding=encoding)
 
 
-class JSONFile(TextFile):
+class JSONFile:
 
     def __init__(self, path: str):
-        super().__init__(path=path)
-        self.__container: Union[dict, list, None] = None
+        super().__init__()
+        self.__file = TextFile(path=path)
+        self.__container: Union[Dict, List, None] = None
+
+    @property
+    def path(self) -> str:
+        return self.__file.path
 
-    def read(self, **kwargs) -> Union[dict, list, None]:
+    def read(self) -> Union[Dict, List, None]:
         if self.__container is not None:
             # get content from cache
             return self.__container
         # read as text file
-        text = super().read()
+        text = self.__file.read()
         if text is not None:
             # convert text string to JSON object
             self.__container = json.loads(text)
         return self.__container
 
-    def write(self, container: Union[dict, list], **kwargs) -> bool:
+    def write(self, container: Union[Dict, List]) -> bool:
         # convert JSON object to text string
         text = json.dumps(container)
         if text is None:
             raise ValueError('cannot convert to JSON string: %s' % container)
-        if super().write(text):
+        if self.__file.write(text=text):
             # OK, update cache
             self.__container = container
             return True
-
-    def append(self, **kwargs) -> bool:
-        raise AssertionError('JSON file cannot be appended')
```

### Comparing `dimples-1.0.0/dimples/utils/log.py` & `dimples-1.0.1/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-1.0.0/dimples.egg-info/PKG-INFO` & `dimples-1.0.1/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 1.0.0
+Version: 1.0.1
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-1.0.0/dimples.egg-info/SOURCES.txt` & `dimples-1.0.1/dimples.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 dimples/common/protocol/ans.py
 dimples/common/protocol/block.py
 dimples/common/protocol/handshake.py
 dimples/common/protocol/login.py
 dimples/common/protocol/mute.py
 dimples/common/protocol/report.py
 dimples/conn/__init__.py
+dimples/conn/flexible.py
 dimples/conn/gate.py
 dimples/conn/gatekeeper.py
 dimples/conn/mars.py
 dimples/conn/mtp.py
 dimples/conn/queue.py
 dimples/conn/seeker.py
 dimples/conn/session.py
@@ -133,9 +134,8 @@
 dimples/station/handler.py
 dimples/station/shared.py
 dimples/station/start.py
 dimples/utils/__init__.py
 dimples/utils/cache.py
 dimples/utils/config.py
 dimples/utils/dos.py
-dimples/utils/log.py
-dimples/utils/singleton.py
+dimples/utils/log.py
```

### Comparing `dimples-1.0.0/setup.py` & `dimples-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

