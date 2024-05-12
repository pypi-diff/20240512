# Comparing `tmp/aiorubika-0.0.2.tar.gz` & `tmp/aiorubika-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorubika-0.0.2.tar", last modified: Tue Apr  9 13:33:35 2024, max compression
+gzip compressed data, was "aiorubika-1.0.0.tar", last modified: Sun May 12 11:48:46 2024, max compression
```

## Comparing `aiorubika-0.0.2.tar` & `aiorubika-1.0.0.tar`

### file list

```diff
@@ -1,286 +1,107 @@
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.421977 aiorubika-0.0.2/
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1678 2024-04-09 13:33:35.421977 aiorubika-0.0.2/PKG-INFO
--rw-r--r--   0 funlife   (1000) funlife   (1000)      445 2024-04-09 13:19:38.000000 aiorubika-0.0.2/README.md
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.300972 aiorubika-0.0.2/aiorubika/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      247 2024-04-09 13:27:31.000000 aiorubika-0.0.2/aiorubika/__init__.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.302972 aiorubika-0.0.2/aiorubika/bots/
--rw-r--r--   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)    11169 2024-04-09 13:31:17.000000 aiorubika-0.0.2/aiorubika/bots/client.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.315973 aiorubika-0.0.2/aiorubika/bots/types/
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1077 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      163 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/aux_data.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      255 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/bot.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      102 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/bot_command.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1093 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      225 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button_calendar.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      286 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button_location.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      191 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button_number_picker.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      377 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button_selection.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      195 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button_selection_item.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      159 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button_string_picker.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      255 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/button_textbox.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      257 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      132 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/contact_message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      111 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/file.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      214 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/forwarded_from.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      340 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/inline_message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      232 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/keypad.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      141 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/keypad_row.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      340 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/live_location.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)       99 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/location.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      107 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/messaage_text_update.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      887 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      149 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/message_keypad_update.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      156 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/payment_status.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      192 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/poll.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      248 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/poll_status.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      148 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/sticker.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      455 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/bots/types/update.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     3343 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/client.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.315973 aiorubika-0.0.2/aiorubika/crypto/
--rw-r--r--   0 funlife   (1000) funlife   (1000)       26 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/crypto/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     5110 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/crypto/crypto.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.318973 aiorubika-0.0.2/aiorubika/enums/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      230 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/enums/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      597 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/enums/chat_access_type.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      257 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/enums/chat_action.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      370 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/enums/chat_type.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      496 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/enums/message_media_type.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      133 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/enums/poll_type.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1767 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/enums/reaction_type.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1942 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/exceptions.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     6008 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/filters.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     2816 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/handlers.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.319973 aiorubika-0.0.2/aiorubika/methods/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      646 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/__init__.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.320973 aiorubika-0.0.2/aiorubika/methods/advanced/
--rw-r--r--   0 funlife   (1000) funlife   (1000)       75 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/advanced/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1655 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/advanced/build.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.322973 aiorubika-0.0.2/aiorubika/methods/auth/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      185 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/auth/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1887 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/auth/register_device.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      685 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/auth/send_code.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      699 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/auth/sign_in.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.339974 aiorubika-0.0.2/aiorubika/methods/channels/
--rw-r--r--   0 funlife   (1000) funlife   (1000)     2570 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      610 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/add_channel.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      585 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/add_channel_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      675 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/ban_channel_member.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      428 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/channel_preview_by_join_link.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      301 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/check_channel_username.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      373 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/create_channel_voice_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      339 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/delete_no_access_group_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      485 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/discard_channel_voice_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1881 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/edit_channel_info.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      426 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_banned_group_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      481 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_channel_admin_access_list.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      451 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_channel_admin_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      669 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_channel_all_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      348 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_channel_info.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      348 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_channel_link.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      332 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_group_default_access.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      440 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_group_mention_list.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      633 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/get_group_voice_chat_updates.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      598 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/join_channel_action.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      329 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/join_channel_by_link.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      343 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/join_group.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      297 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/leave_group.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      430 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/leave_group_voice_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      344 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/remove_channel.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      499 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/seen_channel_messages.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      348 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/set_channel_link.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      617 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/set_channel_voice_chat_setting.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1014 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/set_group_admin.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      558 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/set_group_default_access.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      421 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/channels/update_channel_username.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.346974 aiorubika-0.0.2/aiorubika/methods/chats/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      807 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      398 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/delete_avatar.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      479 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/delete_chat_history.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      448 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/get_abs_objects.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      300 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/get_avatars.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      333 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/get_chats.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      432 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/get_chats_updates.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      312 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/get_link_from_app_url.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      641 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/search_chat_messages.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      292 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/seen_chats.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      598 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/send_chat_activity.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      535 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/set_action_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      849 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/chats/upload_avatar.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.348974 aiorubika-0.0.2/aiorubika/methods/contacts/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      299 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/contacts/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      455 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/contacts/add_address_book.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      253 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/contacts/delete_contact.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      314 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/contacts/get_contacts.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      375 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/contacts/get_contacts_updates.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.351974 aiorubika-0.0.2/aiorubika/methods/decorators/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      415 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/decorators/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      323 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/decorators/on_chat_updates.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      332 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/decorators/on_message_updates.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      347 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/decorators/on_remove_notifications.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      332 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/decorators/on_show_activities.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      341 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/decorators/on_show_notifications.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/decorators/on_start.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.356974 aiorubika-0.0.2/aiorubika/methods/extras/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      559 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      400 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/ban_member.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      650 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/get_info.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      366 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/get_object_by_username.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      250 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/get_profile_link_items.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      286 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/get_related_objects.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      456 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/get_transcription.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      401 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/join.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      351 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/leave_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      328 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/extras/search_global_objects.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.358974 aiorubika-0.0.2/aiorubika/methods/gif/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      235 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/gif/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      351 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/gif/add_to_my_gif_set.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      139 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/gif/get_my_gif_set.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      240 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/gif/remove_from_my_gif_set.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.371975 aiorubika-0.0.2/aiorubika/methods/groups/
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1857 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      512 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/add_group.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      545 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/add_group_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      631 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/ban_group_member.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      329 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/create_group_voice_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      339 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/delete_no_access_group_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1832 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/edit_group_info.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      426 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_banned_group_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      437 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_admin_access_list.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      423 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_admin_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      663 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_all_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      332 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_default_access.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      304 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_info.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      304 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_link.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      440 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_mention_list.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      633 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/get_group_voice_chat_updates.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      422 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/group_preview_by_join_link.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      348 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/join_group.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      218 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/leave_group.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      430 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/leave_group_voice_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      300 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/remove_group.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1014 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/set_group_admin.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      558 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/set_group_default_access.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      304 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/set_group_link.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      573 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/groups/set_group_voice_chat_setting.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.384975 aiorubika-0.0.2/aiorubika/methods/messages/
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1747 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      608 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/action_on_message_reaction.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      323 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/auto_delete_message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1346 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/create_poll.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      758 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/delete_messages.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      660 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/edit_message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      678 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/forward_messages.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      397 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/get_message_share_url.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      548 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/get_messages_by_id.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      491 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/get_messages_interval.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      487 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/get_messages_updates.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      510 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/get_poll_option_voters.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      313 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/get_poll_status.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      396 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/reaction.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      412 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/remove_reaction.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      487 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/request_send_file.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1081 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_document.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1027 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_gif.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     5816 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1045 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_music.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1101 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_photo.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1193 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_video.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1101 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_video_message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1045 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/send_voice.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1257 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/set_pin_message.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      439 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/messages/vote_poll.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.390976 aiorubika-0.0.2/aiorubika/methods/settings/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      878 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      265 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/delete_folder.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      148 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/get_blocked_users.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      345 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/get_folders.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      142 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/get_my_sessions.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      154 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/get_privacy_setting.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      160 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/get_suggested_folders.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      164 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/get_two_passcode_status.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     2419 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/set_setting.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      528 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/setup_two_step_verification.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      279 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/terminate_session.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      908 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/update_profile.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      206 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/settings/update_username.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.394976 aiorubika-0.0.2/aiorubika/methods/stickers/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      578 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      601 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/action_on_sticker_set.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      152 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/get_my_sticker_sets.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      300 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/get_sticker_set_by_id.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      334 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/get_stickers_by_emoji.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      447 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/get_stickers_by_set_ids.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      292 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/get_trend_sticker_sets.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      450 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/stickers/search_stickers.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.397976 aiorubika-0.0.2/aiorubika/methods/users/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      331 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/users/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      202 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/users/check_user_username.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      483 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/users/delete_user_chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)       84 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/users/get_me.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      351 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/users/get_user_info.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      511 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/users/set_block_user.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.402976 aiorubika-0.0.2/aiorubika/methods/utilities/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      613 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)       99 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/add_handler.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      705 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/connect.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      422 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/disconnect.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      664 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/download.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      890 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/download_profile_picture.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      747 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/get_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      137 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/get_updates.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      152 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/remove_handler.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      419 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/run.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     3112 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/start.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     3756 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/thumbnail.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      181 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/methods/utilities/upload.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)    12274 2024-04-09 13:31:17.000000 aiorubika-0.0.2/aiorubika/network.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.403976 aiorubika-0.0.2/aiorubika/parser/
--rw-r--r--   0 funlife   (1000) funlife   (1000)       30 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/parser/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     4713 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/parser/markdown.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/parser/parser.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.404976 aiorubika-0.0.2/aiorubika/rubino/
--rw-r--r--   0 funlife   (1000) funlife   (1000)       26 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/rubino/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)    11814 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/rubino/client.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.405976 aiorubika-0.0.2/aiorubika/sessions/
--rw-r--r--   0 funlife   (1000) funlife   (1000)       82 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/sessions/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     2294 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/sessions/sqliteSession.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1223 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/sessions/stringSession.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     3594 2024-04-09 13:31:17.000000 aiorubika-0.0.2/aiorubika/sync.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.414976 aiorubika-0.0.2/aiorubika/types/
--rw-r--r--   0 funlife   (1000) funlife   (1000)      268 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      418 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/abs_object.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      241 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/avatar_thumbnail.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      802 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/chat.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      141 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/chat_reaction_setting.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      141 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/chat_update.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      302 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/file.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      556 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/file_inline.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      210 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/forwarded_from.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      509 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/group.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      294 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/in_chat_members.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      619 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/member.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      499 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/message.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.419977 aiorubika-0.0.2/aiorubika/types/models/
--rw-r--r--   0 funlife   (1000) funlife   (1000)       72 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/__init__.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     4505 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/chats.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1781 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/contacts.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     8849 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/extras.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     9489 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/groups.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)    30534 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/messages.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1670 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/stickers.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     3507 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/models/users.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      163 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/online_time.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     2275 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/results.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)    20643 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/socket_results.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      307 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/sticker.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)      500 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/types/user.py
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1345 2024-04-09 13:13:13.000000 aiorubika-0.0.2/aiorubika/utils.py
-drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:33:35.419977 aiorubika-0.0.2/aiorubika.egg-info/
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1678 2024-04-09 13:33:35.000000 aiorubika-0.0.2/aiorubika.egg-info/PKG-INFO
--rw-r--r--   0 funlife   (1000) funlife   (1000)    10545 2024-04-09 13:33:35.000000 aiorubika-0.0.2/aiorubika.egg-info/SOURCES.txt
--rw-r--r--   0 funlife   (1000) funlife   (1000)        1 2024-04-09 13:33:35.000000 aiorubika-0.0.2/aiorubika.egg-info/dependency_links.txt
--rw-r--r--   0 funlife   (1000) funlife   (1000)       82 2024-04-09 13:33:35.000000 aiorubika-0.0.2/aiorubika.egg-info/requires.txt
--rw-r--r--   0 funlife   (1000) funlife   (1000)       10 2024-04-09 13:33:35.000000 aiorubika-0.0.2/aiorubika.egg-info/top_level.txt
--rw-r--r--   0 funlife   (1000) funlife   (1000)       38 2024-04-09 13:33:35.422977 aiorubika-0.0.2/setup.cfg
--rw-r--r--   0 funlife   (1000) funlife   (1000)     1594 2024-04-09 13:33:04.000000 aiorubika-0.0.2/setup.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.855692 aiorubika-1.0.0/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1071 2024-05-12 09:58:53.000000 aiorubika-1.0.0/LICENSE
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1767 2024-05-12 11:48:46.854692 aiorubika-1.0.0/PKG-INFO
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      418 2024-05-12 11:32:48.000000 aiorubika-1.0.0/README.md
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.835691 aiorubika-1.0.0/aiorubika/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      140 2024-05-12 10:06:49.000000 aiorubika-1.0.0/aiorubika/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     3318 2024-05-12 11:42:11.000000 aiorubika-1.0.0/aiorubika/client.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.837691 aiorubika-1.0.0/aiorubika/crypto/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       27 2024-05-12 11:19:47.000000 aiorubika-1.0.0/aiorubika/crypto/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     5116 2024-05-12 11:20:50.000000 aiorubika-1.0.0/aiorubika/crypto/crypto.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.839691 aiorubika-1.0.0/aiorubika/enums/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      232 2024-05-12 11:17:10.000000 aiorubika-1.0.0/aiorubika/enums/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      601 2024-05-12 11:17:32.000000 aiorubika-1.0.0/aiorubika/enums/chat_access_type.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      261 2024-05-12 11:17:53.000000 aiorubika-1.0.0/aiorubika/enums/chat_action.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      372 2024-05-12 11:18:11.000000 aiorubika-1.0.0/aiorubika/enums/chat_type.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      500 2024-05-12 11:18:39.000000 aiorubika-1.0.0/aiorubika/enums/message_media_type.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      137 2024-05-12 11:18:58.000000 aiorubika-1.0.0/aiorubika/enums/poll_type.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1771 2024-05-12 11:19:22.000000 aiorubika-1.0.0/aiorubika/enums/reaction_type.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1956 2024-05-12 10:14:27.000000 aiorubika-1.0.0/aiorubika/exceptions.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     5773 2024-05-12 10:16:58.000000 aiorubika-1.0.0/aiorubika/filters.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     2840 2024-05-12 10:18:24.000000 aiorubika-1.0.0/aiorubika/handlers.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.839691 aiorubika-1.0.0/aiorubika/methods/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      351 2024-05-12 11:38:40.000000 aiorubika-1.0.0/aiorubika/methods/__init__.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.839691 aiorubika-1.0.0/aiorubika/methods/advanced/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       77 2024-05-12 11:15:58.000000 aiorubika-1.0.0/aiorubika/methods/advanced/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1326 2024-05-12 11:16:51.000000 aiorubika-1.0.0/aiorubika/methods/advanced/build.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.840691 aiorubika-1.0.0/aiorubika/methods/auth/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      187 2024-05-12 11:15:36.000000 aiorubika-1.0.0/aiorubika/methods/auth/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1694 2024-05-12 11:11:28.000000 aiorubika-1.0.0/aiorubika/methods/auth/register_device.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      672 2024-05-12 11:13:33.000000 aiorubika-1.0.0/aiorubika/methods/auth/send_code.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      567 2024-05-12 11:15:12.000000 aiorubika-1.0.0/aiorubika/methods/auth/sign_in.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.841692 aiorubika-1.0.0/aiorubika/methods/decorators/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       79 2024-05-12 11:36:41.000000 aiorubika-1.0.0/aiorubika/methods/decorators/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      342 2024-05-12 11:32:48.000000 aiorubika-1.0.0/aiorubika/methods/decorators/on_message.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.841692 aiorubika-1.0.0/aiorubika/methods/messages/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       77 2024-05-12 11:06:26.000000 aiorubika-1.0.0/aiorubika/methods/messages/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     5616 2024-05-12 11:03:55.000000 aiorubika-1.0.0/aiorubika/methods/messages/send_message.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.843692 aiorubika-1.0.0/aiorubika/methods/settings/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      355 2024-05-12 10:54:58.000000 aiorubika-1.0.0/aiorubika/methods/settings/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      154 2024-05-12 10:55:23.000000 aiorubika-1.0.0/aiorubika/methods/settings/get_my_sessions.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      174 2024-05-12 10:56:02.000000 aiorubika-1.0.0/aiorubika/methods/settings/get_two_passcode_status.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      528 2024-05-12 10:56:54.000000 aiorubika-1.0.0/aiorubika/methods/settings/setup_two_step_verification.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      321 2024-05-12 10:58:17.000000 aiorubika-1.0.0/aiorubika/methods/settings/terminate_session.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.843692 aiorubika-1.0.0/aiorubika/methods/users/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      115 2024-05-12 11:48:12.000000 aiorubika-1.0.0/aiorubika/methods/users/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       88 2024-05-12 10:53:34.000000 aiorubika-1.0.0/aiorubika/methods/users/get_me.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      389 2024-05-12 11:47:12.000000 aiorubika-1.0.0/aiorubika/methods/users/get_user_info.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.847692 aiorubika-1.0.0/aiorubika/methods/utilities/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      615 2024-05-12 10:35:41.000000 aiorubika-1.0.0/aiorubika/methods/utilities/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      103 2024-05-12 10:36:01.000000 aiorubika-1.0.0/aiorubika/methods/utilities/add_handler.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      599 2024-05-12 10:37:09.000000 aiorubika-1.0.0/aiorubika/methods/utilities/connect.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      364 2024-05-12 10:37:55.000000 aiorubika-1.0.0/aiorubika/methods/utilities/disconnect.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      792 2024-05-12 10:39:36.000000 aiorubika-1.0.0/aiorubika/methods/utilities/download.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      904 2024-05-12 10:40:24.000000 aiorubika-1.0.0/aiorubika/methods/utilities/download_profile_picture.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      759 2024-05-12 10:41:48.000000 aiorubika-1.0.0/aiorubika/methods/utilities/get_members.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      147 2024-05-12 10:42:24.000000 aiorubika-1.0.0/aiorubika/methods/utilities/get_updates.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      156 2024-05-12 10:42:52.000000 aiorubika-1.0.0/aiorubika/methods/utilities/remove_handler.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      429 2024-05-12 10:43:33.000000 aiorubika-1.0.0/aiorubika/methods/utilities/run.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     3015 2024-05-12 10:44:52.000000 aiorubika-1.0.0/aiorubika/methods/utilities/start.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     3330 2024-05-12 10:47:59.000000 aiorubika-1.0.0/aiorubika/methods/utilities/thumbnail.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      191 2024-05-12 10:48:44.000000 aiorubika-1.0.0/aiorubika/methods/utilities/upload.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)    12025 2024-05-12 10:24:14.000000 aiorubika-1.0.0/aiorubika/network.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.847692 aiorubika-1.0.0/aiorubika/parser/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       31 2024-05-12 10:34:09.000000 aiorubika-1.0.0/aiorubika/parser/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     5179 2024-05-12 10:33:56.000000 aiorubika-1.0.0/aiorubika/parser/markdown.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 10:03:43.000000 aiorubika-1.0.0/aiorubika/parser/parser.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.848692 aiorubika-1.0.0/aiorubika/sessions/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       86 2024-05-12 10:07:45.000000 aiorubika-1.0.0/aiorubika/sessions/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     2222 2024-05-12 10:32:35.000000 aiorubika-1.0.0/aiorubika/sessions/sqlite_session.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1184 2024-05-12 10:32:27.000000 aiorubika-1.0.0/aiorubika/sessions/string_session.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.852692 aiorubika-1.0.0/aiorubika/types/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      129 2024-05-12 10:05:17.000000 aiorubika-1.0.0/aiorubika/types/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      410 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/abs_object.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      234 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/avatar_thumbnail.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      782 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/chat.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      138 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/chat_reaction_setting.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      138 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/chat_update.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      293 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/file.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      540 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/file_inline.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      204 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/forwarded_from.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      495 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/group.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      287 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/in_chat_members.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      604 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/member.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      486 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/message.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.853692 aiorubika-1.0.0/aiorubika/types/models/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       73 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/__init__.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     4388 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/chats.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1735 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/contacts.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     8641 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/extras.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     9255 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/groups.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)    29434 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/messages.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1629 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/stickers.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     3416 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/models/users.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      158 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/online_time.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     2198 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/results.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)    19878 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/socket_results.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      299 2024-05-12 10:31:58.000000 aiorubika-1.0.0/aiorubika/types/sticker.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)      504 2024-05-12 10:28:34.000000 aiorubika-1.0.0/aiorubika/types/user.py
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1375 2024-05-12 10:25:00.000000 aiorubika-1.0.0/aiorubika/utils.py
+drwxr-xr-x   0 Dev.amirali  (1000) Dev.amirali  (1000)        0 2024-05-12 11:48:46.853692 aiorubika-1.0.0/aiorubika.egg-info/
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1767 2024-05-12 11:48:46.000000 aiorubika-1.0.0/aiorubika.egg-info/PKG-INFO
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     2931 2024-05-12 11:48:46.000000 aiorubika-1.0.0/aiorubika.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)        1 2024-05-12 11:48:46.000000 aiorubika-1.0.0/aiorubika.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       82 2024-05-12 11:48:46.000000 aiorubika-1.0.0/aiorubika.egg-info/requires.txt
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       10 2024-05-12 11:48:46.000000 aiorubika-1.0.0/aiorubika.egg-info/top_level.txt
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)       38 2024-05-12 11:48:46.855692 aiorubika-1.0.0/setup.cfg
+-rw-r--r--   0 Dev.amirali  (1000) Dev.amirali  (1000)     1621 2024-05-12 11:25:11.000000 aiorubika-1.0.0/setup.py
```

### Comparing `aiorubika-0.0.2/PKG-INFO` & `aiorubika-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aiorubika
-Version: 0.0.2
-Summary:  Rubika API Framework for Python
-Home-page: https://github.com/metect/rubika
+Version: 1.0.0
+Summary: aiorubika is a modern and fully asynchronous framework for Rubika Self API written in Python 
+Home-page: https://github.com/irvanyamirali/aiorubika
 Author: amirali irvany
-Author-email: dev.amirali.irvany@gmail.com
-Keywords: rubika,aiorubika,chat,bot,robot,asyncio
+Author-email: irvanyamirali@gmail.com
+Keywords: rubika,aiorubika,bot,asyncio,aiohttp,pydantic
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -17,38 +17,40 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: pycryptodome
 Requires-Dist: pydantic==1.10.12
 Requires-Dist: aiofiles
 Provides-Extra: cv
 Requires-Dist: opencv-python; extra == "cv"
 Provides-Extra: pil
 Requires-Dist: pillow; extra == "pil"
 
-# AIORubika
-Rubika API Framework for Python
+# aiorubika
 
-### Examples
+Python-based asynchronous framework for Rubika messenger API
+
+## Install
+```bash
+pip install aiorubika
+```
+
+
+## Quik Start
 ```python
 from aiorubika import Client, filters, utils
-from aiorubika.types import Updates
-
-bot = Client(name='rubpy')
 
-@bot.on_message_updates(filters.text)
-async def updates(update: Updates):
+bot = Client(name='bot')
+@bot.on_message_updates(filters.is_private)
+async def updates(update):
     print(update)
-    await update.reply(utils.Code('hello') + utils.Underline('from') + utils.Bold('rubpy'))
+    await update.reply(utils.Code('hello') + utils.Underline('from') + utils.Bold('aiorubika'))
 
 bot.run()
 ```
 
-## Install
-```bash
-pip install aiorubika
-```
```

### Comparing `aiorubika-0.0.2/aiorubika/client.py` & `aiorubika-1.0.0/aiorubika/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from .sessions import SQLiteSession, StringSession
-from .parser import Markdown
 from .methods import Methods
-from typing import Optional, Union
+from .parser import Markdown
+
+from typing import Optional
 
 
 class Client(Methods):
+
     DEFAULT_PLATFORM = {
         'app_name': 'Main',
         'app_version': '4.4.6',
         'platform': 'Web',
         'package': 'web.rubika.ir',
-        }
+    }
 
-    USER_AGENT = ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
-                  'AppleWebKit/537.36 (KHTML, like Gecko)'
-                  'Chrome/102.0.0.0 Safari/537.36')
+    USER_AGENT: str = (
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
+        'AppleWebKit/537.36 (KHTML, like Gecko)'
+        'Chrome/102.0.0.0 Safari/537.36'
+    )
 
     API_VERSION = '6'
 
-    def __init__(self,
-                 name: str,
-                 auth: Optional[str] = None,
-                 private_key: Optional[Union[str, bytes]] = None,
-                 bot_token: Optional[str] = None,
-                 phone_number: Optional[str] = None,
-                 user_agent: Optional[str] = None or USER_AGENT,
-                 timeout: Optional[Union[str, int]] = 20,
-                 lang_code: Optional[str] = 'fa',
-                 parse_mode: Optional[str] = 'All',
+    def __init__(
+            self,
+            name: str,
+            auth: Optional[str] = None,
+            private_key: Optional[str] = None,
+            bot_token: Optional[str] = None,
+            phone_number: Optional[str] = None,
+            user_agent: Optional[str] = None or USER_AGENT,
+            timeout: Optional[int] = 20,
+            lang_code: Optional[str] = 'fa',
+            parse_mode: Optional[str] = 'All',
     ) -> None:
         super().__init__()
         if auth and not isinstance(auth, str):
             raise ValueError('`auth` is `string` arg.')
 
         if private_key:
             if not type(private_key) in (str, bytes):
@@ -49,38 +54,41 @@
         if not isinstance(timeout, int):
             timeout = int(timeout)
 
         if isinstance(name, str):
             session = SQLiteSession(name)
 
         elif not isinstance(name, StringSession):
-            raise TypeError('The given session must be a '
-                            'str or [rubpy.sessions.StringSession]')
+            raise TypeError(
+                'The given session must be a str or [rubpy.sessions.StringSession]'
+            )
 
         if parse_mode not in ('All', 'html', 'markdown', 'mk'):
-            raise ValueError('The `parse_mode` argument can only be in `("All", "html", "markdown", "mk")`.')
+            raise ValueError(
+                'The `parse_mode` argument can only be in `("All", "html", "markdown", "mk")`.'
+            )
 
-        self.DEFAULT_PLATFORM['lang_code'] = lang_code
         self.name = name
         self.auth = auth
+        self.session = session
+        self.timeout = timeout
         self.private_key = private_key
-        self.bot_token = bot_token
         self.phone_number = phone_number
+        self.bot_token = bot_token
         self.user_agent = user_agent
         self.lang_code = lang_code
-        self.timeout = timeout
-        self.session = session
         self.parse_mode = parse_mode
+        self.handlers = dict()
         self.markdown = Markdown()
+        self.guid = None
+        self.key = None
         self.database = None
         self.decode_auth = None
         self.import_key = None
-        self.guid = None
-        self.key = None
-        self.handlers = {}
+        self.DEFAULT_PLATFORM['lang_code'] = lang_code
 
     def __enter__(self):
         return self.start()
 
     def __exit__(self, *args, **kwargs):
         try:
             return self.disconnect()
@@ -90,8 +98,8 @@
     async def __aenter__(self):
         return await self.start()
 
     async def __aexit__(self, *args, **kwargs):
         try:
             return await self.disconnect()
         except Exception as exc:
-            print(exc.__name__, exc)
+            print(exc.__name__, exc)
```

### Comparing `aiorubika-0.0.2/aiorubika/crypto/crypto.py` & `aiorubika-1.0.0/aiorubika/crypto/crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import re
-import json
-import base64
-import string
-import secrets
 from Crypto.Cipher import AES
 from Crypto.Hash import SHA256
+from Crypto.PublicKey import RSA
 from Crypto.Signature import pkcs1_15
 from Crypto.Util.Padding import pad, unpad
-from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_OAEP
+
 from string import ascii_lowercase, ascii_uppercase
+import secrets
+import base64
+import string
+import json
+import re
+
 
 class Crypto:
     AES_IV = b'\x00' * 16
 
     @staticmethod
     def decode_auth(auth: str) -> str:
         """
@@ -153,8 +155,8 @@
             private_key (str): The RSA private key.
             data (str): The encrypted data.
 
         Returns:
             str: The decrypted data as a string.
         """
         key = RSA.import_key(private_key.encode('utf-8'))
-        return PKCS1_OAEP.new(key).decrypt(base64.b64decode(data)).decode('utf-8')
+        return PKCS1_OAEP.new(key).decrypt(base64.b64decode(data)).decode('utf-8')
```

### Comparing `aiorubika-0.0.2/aiorubika/enums/chat_access_type.py` & `aiorubika-1.0.0/aiorubika/enums/chat_access_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 class Access:
     ChangeInfo = "ChangeInfo"
     PinMessages = "PinMessages"
     DeleteGlobalAllMessages = "DeleteGlobalAllMessages"
     BanMember = "BanMember"
     SetAdmin = "SetAdmin"
     SetJoinLink = "SetJoinLink"
@@ -10,8 +11,8 @@
     ViewAdmins = "ViewAdmins"
     SendMessages = "SendMessages"
     AddMember = "AddMember"
     ViewInfo = "ViewInfo"
     ViewMessages = "ViewMessages"
     DeleteLocalMessages = "DeleteLocalMessages"
     EditMyMessages = "EditMyMessages"
-    DeleteGlobalMyMessages = "DeleteGlobalMyMessages"
+    DeleteGlobalMyMessages = "DeleteGlobalMyMessages"
```

### Comparing `aiorubika-0.0.2/aiorubika/enums/reaction_type.py` & `aiorubika-1.0.0/aiorubika/enums/reaction_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 
+
 class ReactionType(int, Enum):
     RED_HEART = 1
     THUMBS_UP, LIKE = 2, 2
     THUMBS_DOWN, UN_LIKE = 3, 3
     FIRE = 4
     SMILING_FACE_WITH_HEARTS = 5
     CLAPPING_HANDS = 6
@@ -68,8 +69,8 @@
     PILL = 65
     SPEAK_NO_EVIL_MONKEY = 66
     SMILING_FACE_WITH_SUNGLASSES = 67
     ALIEN_MONSTER = 68
     SHRUGGING_MAN = 69
     SHRUGGING_PERSON = 70
     SHRUGGING_WOMAN = 71
-    RAGE = 72
+    RAGE = 72
```

### Comparing `aiorubika-0.0.2/aiorubika/exceptions.py` & `aiorubika-1.0.0/aiorubika/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import sys
 
 
 class ClientError(Exception):
     pass
 
+
 class StopHandler(ClientError):
     pass
 
+
 class APIException(Exception):
     pass
 
+
 class CancelledError(ClientError):
     pass
 
 
 class RequestError(ClientError):
     def __init__(self, message, request=None):
         self.message = str(message)
         self.request = request
 
 
 class UploadError(Exception):
-    def __init__(self, status, status_det, dev_message: str=None):
+    def __init__(self, status, status_det, dev_message: str = None):
         self.status = status
         self.status_det = status_det
         self.dev_message = dev_message
 
+
 class CodeIsUsed(RequestError):
     pass
 
 
 class TooRequests(RequestError):
     pass
 
@@ -103,18 +107,20 @@
 
 
 class NotSupportedApiVersion(RequestError):
     pass
 
 
 class ExcetionsHandler:
+
     def __init__(self, name) -> None:
         self.name = name
 
     def __getattr__(self, name):
         name = ''.join([chunk.title() for chunk in name.split('_')])
         return globals().get(name, ClientError)
 
     def __call__(self, name, *args, **kwargs):
         return getattr(self, name)
 
+
 sys.modules[__name__] = ExcetionsHandler(__name__)
```

### Comparing `aiorubika-0.0.2/aiorubika/filters.py` & `aiorubika-1.0.0/aiorubika/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from typing import Type
+import warnings
 import difflib
 import inspect
-import warnings
 import sys
 import re
 
-__all__ = ['Operator', 'BaseModel', 'RegexModel']
-__models__ = [
+__all__: list = ['Operator', 'BaseModel', 'RegexModel']
+
+__models__: list = [
     'is_pinned', 'is_mute', 'count_unseen', 'message_id',
     'is_group', 'is_private', 'is_channel', 'is_in_contact',
-    'raw_text', 'original_update', 'object_guid', 'author_guid', 'time', 'reply_message_id']
+    'raw_text', 'original_update', 'object_guid', 'author_guid', 'time', 'reply_message_id'
+]
+
 
 def create(name, __base, authorise: list = [], exception: bool = True, *args, **kwargs):
         result = None
         if name in authorise:
             result = name
 
         else:
             proposal = difflib.get_close_matches(name, authorise, n=1)
             if proposal:
                 result = proposal[0]
                 caller = inspect.getframeinfo(inspect.stack()[2][0])
                 warnings.warn(
-                    f'{caller.filename}:{caller.lineno}: do you mean'
-                    f' "{name}", "{result}"? correct it')
+                    f'{caller.filename}:{caller.lineno}: do you mean "{name}", "{result}"? correct it'
+                )
 
         if result is not None or not exception:
             if result is None:
                 result = name
-            return type(result, __base, {'__name__': result, **kwargs})
+            return type(
+                result, __base, {
+                    '__name__': result, **kwargs
+                }
+            )
 
         raise AttributeError(f'module has no attribute ({name})')
 
 
 class Operator:
     Or = 'OR'
     And = 'AND'
@@ -48,14 +55,15 @@
         self.operator = operator
 
     def __eq__(self, value) -> bool:
         return self.operator == value
 
 
 class BaseModel:
+
     def __init__(self, func=None, filters=[], *args, **kwargs) -> None:
         self.func = func
         if not isinstance(filters, list):
             filters = [filters]
         self.filters = filters
 
     def insert(self, filter):
@@ -83,26 +91,24 @@
     def __gt__(self, value):
         return self.insert(Operator(value, Operator.Greater))
 
     def __ge__(self, value):
         return self.insert(Operator(value, Operator.Greatere))
 
     async def build(self, update):
-        # get key
         result = getattr(update, self.__class__.__name__, None)
         if callable(self.func):
             if update.is_async(self.func):
                 result = await self.func(result)
             else:
                 result = self.func(result)
 
         for filter in self.filters:
             value = filter.value
 
-            # if the comparison was with a function
             if callable(value):
                 if update.is_async(value):
                     value = await value(update, result)
                 else:
                     value = value(update, result)
 
             if self.func:
@@ -168,21 +174,14 @@
         return self.__getattr__(name)
 
     def __getattr__(self, name):
         if name in __all__:
             return globals()[name]
         return create(name, (BaseModel,), authorize=__models__, exception=False)
 
-    # async def text(self):
-    #     print('call text')
-    #     return create('text', (BaseModel,), exception=False)
-
-    # async def text(self, *args, **kwargs):
-    #     print('called.')
-    #     return Operator('text', Operator.Equal)
 
 sys.modules[__name__] = Models(__name__)
 
 is_pinned: Type[BaseModel]
 is_mute: Type[BaseModel]
 count_unseen: Type[BaseModel]
 message_id: Type[BaseModel]
@@ -191,8 +190,8 @@
 is_channel: Type[BaseModel]
 is_in_contact: Type[BaseModel]
 raw_text: Type[BaseModel]
 original_update: Type[BaseModel]
 object_guid: Type[BaseModel]
 author_guid: Type[BaseModel]
 time: Type[BaseModel]
-reply_message_id: Type[BaseModel]
+reply_message_id: Type[BaseModel]
```

### Comparing `aiorubika-0.0.2/aiorubika/handlers.py` & `aiorubika-1.0.0/aiorubika/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,53 @@
-import sys
+from .types import SocketResults
+
 import difflib
 import inspect
 import warnings
 import asyncio
-from .types import SocketResults
+import sys
 
 
 __handlers__ = [
     'ChatUpdates',
     'MessageUpdates',
     'ShowActivities',
     'ShowNotifications',
     'RemoveNotifications'
 ]
 
+
 def create(name, __base, authorise: list = [], exception: bool = True, *args, **kwargs):
         result = None
         if name in authorise:
             result = name
 
         else:
             proposal = difflib.get_close_matches(name, authorise, n=1)
             if proposal:
                 result = proposal[0]
                 caller = inspect.getframeinfo(inspect.stack()[2][0])
                 warnings.warn(
-                    f'{caller.filename}:{caller.lineno}: do you mean'
-                    f' "{name}", "{result}"? correct it')
+                    f'{caller.filename}:{caller.lineno}: do you mean "{name}", "{result}"? correct it'
+                )
 
         if result is not None or not exception:
             if result is None:
                 result = name
-            return type(result, __base, {'__name__': result, **kwargs})
+            return type(
+                result, __base, {
+                    '__name__': result, **kwargs
+                }
+            )
 
         raise AttributeError(f'module has no attribute ({name})')
 
 
 class BaseHandlers(SocketResults):
+
     __name__ = 'CustomHandlers'
 
     def __init__(self, *models, __any: bool = False, **kwargs) -> None:
         self.__models = models
         self.__any = __any
 
     def is_async(self, value, *args, **kwargs):
@@ -54,15 +61,14 @@
         return result
 
     async def __call__(self, update: dict, *args, **kwargs) -> bool:
         self.original_update = update
         if self.__models:
             for filter in self.__models:
                 if callable(filter):
-                    # if BaseModels is not called
                     if isinstance(filter, type):
                         filter = filter(func=None)
 
                     if self.is_async(filter):
                         status = await filter(self, result=None)
 
                     else:
@@ -74,14 +80,15 @@
                     elif not status:
                         return False
 
         return True
 
 
 class Handlers:
+
     def __init__(self, name, *args, **kwargs) -> None:
         self.__name__ = name
 
     def __eq__(self, value: object) -> bool:
         return BaseHandlers in value.__bases__
 
     def __dir__(self):
@@ -89,8 +96,9 @@
 
     def __call__(self, name, *args, **kwargs):
         return self.__getattr__(name)(*args, **kwargs)
 
     def __getattr__(self, name):
         return create(name, (BaseHandlers,), __handlers__)
 
+
 sys.modules[__name__] = Handlers(__name__)
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/advanced/build.py` & `aiorubika-1.0.0/aiorubika/methods/advanced/build.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from ...crypto import Crypto
 from ... import exceptions
 from ...types import Results
+
 from typing import Union
-import rubpy
+
+import aiorubika
+
 
 class Builder:
     async def builder(
-            self: "rubpy.Client",
+            self: "aiorubika.Client",
             name: str,
             tmp_session: bool = False,
             encrypt: bool = True,
             dict: bool = False,
             input: dict = None,
     ) -> Union[Results, dict]:
         if not self.connection.api_url:
             await self.connection.get_dcs()
 
         if self.auth is None:
             self.auth = Crypto.secret(length=32)
-            # self._client._logger.info(
-            #     'create auth secret', extra={'data': self._client._auth})
 
         if self.key is None:
             self.key = Crypto.passphrase(self.auth)
-            # self._client._logger.info(
-            #     'create key passphrase', extra={'data': self._client._key})
 
-        result = await self.connection.send(method=name,
-                                            tmp_session=tmp_session,
-                                            encrypt=encrypt,
-                                            input=input)
+        result = await self.connection.send(
+            method=name,
+            tmp_session=tmp_session,
+            encrypt=encrypt,
+            input=input
+        )
         data_enc = result.get('data_enc')
         if data_enc:
-            result = Crypto.decrypt(data_enc,
-                                key=self.key)
+            result = Crypto.decrypt(data_enc, key=self.key)
 
         status = result['status']
         status_det = result['status_det']
 
         if status == 'OK' and status_det == 'OK':
             if dict:
                 return result.get('data')
 
             result['data']['_client'] = self
             return Results(result['data'])
 
-        raise exceptions(status_det)(result, request=None)
+        raise exceptions(status_det)(result, request=None)
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/auth/register_device.py` & `aiorubika-1.0.0/aiorubika/methods/auth/register_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-import rubpy
 import warnings
 import re
 
+import aiorubika
+
 
 system_versions = {
-        'Windows NT 10.0': 'Windows 10',
-        'Windows NT 6.2': 'Windows 8',
-        'Windows NT 6.1': 'Windows 7',
-        'Windows NT 6.0': 'Windows Vista',
-        'Windows NT 5.1': 'windows XP',
-        'Windows NT 5.0': 'Windows 2000',
-        'Mac': 'Mac/iOS',
-        'X11': 'UNIX',
-        'Linux': 'Linux'
-    }
+    'Windows NT 10.0': 'Windows 10',
+    'Windows NT 6.2': 'Windows 8',
+    'Windows NT 6.1': 'Windows 7',
+    'Windows NT 6.0': 'Windows Vista',
+    'Windows NT 5.1': 'windows XP',
+    'Windows NT 5.0': 'Windows 2000',
+    'Mac': 'Mac/iOS',
+    'X11': 'UNIX',
+    'Linux': 'Linux'
+}
 
 
 async def get_browser(user_agent, lang_code, app_version, *args, **kwargs):
-        device_model = re.search(r'(opera|chrome|safari|firefox|msie'
-                                 r'|trident)\/(\d+)', user_agent.lower())
+        device_model = re.search(
+            r'(opera|chrome|safari|firefox|msie|trident)\/(\d+)', user_agent.lower()
+        )
         if not device_model:
             device_model = 'Unknown'
             warnings.warn(f'can not parse user-agent ({user_agent})')
 
         else:
             device_model = device_model.group(1) + ' ' + device_model.group(2)
 
         system_version = 'Unknown'
         for key, value in system_versions.items():
             if key in user_agent:
                 system_version = value
                 break
 
-        # window.navigator.mimeTypes.length (outdated . Defaults to '2')
         device_hash = '2'
         return {
             'token': '',
             'lang_code': lang_code,
             'token_type': 'Web',
             'app_version': f'WB_{app_version}',
             'system_version': system_version,
             'device_model': device_model.title(),
-            'device_hash': device_hash + ''.join(re.findall(r'\d+', user_agent))}
+            'device_hash': device_hash + ''.join(re.findall(r'\d+', user_agent))
+        }
 
 
 class RegisterDevice:
-    async def register_device(self: "rubpy.Client"):
-        return await self.builder(name='registerDevice',
-                                 input=await get_browser(self.user_agent,
-                                                         self.lang_code,
-                                                         self.DEFAULT_PLATFORM.get('app_version')))
+    async def register_device(self: "aiorubika.Client"):
+        return await self.builder(
+            name='registerDevice',
+            input=await get_browser(self.user_agent,
+            self.lang_code,
+            self.DEFAULT_PLATFORM.get('app_version'))
+        )
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/auth/send_code.py` & `aiorubika-1.0.0/aiorubika/methods/auth/send_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from typing import Optional
-import rubpy
+
+import aiorubika
 
 
 class SendCode:
-    async def send_code(self: "rubpy.Client",
-                        phone_number: str,
-                        pass_key: Optional[str] = None,
-                        send_type: Optional[str] = 'SMS',
+    async def send_code(
+            self: "aiorubika.Client",
+            phone_number: str,
+            pass_key: Optional[str] = None,
+            send_type: Optional[str] = 'SMS',
     ):
         if send_type not in ('SMS', 'Internal'):
             raise ValueError('send_type can only be `SMS` or `Internal`.')
 
-        data = {'phone_number': phone_number,
-                'pass_key': pass_key,
-                'send_type': send_type}
+        data = {
+            'phone_number': phone_number,
+            'pass_key': pass_key,
+            'send_type': send_type
+        }
 
-        return await self.builder(name='sendCode',
-                                 input=data,
-                                 tmp_session=True,)
+        return await self.builder(
+            name='sendCode',
+            input=data,
+            tmp_session=True
+        )
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/auth/sign_in.py` & `aiorubika-1.0.0/aiorubika/methods/auth/sign_in.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import rubpy
+import aiorubika
 
 
 class SignIn:
-    async def sign_in(self: "rubpy.Client",
-                     phone_code: str,
-                     phone_number: str,
-                     phone_code_hash: str,
-                     public_key: str,
+    async def sign_in(
+            self: "aiorubika.Client",
+            phone_code: str,
+            phone_number: str,
+            phone_code_hash: str,
+            public_key: str,
     ):
-        return await self.builder(name='signIn',
-                                 input={
-                                     'phone_code': phone_code,
-                                     'phone_number': phone_number,
-                                     'phone_code_hash': phone_code_hash,
-                                     'public_key': public_key,
-                                 },
-                                 tmp_session=True,)
+        return await self.builder(
+            name='signIn',
+            input={
+                 'phone_code': phone_code,
+                 'phone_number': phone_number,
+                 'phone_code_hash': phone_code_hash,
+                 'public_key': public_key,
+            },
+            tmp_session=True
+        )
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/channels/get_channel_all_members.py` & `aiorubika-1.0.0/aiorubika/methods/utilities/get_members.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-import rubpy
 from ...types.in_chat_members import InChatMembers
 
+import aiorubika
 
-class GetChannelAllMembers:
-    async def get_channel_all_members(
-            self: "rubpy.Client",
-            channel_guid: str,
-            search_text: str='',
-            start_id: str=None,
-    ):
-        result = await self.builder('getChannelAllMembers',
-                                  input={
-                                      'channel_guid': channel_guid,
-                                      'search_text': search_text,
-                                      'start_id': start_id,
-                                  }, dict=True)
-        return InChatMembers(**result)
+
+class GetMembers:
+    async def get_members(
+            self: "aiorubika.Client",
+            object_guid: str,
+            start_id: int = None,
+            search_text: str = '',
+    ) -> InChatMembers:
+        if object_guid.startswith('c0'):
+            return await self.get_channel_all_members(
+                channel_guid=object_guid,
+                search_text=search_text,
+                start_id=start_id,
+            )
+
+        else:
+            return await self.get_group_all_members(
+                group_guid=object_guid,
+                search_text=None if search_text == '' else search_text,
+                start_id=start_id,
+            )
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/messages/send_message.py` & `aiorubika-1.0.0/aiorubika/methods/messages/send_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from ...types import Results
 from ..utilities import thumbnail
+
 from typing import Optional, Union
 from aiofiles import open as aiopen
 from asyncio import create_task
+from random import random
 from pathlib import Path
 from os import path
-from random import random
-import rubpy
 import aiohttp
 
+import aiorubika
+
 
 class SendMessage:
-    async def send_message(self: "rubpy.Client",
-                           object_guid: str,
-                           text: Optional[str] = None,
-                           reply_to_message_id: Optional[str] = None,
-                           file_inline: Optional[Union[Path, bytes]] = None,
-                           type: str = 'File',
-                           is_spoil: bool = False,
-                           thumb: bool = True,
-                           auto_delete: Optional[int] = None,
-                           parse_mode: Optional[str] = None, *args, **kwargs):
+    async def send_message(
+            self: "aiorubika.Client",
+            object_guid: str,
+            text: Optional[str] = None,
+            reply_to_message_id: Optional[str] = None,
+            file_inline: Optional[Union[Path, bytes]] = None,
+            type: str = 'File',
+            is_spoil: bool = False,
+            thumb: bool = True,
+            auto_delete: Optional[int] = None,
+            parse_mode: Optional[str] = None,
+            *args,
+            **kwargs
+    ):
         """_send message_
 
         Args:
             object_guid (str):
                 _object guid_
 
             message (Any, optional):
@@ -73,21 +79,22 @@
                 if isinstance(file_inline, str):
                     if file_inline.startswith('http'):
                         async with aiohttp.ClientSession(headers={'user-agent': self.user_agent}) as cs:
                             async with cs.get(file_inline) as result:
                                 if result.ok:
                                     file_name = file_inline.split('/')[-1]
                                     file_inline = await result.read()
-                                    kwargs['file_name'] = kwargs.get('file_name',
-                                                                     file_name if '.' in file_name else file_name+'.'+type)
+                                    kwargs['file_name'] = kwargs.get(
+                                        'file_name',
+                                        file_name if '.' in file_name else file_name + '.' + type
+                                    )
 
                     else:
                         async with aiopen(file_inline, 'rb') as file:
-                            kwargs['file_name'] = kwargs.get(
-                                'file_name', path.basename(file_inline))
+                            kwargs['file_name'] = kwargs.get('file_name', path.basename(file_inline))
                             file_inline = await file.read()
 
                 if type in ('Music', 'Voice'):
                     thumb = None
 
                 if thumb:
                     if type in ('Video', 'Gif'):
@@ -124,15 +131,16 @@
 
         result = await self.builder('sendMessage', input=input)
 
         if auto_delete is not None:
             if not isinstance(auto_delete, int):
                 raise ValueError('The `auto_delete` parameter can only be Integer.')
 
-            create_task(self.auto_delete_message(result.object_guid,
-                                                         result.message_id,
-                                                         auto_delete))
+            create_task(
+                self.auto_delete_message(
+                    result.object_guid,
+                    result.message_id,
+                    auto_delete
+                )
+            )
 
         return result
-        # message = messages.SendMessage(**result.to_dict())
-        # await message.set_shared_data(self, message)
-        # return message
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/utilities/__init__.py` & `aiorubika-1.0.0/aiorubika/methods/utilities/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     Run,
     UploadFile,
     Download,
     GetUpdates,
     DownloadProfilePicture,
     GetMembers,
 ):
-    pass
+    pass
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/utilities/download.py` & `aiorubika-1.0.0/aiorubika/methods/utilities/download.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,31 @@
-import rubpy
 import aiofiles
 
+import aiorubika
+
+
 class Download:
-    async def download(self: "rubpy.Client", file_inline: "rubpy.types.Results", save_as: str = None, chunk_size: int = 131072, callback=None, *args, **kwargs):
+
+    async def download(
+            self: "aiorubika.Client",
+            file_inline: "aiorubika.types.Results",
+            save_as: str = None,
+            chunk_size: int = 131072,
+            callback=None,
+            *args,
+            **kwargs
+    ):
         result = await self.connection.download(
             file_inline.dc_id,
             file_inline.file_id,
             file_inline.access_hash_rec,
             file_inline.size,
             chunk=chunk_size,
-            callback=callback)
+            callback=callback
+        )
 
         if isinstance(save_as, str):
             async with aiofiles.open(save_as, 'wb+') as file:
                 await file.write(result)
                 return save_as
 
-        return result
+        return result
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/utilities/download_profile_picture.py` & `aiorubika-1.0.0/aiorubika/methods/utilities/download_profile_picture.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import rubpy
+import aiorubika
+
 
 class DownloadProfilePicture:
+
     async def download_profile_picture(
-            self: "rubpy.Client",
+            self: "aiorubika.Client",
             object_guid: str,
     ):
         object = await self.get_info(object_guid)
 
         if object_guid.startswith('c0'):
             avatar_thumbnail = object.channel.avatar_thumbnail
         elif object_guid.startswith('g0'):
@@ -16,8 +18,8 @@
 
         if avatar_thumbnail:
             async with self.connection.session.get(
                 url=f'https://messenger{avatar_thumbnail.dc_id}.iranlms.ir/InternFile.ashx',
                 params={'id': avatar_thumbnail.file_id, 'ach': avatar_thumbnail.access_hash_rec},
             ) as response:
                 if response.ok:
-                    return await response.read()
+                    return await response.read()
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/utilities/start.py` & `aiorubika-1.0.0/aiorubika/methods/utilities/start.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from ... import exceptions
 from ...crypto import Crypto
+
 from Crypto.PublicKey import RSA
 from Crypto.Signature import pkcs1_15
 
 
 class Start:
     async def start(self, phone_number: str = None):
         if not hasattr(self, 'connection'):
             await self.connect()
 
         try:
-            #self._logger.info('user info', extra={'data': await self.get_me()})
             self.decode_auth = Crypto.decode_auth(self.auth) if self.auth is not None else None
             self.import_key = pkcs1_15.new(RSA.import_key(self.private_key.encode())) if self.private_key is not None else None
             await self.get_me()
 
         except exceptions.NotRegistered:
-            #self._logger.debug('user not registered!')
             if phone_number is None:
                 phone_number = input('Phone Number: ')
                 is_phone_number_true = True
                 while is_phone_number_true:
                     if input(f'Is the {phone_number} correct[y or n] > ').lower() == 'y':
                         is_phone_number_true = False
                     else:
@@ -42,31 +41,32 @@
 
                     if result.status == 'OK':
                         break
 
             public_key, self.private_key = Crypto.create_keys()
             while True:
                 phone_code = input('Code: ')
-
                 result = await self.sign_in(
                     phone_code=phone_code,
                     phone_number=phone_number,
                     phone_code_hash=result.phone_code_hash,
-                    public_key=public_key)
+                    public_key=public_key
+                )
 
                 if result.status == 'OK':
                     result.auth = Crypto.decrypt_RSA_OAEP(self.private_key, result.auth)
-                    self.key = Crypto.passphrase(result.auth)
                     self.auth = result.auth
+                    self.key = Crypto.passphrase(result.auth)
                     self.decode_auth = Crypto.decode_auth(self.auth)
                     self.import_key = pkcs1_15.new(RSA.import_key(self.private_key.encode())) if self.private_key is not None else None
                     self.session.insert(
                         auth=self.auth,
                         guid=result.user.user_guid,
                         user_agent=self.user_agent,
                         phone_number=result.user.phone,
-                        private_key=self.private_key)
+                        private_key=self.private_key
+                    )
 
                     await self.register_device()
                     break
 
-        return self
+        return self
```

### Comparing `aiorubika-0.0.2/aiorubika/methods/utilities/thumbnail.py` & `aiorubika-1.0.0/aiorubika/methods/utilities/thumbnail.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import base64
-import typing
-import tempfile
 import warnings
+import tempfile
+import typing
+import base64
 import io
 
 try:
     import cv2
     import numpy as np
 
 except ImportError as e:
@@ -19,19 +19,21 @@
     PIL = None
 
 
 class ResultMedia:
     def __repr__(self) -> str:
         return repr(vars(self))
 
-    def __init__(self,
-                 image: bytes,
-                 width: typing.Optional[int] = 200,
-                 height: typing.Optional[int] = 200,
-                 seconds: typing.Optional[int] = 1) -> None:
+    def __init__(
+            self,
+            image: bytes,
+            width: typing.Optional[int] = 200,
+            height: typing.Optional[int] = 200,
+            seconds: typing.Optional[int] = 1
+    ) -> None:
         self.image = image
         self.width = width
         self.height = height
         self.seconds = seconds
 
         if hasattr(cv2, 'imdecode'):
             if not isinstance(image, np.ndarray):
@@ -40,72 +42,65 @@
 
             self.image = self.ndarray_to_bytes(image)
 
     def ndarray_to_bytes(self, image, *args, **kwargs) -> str:
         if hasattr(cv2, 'resize'):
             self.width = image.shape[1]
             self.height = image.shape[0]
-            image = cv2.resize(image,
-                               (round(self.width / 10), round(self.height / 10)),
-                               interpolation=cv2.INTER_CUBIC)
+            image = cv2.resize(
+                image,
+                (round(self.width / 10), round(self.height / 10)),
+                interpolation=cv2.INTER_CUBIC
+            )
 
             status, buffer = cv2.imencode('.png', image)
             if status is True:
                 return io.BytesIO(buffer).read()
 
     def to_base64(self):
         return base64.b64encode(self.image).decode('utf-8')
 
 
 class MediaThumbnail:
     @classmethod
     def from_image(cls, image: bytes) -> ResultMedia:
-        # Check if PIL is avaliable
         if PIL is not None:
             image, output = PIL.Image.open(io.BytesIO(image)), io.BytesIO()
             width, height = image.size
             image.save(output, format='PNG')
             return ResultMedia(output.getvalue(), width=width, height=height)
 
-        # Check if OpenCV and NumPy are available
         if cv2 is None or np is None:
             warnings.warn('OpenCV or NumPy not found, image processing disabled')
             return None
 
-        # If image is not a NumPy array, convert it
         if not isinstance(image, np.ndarray):
             image = np.frombuffer(image, dtype=np.uint8)
             image = cv2.imdecode(image, flags=1)
 
-        # Resize the image
         height, width = image.shape[0], image.shape[1]
         image = cv2.resize(image, (round(width / 10), round(height / 10)), interpolation=cv2.INTER_CUBIC)
 
-        # Encode the image to PNG format
         status, buffer = cv2.imencode('.png', image)
         if status:
             return ResultMedia(bytes(buffer), width=width, height=height)
 
     @classmethod
     def from_video(cls, video: bytes) -> typing.Optional[ResultMedia]:
-        # Check if OpenCV is available
         if cv2 is None:
             warnings.warn('OpenCV not found, video processing disabled')
             return None
 
-        # Write video content to a temporary file
         with tempfile.NamedTemporaryFile(mode='wb+', suffix='.mp4') as file:
             file.write(video)
 
-            # Read the video using OpenCV
             capture = cv2.VideoCapture(file.name)
             status, image = capture.read()
 
-            # If successful, calculate video duration and create ResultMedia object
             if status is True:
                 fps = capture.get(cv2.CAP_PROP_FPS)
                 frames = capture.get(cv2.CAP_PROP_FRAME_COUNT)
                 seconds = int(frames / fps) * 1000
                 width = image.shape[1]
                 height = image.shape[0]
 
-                return ResultMedia(image, width, height, seconds)
+                return ResultMedia(image, width, height, seconds)
```

### Comparing `aiorubika-0.0.2/aiorubika/network.py` & `aiorubika-1.0.0/aiorubika/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import asyncio
 import aiohttp
-import aiorubika
 import aiofiles
 import json
 import os
+
+import aiorubika
+
 from .crypto import Crypto
-from . import exceptions
 from .types import Results
+from . import exceptions
+
 
 def capitalize(text: str):
     return ''.join([c.title() for c in text.split('_')])
 
+
 class Network:
-    HEADERS = {'user-agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
-                              'AppleWebKit/537.36 (KHTML, like Gecko)'
-                              'Chrome/102.0.0.0 Safari/537.36'),
-            	'origin': 'https://web.rubika.ir',
-            	'referer': 'https://web.rubika.ir/',
-                'connection': 'keep-alive',
-                }
+
+    HEADERS: dict = {
+        'user-agent': (
+            'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
+            'AppleWebKit/537.36 (KHTML, like Gecko)'
+            'Chrome/102.0.0.0 Safari/537.36'
+        ),
+        'origin': 'https://web.rubika.ir',
+        'referer': 'https://web.rubika.ir/',
+        'connection': 'keep-alive',
+    }
 
     def __init__(self, client: "aiorubika.Client") -> None:
         self.client = client
         connector = aiohttp.TCPConnector(verify_ssl=False)
         self.json_decoder = json.JSONDecoder().decode
         self.json_encoder = json.JSONEncoder().encode
         self.session = aiohttp.ClientSession(
@@ -86,22 +94,22 @@
             except aiohttp.ClientError:
                 print('Client error, try again ({})'.format(_))
 
             except Exception as err:
                 print('Unknown Error:', err, '{}'.format(_))
 
     async def send(self, **kwargs):
-        api_version: str = str(kwargs.get('api_version', self.client.API_VERSION))
+        url: str = kwargs.get('url', self.api_url)
         auth: str = kwargs.get('auth', self.client.auth)
         client: dict = kwargs.get('client', self.client.DEFAULT_PLATFORM)
-        input: dict = kwargs.get('input', {})
+        input: dict = kwargs.get('input', dict())
         method: str = kwargs.get('method', 'getUserInfo')
         encrypt: bool = kwargs.get('encrypt', True)
         tmp_session: bool = kwargs.get('tmp_session', False)
-        url: str = kwargs.get('url', self.api_url)
+        api_version: str = str(kwargs.get('api_version', self.client.API_VERSION))
 
         data = dict(
             api_version=api_version,
         )
 
         data['tmp_session' if tmp_session is True else 'auth'] = auth if tmp_session is True else self.client.decode_auth
 
@@ -154,37 +162,33 @@
 
                 for update in package:
                     update['client'] = self.client
                     update['user_guid'] = user_guid
 
                 for func, handler in self.client.handlers.items():
                     try:
-                        # if handler is empty filters
                         if isinstance(handler, type):
                             handler = handler()
 
                         if handler.__name__ != capitalize(name):
                             return
 
-                        # analyze handlers
                         if not await handler(update=update):
                             return
 
                         asyncio.create_task(func(handler))
 
                     except exceptions.StopHandler:
                         break
 
                     except Exception:
                         pass
 
             for name, package in result.items():
                 asyncio.create_task(complete(name, package))
-                        # self._client._logger.error(
-                        #     'handler raised an exception', extra={'data': update}, exc_info=True)
 
     async def get_updates(self):
         while True:
             try:
                 async with self.session.ws_connect(self.wss_url, verify_ssl=False, heartbeat=30) as ws:
                     await self.send_json_to_ws(ws)
                     asyncio.create_task(self.send_json_to_ws(ws, data=True))
@@ -209,23 +213,33 @@
                 try:
                     await asyncio.sleep(10)
                     await ws.send_json({})
                     await self.client.get_chats_updates()
                 except:
                     pass
 
-        return await ws.send_json(dict(
-            method='handShake',
-            auth=self.client.auth,
-            api_version='5',
-            data='',
-        ))
+        return await ws.send_json(
+            dict(
+                method='handShake',
+                auth=self.client.auth,
+                api_version='5',
+                data='',
+            )
+        )
 
-    async def upload_file(self, file, mime: str = None, file_name: str = None, chunk: int = 1048576 * 2,
-                          callback=None, *args, **kwargs):
+    async def upload_file(
+            self,
+            file,
+            mime: str = None,
+            file_name: str = None,
+            chunk: int = 1048576 * 2,
+            callback=None,
+            *args,
+            **kwargs
+    ):
         if isinstance(file, str):
             if not os.path.exists(file):
                 raise ValueError('file not found in the given path')
 
             if file_name is None:
                 file_name = os.path.basename(file)
 
@@ -264,17 +278,19 @@
                             'access-hash-send': access_hash_send
                         },
                         data=data
                     )
                 result = await result.json()
                 
                 if result.get('status') != 'OK':
-                    raise exceptions.UploadError(result.get('status'),
-                                                 result.get('status_det'),
-                                                 dev_message=result.get('dev_message'))
+                    raise exceptions.UploadError(
+                        result.get('status'),
+                        result.get('status_det'),
+                        dev_message=result.get('dev_message')
+                    )
 
                 if callable(callback):
                     try:
                         await callback(len(file), index * chunk)
 
                     except exceptions.CancelledError:
                         return None
@@ -298,22 +314,30 @@
                 'file_id': id,
                 'file_name': file_name,
                 'access_hash_rec': result['data']['access_hash_rec']
             }
 
             return Results(result)
 
-        #self._client._logger.debug('upload failed', extra={'data': result})
         raise exceptions(status_det)(result, request=result)
     
-    async def download(self, dc_id: int, file_id: int, access_hash: str, size: int, chunk=131072, callback=None):
-        url = f'https://messenger{dc_id}.iranlms.ir/GetFile.ashx'
-        start_index = 0
+    async def download(
+            self,
+            dc_id: int,
+            file_id: int,
+            access_hash: str,
+            size: int,
+            chunk=131072,
+            callback=None
+    ):
         result = b''
 
+        start_index = 0
+        url = f'https://messenger{dc_id}.iranlms.ir/GetFile.ashx'
+
         headers = {
             'auth': self.client.auth,
             'access-hash-rec': access_hash,
             'file-id': str(file_id),
             'user-agent': self.client.user_agent
         }
 
@@ -329,15 +353,13 @@
                     data = await response.read()
                     if data:
                         result += data
 
                         if callback:
                             await callback(size, len(result))
 
-                # Check for the end of the file
                 if len(result) >= size:
                     break
 
-                # Update the start_index value to fetch the next part of the file
                 start_index = last_index + 1
 
-        return result
+        return result
```

### Comparing `aiorubika-0.0.2/aiorubika/parser/markdown.py` & `aiorubika-1.0.0/aiorubika/parser/markdown.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,117 +1,138 @@
-import re
-
-MARKDOWN_RE = (
-    r'\*\*(.*?)\*\*|`(.*?)`|__(.*?)__|--(.*?)--|~~(.*?)~~|\|\|(.*?)\|\||\[(.*?)\]\((\S+)\)'
-)
-
-class Markdown:
-    def __init__(self) -> None:
-        self.pattern = re.compile(MARKDOWN_RE)
-
-    def to_metadata(self, text: str) -> dict:
-        meta_data_parts = []
-
-        while True:
-            for markdown in self.pattern.finditer(text):
-                string = markdown.group(0)
-                span = markdown.span()
-                from_index = span[0]
-
-                if string.startswith('**'):
-                    text = self.pattern.sub(r'\1', text, count=1)
-                    meta_data_parts.append({
-                        'type': 'Bold',
-                        'from_index': from_index,
-                        'length': len(string) - 4,
-                    })
-                    break
-                elif string.startswith('`'):
-                    text = self.pattern.sub(r'\2', text, count=1)
-                    meta_data_parts.append({
-                        'type': 'Mono',
-                        'from_index': from_index,
-                        'length': len(string) - 4,
-                    })
-                    break
-                elif string.startswith('__'):
-                    text = self.pattern.sub(r'\3', text, count=1)
-                    meta_data_parts.append({
-                        'type': 'Italic',
-                        'from_index': from_index,
-                        'length': len(string) - 4,
-                    })
-                    break
-                elif string.startswith('--'):
-                    text = self.pattern.sub(r'\4', text, count=1)
-                    meta_data_parts.append({
-                        'type': 'Underline',
-                        'from_index': from_index,
-                        'length': len(string) - 4,
-                    })
-                    break
-                elif string.startswith('~~'):
-                    text = self.pattern.sub(r'\5', text, count=1)
-                    meta_data_parts.append({
-                        'type': 'Strike',
-                        'from_index': from_index,
-                        'length': len(string) - 4,
-                    })
-                    break
-                elif string.startswith('||'):
-                    text = self.pattern.sub(r'\6', text, count=1)
-                    meta_data_parts.append({
-                        'type': 'Spoiler',
-                        'from_index': from_index,
-                        'length': len(string) - 4,
-                    })
-                    break
-
-                else:
-                    text = self.pattern.sub(r'\7', text, count=1)
-                    mention_text_object_type = 'hyperlink'
-                    mention_type = 'MentionText'
-                    mention_text_object_guid = markdown.group(8)
-                    length = len(markdown.group(7))
-
-                    if mention_text_object_guid.startswith('u'):
-                        mention_text_object_type = 'User'
-                    elif mention_text_object_guid.startswith('g'):
-                        mention_text_object_type = 'Group'
-                    elif mention_text_object_guid.startswith('c'):
-                        mention_text_object_type = 'Channel'
-                    else:
-                        mention_type = 'Link'
-
-                    if mention_type == 'MentionText':
-                        meta_data_parts.append({
-                            'type': mention_type,
-                            'from_index': from_index,
-                            'length': length,
-                            'mention_text_object_guid': mention_text_object_guid,
-                            'mention_text_object_type': mention_text_object_type
-                        })
-                        break
-
-                    else:
-                        meta_data_parts.append({
-                            'from_index': from_index,
-                            'length': length,
-                            'link': {
-                                'hyperlink_data': {
-                                    'url': mention_text_object_guid,
-                                },
-                                'type': mention_text_object_type,
-                            },
-                            'type': mention_type,
-                        })
-                        break
-
-            else:
-                break
-
-        result = {'text': text.strip()}
-
-        if meta_data_parts:
-            result['metadata'] = {'meta_data_parts': meta_data_parts}
-
-        return result
+import re
+
+MARKDOWN_RE = (
+    r'\*\*(.*?)\*\*|`(.*?)`|__(.*?)__|--(.*?)--|~~(.*?)~~|\|\|(.*?)\|\||\[(.*?)\]\((\S+)\)'
+)
+
+
+class Markdown:
+
+    def __init__(self) -> None:
+        self.pattern = re.compile(MARKDOWN_RE)
+
+    def to_metadata(self, text: str) -> dict:
+
+        meta_data_parts = list()
+
+        while True:
+            for markdown in self.pattern.finditer(text):
+                string = markdown.group(0)
+                span = markdown.span()
+                from_index = span[0]
+
+                if string.startswith('**'):
+                    text = self.pattern.sub(r'\1', text, count=1)
+                    meta_data_parts.append(
+                        {
+                            'type': 'Bold',
+                            'from_index': from_index,
+                            'length': len(string) - 4,
+                        }
+                    )
+                    break
+                elif string.startswith('`'):
+                    text = self.pattern.sub(r'\2', text, count=1)
+                    meta_data_parts.append(
+                        {
+                            'type': 'Mono',
+                            'from_index': from_index,
+                            'length': len(string) - 4,
+                        }
+                    )
+                    break
+                elif string.startswith('__'):
+                    text = self.pattern.sub(r'\3', text, count=1)
+                    meta_data_parts.append(
+                        {
+                            'type': 'Italic',
+                            'from_index': from_index,
+                            'length': len(string) - 4,
+                        }
+                    )
+                    break
+                elif string.startswith('--'):
+                    text = self.pattern.sub(r'\4', text, count=1)
+                    meta_data_parts.append(
+                        {
+                            'type': 'Underline',
+                            'from_index': from_index,
+                            'length': len(string) - 4,
+                        }
+                    )
+                    break
+                elif string.startswith('~~'):
+                    text = self.pattern.sub(r'\5', text, count=1)
+                    meta_data_parts.append(
+                        {
+                            'type': 'Strike',
+                            'from_index': from_index,
+                            'length': len(string) - 4,
+                        }
+                    )
+                    break
+                elif string.startswith('||'):
+                    text = self.pattern.sub(r'\6', text, count=1)
+                    meta_data_parts.append(
+                        {
+                            'type': 'Spoiler',
+                            'from_index': from_index,
+                            'length': len(string) - 4,
+                        }
+                    )
+                    break
+
+                else:
+                    text = self.pattern.sub(r'\7', text, count=1)
+                    mention_text_object_type = 'hyperlink'
+                    mention_type = 'MentionText'
+                    mention_text_object_guid = markdown.group(8)
+                    length = len(markdown.group(7))
+
+                    if mention_text_object_guid.startswith('u'):
+                        mention_text_object_type = 'User'
+                    elif mention_text_object_guid.startswith('g'):
+                        mention_text_object_type = 'Group'
+                    elif mention_text_object_guid.startswith('c'):
+                        mention_text_object_type = 'Channel'
+                    else:
+                        mention_type = 'Link'
+
+                    if mention_type == 'MentionText':
+                        meta_data_parts.append(
+                            {
+                                'type': mention_type,
+                                'from_index': from_index,
+                                'length': length,
+                                'mention_text_object_guid': mention_text_object_guid,
+                                'mention_text_object_type': mention_text_object_type
+                            }
+                        )
+                        break
+
+                    else:
+                        meta_data_parts.append(
+                            {
+                                'from_index': from_index,
+                                'length': length,
+                                'link': {
+                                    'hyperlink_data': {
+                                        'url': mention_text_object_guid,
+                                    },
+                                    'type': mention_text_object_type,
+                                },
+                                'type': mention_type,
+                            }
+                        )
+                        break
+
+            else:
+                break
+
+        result = {'text': text.strip()}
+
+        if meta_data_parts:
+            result['metadata'] = {
+                'meta_data_parts': meta_data_parts
+            }
+
+        return result
```

### Comparing `aiorubika-0.0.2/aiorubika/sessions/sqliteSession.py` & `aiorubika-1.0.0/aiorubika/sessions/sqlite_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,72 @@
-# import os
-import sqlite3
-
-suffix = '.rp'
-rbs_version = 1
-
-
-class SQLiteSession(object):
-
-    def __init__(self, session: str) -> None:
-        self.filename = session
-        if not session.endswith(suffix):
-            self.filename += suffix
-
-        self._connection = sqlite3.connect(self.filename,
-                                           check_same_thread=False)
-        cursor = self._connection.cursor()
-        cursor.execute('select name from sqlite_master '
-                       'where type=? and name=?', ('table', 'version'))
-        if cursor.fetchone():
-            cursor.execute('select version from version')
-            version = cursor.fetchone()[0]
-            if rbs_version != version:
-                self.upgrade_database(version)
-
-        else:
-            cursor.execute(
-                'create table version (version integer primary key)')
-            cursor.execute('insert into version values (?)', (rbs_version,))
-            cursor.execute('create table session (phone text primary key'
-                           ', auth text, guid text, agent text, private_key text)')
-            self._connection.commit()
-        cursor.close()
-
-    def upgrade_database(self, version):
-        pass
-
-    def information(self):
-        cursor = self._connection.cursor()
-        cursor.execute('select * from session')
-        result = cursor.fetchone()
-        cursor.close()
-        return result
-
-    def insert(self, phone_number, auth, guid, user_agent, private_key, *args, **kwargs):
-        cursor = self._connection.cursor()
-        cursor.execute(
-            'insert or replace into session (phone, auth, guid, agent, private_key)'
-            ' values (?, ?, ?, ?, ?)',
-            (phone_number, auth, guid, user_agent, private_key)
-        )
-        self._connection.commit()
-        cursor.close()
-
-    @classmethod
-    def from_string(cls, session, file_name=None):
-        info = session.information()
-        if file_name is None:
-            if info is None:
-                raise ValueError('file_name arg is not set')
-            file_name = info[0]
-
-        session = SQLiteSession(file_name)
-        if info is not None:
-            session.insert(*info)
-
-        return session
+import sqlite3
+
+suffix = '.session'
+rbs_version = 1
+
+
+class SQLiteSession(object):
+
+    def __init__(self, session: str) -> None:
+        self.filename = session
+        if not session.endswith(suffix):
+            self.filename += suffix
+
+        self._connection = sqlite3.connect(self.filename, check_same_thread=False)
+        cursor = self._connection.cursor()
+        cursor.execute(
+            'select name from sqlite_master '
+            'where type=? and name=?', ('table', 'version')
+        )
+
+        if cursor.fetchone():
+            cursor.execute('select version from version')
+            version = cursor.fetchone()[0]
+            if rbs_version != version:
+                self.upgrade_database(version)
+
+        else:
+            cursor.execute(
+                'create table version (version integer primary key)'
+            )
+
+            cursor.execute('insert into version values (?)', (rbs_version,))
+            cursor.execute(
+                'create table session (phone text primary key'
+                ', auth text, guid text, agent text, private_key text)'
+            )
+            self._connection.commit()
+        cursor.close()
+
+    def upgrade_database(self, version):
+        pass
+
+    def information(self):
+        cursor = self._connection.cursor()
+        cursor.execute('select * from session')
+        result = cursor.fetchone()
+        cursor.close()
+        return result
+
+    def insert(self, phone_number, auth, guid, user_agent, private_key, *args, **kwargs):
+        cursor = self._connection.cursor()
+        cursor.execute(
+            'insert or replace into session (phone, auth, guid, agent, private_key)'
+            ' values (?, ?, ?, ?, ?)',
+            (phone_number, auth, guid, user_agent, private_key)
+        )
+        self._connection.commit()
+        cursor.close()
+
+    @classmethod
+    def from_string(cls, session, file_name=None):
+        info = session.information()
+        if file_name is None:
+            if info is None:
+                raise ValueError('file_name arg is not set')
+            file_name = info[0]
+
+        session = SQLiteSession(file_name)
+        if info is not None:
+            session.insert(*info)
+
+        return session
```

### Comparing `aiorubika-0.0.2/aiorubika/sessions/stringSession.py` & `aiorubika-1.0.0/aiorubika/sessions/string_session.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import json
-import base64
-
-
-class StringSession(object):
-    def __init__(self, session: str = None) -> None:
-        self.session = self.load(session)
-
-    @classmethod
-    def load(cls, session):
-        if isinstance(session, str):
-            return json.loads(base64.b64decode(session))
-
-    @classmethod
-    def dump(cls, session):
-        if isinstance(session, list):
-            session = json.dumps(session).encode('utf-8')
-            return base64.b64encode(session).decode('utf-8')
-
-    @classmethod
-    def from_sqlite(cls, session):
-        session = cls.dump(session.information())
-        return StringSession(session)
-
-    def insert(self, phone_number, auth, guid, user_agent, *args, **kwargs):
-        self.session = [phone_number, auth, guid, user_agent]
-
-    def information(self):
-        return self.session
-
-    def save(self, file_name=None):
-        result = self.dump(self.session)
-        if result is None:
-            if isinstance(file_name, str):
-                if not file_name.endswith('.txt'):
-                    file_name += '.txt'
-                with open(file_name, 'w+') as file:
-                    file.write(result)
-        return result
+import json
+import base64
+
+
+class StringSession(object):
+    def __init__(self, session: str = None) -> None:
+        self.session = self.load(session)
+
+    @classmethod
+    def load(cls, session):
+        if isinstance(session, str):
+            return json.loads(base64.b64decode(session))
+
+    @classmethod
+    def dump(cls, session):
+        if isinstance(session, list):
+            session = json.dumps(session).encode('utf-8')
+            return base64.b64encode(session).decode('utf-8')
+
+    @classmethod
+    def from_sqlite(cls, session):
+        session = cls.dump(session.information())
+        return StringSession(session)
+
+    def insert(self, phone_number, auth, guid, user_agent, *args, **kwargs):
+        self.session = [phone_number, auth, guid, user_agent]
+
+    def information(self):
+        return self.session
+
+    def save(self, file_name=None):
+        result = self.dump(self.session)
+        if result is None:
+            if isinstance(file_name, str):
+                if not file_name.endswith('.txt'):
+                    file_name += '.txt'
+                with open(file_name, 'w+') as file:
+                    file.write(result)
+        return result
```

### Comparing `aiorubika-0.0.2/aiorubika/types/chat.py` & `aiorubika-1.0.0/aiorubika/types/chat.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import Optional, List
-from pydantic import BaseModel
-from .message import Message
-from .abs_object import AbsObject
-
-
-class Chat(BaseModel):
-    object_guid: Optional[str] = None
-    access: Optional[List[str]] = None
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[Message] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    abs_object: Optional[AbsObject] = None
-    is_blocked: Optional[bool] = None
-    last_message_id: Optional[str] = None
-    last_deleted_mid: Optional[str] = None
-    is_in_contact: Optional[bool] = None
+from typing import Optional, List
+from pydantic import BaseModel
+
+from .abs_object import AbsObject
+from .message import Message
+
+
+class Chat(BaseModel):
+    object_guid: Optional[str] = None
+    access: Optional[List[str]] = None
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[Message] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    abs_object: Optional[AbsObject] = None
+    is_blocked: Optional[bool] = None
+    last_message_id: Optional[str] = None
+    last_deleted_mid: Optional[str] = None
+    is_in_contact: Optional[bool] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/file_inline.py` & `aiorubika-1.0.0/aiorubika/types/file_inline.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Optional
-from pydantic import BaseModel
-
-
-class FileInline(BaseModel):
-    file_id: Optional[int] = None
-    mime: Optional[str] = None
-    dc_id: Optional[int] = None
-    access_hash_rec: Optional[str] = None
-    file_name: Optional[str] = None
-    thumb_inline: Optional[str] = None
-    width: Optional[int] = None
-    height: Optional[int] = None
-    time: Optional[int] = None
-    size: Optional[int] = None
-    type: Optional[str] = None
-    is_round: Optional[bool] = None
-    music_performer: Optional[str] = None
+from pydantic import BaseModel
+from typing import Optional
+
+
+class FileInline(BaseModel):
+    file_id: Optional[int] = None
+    mime: Optional[str] = None
+    dc_id: Optional[int] = None
+    access_hash_rec: Optional[str] = None
+    file_name: Optional[str] = None
+    thumb_inline: Optional[str] = None
+    width: Optional[int] = None
+    height: Optional[int] = None
+    time: Optional[int] = None
+    size: Optional[int] = None
+    type: Optional[str] = None
+    is_round: Optional[bool] = None
+    music_performer: Optional[str] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/member.py` & `aiorubika-1.0.0/aiorubika/types/member.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from pydantic import BaseModel
-from typing import Optional
-from .online_time import OnlineTime
-from .avatar_thumbnail import AvatarThumbnail
-
-
-class Member(BaseModel):
-    member_type: Optional[str] = None
-    member_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-    last_online: Optional[int] = None
-    join_type: Optional[str] = None
-    username: Optional[str] = None
-    online_time: Optional[OnlineTime] = None
+from pydantic import BaseModel
+from typing import Optional
+
+from .online_time import OnlineTime
+from .avatar_thumbnail import AvatarThumbnail
+
+
+class Member(BaseModel):
+    member_type: Optional[str] = None
+    member_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+    last_online: Optional[int] = None
+    join_type: Optional[str] = None
+    username: Optional[str] = None
+    online_time: Optional[OnlineTime] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/models/chats.py` & `aiorubika-1.0.0/aiorubika/types/models/chats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,151 @@
-from pydantic import BaseModel
-from typing import Optional, List
-
-class AvatarThumbnail(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-
-class OnlineTime(BaseModel):
-    type: Optional[str] = None
-    exact_time: Optional[int] = None
-
-class LastMessage(BaseModel):
-    message_id: Optional[str] = None
-    type: Optional[str] = None
-    text: Optional[str] = None
-    author_object_guid: Optional[str] = None
-    is_mine: Optional[bool] = None
-    author_title: Optional[str] = None
-    author_type: Optional[str] = None
-
-class ChatInfo(BaseModel):
-    object_guid: Optional[str] = None
-    access: Optional[List[str]] = []
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[LastMessage] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-
-class UserInfo(BaseModel):
-    user_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    phone: Optional[str] = None
-    username: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    last_online: Optional[int] = None
-    bio: Optional[str] = None
-    is_deleted: Optional[bool] = None
-    is_verified: Optional[bool] = None
-    online_time: Optional[OnlineTime] = None
-
-class AvatarData(BaseModel):
-    avatar_id: Optional[str] = None
-    thumbnail: Optional[AvatarThumbnail] = None
-    main: Optional[AvatarThumbnail] = None
-    create_time: Optional[int] = None
-
-class GetAvatars(BaseModel):
-    avatars: Optional[List[AvatarData]] = []
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class ChatAccess(BaseModel):
-    access: Optional[List[str]] = []
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[LastMessage] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    pinned_message_id: Optional[str] = None
-    abs_object: Optional[dict] = None
-    is_blocked: Optional[bool] = None
-    last_message_id: Optional[str] = None
-    last_deleted_mid: Optional[str] = None
-    slow_mode_duration: Optional[int] = None
-    group_my_last_send_time: Optional[int] = None
-    pinned_message_ids: Optional[List[str]] = []
-
-class ChatUpdate(BaseModel):
-    object_guid: Optional[str] = None
-    action: Optional[str] = None
-    chat: Optional[ChatAccess] = None
-    updated_parameters: Optional[List[str]] = []
-    timestamp: Optional[str] = None
-    type: Optional[str] = None
-
-class DeleteAvatar(BaseModel):
-    user: Optional[UserInfo] = None
-    chat_update: Optional[ChatUpdate] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetChats(BaseModel):
-    chats: Optional[List[ChatInfo]] = []
-    next_start_id: Optional[str] = None
-    state: Optional[int] = None
-    has_continue: Optional[bool] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class SeenChats(BaseModel):
-    chat_updates: Optional[List[ChatUpdate]] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class SetActionChat(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetChatsUpdates(BaseModel):
-    chats: List[ChatInfo]
-    new_state: Optional[int] = None
-    status: Optional[str] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class SendChatActivity(BaseModel):
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class DeleteChatHistory(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class SearchChatMessages(BaseModel):
-    message_ids: List[str]
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
+from typing import Optional, List
+from pydantic import BaseModel
+
+
+class AvatarThumbnail(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+
+
+class OnlineTime(BaseModel):
+    type: Optional[str] = None
+    exact_time: Optional[int] = None
+
+
+class LastMessage(BaseModel):
+    message_id: Optional[str] = None
+    type: Optional[str] = None
+    text: Optional[str] = None
+    author_object_guid: Optional[str] = None
+    is_mine: Optional[bool] = None
+    author_title: Optional[str] = None
+    author_type: Optional[str] = None
+
+
+class ChatInfo(BaseModel):
+    object_guid: Optional[str] = None
+    access: Optional[List[str]] = []
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[LastMessage] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+
+
+class UserInfo(BaseModel):
+    user_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    phone: Optional[str] = None
+    username: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    last_online: Optional[int] = None
+    bio: Optional[str] = None
+    is_deleted: Optional[bool] = None
+    is_verified: Optional[bool] = None
+    online_time: Optional[OnlineTime] = None
+
+
+class AvatarData(BaseModel):
+    avatar_id: Optional[str] = None
+    thumbnail: Optional[AvatarThumbnail] = None
+    main: Optional[AvatarThumbnail] = None
+    create_time: Optional[int] = None
+
+
+class GetAvatars(BaseModel):
+    avatars: Optional[List[AvatarData]] = []
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class ChatAccess(BaseModel):
+    access: Optional[List[str]] = []
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[LastMessage] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    pinned_message_id: Optional[str] = None
+    abs_object: Optional[dict] = None
+    is_blocked: Optional[bool] = None
+    last_message_id: Optional[str] = None
+    last_deleted_mid: Optional[str] = None
+    slow_mode_duration: Optional[int] = None
+    group_my_last_send_time: Optional[int] = None
+    pinned_message_ids: Optional[List[str]] = []
+
+
+class ChatUpdate(BaseModel):
+    object_guid: Optional[str] = None
+    action: Optional[str] = None
+    chat: Optional[ChatAccess] = None
+    updated_parameters: Optional[List[str]] = []
+    timestamp: Optional[str] = None
+    type: Optional[str] = None
+
+
+class DeleteAvatar(BaseModel):
+    user: Optional[UserInfo] = None
+    chat_update: Optional[ChatUpdate] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetChats(BaseModel):
+    chats: Optional[List[ChatInfo]] = []
+    next_start_id: Optional[str] = None
+    state: Optional[int] = None
+    has_continue: Optional[bool] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class SeenChats(BaseModel):
+    chat_updates: Optional[List[ChatUpdate]] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class SetActionChat(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetChatsUpdates(BaseModel):
+    chats: List[ChatInfo]
+    new_state: Optional[int] = None
+    status: Optional[str] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class SendChatActivity(BaseModel):
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class DeleteChatHistory(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class SearchChatMessages(BaseModel):
+    message_ids: List[str]
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/models/contacts.py` & `aiorubika-1.0.0/aiorubika/types/models/contacts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,62 @@
-from pydantic import BaseModel
-from typing import Optional, List
-
-class OnlineTime(BaseModel):
-    type: Optional[str] = None
-    approximate_period: Optional[str] = None
-
-class AvatarThumbnail(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-    file_name: Optional[str] = None
-    cdn_tag: Optional[str] = None
-
-class WarningInfo(BaseModel):
-    warning_id: Optional[str] = None
-    title: Optional[str] = None
-    text: Optional[str] = None
-    link: Optional[dict] = None
-    title_color: Optional[dict] = None
-
-class User(BaseModel):
-    user_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    phone: Optional[str] = None
-    username: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    last_online: Optional[int] = None
-    bio: Optional[str] = None
-    is_deleted: Optional[bool] = None
-    is_verified: Optional[bool] = None
-    online_time: Optional[OnlineTime] = None
-    warning_info: Optional[WarningInfo] = None
-
-class DeleteContact(BaseModel):
-    user: Optional[User] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class AddAddressBook(BaseModel):
-    user: Optional[User] = None
-    user_exist: Optional[bool] = None
-    timestamp: Optional[str] = None
-    can_receive_call: Optional[bool] = None
-    can_video_call: Optional[bool] = None
-
-class GetContacts(BaseModel):
-    users: Optional[List[User]] = []
-    next_start_id: Optional[str] = None
-    has_continue: Optional[bool] = None
-    state: Optional[int] = None
-    timestamp: Optional[str] = None
+from pydantic import BaseModel
+from typing import Optional, List
+
+
+class OnlineTime(BaseModel):
+    type: Optional[str] = None
+    approximate_period: Optional[str] = None
+
+
+class AvatarThumbnail(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+    file_name: Optional[str] = None
+    cdn_tag: Optional[str] = None
+
+
+class WarningInfo(BaseModel):
+    warning_id: Optional[str] = None
+    title: Optional[str] = None
+    text: Optional[str] = None
+    link: Optional[dict] = None
+    title_color: Optional[dict] = None
+
+
+class User(BaseModel):
+    user_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    phone: Optional[str] = None
+    username: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    last_online: Optional[int] = None
+    bio: Optional[str] = None
+    is_deleted: Optional[bool] = None
+    is_verified: Optional[bool] = None
+    online_time: Optional[OnlineTime] = None
+    warning_info: Optional[WarningInfo] = None
+
+
+class DeleteContact(BaseModel):
+    user: Optional[User] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class AddAddressBook(BaseModel):
+    user: Optional[User] = None
+    user_exist: Optional[bool] = None
+    timestamp: Optional[str] = None
+    can_receive_call: Optional[bool] = None
+    can_video_call: Optional[bool] = None
+
+
+class GetContacts(BaseModel):
+    users: Optional[List[User]] = []
+    next_start_id: Optional[str] = None
+    has_continue: Optional[bool] = None
+    state: Optional[int] = None
+    timestamp: Optional[str] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/models/extras.py` & `aiorubika-1.0.0/aiorubika/types/models/extras.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,238 +1,268 @@
-from pydantic import BaseModel, HttpUrl, Field, PositiveInt
-from typing import Optional, List
-
-class AvatarThumbnail(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-
-class Object(BaseModel):
-    object_guid: Optional[str] = None
-    type: Optional[str] = None
-    title: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-    count_members: Optional[int] = None
-    username: Optional[str] = None
-
-class SearchGlobalObjects(BaseModel):
-    objects: List[Object]
-    has_continue: Optional[bool] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class OnlineTime(BaseModel):
-    type: Optional[str] = None
-    approximate_period: Optional[str] = None
-
-class AvatarThumbnail(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-
-class LastMessage(BaseModel):
-    message_id: Optional[str] = None
-    type: Optional[str] = None
-    text: Optional[str] = None
-    author_object_guid: Optional[str] = None
-    is_mine: Optional[bool] = None
-    author_type: Optional[str] = None
-
-class AbsObject(BaseModel):
-    object_guid: Optional[str] = None
-    type: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-
-class Chat(BaseModel):
-    object_guid: Optional[str] = None
-    access: Optional[List[str]] = []
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[LastMessage] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    abs_object: Optional[AbsObject] = None
-    is_blocked: Optional[bool] = None
-    last_message_id: Optional[str] = None
-    last_deleted_mid: Optional[str] = None
-    is_in_contact: Optional[bool] = None
-
-class ChatReactionSetting(BaseModel):
-    reaction_type: Optional[str] = Field(None, description="Type of reactions in chat")
-    selected_reactions: Optional[List[str]] = Field(None, description="List of selected reactions in the chat")
-
-class User(BaseModel):
-    user_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    phone: Optional[str] = None
-    username: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    last_online: Optional[int] = None
-    bio: Optional[str] = None
-    is_deleted: Optional[bool] = None
-    is_verified: Optional[bool] = None
-    online_time: Optional[OnlineTime] = None
-
-class Channel(BaseModel):
-    channel_guid: Optional[str] = Field(None, description="Channel ID")
-    channel_title: Optional[str] = Field(None, description="Channel title")
-    avatar_thumbnail: Optional[AvatarThumbnail] = Field(None, description="Profile image information")
-    count_members: Optional[PositiveInt] = Field(None, description="Number of channel members")
-    description: Optional[str] = Field(None, description="Channel description")
-    username: Optional[str] = Field(None, description="Channel username")
-    is_deleted: Optional[bool] = Field(None, description="Channel deletion status")
-    is_verified: Optional[bool] = Field(None, description="Channel verification status")
-    share_url: Optional[HttpUrl] = Field(None, description="Channel sharing URL")
-    channel_type: Optional[str] = Field(None, description="Channel type")
-    sign_messages: Optional[bool] = Field(None, description="Message signing capability status")
-    chat_reaction_setting: Optional[ChatReactionSetting] = Field(None, description="Conversation reaction settings")
-
-class GetObjectByUsername(BaseModel):
-    exist: Optional[bool] = None
-    type: Optional[str] = None
-    user: Optional[User] = None
-    channel: Optional[Channel] = None
-    chat: Optional[Chat] = None
-    timestamp: Optional[str] = None
-    is_in_contact: Optional[bool] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class OpenChatData(BaseModel):
-    object_guid: Optional[str] = None
-    object_type: Optional[str] = None
-    message_id: Optional[int] = None
-
-class LinkData(BaseModel):
-    type: Optional[str] = None
-    link_url: Optional[str] = None
-    open_chat_data: Optional[OpenChatData] = None
-
-class GetLinkFromAppUrl(BaseModel):
-    link: Optional[LinkData] = None
-
-class ChatGuidType(BaseModel):
-    type: Optional[str] = None
-    object_guid: Optional[str] = None
-
-class MessageInfo(BaseModel):
-    message_id: Optional[str] = None
-    type: Optional[str] = None
-    text: Optional[str] = None
-    is_mine: Optional[bool] = None
-
-class ChatInfo(BaseModel):
-    time_string: Optional[str] = None
-    last_message: Optional[MessageInfo] = None
-    time: Optional[int] = None
-    last_message_id: Optional[str] = None
-    group_voice_chat_id: Optional[str] = None
-
-class ChatUpdate(BaseModel):
-    object_guid: Optional[str] = None
-    action: Optional[str] = None
-    chat: Optional[ChatInfo] = None
-    updated_parameters: Optional[List[str]] = None
-    timestamp: Optional[str] = None
-    type: Optional[str] = None
-
-class PerformerData(BaseModel):
-    type: Optional[str] = None
-    object_guid: Optional[str] = None
-
-class EventData(BaseModel):
-    type: Optional[str] = None
-    performer_object: Optional[PerformerData] = None
-
-class MessageData(BaseModel):
-    message_id: Optional[str] = None
-    text: Optional[str] = None
-    time: Optional[str] = None
-    is_edited: Optional[bool] = None
-    type: Optional[str] = None
-    event_data: Optional[EventData] = None
-
-class MessageUpdate(BaseModel):
-    message_id: Optional[str] = None
-    action: Optional[str] = None
-    message: Optional[MessageData] = None
-    updated_parameters: Optional[List[str]] = None
-    timestamp: Optional[str] = None
-    prev_message_id: Optional[str] = None
-    object_guid: Optional[str] = None
-    type: Optional[str] = None
-    state: Optional[str] = None
-
-class GroupVoiceChatData(BaseModel):
-    voice_chat_id: Optional[str] = None
-    state: Optional[str] = None
-    join_muted: Optional[bool] = None
-    participant_count: Optional[int] = None
-    title: Optional[str] = None
-    version: Optional[int] = None
-
-class ChannelVoiceChatData(BaseModel):
-    voice_chat_id: Optional[str] = None
-    state: Optional[str] = None
-    join_muted: Optional[bool] = None
-    participant_count: Optional[int] = None
-    title: Optional[str] = None
-    version: Optional[int] = None
-
-class GroupVoiceChatUpdate(BaseModel):
-    voice_chat_id: Optional[str] = None
-    group_guid: Optional[str] = None
-    action: Optional[str] = None
-    group_voice_chat: Optional[GroupVoiceChatData] = None
-    updated_parameters: Optional[List[str]] = None
-    timestamp: Optional[str] = None
-    chat_guid_type: Optional[ChatGuidType] = None
-
-class ChannelVoiceChatUpdate(BaseModel):
-    voice_chat_id: Optional[str] = None
-    channel_guid: Optional[str] = None
-    action: Optional[str] = None
-    channel_voice_chat: Optional[ChannelVoiceChatData] = None
-    updated_parameters: Optional[List[str]] = None
-    timestamp: Optional[str] = None
-    chat_guid_type: Optional[ChatGuidType] = None
-
-class ExistGroupVoiceChat(BaseModel):
-    voice_chat_id: Optional[str] = None
-    state: Optional[str] = None
-    join_muted: Optional[bool] = None
-    participant_count: Optional[int] = None
-    title: Optional[str] = None
-    version: Optional[int] = None
-
-class ExistChannelVoiceChat(BaseModel):
-    voice_chat_id: Optional[str] = None
-    state: Optional[str] = None
-    join_muted: Optional[bool] = None
-    participant_count: Optional[int] = None
-    title: Optional[str] = None
-    version: Optional[int] = None
-
-class CreateVoiceCall(BaseModel):
-    status: Optional[str] = None
-    chat_update: Optional[ChatUpdate] = None
-    message_update: Optional[MessageUpdate] = None
-    group_voice_chat_update: Optional[GroupVoiceChatUpdate] = None
-    channel_voice_chat_update: Optional[ChannelVoiceChatUpdate] = None
-    exist_group_voice_chat: Optional[ExistGroupVoiceChat] = None
-    exist_channel_voice_chat: Optional[ExistChannelVoiceChat] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
+from pydantic import BaseModel, HttpUrl, Field, PositiveInt
+from typing import Optional, List
+
+
+class AvatarThumbnail(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+
+
+class Object(BaseModel):
+    object_guid: Optional[str] = None
+    type: Optional[str] = None
+    title: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+    count_members: Optional[int] = None
+    username: Optional[str] = None
+
+
+class SearchGlobalObjects(BaseModel):
+    objects: List[Object]
+    has_continue: Optional[bool] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class OnlineTime(BaseModel):
+    type: Optional[str] = None
+    approximate_period: Optional[str] = None
+
+
+class AvatarThumbnail(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+
+
+class LastMessage(BaseModel):
+    message_id: Optional[str] = None
+    type: Optional[str] = None
+    text: Optional[str] = None
+    author_object_guid: Optional[str] = None
+    is_mine: Optional[bool] = None
+    author_type: Optional[str] = None
+
+
+class AbsObject(BaseModel):
+    object_guid: Optional[str] = None
+    type: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+
+
+class Chat(BaseModel):
+    object_guid: Optional[str] = None
+    access: Optional[List[str]] = []
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[LastMessage] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    abs_object: Optional[AbsObject] = None
+    is_blocked: Optional[bool] = None
+    last_message_id: Optional[str] = None
+    last_deleted_mid: Optional[str] = None
+    is_in_contact: Optional[bool] = None
+
+
+class ChatReactionSetting(BaseModel):
+    reaction_type: Optional[str] = Field(None, description="Type of reactions in chat")
+    selected_reactions: Optional[List[str]] = Field(None, description="List of selected reactions in the chat")
+
+
+class User(BaseModel):
+    user_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    phone: Optional[str] = None
+    username: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    last_online: Optional[int] = None
+    bio: Optional[str] = None
+    is_deleted: Optional[bool] = None
+    is_verified: Optional[bool] = None
+    online_time: Optional[OnlineTime] = None
+
+
+class Channel(BaseModel):
+    channel_guid: Optional[str] = Field(None, description="Channel ID")
+    channel_title: Optional[str] = Field(None, description="Channel title")
+    avatar_thumbnail: Optional[AvatarThumbnail] = Field(None, description="Profile image information")
+    count_members: Optional[PositiveInt] = Field(None, description="Number of channel members")
+    description: Optional[str] = Field(None, description="Channel description")
+    username: Optional[str] = Field(None, description="Channel username")
+    is_deleted: Optional[bool] = Field(None, description="Channel deletion status")
+    is_verified: Optional[bool] = Field(None, description="Channel verification status")
+    share_url: Optional[HttpUrl] = Field(None, description="Channel sharing URL")
+    channel_type: Optional[str] = Field(None, description="Channel type")
+    sign_messages: Optional[bool] = Field(None, description="Message signing capability status")
+    chat_reaction_setting: Optional[ChatReactionSetting] = Field(None, description="Conversation reaction settings")
+
+
+class GetObjectByUsername(BaseModel):
+    exist: Optional[bool] = None
+    type: Optional[str] = None
+    user: Optional[User] = None
+    channel: Optional[Channel] = None
+    chat: Optional[Chat] = None
+    timestamp: Optional[str] = None
+    is_in_contact: Optional[bool] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class OpenChatData(BaseModel):
+    object_guid: Optional[str] = None
+    object_type: Optional[str] = None
+    message_id: Optional[int] = None
+
+
+class LinkData(BaseModel):
+    type: Optional[str] = None
+    link_url: Optional[str] = None
+    open_chat_data: Optional[OpenChatData] = None
+
+
+class GetLinkFromAppUrl(BaseModel):
+    link: Optional[LinkData] = None
+
+
+class ChatGuidType(BaseModel):
+    type: Optional[str] = None
+    object_guid: Optional[str] = None
+
+
+class MessageInfo(BaseModel):
+    message_id: Optional[str] = None
+    type: Optional[str] = None
+    text: Optional[str] = None
+    is_mine: Optional[bool] = None
+
+
+class ChatInfo(BaseModel):
+    time_string: Optional[str] = None
+    last_message: Optional[MessageInfo] = None
+    time: Optional[int] = None
+    last_message_id: Optional[str] = None
+    group_voice_chat_id: Optional[str] = None
+
+
+class ChatUpdate(BaseModel):
+    object_guid: Optional[str] = None
+    action: Optional[str] = None
+    chat: Optional[ChatInfo] = None
+    updated_parameters: Optional[List[str]] = None
+    timestamp: Optional[str] = None
+    type: Optional[str] = None
+
+
+class PerformerData(BaseModel):
+    type: Optional[str] = None
+    object_guid: Optional[str] = None
+
+
+class EventData(BaseModel):
+    type: Optional[str] = None
+    performer_object: Optional[PerformerData] = None
+
+
+class MessageData(BaseModel):
+    message_id: Optional[str] = None
+    text: Optional[str] = None
+    time: Optional[str] = None
+    is_edited: Optional[bool] = None
+    type: Optional[str] = None
+    event_data: Optional[EventData] = None
+
+
+class MessageUpdate(BaseModel):
+    message_id: Optional[str] = None
+    action: Optional[str] = None
+    message: Optional[MessageData] = None
+    updated_parameters: Optional[List[str]] = None
+    timestamp: Optional[str] = None
+    prev_message_id: Optional[str] = None
+    object_guid: Optional[str] = None
+    type: Optional[str] = None
+    state: Optional[str] = None
+
+
+class GroupVoiceChatData(BaseModel):
+    voice_chat_id: Optional[str] = None
+    state: Optional[str] = None
+    join_muted: Optional[bool] = None
+    participant_count: Optional[int] = None
+    title: Optional[str] = None
+    version: Optional[int] = None
+
+
+class ChannelVoiceChatData(BaseModel):
+    voice_chat_id: Optional[str] = None
+    state: Optional[str] = None
+    join_muted: Optional[bool] = None
+    participant_count: Optional[int] = None
+    title: Optional[str] = None
+    version: Optional[int] = None
+
+
+class GroupVoiceChatUpdate(BaseModel):
+    voice_chat_id: Optional[str] = None
+    group_guid: Optional[str] = None
+    action: Optional[str] = None
+    group_voice_chat: Optional[GroupVoiceChatData] = None
+    updated_parameters: Optional[List[str]] = None
+    timestamp: Optional[str] = None
+    chat_guid_type: Optional[ChatGuidType] = None
+
+
+class ChannelVoiceChatUpdate(BaseModel):
+    voice_chat_id: Optional[str] = None
+    channel_guid: Optional[str] = None
+    action: Optional[str] = None
+    channel_voice_chat: Optional[ChannelVoiceChatData] = None
+    updated_parameters: Optional[List[str]] = None
+    timestamp: Optional[str] = None
+    chat_guid_type: Optional[ChatGuidType] = None
+
+
+class ExistGroupVoiceChat(BaseModel):
+    voice_chat_id: Optional[str] = None
+    state: Optional[str] = None
+    join_muted: Optional[bool] = None
+    participant_count: Optional[int] = None
+    title: Optional[str] = None
+    version: Optional[int] = None
+
+
+class ExistChannelVoiceChat(BaseModel):
+    voice_chat_id: Optional[str] = None
+    state: Optional[str] = None
+    join_muted: Optional[bool] = None
+    participant_count: Optional[int] = None
+    title: Optional[str] = None
+    version: Optional[int] = None
+
+
+class CreateVoiceCall(BaseModel):
+    status: Optional[str] = None
+    chat_update: Optional[ChatUpdate] = None
+    message_update: Optional[MessageUpdate] = None
+    group_voice_chat_update: Optional[GroupVoiceChatUpdate] = None
+    channel_voice_chat_update: Optional[ChannelVoiceChatUpdate] = None
+    exist_group_voice_chat: Optional[ExistGroupVoiceChat] = None
+    exist_channel_voice_chat: Optional[ExistChannelVoiceChat] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/models/groups.py` & `aiorubika-1.0.0/aiorubika/types/models/groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,267 +1,298 @@
-from pydantic import BaseModel
-from typing import Optional, List, Dict, Union
-
-class LastMessage(BaseModel):
-    message_id: Optional[str] = None
-    type: Optional[str] = None
-    text: Optional[str] = None
-    author_object_guid: Optional[str] = None
-    is_mine: Optional[bool] = None
-    author_title: Optional[str] = None
-    author_type: Optional[str] = None
-
-class ChatAccess(BaseModel):
-    access: Optional[List[str]] = []
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[LastMessage] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    pinned_message_id: Optional[str] = None
-    abs_object: Optional[Dict] = None
-    is_blocked: Optional[bool] = None
-    last_message_id: Optional[str] = None
-    last_deleted_mid: Optional[str] = None
-    slow_mode_duration: Optional[int] = None
-    group_my_last_send_time: Optional[int] = None
-    pinned_message_ids: Optional[List[str]] = []
-
-class ChatUpdate(BaseModel):
-    object_guid: Optional[str] = None
-    action: Optional[str] = None
-    chat: Optional[ChatAccess] = None
-    updated_parameters: Optional[List[str]] = None
-    timestamp: Optional[str] = None
-    type: Optional[str] = None
-
-class LeaveGroup(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class Group(BaseModel):
-    group_guid: Optional[str] = None
-    group_title: Optional[str] = None
-    count_members: Optional[int] = None
-    is_deleted: Optional[bool] = None
-    is_verified: Optional[bool] = None
-    slow_mode: Optional[int] = None
-    chat_history_for_new_members: Optional[str] = None
-    event_messages: Optional[bool] = None
-    chat_reaction_setting: Optional[Union[str, Dict]] = None
-
-class Chat(BaseModel):
-    object_guid: Optional[str] = None
-    action: Optional[str] = None
-    access: Optional[List[str]] = None
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[Dict] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    abs_object: Optional[Dict] = None
-    is_blocked: Optional[bool] = None
-    last_message_id: Optional[str] = None
-    last_deleted_mid: Optional[str] = None
-    slow_mode_duration: Optional[int] = None
-
-class MessageUpdate(BaseModel):
-    message_id: Optional[str] = None
-    action: Optional[str] = None
-    message: Optional[Dict] = None
-    updated_parameters: Optional[List[str]] = None
-    timestamp: Optional[str] = None
-    prev_message_id: Optional[str] = None
-    object_guid: Optional[str] = None
-    type: Optional[str] = None
-    state: Optional[str] = None
-
-class JoinGroup(BaseModel):
-    group: Optional[Group] = None
-    is_valid: Optional[bool] = None
-    chat_update: Optional[Chat] = None
-    message_update: Optional[MessageUpdate] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class AddGroup(BaseModel):
-    group: Optional[Group] = None
-    chat_update: Optional[Chat] = None
-    message_update: Optional[MessageUpdate] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class RemoveGroup(BaseModel):
-    chat_update: Optional[Chat] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetGroupInfo(BaseModel):
-    group: Optional[Group] = None
-    chat: Optional[Chat] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-    message_update: Optional[MessageUpdate] = None
-
-class GroupLink(BaseModel):
-    join_link: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class EditGroupInfo(BaseModel):
-    group: Optional[Group] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class OnlineTime(BaseModel):
-    type: Optional[str] = None
-    approximate_period: Optional[str] = None
-
-class InChatMemberList(BaseModel):
-    member_type: Optional[str] = None
-    member_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-    promoted_by_object_guid: Optional[str] = None
-    promoted_by_object_type: Optional[str] = None
-    join_type: Optional[str] = None
-    online_time: Optional[OnlineTime] = None
-
-class InChatMember(BaseModel):
-    in_chat_member: Optional[InChatMemberList] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class BanGroupMember(BaseModel):
-    group: Optional[Group] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[Dict] = None
-
-class AvatarThumbnail(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-
-class AddedInChatMember(BaseModel):
-    member_type: Optional[str] = None
-    member_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-    last_online: Optional[int] = None
-    join_type: Optional[str] = None
-    username: Optional[str] = None
-    online_time: Optional[OnlineTime] = None
-
-class AddGroupMembers(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    message_update: Optional[MessageUpdate] = None
-    added_in_chat_members: Optional[List[AddedInChatMember]] = None
-    timestamp: Optional[str] = None
-    group: Optional[Group] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class InChatGroupMember(BaseModel):
-    member_type: Optional[str] = None
-    member_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-    last_online: Optional[int] = None
-    join_type: Optional[str] = None
-    online_time: Optional[OnlineTime] = None
-    promoted_by_object_guid: Optional[str] = None
-    promoted_by_object_type: Optional[str] = None
-    removed_by_object_guid: Optional[str] = None
-    removed_by_object_type: Optional[str] = None
-
-class GetAllGroupMembers(BaseModel):
-    in_chat_members: Optional[List[InChatGroupMember]] = None
-    next_start_id: Optional[str] = None
-    has_continue: Optional[bool] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetGroupAdminMembers(BaseModel):
-    in_chat_members: Optional[List[InChatGroupMember]] = None
-    next_start_id: Optional[str] = None
-    has_continue: Optional[bool] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetGroupMentionList(BaseModel):
-    in_chat_members: Optional[List[InChatGroupMember]] = None
-    next_start_id: Optional[str] = None
-    has_continue: Optional[bool] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetGroupDefaultAccess(BaseModel):
-    access_list: Optional[List] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class OnlineTime(BaseModel):
-    type: Optional[str] = None
-    approximate_period: Optional[str] = None
-
-class TopParticipants(BaseModel):
-    member_type: Optional[str] = None
-    member_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-    username: Optional[str] = None
-    online_time: Optional[OnlineTime] = None
-
-class GroupPreviewByJoinLink(BaseModel):
-    is_valid: Optional[bool] = None
-    group: Optional[Group] = None
-    has_joined: Optional[bool] = None
-    top_participants: Optional[List[TopParticipants]] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class DeleteNoAccessGroupChat(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    status: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetGroupAdminAccessList(BaseModel):
-    access_list: Optional[List] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetBannedGroupMembers(BaseModel):
-    in_chat_members: Optional[List[InChatGroupMember]] = []
-    next_start_id: Optional[str] = None
-    has_continue: Optional[bool] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
+from pydantic import BaseModel
+from typing import Optional, List, Dict, Union
+
+
+class LastMessage(BaseModel):
+    message_id: Optional[str] = None
+    type: Optional[str] = None
+    text: Optional[str] = None
+    author_object_guid: Optional[str] = None
+    is_mine: Optional[bool] = None
+    author_title: Optional[str] = None
+    author_type: Optional[str] = None
+
+
+class ChatAccess(BaseModel):
+    access: Optional[List[str]] = []
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[LastMessage] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    pinned_message_id: Optional[str] = None
+    abs_object: Optional[Dict] = None
+    is_blocked: Optional[bool] = None
+    last_message_id: Optional[str] = None
+    last_deleted_mid: Optional[str] = None
+    slow_mode_duration: Optional[int] = None
+    group_my_last_send_time: Optional[int] = None
+    pinned_message_ids: Optional[List[str]] = []
+
+
+class ChatUpdate(BaseModel):
+    object_guid: Optional[str] = None
+    action: Optional[str] = None
+    chat: Optional[ChatAccess] = None
+    updated_parameters: Optional[List[str]] = None
+    timestamp: Optional[str] = None
+    type: Optional[str] = None
+
+
+class LeaveGroup(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class Group(BaseModel):
+    group_guid: Optional[str] = None
+    group_title: Optional[str] = None
+    count_members: Optional[int] = None
+    is_deleted: Optional[bool] = None
+    is_verified: Optional[bool] = None
+    slow_mode: Optional[int] = None
+    chat_history_for_new_members: Optional[str] = None
+    event_messages: Optional[bool] = None
+    chat_reaction_setting: Optional[Union[str, Dict]] = None
+
+
+class Chat(BaseModel):
+    object_guid: Optional[str] = None
+    action: Optional[str] = None
+    access: Optional[List[str]] = None
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[Dict] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    abs_object: Optional[Dict] = None
+    is_blocked: Optional[bool] = None
+    last_message_id: Optional[str] = None
+    last_deleted_mid: Optional[str] = None
+    slow_mode_duration: Optional[int] = None
+
+
+class MessageUpdate(BaseModel):
+    message_id: Optional[str] = None
+    action: Optional[str] = None
+    message: Optional[Dict] = None
+    updated_parameters: Optional[List[str]] = None
+    timestamp: Optional[str] = None
+    prev_message_id: Optional[str] = None
+    object_guid: Optional[str] = None
+    type: Optional[str] = None
+    state: Optional[str] = None
+
+
+class JoinGroup(BaseModel):
+    group: Optional[Group] = None
+    is_valid: Optional[bool] = None
+    chat_update: Optional[Chat] = None
+    message_update: Optional[MessageUpdate] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class AddGroup(BaseModel):
+    group: Optional[Group] = None
+    chat_update: Optional[Chat] = None
+    message_update: Optional[MessageUpdate] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class RemoveGroup(BaseModel):
+    chat_update: Optional[Chat] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetGroupInfo(BaseModel):
+    group: Optional[Group] = None
+    chat: Optional[Chat] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+    message_update: Optional[MessageUpdate] = None
+
+
+class GroupLink(BaseModel):
+    join_link: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class EditGroupInfo(BaseModel):
+    group: Optional[Group] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class OnlineTime(BaseModel):
+    type: Optional[str] = None
+    approximate_period: Optional[str] = None
+
+
+class InChatMemberList(BaseModel):
+    member_type: Optional[str] = None
+    member_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+    promoted_by_object_guid: Optional[str] = None
+    promoted_by_object_type: Optional[str] = None
+    join_type: Optional[str] = None
+    online_time: Optional[OnlineTime] = None
+
+
+class InChatMember(BaseModel):
+    in_chat_member: Optional[InChatMemberList] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class BanGroupMember(BaseModel):
+    group: Optional[Group] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[Dict] = None
+
+
+class AvatarThumbnail(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+
+
+class AddedInChatMember(BaseModel):
+    member_type: Optional[str] = None
+    member_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+    last_online: Optional[int] = None
+    join_type: Optional[str] = None
+    username: Optional[str] = None
+    online_time: Optional[OnlineTime] = None
+
+
+class AddGroupMembers(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    message_update: Optional[MessageUpdate] = None
+    added_in_chat_members: Optional[List[AddedInChatMember]] = None
+    timestamp: Optional[str] = None
+    group: Optional[Group] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class InChatGroupMember(BaseModel):
+    member_type: Optional[str] = None
+    member_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+    last_online: Optional[int] = None
+    join_type: Optional[str] = None
+    online_time: Optional[OnlineTime] = None
+    promoted_by_object_guid: Optional[str] = None
+    promoted_by_object_type: Optional[str] = None
+    removed_by_object_guid: Optional[str] = None
+    removed_by_object_type: Optional[str] = None
+
+
+class GetAllGroupMembers(BaseModel):
+    in_chat_members: Optional[List[InChatGroupMember]] = None
+    next_start_id: Optional[str] = None
+    has_continue: Optional[bool] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetGroupAdminMembers(BaseModel):
+    in_chat_members: Optional[List[InChatGroupMember]] = None
+    next_start_id: Optional[str] = None
+    has_continue: Optional[bool] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetGroupMentionList(BaseModel):
+    in_chat_members: Optional[List[InChatGroupMember]] = None
+    next_start_id: Optional[str] = None
+    has_continue: Optional[bool] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetGroupDefaultAccess(BaseModel):
+    access_list: Optional[List] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class OnlineTime(BaseModel):
+    type: Optional[str] = None
+    approximate_period: Optional[str] = None
+
+
+class TopParticipants(BaseModel):
+    member_type: Optional[str] = None
+    member_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+    username: Optional[str] = None
+    online_time: Optional[OnlineTime] = None
+
+
+class GroupPreviewByJoinLink(BaseModel):
+    is_valid: Optional[bool] = None
+    group: Optional[Group] = None
+    has_joined: Optional[bool] = None
+    top_participants: Optional[List[TopParticipants]] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class DeleteNoAccessGroupChat(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    status: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetGroupAdminAccessList(BaseModel):
+    access_list: Optional[List] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetBannedGroupMembers(BaseModel):
+    in_chat_members: Optional[List[InChatGroupMember]] = []
+    next_start_id: Optional[str] = None
+    has_continue: Optional[bool] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/models/messages.py` & `aiorubika-1.0.0/aiorubika/types/models/messages.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,827 +1,852 @@
-from .. import methods
-from .. import thumbnail
-from base64 import b64decode
-from pydantic import BaseModel
-from typing import Optional, List
-
-class FileInline(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-    file_name: Optional[str] = None
-    thumb_inline: Optional[str] = None
-    music_performer: Optional[str] = None
-    width: Optional[int] = None
-    height: Optional[int] = None
-    time: Optional[int] = None
-    size: Optional[int] = None
-    type: Optional[str] = None
-
-class ForwardedFrom(BaseModel):
-    type_from: Optional[str] = None
-    message_id: Optional[str] = None
-    object_guid: Optional[str] = None
-
-class PollOption(BaseModel):
-    options: Optional[List[str]] = []
-    poll_status: Optional[dict] = None
-    is_anonymous: Optional[bool] = None
-    type: Optional[str] = None
-    allows_multiple_answers: Optional[bool] = None
-
-class Poll(BaseModel):
-    poll_id: Optional[str] = None
-    question: Optional[str] = None
-    options: Optional[List[str]] = None
-    poll_status: Optional[dict] = None
-    is_anonymous: Optional[bool] = None
-    type: Optional[str] = None
-    allows_multiple_answers: Optional[bool] = None
-
-class AvatarThumbnail(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-
-class MessageData(BaseModel):
-    message_id: Optional[str] = None
-    text: Optional[str] = None
-    file_inline: Optional[FileInline] = None
-    time: Optional[str] = None
-    is_edited: Optional[bool] = None
-    type: Optional[str] = None
-    author_type: Optional[str] = None
-    author_object_guid: Optional[str] = None
-    forwarded_from: Optional[ForwardedFrom] = None
-    poll: Optional[Poll] = None
-
-class AbsObject(BaseModel):
-    object_guid: Optional[str] = None
-    type: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    avatar_thumbnail: Optional[AvatarThumbnail] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-
-class Message(BaseModel):
-    message_id: Optional[str] = None
-    text: Optional[str] = None
-    file_inline: Optional[FileInline] = None
-    time: Optional[str] = None
-    is_edited: Optional[bool] = None
-    type: Optional[str] = None
-    author_type: Optional[str] = None
-    author_object_guid: Optional[str] = None
-    forwarded_from: Optional[ForwardedFrom] = None
-    poll: Optional[Poll] = None
-    object_guid: Optional[str] = None
-    message: Optional[MessageData] = None
-    abs_object: Optional[AbsObject] = None
-    last_seen_peer_mid: Optional[int] = None
-
-class MessageUpdate(BaseModel):
-    message_id: Optional[str] = None
-    action: Optional[str] = None
-    message: Optional[Message] = None
-    updated_parameters: Optional[List] = None
-    timestamp: Optional[str] = None
-    prev_message_id: Optional[str] = None
-    object_guid: Optional[str] = None
-    type: Optional[str] = None
-    state: Optional[str] = None
-
-class LastMessage(BaseModel):
-    message_id: Optional[str] = None
-    type: Optional[str] = None
-    text: Optional[str] = None
-    author_object_guid: Optional[str] = None
-    is_mine: Optional[bool] = None
-    author_title: Optional[str] = None
-    author_type: Optional[str] = None
-
-class Chat(BaseModel):
-    time_string: Optional[str] = None
-    last_message: Optional[LastMessage] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[int] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    last_message_id: Optional[str] = None
-
-class ChatUpdate(BaseModel):
-    object_guid: Optional[str] = None
-    action: Optional[str] = None
-    chat: Optional[Chat] = None
-    updated_parameters: Optional[List] = None
-    timestamp: Optional[str] = None
-    type: Optional[str] = None
-
-class SendMessage(BaseModel):
-    message_update: Optional[MessageUpdate] = None
-    status: Optional[str] = None
-    chat_update: Optional[ChatUpdate] = None
-
-    @classmethod
-    async def set_shared_data(cls, client, message):
-        cls._client = client
-        cls._message = message
-
-    @classmethod
-    async def pin(cls,
-                  object_guid: str = None,
-                  message_id: str = None,
-                  action: str = methods.messages.Pin, *args, **kwargs):
-        """_pin_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-            message_id (str, optional):
-                _custom message id_. Defaults to update.message_id.
-            action (bool, optional):
-                _pin or unpin_. Defaults to methods.messages.Pin. (
-                    methods.messages.Pin,
-                    methods.messages.Unpin
-                )
-        Returns:
-            BaseResults: result
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_id is None:
-            message_id = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.SetPinMessage(
-                object_guid=object_guid,
-                message_id=message_id,
-                action=action))
-
-    @classmethod
-    async def edit(cls,
-                   text: str,
-                   object_guid: str = None,
-                   message_id: str = None, *args, **kwargs):
-        """_edit_
-        Args:
-            text (str):
-                _message text_
-            object_guid (str, optional):
-                _custom objec guid_. Defaults to update.object_guid.
-            message_id (str, optional):
-                _custom message id_. Defaults to update.message_id.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_id is None:
-            message_id = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.EditMessage(
-                object_guid=object_guid,
-                message_id=message_id,
-                text=text))
-    
-    @classmethod
-    async def copy(cls,
-                   to_object_guid: str,
-                   from_object_guid: str = None, message_ids=None, *args, **kwargs):
-        """_copy_
-        Args:
-            to_object_guid (str):
-                _to object guid_.
-            from_object_guid (str, optional):
-                _from object guid_. Defaults to update.object_guid.
-            message_ids (typing.Union[str, int, typing.List[str]], optional):
-                _message ids_. Defaults to update.message_id.
-        """
-            
-        if from_object_guid is None:
-            from_object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-        
-        result = await cls.get_messages(from_object_guid, message_ids)
-        messages = []
-        if result.messages:
-            for message in result.messages:
-                
-                try:
-                    file_inline = message.file_inline
-                    kwargs.update(file_inline.to_dict())
-
-                except AttributeError:
-                    file_inline = None
-
-                try:
-                    thumb = thumbnail.Thumbnail(
-                        b64decode(message.thumb_inline), *args, **kwargs)
-                    
-                except AttributeError:
-                    thumb = kwargs.get('thumb', True)
-                                
-                try:
-                    message = message.sticker
-                
-                except AttributeError:
-                    message = message.raw_text
-                
-                if file_inline is not None:
-                    if file_inline.type not in [methods.messages.Gif,
-                                                methods.messages.Sticker]:
-                        file_inline = await cls.download(file_inline)
-                        messages.append(await cls._client.send_message(
-                            thumb=thumb,
-                            message=message,
-                            file_inline=file_inline,
-                            object_guid=to_object_guid, *args, **kwargs))
-                        continue
-
-                messages.append(await cls._client.send_message(
-                    message=message,
-                    object_guid=to_object_guid,
-                    file_inline=file_inline, *args, **kwargs))
-    
-        return {'status': 'OK', 'messages': messages}
-
-    @classmethod
-    async def seen(cls, seen_list: dict = None, *args, **kwargs):
-        """_seen_
-        Args:
-            seen_list (dict, optional):
-                _description_. Defaults t
-                    {update.object_guid: update.message_id}
-        """
-
-        if seen_list is None:
-            seen_list = {cls._message.message_update.object_guid: cls._message.message_update.message_id}
-        return await cls._client(methods.chats.SeenChats(seen_list=seen_list))
-
-    @classmethod
-    async def reply(cls,
-                    message=None,
-                    object_guid: str = None,
-                    reply_to_message_id: str = None,
-                    file_inline: str = None, *args, **kwargs):
-        """_reply_
-        Args:
-            message (Any, optional):
-                _message or cation or sticker_ . Defaults to None.
-            object_guid (str):
-                _object guid_ . Defaults to update.object_guid
-            reply_to_message_id (str, optional):
-                _reply to message id_. Defaults to None.
-            file_inline (typing.Union[pathlib.Path, bytes], optional):
-                _file_. Defaults to None.
-            is_gif (bool, optional):
-                _is it a gif file or not_. Defaults to None.
-            is_image (bool, optional):
-                _is it a image file or not_. Defaults to None.
-            is_voice (bool, optional):
-                _is it a voice file or not_. Defaults to None.
-            is_music (bool, optional):
-                _is it a music file or not_. Defaults to None.
-            is_video (bool, optional):
-                _is it a video file or not_. Defaults to None.
-            thumb (bool, optional):
-                if value is "True",
-                the lib will try to build the thumb ( require cv2 )
-                if value is thumbnail.Thumbnail, to set custom
-                Defaults to True.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_id is None:
-            message_id = cls._message.message_update.message_id
-
-        return await cls._client.send_message(
-            message=message,
-            object_guid=object_guid,
-            file_inline=file_inline,
-            reply_to_message_id=reply_to_message_id, *args, **kwargs)
-
-    @classmethod
-    async def forwards(cls,
-                       to_object_guid: str,
-                       from_object_guid: str = None,
-                       message_ids=None, *args, **kwargs):
-        """_forwards_
-        Args:
-            to_object_guid (str):
-                _to object guid_.
-            from_object_guid (str, optional):
-                _from object guid_. Defaults to update.object_guid.
-            message_ids (typing.Union[str, int, typing.List[str]], optional):
-                _message ids_. Defaults to update.message_id.
-        """
-
-        if from_object_guid is None:
-            from_object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.ForwardMessages(
-                from_object_guid=from_object_guid,
-                to_object_guid=to_object_guid,
-                message_ids=message_ids))
-
-    @classmethod
-    async def download(cls, file_inline=None, file=None, *args, **kwargs):
-        return await cls._client.download_file_inline(
-            file_inline or cls._message.file_inline,
-            file=file, *args, **kwargs)
-
-    @classmethod
-    async def get_author(cls, author_guid: str = None, *args, **kwargs):
-        """_get user or author information_
-        Args:
-            author_guid (str, optional):
-                _custom author guid_. Defaults to update.author_guid
-        """
-
-        if author_guid is None:
-            author_guid = cls._message.message_update.message.author_object_guid
-
-        return await cls.get_object(object_guid=author_guid, *args, **kwargs)
-
-    @classmethod
-    async def get_object(cls, object_guid: str = None, *args, **kwargs):
-        """_get object information_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-
-        if cls.guid_type(object_guid) == 'User':
-            return await cls._client(
-                methods.users.GetUserInfo(
-                    user_guid=object_guid))
-
-        elif cls.guid_type(object_guid) == 'Group':
-            return await cls._client(
-                methods.groups.GetGroupInfo(
-                    object_guid=object_guid))
-
-        elif cls.guid_type(object_guid) == 'Channel':
-            return await cls._client(
-                methods.channels.GetChannelInfo(
-                    object_guid=object_guid))
-
-    @classmethod
-    async def get_message(cls,
-                           object_guid: str = None,
-                           message_ids=None, *args, **kwargs):
-        """_get messages_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-            message_ids (str, int, typing.List[str]], optional):
-                _message ids_. Defaults to update.message_id.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.GetMessagesByID(
-                object_guid=object_guid, message_ids=message_ids))
-
-    @classmethod
-    async def delete(cls,
-                              object_guid: str = None,
-                              message_ids=None, *args, **kwargs):
-        """_delete messages_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-            message_ids (str, list, optional):
-                _custom message ids_. Defaults to update.message_id.
-            type(str, optional):
-                the message should be deleted for everyone or not.
-                Defaults to methods.messages.Global (
-                    methods.messages.Local,
-                    methods.messages.Global
-                )
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.DeleteMessages(
-                object_guid=object_guid,
-                message_ids=message_ids, *args, **kwargs))
-
-class EditMessage(BaseModel):
-    message_update: Optional[MessageUpdate] = None
-    chat_update: Optional[ChatUpdate] = None
-    
-    @classmethod
-    async def set_shared_data(cls, client, message):
-        cls._client = client
-        cls._message = message
-
-    @classmethod
-    async def pin(cls,
-                  object_guid: str = None,
-                  message_id: str = None,
-                  action: str = methods.messages.Pin, *args, **kwargs):
-        """_pin_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-            message_id (str, optional):
-                _custom message id_. Defaults to update.message_id.
-            action (bool, optional):
-                _pin or unpin_. Defaults to methods.messages.Pin. (
-                    methods.messages.Pin,
-                    methods.messages.Unpin
-                )
-        Returns:
-            BaseResults: result
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_id is None:
-            message_id = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.SetPinMessage(
-                object_guid=object_guid,
-                message_id=message_id,
-                action=action))
-
-    @classmethod
-    async def edit(cls,
-                   text: str,
-                   object_guid: str = None,
-                   message_id: str = None, *args, **kwargs):
-        """_edit_
-        Args:
-            text (str):
-                _message text_
-            object_guid (str, optional):
-                _custom objec guid_. Defaults to update.object_guid.
-            message_id (str, optional):
-                _custom message id_. Defaults to update.message_id.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_id is None:
-            message_id = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.EditMessage(
-                object_guid=object_guid,
-                message_id=message_id,
-                text=text))
-    
-    @classmethod
-    async def copy(cls,
-                   to_object_guid: str,
-                   from_object_guid: str = None, message_ids=None, *args, **kwargs):
-        """_copy_
-        Args:
-            to_object_guid (str):
-                _to object guid_.
-            from_object_guid (str, optional):
-                _from object guid_. Defaults to update.object_guid.
-            message_ids (typing.Union[str, int, typing.List[str]], optional):
-                _message ids_. Defaults to update.message_id.
-        """
-            
-        if from_object_guid is None:
-            from_object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-        
-        result = await cls.get_messages(from_object_guid, message_ids)
-        messages = []
-        if result.messages:
-            for message in result.messages:
-                
-                try:
-                    file_inline = message.file_inline
-                    kwargs.update(file_inline.to_dict())
-
-                except AttributeError:
-                    file_inline = None
-
-                try:
-                    thumb = thumbnail.Thumbnail(
-                        b64decode(message.thumb_inline), *args, **kwargs)
-                    
-                except AttributeError:
-                    thumb = kwargs.get('thumb', True)
-                                
-                try:
-                    message = message.sticker
-                
-                except AttributeError:
-                    message = message.raw_text
-                
-                if file_inline is not None:
-                    if file_inline.type not in [methods.messages.Gif,
-                                                methods.messages.Sticker]:
-                        file_inline = await cls.download(file_inline)
-                        messages.append(await cls._client.send_message(
-                            thumb=thumb,
-                            message=message,
-                            file_inline=file_inline,
-                            object_guid=to_object_guid, *args, **kwargs))
-                        continue
-
-                messages.append(await cls._client.send_message(
-                    message=message,
-                    object_guid=to_object_guid,
-                    file_inline=file_inline, *args, **kwargs))
-    
-        return {'status': 'OK', 'messages': messages}
-
-    @classmethod
-    async def seen(cls, seen_list: dict = None, *args, **kwargs):
-        """_seen_
-        Args:
-            seen_list (dict, optional):
-                _description_. Defaults t
-                    {update.object_guid: update.message_id}
-        """
-
-        if seen_list is None:
-            seen_list = {cls._message.message_update.object_guid: cls._message.message_update.message_id}
-        return await cls._client(methods.chats.SeenChats(seen_list=seen_list))
-
-    @classmethod
-    async def reply(cls,
-                    message=None,
-                    object_guid: str = None,
-                    reply_to_message_id: str = None,
-                    file_inline: str = None, *args, **kwargs):
-        """_reply_
-        Args:
-            message (Any, optional):
-                _message or cation or sticker_ . Defaults to None.
-            object_guid (str):
-                _object guid_ . Defaults to update.object_guid
-            reply_to_message_id (str, optional):
-                _reply to message id_. Defaults to None.
-            file_inline (typing.Union[pathlib.Path, bytes], optional):
-                _file_. Defaults to None.
-            is_gif (bool, optional):
-                _is it a gif file or not_. Defaults to None.
-            is_image (bool, optional):
-                _is it a image file or not_. Defaults to None.
-            is_voice (bool, optional):
-                _is it a voice file or not_. Defaults to None.
-            is_music (bool, optional):
-                _is it a music file or not_. Defaults to None.
-            is_video (bool, optional):
-                _is it a video file or not_. Defaults to None.
-            thumb (bool, optional):
-                if value is "True",
-                the lib will try to build the thumb ( require cv2 )
-                if value is thumbnail.Thumbnail, to set custom
-                Defaults to True.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_id is None:
-            message_id = cls._message.message_update.message_id
-
-        return await cls._client.send_message(
-            message=message,
-            object_guid=object_guid,
-            file_inline=file_inline,
-            reply_to_message_id=reply_to_message_id, *args, **kwargs)
-
-    @classmethod
-    async def forwards(cls,
-                       to_object_guid: str,
-                       from_object_guid: str = None,
-                       message_ids=None, *args, **kwargs):
-        """_forwards_
-        Args:
-            to_object_guid (str):
-                _to object guid_.
-            from_object_guid (str, optional):
-                _from object guid_. Defaults to update.object_guid.
-            message_ids (typing.Union[str, int, typing.List[str]], optional):
-                _message ids_. Defaults to update.message_id.
-        """
-
-        if from_object_guid is None:
-            from_object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.ForwardMessages(
-                from_object_guid=from_object_guid,
-                to_object_guid=to_object_guid,
-                message_ids=message_ids))
-
-    @classmethod
-    async def download(cls, file_inline=None, file=None, *args, **kwargs):
-        return await cls._client.download_file_inline(
-            file_inline or cls._message.file_inline,
-            file=file, *args, **kwargs)
-
-    @classmethod
-    async def get_author(cls, author_guid: str = None, *args, **kwargs):
-        """_get user or author information_
-        Args:
-            author_guid (str, optional):
-                _custom author guid_. Defaults to update.author_guid
-        """
-
-        if author_guid is None:
-            author_guid = cls._message.message_update.message.author_object_guid
-
-        return await cls.get_object(object_guid=author_guid, *args, **kwargs)
-
-    @classmethod
-    async def get_object(cls, object_guid: str = None, *args, **kwargs):
-        """_get object information_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-
-        if cls.guid_type(object_guid) == 'User':
-            return await cls._client(
-                methods.users.GetUserInfo(
-                    user_guid=object_guid))
-
-        elif cls.guid_type(object_guid) == 'Group':
-            return await cls._client(
-                methods.groups.GetGroupInfo(
-                    object_guid=object_guid))
-
-        elif cls.guid_type(object_guid) == 'Channel':
-            return await cls._client(
-                methods.channels.GetChannelInfo(
-                    object_guid=object_guid))
-
-    @classmethod
-    async def get_message(cls,
-                           object_guid: str = None,
-                           message_ids=None, *args, **kwargs):
-        """_get messages_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-            message_ids (str, int, typing.List[str]], optional):
-                _message ids_. Defaults to update.message_id.
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.GetMessagesByID(
-                object_guid=object_guid, message_ids=message_ids))
-
-    @classmethod
-    async def delete(cls,
-                              object_guid: str = None,
-                              message_ids=None, *args, **kwargs):
-        """_delete messages_
-        Args:
-            object_guid (str, optional):
-                _custom object guid_. Defaults to update.object_guid.
-            message_ids (str, list, optional):
-                _custom message ids_. Defaults to update.message_id.
-            type(str, optional):
-                the message should be deleted for everyone or not.
-                Defaults to methods.messages.Global (
-                    methods.messages.Local,
-                    methods.messages.Global
-                )
-        """
-
-        if object_guid is None:
-            object_guid = cls._message.message_update.object_guid
-
-        if message_ids is None:
-            message_ids = cls._message.message_update.message_id
-
-        return await cls._client(
-            methods.messages.DeleteMessages(
-                object_guid=object_guid,
-                message_ids=message_ids, *args, **kwargs))
-
-class DeleteMessages(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    message_updates: Optional[List[MessageUpdate]] = []
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class RequestSendFile(BaseModel):
-    id: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_send: Optional[str] = None
-    upload_url: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class ForwardMessages(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    message_updates: Optional[List[MessageUpdate]] = []
-    status: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class PollStatus(BaseModel):
-    state: Optional[str] = None
-    selection_index: Optional[int] = None
-    percent_vote_options: Optional[List[int]] = None
-    total_vote: Optional[int] = None
-    show_total_votes: Optional[bool] = None
-
-class VotePoll(BaseModel):
-    poll_status: Optional[PollStatus] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class SetPinMessage(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    status: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetMessagesUpdates(BaseModel):
-    updated_messages: Optional[List[MessageUpdate]] = []
-    new_state: Optional[int] = None
-    status: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class SearchGlobalMessages(BaseModel):
-    messages: Optional[List[Message]] = []
-    next_start_id: Optional[str] = None
-    has_continue: Optional[bool] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetMessagesByID(BaseModel):
-    messages: Optional[List[Message]] = []
-    timestamp: Optional[int] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class GetMessagesInterval(BaseModel):
-    messages: Optional[List[Message]] = []
-    state: Optional[str] = None
-    new_has_continue: Optional[bool] = None
-    old_has_continue: Optional[bool] = None
-    new_min_id: Optional[int] = None
-    old_max_id: Optional[int] = None
-    timestamp: Optional[str] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class Reactions(BaseModel):
-    user_guids: Optional[List] = []
-    reaction_count: Optional[int] = None
-    emoji_char: Optional[str] = None
-    reaction_id: Optional[int] = None
-    is_selected: Optional[bool] = None
-
-class Reacion(BaseModel):
-    reactions: Optional[List[Reactions]] = []
+from typing import Optional, List
+from pydantic import BaseModel
+from base64 import b64decode
+
+from .. import methods
+from .. import thumbnail
+
+
+class FileInline(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+    file_name: Optional[str] = None
+    thumb_inline: Optional[str] = None
+    music_performer: Optional[str] = None
+    width: Optional[int] = None
+    height: Optional[int] = None
+    time: Optional[int] = None
+    size: Optional[int] = None
+    type: Optional[str] = None
+
+
+class ForwardedFrom(BaseModel):
+    type_from: Optional[str] = None
+    message_id: Optional[str] = None
+    object_guid: Optional[str] = None
+
+
+class PollOption(BaseModel):
+    options: Optional[List[str]] = []
+    poll_status: Optional[dict] = None
+    is_anonymous: Optional[bool] = None
+    type: Optional[str] = None
+    allows_multiple_answers: Optional[bool] = None
+
+
+class Poll(BaseModel):
+    poll_id: Optional[str] = None
+    question: Optional[str] = None
+    options: Optional[List[str]] = None
+    poll_status: Optional[dict] = None
+    is_anonymous: Optional[bool] = None
+    type: Optional[str] = None
+    allows_multiple_answers: Optional[bool] = None
+
+
+class AvatarThumbnail(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+
+
+class MessageData(BaseModel):
+    message_id: Optional[str] = None
+    text: Optional[str] = None
+    file_inline: Optional[FileInline] = None
+    time: Optional[str] = None
+    is_edited: Optional[bool] = None
+    type: Optional[str] = None
+    author_type: Optional[str] = None
+    author_object_guid: Optional[str] = None
+    forwarded_from: Optional[ForwardedFrom] = None
+    poll: Optional[Poll] = None
+
+
+class AbsObject(BaseModel):
+    object_guid: Optional[str] = None
+    type: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    avatar_thumbnail: Optional[AvatarThumbnail] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+
+
+class Message(BaseModel):
+    message_id: Optional[str] = None
+    text: Optional[str] = None
+    file_inline: Optional[FileInline] = None
+    time: Optional[str] = None
+    is_edited: Optional[bool] = None
+    type: Optional[str] = None
+    author_type: Optional[str] = None
+    author_object_guid: Optional[str] = None
+    forwarded_from: Optional[ForwardedFrom] = None
+    poll: Optional[Poll] = None
+    object_guid: Optional[str] = None
+    message: Optional[MessageData] = None
+    abs_object: Optional[AbsObject] = None
+    last_seen_peer_mid: Optional[int] = None
+
+
+class MessageUpdate(BaseModel):
+    message_id: Optional[str] = None
+    action: Optional[str] = None
+    message: Optional[Message] = None
+    updated_parameters: Optional[List] = None
+    timestamp: Optional[str] = None
+    prev_message_id: Optional[str] = None
+    object_guid: Optional[str] = None
+    type: Optional[str] = None
+    state: Optional[str] = None
+
+
+class LastMessage(BaseModel):
+    message_id: Optional[str] = None
+    type: Optional[str] = None
+    text: Optional[str] = None
+    author_object_guid: Optional[str] = None
+    is_mine: Optional[bool] = None
+    author_title: Optional[str] = None
+    author_type: Optional[str] = None
+
+
+class Chat(BaseModel):
+    time_string: Optional[str] = None
+    last_message: Optional[LastMessage] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[int] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    last_message_id: Optional[str] = None
+
+
+class ChatUpdate(BaseModel):
+    object_guid: Optional[str] = None
+    action: Optional[str] = None
+    chat: Optional[Chat] = None
+    updated_parameters: Optional[List] = None
+    timestamp: Optional[str] = None
+    type: Optional[str] = None
+
+
+class SendMessage(BaseModel):
+    message_update: Optional[MessageUpdate] = None
+    status: Optional[str] = None
+    chat_update: Optional[ChatUpdate] = None
+
+    @classmethod
+    async def set_shared_data(cls, client, message):
+        cls._client = client
+        cls._message = message
+
+    @classmethod
+    async def pin(cls,
+                  object_guid: str = None,
+                  message_id: str = None,
+                  action: str = methods.messages.Pin, *args, **kwargs):
+        """_pin_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+            message_id (str, optional):
+                _custom message id_. Defaults to update.message_id.
+            action (bool, optional):
+                _pin or unpin_. Defaults to methods.messages.Pin. (
+                    methods.messages.Pin,
+                    methods.messages.Unpin
+                )
+        Returns:
+            BaseResults: result
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_id is None:
+            message_id = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.SetPinMessage(
+                object_guid=object_guid,
+                message_id=message_id,
+                action=action))
+
+    @classmethod
+    async def edit(cls,
+                   text: str,
+                   object_guid: str = None,
+                   message_id: str = None, *args, **kwargs):
+        """_edit_
+        Args:
+            text (str):
+                _message text_
+            object_guid (str, optional):
+                _custom objec guid_. Defaults to update.object_guid.
+            message_id (str, optional):
+                _custom message id_. Defaults to update.message_id.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_id is None:
+            message_id = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.EditMessage(
+                object_guid=object_guid,
+                message_id=message_id,
+                text=text))
+
+    @classmethod
+    async def copy(cls,
+                   to_object_guid: str,
+                   from_object_guid: str = None, message_ids=None, *args, **kwargs):
+        """_copy_
+        Args:
+            to_object_guid (str):
+                _to object guid_.
+            from_object_guid (str, optional):
+                _from object guid_. Defaults to update.object_guid.
+            message_ids (typing.Union[str, int, typing.List[str]], optional):
+                _message ids_. Defaults to update.message_id.
+        """
+
+        if from_object_guid is None:
+            from_object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        result = await cls.get_messages(from_object_guid, message_ids)
+        messages = []
+        if result.messages:
+            for message in result.messages:
+
+                try:
+                    file_inline = message.file_inline
+                    kwargs.update(file_inline.to_dict())
+
+                except AttributeError:
+                    file_inline = None
+
+                try:
+                    thumb = thumbnail.Thumbnail(
+                        b64decode(message.thumb_inline), *args, **kwargs)
+
+                except AttributeError:
+                    thumb = kwargs.get('thumb', True)
+
+                try:
+                    message = message.sticker
+
+                except AttributeError:
+                    message = message.raw_text
+
+                if file_inline is not None:
+                    if file_inline.type not in [methods.messages.Gif,
+                                                methods.messages.Sticker]:
+                        file_inline = await cls.download(file_inline)
+                        messages.append(await cls._client.send_message(
+                            thumb=thumb,
+                            message=message,
+                            file_inline=file_inline,
+                            object_guid=to_object_guid, *args, **kwargs))
+                        continue
+
+                messages.append(await cls._client.send_message(
+                    message=message,
+                    object_guid=to_object_guid,
+                    file_inline=file_inline, *args, **kwargs))
+
+        return {'status': 'OK', 'messages': messages}
+
+    @classmethod
+    async def seen(cls, seen_list: dict = None, *args, **kwargs):
+        """_seen_
+        Args:
+            seen_list (dict, optional):
+                _description_. Defaults t
+                    {update.object_guid: update.message_id}
+        """
+
+        if seen_list is None:
+            seen_list = {cls._message.message_update.object_guid: cls._message.message_update.message_id}
+        return await cls._client(methods.chats.SeenChats(seen_list=seen_list))
+
+    @classmethod
+    async def reply(cls,
+                    message=None,
+                    object_guid: str = None,
+                    reply_to_message_id: str = None,
+                    file_inline: str = None, *args, **kwargs):
+        """_reply_
+        Args:
+            message (Any, optional):
+                _message or cation or sticker_ . Defaults to None.
+            object_guid (str):
+                _object guid_ . Defaults to update.object_guid
+            reply_to_message_id (str, optional):
+                _reply to message id_. Defaults to None.
+            file_inline (typing.Union[pathlib.Path, bytes], optional):
+                _file_. Defaults to None.
+            is_gif (bool, optional):
+                _is it a gif file or not_. Defaults to None.
+            is_image (bool, optional):
+                _is it a image file or not_. Defaults to None.
+            is_voice (bool, optional):
+                _is it a voice file or not_. Defaults to None.
+            is_music (bool, optional):
+                _is it a music file or not_. Defaults to None.
+            is_video (bool, optional):
+                _is it a video file or not_. Defaults to None.
+            thumb (bool, optional):
+                if value is "True",
+                the lib will try to build the thumb ( require cv2 )
+                if value is thumbnail.Thumbnail, to set custom
+                Defaults to True.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_id is None:
+            message_id = cls._message.message_update.message_id
+
+        return await cls._client.send_message(
+            message=message,
+            object_guid=object_guid,
+            file_inline=file_inline,
+            reply_to_message_id=reply_to_message_id, *args, **kwargs)
+
+    @classmethod
+    async def forwards(cls,
+                       to_object_guid: str,
+                       from_object_guid: str = None,
+                       message_ids=None, *args, **kwargs):
+        """_forwards_
+        Args:
+            to_object_guid (str):
+                _to object guid_.
+            from_object_guid (str, optional):
+                _from object guid_. Defaults to update.object_guid.
+            message_ids (typing.Union[str, int, typing.List[str]], optional):
+                _message ids_. Defaults to update.message_id.
+        """
+
+        if from_object_guid is None:
+            from_object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.ForwardMessages(
+                from_object_guid=from_object_guid,
+                to_object_guid=to_object_guid,
+                message_ids=message_ids))
+
+    @classmethod
+    async def download(cls, file_inline=None, file=None, *args, **kwargs):
+        return await cls._client.download_file_inline(
+            file_inline or cls._message.file_inline,
+            file=file, *args, **kwargs)
+
+    @classmethod
+    async def get_author(cls, author_guid: str = None, *args, **kwargs):
+        """_get user or author information_
+        Args:
+            author_guid (str, optional):
+                _custom author guid_. Defaults to update.author_guid
+        """
+
+        if author_guid is None:
+            author_guid = cls._message.message_update.message.author_object_guid
+
+        return await cls.get_object(object_guid=author_guid, *args, **kwargs)
+
+    @classmethod
+    async def get_object(cls, object_guid: str = None, *args, **kwargs):
+        """_get object information_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if cls.guid_type(object_guid) == 'User':
+            return await cls._client(
+                methods.users.GetUserInfo(
+                    user_guid=object_guid))
+
+        elif cls.guid_type(object_guid) == 'Group':
+            return await cls._client(
+                methods.groups.GetGroupInfo(
+                    object_guid=object_guid))
+
+        elif cls.guid_type(object_guid) == 'Channel':
+            return await cls._client(
+                methods.channels.GetChannelInfo(
+                    object_guid=object_guid))
+
+    @classmethod
+    async def get_message(cls,
+                          object_guid: str = None,
+                          message_ids=None, *args, **kwargs):
+        """_get messages_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+            message_ids (str, int, typing.List[str]], optional):
+                _message ids_. Defaults to update.message_id.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.GetMessagesByID(
+                object_guid=object_guid, message_ids=message_ids))
+
+    @classmethod
+    async def delete(cls,
+                     object_guid: str = None,
+                     message_ids=None, *args, **kwargs):
+        """_delete messages_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+            message_ids (str, list, optional):
+                _custom message ids_. Defaults to update.message_id.
+            type(str, optional):
+                the message should be deleted for everyone or not.
+                Defaults to methods.messages.Global (
+                    methods.messages.Local,
+                    methods.messages.Global
+                )
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.DeleteMessages(
+                object_guid=object_guid,
+                message_ids=message_ids, *args, **kwargs))
+
+
+class EditMessage(BaseModel):
+    message_update: Optional[MessageUpdate] = None
+    chat_update: Optional[ChatUpdate] = None
+
+    @classmethod
+    async def set_shared_data(cls, client, message):
+        cls._client = client
+        cls._message = message
+
+    @classmethod
+    async def pin(cls,
+                  object_guid: str = None,
+                  message_id: str = None,
+                  action: str = methods.messages.Pin, *args, **kwargs):
+        """_pin_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+            message_id (str, optional):
+                _custom message id_. Defaults to update.message_id.
+            action (bool, optional):
+                _pin or unpin_. Defaults to methods.messages.Pin. (
+                    methods.messages.Pin,
+                    methods.messages.Unpin
+                )
+        Returns:
+            BaseResults: result
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_id is None:
+            message_id = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.SetPinMessage(
+                object_guid=object_guid,
+                message_id=message_id,
+                action=action))
+
+    @classmethod
+    async def edit(cls,
+                   text: str,
+                   object_guid: str = None,
+                   message_id: str = None, *args, **kwargs):
+        """_edit_
+        Args:
+            text (str):
+                _message text_
+            object_guid (str, optional):
+                _custom objec guid_. Defaults to update.object_guid.
+            message_id (str, optional):
+                _custom message id_. Defaults to update.message_id.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_id is None:
+            message_id = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.EditMessage(
+                object_guid=object_guid,
+                message_id=message_id,
+                text=text))
+
+    @classmethod
+    async def copy(cls,
+                   to_object_guid: str,
+                   from_object_guid: str = None, message_ids=None, *args, **kwargs):
+        """_copy_
+        Args:
+            to_object_guid (str):
+                _to object guid_.
+            from_object_guid (str, optional):
+                _from object guid_. Defaults to update.object_guid.
+            message_ids (typing.Union[str, int, typing.List[str]], optional):
+                _message ids_. Defaults to update.message_id.
+        """
+
+        if from_object_guid is None:
+            from_object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        result = await cls.get_messages(from_object_guid, message_ids)
+        messages = []
+        if result.messages:
+            for message in result.messages:
+
+                try:
+                    file_inline = message.file_inline
+                    kwargs.update(file_inline.to_dict())
+
+                except AttributeError:
+                    file_inline = None
+
+                try:
+                    thumb = thumbnail.Thumbnail(
+                        b64decode(message.thumb_inline), *args, **kwargs)
+
+                except AttributeError:
+                    thumb = kwargs.get('thumb', True)
+
+                try:
+                    message = message.sticker
+
+                except AttributeError:
+                    message = message.raw_text
+
+                if file_inline is not None:
+                    if file_inline.type not in [methods.messages.Gif,
+                                                methods.messages.Sticker]:
+                        file_inline = await cls.download(file_inline)
+                        messages.append(await cls._client.send_message(
+                            thumb=thumb,
+                            message=message,
+                            file_inline=file_inline,
+                            object_guid=to_object_guid, *args, **kwargs))
+                        continue
+
+                messages.append(await cls._client.send_message(
+                    message=message,
+                    object_guid=to_object_guid,
+                    file_inline=file_inline, *args, **kwargs))
+
+        return {'status': 'OK', 'messages': messages}
+
+    @classmethod
+    async def seen(cls, seen_list: dict = None, *args, **kwargs):
+        """_seen_
+        Args:
+            seen_list (dict, optional):
+                _description_. Defaults t
+                    {update.object_guid: update.message_id}
+        """
+
+        if seen_list is None:
+            seen_list = {cls._message.message_update.object_guid: cls._message.message_update.message_id}
+        return await cls._client(methods.chats.SeenChats(seen_list=seen_list))
+
+    @classmethod
+    async def reply(cls,
+                    message=None,
+                    object_guid: str = None,
+                    reply_to_message_id: str = None,
+                    file_inline: str = None, *args, **kwargs):
+        """_reply_
+        Args:
+            message (Any, optional):
+                _message or cation or sticker_ . Defaults to None.
+            object_guid (str):
+                _object guid_ . Defaults to update.object_guid
+            reply_to_message_id (str, optional):
+                _reply to message id_. Defaults to None.
+            file_inline (typing.Union[pathlib.Path, bytes], optional):
+                _file_. Defaults to None.
+            is_gif (bool, optional):
+                _is it a gif file or not_. Defaults to None.
+            is_image (bool, optional):
+                _is it a image file or not_. Defaults to None.
+            is_voice (bool, optional):
+                _is it a voice file or not_. Defaults to None.
+            is_music (bool, optional):
+                _is it a music file or not_. Defaults to None.
+            is_video (bool, optional):
+                _is it a video file or not_. Defaults to None.
+            thumb (bool, optional):
+                if value is "True",
+                the lib will try to build the thumb ( require cv2 )
+                if value is thumbnail.Thumbnail, to set custom
+                Defaults to True.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_id is None:
+            message_id = cls._message.message_update.message_id
+
+        return await cls._client.send_message(
+            message=message,
+            object_guid=object_guid,
+            file_inline=file_inline,
+            reply_to_message_id=reply_to_message_id, *args, **kwargs)
+
+    @classmethod
+    async def forwards(cls,
+                       to_object_guid: str,
+                       from_object_guid: str = None,
+                       message_ids=None, *args, **kwargs):
+        """_forwards_
+        Args:
+            to_object_guid (str):
+                _to object guid_.
+            from_object_guid (str, optional):
+                _from object guid_. Defaults to update.object_guid.
+            message_ids (typing.Union[str, int, typing.List[str]], optional):
+                _message ids_. Defaults to update.message_id.
+        """
+
+        if from_object_guid is None:
+            from_object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.ForwardMessages(
+                from_object_guid=from_object_guid,
+                to_object_guid=to_object_guid,
+                message_ids=message_ids))
+
+    @classmethod
+    async def download(cls, file_inline=None, file=None, *args, **kwargs):
+        return await cls._client.download_file_inline(
+            file_inline or cls._message.file_inline,
+            file=file, *args, **kwargs)
+
+    @classmethod
+    async def get_author(cls, author_guid: str = None, *args, **kwargs):
+        """_get user or author information_
+        Args:
+            author_guid (str, optional):
+                _custom author guid_. Defaults to update.author_guid
+        """
+
+        if author_guid is None:
+            author_guid = cls._message.message_update.message.author_object_guid
+
+        return await cls.get_object(object_guid=author_guid, *args, **kwargs)
+
+    @classmethod
+    async def get_object(cls, object_guid: str = None, *args, **kwargs):
+        """_get object information_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if cls.guid_type(object_guid) == 'User':
+            return await cls._client(
+                methods.users.GetUserInfo(
+                    user_guid=object_guid))
+
+        elif cls.guid_type(object_guid) == 'Group':
+            return await cls._client(
+                methods.groups.GetGroupInfo(
+                    object_guid=object_guid))
+
+        elif cls.guid_type(object_guid) == 'Channel':
+            return await cls._client(
+                methods.channels.GetChannelInfo(
+                    object_guid=object_guid))
+
+    @classmethod
+    async def get_message(cls,
+                          object_guid: str = None,
+                          message_ids=None, *args, **kwargs):
+        """_get messages_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+            message_ids (str, int, typing.List[str]], optional):
+                _message ids_. Defaults to update.message_id.
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.GetMessagesByID(
+                object_guid=object_guid, message_ids=message_ids))
+
+    @classmethod
+    async def delete(cls,
+                     object_guid: str = None,
+                     message_ids=None, *args, **kwargs):
+        """_delete messages_
+        Args:
+            object_guid (str, optional):
+                _custom object guid_. Defaults to update.object_guid.
+            message_ids (str, list, optional):
+                _custom message ids_. Defaults to update.message_id.
+            type(str, optional):
+                the message should be deleted for everyone or not.
+                Defaults to methods.messages.Global (
+                    methods.messages.Local,
+                    methods.messages.Global
+                )
+        """
+
+        if object_guid is None:
+            object_guid = cls._message.message_update.object_guid
+
+        if message_ids is None:
+            message_ids = cls._message.message_update.message_id
+
+        return await cls._client(
+            methods.messages.DeleteMessages(
+                object_guid=object_guid,
+                message_ids=message_ids, *args, **kwargs))
+
+
+class DeleteMessages(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    message_updates: Optional[List[MessageUpdate]] = []
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class RequestSendFile(BaseModel):
+    id: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_send: Optional[str] = None
+    upload_url: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class ForwardMessages(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    message_updates: Optional[List[MessageUpdate]] = []
+    status: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class PollStatus(BaseModel):
+    state: Optional[str] = None
+    selection_index: Optional[int] = None
+    percent_vote_options: Optional[List[int]] = None
+    total_vote: Optional[int] = None
+    show_total_votes: Optional[bool] = None
+
+
+class VotePoll(BaseModel):
+    poll_status: Optional[PollStatus] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class SetPinMessage(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    status: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetMessagesUpdates(BaseModel):
+    updated_messages: Optional[List[MessageUpdate]] = []
+    new_state: Optional[int] = None
+    status: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class SearchGlobalMessages(BaseModel):
+    messages: Optional[List[Message]] = []
+    next_start_id: Optional[str] = None
+    has_continue: Optional[bool] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetMessagesByID(BaseModel):
+    messages: Optional[List[Message]] = []
+    timestamp: Optional[int] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class GetMessagesInterval(BaseModel):
+    messages: Optional[List[Message]] = []
+    state: Optional[str] = None
+    new_has_continue: Optional[bool] = None
+    old_has_continue: Optional[bool] = None
+    new_min_id: Optional[int] = None
+    old_max_id: Optional[int] = None
+    timestamp: Optional[str] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class Reactions(BaseModel):
+    user_guids: Optional[List] = []
+    reaction_count: Optional[int] = None
+    emoji_char: Optional[str] = None
+    reaction_id: Optional[int] = None
+    is_selected: Optional[bool] = None
+
+
+class Reacion(BaseModel):
+    reactions: Optional[List[Reactions]] = []
```

### Comparing `aiorubika-0.0.2/aiorubika/types/models/stickers.py` & `aiorubika-1.0.0/aiorubika/types/models/stickers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-from pydantic import BaseModel, HttpUrl
-from typing import List, Optional
-
-class File(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-    file_name: Optional[str] = None
-    cdn_tag: Optional[str] = None
-
-class Sticker(BaseModel):
-    emoji_character: Optional[str] = None
-    w_h_ratio: Optional[str] = None
-    sticker_id: Optional[str] = None
-    file: Optional[File] = None
-    sticker_set_id: Optional[str] = None
-
-class SetImage(BaseModel):
-    file_id: Optional[str] = None
-    mime: Optional[str] = None
-    dc_id: Optional[str] = None
-    access_hash_rec: Optional[str] = None
-    cdn_tag: Optional[str] = None
-
-class TrendStickerSet(BaseModel):
-    sticker_set_id: Optional[str] = None
-    title: Optional[str] = None
-    count_stickers: Optional[int] = None
-    set_image: Optional[SetImage] = None
-    top_stickers: Optional[List[Sticker]] = None
-    share_string: Optional[HttpUrl] = None
-    update_time: Optional[int] = None
-
-class GetTrendStickerSets(BaseModel):
-    sticker_sets: Optional[List[TrendStickerSet]] = None
-    next_start_id: Optional[str] = None
-    has_continue: Optional[bool] = None
-
-class GetStickersBySetIDs(BaseModel):
-    stickers: Optional[List[Sticker]] = []
-
-class StickerSets(BaseModel):
-    sticker_set_id: Optional[str] = None
-    title: Optional[str] = None
-    count_stickers: Optional[int] = None
-    set_image: Optional[SetImage] = None
-    top_stickers: Optional[List[Sticker]] = []
-
-class GetMyStickerSets(BaseModel):
-    sticker_sets: Optional[List[StickerSets]] = []
+from pydantic import BaseModel, HttpUrl
+from typing import List, Optional
+
+
+class File(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+    file_name: Optional[str] = None
+    cdn_tag: Optional[str] = None
+
+
+class Sticker(BaseModel):
+    emoji_character: Optional[str] = None
+    w_h_ratio: Optional[str] = None
+    sticker_id: Optional[str] = None
+    file: Optional[File] = None
+    sticker_set_id: Optional[str] = None
+
+
+class SetImage(BaseModel):
+    file_id: Optional[str] = None
+    mime: Optional[str] = None
+    dc_id: Optional[str] = None
+    access_hash_rec: Optional[str] = None
+    cdn_tag: Optional[str] = None
+
+
+class TrendStickerSet(BaseModel):
+    sticker_set_id: Optional[str] = None
+    title: Optional[str] = None
+    count_stickers: Optional[int] = None
+    set_image: Optional[SetImage] = None
+    top_stickers: Optional[List[Sticker]] = None
+    share_string: Optional[HttpUrl] = None
+    update_time: Optional[int] = None
+
+
+class GetTrendStickerSets(BaseModel):
+    sticker_sets: Optional[List[TrendStickerSet]] = None
+    next_start_id: Optional[str] = None
+    has_continue: Optional[bool] = None
+
+
+class GetStickersBySetIDs(BaseModel):
+    stickers: Optional[List[Sticker]] = []
+
+
+class StickerSets(BaseModel):
+    sticker_set_id: Optional[str] = None
+    title: Optional[str] = None
+    count_stickers: Optional[int] = None
+    set_image: Optional[SetImage] = None
+    top_stickers: Optional[List[Sticker]] = []
+
+
+class GetMyStickerSets(BaseModel):
+    sticker_sets: Optional[List[StickerSets]] = []
```

### Comparing `aiorubika-0.0.2/aiorubika/types/models/users.py` & `aiorubika-1.0.0/aiorubika/types/models/users.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,113 @@
-from pydantic import BaseModel
-from typing import List, Optional
-
-class OnlineTime(BaseModel):
-    type: Optional[str] = None
-    exact_time: Optional[int] = None
-
-class LastMessage(BaseModel):
-    message_id: Optional[str] = None
-    type: Optional[str] = None
-    text: Optional[str] = None
-    author_object_guid: Optional[str] = None
-    is_mine: Optional[bool] = None
-    author_title: Optional[str] = None
-    author_type: Optional[str] = None
-
-class AbsObject(BaseModel):
-    object_guid: Optional[str] = None
-    type: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    is_verified: Optional[bool] = None
-    is_deleted: Optional[bool] = None
-
-class Chat(BaseModel):
-    object_guid: Optional[str] = None
-    access: Optional[List[str]] = None
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[LastMessage] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    abs_object: Optional[AbsObject] = None
-    is_blocked: Optional[bool] = None
-    last_message_id: Optional[str] = None
-    last_deleted_mid: Optional[str] = None
-
-class UserInfo(BaseModel):
-    user_guid: Optional[str] = None
-    first_name: Optional[str] = None
-    last_name: Optional[str] = None
-    phone: Optional[str] = None
-    username: Optional[str] = None
-    last_online: Optional[int] = None
-    bio: Optional[str] = None
-    is_deleted: Optional[bool] = None
-    is_verified: Optional[bool] = None
-    online_time: Optional[OnlineTime] = None
-
-class GetUserInfo(BaseModel):
-    user: Optional[UserInfo] = None
-    chat: Optional[Chat] = None
-    timestamp: Optional[str] = None
-    can_receive_call: Optional[bool] = None
-    can_video_call: Optional[bool] = None
-
-class ChatAccess(BaseModel):
-    access: Optional[List[str]] = None
-    count_unseen: Optional[int] = None
-    is_mute: Optional[bool] = None
-    is_pinned: Optional[bool] = None
-    time_string: Optional[str] = None
-    last_message: Optional[LastMessage] = None
-    last_seen_my_mid: Optional[str] = None
-    last_seen_peer_mid: Optional[str] = None
-    status: Optional[str] = None
-    time: Optional[int] = None
-    pinned_message_id: Optional[str] = None
-    abs_object: Optional[AbsObject] = None
-    is_blocked: Optional[bool] = None
-    last_message_id: Optional[str] = None
-    last_deleted_mid: Optional[str] = None
-    slow_mode_duration: Optional[int] = None
-    group_my_last_send_time: Optional[int] = None
-    pinned_message_ids: Optional[List[str]] = None
-
-class ChatUpdate(BaseModel):
-    object_guid: Optional[str] = None
-    action: Optional[str] = None
-    chat: Optional[ChatAccess] = None
-    updated_parameters: Optional[List[str]] = None
-    timestamp: Optional[str] = None
-    type: Optional[str] = None
-
-class BlockUser(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class DeleteUserChat(BaseModel):
-    chat_update: Optional[ChatUpdate] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
-
-class CheckUserName(BaseModel):
-    exist: Optional[bool] = None
-    _client: Optional[str] = None
-    original_update: Optional[str] = None
+from typing import List, Optional
+from pydantic import BaseModel
+
+
+class OnlineTime(BaseModel):
+    type: Optional[str] = None
+    exact_time: Optional[int] = None
+
+
+class LastMessage(BaseModel):
+    message_id: Optional[str] = None
+    type: Optional[str] = None
+    text: Optional[str] = None
+    author_object_guid: Optional[str] = None
+    is_mine: Optional[bool] = None
+    author_title: Optional[str] = None
+    author_type: Optional[str] = None
+
+
+class AbsObject(BaseModel):
+    object_guid: Optional[str] = None
+    type: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    is_verified: Optional[bool] = None
+    is_deleted: Optional[bool] = None
+
+
+class Chat(BaseModel):
+    object_guid: Optional[str] = None
+    access: Optional[List[str]] = None
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[LastMessage] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    abs_object: Optional[AbsObject] = None
+    is_blocked: Optional[bool] = None
+    last_message_id: Optional[str] = None
+    last_deleted_mid: Optional[str] = None
+
+
+class UserInfo(BaseModel):
+    user_guid: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    phone: Optional[str] = None
+    username: Optional[str] = None
+    last_online: Optional[int] = None
+    bio: Optional[str] = None
+    is_deleted: Optional[bool] = None
+    is_verified: Optional[bool] = None
+    online_time: Optional[OnlineTime] = None
+
+
+class GetUserInfo(BaseModel):
+    user: Optional[UserInfo] = None
+    chat: Optional[Chat] = None
+    timestamp: Optional[str] = None
+    can_receive_call: Optional[bool] = None
+    can_video_call: Optional[bool] = None
+
+
+class ChatAccess(BaseModel):
+    access: Optional[List[str]] = None
+    count_unseen: Optional[int] = None
+    is_mute: Optional[bool] = None
+    is_pinned: Optional[bool] = None
+    time_string: Optional[str] = None
+    last_message: Optional[LastMessage] = None
+    last_seen_my_mid: Optional[str] = None
+    last_seen_peer_mid: Optional[str] = None
+    status: Optional[str] = None
+    time: Optional[int] = None
+    pinned_message_id: Optional[str] = None
+    abs_object: Optional[AbsObject] = None
+    is_blocked: Optional[bool] = None
+    last_message_id: Optional[str] = None
+    last_deleted_mid: Optional[str] = None
+    slow_mode_duration: Optional[int] = None
+    group_my_last_send_time: Optional[int] = None
+    pinned_message_ids: Optional[List[str]] = None
+
+
+class ChatUpdate(BaseModel):
+    object_guid: Optional[str] = None
+    action: Optional[str] = None
+    chat: Optional[ChatAccess] = None
+    updated_parameters: Optional[List[str]] = None
+    timestamp: Optional[str] = None
+    type: Optional[str] = None
+
+
+class BlockUser(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class DeleteUserChat(BaseModel):
+    chat_update: Optional[ChatUpdate] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
+
+
+class CheckUserName(BaseModel):
+    exist: Optional[bool] = None
+    _client: Optional[str] = None
+    original_update: Optional[str] = None
```

### Comparing `aiorubika-0.0.2/aiorubika/types/results.py` & `aiorubika-1.0.0/aiorubika/types/results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,77 @@
-from json import dumps
-
-
-class Results:
-    def __str__(self) -> str:
-        return self.jsonify(indent=2)
-
-    def __getattr__(self, name):
-        return self.find_keys(keys=name)
-
-    def __setitem__(self, key, value):
-        self.original_update[key] = value
-
-    def __getitem__(self, key):
-        return self.original_update[key]
-
-    def __lts__(self, update: list, *args, **kwargs):
-        for index, element in enumerate(update):
-            if isinstance(element, list):
-                update[index] = self.__lts__(update=element)
-
-            elif isinstance(element, dict):
-                update[index] = Results(update=element)
-
-            else:
-                update[index] = element
-        return update
-
-    def __init__(self, update: dict, *args, **kwargs) -> None:
-        self.original_update = update
-
-    def to_dict(self):
-        return self.original_update
-
-    def jsonify(self, indent=None, *args, **kwargs) -> str:
-        result = self.original_update
-        result['original_update'] = 'dict{...}'
-        return dumps(result, indent=indent,
-                          ensure_ascii=False,
-                          default=lambda value: str(value))
-
-    def find_keys(self, keys, original_update=None, *args, **kwargs):
-
-        if original_update is None:
-            original_update = self.original_update
-
-        if not isinstance(keys, list):
-            keys = [keys]
-
-        if isinstance(original_update, dict):
-            for key in keys:
-                try:
-                    update = original_update[key]
-                    if isinstance(update, dict):
-                        update = Results(update=update)
-
-                    elif isinstance(update, list):
-                        update = self.__lts__(update=update)
-
-                    return update
-
-                except KeyError:
-                    pass
-            original_update = original_update.values()
-
-        for value in original_update:
-            if isinstance(value, (dict, list)):
-                try:
-                    return self.find_keys(keys=keys, original_update=value)
-
-                except AttributeError:
-                    return None
-
-        return None
+from json import dumps
+
+
+class Results:
+
+    def __str__(self) -> str:
+        return self.jsonify(indent=2)
+
+    def __getattr__(self, name):
+        return self.find_keys(keys=name)
+
+    def __setitem__(self, key, value):
+        self.original_update[key] = value
+
+    def __getitem__(self, key):
+        return self.original_update[key]
+
+    def __lts__(self, update: list, *args, **kwargs):
+        for index, element in enumerate(update):
+            if isinstance(element, list):
+                update[index] = self.__lts__(update=element)
+
+            elif isinstance(element, dict):
+                update[index] = Results(update=element)
+
+            else:
+                update[index] = element
+        return update
+
+    def __init__(self, update: dict, *args, **kwargs) -> None:
+        self.original_update = update
+
+    def to_dict(self):
+        return self.original_update
+
+    def jsonify(self, indent=None, *args, **kwargs) -> str:
+        result = self.original_update
+        result['original_update'] = 'dict{...}'
+        return dumps(
+            result, indent=indent,
+            ensure_ascii=False,
+            default=lambda value: str(value)
+        )
+
+    def find_keys(self, keys, original_update=None, *args, **kwargs):
+
+        if original_update is None:
+            original_update = self.original_update
+
+        if not isinstance(keys, list):
+            keys = [keys]
+
+        if isinstance(original_update, dict):
+            for key in keys:
+                try:
+                    update = original_update[key]
+                    if isinstance(update, dict):
+                        update = Results(update=update)
+
+                    elif isinstance(update, list):
+                        update = self.__lts__(update=update)
+
+                    return update
+
+                except KeyError:
+                    pass
+            original_update = original_update.values()
+
+        for value in original_update:
+            if isinstance(value, (dict, list)):
+                try:
+                    return self.find_keys(keys=keys, original_update=value)
+
+                except AttributeError:
+                    return None
+
+        return None
```

### Comparing `aiorubika-0.0.2/aiorubika/utils.py` & `aiorubika-1.0.0/aiorubika/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,61 @@
 import re
 
 RUBIKA_LINK_PATTERN = re.compile(r'\brubika\.ir\b')
-GROUP_LINK_PATTERN = re.compile(r'https://rubika\.ir/joing/[A-Z0-9]+')
 USERNAME_PATTERN = re.compile(r'@([a-zA-Z0-9_]{3,32})')
+GROUP_LINK_PATTERN = re.compile(r'https://rubika\.ir/joing/[A-Z0-9]+')
+
 
 def is_rubika_link(string: str) -> bool:
     return bool(RUBIKA_LINK_PATTERN.search(string))
 
+
 def is_group_link(string: str) -> bool:
     return bool(GROUP_LINK_PATTERN.search(string))
 
+
 def is_username(string: str) -> bool:
     return bool(USERNAME_PATTERN.search(string))
 
+
 def get_rubika_links(string: str) -> list:
     return RUBIKA_LINK_PATTERN.findall(string)
 
+
 def get_group_links(string: str) -> list:
     return GROUP_LINK_PATTERN.findall(string)
 
+
 def get_usernames(string: str) -> list:
     return USERNAME_PATTERN.findall(string)
 
+
 def Bold(text: str) -> str:
     return f'**{text.strip()}**'
 
+
 def Italic(text: str) -> str:
     return f'__{text.strip()}__'
 
+
 def Underline(text: str) -> str:
     return f'--{text.strip()}--'
 
+
 def Strike(text: str) -> str:
     return f'~~{text.strip()}~~'
 
+
 def Spoiler(text: str) -> str:
     return f'||{text.strip()}||'
 
+
 def Code(text: str):
     return f'`{text.strip()}`'
 
+
 def Mention(text: str, object_guid: str) -> str:
     return f'[{text.strip()}]({object_guid.strip()})'
 
+
 def HyperLink(text: str, link: str) -> str:
-    return f'[{text.strip()}]({link.strip()})'
+    return f'[{text.strip()}]({link.strip()})'
```

### Comparing `aiorubika-0.0.2/aiorubika.egg-info/PKG-INFO` & `aiorubika-1.0.0/aiorubika.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aiorubika
-Version: 0.0.2
-Summary:  Rubika API Framework for Python
-Home-page: https://github.com/metect/rubika
+Version: 1.0.0
+Summary: aiorubika is a modern and fully asynchronous framework for Rubika Self API written in Python 
+Home-page: https://github.com/irvanyamirali/aiorubika
 Author: amirali irvany
-Author-email: dev.amirali.irvany@gmail.com
-Keywords: rubika,aiorubika,chat,bot,robot,asyncio
+Author-email: irvanyamirali@gmail.com
+Keywords: rubika,aiorubika,bot,asyncio,aiohttp,pydantic
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -17,38 +17,40 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: pycryptodome
 Requires-Dist: pydantic==1.10.12
 Requires-Dist: aiofiles
 Provides-Extra: cv
 Requires-Dist: opencv-python; extra == "cv"
 Provides-Extra: pil
 Requires-Dist: pillow; extra == "pil"
 
-# AIORubika
-Rubika API Framework for Python
+# aiorubika
 
-### Examples
+Python-based asynchronous framework for Rubika messenger API
+
+## Install
+```bash
+pip install aiorubika
+```
+
+
+## Quik Start
 ```python
 from aiorubika import Client, filters, utils
-from aiorubika.types import Updates
-
-bot = Client(name='rubpy')
 
-@bot.on_message_updates(filters.text)
-async def updates(update: Updates):
+bot = Client(name='bot')
+@bot.on_message_updates(filters.is_private)
+async def updates(update):
     print(update)
-    await update.reply(utils.Code('hello') + utils.Underline('from') + utils.Bold('rubpy'))
+    await update.reply(utils.Code('hello') + utils.Underline('from') + utils.Bold('aiorubika'))
 
 bot.run()
 ```
 
-## Install
-```bash
-pip install aiorubika
-```
```

### Comparing `aiorubika-0.0.2/setup.py` & `aiorubika-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from setuptools import setup, find_packages
-
-requirements = [
-    'aiohttp',
-    'pycryptodome',
-    'pydantic==1.10.12',
-    'aiofiles',
-]
-
-with open('README.md', encoding='UTF-8') as f:
-    readme = f.read()
-
-setup(
-    name='aiorubika',
-    version='0.0.2',
-    author='amirali irvany',
-    author_email='dev.amirali.irvany@gmail.com',
-    description=' Rubika API Framework for Python',
-    keywords=['rubika', 'aiorubika', 'chat', 'bot', 'robot', 'asyncio'],
-    long_description=readme,
-    python_requires="~=3.7",
-    long_description_content_type='text/markdown',
-    url='https://github.com/metect/rubika',
-    packages=find_packages(),
-    exclude_package_data={'': ['*.pyc', '*__pycache__*']},
-    install_requires=requirements,
-    extras_require={
-        'cv': ['opencv-python'],
-        'pil': ['pillow']
-    },
-    classifiers=[
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Topic :: Internet',
-        'Topic :: Communications',
-        'Topic :: Communications :: Chat',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Software Development :: Libraries :: Application Frameworks'
-    ],
-)
+from setuptools import setup, find_packages
+
+requirements = [
+    'aiohttp',
+    'pycryptodome',
+    'pydantic==1.10.12',
+    'aiofiles',
+]
+
+with open('README.md', encoding='UTF-8') as f:
+    readme = f.read()
+
+
+setup(
+    name='aiorubika',
+    version='1.0.0',
+    author='amirali irvany',
+    author_email='irvanyamirali@gmail.com',
+    description='aiorubika is a modern and fully asynchronous framework for Rubika Self API written in Python ',
+    keywords=['rubika', 'aiorubika', 'bot', 'asyncio', 'aiohttp', 'pydantic'],
+    long_description=readme,
+    python_requires="~=3.7",
+    long_description_content_type='text/markdown',
+    url='https://github.com/irvanyamirali/aiorubika',
+    packages=find_packages(),
+    exclude_package_data={'': ['*.pyc', '*__pycache__*']},
+    install_requires=requirements,
+    extras_require={
+        'cv': ['opencv-python'],
+        'pil': ['pillow']
+    },
+    classifiers=[
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
+        'Topic :: Internet',
+        'Topic :: Communications',
+        'Topic :: Communications :: Chat',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Software Development :: Libraries :: Application Frameworks'
+    ],
+)
```

