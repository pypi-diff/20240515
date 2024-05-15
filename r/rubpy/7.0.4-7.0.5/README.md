# Comparing `tmp/rubpy-7.0.4.tar.gz` & `tmp/rubpy-7.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-7.0.4.tar", last modified: Tue May  7 00:09:05 2024, max compression
+gzip compressed data, was "rubpy-7.0.5.tar", last modified: Wed May 15 01:21:49 2024, max compression
```

## Comparing `rubpy-7.0.4.tar` & `rubpy-7.0.5.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.850391 rubpy-7.0.4/
--rw-rw-rw-   0        0        0     3721 2024-05-07 00:09:05.849416 rubpy-7.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2024-03-14 02:30:28.000000 rubpy-7.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.545879 rubpy-7.0.4/rubpy/
--rw-rw-rw-   0        0        0      488 2024-05-07 00:08:50.000000 rubpy-7.0.4/rubpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.602489 rubpy-7.0.4/rubpy/bots/
--rw-rw-rw-   0        0        0        0 2024-01-08 21:58:47.000000 rubpy-7.0.4/rubpy/bots/__init__.py
--rw-rw-rw-   0        0        0    11161 2024-01-08 22:59:16.000000 rubpy-7.0.4/rubpy/bots/client.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.695208 rubpy-7.0.4/rubpy/bots/types/
--rw-rw-rw-   0        0        0     1077 2024-01-08 22:47:11.000000 rubpy-7.0.4/rubpy/bots/types/__init__.py
--rw-rw-rw-   0        0        0      163 2024-01-08 22:26:46.000000 rubpy-7.0.4/rubpy/bots/types/aux_data.py
--rw-rw-rw-   0        0        0      255 2024-01-08 22:11:16.000000 rubpy-7.0.4/rubpy/bots/types/bot.py
--rw-rw-rw-   0        0        0      102 2024-01-08 22:11:52.000000 rubpy-7.0.4/rubpy/bots/types/bot_command.py
--rw-rw-rw-   0        0        0     1093 2024-01-08 22:29:20.000000 rubpy-7.0.4/rubpy/bots/types/button.py
--rw-rw-rw-   0        0        0      225 2024-01-08 22:20:24.000000 rubpy-7.0.4/rubpy/bots/types/button_calendar.py
--rw-rw-rw-   0        0        0      286 2024-01-08 22:25:55.000000 rubpy-7.0.4/rubpy/bots/types/button_location.py
--rw-rw-rw-   0        0        0      191 2024-01-08 22:21:11.000000 rubpy-7.0.4/rubpy/bots/types/button_number_picker.py
--rw-rw-rw-   0        0        0      377 2024-01-08 22:19:28.000000 rubpy-7.0.4/rubpy/bots/types/button_selection.py
--rw-rw-rw-   0        0        0      195 2024-01-08 22:18:19.000000 rubpy-7.0.4/rubpy/bots/types/button_selection_item.py
--rw-rw-rw-   0        0        0      159 2024-01-08 22:22:12.000000 rubpy-7.0.4/rubpy/bots/types/button_string_picker.py
--rw-rw-rw-   0        0        0      255 2024-01-08 22:24:13.000000 rubpy-7.0.4/rubpy/bots/types/button_textbox.py
--rw-rw-rw-   0        0        0      257 2024-01-08 22:02:54.000000 rubpy-7.0.4/rubpy/bots/types/chat.py
--rw-rw-rw-   0        0        0      132 2024-01-08 22:13:08.000000 rubpy-7.0.4/rubpy/bots/types/contact_message.py
--rw-rw-rw-   0        0        0      111 2024-01-08 22:02:20.000000 rubpy-7.0.4/rubpy/bots/types/file.py
--rw-rw-rw-   0        0        0      214 2024-01-08 22:03:18.000000 rubpy-7.0.4/rubpy/bots/types/forwarded_from.py
--rw-rw-rw-   0        0        0      340 2024-01-08 22:36:23.000000 rubpy-7.0.4/rubpy/bots/types/inline_message.py
--rw-rw-rw-   0        0        0      232 2024-01-08 22:30:58.000000 rubpy-7.0.4/rubpy/bots/types/keypad.py
--rw-rw-rw-   0        0        0      141 2024-01-08 22:30:09.000000 rubpy-7.0.4/rubpy/bots/types/keypad_row.py
--rw-rw-rw-   0        0        0      340 2024-01-08 22:17:29.000000 rubpy-7.0.4/rubpy/bots/types/live_location.py
--rw-rw-rw-   0        0        0       99 2024-01-08 22:15:36.000000 rubpy-7.0.4/rubpy/bots/types/location.py
--rw-rw-rw-   0        0        0      107 2024-01-08 22:09:39.000000 rubpy-7.0.4/rubpy/bots/types/messaage_text_update.py
--rw-rw-rw-   0        0        0      887 2024-01-08 22:34:09.000000 rubpy-7.0.4/rubpy/bots/types/message.py
--rw-rw-rw-   0        0        0      149 2024-01-08 22:31:58.000000 rubpy-7.0.4/rubpy/bots/types/message_keypad_update.py
--rw-rw-rw-   0        0        0      156 2024-01-08 22:03:44.000000 rubpy-7.0.4/rubpy/bots/types/payment_status.py
--rw-rw-rw-   0        0        0      192 2024-01-08 22:14:43.000000 rubpy-7.0.4/rubpy/bots/types/poll.py
--rw-rw-rw-   0        0        0      248 2024-01-08 22:13:58.000000 rubpy-7.0.4/rubpy/bots/types/poll_status.py
--rw-rw-rw-   0        0        0      148 2024-01-08 22:12:28.000000 rubpy-7.0.4/rubpy/bots/types/sticker.py
--rw-rw-rw-   0        0        0      455 2024-01-08 22:35:18.000000 rubpy-7.0.4/rubpy/bots/types/update.py
--rw-rw-rw-   0        0        0     5768 2024-03-14 02:20:07.000000 rubpy-7.0.4/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.696183 rubpy-7.0.4/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-7.0.4/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     5386 2024-04-24 22:40:45.000000 rubpy-7.0.4/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.703015 rubpy-7.0.4/rubpy/enums/
--rw-rw-rw-   0        0        0      320 2024-04-24 21:33:03.000000 rubpy-7.0.4/rubpy/enums/__init__.py
--rw-rw-rw-   0        0        0      633 2024-02-03 10:53:26.000000 rubpy-7.0.4/rubpy/enums/chat_access_type.py
--rw-rw-rw-   0        0        0      214 2024-02-03 10:54:38.000000 rubpy-7.0.4/rubpy/enums/chat_action.py
--rw-rw-rw-   0        0        0      370 2024-01-11 13:02:06.000000 rubpy-7.0.4/rubpy/enums/chat_type.py
--rw-rw-rw-   0        0        0      568 2024-04-06 22:47:37.000000 rubpy-7.0.4/rubpy/enums/message_media_type.py
--rw-rw-rw-   0        0        0      100 2024-02-10 16:11:46.000000 rubpy-7.0.4/rubpy/enums/parse_mode.py
--rw-rw-rw-   0        0        0      133 2024-01-11 13:07:44.000000 rubpy-7.0.4/rubpy/enums/poll_type.py
--rw-rw-rw-   0        0        0     1767 2024-01-16 12:03:08.000000 rubpy-7.0.4/rubpy/enums/reaction_type.py
--rw-rw-rw-   0        0        0      280 2024-04-24 21:38:53.000000 rubpy-7.0.4/rubpy/enums/report_type.py
--rw-rw-rw-   0        0        0     1942 2024-01-08 22:38:06.000000 rubpy-7.0.4/rubpy/exceptions.py
--rw-rw-rw-   0        0        0    12916 2024-05-01 22:34:27.000000 rubpy-7.0.4/rubpy/filters.py
--rw-rw-rw-   0        0        0     4886 2024-02-24 22:37:29.000000 rubpy-7.0.4/rubpy/handlers.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.703991 rubpy-7.0.4/rubpy/methods/
--rw-rw-rw-   0        0        0      697 2024-02-23 15:20:39.000000 rubpy-7.0.4/rubpy/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.705943 rubpy-7.0.4/rubpy/methods/advanced/
--rw-rw-rw-   0        0        0      143 2024-02-22 17:41:57.000000 rubpy-7.0.4/rubpy/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     2312 2024-03-14 01:56:23.000000 rubpy-7.0.4/rubpy/methods/advanced/build.py
--rw-rw-rw-   0        0        0     4483 2024-02-25 17:08:53.000000 rubpy-7.0.4/rubpy/methods/advanced/voice_chat_player.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.708871 rubpy-7.0.4/rubpy/methods/auth/
--rw-rw-rw-   0        0        0      185 2023-12-15 18:54:26.000000 rubpy-7.0.4/rubpy/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     2007 2024-03-09 18:53:42.000000 rubpy-7.0.4/rubpy/methods/auth/register_device.py
--rw-rw-rw-   0        0        0      798 2024-02-24 22:49:22.000000 rubpy-7.0.4/rubpy/methods/auth/send_code.py
--rw-rw-rw-   0        0        0      576 2024-02-24 22:51:51.000000 rubpy-7.0.4/rubpy/methods/auth/sign_in.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.725463 rubpy-7.0.4/rubpy/methods/channels/
--rw-rw-rw-   0        0        0     1826 2024-01-22 20:05:38.000000 rubpy-7.0.4/rubpy/methods/channels/__init__.py
--rw-rw-rw-   0        0        0     1042 2024-02-24 22:53:48.000000 rubpy-7.0.4/rubpy/methods/channels/add_channel.py
--rw-rw-rw-   0        0        0      882 2024-02-24 22:53:29.000000 rubpy-7.0.4/rubpy/methods/channels/add_channel_members.py
--rw-rw-rw-   0        0        0     1065 2024-02-24 22:54:12.000000 rubpy-7.0.4/rubpy/methods/channels/ban_channel_member.py
--rw-rw-rw-   0        0        0      613 2024-02-24 22:54:34.000000 rubpy-7.0.4/rubpy/methods/channels/channel_preview_by_join_link.py
--rw-rw-rw-   0        0        0      574 2024-02-24 22:54:51.000000 rubpy-7.0.4/rubpy/methods/channels/check_channel_username.py
--rw-rw-rw-   0        0        0      523 2024-02-24 22:55:07.000000 rubpy-7.0.4/rubpy/methods/channels/create_channel_voice_chat.py
--rw-rw-rw-   0        0        0      748 2024-02-24 22:55:21.000000 rubpy-7.0.4/rubpy/methods/channels/discard_channel_voice_chat.py
--rw-rw-rw-   0        0        0     2601 2024-02-24 22:55:49.000000 rubpy-7.0.4/rubpy/methods/channels/edit_channel_info.py
--rw-rw-rw-   0        0        0      705 2024-02-24 22:56:18.000000 rubpy-7.0.4/rubpy/methods/channels/get_banned_group_members.py
--rw-rw-rw-   0        0        0      681 2024-02-24 22:56:34.000000 rubpy-7.0.4/rubpy/methods/channels/get_channel_admin_access_list.py
--rw-rw-rw-   0        0        0      681 2024-02-24 22:56:52.000000 rubpy-7.0.4/rubpy/methods/channels/get_channel_admin_members.py
--rw-rw-rw-   0        0        0      819 2024-02-24 22:58:08.000000 rubpy-7.0.4/rubpy/methods/channels/get_channel_all_members.py
--rw-rw-rw-   0        0        0      504 2024-02-24 22:58:25.000000 rubpy-7.0.4/rubpy/methods/channels/get_channel_info.py
--rw-rw-rw-   0        0        0      503 2024-02-24 22:58:39.000000 rubpy-7.0.4/rubpy/methods/channels/get_channel_link.py
--rw-rw-rw-   0        0        0      996 2024-02-24 22:58:58.000000 rubpy-7.0.4/rubpy/methods/channels/join_channel_action.py
--rw-rw-rw-   0        0        0      609 2024-02-24 22:59:21.000000 rubpy-7.0.4/rubpy/methods/channels/join_channel_by_link.py
--rw-rw-rw-   0        0        0      610 2024-02-24 22:59:38.000000 rubpy-7.0.4/rubpy/methods/channels/remove_channel.py
--rw-rw-rw-   0        0        0      956 2024-02-24 23:00:34.000000 rubpy-7.0.4/rubpy/methods/channels/seen_channel_messages.py
--rw-rw-rw-   0        0        0      631 2024-02-24 23:00:59.000000 rubpy-7.0.4/rubpy/methods/channels/set_channel_link.py
--rw-rw-rw-   0        0        0     1051 2024-02-24 23:01:17.000000 rubpy-7.0.4/rubpy/methods/channels/set_channel_voice_chat_setting.py
--rw-rw-rw-   0        0        0      772 2024-02-24 23:01:35.000000 rubpy-7.0.4/rubpy/methods/channels/update_channel_username.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.735230 rubpy-7.0.4/rubpy/methods/chats/
--rw-rw-rw-   0        0        0      807 2023-12-20 14:35:52.000000 rubpy-7.0.4/rubpy/methods/chats/__init__.py
--rw-rw-rw-   0        0        0      806 2024-02-24 23:02:06.000000 rubpy-7.0.4/rubpy/methods/chats/delete_avatar.py
--rw-rw-rw-   0        0        0      966 2024-02-24 23:02:35.000000 rubpy-7.0.4/rubpy/methods/chats/delete_chat_history.py
--rw-rw-rw-   0        0        0      790 2024-02-24 23:02:59.000000 rubpy-7.0.4/rubpy/methods/chats/get_abs_objects.py
--rw-rw-rw-   0        0        0      636 2024-02-24 23:03:23.000000 rubpy-7.0.4/rubpy/methods/chats/get_avatars.py
--rw-rw-rw-   0        0        0      601 2024-02-24 23:05:28.000000 rubpy-7.0.4/rubpy/methods/chats/get_chats.py
--rw-rw-rw-   0        0        0      745 2024-02-24 23:04:22.000000 rubpy-7.0.4/rubpy/methods/chats/get_chats_updates.py
--rw-rw-rw-   0        0        0      599 2024-02-24 23:08:10.000000 rubpy-7.0.4/rubpy/methods/chats/get_link_from_app_url.py
--rw-rw-rw-   0        0        0     1265 2024-02-24 23:08:43.000000 rubpy-7.0.4/rubpy/methods/chats/search_chat_messages.py
--rw-rw-rw-   0        0        0      611 2024-02-24 23:10:47.000000 rubpy-7.0.4/rubpy/methods/chats/seen_chats.py
--rw-rw-rw-   0        0        0     1110 2024-02-24 23:11:34.000000 rubpy-7.0.4/rubpy/methods/chats/send_chat_activity.py
--rw-rw-rw-   0        0        0     1014 2024-02-24 23:12:16.000000 rubpy-7.0.4/rubpy/methods/chats/set_action_chat.py
--rw-rw-rw-   0        0        0     1818 2024-02-24 23:13:42.000000 rubpy-7.0.4/rubpy/methods/chats/upload_avatar.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.739127 rubpy-7.0.4/rubpy/methods/contacts/
--rw-rw-rw-   0        0        0      299 2023-12-22 14:16:01.000000 rubpy-7.0.4/rubpy/methods/contacts/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-02-24 23:15:53.000000 rubpy-7.0.4/rubpy/methods/contacts/add_address_book.py
--rw-rw-rw-   0        0        0      753 2024-02-24 23:16:17.000000 rubpy-7.0.4/rubpy/methods/contacts/delete_contact.py
--rw-rw-rw-   0        0        0      622 2024-02-24 23:18:12.000000 rubpy-7.0.4/rubpy/methods/contacts/get_contacts.py
--rw-rw-rw-   0        0        0      770 2024-02-24 23:17:44.000000 rubpy-7.0.4/rubpy/methods/contacts/get_contacts_updates.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.743031 rubpy-7.0.4/rubpy/methods/decorators/
--rw-rw-rw-   0        0        0      415 2023-12-25 13:18:28.000000 rubpy-7.0.4/rubpy/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0      592 2024-02-24 23:18:27.000000 rubpy-7.0.4/rubpy/methods/decorators/on_chat_updates.py
--rw-rw-rw-   0        0        0      604 2024-02-24 23:18:42.000000 rubpy-7.0.4/rubpy/methods/decorators/on_message_updates.py
--rw-rw-rw-   0        0        0      624 2024-02-24 23:18:56.000000 rubpy-7.0.4/rubpy/methods/decorators/on_remove_notifications.py
--rw-rw-rw-   0        0        0      604 2024-02-24 23:19:09.000000 rubpy-7.0.4/rubpy/methods/decorators/on_show_activities.py
--rw-rw-rw-   0        0        0      616 2024-02-24 23:19:21.000000 rubpy-7.0.4/rubpy/methods/decorators/on_show_notifications.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.753768 rubpy-7.0.4/rubpy/methods/extras/
--rw-rw-rw-   0        0        0      745 2024-02-15 12:50:33.000000 rubpy-7.0.4/rubpy/methods/extras/__init__.py
--rw-rw-rw-   0        0        0      739 2024-02-24 23:19:55.000000 rubpy-7.0.4/rubpy/methods/extras/ban_member.py
--rw-rw-rw-   0        0        0     1039 2024-02-24 23:20:10.000000 rubpy-7.0.4/rubpy/methods/extras/get_info.py
--rw-rw-rw-   0        0        0      693 2024-02-24 23:20:43.000000 rubpy-7.0.4/rubpy/methods/extras/get_object_by_username.py
--rw-rw-rw-   0        0        0      538 2024-02-24 23:21:03.000000 rubpy-7.0.4/rubpy/methods/extras/get_profile_link_items.py
--rw-rw-rw-   0        0        0      530 2024-02-24 23:21:19.000000 rubpy-7.0.4/rubpy/methods/extras/get_related_objects.py
--rw-rw-rw-   0        0        0      770 2024-02-24 23:22:06.000000 rubpy-7.0.4/rubpy/methods/extras/get_transcription.py
--rw-rw-rw-   0        0        0      690 2024-02-24 23:22:29.000000 rubpy-7.0.4/rubpy/methods/extras/join.py
--rw-rw-rw-   0        0        0      648 2024-02-24 23:22:49.000000 rubpy-7.0.4/rubpy/methods/extras/leave_chat.py
--rw-rw-rw-   0        0        0     1305 2024-04-24 21:38:46.000000 rubpy-7.0.4/rubpy/methods/extras/report_object.py
--rw-rw-rw-   0        0        0      665 2024-02-24 23:24:05.000000 rubpy-7.0.4/rubpy/methods/extras/search_global_objects.py
--rw-rw-rw-   0        0        0      695 2024-02-24 23:25:58.000000 rubpy-7.0.4/rubpy/methods/extras/transcribe_voice.py
--rw-rw-rw-   0        0        0     1019 2024-02-24 23:26:53.000000 rubpy-7.0.4/rubpy/methods/extras/user_is_admin.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.757672 rubpy-7.0.4/rubpy/methods/gif/
--rw-rw-rw-   0        0        0      235 2024-01-09 12:00:36.000000 rubpy-7.0.4/rubpy/methods/gif/__init__.py
--rw-rw-rw-   0        0        0      611 2024-02-24 23:27:54.000000 rubpy-7.0.4/rubpy/methods/gif/add_to_my_gif_set.py
--rw-rw-rw-   0        0        0      341 2024-02-24 23:28:10.000000 rubpy-7.0.4/rubpy/methods/gif/get_my_gif_set.py
--rw-rw-rw-   0        0        0      430 2024-02-24 23:28:39.000000 rubpy-7.0.4/rubpy/methods/gif/remove_from_my_gif_set.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.776215 rubpy-7.0.4/rubpy/methods/groups/
--rw-rw-rw-   0        0        0     1857 2023-12-22 17:47:50.000000 rubpy-7.0.4/rubpy/methods/groups/__init__.py
--rw-rw-rw-   0        0        0      987 2024-02-24 23:33:24.000000 rubpy-7.0.4/rubpy/methods/groups/add_group.py
--rw-rw-rw-   0        0        0      958 2024-02-24 23:29:42.000000 rubpy-7.0.4/rubpy/methods/groups/add_group_members.py
--rw-rw-rw-   0        0        0     1229 2024-02-24 23:33:49.000000 rubpy-7.0.4/rubpy/methods/groups/ban_group_member.py
--rw-rw-rw-   0        0        0      600 2024-02-24 23:34:06.000000 rubpy-7.0.4/rubpy/methods/groups/create_group_voice_chat.py
--rw-rw-rw-   0        0        0      618 2024-02-24 23:34:23.000000 rubpy-7.0.4/rubpy/methods/groups/delete_no_access_group_chat.py
--rw-rw-rw-   0        0        0     2648 2024-02-24 23:34:53.000000 rubpy-7.0.4/rubpy/methods/groups/edit_group_info.py
--rw-rw-rw-   0        0        0      785 2024-02-24 23:35:11.000000 rubpy-7.0.4/rubpy/methods/groups/get_banned_group_members.py
--rw-rw-rw-   0        0        0      820 2024-02-24 23:35:36.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_admin_access_list.py
--rw-rw-rw-   0        0        0      791 2024-02-24 23:35:53.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_admin_members.py
--rw-rw-rw-   0        0        0     1003 2024-02-25 13:45:13.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_all_members.py
--rw-rw-rw-   0        0        0      644 2024-02-24 23:36:57.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_default_access.py
--rw-rw-rw-   0        0        0      584 2024-02-24 23:37:09.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_info.py
--rw-rw-rw-   0        0        0      578 2024-02-24 23:37:26.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_link.py
--rw-rw-rw-   0        0        0      787 2024-02-24 23:37:39.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_mention_list.py
--rw-rw-rw-   0        0        0     1096 2024-02-24 23:38:09.000000 rubpy-7.0.4/rubpy/methods/groups/get_group_voice_chat_updates.py
--rw-rw-rw-   0        0        0      688 2024-02-24 23:38:23.000000 rubpy-7.0.4/rubpy/methods/groups/group_preview_by_join_link.py
--rw-rw-rw-   0        0        0      645 2024-02-24 23:38:40.000000 rubpy-7.0.4/rubpy/methods/groups/join_group.py
--rw-rw-rw-   0        0        0      460 2024-02-24 23:39:16.000000 rubpy-7.0.4/rubpy/methods/groups/leave_group.py
--rw-rw-rw-   0        0        0      784 2024-02-24 23:38:58.000000 rubpy-7.0.4/rubpy/methods/groups/leave_group_voice_chat.py
--rw-rw-rw-   0        0        0      466 2024-02-24 23:39:33.000000 rubpy-7.0.4/rubpy/methods/groups/remove_group.py
--rw-rw-rw-   0        0        0     1549 2024-02-24 23:40:14.000000 rubpy-7.0.4/rubpy/methods/groups/set_group_admin.py
--rw-rw-rw-   0        0        0      920 2024-02-24 23:42:43.000000 rubpy-7.0.4/rubpy/methods/groups/set_group_default_access.py
--rw-rw-rw-   0        0        0      596 2024-02-24 23:45:52.000000 rubpy-7.0.4/rubpy/methods/groups/set_group_link.py
--rw-rw-rw-   0        0        0      980 2024-02-24 23:49:50.000000 rubpy-7.0.4/rubpy/methods/groups/set_group_voice_chat_setting.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.796712 rubpy-7.0.4/rubpy/methods/messages/
--rw-rw-rw-   0        0        0     1808 2024-02-25 13:57:52.000000 rubpy-7.0.4/rubpy/methods/messages/__init__.py
--rw-rw-rw-   0        0        0     1431 2024-02-25 13:21:28.000000 rubpy-7.0.4/rubpy/methods/messages/action_on_message_reaction.py
--rw-rw-rw-   0        0        0     1148 2024-02-25 13:22:34.000000 rubpy-7.0.4/rubpy/methods/messages/auto_delete_message.py
--rw-rw-rw-   0        0        0     2603 2024-02-25 13:23:17.000000 rubpy-7.0.4/rubpy/methods/messages/create_poll.py
--rw-rw-rw-   0        0        0     1550 2024-02-25 13:24:10.000000 rubpy-7.0.4/rubpy/methods/messages/delete_messages.py
--rw-rw-rw-   0        0        0     1633 2024-02-25 13:25:45.000000 rubpy-7.0.4/rubpy/methods/messages/edit_message.py
--rw-rw-rw-   0        0        0     1635 2024-02-25 13:27:51.000000 rubpy-7.0.4/rubpy/methods/messages/forward_messages.py
--rw-rw-rw-   0        0        0     1044 2024-03-14 20:52:58.000000 rubpy-7.0.4/rubpy/methods/messages/get_message_share_url.py
--rw-rw-rw-   0        0        0     1193 2024-02-25 13:28:35.000000 rubpy-7.0.4/rubpy/methods/messages/get_messages_by_id.py
--rw-rw-rw-   0        0        0     1245 2024-02-25 13:28:56.000000 rubpy-7.0.4/rubpy/methods/messages/get_messages_interval.py
--rw-rw-rw-   0        0        0     1165 2024-02-25 13:29:20.000000 rubpy-7.0.4/rubpy/methods/messages/get_messages_updates.py
--rw-rw-rw-   0        0        0     1250 2024-02-25 13:31:15.000000 rubpy-7.0.4/rubpy/methods/messages/get_poll_option_voters.py
--rw-rw-rw-   0        0        0      823 2024-02-25 13:31:35.000000 rubpy-7.0.4/rubpy/methods/messages/get_poll_status.py
--rw-rw-rw-   0        0        0     1090 2024-02-25 13:31:55.000000 rubpy-7.0.4/rubpy/methods/messages/reaction.py
--rw-rw-rw-   0        0        0     1136 2024-02-25 13:32:18.000000 rubpy-7.0.4/rubpy/methods/messages/remove_reaction.py
--rw-rw-rw-   0        0        0     1156 2024-02-25 13:32:38.000000 rubpy-7.0.4/rubpy/methods/messages/request_send_file.py
--rw-rw-rw-   0        0        0     1515 2024-02-25 13:32:59.000000 rubpy-7.0.4/rubpy/methods/messages/send_document.py
--rw-rw-rw-   0        0        0     1248 2024-02-25 13:35:35.000000 rubpy-7.0.4/rubpy/methods/messages/send_gif.py
--rw-rw-rw-   0        0        0     7849 2024-05-07 00:06:38.000000 rubpy-7.0.4/rubpy/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     1266 2024-02-25 13:35:46.000000 rubpy-7.0.4/rubpy/methods/messages/send_music.py
--rw-rw-rw-   0        0        0     1492 2024-02-25 13:35:55.000000 rubpy-7.0.4/rubpy/methods/messages/send_photo.py
--rw-rw-rw-   0        0        0     1785 2024-02-25 13:45:22.000000 rubpy-7.0.4/rubpy/methods/messages/send_sticker.py
--rw-rw-rw-   0        0        0     1236 2024-02-25 13:45:25.000000 rubpy-7.0.4/rubpy/methods/messages/send_video.py
--rw-rw-rw-   0        0        0     1374 2024-02-25 13:45:23.000000 rubpy-7.0.4/rubpy/methods/messages/send_video_message.py
--rw-rw-rw-   0        0        0     1384 2024-02-25 13:44:36.000000 rubpy-7.0.4/rubpy/methods/messages/send_voice.py
--rw-rw-rw-   0        0        0     2422 2024-02-25 13:43:55.000000 rubpy-7.0.4/rubpy/methods/messages/set_pin_message.py
--rw-rw-rw-   0        0        0      799 2024-02-25 13:44:20.000000 rubpy-7.0.4/rubpy/methods/messages/vote_poll.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.807448 rubpy-7.0.4/rubpy/methods/settings/
--rw-rw-rw-   0        0        0      878 2023-12-22 15:33:50.000000 rubpy-7.0.4/rubpy/methods/settings/__init__.py
--rw-rw-rw-   0        0        0      746 2024-02-25 13:16:01.000000 rubpy-7.0.4/rubpy/methods/settings/delete_folder.py
--rw-rw-rw-   0        0        0      586 2024-02-25 13:17:26.000000 rubpy-7.0.4/rubpy/methods/settings/get_blocked_users.py
--rw-rw-rw-   0        0        0      832 2024-02-25 13:17:43.000000 rubpy-7.0.4/rubpy/methods/settings/get_folders.py
--rw-rw-rw-   0        0        0      660 2024-02-25 13:18:03.000000 rubpy-7.0.4/rubpy/methods/settings/get_my_sessions.py
--rw-rw-rw-   0        0        0      640 2024-02-25 13:18:19.000000 rubpy-7.0.4/rubpy/methods/settings/get_privacy_setting.py
--rw-rw-rw-   0        0        0      648 2024-02-25 13:18:36.000000 rubpy-7.0.4/rubpy/methods/settings/get_suggested_folders.py
--rw-rw-rw-   0        0        0      662 2024-02-25 13:18:52.000000 rubpy-7.0.4/rubpy/methods/settings/get_two_passcode_status.py
--rw-rw-rw-   0        0        0     3312 2024-02-25 13:19:21.000000 rubpy-7.0.4/rubpy/methods/settings/set_setting.py
--rw-rw-rw-   0        0        0     1267 2024-02-25 13:20:00.000000 rubpy-7.0.4/rubpy/methods/settings/setup_two_step_verification.py
--rw-rw-rw-   0        0        0      801 2024-02-25 13:20:16.000000 rubpy-7.0.4/rubpy/methods/settings/terminate_session.py
--rw-rw-rw-   0        0        0     1663 2024-02-25 13:20:39.000000 rubpy-7.0.4/rubpy/methods/settings/update_profile.py
--rw-rw-rw-   0        0        0      745 2024-02-25 13:20:56.000000 rubpy-7.0.4/rubpy/methods/settings/update_username.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.813305 rubpy-7.0.4/rubpy/methods/stickers/
--rw-rw-rw-   0        0        0      578 2023-12-22 16:07:24.000000 rubpy-7.0.4/rubpy/methods/stickers/__init__.py
--rw-rw-rw-   0        0        0     1283 2024-02-25 13:08:37.000000 rubpy-7.0.4/rubpy/methods/stickers/action_on_sticker_set.py
--rw-rw-rw-   0        0        0      564 2024-02-25 13:09:11.000000 rubpy-7.0.4/rubpy/methods/stickers/get_my_sticker_sets.py
--rw-rw-rw-   0        0        0      778 2024-02-25 13:09:47.000000 rubpy-7.0.4/rubpy/methods/stickers/get_sticker_set_by_id.py
--rw-rw-rw-   0        0        0      877 2024-02-25 13:45:26.000000 rubpy-7.0.4/rubpy/methods/stickers/get_stickers_by_emoji.py
--rw-rw-rw-   0        0        0      941 2024-02-25 13:14:21.000000 rubpy-7.0.4/rubpy/methods/stickers/get_stickers_by_set_ids.py
--rw-rw-rw-   0        0        0      766 2024-02-25 13:14:11.000000 rubpy-7.0.4/rubpy/methods/stickers/get_trend_sticker_sets.py
--rw-rw-rw-   0        0        0      929 2024-02-25 13:14:28.000000 rubpy-7.0.4/rubpy/methods/stickers/search_stickers.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.817207 rubpy-7.0.4/rubpy/methods/users/
--rw-rw-rw-   0        0        0      331 2023-12-19 22:35:32.000000 rubpy-7.0.4/rubpy/methods/users/__init__.py
--rw-rw-rw-   0        0        0      713 2024-02-25 13:03:33.000000 rubpy-7.0.4/rubpy/methods/users/check_user_username.py
--rw-rw-rw-   0        0        0     1042 2024-02-25 13:04:30.000000 rubpy-7.0.4/rubpy/methods/users/delete_user_chat.py
--rw-rw-rw-   0        0        0      539 2024-02-25 13:05:08.000000 rubpy-7.0.4/rubpy/methods/users/get_me.py
--rw-rw-rw-   0        0        0      881 2024-02-26 15:47:56.000000 rubpy-7.0.4/rubpy/methods/users/get_user_info.py
--rw-rw-rw-   0        0        0     1265 2024-02-25 13:06:50.000000 rubpy-7.0.4/rubpy/methods/users/set_block_user.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.833799 rubpy-7.0.4/rubpy/methods/utilities/
--rw-rw-rw-   0        0        0      613 2024-01-12 14:48:33.000000 rubpy-7.0.4/rubpy/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0      762 2024-02-25 12:47:55.000000 rubpy-7.0.4/rubpy/methods/utilities/add_handler.py
--rw-rw-rw-   0        0        0      741 2024-04-01 23:10:22.000000 rubpy-7.0.4/rubpy/methods/utilities/audio.py
--rw-rw-rw-   0        0        0      708 2024-02-26 14:31:15.000000 rubpy-7.0.4/rubpy/methods/utilities/connect.py
--rw-rw-rw-   0        0        0      574 2024-02-25 12:48:51.000000 rubpy-7.0.4/rubpy/methods/utilities/disconnect.py
--rw-rw-rw-   0        0        0     1756 2024-04-24 22:13:20.000000 rubpy-7.0.4/rubpy/methods/utilities/download.py
--rw-rw-rw-   0        0        0     1080 2024-03-20 23:17:03.000000 rubpy-7.0.4/rubpy/methods/utilities/download_profile_picture.py
--rw-rw-rw-   0        0        0     1419 2024-02-25 12:52:55.000000 rubpy-7.0.4/rubpy/methods/utilities/get_members.py
--rw-rw-rw-   0        0        0      337 2024-02-25 12:53:13.000000 rubpy-7.0.4/rubpy/methods/utilities/get_updates.py
--rw-rw-rw-   0        0        0      326 2024-02-25 12:54:09.000000 rubpy-7.0.4/rubpy/methods/utilities/remove_handler.py
--rw-rw-rw-   0        0        0      967 2024-02-25 12:54:38.000000 rubpy-7.0.4/rubpy/methods/utilities/run.py
--rw-rw-rw-   0        0        0     3646 2024-03-09 18:54:30.000000 rubpy-7.0.4/rubpy/methods/utilities/start.py
--rw-rw-rw-   0        0        0     6614 2024-04-06 23:05:13.000000 rubpy-7.0.4/rubpy/methods/utilities/thumbnail.py
--rw-rw-rw-   0        0        0      671 2024-02-25 13:02:33.000000 rubpy-7.0.4/rubpy/methods/utilities/upload.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.836727 rubpy-7.0.4/rubpy/methods/voice_chat/
--rw-rw-rw-   0        0        0      278 2024-02-25 16:36:44.000000 rubpy-7.0.4/rubpy/methods/voice_chat/__init__.py
--rw-rw-rw-   0        0        0      918 2024-02-24 23:57:22.000000 rubpy-7.0.4/rubpy/methods/voice_chat/join_voice_chat.py
--rw-rw-rw-   0        0        0     1077 2024-02-24 23:55:36.000000 rubpy-7.0.4/rubpy/methods/voice_chat/send_group_voice_chat_activity.py
--rw-rw-rw-   0        0        0     1181 2024-02-25 16:36:50.000000 rubpy-7.0.4/rubpy/methods/voice_chat/set_voice_chat_state.py
--rw-rw-rw-   0        0        0    15334 2024-05-02 13:34:22.000000 rubpy-7.0.4/rubpy/network.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.837704 rubpy-7.0.4/rubpy/parser/
--rw-rw-rw-   0        0        0       30 2024-01-09 13:49:12.000000 rubpy-7.0.4/rubpy/parser/__init__.py
--rw-rw-rw-   0        0        0     3941 2024-05-07 00:07:00.000000 rubpy-7.0.4/rubpy/parser/markdown.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.844536 rubpy-7.0.4/rubpy/rubino/
--rw-rw-rw-   0        0        0       26 2024-01-08 21:17:13.000000 rubpy-7.0.4/rubpy/rubino/__init__.py
--rw-rw-rw-   0        0        0    16027 2024-03-14 00:36:15.000000 rubpy-7.0.4/rubpy/rubino/client.py
--rw-rw-rw-   0        0        0     7036 2024-05-03 02:14:46.000000 rubpy-7.0.4/rubpy/rubino/thumbnail.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.847464 rubpy-7.0.4/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-7.0.4/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2294 2023-12-19 12:35:20.000000 rubpy-7.0.4/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-7.0.4/rubpy/sessions/stringSession.py
--rw-rw-rw-   0        0        0     3430 2024-03-14 02:26:10.000000 rubpy-7.0.4/rubpy/sync.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.849416 rubpy-7.0.4/rubpy/types/
--rw-rw-rw-   0        0        0       65 2024-02-24 22:46:34.000000 rubpy-7.0.4/rubpy/types/__init__.py
--rw-rw-rw-   0        0        0    30721 2024-04-24 22:04:33.000000 rubpy-7.0.4/rubpy/types/update.py
--rw-rw-rw-   0        0        0     4530 2024-02-24 22:36:34.000000 rubpy-7.0.4/rubpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-07 00:09:05.584921 rubpy-7.0.4/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3721 2024-05-07 00:09:05.000000 rubpy-7.0.4/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8875 2024-05-07 00:09:05.000000 rubpy-7.0.4/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 00:09:05.000000 rubpy-7.0.4/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2024-05-07 00:09:05.000000 rubpy-7.0.4/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-07 00:09:05.000000 rubpy-7.0.4/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 00:09:05.850391 rubpy-7.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1838 2024-05-07 00:08:41.000000 rubpy-7.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.114991 rubpy-7.0.5/
+-rw-rw-rw-   0        0        0     3721 2024-05-15 01:21:49.114014 rubpy-7.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2024-03-14 02:30:28.000000 rubpy-7.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.545721 rubpy-7.0.5/rubpy/
+-rw-rw-rw-   0        0        0      488 2024-05-15 01:16:47.000000 rubpy-7.0.5/rubpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.602328 rubpy-7.0.5/rubpy/bots/
+-rw-rw-rw-   0        0        0        0 2024-01-08 21:58:47.000000 rubpy-7.0.5/rubpy/bots/__init__.py
+-rw-rw-rw-   0        0        0    11161 2024-01-08 22:59:16.000000 rubpy-7.0.5/rubpy/bots/client.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.834773 rubpy-7.0.5/rubpy/bots/types/
+-rw-rw-rw-   0        0        0     1077 2024-01-08 22:47:11.000000 rubpy-7.0.5/rubpy/bots/types/__init__.py
+-rw-rw-rw-   0        0        0      163 2024-01-08 22:26:46.000000 rubpy-7.0.5/rubpy/bots/types/aux_data.py
+-rw-rw-rw-   0        0        0      255 2024-01-08 22:11:16.000000 rubpy-7.0.5/rubpy/bots/types/bot.py
+-rw-rw-rw-   0        0        0      102 2024-01-08 22:11:52.000000 rubpy-7.0.5/rubpy/bots/types/bot_command.py
+-rw-rw-rw-   0        0        0     1093 2024-01-08 22:29:20.000000 rubpy-7.0.5/rubpy/bots/types/button.py
+-rw-rw-rw-   0        0        0      225 2024-01-08 22:20:24.000000 rubpy-7.0.5/rubpy/bots/types/button_calendar.py
+-rw-rw-rw-   0        0        0      286 2024-01-08 22:25:55.000000 rubpy-7.0.5/rubpy/bots/types/button_location.py
+-rw-rw-rw-   0        0        0      191 2024-01-08 22:21:11.000000 rubpy-7.0.5/rubpy/bots/types/button_number_picker.py
+-rw-rw-rw-   0        0        0      377 2024-01-08 22:19:28.000000 rubpy-7.0.5/rubpy/bots/types/button_selection.py
+-rw-rw-rw-   0        0        0      195 2024-01-08 22:18:19.000000 rubpy-7.0.5/rubpy/bots/types/button_selection_item.py
+-rw-rw-rw-   0        0        0      159 2024-01-08 22:22:12.000000 rubpy-7.0.5/rubpy/bots/types/button_string_picker.py
+-rw-rw-rw-   0        0        0      255 2024-01-08 22:24:13.000000 rubpy-7.0.5/rubpy/bots/types/button_textbox.py
+-rw-rw-rw-   0        0        0      257 2024-01-08 22:02:54.000000 rubpy-7.0.5/rubpy/bots/types/chat.py
+-rw-rw-rw-   0        0        0      132 2024-01-08 22:13:08.000000 rubpy-7.0.5/rubpy/bots/types/contact_message.py
+-rw-rw-rw-   0        0        0      111 2024-01-08 22:02:20.000000 rubpy-7.0.5/rubpy/bots/types/file.py
+-rw-rw-rw-   0        0        0      214 2024-01-08 22:03:18.000000 rubpy-7.0.5/rubpy/bots/types/forwarded_from.py
+-rw-rw-rw-   0        0        0      340 2024-01-08 22:36:23.000000 rubpy-7.0.5/rubpy/bots/types/inline_message.py
+-rw-rw-rw-   0        0        0      232 2024-01-08 22:30:58.000000 rubpy-7.0.5/rubpy/bots/types/keypad.py
+-rw-rw-rw-   0        0        0      141 2024-01-08 22:30:09.000000 rubpy-7.0.5/rubpy/bots/types/keypad_row.py
+-rw-rw-rw-   0        0        0      340 2024-01-08 22:17:29.000000 rubpy-7.0.5/rubpy/bots/types/live_location.py
+-rw-rw-rw-   0        0        0       99 2024-01-08 22:15:36.000000 rubpy-7.0.5/rubpy/bots/types/location.py
+-rw-rw-rw-   0        0        0      107 2024-01-08 22:09:39.000000 rubpy-7.0.5/rubpy/bots/types/messaage_text_update.py
+-rw-rw-rw-   0        0        0      887 2024-01-08 22:34:09.000000 rubpy-7.0.5/rubpy/bots/types/message.py
+-rw-rw-rw-   0        0        0      149 2024-01-08 22:31:58.000000 rubpy-7.0.5/rubpy/bots/types/message_keypad_update.py
+-rw-rw-rw-   0        0        0      156 2024-01-08 22:03:44.000000 rubpy-7.0.5/rubpy/bots/types/payment_status.py
+-rw-rw-rw-   0        0        0      192 2024-01-08 22:14:43.000000 rubpy-7.0.5/rubpy/bots/types/poll.py
+-rw-rw-rw-   0        0        0      248 2024-01-08 22:13:58.000000 rubpy-7.0.5/rubpy/bots/types/poll_status.py
+-rw-rw-rw-   0        0        0      148 2024-01-08 22:12:28.000000 rubpy-7.0.5/rubpy/bots/types/sticker.py
+-rw-rw-rw-   0        0        0      455 2024-01-08 22:35:18.000000 rubpy-7.0.5/rubpy/bots/types/update.py
+-rw-rw-rw-   0        0        0     5954 2024-05-15 01:20:31.000000 rubpy-7.0.5/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.835747 rubpy-7.0.5/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-7.0.5/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     5386 2024-04-24 22:40:45.000000 rubpy-7.0.5/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.903091 rubpy-7.0.5/rubpy/enums/
+-rw-rw-rw-   0        0        0      320 2024-04-24 21:33:03.000000 rubpy-7.0.5/rubpy/enums/__init__.py
+-rw-rw-rw-   0        0        0      633 2024-02-03 10:53:26.000000 rubpy-7.0.5/rubpy/enums/chat_access_type.py
+-rw-rw-rw-   0        0        0      214 2024-02-03 10:54:38.000000 rubpy-7.0.5/rubpy/enums/chat_action.py
+-rw-rw-rw-   0        0        0      370 2024-01-11 13:02:06.000000 rubpy-7.0.5/rubpy/enums/chat_type.py
+-rw-rw-rw-   0        0        0      568 2024-04-06 22:47:37.000000 rubpy-7.0.5/rubpy/enums/message_media_type.py
+-rw-rw-rw-   0        0        0      100 2024-02-10 16:11:46.000000 rubpy-7.0.5/rubpy/enums/parse_mode.py
+-rw-rw-rw-   0        0        0      133 2024-01-11 13:07:44.000000 rubpy-7.0.5/rubpy/enums/poll_type.py
+-rw-rw-rw-   0        0        0     1767 2024-01-16 12:03:08.000000 rubpy-7.0.5/rubpy/enums/reaction_type.py
+-rw-rw-rw-   0        0        0      280 2024-04-24 21:38:53.000000 rubpy-7.0.5/rubpy/enums/report_type.py
+-rw-rw-rw-   0        0        0     1942 2024-01-08 22:38:06.000000 rubpy-7.0.5/rubpy/exceptions.py
+-rw-rw-rw-   0        0        0    11833 2024-05-15 01:16:18.000000 rubpy-7.0.5/rubpy/filters.py
+-rw-rw-rw-   0        0        0     4886 2024-02-24 22:37:29.000000 rubpy-7.0.5/rubpy/handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.904066 rubpy-7.0.5/rubpy/methods/
+-rw-rw-rw-   0        0        0      697 2024-02-23 15:20:39.000000 rubpy-7.0.5/rubpy/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.906994 rubpy-7.0.5/rubpy/methods/advanced/
+-rw-rw-rw-   0        0        0      143 2024-02-22 17:41:57.000000 rubpy-7.0.5/rubpy/methods/advanced/__init__.py
+-rw-rw-rw-   0        0        0     2312 2024-03-14 01:56:23.000000 rubpy-7.0.5/rubpy/methods/advanced/build.py
+-rw-rw-rw-   0        0        0     4483 2024-02-25 17:08:53.000000 rubpy-7.0.5/rubpy/methods/advanced/voice_chat_player.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.911875 rubpy-7.0.5/rubpy/methods/auth/
+-rw-rw-rw-   0        0        0      185 2023-12-15 18:54:26.000000 rubpy-7.0.5/rubpy/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     2007 2024-03-09 18:53:42.000000 rubpy-7.0.5/rubpy/methods/auth/register_device.py
+-rw-rw-rw-   0        0        0      798 2024-02-24 22:49:22.000000 rubpy-7.0.5/rubpy/methods/auth/send_code.py
+-rw-rw-rw-   0        0        0      576 2024-02-24 22:51:51.000000 rubpy-7.0.5/rubpy/methods/auth/sign_in.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.933883 rubpy-7.0.5/rubpy/methods/channels/
+-rw-rw-rw-   0        0        0     1826 2024-01-22 20:05:38.000000 rubpy-7.0.5/rubpy/methods/channels/__init__.py
+-rw-rw-rw-   0        0        0     1042 2024-02-24 22:53:48.000000 rubpy-7.0.5/rubpy/methods/channels/add_channel.py
+-rw-rw-rw-   0        0        0      882 2024-02-24 22:53:29.000000 rubpy-7.0.5/rubpy/methods/channels/add_channel_members.py
+-rw-rw-rw-   0        0        0     1065 2024-02-24 22:54:12.000000 rubpy-7.0.5/rubpy/methods/channels/ban_channel_member.py
+-rw-rw-rw-   0        0        0      613 2024-02-24 22:54:34.000000 rubpy-7.0.5/rubpy/methods/channels/channel_preview_by_join_link.py
+-rw-rw-rw-   0        0        0      574 2024-02-24 22:54:51.000000 rubpy-7.0.5/rubpy/methods/channels/check_channel_username.py
+-rw-rw-rw-   0        0        0      523 2024-02-24 22:55:07.000000 rubpy-7.0.5/rubpy/methods/channels/create_channel_voice_chat.py
+-rw-rw-rw-   0        0        0      748 2024-02-24 22:55:21.000000 rubpy-7.0.5/rubpy/methods/channels/discard_channel_voice_chat.py
+-rw-rw-rw-   0        0        0     2601 2024-02-24 22:55:49.000000 rubpy-7.0.5/rubpy/methods/channels/edit_channel_info.py
+-rw-rw-rw-   0        0        0      705 2024-02-24 22:56:18.000000 rubpy-7.0.5/rubpy/methods/channels/get_banned_group_members.py
+-rw-rw-rw-   0        0        0      681 2024-02-24 22:56:34.000000 rubpy-7.0.5/rubpy/methods/channels/get_channel_admin_access_list.py
+-rw-rw-rw-   0        0        0      681 2024-02-24 22:56:52.000000 rubpy-7.0.5/rubpy/methods/channels/get_channel_admin_members.py
+-rw-rw-rw-   0        0        0      819 2024-02-24 22:58:08.000000 rubpy-7.0.5/rubpy/methods/channels/get_channel_all_members.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 22:58:25.000000 rubpy-7.0.5/rubpy/methods/channels/get_channel_info.py
+-rw-rw-rw-   0        0        0      503 2024-02-24 22:58:39.000000 rubpy-7.0.5/rubpy/methods/channels/get_channel_link.py
+-rw-rw-rw-   0        0        0      996 2024-02-24 22:58:58.000000 rubpy-7.0.5/rubpy/methods/channels/join_channel_action.py
+-rw-rw-rw-   0        0        0      609 2024-02-24 22:59:21.000000 rubpy-7.0.5/rubpy/methods/channels/join_channel_by_link.py
+-rw-rw-rw-   0        0        0      610 2024-02-24 22:59:38.000000 rubpy-7.0.5/rubpy/methods/channels/remove_channel.py
+-rw-rw-rw-   0        0        0      956 2024-02-24 23:00:34.000000 rubpy-7.0.5/rubpy/methods/channels/seen_channel_messages.py
+-rw-rw-rw-   0        0        0      631 2024-02-24 23:00:59.000000 rubpy-7.0.5/rubpy/methods/channels/set_channel_link.py
+-rw-rw-rw-   0        0        0     1051 2024-02-24 23:01:17.000000 rubpy-7.0.5/rubpy/methods/channels/set_channel_voice_chat_setting.py
+-rw-rw-rw-   0        0        0      772 2024-02-24 23:01:35.000000 rubpy-7.0.5/rubpy/methods/channels/update_channel_username.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.947546 rubpy-7.0.5/rubpy/methods/chats/
+-rw-rw-rw-   0        0        0      807 2023-12-20 14:35:52.000000 rubpy-7.0.5/rubpy/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0      806 2024-02-24 23:02:06.000000 rubpy-7.0.5/rubpy/methods/chats/delete_avatar.py
+-rw-rw-rw-   0        0        0      966 2024-02-24 23:02:35.000000 rubpy-7.0.5/rubpy/methods/chats/delete_chat_history.py
+-rw-rw-rw-   0        0        0      790 2024-02-24 23:02:59.000000 rubpy-7.0.5/rubpy/methods/chats/get_abs_objects.py
+-rw-rw-rw-   0        0        0      636 2024-02-24 23:03:23.000000 rubpy-7.0.5/rubpy/methods/chats/get_avatars.py
+-rw-rw-rw-   0        0        0      601 2024-02-24 23:05:28.000000 rubpy-7.0.5/rubpy/methods/chats/get_chats.py
+-rw-rw-rw-   0        0        0      745 2024-02-24 23:04:22.000000 rubpy-7.0.5/rubpy/methods/chats/get_chats_updates.py
+-rw-rw-rw-   0        0        0      599 2024-02-24 23:08:10.000000 rubpy-7.0.5/rubpy/methods/chats/get_link_from_app_url.py
+-rw-rw-rw-   0        0        0     1265 2024-02-24 23:08:43.000000 rubpy-7.0.5/rubpy/methods/chats/search_chat_messages.py
+-rw-rw-rw-   0        0        0      611 2024-02-24 23:10:47.000000 rubpy-7.0.5/rubpy/methods/chats/seen_chats.py
+-rw-rw-rw-   0        0        0     1110 2024-02-24 23:11:34.000000 rubpy-7.0.5/rubpy/methods/chats/send_chat_activity.py
+-rw-rw-rw-   0        0        0     1014 2024-02-24 23:12:16.000000 rubpy-7.0.5/rubpy/methods/chats/set_action_chat.py
+-rw-rw-rw-   0        0        0     1818 2024-02-24 23:13:42.000000 rubpy-7.0.5/rubpy/methods/chats/upload_avatar.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.952427 rubpy-7.0.5/rubpy/methods/contacts/
+-rw-rw-rw-   0        0        0      299 2023-12-22 14:16:01.000000 rubpy-7.0.5/rubpy/methods/contacts/__init__.py
+-rw-rw-rw-   0        0        0     1247 2024-02-24 23:15:53.000000 rubpy-7.0.5/rubpy/methods/contacts/add_address_book.py
+-rw-rw-rw-   0        0        0      753 2024-02-24 23:16:17.000000 rubpy-7.0.5/rubpy/methods/contacts/delete_contact.py
+-rw-rw-rw-   0        0        0      622 2024-02-24 23:18:12.000000 rubpy-7.0.5/rubpy/methods/contacts/get_contacts.py
+-rw-rw-rw-   0        0        0      770 2024-02-24 23:17:44.000000 rubpy-7.0.5/rubpy/methods/contacts/get_contacts_updates.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.959258 rubpy-7.0.5/rubpy/methods/decorators/
+-rw-rw-rw-   0        0        0      415 2023-12-25 13:18:28.000000 rubpy-7.0.5/rubpy/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0      592 2024-02-24 23:18:27.000000 rubpy-7.0.5/rubpy/methods/decorators/on_chat_updates.py
+-rw-rw-rw-   0        0        0      604 2024-02-24 23:18:42.000000 rubpy-7.0.5/rubpy/methods/decorators/on_message_updates.py
+-rw-rw-rw-   0        0        0      624 2024-02-24 23:18:56.000000 rubpy-7.0.5/rubpy/methods/decorators/on_remove_notifications.py
+-rw-rw-rw-   0        0        0      604 2024-02-24 23:19:09.000000 rubpy-7.0.5/rubpy/methods/decorators/on_show_activities.py
+-rw-rw-rw-   0        0        0      616 2024-02-24 23:19:21.000000 rubpy-7.0.5/rubpy/methods/decorators/on_show_notifications.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.978779 rubpy-7.0.5/rubpy/methods/extras/
+-rw-rw-rw-   0        0        0      745 2024-02-15 12:50:33.000000 rubpy-7.0.5/rubpy/methods/extras/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-02-24 23:19:55.000000 rubpy-7.0.5/rubpy/methods/extras/ban_member.py
+-rw-rw-rw-   0        0        0     1039 2024-02-24 23:20:10.000000 rubpy-7.0.5/rubpy/methods/extras/get_info.py
+-rw-rw-rw-   0        0        0      693 2024-02-24 23:20:43.000000 rubpy-7.0.5/rubpy/methods/extras/get_object_by_username.py
+-rw-rw-rw-   0        0        0      538 2024-02-24 23:21:03.000000 rubpy-7.0.5/rubpy/methods/extras/get_profile_link_items.py
+-rw-rw-rw-   0        0        0      530 2024-02-24 23:21:19.000000 rubpy-7.0.5/rubpy/methods/extras/get_related_objects.py
+-rw-rw-rw-   0        0        0      770 2024-02-24 23:22:06.000000 rubpy-7.0.5/rubpy/methods/extras/get_transcription.py
+-rw-rw-rw-   0        0        0      690 2024-02-24 23:22:29.000000 rubpy-7.0.5/rubpy/methods/extras/join.py
+-rw-rw-rw-   0        0        0      648 2024-02-24 23:22:49.000000 rubpy-7.0.5/rubpy/methods/extras/leave_chat.py
+-rw-rw-rw-   0        0        0     1305 2024-04-24 21:38:46.000000 rubpy-7.0.5/rubpy/methods/extras/report_object.py
+-rw-rw-rw-   0        0        0      665 2024-02-24 23:24:05.000000 rubpy-7.0.5/rubpy/methods/extras/search_global_objects.py
+-rw-rw-rw-   0        0        0      695 2024-02-24 23:25:58.000000 rubpy-7.0.5/rubpy/methods/extras/transcribe_voice.py
+-rw-rw-rw-   0        0        0     1019 2024-02-24 23:26:53.000000 rubpy-7.0.5/rubpy/methods/extras/user_is_admin.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.982683 rubpy-7.0.5/rubpy/methods/gif/
+-rw-rw-rw-   0        0        0      235 2024-01-09 12:00:36.000000 rubpy-7.0.5/rubpy/methods/gif/__init__.py
+-rw-rw-rw-   0        0        0      611 2024-02-24 23:27:54.000000 rubpy-7.0.5/rubpy/methods/gif/add_to_my_gif_set.py
+-rw-rw-rw-   0        0        0      341 2024-02-24 23:28:10.000000 rubpy-7.0.5/rubpy/methods/gif/get_my_gif_set.py
+-rw-rw-rw-   0        0        0      430 2024-02-24 23:28:39.000000 rubpy-7.0.5/rubpy/methods/gif/remove_from_my_gif_set.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.007083 rubpy-7.0.5/rubpy/methods/groups/
+-rw-rw-rw-   0        0        0     1857 2023-12-22 17:47:50.000000 rubpy-7.0.5/rubpy/methods/groups/__init__.py
+-rw-rw-rw-   0        0        0      987 2024-02-24 23:33:24.000000 rubpy-7.0.5/rubpy/methods/groups/add_group.py
+-rw-rw-rw-   0        0        0      958 2024-02-24 23:29:42.000000 rubpy-7.0.5/rubpy/methods/groups/add_group_members.py
+-rw-rw-rw-   0        0        0     1229 2024-02-24 23:33:49.000000 rubpy-7.0.5/rubpy/methods/groups/ban_group_member.py
+-rw-rw-rw-   0        0        0      600 2024-02-24 23:34:06.000000 rubpy-7.0.5/rubpy/methods/groups/create_group_voice_chat.py
+-rw-rw-rw-   0        0        0      618 2024-02-24 23:34:23.000000 rubpy-7.0.5/rubpy/methods/groups/delete_no_access_group_chat.py
+-rw-rw-rw-   0        0        0     2648 2024-02-24 23:34:53.000000 rubpy-7.0.5/rubpy/methods/groups/edit_group_info.py
+-rw-rw-rw-   0        0        0      785 2024-02-24 23:35:11.000000 rubpy-7.0.5/rubpy/methods/groups/get_banned_group_members.py
+-rw-rw-rw-   0        0        0      820 2024-02-24 23:35:36.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_admin_access_list.py
+-rw-rw-rw-   0        0        0      791 2024-02-24 23:35:53.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_admin_members.py
+-rw-rw-rw-   0        0        0     1003 2024-02-25 13:45:13.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_all_members.py
+-rw-rw-rw-   0        0        0      644 2024-02-24 23:36:57.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_default_access.py
+-rw-rw-rw-   0        0        0      584 2024-02-24 23:37:09.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_info.py
+-rw-rw-rw-   0        0        0      578 2024-02-24 23:37:26.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_link.py
+-rw-rw-rw-   0        0        0      787 2024-02-24 23:37:39.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_mention_list.py
+-rw-rw-rw-   0        0        0     1096 2024-02-24 23:38:09.000000 rubpy-7.0.5/rubpy/methods/groups/get_group_voice_chat_updates.py
+-rw-rw-rw-   0        0        0      688 2024-02-24 23:38:23.000000 rubpy-7.0.5/rubpy/methods/groups/group_preview_by_join_link.py
+-rw-rw-rw-   0        0        0      645 2024-02-24 23:38:40.000000 rubpy-7.0.5/rubpy/methods/groups/join_group.py
+-rw-rw-rw-   0        0        0      460 2024-02-24 23:39:16.000000 rubpy-7.0.5/rubpy/methods/groups/leave_group.py
+-rw-rw-rw-   0        0        0      784 2024-02-24 23:38:58.000000 rubpy-7.0.5/rubpy/methods/groups/leave_group_voice_chat.py
+-rw-rw-rw-   0        0        0      466 2024-02-24 23:39:33.000000 rubpy-7.0.5/rubpy/methods/groups/remove_group.py
+-rw-rw-rw-   0        0        0     1549 2024-02-24 23:40:14.000000 rubpy-7.0.5/rubpy/methods/groups/set_group_admin.py
+-rw-rw-rw-   0        0        0      920 2024-02-24 23:42:43.000000 rubpy-7.0.5/rubpy/methods/groups/set_group_default_access.py
+-rw-rw-rw-   0        0        0      596 2024-02-24 23:45:52.000000 rubpy-7.0.5/rubpy/methods/groups/set_group_link.py
+-rw-rw-rw-   0        0        0      980 2024-02-24 23:49:50.000000 rubpy-7.0.5/rubpy/methods/groups/set_group_voice_chat_setting.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.033978 rubpy-7.0.5/rubpy/methods/messages/
+-rw-rw-rw-   0        0        0     1808 2024-02-25 13:57:52.000000 rubpy-7.0.5/rubpy/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0     1431 2024-02-25 13:21:28.000000 rubpy-7.0.5/rubpy/methods/messages/action_on_message_reaction.py
+-rw-rw-rw-   0        0        0     1148 2024-02-25 13:22:34.000000 rubpy-7.0.5/rubpy/methods/messages/auto_delete_message.py
+-rw-rw-rw-   0        0        0     2603 2024-02-25 13:23:17.000000 rubpy-7.0.5/rubpy/methods/messages/create_poll.py
+-rw-rw-rw-   0        0        0     1550 2024-02-25 13:24:10.000000 rubpy-7.0.5/rubpy/methods/messages/delete_messages.py
+-rw-rw-rw-   0        0        0     1633 2024-02-25 13:25:45.000000 rubpy-7.0.5/rubpy/methods/messages/edit_message.py
+-rw-rw-rw-   0        0        0     1635 2024-02-25 13:27:51.000000 rubpy-7.0.5/rubpy/methods/messages/forward_messages.py
+-rw-rw-rw-   0        0        0     1044 2024-03-14 20:52:58.000000 rubpy-7.0.5/rubpy/methods/messages/get_message_share_url.py
+-rw-rw-rw-   0        0        0     1193 2024-02-25 13:28:35.000000 rubpy-7.0.5/rubpy/methods/messages/get_messages_by_id.py
+-rw-rw-rw-   0        0        0     1245 2024-02-25 13:28:56.000000 rubpy-7.0.5/rubpy/methods/messages/get_messages_interval.py
+-rw-rw-rw-   0        0        0     1165 2024-02-25 13:29:20.000000 rubpy-7.0.5/rubpy/methods/messages/get_messages_updates.py
+-rw-rw-rw-   0        0        0     1250 2024-02-25 13:31:15.000000 rubpy-7.0.5/rubpy/methods/messages/get_poll_option_voters.py
+-rw-rw-rw-   0        0        0      823 2024-02-25 13:31:35.000000 rubpy-7.0.5/rubpy/methods/messages/get_poll_status.py
+-rw-rw-rw-   0        0        0     1090 2024-02-25 13:31:55.000000 rubpy-7.0.5/rubpy/methods/messages/reaction.py
+-rw-rw-rw-   0        0        0     1136 2024-02-25 13:32:18.000000 rubpy-7.0.5/rubpy/methods/messages/remove_reaction.py
+-rw-rw-rw-   0        0        0     1156 2024-02-25 13:32:38.000000 rubpy-7.0.5/rubpy/methods/messages/request_send_file.py
+-rw-rw-rw-   0        0        0     1515 2024-02-25 13:32:59.000000 rubpy-7.0.5/rubpy/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     1248 2024-02-25 13:35:35.000000 rubpy-7.0.5/rubpy/methods/messages/send_gif.py
+-rw-rw-rw-   0        0        0     7849 2024-05-07 00:06:38.000000 rubpy-7.0.5/rubpy/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     1266 2024-02-25 13:35:46.000000 rubpy-7.0.5/rubpy/methods/messages/send_music.py
+-rw-rw-rw-   0        0        0     1492 2024-02-25 13:35:55.000000 rubpy-7.0.5/rubpy/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     1785 2024-02-25 13:45:22.000000 rubpy-7.0.5/rubpy/methods/messages/send_sticker.py
+-rw-rw-rw-   0        0        0     1236 2024-02-25 13:45:25.000000 rubpy-7.0.5/rubpy/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     1374 2024-02-25 13:45:23.000000 rubpy-7.0.5/rubpy/methods/messages/send_video_message.py
+-rw-rw-rw-   0        0        0     1384 2024-02-25 13:44:36.000000 rubpy-7.0.5/rubpy/methods/messages/send_voice.py
+-rw-rw-rw-   0        0        0     2422 2024-02-25 13:43:55.000000 rubpy-7.0.5/rubpy/methods/messages/set_pin_message.py
+-rw-rw-rw-   0        0        0      799 2024-02-25 13:44:20.000000 rubpy-7.0.5/rubpy/methods/messages/vote_poll.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.045690 rubpy-7.0.5/rubpy/methods/settings/
+-rw-rw-rw-   0        0        0      878 2023-12-22 15:33:50.000000 rubpy-7.0.5/rubpy/methods/settings/__init__.py
+-rw-rw-rw-   0        0        0      746 2024-02-25 13:16:01.000000 rubpy-7.0.5/rubpy/methods/settings/delete_folder.py
+-rw-rw-rw-   0        0        0      586 2024-02-25 13:17:26.000000 rubpy-7.0.5/rubpy/methods/settings/get_blocked_users.py
+-rw-rw-rw-   0        0        0      832 2024-02-25 13:17:43.000000 rubpy-7.0.5/rubpy/methods/settings/get_folders.py
+-rw-rw-rw-   0        0        0      660 2024-02-25 13:18:03.000000 rubpy-7.0.5/rubpy/methods/settings/get_my_sessions.py
+-rw-rw-rw-   0        0        0      640 2024-02-25 13:18:19.000000 rubpy-7.0.5/rubpy/methods/settings/get_privacy_setting.py
+-rw-rw-rw-   0        0        0      648 2024-02-25 13:18:36.000000 rubpy-7.0.5/rubpy/methods/settings/get_suggested_folders.py
+-rw-rw-rw-   0        0        0      662 2024-02-25 13:18:52.000000 rubpy-7.0.5/rubpy/methods/settings/get_two_passcode_status.py
+-rw-rw-rw-   0        0        0     3312 2024-02-25 13:19:21.000000 rubpy-7.0.5/rubpy/methods/settings/set_setting.py
+-rw-rw-rw-   0        0        0     1267 2024-02-25 13:20:00.000000 rubpy-7.0.5/rubpy/methods/settings/setup_two_step_verification.py
+-rw-rw-rw-   0        0        0      801 2024-02-25 13:20:16.000000 rubpy-7.0.5/rubpy/methods/settings/terminate_session.py
+-rw-rw-rw-   0        0        0     1663 2024-02-25 13:20:39.000000 rubpy-7.0.5/rubpy/methods/settings/update_profile.py
+-rw-rw-rw-   0        0        0      745 2024-02-25 13:20:56.000000 rubpy-7.0.5/rubpy/methods/settings/update_username.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.053499 rubpy-7.0.5/rubpy/methods/stickers/
+-rw-rw-rw-   0        0        0      578 2023-12-22 16:07:24.000000 rubpy-7.0.5/rubpy/methods/stickers/__init__.py
+-rw-rw-rw-   0        0        0     1283 2024-02-25 13:08:37.000000 rubpy-7.0.5/rubpy/methods/stickers/action_on_sticker_set.py
+-rw-rw-rw-   0        0        0      564 2024-02-25 13:09:11.000000 rubpy-7.0.5/rubpy/methods/stickers/get_my_sticker_sets.py
+-rw-rw-rw-   0        0        0      778 2024-02-25 13:09:47.000000 rubpy-7.0.5/rubpy/methods/stickers/get_sticker_set_by_id.py
+-rw-rw-rw-   0        0        0      877 2024-02-25 13:45:26.000000 rubpy-7.0.5/rubpy/methods/stickers/get_stickers_by_emoji.py
+-rw-rw-rw-   0        0        0      941 2024-02-25 13:14:21.000000 rubpy-7.0.5/rubpy/methods/stickers/get_stickers_by_set_ids.py
+-rw-rw-rw-   0        0        0      766 2024-02-25 13:14:11.000000 rubpy-7.0.5/rubpy/methods/stickers/get_trend_sticker_sets.py
+-rw-rw-rw-   0        0        0      929 2024-02-25 13:14:28.000000 rubpy-7.0.5/rubpy/methods/stickers/search_stickers.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.059353 rubpy-7.0.5/rubpy/methods/users/
+-rw-rw-rw-   0        0        0      331 2023-12-19 22:35:32.000000 rubpy-7.0.5/rubpy/methods/users/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-02-25 13:03:33.000000 rubpy-7.0.5/rubpy/methods/users/check_user_username.py
+-rw-rw-rw-   0        0        0     1042 2024-02-25 13:04:30.000000 rubpy-7.0.5/rubpy/methods/users/delete_user_chat.py
+-rw-rw-rw-   0        0        0      539 2024-02-25 13:05:08.000000 rubpy-7.0.5/rubpy/methods/users/get_me.py
+-rw-rw-rw-   0        0        0      881 2024-02-26 15:47:56.000000 rubpy-7.0.5/rubpy/methods/users/get_user_info.py
+-rw-rw-rw-   0        0        0     1265 2024-02-25 13:06:50.000000 rubpy-7.0.5/rubpy/methods/users/set_block_user.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.098396 rubpy-7.0.5/rubpy/methods/utilities/
+-rw-rw-rw-   0        0        0      613 2024-01-12 14:48:33.000000 rubpy-7.0.5/rubpy/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0      762 2024-02-25 12:47:55.000000 rubpy-7.0.5/rubpy/methods/utilities/add_handler.py
+-rw-rw-rw-   0        0        0      741 2024-04-01 23:10:22.000000 rubpy-7.0.5/rubpy/methods/utilities/audio.py
+-rw-rw-rw-   0        0        0      708 2024-02-26 14:31:15.000000 rubpy-7.0.5/rubpy/methods/utilities/connect.py
+-rw-rw-rw-   0        0        0      574 2024-02-25 12:48:51.000000 rubpy-7.0.5/rubpy/methods/utilities/disconnect.py
+-rw-rw-rw-   0        0        0     1756 2024-04-24 22:13:20.000000 rubpy-7.0.5/rubpy/methods/utilities/download.py
+-rw-rw-rw-   0        0        0     1080 2024-03-20 23:17:03.000000 rubpy-7.0.5/rubpy/methods/utilities/download_profile_picture.py
+-rw-rw-rw-   0        0        0     1419 2024-02-25 12:52:55.000000 rubpy-7.0.5/rubpy/methods/utilities/get_members.py
+-rw-rw-rw-   0        0        0      337 2024-02-25 12:53:13.000000 rubpy-7.0.5/rubpy/methods/utilities/get_updates.py
+-rw-rw-rw-   0        0        0      326 2024-02-25 12:54:09.000000 rubpy-7.0.5/rubpy/methods/utilities/remove_handler.py
+-rw-rw-rw-   0        0        0      967 2024-02-25 12:54:38.000000 rubpy-7.0.5/rubpy/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     3450 2024-05-15 01:17:52.000000 rubpy-7.0.5/rubpy/methods/utilities/start.py
+-rw-rw-rw-   0        0        0     6614 2024-04-06 23:05:13.000000 rubpy-7.0.5/rubpy/methods/utilities/thumbnail.py
+-rw-rw-rw-   0        0        0      671 2024-02-25 13:02:33.000000 rubpy-7.0.5/rubpy/methods/utilities/upload.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.103278 rubpy-7.0.5/rubpy/methods/voice_chat/
+-rw-rw-rw-   0        0        0      278 2024-02-25 16:36:44.000000 rubpy-7.0.5/rubpy/methods/voice_chat/__init__.py
+-rw-rw-rw-   0        0        0      918 2024-02-24 23:57:22.000000 rubpy-7.0.5/rubpy/methods/voice_chat/join_voice_chat.py
+-rw-rw-rw-   0        0        0     1077 2024-02-24 23:55:36.000000 rubpy-7.0.5/rubpy/methods/voice_chat/send_group_voice_chat_activity.py
+-rw-rw-rw-   0        0        0     1181 2024-02-25 16:36:50.000000 rubpy-7.0.5/rubpy/methods/voice_chat/set_voice_chat_state.py
+-rw-rw-rw-   0        0        0    15334 2024-05-15 00:41:47.000000 rubpy-7.0.5/rubpy/network.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.106202 rubpy-7.0.5/rubpy/parser/
+-rw-rw-rw-   0        0        0       30 2024-01-09 13:49:12.000000 rubpy-7.0.5/rubpy/parser/__init__.py
+-rw-rw-rw-   0        0        0     4366 2024-05-14 23:59:01.000000 rubpy-7.0.5/rubpy/parser/markdown.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.108154 rubpy-7.0.5/rubpy/rubino/
+-rw-rw-rw-   0        0        0       26 2024-01-08 21:17:13.000000 rubpy-7.0.5/rubpy/rubino/__init__.py
+-rw-rw-rw-   0        0        0    19933 2024-05-15 00:54:05.000000 rubpy-7.0.5/rubpy/rubino/client.py
+-rw-rw-rw-   0        0        0     8422 2024-05-15 01:09:29.000000 rubpy-7.0.5/rubpy/rubino/thumbnail.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.112059 rubpy-7.0.5/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-7.0.5/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2294 2023-12-19 12:35:20.000000 rubpy-7.0.5/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-7.0.5/rubpy/sessions/stringSession.py
+-rw-rw-rw-   0        0        0     3430 2024-03-14 02:26:10.000000 rubpy-7.0.5/rubpy/sync.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:49.113035 rubpy-7.0.5/rubpy/types/
+-rw-rw-rw-   0        0        0       65 2024-02-24 22:46:34.000000 rubpy-7.0.5/rubpy/types/__init__.py
+-rw-rw-rw-   0        0        0    30721 2024-04-24 22:04:33.000000 rubpy-7.0.5/rubpy/types/update.py
+-rw-rw-rw-   0        0        0     4530 2024-02-24 22:36:34.000000 rubpy-7.0.5/rubpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 01:21:48.584761 rubpy-7.0.5/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3721 2024-05-15 01:21:48.000000 rubpy-7.0.5/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8875 2024-05-15 01:21:48.000000 rubpy-7.0.5/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 01:21:48.000000 rubpy-7.0.5/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2024-05-15 01:21:48.000000 rubpy-7.0.5/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-15 01:21:48.000000 rubpy-7.0.5/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 01:21:49.114991 rubpy-7.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2024-05-15 01:21:26.000000 rubpy-7.0.5/setup.py
```

### Comparing `rubpy-7.0.4/PKG-INFO` & `rubpy-7.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 7.0.4
+Version: 7.0.5
 Summary: A powerful, fast and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 7.0.4 Summary: A powerful, fast and
+Metadata-Version: 2.1 Name: rubpy Version: 7.0.5 Summary: A powerful, fast and
 optimal library for making robots in Rubika with sync and async support. Home-
 page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-
 email: contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-7.0.4/README.md` & `rubpy-7.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/bots/client.py` & `rubpy-7.0.5/rubpy/bots/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/bots/types/__init__.py` & `rubpy-7.0.5/rubpy/bots/types/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/bots/types/button.py` & `rubpy-7.0.5/rubpy/bots/types/button.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/bots/types/message.py` & `rubpy-7.0.5/rubpy/bots/types/message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/client.py` & `rubpy-7.0.5/rubpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .sessions import SQLiteSession, StringSession
 from .parser import Markdown
 from .methods import Methods
 from typing import Optional, Union, Literal
 from . import __name__ as logger_name
 import logging
-#import re
+import rubpy
+import time
 
 
 class Client(Methods):
     DEFAULT_PLATFORM = {
         'app_name': 'Main',
         'app_version': '4.4.9',
         'platform': 'Web',
@@ -133,14 +134,19 @@
         self.decode_auth = None
         self.import_key = None
         self.is_sync = False
         self.guid = None
         self.key = None
         self.handlers = {}
 
+        if self.display_welcome:
+            for char in rubpy.__welcome__:
+                print(char, sep='', end='', flush=True)
+                time.sleep(0.01)
+
     def __enter__(self) -> "Client":
         return self.start()
 
     def __exit__(self, *args, **kwargs):
         try:
             return self.disconnect()
```

### Comparing `rubpy-7.0.4/rubpy/crypto/crypto.py` & `rubpy-7.0.5/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/enums/chat_access_type.py` & `rubpy-7.0.5/rubpy/enums/chat_access_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/enums/message_media_type.py` & `rubpy-7.0.5/rubpy/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/enums/reaction_type.py` & `rubpy-7.0.5/rubpy/enums/reaction_type.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/exceptions.py` & `rubpy-7.0.5/rubpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/filters.py` & `rubpy-7.0.5/rubpy/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import difflib
 import inspect
 import warnings
 import sys
 import re
 
 # List of public elements to be exported
-__all__ = ['Operator', 'BaseModel', 'RegexModel',
-           'AuthorGuids', 'ObjectGuids', 'Commands']
+__all__ = ['Operator', 'BaseModel', 'author_guids', 'object_guids', 'commands', 'regex',
+           'AuthorGuids', 'ObjectGuids', 'Commands', 'RegexModel']
 # List of models for internal use
 __models__ = [
     'is_pinned', 'is_mute', 'count_unseen', 'message_id',
     'is_group', 'is_private', 'is_channel', 'is_in_contact',
     'text', 'original_update', 'object_guid', 'author_guid',
     'time', 'reply_message_id', 'is_me', 'is_forward', 'is_text',
     'music', 'file', 'photo', 'sticker', 'video', 'voice',
@@ -148,22 +148,22 @@
 
         return bool(result)
 
     async def __call__(self, update, *args, **kwargs):
         return await self.build(update)
 
 
-class Commands(BaseModel):
+class commands(BaseModel):
     """
     Filter for commands in text messages.
     """
     def __init__(
             self,
             commands: Union[str, List[str]],
-            prefixes: Union[str, List[str]] = "/",
+            prefixes: Union[str, List[str]] = '/',
             case_sensitive: bool = False, *args, **kwargs,
     ) -> None:
         """Filter Commands, i.e.: text messages starting with "/" or any other custom prefix.
 
         Parameters:
             commands (``str`` | ``list``):
                 The command or list of commands as string the filter should look for.
@@ -241,28 +241,14 @@
     async def __call__(self, update, *args, **kwargs) -> bool:
         if update.text is None:
             return False
 
         update.pattern_match = self.pattern.match(update.text)
         return bool(update.pattern_match)
 
-class RegexModel(BaseModel):
-    """
-    Filter for matching text using regular expressions.
-    """
-    def __init__(self, pattern: Pattern, *args, **kwargs) -> None:
-        self.pattern = re.compile(pattern)
-        super().__init__(*args, **kwargs)
-
-    async def __call__(self, update, *args, **kwargs) -> bool:
-        if update.text is None:
-            return False
-
-        update.pattern_match = self.pattern.match(update.text)
-        return bool(update.pattern_match)
 
 class object_guids(BaseModel):
     """
     Filter based on object GUIDs.
     """
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
@@ -272,39 +258,16 @@
                 self.object_guids.extend(arg)
             elif isinstance(arg, tuple):
                 self.object_guids.extend(list(arg))
             else:
                 self.object_guids.append(arg)
 
     async def __call__(self, update, *args, **kwargs) -> bool:
-        if update.object_guid is None:
-            return False
-
-        return update.object_guid in self.object_guids
-
-class ObjectGuids(BaseModel):
-    """
-    Filter based on object GUIDs.
-    """
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-        self.object_guids = []
-        for arg in args:
-            if isinstance(arg, list):
-                self.object_guids.extend(arg)
-            elif isinstance(arg, tuple):
-                self.object_guids.extend(list(arg))
-            else:
-                self.object_guids.append(arg)
-
-    async def __call__(self, update, *args, **kwargs) -> bool:
-        if update.object_guid is None:
-            return False
+        return update.object_guid is not None and update.object_guid in self.object_guids
 
-        return update.object_guid in self.object_guids
 
 class author_guids(BaseModel):
     """
     Filter based on author GUIDs.
     """
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
@@ -314,18 +277,16 @@
                 self.author_guids.extend(arg)
             elif isinstance(arg, tuple):
                 self.author_guids.extend(list(arg))
             else:
                 self.author_guids.append(arg)
 
     async def __call__(self, update, *args, **kwargs) -> bool:
-        if update.author_guid is None:
-            return False
+        return update.author_guid is not None and update.author_guid in self.author_guids
 
-        return update.author_guid in self.author_guids
 
 class Models:
     """
     Class to handle and create specific models.
     """
     def __init__(self, name, *args, **kwargs) -> None:
         self.__name__ = name
@@ -372,8 +333,9 @@
 video: Type[BaseModel]
 voice: Type[BaseModel]
 contact: Type[BaseModel]
 location: Type[BaseModel]
 poll: Type[BaseModel]
 gif: Type[BaseModel]
 sticker: Type[BaseModel]
-is_event: Type[BaseModel]
+is_event: Type[BaseModel]
+AuthorGuids, ObjectGuids, Commands, RegexModel = author_guids, object_guids, commands, regex
```

### Comparing `rubpy-7.0.4/rubpy/handlers.py` & `rubpy-7.0.5/rubpy/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/__init__.py` & `rubpy-7.0.5/rubpy/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/advanced/build.py` & `rubpy-7.0.5/rubpy/methods/advanced/build.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/advanced/voice_chat_player.py` & `rubpy-7.0.5/rubpy/methods/advanced/voice_chat_player.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/auth/register_device.py` & `rubpy-7.0.5/rubpy/methods/auth/register_device.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/auth/send_code.py` & `rubpy-7.0.5/rubpy/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/auth/sign_in.py` & `rubpy-7.0.5/rubpy/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/__init__.py` & `rubpy-7.0.5/rubpy/methods/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/add_channel.py` & `rubpy-7.0.5/rubpy/methods/channels/add_channel.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/add_channel_members.py` & `rubpy-7.0.5/rubpy/methods/channels/add_channel_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/ban_channel_member.py` & `rubpy-7.0.5/rubpy/methods/channels/ban_channel_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/channel_preview_by_join_link.py` & `rubpy-7.0.5/rubpy/methods/channels/channel_preview_by_join_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/check_channel_username.py` & `rubpy-7.0.5/rubpy/methods/channels/check_channel_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/create_channel_voice_chat.py` & `rubpy-7.0.5/rubpy/methods/channels/create_channel_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/discard_channel_voice_chat.py` & `rubpy-7.0.5/rubpy/methods/channels/discard_channel_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/edit_channel_info.py` & `rubpy-7.0.5/rubpy/methods/channels/edit_channel_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/get_banned_group_members.py` & `rubpy-7.0.5/rubpy/methods/channels/get_banned_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/get_channel_admin_access_list.py` & `rubpy-7.0.5/rubpy/methods/channels/get_channel_admin_access_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/get_channel_admin_members.py` & `rubpy-7.0.5/rubpy/methods/channels/get_channel_admin_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/get_channel_all_members.py` & `rubpy-7.0.5/rubpy/methods/channels/get_channel_all_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/join_channel_action.py` & `rubpy-7.0.5/rubpy/methods/channels/join_channel_action.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/join_channel_by_link.py` & `rubpy-7.0.5/rubpy/methods/channels/join_channel_by_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/remove_channel.py` & `rubpy-7.0.5/rubpy/methods/channels/remove_channel.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/seen_channel_messages.py` & `rubpy-7.0.5/rubpy/methods/channels/seen_channel_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/set_channel_link.py` & `rubpy-7.0.5/rubpy/methods/channels/set_channel_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/set_channel_voice_chat_setting.py` & `rubpy-7.0.5/rubpy/methods/channels/set_channel_voice_chat_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/channels/update_channel_username.py` & `rubpy-7.0.5/rubpy/methods/channels/update_channel_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/__init__.py` & `rubpy-7.0.5/rubpy/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/delete_avatar.py` & `rubpy-7.0.5/rubpy/methods/chats/delete_avatar.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/delete_chat_history.py` & `rubpy-7.0.5/rubpy/methods/chats/delete_chat_history.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/get_abs_objects.py` & `rubpy-7.0.5/rubpy/methods/chats/get_abs_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/get_avatars.py` & `rubpy-7.0.5/rubpy/methods/chats/get_avatars.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/get_chats.py` & `rubpy-7.0.5/rubpy/methods/chats/get_chats.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/get_chats_updates.py` & `rubpy-7.0.5/rubpy/methods/chats/get_chats_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/get_link_from_app_url.py` & `rubpy-7.0.5/rubpy/methods/chats/get_link_from_app_url.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/search_chat_messages.py` & `rubpy-7.0.5/rubpy/methods/chats/search_chat_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/seen_chats.py` & `rubpy-7.0.5/rubpy/methods/chats/seen_chats.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/send_chat_activity.py` & `rubpy-7.0.5/rubpy/methods/chats/send_chat_activity.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/set_action_chat.py` & `rubpy-7.0.5/rubpy/methods/chats/set_action_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/chats/upload_avatar.py` & `rubpy-7.0.5/rubpy/methods/chats/upload_avatar.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/contacts/add_address_book.py` & `rubpy-7.0.5/rubpy/methods/contacts/add_address_book.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/contacts/delete_contact.py` & `rubpy-7.0.5/rubpy/methods/contacts/delete_contact.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/contacts/get_contacts.py` & `rubpy-7.0.5/rubpy/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/contacts/get_contacts_updates.py` & `rubpy-7.0.5/rubpy/methods/contacts/get_contacts_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/decorators/on_chat_updates.py` & `rubpy-7.0.5/rubpy/methods/decorators/on_chat_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/decorators/on_message_updates.py` & `rubpy-7.0.5/rubpy/methods/decorators/on_message_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/decorators/on_remove_notifications.py` & `rubpy-7.0.5/rubpy/methods/decorators/on_remove_notifications.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/decorators/on_show_activities.py` & `rubpy-7.0.5/rubpy/methods/decorators/on_show_activities.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/decorators/on_show_notifications.py` & `rubpy-7.0.5/rubpy/methods/decorators/on_show_notifications.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/__init__.py` & `rubpy-7.0.5/rubpy/methods/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/ban_member.py` & `rubpy-7.0.5/rubpy/methods/extras/ban_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/get_info.py` & `rubpy-7.0.5/rubpy/methods/extras/get_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/get_object_by_username.py` & `rubpy-7.0.5/rubpy/methods/extras/get_object_by_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/get_profile_link_items.py` & `rubpy-7.0.5/rubpy/methods/extras/get_profile_link_items.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/get_related_objects.py` & `rubpy-7.0.5/rubpy/methods/extras/get_related_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/get_transcription.py` & `rubpy-7.0.5/rubpy/methods/extras/get_transcription.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/join.py` & `rubpy-7.0.5/rubpy/methods/extras/join.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/leave_chat.py` & `rubpy-7.0.5/rubpy/methods/extras/leave_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/report_object.py` & `rubpy-7.0.5/rubpy/methods/extras/report_object.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/search_global_objects.py` & `rubpy-7.0.5/rubpy/methods/extras/search_global_objects.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/transcribe_voice.py` & `rubpy-7.0.5/rubpy/methods/extras/transcribe_voice.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/extras/user_is_admin.py` & `rubpy-7.0.5/rubpy/methods/extras/user_is_admin.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/gif/add_to_my_gif_set.py` & `rubpy-7.0.5/rubpy/methods/gif/add_to_my_gif_set.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/__init__.py` & `rubpy-7.0.5/rubpy/methods/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/add_group.py` & `rubpy-7.0.5/rubpy/methods/groups/add_group.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/add_group_members.py` & `rubpy-7.0.5/rubpy/methods/groups/add_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/ban_group_member.py` & `rubpy-7.0.5/rubpy/methods/groups/ban_group_member.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/create_group_voice_chat.py` & `rubpy-7.0.5/rubpy/methods/groups/create_group_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/delete_no_access_group_chat.py` & `rubpy-7.0.5/rubpy/methods/groups/delete_no_access_group_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/edit_group_info.py` & `rubpy-7.0.5/rubpy/methods/groups/edit_group_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_banned_group_members.py` & `rubpy-7.0.5/rubpy/methods/groups/get_banned_group_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_admin_access_list.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_admin_access_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_admin_members.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_admin_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_all_members.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_all_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_default_access.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_default_access.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_info.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_link.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_mention_list.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_mention_list.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/get_group_voice_chat_updates.py` & `rubpy-7.0.5/rubpy/methods/groups/get_group_voice_chat_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/group_preview_by_join_link.py` & `rubpy-7.0.5/rubpy/methods/groups/group_preview_by_join_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/join_group.py` & `rubpy-7.0.5/rubpy/methods/groups/join_group.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/leave_group_voice_chat.py` & `rubpy-7.0.5/rubpy/methods/groups/leave_group_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/set_group_admin.py` & `rubpy-7.0.5/rubpy/methods/groups/set_group_admin.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/set_group_default_access.py` & `rubpy-7.0.5/rubpy/methods/groups/set_group_default_access.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/set_group_link.py` & `rubpy-7.0.5/rubpy/methods/groups/set_group_link.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/groups/set_group_voice_chat_setting.py` & `rubpy-7.0.5/rubpy/methods/groups/set_group_voice_chat_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/__init__.py` & `rubpy-7.0.5/rubpy/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/action_on_message_reaction.py` & `rubpy-7.0.5/rubpy/methods/messages/action_on_message_reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/auto_delete_message.py` & `rubpy-7.0.5/rubpy/methods/messages/auto_delete_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/create_poll.py` & `rubpy-7.0.5/rubpy/methods/messages/create_poll.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/delete_messages.py` & `rubpy-7.0.5/rubpy/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/edit_message.py` & `rubpy-7.0.5/rubpy/methods/messages/edit_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/forward_messages.py` & `rubpy-7.0.5/rubpy/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/get_message_share_url.py` & `rubpy-7.0.5/rubpy/methods/messages/get_message_share_url.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/get_messages_by_id.py` & `rubpy-7.0.5/rubpy/methods/messages/get_messages_by_id.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/get_messages_interval.py` & `rubpy-7.0.5/rubpy/methods/messages/get_messages_interval.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/get_messages_updates.py` & `rubpy-7.0.5/rubpy/methods/messages/get_messages_updates.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/get_poll_option_voters.py` & `rubpy-7.0.5/rubpy/methods/messages/get_poll_option_voters.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/get_poll_status.py` & `rubpy-7.0.5/rubpy/methods/messages/get_poll_status.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/reaction.py` & `rubpy-7.0.5/rubpy/methods/messages/reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/remove_reaction.py` & `rubpy-7.0.5/rubpy/methods/messages/remove_reaction.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/request_send_file.py` & `rubpy-7.0.5/rubpy/methods/messages/request_send_file.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_document.py` & `rubpy-7.0.5/rubpy/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_gif.py` & `rubpy-7.0.5/rubpy/methods/messages/send_gif.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_message.py` & `rubpy-7.0.5/rubpy/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_music.py` & `rubpy-7.0.5/rubpy/methods/messages/send_music.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_photo.py` & `rubpy-7.0.5/rubpy/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_sticker.py` & `rubpy-7.0.5/rubpy/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_video.py` & `rubpy-7.0.5/rubpy/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_video_message.py` & `rubpy-7.0.5/rubpy/methods/messages/send_video_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/send_voice.py` & `rubpy-7.0.5/rubpy/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/set_pin_message.py` & `rubpy-7.0.5/rubpy/methods/messages/set_pin_message.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/messages/vote_poll.py` & `rubpy-7.0.5/rubpy/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/__init__.py` & `rubpy-7.0.5/rubpy/methods/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/delete_folder.py` & `rubpy-7.0.5/rubpy/methods/settings/delete_folder.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/get_blocked_users.py` & `rubpy-7.0.5/rubpy/methods/settings/get_blocked_users.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/get_folders.py` & `rubpy-7.0.5/rubpy/methods/settings/get_folders.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/get_my_sessions.py` & `rubpy-7.0.5/rubpy/methods/settings/get_my_sessions.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/get_privacy_setting.py` & `rubpy-7.0.5/rubpy/methods/settings/get_privacy_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/get_suggested_folders.py` & `rubpy-7.0.5/rubpy/methods/settings/get_suggested_folders.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/get_two_passcode_status.py` & `rubpy-7.0.5/rubpy/methods/settings/get_two_passcode_status.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/set_setting.py` & `rubpy-7.0.5/rubpy/methods/settings/set_setting.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/setup_two_step_verification.py` & `rubpy-7.0.5/rubpy/methods/settings/setup_two_step_verification.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/terminate_session.py` & `rubpy-7.0.5/rubpy/methods/settings/terminate_session.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/update_profile.py` & `rubpy-7.0.5/rubpy/methods/settings/update_profile.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/settings/update_username.py` & `rubpy-7.0.5/rubpy/methods/settings/update_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/__init__.py` & `rubpy-7.0.5/rubpy/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/action_on_sticker_set.py` & `rubpy-7.0.5/rubpy/methods/stickers/action_on_sticker_set.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/get_my_sticker_sets.py` & `rubpy-7.0.5/rubpy/methods/stickers/get_my_sticker_sets.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/get_sticker_set_by_id.py` & `rubpy-7.0.5/rubpy/methods/stickers/get_sticker_set_by_id.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/get_stickers_by_emoji.py` & `rubpy-7.0.5/rubpy/methods/stickers/get_stickers_by_emoji.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/get_stickers_by_set_ids.py` & `rubpy-7.0.5/rubpy/methods/stickers/get_stickers_by_set_ids.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/get_trend_sticker_sets.py` & `rubpy-7.0.5/rubpy/methods/stickers/get_trend_sticker_sets.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/stickers/search_stickers.py` & `rubpy-7.0.5/rubpy/methods/stickers/search_stickers.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/users/check_user_username.py` & `rubpy-7.0.5/rubpy/methods/users/check_user_username.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/users/delete_user_chat.py` & `rubpy-7.0.5/rubpy/methods/users/delete_user_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/users/get_me.py` & `rubpy-7.0.5/rubpy/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/users/get_user_info.py` & `rubpy-7.0.5/rubpy/methods/users/get_user_info.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/users/set_block_user.py` & `rubpy-7.0.5/rubpy/methods/users/set_block_user.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/__init__.py` & `rubpy-7.0.5/rubpy/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/add_handler.py` & `rubpy-7.0.5/rubpy/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/audio.py` & `rubpy-7.0.5/rubpy/methods/utilities/audio.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/connect.py` & `rubpy-7.0.5/rubpy/methods/utilities/connect.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/disconnect.py` & `rubpy-7.0.5/rubpy/methods/utilities/disconnect.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/download.py` & `rubpy-7.0.5/rubpy/methods/utilities/download.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/download_profile_picture.py` & `rubpy-7.0.5/rubpy/methods/utilities/download_profile_picture.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/get_members.py` & `rubpy-7.0.5/rubpy/methods/utilities/get_members.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/run.py` & `rubpy-7.0.5/rubpy/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/start.py` & `rubpy-7.0.5/rubpy/methods/utilities/start.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from ... import exceptions
 from ...crypto import Crypto
 from Crypto.PublicKey import RSA
 from Crypto.Signature import pkcs1_15
-import asyncio
 import rubpy
 
 
 class Start:
     async def start(self: "rubpy.Client", phone_number: str = None):
         """
         Start the RubPy client, handling user registration if necessary.
 
         Args:
         - phone_number (str): The phone number to use for starting the client.
 
         Returns:
         - The initialized client.
         """
-        if self.display_welcome:
-            for char in rubpy.__welcome__:
-                print(char, sep='', end='', flush=True)
-                await asyncio.sleep(0.01)
-
         if not hasattr(self, 'connection'):
             await self.connect()
 
         try:
             self.decode_auth = Crypto.decode_auth(self.auth) if self.auth is not None else None
             self.import_key = pkcs1_15.new(RSA.import_key(self.private_key.encode())) if self.private_key is not None else None
             result = await self.get_me()
```

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/thumbnail.py` & `rubpy-7.0.5/rubpy/methods/utilities/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/utilities/upload.py` & `rubpy-7.0.5/rubpy/methods/utilities/upload.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/voice_chat/join_voice_chat.py` & `rubpy-7.0.5/rubpy/methods/voice_chat/join_voice_chat.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/voice_chat/send_group_voice_chat_activity.py` & `rubpy-7.0.5/rubpy/methods/voice_chat/send_group_voice_chat_activity.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/methods/voice_chat/set_voice_chat_state.py` & `rubpy-7.0.5/rubpy/methods/voice_chat/set_voice_chat_state.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/network.py` & `rubpy-7.0.5/rubpy/network.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/parser/markdown.py` & `rubpy-7.0.5/rubpy/parser/markdown.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import markdownify
 import re
 
-MARKDOWN_RE = re.compile(r'\*\*(.*?)\*\*|`(.*?)`|__(.*?)__|--(.*?)--|~~(.*?)~~|\|\|(.*?)\|\||\[(.*?)\]\((\S+)\)')
+MARKDOWN_RE = re.compile(r'```(.*?)```|\*\*(.*?)\*\*|`(.*?)`|__(.*?)__|--(.*?)--|~~(.*?)~~|\|\|(.*?)\|\||\[(.*?)\]\((\S+)\)',
+                         flags=re.DOTALL)
 
 def get_repl(group: str):
-    if group.startswith('**'):
+    if group.startswith('```'):
         return r'\1'
-    elif group.startswith('```'):
+    elif group.startswith('**'):
         return r'\2'
-    elif group.startswith('__'):
+    elif group.startswith('`'):
         return r'\3'
-    elif group.startswith('--'):
+    elif group.startswith('__'):
         return r'\4'
-    elif group.startswith('~~'):
+    elif group.startswith('--'):
         return r'\5'
-    elif group.startswith('||'):
+    elif group.startswith('~~'):
         return r'\6'
-    else:
+    elif group.startswith('||'):
         return r'\7'
+    else:
+        return r'\8'
 
 
 class Markdown:
     def __init__(self) -> None:
         pass
 
     def to_markdown(self, text: str) -> str:
@@ -43,23 +46,28 @@
         Args:
             - text (str): Markdown text.
 
         Returns:
             - Dict[str, Any]: Dictionary containing 'text' and 'metadata' keys.
         """
         meta_data_parts = []
-        text = text.replace('```', '')
 
         while True:
             for find in MARKDOWN_RE.finditer(text):
                 group = find.group()
                 span = find.span()
                 text: str = MARKDOWN_RE.sub(get_repl(group), text, count=1)
 
-                if group.startswith('**'):
+                if group.startswith('```'):
+                    delim_and_language = group[group.find('```'):].split('\n')[0]
+                    language = delim_and_language[len('```'):]
+                    meta_data_parts.append({'type': 'Pre', 'language': language, 'from_index': span[0], 'length': len(group) - 6})
+                    break
+
+                elif group.startswith('**'):
                     meta_data_parts.append({'type': 'Bold', 'from_index': span[0], 'length': len(group) - 4})
                     break
 
                 elif group.startswith('`'):
                     meta_data_parts.append({'type': 'Mono', 'from_index': span[0], 'length': len(group) - 2})
                     break
 
@@ -76,15 +84,15 @@
                     break
 
                 elif group.startswith('||'):
                     meta_data_parts.append({'type': 'Spoiler', 'from_index': span[0], 'length': len(group) - 4})
                     break
 
                 else:
-                    length, url = len(find.group(7)), find.group(8)
+                    length, url = len(find.group(8)), find.group(9)
 
                     if url.startswith('u'):
                         mention_text_object_type = 'User'
                     elif url.startswith('g'):
                         mention_text_object_type = 'Group'
                     elif url.startswith('c'):
                         mention_text_object_type = 'Channel'
```

### Comparing `rubpy-7.0.4/rubpy/rubino/client.py` & `rubpy-7.0.5/rubpy/rubino/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args, **kwargs):
         return
 
     async def _execute_request(self, method: str, data: Dict[str, Union[int, str, bool]]) -> Update:
+        if not hasattr(self.client, 'connection'):
+            await self.client.connect()
+
         result = await self.client.connection.send(
             api_version='0',
             input=data,
             method=method,
             url=self.url,
             client=self.DEFAULT_PLATFORM,
         )
@@ -226,81 +229,77 @@
 
     async def remove_page(self, profile_id: str, record_id: str) -> dict:
         return await self._execute_request('removeRecord', {'model': 'Profile', 'record_id': record_id, 'profile_id': profile_id})
 
     async def upload_file(self, file, profile_id: str, file_type: str, file_name: str = None, chunk: int = 1048576,
                           callback=None, *args, **kwargs):
         """
-        Upload a file to Rubika.
-
-        Parameters:
-        - file: File path or bytes.
-        - mime: MIME type of the file.
-        - file_name: Name of the file.
-        - chunk: Chunk size for uploading.
-        - callback: Progress callback.
+         Upload a file to Rubino.
 
-        Returns:
-        Results object.
-        """
+         Parameters:
+         - file: File path or bytes.
+         - mime: MIME type of the file.
+         - file_name: Name of the file.
+         - chunk: Chunk size for uploading.
+         - callback: Progress callback.
+
+         Returns:
+         Results object.
+         """
         if isinstance(file, str):
             if not os.path.exists(file):
                 raise ValueError('File not found in the given path')
 
             if file_name is None:
                 file_name = os.path.basename(file)
 
-            async with aiofiles.open(file, 'rb+') as file:
+            async with aiofiles.open(file, 'rb') as file:
                 file = await file.read()
 
         elif not isinstance(file, bytes):
             raise TypeError('File argument must be a file path or bytes')
 
         if file_name is None:
             raise ValueError('File name is not set')
 
         result = await self.request_upload_file(profile_id, file_name, len(file), file_type)
 
         id = result.file_id
         index = 0
-        count_retry = 0
-        max_retring = 3
         total = int(len(file) / chunk + 1)
         upload_url = result.server_url
         hash_file_request = result.hash_file_request
 
         while index < total:
-            if count_retry == max_retring:
-                break
-
             data = file[index * chunk: index * chunk + chunk]
             try:
                 response = await self.client.connection.session.post(
-                    upload_url,
+                    url=upload_url,
                     headers={
                         'auth': self.client.auth,
                         'file-id': id,
                         'total-part': str(total),
                         'part-number': str(index + 1),
                         'chunk-size': str(len(data)),
                         'hash-file-request': hash_file_request
                     },
                     data=data,
                     proxy=self.client.proxy,
                 )
                 response = await response.json()
+                self.client.logger.info(rf'UploadFile({file_name}) | Rubino | response={response}')
 
-                if response.get('status') != 'OK':
+                if response.get('status') == 'ERROR_TRY_AGAIN':
                     result = await self.request_upload_file(profile_id, file_name, len(file), file_type)
                     id = result.file_id
                     index = 0
                     total = int(len(file) / chunk + 1)
                     upload_url = result.server_url
                     hash_file_request = result.hash_file_request
-                    count_retry += 1
+                    continue
 
                 if callable(callback):
                     try:
                         if inspect.iscoroutinefunction(callback):
                             await callback(len(file), index * chunk)
 
                         else:
@@ -311,25 +310,126 @@
 
                     except Exception:
                         pass
 
                 index += 1
 
             except Exception:
-                pass
+                self.client.logger.error(
+                    f'UploadFile({file_name}) | Messenger | raised an exception',
+                    extra={'data': self.url}, exc_info=True)
 
         status = response['status']
         status_det = response['status_det']
-
+    
         if status == 'OK' and status_det == 'OK':
             response.update(result.original_update)
             return Update(response)
 
         raise exceptions(status_det)(response, request=response)
 
+    # async def upload_file(self, file, profile_id: str, file_type: str, file_name: str = None, chunk: int = 1048576,
+    #                       callback=None, *args, **kwargs):
+    #     """
+    #     Upload a file to Rubika.
+
+    #     Parameters:
+    #     - file: File path or bytes.
+    #     - mime: MIME type of the file.
+    #     - file_name: Name of the file.
+    #     - chunk: Chunk size for uploading.
+    #     - callback: Progress callback.
+
+    #     Returns:
+    #     Results object.
+    #     """
+    #     if isinstance(file, str):
+    #         if not os.path.exists(file):
+    #             raise ValueError('File not found in the given path')
+
+    #         if file_name is None:
+    #             file_name = os.path.basename(file)
+
+    #         async with aiofiles.open(file, 'rb+') as file:
+    #             file = await file.read()
+
+    #     elif not isinstance(file, bytes):
+    #         raise TypeError('File argument must be a file path or bytes')
+
+    #     if file_name is None:
+    #         raise ValueError('File name is not set')
+
+    #     result = await self.request_upload_file(profile_id, file_name, len(file), file_type)
+
+    #     id = result.file_id
+    #     index = 0
+    #     count_retry = 0
+    #     max_retring = 3
+    #     total = int(len(file) / chunk + 1)
+    #     upload_url = result.server_url
+    #     hash_file_request = result.hash_file_request
+
+    #     while index < total:
+    #         if count_retry == max_retring:
+    #             break
+
+    #         data = file[index * chunk: index * chunk + chunk]
+    #         try:
+    #             response = await self.client.connection.session.post(
+    #                 upload_url,
+    #                 headers={
+    #                     'auth': self.client.auth,
+    #                     'file-id': id,
+    #                     'total-part': str(total),
+    #                     'part-number': str(index + 1),
+    #                     'chunk-size': str(len(data)),
+    #                     'hash-file-request': hash_file_request
+    #                 },
+    #                 data=data,
+    #                 proxy=self.client.proxy,
+    #             )
+    #             response = await response.json()
+
+    #             if response.get('status') != 'OK':
+    #                 result = await self.request_upload_file(profile_id, file_name, len(file), file_type)
+    #                 id = result.file_id
+    #                 index = 0
+    #                 total = int(len(file) / chunk + 1)
+    #                 upload_url = result.server_url
+    #                 hash_file_request = result.hash_file_request
+    #                 count_retry += 1
+
+    #             if callable(callback):
+    #                 try:
+    #                     if inspect.iscoroutinefunction(callback):
+    #                         await callback(len(file), index * chunk)
+
+    #                     else:
+    #                         callback(len(file), index * chunk)
+
+    #                 except exceptions.CancelledError:
+    #                     return None
+
+    #                 except Exception:
+    #                     pass
+
+    #             index += 1
+
+    #         except Exception:
+    #             pass
+
+    #     status = response['status']
+    #     status_det = response['status_det']
+
+    #     if status == 'OK' and status_det == 'OK':
+    #         response.update(result.original_update)
+    #         return Update(response)
+
+    #     raise exceptions(status_det)(response, request=response)
+
     async def add_post(self, profile_id: str, post: str, post_type: str, caption: str = None, file_name: str = None):
         if isinstance(post, str):
             if not os.path.exists(post):
                 raise ValueError('File not found in the given path')
 
             if file_name is None:
                 file_name = os.path.basename(post)
```

### Comparing `rubpy-7.0.4/rubpy/rubino/thumbnail.py` & `rubpy-7.0.5/rubpy/rubino/thumbnail.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tempfile
 import warnings
 import base64
 import typing
+import os
 import io
 from pathlib import Path
 
 DEFAULT_TEMP_PATH = r'./temps'
 path = Path(DEFAULT_TEMP_PATH)
 
 if not path.exists():
@@ -20,14 +21,19 @@
     numpy = None
 
 try:
     import PIL.Image
 except ImportError:
     PIL = None
 
+try:
+    from moviepy.editor import VideoFileClip
+except ImportError:
+    VideoFileClip = None
+
 
 class ResultMedia:
     """
     Represents media data along with its metadata.
 
     Attributes:
     - image (bytes): The raw image data.
@@ -158,52 +164,99 @@
 
         Args:
         - video (bytes): The raw video data.
 
         Returns:
         - ResultMedia: ResultMedia object containing the thumbnail and metadata.
         """
-        # if VideoFileClip is not None:
-        #     try:
-        #         with tempfile.NamedTemporaryFile(mode='wb+', suffix='.mp4', dir=DEFAULT_TEMP_PATH, delete=False) as file:
-        #             file.write(video)
-        #             file_name = file.name
-
-        #         capture = VideoFileClip(file_name)
-        #         width, height = capture.size
-        #         seconds = int(capture.duration)
-        #         # Extract frame from the middle of the video
-        #         frame = capture.get_frame(seconds / 2)
-        #         # Resize the frame to 720x720
-        #         frame = cv2.resize(frame, (720, 720), interpolation=cv2.INTER_CUBIC)
-        #         capture.close()
-        #         os.remove(file_name)
-        #         return ResultMedia(frame, width=720, height=720, seconds=seconds)
-        #     except Exception as e:
-        #         print(f"Error processing video with moviepy: {e}")
-        #         os.remove(file_name)
-        #         return None
-
-        # Continue with the OpenCV approach if moviepy is not available
-        if cv2 is None:
-            warnings.warn('OpenCV not found, video processing disabled')
+        if VideoFileClip is not None:
+            return cls._from_video_moviepy(video)
+        elif cv2 is not None:
+            return cls._from_video_opencv(video)
+        elif PIL is not None:
+            return cls._from_video_moviepy(video)
+        else:
+            warnings.warn('OpenCV and MoviePy not found, video processing disabled')
             return None
 
+    @classmethod
+    def _from_video_opencv(cls, video: bytes) -> typing.Optional[ResultMedia]:
+        """
+        Generate a thumbnail from video data using OpenCV.
+
+        Args:
+        - video (bytes): The raw video data.
+
+        Returns:
+        - ResultMedia: ResultMedia object containing the thumbnail and metadata.
+        """
         with tempfile.NamedTemporaryFile(mode='wb+', suffix='.mp4', dir=DEFAULT_TEMP_PATH) as file:
             file.write(video)
 
             # Read the video using OpenCV
             capture = cv2.VideoCapture(file.name)
-            total_frames = int(capture.get(cv2.CAP_PROP_FRAME_COUNT))
-            middle_frame_index = total_frames // 2
-            capture.set(cv2.CAP_PROP_POS_FRAMES, middle_frame_index)
+            # Check if the video is opened successfully
+            if not capture.isOpened():
+                warnings.warn('Failed to open video file')
+                return None
+
+            # Read the first frame
             status, frame = capture.read()
 
-            # If successful, calculate video duration and create ResultMedia object
-            if status is True:
+            # If successful, create ResultMedia object
+            if status:
+                # Get video properties
+                width = int(capture.get(cv2.CAP_PROP_FRAME_WIDTH))
+                height = int(capture.get(cv2.CAP_PROP_FRAME_HEIGHT))
                 fps = capture.get(cv2.CAP_PROP_FPS)
+                total_frames = int(capture.get(cv2.CAP_PROP_FRAME_COUNT))
                 seconds = int(total_frames / fps)
+
                 # Resize the frame to 720x720
                 frame = cv2.resize(frame, (720, 720), interpolation=cv2.INTER_CUBIC)
+
+                # Release the video capture object
+                capture.release()
+
                 return ResultMedia(frame, width=720, height=720, seconds=seconds)
 
         return None
+
+    @classmethod
+    def _from_video_moviepy(cls, video: bytes) -> typing.Optional[ResultMedia]:
+        """
+        Generate a thumbnail from video data using MoviePy.
+
+        Args:
+        - video (bytes): The raw video data.
+
+        Returns:
+        - ResultMedia: ResultMedia object containing the thumbnail and metadata.
+        """
+        try:
+            # Save the video to a temporary file
+            with tempfile.NamedTemporaryFile(mode='wb+', suffix='.mp4', dir=DEFAULT_TEMP_PATH, delete=False) as file:
+                file.write(video)
+                file_name = file.name
+
+            # Read the video using MoviePy
+            clip = VideoFileClip(file_name)
+
+            # Extract the first frame
+            frame = clip.get_frame(0)
+
+            # Close the clip and remove the temporary file
+            clip.close()
+            os.remove(file_name)
+
+            # Resize the frame to 720x720
+            frame_resized = cv2.resize(frame, (720, 720), interpolation=cv2.INTER_CUBIC)
+
+            # Convert frame to BGR (OpenCV uses BGR by default)
+            frame_bgr = cv2.cvtColor(frame_resized, cv2.COLOR_RGB2BGR)
+
+            return ResultMedia(frame_bgr, width=720, height=720, seconds=int(clip.duration))
+
+        except Exception as e:
+            print(f"Error processing video with MoviePy: {e}")
+            os.remove(file_name)
+            return None
```

### Comparing `rubpy-7.0.4/rubpy/sessions/sqliteSession.py` & `rubpy-7.0.5/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/sessions/stringSession.py` & `rubpy-7.0.5/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/sync.py` & `rubpy-7.0.5/rubpy/sync.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/types/update.py` & `rubpy-7.0.5/rubpy/types/update.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy/utils.py` & `rubpy-7.0.5/rubpy/utils.py`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/rubpy.egg-info/PKG-INFO` & `rubpy-7.0.5/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 7.0.4
+Version: 7.0.5
 Summary: A powerful, fast and optimal library for making robots in Rubika with sync and async support.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 7.0.4 Summary: A powerful, fast and
+Metadata-Version: 2.1 Name: rubpy Version: 7.0.5 Summary: A powerful, fast and
 optimal library for making robots in Rubika with sync and async support. Home-
 page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-
 email: contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-7.0.4/rubpy.egg-info/SOURCES.txt` & `rubpy-7.0.5/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-7.0.4/setup.py` & `rubpy-7.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 
 with open('README.md', encoding='UTF-8') as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '7.0.4',
+    version = '7.0.5',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'A powerful, fast and optimal library for making robots in Rubika with sync and async support.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires='~=3.7',
     long_description_content_type = 'text/markdown',
```

