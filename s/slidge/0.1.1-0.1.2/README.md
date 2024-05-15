# Comparing `tmp/slidge-0.1.1.tar.gz` & `tmp/slidge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slidge-0.1.1.tar", max compression
+gzip compressed data, was "slidge-0.1.2.tar", max compression
```

## Comparing `slidge-0.1.1.tar` & `slidge-0.1.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0    34523 2024-05-12 04:44:15.843167 slidge-0.1.1/LICENSE
--rw-r--r--   0        0        0     3684 2024-05-12 04:44:15.843167 slidge-0.1.1/README.md
--rw-r--r--   0        0        0     2002 2024-05-12 04:44:32.601630 slidge-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1624 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/__init__.py
--rw-r--r--   0        0        0     5804 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/__main__.py
--rw-r--r--   0        0        0      613 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/__init__.py
--rw-r--r--   0        0        0     9188 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/adhoc.py
--rw-r--r--   0        0        0     5759 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/admin.py
--rw-r--r--   0        0        0    13073 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/base.py
--rw-r--r--   0        0        0       99 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/categories.py
--rw-r--r--   0        0        0     9975 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/chat_command.py
--rw-r--r--   0        0        0     6014 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/register.py
--rw-r--r--   0        0        0     8781 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/user.py
--rw-r--r--   0        0        0      191 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/contact/__init__.py
--rw-r--r--   0        0        0    16101 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/contact/contact.py
--rw-r--r--   0        0        0     7489 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/contact/roster.py
--rw-r--r--   0        0        0       68 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/__init__.py
--rw-r--r--   0        0        0     5443 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/cache.py
--rw-r--r--   0        0        0     7392 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/config.py
--rw-r--r--   0        0        0       58 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/__init__.py
--rw-r--r--   0        0        0    34649 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/base.py
--rw-r--r--   0        0        0     1919 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/caps.py
--rw-r--r--   0        0        0     1352 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/delivery_receipt.py
--rw-r--r--   0        0        0     2230 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/disco.py
--rw-r--r--   0        0        0     2471 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/mam.py
--rw-r--r--   0        0        0     1033 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/muc_admin.py
--rw-r--r--   0        0        0     1753 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/ping.py
--rw-r--r--   0        0        0     2732 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/presence.py
--rw-r--r--   0        0        0     1619 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/registration.py
--rw-r--r--   0        0        0     3518 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/search.py
--rw-r--r--   0        0        0    28927 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/session_dispatcher.py
--rw-r--r--   0        0        0     4639 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/vcard_temp.py
--rw-r--r--   0        0        0      368 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/__init__.py
--rw-r--r--   0        0        0    17808 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/attachment.py
--rw-r--r--   0        0        0     5493 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/avatar.py
--rw-r--r--   0        0        0      702 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/base.py
--rw-r--r--   0        0        0     3935 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/disco.py
--rw-r--r--   0        0        0      913 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/lock.py
--rw-r--r--   0        0        0    14790 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/message.py
--rw-r--r--   0        0        0     5606 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/message_maker.py
--rw-r--r--   0        0        0     7216 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/presence.py
--rw-r--r--   0        0        0     1302 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/recipient.py
--rw-r--r--   0        0        0    18268 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/pubsub.py
--rw-r--r--   0        0        0    26134 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/session.py
--rw-r--r--   0        0        0      258 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/__init__.py
--rw-r--r--   0        0        0     3426 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/archive.py
--rw-r--r--   0        0        0     5944 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/bookmarks.py
--rw-r--r--   0        0        0    14862 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/participant.py
--rw-r--r--   0        0        0    38972 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/room.py
--rw-r--r--   0        0        0      334 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/migration.py
--rw-r--r--   0        0        0        0 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/py.typed
--rw-r--r--   0        0        0     1777 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/__init__.py
--rw-r--r--   0        0        0      290 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/link_preview/__init__.py
--rw-r--r--   0        0        0      448 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/link_preview/link_preview.py
--rw-r--r--   0        0        0     2664 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/link_preview/stanza.py
--rw-r--r--   0        0        0     1545 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/roster.py
--rw-r--r--   0        0        0      325 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0077/__init__.py
--rw-r--r--   0        0        0    10431 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0077/register.py
--rw-r--r--   0        0        0     2410 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0077/stanza.py
--rw-r--r--   0        0        0      107 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0100/__init__.py
--rw-r--r--   0        0        0     4501 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0100/gateway.py
--rw-r--r--   0        0        0      232 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0100/stanza.py
--rw-r--r--   0        0        0      319 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0153/__init__.py
--rw-r--r--   0        0        0      735 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0153/stanza.py
--rw-r--r--   0        0        0      658 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0153/vcard_avatar.py
--rw-r--r--   0        0        0      109 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0264/__init__.py
--rw-r--r--   0        0        0      864 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0264/stanza.py
--rw-r--r--   0        0        0      456 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0264/thumbnail.py
--rw-r--r--   0        0        0       98 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0292/__init__.py
--rw-r--r--   0        0        0     3113 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0292/vcard4.py
--rw-r--r--   0        0        0      368 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0313/__init__.py
--rw-r--r--   0        0        0     9211 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0313/mam.py
--rw-r--r--   0        0        0    10249 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0313/stanza.py
--rw-r--r--   0        0        0      104 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0317/__init__.py
--rw-r--r--   0        0        0      290 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0317/hats.py
--rw-r--r--   0        0        0      659 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0317/stanza.py
--rw-r--r--   0        0        0      180 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0356_old/__init__.py
--rw-r--r--   0        0        0     5338 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0356_old/privilege.py
--rw-r--r--   0        0        0     1229 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0356_old/stanza.py
--rw-r--r--   0        0        0      284 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0424/__init__.py
--rw-r--r--   0        0        0     2448 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0424/retraction.py
--rw-r--r--   0        0        0      753 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0424/stanza.py
--rw-r--r--   0        0        0      158 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0490/__init__.py
--rw-r--r--   0        0        0     1527 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0490/mds.py
--rw-r--r--   0        0        0      443 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0490/stanza.py
--rw-r--r--   0        0        0      301 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/__init__.py
--rw-r--r--   0        0        0     1686 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/archive_msg.py
--rw-r--r--   0        0        0     6613 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/conf.py
--rw-r--r--   0        0        0     6604 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/db.py
--rw-r--r--   0        0        0     2682 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/schema.sql
--rw-r--r--   0        0        0    16517 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/sql.py
--rw-r--r--   0        0        0    10688 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/test.py
--rw-r--r--   0        0        0     4689 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/types.py
--rw-r--r--   0        0        0     8587 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/util.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 slidge-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-15 04:30:01.982549 slidge-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3706 2024-05-15 04:30:01.982549 slidge-0.1.2/README.md
+-rw-r--r--   0        0        0     2088 2024-05-15 04:30:17.436757 slidge-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1624 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/__init__.py
+-rw-r--r--   0        0        0     5804 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/__main__.py
+-rw-r--r--   0        0        0      613 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/__init__.py
+-rw-r--r--   0        0        0     9188 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/adhoc.py
+-rw-r--r--   0        0        0     5759 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/admin.py
+-rw-r--r--   0        0        0    13073 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/base.py
+-rw-r--r--   0        0        0       99 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/categories.py
+-rw-r--r--   0        0        0     9975 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/chat_command.py
+-rw-r--r--   0        0        0     6014 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/register.py
+-rw-r--r--   0        0        0     8781 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/user.py
+-rw-r--r--   0        0        0      191 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/contact/__init__.py
+-rw-r--r--   0        0        0    16101 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/contact/contact.py
+-rw-r--r--   0        0        0     7489 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/contact/roster.py
+-rw-r--r--   0        0        0       68 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/__init__.py
+-rw-r--r--   0        0        0     5443 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/cache.py
+-rw-r--r--   0        0        0     7392 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/config.py
+-rw-r--r--   0        0        0       58 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/__init__.py
+-rw-r--r--   0        0        0    34645 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/base.py
+-rw-r--r--   0        0        0     1919 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/caps.py
+-rw-r--r--   0        0        0     1352 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/delivery_receipt.py
+-rw-r--r--   0        0        0     2230 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/disco.py
+-rw-r--r--   0        0        0     2471 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/mam.py
+-rw-r--r--   0        0        0     1033 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/muc_admin.py
+-rw-r--r--   0        0        0     1753 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/ping.py
+-rw-r--r--   0        0        0     2732 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/presence.py
+-rw-r--r--   0        0        0     1619 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/registration.py
+-rw-r--r--   0        0        0     3518 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/search.py
+-rw-r--r--   0        0        0    29193 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/session_dispatcher.py
+-rw-r--r--   0        0        0     4639 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/vcard_temp.py
+-rw-r--r--   0        0        0      368 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/__init__.py
+-rw-r--r--   0        0        0    17808 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/attachment.py
+-rw-r--r--   0        0        0     5493 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/avatar.py
+-rw-r--r--   0        0        0      702 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/base.py
+-rw-r--r--   0        0        0     3935 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/disco.py
+-rw-r--r--   0        0        0      913 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/lock.py
+-rw-r--r--   0        0        0    14790 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/message.py
+-rw-r--r--   0        0        0     5606 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/message_maker.py
+-rw-r--r--   0        0        0     7216 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/presence.py
+-rw-r--r--   0        0        0     1302 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/recipient.py
+-rw-r--r--   0        0        0    18268 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/pubsub.py
+-rw-r--r--   0        0        0    26134 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/session.py
+-rw-r--r--   0        0        0      258 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/__init__.py
+-rw-r--r--   0        0        0     3426 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/archive.py
+-rw-r--r--   0        0        0     5944 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/bookmarks.py
+-rw-r--r--   0        0        0    14908 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/participant.py
+-rw-r--r--   0        0        0    38972 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/room.py
+-rw-r--r--   0        0        0      334 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/migration.py
+-rw-r--r--   0        0        0        0 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/py.typed
+-rw-r--r--   0        0        0     1777 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/link_preview/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/link_preview/link_preview.py
+-rw-r--r--   0        0        0     2664 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/link_preview/stanza.py
+-rw-r--r--   0        0        0     1545 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/roster.py
+-rw-r--r--   0        0        0      325 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0077/__init__.py
+-rw-r--r--   0        0        0    10431 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0077/register.py
+-rw-r--r--   0        0        0     2410 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0077/stanza.py
+-rw-r--r--   0        0        0      107 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0100/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0100/gateway.py
+-rw-r--r--   0        0        0      232 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0100/stanza.py
+-rw-r--r--   0        0        0      319 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0153/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0153/stanza.py
+-rw-r--r--   0        0        0      658 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0153/vcard_avatar.py
+-rw-r--r--   0        0        0      109 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0264/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0264/stanza.py
+-rw-r--r--   0        0        0      456 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0264/thumbnail.py
+-rw-r--r--   0        0        0       98 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0292/__init__.py
+-rw-r--r--   0        0        0     3113 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0292/vcard4.py
+-rw-r--r--   0        0        0      368 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0313/__init__.py
+-rw-r--r--   0        0        0     9211 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0313/mam.py
+-rw-r--r--   0        0        0    10249 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0313/stanza.py
+-rw-r--r--   0        0        0      104 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0317/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0317/hats.py
+-rw-r--r--   0        0        0      659 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0317/stanza.py
+-rw-r--r--   0        0        0      180 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0356_old/__init__.py
+-rw-r--r--   0        0        0     5338 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0356_old/privilege.py
+-rw-r--r--   0        0        0     1229 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0356_old/stanza.py
+-rw-r--r--   0        0        0      284 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0424/__init__.py
+-rw-r--r--   0        0        0     2448 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0424/retraction.py
+-rw-r--r--   0        0        0      753 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0424/stanza.py
+-rw-r--r--   0        0        0      158 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0490/__init__.py
+-rw-r--r--   0        0        0     1527 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0490/mds.py
+-rw-r--r--   0        0        0      443 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0490/stanza.py
+-rw-r--r--   0        0        0      301 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/archive_msg.py
+-rw-r--r--   0        0        0     6613 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/conf.py
+-rw-r--r--   0        0        0     6604 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/db.py
+-rw-r--r--   0        0        0     2682 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/schema.sql
+-rw-r--r--   0        0        0    16517 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/sql.py
+-rw-r--r--   0        0        0    10688 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/test.py
+-rw-r--r--   0        0        0     4689 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/types.py
+-rw-r--r--   0        0        0     8587 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/util.py
+-rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 slidge-0.1.2/PKG-INFO
```

### Comparing `slidge-0.1.1/LICENSE` & `slidge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/README.md` & `slidge-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Slidge logo](./dev/assets/slidge-color-small.png)
+![Slidge logo](https://git.sr.ht/~nicoco/slidge/blob/master/dev/assets/slidge-color-small.png)
 
 [Home](https://sr.ht/~nicoco/slidge) |
 [Docs](https://slidge.im/core) |
 [Source](https://sr.ht/~nicoco/slidge/sources) |
 [Issues](https://sr.ht/~nicoco/slidge/trackers) |
 [Patches](https://lists.sr.ht/~nicoco/public-inbox) |
 [Chat](xmpp:slidge@conference.nicoco.fr?join)
@@ -38,16 +38,15 @@
 If you use debian, you might also be interested in the
 [slidge-debian](https://git.sr.ht/~nicoco/slidge-debian)
 bundle.
 
 Status
 ------
 
-Slidge is **beta**-grade software for 1:1 chats.
-Group chat support is **experimental**.
+Slidge is **beta**-grade software. It support groups and 1:1 chats.
 
 Try slidge and give us some
 feedback, through the [MUC](xmpp:slidge@conference.nicoco.fr?join), the
 [issue tracker](https://todo.sr.ht/~nicoco/slidge) or in the
 [public inbox](https://lists.sr.ht/~nicoco/public-inbox).
 Don't be shy!
```

### Comparing `slidge-0.1.1/pyproject.toml` & `slidge-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [tool.poetry]
 name = "slidge"
-version = "0.1.1"
+version = "0.1.2"
 description = "XMPP bridging framework"
 authors = ["Nicolas Cedilnik <nicoco@nicoco.fr>"]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://sr.ht/~nicoco/slidge/"
+repository = "https://git.sr.ht/~nicoco/slidge/"
+documentation = "https://slidge.im/"
 include = ["slidge/util/schema.sql"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 qrcode = "^7.4.1"
 Pillow = "^10"
 aiohttp = {version = "^3.8.3", extras = ["speedups"]}
```

### Comparing `slidge-0.1.1/slidge/__init__.py` & `slidge-0.1.2/slidge/__init__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/__main__.py` & `slidge-0.1.2/slidge/__main__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/command/__init__.py` & `slidge-0.1.2/slidge/command/__init__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/command/adhoc.py` & `slidge-0.1.2/slidge/command/adhoc.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/command/admin.py` & `slidge-0.1.2/slidge/command/admin.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/command/base.py` & `slidge-0.1.2/slidge/command/base.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/command/chat_command.py` & `slidge-0.1.2/slidge/command/chat_command.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/command/register.py` & `slidge-0.1.2/slidge/command/register.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/command/user.py` & `slidge-0.1.2/slidge/command/user.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/contact/contact.py` & `slidge-0.1.2/slidge/contact/contact.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/contact/roster.py` & `slidge-0.1.2/slidge/contact/roster.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/cache.py` & `slidge-0.1.2/slidge/core/cache.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/config.py` & `slidge-0.1.2/slidge/core/config.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/base.py` & `slidge-0.1.2/slidge/core/gateway/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
 
     async def _on_user_register(self, iq: Iq):
         session = self.get_session_from_stanza(iq)
         for jid in config.ADMINS:
             self.send_message(
                 mto=jid,
                 mbody=f"{iq.get_from()} has registered",
-                mtype="headline",
+                mtype="chat",
                 mfrom=self.boundjid.bare,
             )
         session.send_gateway_message(self.WELCOME_MESSAGE)
         await self.__login_wrap(session)
 
     async def _on_user_unregister(self, iq: Iq):
         await self.session_cls.kill_by_jid(iq.get_from())
```

### Comparing `slidge-0.1.1/slidge/core/gateway/caps.py` & `slidge-0.1.2/slidge/core/gateway/caps.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/delivery_receipt.py` & `slidge-0.1.2/slidge/core/gateway/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/disco.py` & `slidge-0.1.2/slidge/core/gateway/disco.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/mam.py` & `slidge-0.1.2/slidge/core/gateway/mam.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/muc_admin.py` & `slidge-0.1.2/slidge/core/gateway/muc_admin.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/ping.py` & `slidge-0.1.2/slidge/core/gateway/ping.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/presence.py` & `slidge-0.1.2/slidge/core/gateway/presence.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/registration.py` & `slidge-0.1.2/slidge/core/gateway/registration.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/search.py` & `slidge-0.1.2/slidge/core/gateway/search.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/gateway/session_dispatcher.py` & `slidge-0.1.2/slidge/core/gateway/session_dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,14 +469,20 @@
             )
             return
 
         muc = session.bookmarks._mucs_by_bare_jid.get(pto.bare)
         if muc is None or p.get_from().resource not in muc.user_resources:
             return
 
+        if pto.resource == muc.user_nick:
+            # Ignore presence stanzas with the valid nick.
+            # even if joined to the group, we might receive those from clients,
+            # when setting a status message, or going away, etc.
+            return
+
         # We can't use XMPPError here because from must be room@slidge/VALID-USER-NICK
 
         error_from = JID(muc.jid)
         error_from.resource = muc.user_nick
         error_stanza = p.error()
         error_stanza.set_to(p.get_from())
         error_stanza.set_from(error_from)
```

### Comparing `slidge-0.1.1/slidge/core/gateway/vcard_temp.py` & `slidge-0.1.2/slidge/core/gateway/vcard_temp.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/attachment.py` & `slidge-0.1.2/slidge/core/mixins/attachment.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/avatar.py` & `slidge-0.1.2/slidge/core/mixins/avatar.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/base.py` & `slidge-0.1.2/slidge/core/mixins/base.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/disco.py` & `slidge-0.1.2/slidge/core/mixins/disco.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/lock.py` & `slidge-0.1.2/slidge/core/mixins/lock.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/message.py` & `slidge-0.1.2/slidge/core/mixins/message.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/message_maker.py` & `slidge-0.1.2/slidge/core/mixins/message_maker.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/presence.py` & `slidge-0.1.2/slidge/core/mixins/presence.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/mixins/recipient.py` & `slidge-0.1.2/slidge/core/mixins/recipient.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/pubsub.py` & `slidge-0.1.2/slidge/core/pubsub.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/core/session.py` & `slidge-0.1.2/slidge/core/session.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/group/archive.py` & `slidge-0.1.2/slidge/group/archive.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/group/bookmarks.py` & `slidge-0.1.2/slidge/group/bookmarks.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/group/participant.py` & `slidge-0.1.2/slidge/group/participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         self.send_last_presence(force=True, no_cache_online=True)
 
     def send_affiliation_change(self):
         # internal use by slidge
         msg = self._make_message()
         msg["muc"]["affiliation"] = self._affiliation
         msg["type"] = "normal"
-        if not self.muc.is_anonymous:
+        if not self.muc.is_anonymous and not self.is_system:
             if self.contact:
                 msg["muc"]["jid"] = self.contact.jid
             else:
                 warnings.warn(
                     f"Private group but no 1:1 JID associated to '{self}'",
                 )
         self._send(msg)
@@ -231,15 +231,15 @@
         p["muc"]["affiliation"] = self.affiliation
         p["muc"]["role"] = self.role
         if self._hats:
             p["hats"].add_hats(self._hats)
         codes = status_codes or set()
         if self.is_user:
             codes.add(110)
-        if not self.muc.is_anonymous:
+        if not self.muc.is_anonymous and not self.is_system:
             if self.is_user:
                 if user_full_jid:
                     p["muc"]["jid"] = user_full_jid
                 else:
                     jid = copy(self.user.jid)
                     try:
                         jid.resource = next(
```

### Comparing `slidge-0.1.1/slidge/group/room.py` & `slidge-0.1.2/slidge/group/room.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/__init__.py` & `slidge-0.1.2/slidge/slixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/link_preview/stanza.py` & `slidge-0.1.2/slidge/slixfix/link_preview/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/roster.py` & `slidge-0.1.2/slidge/slixfix/roster.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0077/register.py` & `slidge-0.1.2/slidge/slixfix/xep_0077/register.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0077/stanza.py` & `slidge-0.1.2/slidge/slixfix/xep_0077/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0100/gateway.py` & `slidge-0.1.2/slidge/slixfix/xep_0100/gateway.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0153/stanza.py` & `slidge-0.1.2/slidge/slixfix/xep_0153/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0153/vcard_avatar.py` & `slidge-0.1.2/slidge/slixfix/xep_0153/vcard_avatar.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0264/stanza.py` & `slidge-0.1.2/slidge/slixfix/xep_0264/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0292/vcard4.py` & `slidge-0.1.2/slidge/slixfix/xep_0292/vcard4.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0313/mam.py` & `slidge-0.1.2/slidge/slixfix/xep_0313/mam.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0313/stanza.py` & `slidge-0.1.2/slidge/slixfix/xep_0313/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0317/stanza.py` & `slidge-0.1.2/slidge/slixfix/xep_0317/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0356_old/privilege.py` & `slidge-0.1.2/slidge/slixfix/xep_0356_old/privilege.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0356_old/stanza.py` & `slidge-0.1.2/slidge/slixfix/xep_0356_old/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0424/retraction.py` & `slidge-0.1.2/slidge/slixfix/xep_0424/retraction.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0424/stanza.py` & `slidge-0.1.2/slidge/slixfix/xep_0424/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/slixfix/xep_0490/mds.py` & `slidge-0.1.2/slidge/slixfix/xep_0490/mds.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/archive_msg.py` & `slidge-0.1.2/slidge/util/archive_msg.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/conf.py` & `slidge-0.1.2/slidge/util/conf.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/db.py` & `slidge-0.1.2/slidge/util/db.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/schema.sql` & `slidge-0.1.2/slidge/util/schema.sql`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/sql.py` & `slidge-0.1.2/slidge/util/sql.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/test.py` & `slidge-0.1.2/slidge/util/test.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/types.py` & `slidge-0.1.2/slidge/util/types.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/slidge/util/util.py` & `slidge-0.1.2/slidge/util/util.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.1/PKG-INFO` & `slidge-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slidge
-Version: 0.1.1
+Version: 0.1.2
 Summary: XMPP bridging framework
 Home-page: https://sr.ht/~nicoco/slidge/
 License: AGPL-3.0-or-later
 Author: Nicolas Cedilnik
 Author-email: nicoco@nicoco.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -16,17 +16,19 @@
 Requires-Dist: Pillow (>=10,<11)
 Requires-Dist: aiohttp[speedups] (>=3.8.3,<4.0.0)
 Requires-Dist: blurhash-python (>=1.2.1,<2.0.0)
 Requires-Dist: pickle-secure (>=0.99.9,<0.100.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: qrcode (>=7.4.1,<8.0.0)
 Requires-Dist: slixmpp (>=1.8.5,<2.0.0)
+Project-URL: Documentation, https://slidge.im/
+Project-URL: Repository, https://git.sr.ht/~nicoco/slidge/
 Description-Content-Type: text/markdown
 
-![Slidge logo](./dev/assets/slidge-color-small.png)
+![Slidge logo](https://git.sr.ht/~nicoco/slidge/blob/master/dev/assets/slidge-color-small.png)
 
 [Home](https://sr.ht/~nicoco/slidge) |
 [Docs](https://slidge.im/core) |
 [Source](https://sr.ht/~nicoco/slidge/sources) |
 [Issues](https://sr.ht/~nicoco/slidge/trackers) |
 [Patches](https://lists.sr.ht/~nicoco/public-inbox) |
 [Chat](xmpp:slidge@conference.nicoco.fr?join)
@@ -62,16 +64,15 @@
 If you use debian, you might also be interested in the
 [slidge-debian](https://git.sr.ht/~nicoco/slidge-debian)
 bundle.
 
 Status
 ------
 
-Slidge is **beta**-grade software for 1:1 chats.
-Group chat support is **experimental**.
+Slidge is **beta**-grade software. It support groups and 1:1 chats.
 
 Try slidge and give us some
 feedback, through the [MUC](xmpp:slidge@conference.nicoco.fr?join), the
 [issue tracker](https://todo.sr.ht/~nicoco/slidge) or in the
 [public inbox](https://lists.sr.ht/~nicoco/public-inbox).
 Don't be shy!
```

