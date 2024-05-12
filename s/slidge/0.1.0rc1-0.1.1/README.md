# Comparing `tmp/slidge-0.1.0rc1.tar.gz` & `tmp/slidge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slidge-0.1.0rc1.tar", max compression
+gzip compressed data, was "slidge-0.1.1.tar", max compression
```

## Comparing `slidge-0.1.0rc1.tar` & `slidge-0.1.1.tar`

### file list

```diff
@@ -1,99 +1,95 @@
--rw-r--r--   0        0        0    34523 2023-01-08 11:57:11.502146 slidge-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     5897 2023-01-08 11:57:11.502146 slidge-0.1.0rc1/README.md
--rw-r--r--   0        0        0     1792 2023-01-08 12:30:23.708005 slidge-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0      841 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/__init__.py
--rw-r--r--   0        0        0     4257 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/__main__.py
--rw-r--r--   0        0        0       36 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/core/__init__.py
--rw-r--r--   0        0        0    17007 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/core/adhoc.py
--rw-r--r--   0        0        0     2918 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/core/cache.py
--rw-r--r--   0        0        0     7020 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/chat_command.py
--rw-r--r--   0        0        0     3215 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/config.py
--rw-r--r--   0        0        0    14880 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/contact.py
--rw-r--r--   0        0        0     1707 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/disco.py
--rw-r--r--   0        0        0    33682 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/gateway.py
--rw-r--r--   0        0        0      307 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/__init__.py
--rw-r--r--   0        0        0     1072 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/base.py
--rw-r--r--   0        0        0     2113 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/disco.py
--rw-r--r--   0        0        0    14819 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/message.py
--rw-r--r--   0        0        0     3770 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/presence.py
--rw-r--r--   0        0        0      119 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/__init__.py
--rw-r--r--   0        0        0     2697 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/bookmarks.py
--rw-r--r--   0        0        0     5148 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/participant.py
--rw-r--r--   0        0        0    11126 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/room.py
--rw-r--r--   0        0        0    12305 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/pubsub.py
--rw-r--r--   0        0        0    24193 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/session.py
--rw-r--r--   0        0        0        0 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/plugins/__init__.py
--rw-r--r--   0        0        0     3759 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/plugins/discord/__init__.py
--rw-r--r--   0        0        0     4357 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/plugins/discord/client.py
--rw-r--r--   0        0        0     5841 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/discord/session.py
--rw-r--r--   0        0        0    10479 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/dummy.py
--rw-r--r--   0        0        0    22184 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/facebook.py
--rw-r--r--   0        0        0     7604 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/hackernews.py
--rw-r--r--   0        0        0       38 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/__init__.py
--rw-r--r--   0        0        0     9601 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/api.py
--rw-r--r--   0        0        0    16234 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/gateway.py
--rw-r--r--   0        0        0     8504 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/websocket.py
--rw-r--r--   0        0        0      115 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/__init__.py
--rw-r--r--   0        0        0      124 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/config.py
--rw-r--r--   0        0        0     3572 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/contact.py
--rw-r--r--   0        0        0    12953 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/gateway.py
--rw-r--r--   0        0        0     2403 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/group.py
--rw-r--r--   0        0        0    18611 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/session.py
--rw-r--r--   0        0        0      555 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/txt.py
--rw-r--r--   0        0        0     1112 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/util.py
--rw-r--r--   0        0        0    11606 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/skype.py
--rw-r--r--   0        0        0    14752 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/steam.py
--rw-r--r--   0        0        0      185 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/telegram/__init__.py
--rw-r--r--   0        0        0    13681 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/client.py
--rw-r--r--   0        0        0      667 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/config.py
--rw-r--r--   0        0        0     5527 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/contact.py
--rw-r--r--   0        0        0     6687 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/gateway.py
--rw-r--r--   0        0        0     6566 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/group.py
--rw-r--r--   0        0        0     9339 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/session.py
--rw-r--r--   0        0        0     6523 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/util.py
--rw-r--r--   0        0        0      112 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/__init__.py
--rw-r--r--   0        0        0      574 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/config.py
--rw-r--r--   0        0        0     1095 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/contact.py
--rw-r--r--   0        0        0    15365 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/event.go
--rw-r--r--   0        0        0     4997 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/gateway.go
--rw-r--r--   0        0        0     2281 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/gateway.py
--rw-r--r--   0        0        0      484 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/go.mod
--rw-r--r--   0        0        0     2064 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/go.sum
--rw-r--r--   0        0        0    12445 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/session.go
--rw-r--r--   0        0        0    14739 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/session.py
--rw-r--r--   0        0        0      299 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/__init__.py
--rw-r--r--   0        0        0     5708 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/conf.py
--rw-r--r--   0        0        0     7758 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/db.py
--rw-r--r--   0        0        0     9295 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/test.py
--rw-r--r--   0        0        0     1633 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/types.py
--rw-r--r--   0        0        0     3596 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/util.py
--rw-r--r--   0        0        0      372 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/__init__.py
--rw-r--r--   0        0        0    31653 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/disco.py
--rw-r--r--   0        0        0      292 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/stanza/__init__.py
--rw-r--r--   0        0        0    10428 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/stanza/info.py
--rw-r--r--   0        0        0     4608 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/stanza/items.py
--rw-r--r--   0        0        0    17117 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/static.py
--rw-r--r--   0        0        0      305 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0050/__init__.py
--rw-r--r--   0        0        0    22499 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0050/adhoc.py
--rw-r--r--   0        0        0     5814 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0050/stanza.py
--rw-r--r--   0        0        0      325 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0077/__init__.py
--rw-r--r--   0        0        0    10402 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0077/register.py
--rw-r--r--   0        0        0     2186 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0077/stanza.py
--rw-r--r--   0        0        0      107 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0100/__init__.py
--rw-r--r--   0        0        0     4312 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0100/gateway.py
--rw-r--r--   0        0        0      232 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0100/stanza.py
--rw-r--r--   0        0        0       29 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0292/__init__.py
--rw-r--r--   0        0        0     3782 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0292/stanza.py
--rw-r--r--   0        0        0     2102 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0292/vcard4.py
--rw-r--r--   0        0        0      166 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/__init__.py
--rw-r--r--   0        0        0      625 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/permissions.py
--rw-r--r--   0        0        0     5204 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/privilege.py
--rw-r--r--   0        0        0     1206 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/stanza.py
--rw-r--r--   0        0        0      180 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356_old/__init__.py
--rw-r--r--   0        0        0     5299 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356_old/privilege.py
--rw-r--r--   0        0        0     1229 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0356_old/stanza.py
--rw-r--r--   0        0        0      126 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0461/__init__.py
--rw-r--r--   0        0        0     1383 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0461/reply.py
--rw-r--r--   0        0        0     2390 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0461/stanza.py
--rw-r--r--   0        0        0     7811 1970-01-01 00:00:00.000000 slidge-0.1.0rc1/setup.py
--rw-r--r--   0        0        0     7457 1970-01-01 00:00:00.000000 slidge-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-12 04:44:15.843167 slidge-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3684 2024-05-12 04:44:15.843167 slidge-0.1.1/README.md
+-rw-r--r--   0        0        0     2002 2024-05-12 04:44:32.601630 slidge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1624 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/__init__.py
+-rw-r--r--   0        0        0     5804 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/__main__.py
+-rw-r--r--   0        0        0      613 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/__init__.py
+-rw-r--r--   0        0        0     9188 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/adhoc.py
+-rw-r--r--   0        0        0     5759 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/admin.py
+-rw-r--r--   0        0        0    13073 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/base.py
+-rw-r--r--   0        0        0       99 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/categories.py
+-rw-r--r--   0        0        0     9975 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/chat_command.py
+-rw-r--r--   0        0        0     6014 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/register.py
+-rw-r--r--   0        0        0     8781 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/command/user.py
+-rw-r--r--   0        0        0      191 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/contact/__init__.py
+-rw-r--r--   0        0        0    16101 2024-05-12 04:44:15.856597 slidge-0.1.1/slidge/contact/contact.py
+-rw-r--r--   0        0        0     7489 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/contact/roster.py
+-rw-r--r--   0        0        0       68 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/__init__.py
+-rw-r--r--   0        0        0     5443 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/cache.py
+-rw-r--r--   0        0        0     7392 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/config.py
+-rw-r--r--   0        0        0       58 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/__init__.py
+-rw-r--r--   0        0        0    34649 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/base.py
+-rw-r--r--   0        0        0     1919 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/caps.py
+-rw-r--r--   0        0        0     1352 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/delivery_receipt.py
+-rw-r--r--   0        0        0     2230 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/disco.py
+-rw-r--r--   0        0        0     2471 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/mam.py
+-rw-r--r--   0        0        0     1033 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/muc_admin.py
+-rw-r--r--   0        0        0     1753 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/ping.py
+-rw-r--r--   0        0        0     2732 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/presence.py
+-rw-r--r--   0        0        0     1619 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/registration.py
+-rw-r--r--   0        0        0     3518 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/search.py
+-rw-r--r--   0        0        0    28927 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/session_dispatcher.py
+-rw-r--r--   0        0        0     4639 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/gateway/vcard_temp.py
+-rw-r--r--   0        0        0      368 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/__init__.py
+-rw-r--r--   0        0        0    17808 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/attachment.py
+-rw-r--r--   0        0        0     5493 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/avatar.py
+-rw-r--r--   0        0        0      702 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/base.py
+-rw-r--r--   0        0        0     3935 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/disco.py
+-rw-r--r--   0        0        0      913 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/lock.py
+-rw-r--r--   0        0        0    14790 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/message.py
+-rw-r--r--   0        0        0     5606 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/message_maker.py
+-rw-r--r--   0        0        0     7216 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/presence.py
+-rw-r--r--   0        0        0     1302 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/mixins/recipient.py
+-rw-r--r--   0        0        0    18268 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/pubsub.py
+-rw-r--r--   0        0        0    26134 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/core/session.py
+-rw-r--r--   0        0        0      258 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/__init__.py
+-rw-r--r--   0        0        0     3426 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/archive.py
+-rw-r--r--   0        0        0     5944 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/bookmarks.py
+-rw-r--r--   0        0        0    14862 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/participant.py
+-rw-r--r--   0        0        0    38972 2024-05-12 04:44:15.859954 slidge-0.1.1/slidge/group/room.py
+-rw-r--r--   0        0        0      334 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/migration.py
+-rw-r--r--   0        0        0        0 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/py.typed
+-rw-r--r--   0        0        0     1777 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/link_preview/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/link_preview/link_preview.py
+-rw-r--r--   0        0        0     2664 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/link_preview/stanza.py
+-rw-r--r--   0        0        0     1545 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/roster.py
+-rw-r--r--   0        0        0      325 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0077/__init__.py
+-rw-r--r--   0        0        0    10431 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0077/register.py
+-rw-r--r--   0        0        0     2410 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0077/stanza.py
+-rw-r--r--   0        0        0      107 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0100/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0100/gateway.py
+-rw-r--r--   0        0        0      232 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0100/stanza.py
+-rw-r--r--   0        0        0      319 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0153/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0153/stanza.py
+-rw-r--r--   0        0        0      658 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0153/vcard_avatar.py
+-rw-r--r--   0        0        0      109 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0264/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0264/stanza.py
+-rw-r--r--   0        0        0      456 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0264/thumbnail.py
+-rw-r--r--   0        0        0       98 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0292/__init__.py
+-rw-r--r--   0        0        0     3113 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0292/vcard4.py
+-rw-r--r--   0        0        0      368 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0313/__init__.py
+-rw-r--r--   0        0        0     9211 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0313/mam.py
+-rw-r--r--   0        0        0    10249 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0313/stanza.py
+-rw-r--r--   0        0        0      104 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0317/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0317/hats.py
+-rw-r--r--   0        0        0      659 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0317/stanza.py
+-rw-r--r--   0        0        0      180 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0356_old/__init__.py
+-rw-r--r--   0        0        0     5338 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0356_old/privilege.py
+-rw-r--r--   0        0        0     1229 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0356_old/stanza.py
+-rw-r--r--   0        0        0      284 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0424/__init__.py
+-rw-r--r--   0        0        0     2448 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0424/retraction.py
+-rw-r--r--   0        0        0      753 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0424/stanza.py
+-rw-r--r--   0        0        0      158 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0490/__init__.py
+-rw-r--r--   0        0        0     1527 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0490/mds.py
+-rw-r--r--   0        0        0      443 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/slixfix/xep_0490/stanza.py
+-rw-r--r--   0        0        0      301 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/archive_msg.py
+-rw-r--r--   0        0        0     6613 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/conf.py
+-rw-r--r--   0        0        0     6604 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/db.py
+-rw-r--r--   0        0        0     2682 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/schema.sql
+-rw-r--r--   0        0        0    16517 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/sql.py
+-rw-r--r--   0        0        0    10688 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/test.py
+-rw-r--r--   0        0        0     4689 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/types.py
+-rw-r--r--   0        0        0     8587 2024-05-12 04:44:15.863312 slidge-0.1.1/slidge/util/util.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 slidge-0.1.1/PKG-INFO
```

### Comparing `slidge-0.1.0rc1/LICENSE` & `slidge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0rc1/slidge/__main__.py` & `slidge-0.1.1/slidge/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 """
 Slidge can be configured via CLI args, environment variables and/or INI files.
+
 To use env vars, use this convention: ``--home-dir`` becomes ``HOME_DIR``.
+
+Everything in ``/etc/slidge/conf.d/*`` is automatically used.
+To use a plugin-specific INI file, put it in another dir,
+and launch slidge with ``-c /path/to/plugin-specific.conf``.
+Use the long version of the CLI arg without the double dash prefix inside this
+INI file, eg ``debug=true``.
+
+An example configuration file is available at
+https://git.sr.ht/~nicoco/slidge/tree/master/item/dev/confs/slidge-example.ini
 """
+
+import asyncio
 import importlib
 import logging
+import os
 import signal
 from pathlib import Path
 
 import configargparse
 
 from slidge import BaseGateway
 from slidge.core import config
 from slidge.core.cache import avatar_cache
+from slidge.migration import migrate
 from slidge.util.conf import ConfigModule
 from slidge.util.db import user_store
+from slidge.util.util import get_version  # noqa: F401
 
 
 class MainConfig(ConfigModule):
     def update_dynamic_defaults(self, args):
-        logging.basicConfig(level=args.loglevel)
+        # force=True is needed in case we call a logger before this is reached,
+        # or basicConfig has no effect
+        logging.basicConfig(
+            level=args.loglevel,
+            filename=args.log_file,
+            force=True,
+            format=args.log_format,
+        )
 
         if args.home_dir is None:
             args.home_dir = Path("/var/lib/slidge") / str(args.jid)
 
         if args.user_jid_validator is None:
             args.user_jid_validator = ".*@" + args.server
 
 
 class SigTermInterrupt(Exception):
     pass
 
 
 def get_configurator():
     p = configargparse.ArgumentParser(
-        default_config_files=["/etc/slidge/conf.d/*.conf"], description=__doc__
+        default_config_files=os.getenv(
+            "SLIDGE_CONF_DIR", "/etc/slidge/conf.d/*.conf"
+        ).split(":"),
+        description=__doc__,
     )
     p.add_argument(
         "-c",
         "--config",
         help="Path to a INI config file.",
         env_var="SLIDGE_CONFIG",
         is_config_file=True,
@@ -57,14 +82,19 @@
         "--debug",
         help="loglevel=DEBUG",
         action="store_const",
         dest="loglevel",
         const=logging.DEBUG,
         env_var="SLIDGE_DEBUG",
     )
+    p.add_argument(
+        "--version",
+        action="version",
+        version=f"%(prog)s {__version__}",
+    )
     configurator = MainConfig(config, p)
     return configurator
 
 
 def get_parser():
     return get_configurator().parser
 
@@ -76,15 +106,15 @@
     if not (h := config.HOME_DIR).exists():
         logging.info("Creating directory '%s'", h)
         h.mkdir()
 
     db_file = config.HOME_DIR / "slidge.db"
     user_store.set_file(db_file, args.secret_key)
 
-    avatar_cache.set_dir(h / "slidge_avatars")
+    avatar_cache.set_dir(h / "slidge_avatars_v2")
 
     config.UPLOAD_REQUESTER = config.UPLOAD_REQUESTER or config.JID.bare
 
     return unknown_argv
 
 
 def handle_sigterm(_signum, _frame):
@@ -92,31 +122,41 @@
     raise SigTermInterrupt
 
 
 def main():
     signal.signal(signal.SIGTERM, handle_sigterm)
 
     unknown_argv = configure()
+    logging.info("Starting slidge version %s", __version__)
 
     legacy_module = importlib.import_module(config.LEGACY_MODULE)
+    logging.debug("Legacy module: %s", dir(legacy_module))
+    logging.info(
+        "Starting legacy module: '%s' version %s",
+        config.LEGACY_MODULE,
+        getattr(legacy_module, "__version__", "No version"),
+    )
 
     if plugin_config_obj := getattr(
         legacy_module, "config", getattr(legacy_module, "Config", None)
     ):
         logging.debug("Found a config object in plugin: %r", plugin_config_obj)
         ConfigModule.ENV_VAR_PREFIX += (
             f"_{config.LEGACY_MODULE.split('.')[-1].upper()}_"
         )
         logging.debug("Env var prefix: %s", ConfigModule.ENV_VAR_PREFIX)
         ConfigModule(plugin_config_obj).set_conf(unknown_argv)
     else:
         if unknown_argv:
             raise RuntimeError("Some arguments have not been recognized", unknown_argv)
 
-    gateway = BaseGateway.get_unique_subclass()()
+    migrate()
+
+    gateway: BaseGateway = BaseGateway.get_unique_subclass()()
+    avatar_cache.http = gateway.http
     gateway.connect()
 
     return_code = 0
     try:
         gateway.loop.run_forever()
     except KeyboardInterrupt:
         logging.debug("Received SIGINT")
@@ -132,21 +172,27 @@
     finally:
         if gateway.has_crashed:
             if return_code != 0:
                 logging.warning("Return code has been set twice. Please report this.")
             return_code = 3
         if gateway.is_connected():
             logging.debug("Gateway is connected, cleaning up")
-            gateway.shutdown()
+            gateway.loop.run_until_complete(asyncio.gather(*gateway.shutdown()))
             gateway.disconnect()
             gateway.loop.run_until_complete(gateway.disconnected)
         else:
             logging.debug("Gateway is not connected, no need to clean up")
         user_store.close()
         avatar_cache.close()
+        gateway.loop.run_until_complete(gateway.http.close())
         logging.info("Successful clean shut down")
     logging.debug("Exiting with code %s", return_code)
     exit(return_code)
 
 
+# this should be modified before publish, but if someone cloned from the repo,
+# it can help
+__version__ = get_version()
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `slidge-0.1.0rc1/slidge/core/chat_command.py` & `slidge-0.1.1/slidge/util/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,197 +1,206 @@
-import asyncio
 import logging
-from typing import TYPE_CHECKING, Optional
-
-from slixmpp import Message
-from slixmpp.exceptions import XMPPError
-
-from ..util.db import GatewayUser
-from ..util.types import SessionType
-from . import config
-from .adhoc import RegistrationType, TwoFactorNotRequired
-
-if TYPE_CHECKING:
-    from .gateway import BaseGateway
-
-
-class ChatCommandProvider:
-    def __init__(self, xmpp: "BaseGateway"):
-        self.xmpp = xmpp
-
-    async def _chat_command_search(
-        self, *args, msg: Message, session: Optional["SessionType"] = None
-    ):
-        if session is None:
-            msg.reply("Register to the gateway first!")
-            return
-
-        search_form = {}
-        diff = len(args) - len(self.xmpp.SEARCH_FIELDS)
-
-        if diff > 0:
-            session.send_gateway_message("Too many parameters!")
-            return
-
-        for field, arg in zip(self.xmpp.SEARCH_FIELDS, args):
-            search_form[field.var] = arg
-
-        if diff < 0:
-            for field in self.xmpp.SEARCH_FIELDS[diff:]:
-                if not field.required:
-                    continue
-                search_form[field.var] = await session.input(
-                    (field.label or field.var) + "?"
-                )
-
-        results = await session.search(search_form)
-        if results is None:
-            session.send_gateway_message("No results!")
-            return
-
-        result_fields = results.fields
-        for result in results.items:
-            text = ""
-            for f in result_fields:
-                if f.type == "jid-single":
-                    text += f"xmpp:{result[f.var]}\n"
-                else:
-                    text += f"{f.label}: {result[f.var]}\n"
-            session.send_gateway_message(text)
+from functools import cached_property
+from types import GenericAlias
+from typing import Optional, Union, get_args, get_origin, get_type_hints
+
+import configargparse
+
+
+class Option:
+    DOC_SUFFIX = "__DOC"
+    DYNAMIC_DEFAULT_SUFFIX = "__DYNAMIC_DEFAULT"
+    SHORT_SUFFIX = "__SHORT"
+
+    def __init__(self, parent: "ConfigModule", name: str):
+        self.parent = parent
+        self.config_obj = parent.config_obj
+        self.name = name
+
+    @cached_property
+    def doc(self):
+        return getattr(self.config_obj, self.name + self.DOC_SUFFIX)
+
+    @cached_property
+    def required(self):
+        return not hasattr(
+            self.config_obj, self.name + self.DYNAMIC_DEFAULT_SUFFIX
+        ) and not hasattr(self.config_obj, self.name)
+
+    @cached_property
+    def default(self):
+        return getattr(self.config_obj, self.name, None)
+
+    @cached_property
+    def short(self):
+        return getattr(self.config_obj, self.name + self.SHORT_SUFFIX, None)
+
+    @cached_property
+    def nargs(self):
+        type_ = get_type_hints(self.config_obj).get(self.name, type(self.default))
+
+        if isinstance(type_, GenericAlias):
+            args = get_args(type_)
+            if args[1] is Ellipsis:
+                return "*"
+            else:
+                return len(args)
 
-    async def _chat_command_help(
-        self, *_args, msg: Message, session: Optional["SessionType"]
-    ):
-        if session is None:
-            msg.reply("Register to the gateway first!").send()
-        else:
-            t = "|".join(
-                x
-                for x in self.xmpp._chat_commands.keys()
-                if x not in ("register", "help")
-            )
-            log.debug("In help: %s", t)
-            msg.reply(f"Available commands: {t}").send()
-
-    @staticmethod
-    async def _chat_command_list_contacts(
-        *_args, msg: Message, session: Optional["SessionType"]
-    ):
-        if session is None:
-            msg.reply("Register to the gateway first!").send()
+    @cached_property
+    def type(self):
+        type_ = get_type_hints(self.config_obj).get(self.name, type(self.default))
+
+        if _is_optional(type_):
+            type_ = get_args(type_)[0]
+        elif isinstance(type_, GenericAlias):
+            args = get_args(type_)
+            type_ = args[0]
+
+        return type_
+
+    @cached_property
+    def names(self):
+        res = ["--" + self.name.lower().replace("_", "-")]
+        if s := self.short:
+            res.append("-" + s)
+        return res
+
+    @cached_property
+    def kwargs(self):
+        kwargs = dict(
+            required=self.required,
+            help=self.doc,
+            env_var=self.name_to_env_var(),
+        )
+        t = self.type
+        if t is bool:
+            if self.default:
+                kwargs["action"] = "store_false"
+            else:
+                kwargs["action"] = "store_true"
         else:
-            contacts = sorted(
-                session.contacts, key=lambda c: c.name.casefold() if c.name else ""
-            )
-            t = "\n".join(f"{c.name}: xmpp:{c.jid.bare}" for c in contacts)
-            msg.reply(t).send()
-
-    async def _chat_command_register(
-        self, *args, msg: Message, session: Optional["SessionType"]
-    ):
-        if session is not None:
-            msg.reply("You are already registered to this gateway").send()
-            return
-
-        jid = msg.get_from()
-
-        if not self.xmpp.jid_validator.match(jid.bare):  # type:ignore
-            msg.reply("You are not allowed to register to this gateway").send()
-            return
-
-        msg.reply(self.xmpp.REGISTRATION_INSTRUCTIONS).send()
-        form: dict[str, Optional[str]] = {}
-        for field in self.xmpp.REGISTRATION_FIELDS:
-            text = field.label or field.var
-            if field.value != "":
-                text += f" (default: '{field.value}')"
-            if not field.required:
-                text += " (optional, reply with '.' to skip)"
-            if (options := field.options) is not None:
-                for option in options:
-                    label = option["label"]
-                    value = option["value"]
-                    text += f"\n{label}: reply with '{value}'"
-
-            while True:
-                ans = await self.xmpp.input(jid, text + "?")
-                if ans == "." and not field.required:
-                    form[field.var] = None
-                    break
+            kwargs["type"] = t
+            if self.required:
+                kwargs["required"] = True
+            else:
+                kwargs["default"] = self.default
+        if n := self.nargs:
+            kwargs["nargs"] = n
+        return kwargs
+
+    def name_to_env_var(self):
+        return self.parent.ENV_VAR_PREFIX + self.name
+
+
+class ConfigModule:
+    ENV_VAR_PREFIX = "SLIDGE_"
+
+    def __init__(
+        self, config_obj, parser: Optional[configargparse.ArgumentParser] = None
+    ):
+        self.config_obj = config_obj
+        if parser is None:
+            parser = configargparse.ArgumentParser()
+        self.parser = parser
+
+        self.add_options_to_parser()
+
+    def _list_options(self):
+        return {
+            o
+            for o in (set(dir(self.config_obj)) | set(get_type_hints(self.config_obj)))
+            if o.upper() == o and not o.startswith("_") and "__" not in o
+        }
+
+    def set_conf(self, argv: Optional[list[str]] = None):
+        if argv is not None:
+            # this is ugly, but necessary because for plugin config, we used
+            # remaining argv.
+            # when using (a) .ini file(s), for bool options, we end-up with
+            # remaining pseudo-argv such as --some-bool-opt=true when we really
+            # should have just --some-bool-opt
+            # TODO: get rid of configargparse and make this cleaner
+            options_long = {o.name: o for o in self.options}
+            no_explicit_bool = []
+            skip_next = False
+            for a, aa in zip(argv, argv[1:] + [""]):
+                if skip_next:
+                    skip_next = False
+                    continue
+                force_keep = False
+                if "=" in a:
+                    real_name, _value = a.split("=")
+                    opt: Optional[Option] = options_long.get(
+                        _argv_to_option_name(real_name)
+                    )
+                    if opt and opt.type is bool:
+                        if opt.default:
+                            if _value in _TRUEISH or not _value:
+                                continue
+                            else:
+                                a = real_name
+                                force_keep = True
+                        else:
+                            if _value in _TRUEISH:
+                                a = real_name
+                                force_keep = True
+                            else:
+                                continue
                 else:
-                    if (options := field.options) is not None:
-                        valid_choices = [x["value"] for x in options]
-                        if ans not in valid_choices:
-                            continue
-                    form[field.var] = ans
-                    break
-
-        user = GatewayUser(bare_jid=jid.bare, registration_form=form)
-
-        try:
-            two_fa_needed = True
-            try:
-                await self.xmpp.user_prevalidate(jid, form)
-            except TwoFactorNotRequired:
-                if self.xmpp.REGISTRATION_TYPE == RegistrationType.TWO_FACTOR_CODE:
-                    two_fa_needed = False
+                    upper = _argv_to_option_name(a)
+                    opt = options_long.get(upper)
+                    if opt and opt.type is bool:
+                        if _argv_to_option_name(aa) not in options_long:
+                            log.debug("Removing %s from argv", aa)
+                            skip_next = True
+
+                if opt:
+                    if opt.type is bool:
+                        if force_keep or not opt.default:
+                            no_explicit_bool.append(a)
+                    else:
+                        no_explicit_bool.append(a)
                 else:
-                    raise
+                    no_explicit_bool.append(a)
+            log.debug("Removed boolean values from %s to %s", argv, no_explicit_bool)
+            argv = no_explicit_bool
+
+        args, rest = self.parser.parse_known_args(argv)
+        self.update_dynamic_defaults(args)
+        for name in self._list_options():
+            value = getattr(args, name.lower())
+            log.debug("Setting '%s' to %r", name, value)
+            setattr(self.config_obj, name, value)
+        return args, rest
+
+    @cached_property
+    def options(self) -> list[Option]:
+        res = []
+        for opt in self._list_options():
+            res.append(Option(self, opt))
+        return res
+
+    def add_options_to_parser(self):
+        p = self.parser
+        for o in sorted(self.options, key=lambda x: (not x.required, x.name)):
+            p.add_argument(*o.names, **o.kwargs)
+
+    def update_dynamic_defaults(self, args):
+        pass
+
+
+def _is_optional(t):
+    if get_origin(t) is Union:
+        args = get_args(t)
+        if len(args) == 2 and isinstance(None, args[1]):
+            return True
+    return False
 
-            if self.xmpp.REGISTRATION_TYPE == RegistrationType.TWO_FACTOR_CODE:
-                if two_fa_needed:
-                    code = await self.xmpp.input(
-                        jid,
-                        self.xmpp.REGISTRATION_2FA_TITLE
-                        + "\n"
-                        + self.xmpp.REGISTRATION_2FA_INSTRUCTIONS,
-                    )
-                    await self.xmpp.validate_two_factor_code(user, code)
 
-            elif self.xmpp.REGISTRATION_TYPE == RegistrationType.QRCODE:
-                fut = self.xmpp.loop.create_future()
-                self.xmpp.qr_pending_registrations[user.bare_jid] = fut  # type:ignore
-                qr_url = await self.xmpp.get_qr_text(user)
-                self.xmpp.send_message(
-                    mto=jid, mbody=qr_url, mfrom=self.xmpp.boundjid.bare
-                )
-                await self.xmpp.send_qr(qr_url, mto=jid)
-                try:
-                    await asyncio.wait_for(fut, config.QR_TIMEOUT)
-                except asyncio.TimeoutError:
-                    msg.reply(f"You did not flash the QR code in time!").send()
-                    return
+def _argv_to_option_name(arg: str):
+    return arg.upper().removeprefix("--").replace("-", "_")
 
-        except (ValueError, XMPPError) as e:
-            msg.reply(f"Something went wrong: {e}").send()
 
-        else:
-            user.commit()
-            self.xmpp.event("user_register", msg)
-            msg.reply(f"Success!").send()
-
-    async def _chat_command_unregister(
-        self, *args, msg: Message, session: Optional["SessionType"]
-    ):
-        ifrom = msg.get_from()
-        await self.xmpp.plugin["xep_0077"].api["user_remove"](None, None, ifrom)
-        await self.xmpp.session_cls.kill_by_jid(ifrom)
-
-    @staticmethod
-    async def _chat_command_list_groups(
-        *_args, msg: Message, session: Optional["SessionType"]
-    ):
-        if session is None:
-            msg.reply("Register to the gateway first!").send()
-        else:
-            groups = sorted(
-                session.bookmarks,
-                key=lambda m: m.DISCO_NAME.casefold() if m.DISCO_NAME else "",
-            )
-            if groups:
-                t = "\n".join(f"{m.DISCO_NAME}: xmpp:{m.jid}?join" for m in groups)
-                msg.reply(t).send()
-            else:
-                msg.reply("No groups!").send()
+_TRUEISH = {"true", "True", "1", "on", "enabled"}
 
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/core/contact.py` & `slidge-0.1.1/slidge/group/participant.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,441 +1,458 @@
 import logging
-from datetime import date, datetime
-from typing import Any, Generic, Optional, Type, Union
-
-from slixmpp import JID, Message, Presence
-from slixmpp.jid import JID_UNESCAPE_TRANSFORMATIONS, _unescape_node
-
-from ..util import SubclassableOnce
+import string
+import stringprep
+import uuid
+import warnings
+from copy import copy
+from datetime import datetime
+from functools import cached_property
+from typing import TYPE_CHECKING, Optional, Union
+
+from slixmpp import JID, InvalidJID, Message, Presence
+from slixmpp.plugins.xep_0045.stanza import MUCAdminItem
+from slixmpp.stringprep import StringprepError, resourceprep
+from slixmpp.types import MessageTypes, OptJid
+from slixmpp.util.stringprep_profiles import StringPrepError, prohibit_output
+
+from ..contact import LegacyContact
+from ..core.mixins import ChatterDiscoMixin, MessageMixin, PresenceMixin
+from ..util import SubclassableOnce, strip_illegal_chars
+from ..util.sql import CachedPresence
 from ..util.types import (
-    AvatarType,
-    LegacyContactType,
+    Hat,
     LegacyMessageType,
-    LegacyUserIdType,
-    SessionType,
+    MessageOrPresenceTypeVar,
+    MucAffiliation,
+    MucRole,
 )
-from ..util.xep_0292.stanza import VCard4
-from . import config
-from .mixins import FullCarbonMixin
-from .mixins.base import ReactionRecipientMixin
 
+if TYPE_CHECKING:
+    from .room import LegacyMUC
 
-class LegacyContact(
-    Generic[SessionType, LegacyUserIdType],
-    FullCarbonMixin,
-    ReactionRecipientMixin,
+
+def strip_non_printable(nickname: str):
+    new = (
+        "".join(x for x in nickname if x in string.printable)
+        + f"-slidge-{hash(nickname)}"
+    )
+    warnings.warn(f"Could not use {nickname} as a nickname, using {new}")
+    return new
+
+
+class LegacyParticipant(
+    PresenceMixin,
+    MessageMixin,
+    ChatterDiscoMixin,
     metaclass=SubclassableOnce,
 ):
     """
-    This class centralizes actions in relation to a specific legacy contact.
-
-    You shouldn't create instances of contacts manually, but rather rely on
-    :meth:`.LegacyRoster.by_legacy_id` to ensure that contact instances are
-    singletons. The :class:`.LegacyRoster` instance of a session is accessible
-    through the :attr:`.BaseSession.contacts` attribute.
-
-    Typically, your plugin should have methods hook to the legacy events and
-    call appropriate methods here to transmit the "legacy action" to the xmpp
-    user. This should look like this:
-
-    .. code-block:python
-
-        class Session(BaseSession):
-            ...
-
-            async def on_cool_chat_network_new_text_message(self, legacy_msg_event):
-                contact = self.contacts.by_legacy_id(legacy_msg_event.from)
-                contact.send_text(legacy_msg_event.text)
-
-            async def on_cool_chat_network_new_typing_event(self, legacy_typing_event):
-                contact = self.contacts.by_legacy_id(legacy_msg_event.from)
-                contact.composing()
-            ...
-
-    Use ``carbon=True`` as a keyword arg for methods to represent an action FROM
-    the user TO the contact, typically when the user uses an official client to
-    do an action such as sending a message or marking as message as read.
-    This will use :xep:`0363` to impersonate the XMPP user in order.
+    A legacy participant of a legacy group chat.
     """
 
-    session: "SessionType"
-
-    RESOURCE: str = "slidge"
-    """
-    A full JID, including a resource part is required for chat states (and maybe other stuff)
-    to work properly. This is the name of the resource the contacts will use.
-    """
-
-    mtype = "chat"
-    is_group = False
+    mtype: MessageTypes = "groupchat"
+    _can_send_carbon = False
+    USE_STANZA_ID = True
+    STRIP_SHORT_DELAY = False
 
     def __init__(
         self,
-        session: "SessionType",
-        legacy_id: LegacyUserIdType,
-        jid_username: str,
+        muc: "LegacyMUC",
+        nickname: Optional[str] = None,
+        is_user=False,
+        is_system=False,
+        role: MucRole = "participant",
+        affiliation: MucAffiliation = "member",
     ):
-        """
-        :param session: The session this contact is part of
-        :param legacy_id: The contact's legacy ID
-        :param jid_username: User part of this contact's 'puppet' JID.
-            NB: case-insensitive, and some special characters are not allowed
-        """
-        self.session = session
+        super().__init__()
+        self._hats = list[Hat]()
+        self.muc = muc
+        self.session = session = muc.session
         self.user = session.user
-        self.legacy_id = legacy_id
-        self.jid_username = jid_username
-
-        self.added_to_roster = False
-
-        self._name: Optional[str] = None
-        self._avatar: Optional[AvatarType] = None
-
-        self._subscribe_from = True
-        self._subscribe_to = True
-
-        if self.xmpp.MARK_ALL_MESSAGES:
-            self._sent_order = list[str]()
-
         self.xmpp = session.xmpp
-        self.jid = JID(self.jid_username + "@" + self.xmpp.boundjid.bare)
-        self.jid.resource = self.RESOURCE
+        self._role = role
+        self._affiliation = affiliation
+        self.is_user: bool = is_user
+        self.is_system: bool = is_system
+
+        self._nickname = nickname
+
+        self.__update_jid(nickname)
+        log.debug("Instantiation of: %r", self)
+
+        self.contact: Optional["LegacyContact"] = None
+        # we track if we already sent a presence for this participant.
+        # if we didn't, we send it before the first message.
+        # this way, event in plugins that don't map "user has joined" events,
+        # we send a "join"-presence from the participant before the first message
+        self.__presence_sent = False
+        self.log = logging.getLogger(f"{self.user.bare_jid}:{self.jid}")
 
     def __repr__(self):
-        return f"<LegacyContact <{self.jid}> ('{self.legacy_id}') of <{self.user}>"
-
-    def __get_subscription_string(self):
-        if self._subscribe_from and self._subscribe_to:
-            return "both"
-        if self._subscribe_from:
-            return "from"
-        if self._subscribe_to:
-            return "to"
-        return "none"
-
-    def _send(self, stanza: Union[Message, Presence], carbon=False, **send_kwargs):
-        if carbon and isinstance(stanza, Message):
-            stanza["to"] = self.jid.bare
-            stanza["from"] = self.user.jid
-            self._privileged_send(stanza)
-        else:
-            if self.xmpp.MARK_ALL_MESSAGES and is_markable(stanza):
-                self._sent_order.append(stanza["id"])
-            stanza["to"] = self.user.jid
-            stanza.send()
-
-    def get_msg_xmpp_id_up_to(self, horizon_xmpp_id: str):
-        """
-        Return XMPP msg ids sent by this contact up to a given XMPP msg id.
+        return f"<Participant '{self.nickname}'/'{self.jid}' of '{self.muc}'>"
 
-        Plugins have no reason to use this, but it is used by slidge core
-        for legacy networks that need to mark all messages as read (most XMPP
-        clients only send a read marker for the latest message.
-
-        This has side effects, if the horizon XMPP id is found, messages up to
-        this horizon are not cleared, to avoid sending the same read mark twice.
+    @property
+    def affiliation(self):
+        return self._affiliation
 
-        :param horizon_xmpp_id: The latest message
-        :return: A list of XMPP ids or None if horizon_xmpp_id was not found
-        """
-        for i, xmpp_id in enumerate(self._sent_order):
-            if xmpp_id == horizon_xmpp_id:
-                break
-        else:
+    @affiliation.setter
+    def affiliation(self, affiliation: MucAffiliation):
+        if self._affiliation == affiliation:
             return
-        i += 1
-        res = self._sent_order[:i]
-        self._sent_order = self._sent_order[i:]
-        return res
-
-    def send_text(
-        self,
-        body: str,
-        legacy_msg_id: Optional[LegacyMessageType] = None,
-        *,
-        when: Optional[datetime] = None,
-        reply_to_msg_id: Optional[LegacyMessageType] = None,
-        reply_to_fallback_text: Optional[str] = None,
-        reply_self=False,
-        **kwargs,
-    ):
-        """
-        The contact sends a message to the user.
+        self._affiliation = affiliation
+        if not self.__presence_sent:
+            return
+        self.send_last_presence(force=True, no_cache_online=True)
 
-        :param body:
-        :param legacy_msg_id:
-        :param when:
-        :param reply_to_msg_id: Quote another message (:xep:`0461`)
-        :param reply_to_fallback_text: Fallback text for clients not supporting :xep:`0461`
-        :param reply_self: Set to true is this is a self quote. If False, it means the
-            quoted author is the gateway user.
-        """
-        super().send_text(
-            body=body,
-            legacy_msg_id=legacy_msg_id,
-            when=when,
-            reply_to_msg_id=reply_to_msg_id,
-            reply_to_fallback_text=reply_to_fallback_text,
-            reply_to_jid=self.jid if reply_self else self.user.jid,
-            **kwargs,
-        )
+    def send_affiliation_change(self):
+        # internal use by slidge
+        msg = self._make_message()
+        msg["muc"]["affiliation"] = self._affiliation
+        msg["type"] = "normal"
+        if not self.muc.is_anonymous:
+            if self.contact:
+                msg["muc"]["jid"] = self.contact.jid
+            else:
+                warnings.warn(
+                    f"Private group but no 1:1 JID associated to '{self}'",
+                )
+        self._send(msg)
 
     @property
-    def name(self):
-        """
-        Friendly name of the contact, as it should appear in the user's roster
-        """
-        return self._name
+    def role(self):
+        return self._role
 
-    @name.setter
-    def name(self, n: Optional[str]):
-        if self._name == n:
+    @role.setter
+    def role(self, role: MucRole):
+        if self._role == role:
             return
-        self._name = n
-        self.xmpp.pubsub.set_nick(
-            jid=self.jid.bare, nick=n, restrict_to=self.user.jid.bare
-        )
+        self._role = role
+        if not self.__presence_sent:
+            return
+        self.send_last_presence(force=True, no_cache_online=True)
 
-    @property
-    def avatar(self):
-        """
-        An image that represents this contact
-        """
-        return self._avatar
+    def set_hats(self, hats: list[Hat]):
+        if self._hats == hats:
+            return
+        self._hats = hats
+        if not self.__presence_sent:
+            return
+        self.send_last_presence(force=True, no_cache_online=True)
+
+    def __update_jid(self, unescaped_nickname: Optional[str]):
+        j: JID = copy(self.muc.jid)
 
-    @avatar.setter
-    def avatar(self, a: Optional[AvatarType]):
-        if a == self._avatar:
+        if self.is_system:
+            self.jid = j
             return
-        self.xmpp.loop.create_task(
-            self.xmpp.pubsub.set_avatar(
-                jid=self.jid.bare, avatar=a, restrict_to=self.user.jid.bare
-            )
-        )
-        self._avatar = a
 
-    def set_vcard(
-        self,
-        /,
-        full_name: Optional[str] = None,
-        given: Optional[str] = None,
-        surname: Optional[str] = None,
-        birthday: Optional[date] = None,
-        phone: Optional[str] = None,
-        note: Optional[str] = None,
-        url: Optional[str] = None,
-        email: Optional[str] = None,
-        country: Optional[str] = None,
-        locality: Optional[str] = None,
-    ):
-        vcard = VCard4()
-        vcard.add_impp(f"xmpp:{self.jid.bare}")
+        nickname = unescaped_nickname
 
-        if n := self.name:
-            vcard.add_nickname(n)
-        if full_name:
-            vcard["full_name"] = full_name
-        elif n:
-            vcard["full_name"] = n
-
-        if given:
-            vcard["given"] = given
-        if surname:
-            vcard["surname"] = surname
-        if birthday:
-            vcard["birthday"] = birthday
-
-        if note:
-            vcard.add_note(note)
-        if url:
-            vcard.add_url(url)
-        if email:
-            vcard.add_email(email)
-        if phone:
-            vcard.add_tel(phone)
-        if country and locality:
-            vcard.add_address(country, locality)
-        elif country:
-            vcard.add_address(country, locality)
+        if nickname:
+            nickname = self._nickname_no_illegal = strip_illegal_chars(nickname)
+        else:
+            warnings.warn(
+                "Only the system participant is allowed to not have a nickname"
+            )
+            nickname = f"unnamed-{uuid.uuid4()}"
 
-        self.xmpp.vcard.set_vcard(self.jid.bare, vcard, {self.user.jid.bare})
+        assert isinstance(nickname, str)
 
-    async def add_to_roster(self):
-        """
-        Add this contact to the user roster using :xep:`0356`
-        """
-        if config.NO_ROSTER_PUSH:
-            log.debug("Roster push request by plugin ignored (--no-roster-push)")
-            return
-        item = {
-            "subscription": self.__get_subscription_string(),
-            "groups": [self.xmpp.ROSTER_GROUP],
-        }
-        if (n := self.name) is not None:
-            item["name"] = n
-        kw = dict(
-            jid=self.user.jid,
-            roster_items={self.jid.bare: item},
-        )
         try:
-            await self.xmpp["xep_0356"].set_roster(**kw)
-        except PermissionError:
-            try:
-                await self.xmpp["xep_0356_old"].set_roster(**kw)
-            except PermissionError:
-                log.warning(
-                    "Slidge does not have privileges to add contacts to the roster."
-                    "Refer to https://slidge.readthedocs.io/en/latest/admin/xmpp_server.html "
-                    "for more info."
-                )
-                if config.ROSTER_PUSH_PRESENCE_SUBSCRIPTION_REQUEST_FALLBACK:
-                    self._send(self._make_presence(ptype="subscribe"))
-                return
+            # workaround for https://codeberg.org/poezio/slixmpp/issues/3480
+            prohibit_output(nickname, [stringprep.in_table_a1])
+            resourceprep(nickname)
+        except (StringPrepError, StringprepError):
+            nickname = nickname.encode("punycode").decode()
 
-        self.added_to_roster = True
-        self._send_last_presence()
+        # at this point there still might be control chars
+        try:
+            j.resource = nickname
+        except InvalidJID:
+            j.resource = strip_non_printable(nickname)
+
+        if nickname != unescaped_nickname:
+            self.muc._participants_by_escaped_nicknames[nickname] = self  # type:ignore
+
+        self.jid = j
+
+    def send_configuration_change(self, codes: tuple[int]):
+        if not self.is_system:
+            raise RuntimeError("This is only possible for the system participant")
+        msg = self._make_message()
+        msg["muc"]["status_codes"] = codes
+        self._send(msg)
 
-    def unsubscribe(self):
-        """
-        Send an "unsubscribe", "unsubscribed", "unavailable" presence sequence
-        from this contact to the user, ie, "this contact has removed you from
-        their 'friends'".
-        """
-        for ptype in "unsubscribe", "unsubscribed", "unavailable":
-            self.xmpp.send_presence(pfrom=self.jid, pto=self.user.jid.bare, ptype=ptype)  # type: ignore
+    @property
+    def nickname(self):
+        return self._nickname
 
+    @nickname.setter
+    def nickname(self, new_nickname: str):
+        old = self._nickname
+        if new_nickname == old:
+            return
 
-class LegacyRoster(
-    Generic[SessionType, LegacyContactType, LegacyUserIdType],
-    metaclass=SubclassableOnce,
-):
-    """
-    Virtual roster of a gateway user, that allows to represent all
-    of their contacts as singleton instances (if used properly and not too bugged).
+        cache = getattr(self, "_last_presence", None)
+        if cache:
+            last_seen = cache.last_seen
+            kwargs = cache.presence_kwargs
+        else:
+            last_seen = None
+            kwargs = {}
 
-    Every :class:`.BaseSession` instance will have its own :class:`.LegacyRoster` instance
-    accessible via the :attr:`.BaseSession.contacts` attribute.
+        kwargs["status_codes"] = {303}
 
-    Typically, you will mostly use the :meth:`.LegacyRoster.by_legacy_id` function to
-    retrieve a contact instance.
+        p = self._make_presence(ptype="unavailable", last_seen=last_seen, **kwargs)
+        # in this order so pfrom=old resource and we actually use the escaped nick
+        # in the muc/item/nick element
+        self.__update_jid(new_nickname)
+        p["muc"]["item"]["nick"] = self.jid.resource
+        self._send(p)
 
-    You might need to override :meth:`.LegacyRoster.legacy_id_to_jid_username` and/or
-    :meth:`.LegacyRoster.jid_username_to_legacy_id` to incorporate some custom logic
-    if you need some characters when translation JID user parts and legacy IDs.
-    """
+        self._nickname = new_nickname
 
-    def __init__(self, session: "SessionType"):
-        self._contact_cls: Type[
-            LegacyContactType
-        ] = LegacyContact.get_self_or_unique_subclass()
-        self._contact_cls.xmpp = session.xmpp
-
-        self.session = session
-        self._contacts_by_bare_jid: dict[str, LegacyContactType] = {}
-        self._contacts_by_legacy_id: dict[LegacyUserIdType, LegacyContactType] = {}
+        kwargs["status_codes"] = set()
+        p = self._make_presence(ptype="available", last_seen=last_seen, **kwargs)
+        self.__add_nick_element(p)
+        self._send(p)
 
-    def __iter__(self):
-        return iter(self._contacts_by_legacy_id.values())
+        if old:
+            self.muc.rename_participant(old, new_nickname)
 
-    def known_contacts(self):
-        return self._contacts_by_bare_jid.copy()
+    def _make_presence(
+        self,
+        *,
+        last_seen: Optional[datetime] = None,
+        status_codes: Optional[set[int]] = None,
+        user_full_jid: Optional[JID] = None,
+        **presence_kwargs,
+    ):
+        p = super()._make_presence(last_seen=last_seen, **presence_kwargs)
+        p["muc"]["affiliation"] = self.affiliation
+        p["muc"]["role"] = self.role
+        if self._hats:
+            p["hats"].add_hats(self._hats)
+        codes = status_codes or set()
+        if self.is_user:
+            codes.add(110)
+        if not self.muc.is_anonymous:
+            if self.is_user:
+                if user_full_jid:
+                    p["muc"]["jid"] = user_full_jid
+                else:
+                    jid = copy(self.user.jid)
+                    try:
+                        jid.resource = next(
+                            iter(self.muc.user_resources)  # type:ignore
+                        )
+                    except StopIteration:
+                        jid.resource = "pseudo-resource"
+                    p["muc"]["jid"] = self.user.jid
+                codes.add(100)
+            elif self.contact:
+                p["muc"]["jid"] = self.contact.jid
+                if a := self.contact.get_avatar():
+                    p["vcard_temp_update"]["photo"] = a.id
+            else:
+                warnings.warn(
+                    f"Private group but no 1:1 JID associated to '{self}'",
+                )
+        if self.is_user and (hash_ := self.session.avatar_hash):
+            p["vcard_temp_update"]["photo"] = hash_
+        p["muc"]["status_codes"] = codes
+        return p
 
-    async def by_jid(self, contact_jid: JID) -> LegacyContactType:
-        """
-        Retrieve a contact by their JID
+    @property
+    def DISCO_NAME(self):
+        return self.nickname
 
-        If the contact was not instantiated before, it will be created
-        using :meth:`slidge.LegacyRoster.jid_username_to_legacy_id` to infer their
-        legacy user ID.
+    def __send_presence_if_needed(
+        self, stanza: Union[Message, Presence], full_jid: JID, archive_only: bool
+    ):
+        if (
+            archive_only
+            or self.is_system
+            or self.is_user
+            or self.__presence_sent
+            or stanza["subject"]
+        ):
+            return
+        if isinstance(stanza, Message):
+            if stanza.get_plugin("muc", check=True):
+                return
+            self.send_initial_presence(full_jid)
 
-        :param contact_jid:
-        :return:
-        """
-        bare = contact_jid.bare
-        c = self._contacts_by_bare_jid.get(bare)
-        if c is None:
-            jid_username = str(contact_jid.username)
-            log.debug("Contact %s not found", contact_jid)
-            c = self._contact_cls(
-                self.session,
-                await self.jid_username_to_legacy_id(jid_username),
-                jid_username,
-            )
-            await c.update_caps()
-            self._contacts_by_legacy_id[c.legacy_id] = self._contacts_by_bare_jid[
-                bare
-            ] = c
-        return c
+    @cached_property
+    def __occupant_id(self):
+        if self.contact:
+            return self.contact.jid
+        elif self.is_user:
+            return "slidge-user"
+        elif self.is_system:
+            return "room"
+        else:
+            return str(uuid.uuid4())
 
-    async def by_legacy_id(self, legacy_id: Any) -> LegacyContactType:
-        """
-        Retrieve a contact by their legacy_id
+    def _send(
+        self,
+        stanza: MessageOrPresenceTypeVar,
+        full_jid: Optional[JID] = None,
+        archive_only=False,
+        **send_kwargs,
+    ) -> MessageOrPresenceTypeVar:
+        stanza["occupant-id"]["id"] = self.__occupant_id
+        if isinstance(stanza, Presence):
+            if stanza["type"] == "unavailable" and not self.__presence_sent:
+                return stanza  # type:ignore
+            self.__presence_sent = True
+        if full_jid:
+            stanza["to"] = full_jid
+            self.__send_presence_if_needed(stanza, full_jid, archive_only)
+            if self.is_user:
+                assert stanza.stream is not None
+                stanza.stream.send(stanza, use_filters=False)
+            else:
+                stanza.send()
+        else:
+            if isinstance(stanza, Message):
+                self.muc.archive.add(stanza, self)
+            if archive_only:
+                return stanza
+            for user_full_jid in self.muc.user_full_jids():
+                stanza = copy(stanza)
+                stanza["to"] = user_full_jid
+                self.__send_presence_if_needed(stanza, user_full_jid, archive_only)
+                stanza.send()
+        return stanza
+
+    def mucadmin_item(self):
+        item = MUCAdminItem()
+        item["nick"] = self.nickname
+        item["affiliation"] = self.affiliation
+        item["role"] = self.role
+        if not self.muc.is_anonymous:
+            if self.is_user:
+                item["jid"] = self.user.bare_jid
+            elif self.contact:
+                item["jid"] = self.contact.jid.bare
+            else:
+                warnings.warn(
+                    (
+                        f"Public group but no contact JID associated to {self.jid} in"
+                        f" {self}"
+                    ),
+                )
+        return item
 
-        If the contact was not instantiated before, it will be created
-        using :meth:`slidge.LegacyRoster.legacy_id_to_jid_username` to infer their
-        legacy user ID.
+    def __add_nick_element(self, p: Presence):
+        if (nick := self._nickname_no_illegal) != self.jid.resource:
+            n = self.xmpp.plugin["xep_0172"].stanza.UserNick()
+            n["nick"] = nick
+            p.append(n)
+
+    def _get_last_presence(self) -> Optional[CachedPresence]:
+        own = super()._get_last_presence()
+        if own is None and self.contact:
+            return self.contact._get_last_presence()
+        return own
 
-        :param legacy_id:
-        :return:
+    def send_initial_presence(
+        self,
+        full_jid: JID,
+        nick_change=False,
+        presence_id: Optional[str] = None,
+    ):
         """
-        c = self._contacts_by_legacy_id.get(legacy_id)
-        if c is None:
-            log.debug("Contact %s not found in roster", legacy_id)
-            c = self._contact_cls(
-                self.session, legacy_id, await self.legacy_id_to_jid_username(legacy_id)
-            )
-            await c.update_caps()
-            self._contacts_by_bare_jid[c.jid.bare] = self._contacts_by_legacy_id[
-                legacy_id
-            ] = c
-        return c
+        Called when the user joins a MUC, as a mechanism
+        to indicate to the joining XMPP client the list of "participants".
 
-    async def by_stanza(self, s) -> LegacyContactType:
-        """
-        Retrieve a contact by the destination of a stanza
+        Can be called this to trigger a "participant has joined the group" event.
 
-        See :meth:`slidge.Roster.by_legacy_id` for more info.
+        :param full_jid: Set this to only send to a specific user XMPP resource.
+        :param nick_change: Used when the user joins and the MUC renames them (code 210)
+        :param presence_id: set the presence ID. used internally by slidge
+        """
+        #  MUC status codes: https://xmpp.org/extensions/xep-0045.html#registrar-statuscodes
+        codes = set()
+        if nick_change:
+            codes.add(210)
+
+        if self.is_user:
+            # the "initial presence" of the user has to be vanilla, as it is
+            # a crucial part of the MUC join sequence for XMPP clients.
+            kwargs = {}
+        else:
+            cache = self._get_last_presence()
+            self.log.debug("Join muc, initial presence: %s", cache)
+            if cache:
+                ptype = cache.ptype
+                if ptype == "unavailable":
+                    return
+                kwargs = dict(
+                    last_seen=cache.last_seen, pstatus=cache.pstatus, pshow=cache.pshow
+                )
+            else:
+                kwargs = {}
+        p = self._make_presence(
+            status_codes=codes,
+            user_full_jid=full_jid,
+            **kwargs,  # type:ignore
+        )
+        if presence_id:
+            p["id"] = presence_id
+        self.__add_nick_element(p)
+        self._send(p, full_jid)
 
-        :param s:
-        :return:
+    def leave(self):
         """
-        return await self.by_jid(s.get_to())
-
-    async def legacy_id_to_jid_username(self, legacy_id: Any) -> str:
+        Call this when the participant leaves the room
         """
-        Convert a legacy ID to a valid 'user' part of a JID
+        self.muc.remove_participant(self)
 
-        Should be overridden for cases where the str conversion of
-        the legacy_id is not enough, e.g., if it is case-sensitive or contains
-        forbidden characters not covered by :xep:`0106`.
-
-        :param legacy_id:
+    def kick(self):
         """
-        return str(legacy_id).translate(ESCAPE_TABLE)
-
-    async def jid_username_to_legacy_id(self, jid_username: str) -> LegacyUserIdType:
+        Call this when the participant is kicked from the room
         """
-        Convert a JID user part to a legacy ID.
-
-        Should be overridden in case legacy IDs are not strings, or more generally
-        for any case where the username part of a JID (unescaped with to the mapping
-        defined by :xep:`0106`) is not enough to identify a contact on the legacy network.
+        self.muc.remove_participant(self, kick=True)
 
-        Default implementation is an identity operation
-
-        :param jid_username: User part of a JID, ie "user" in "user@example.com"
-        :return: An identifier for the user on the legacy network.
+    def ban(self):
+        """
+        Call this when the participant is banned from the room
         """
-        return _unescape_node(jid_username)
+        self.muc.remove_participant(self, ban=True)
 
+    def get_disco_info(self, jid: OptJid = None, node: Optional[str] = None):
+        if self.contact is not None:
+            return self.contact.get_disco_info()
+        return super().get_disco_info()
 
-def is_markable(stanza: Union[Message, Presence]):
-    if isinstance(stanza, Presence):
-        return False
-    return bool(stanza["body"])
+    def moderate(self, legacy_msg_id: LegacyMessageType, reason: Optional[str] = None):
+        m = self.muc.get_system_participant()._make_message()
+        m["apply_to"]["id"] = self._legacy_to_xmpp(legacy_msg_id)
+        m["apply_to"]["moderated"].enable("retract")
+        m["apply_to"]["moderated"]["by"] = self.jid
+        if reason:
+            m["apply_to"]["moderated"]["reason"] = reason
+        self._send(m)
 
+    def set_room_subject(
+        self,
+        subject: str,
+        full_jid: Optional[JID] = None,
+        when: Optional[datetime] = None,
+        update_muc=True,
+    ):
+        if update_muc:
+            self.muc._subject = subject  # type: ignore
+            self.muc.subject_setter = self
+            self.muc.subject_date = when
+
+        msg = self._make_message()
+        if when is not None:
+            msg["delay"].set_stamp(when)
+            msg["delay"]["from"] = self.muc.jid
+        msg["subject"] = subject or str(self.muc.name)
+        self._send(msg, full_jid)
 
-ESCAPE_TABLE = "".maketrans(
-    {v: k for k, v in JID_UNESCAPE_TRANSFORMATIONS.items()}  # type:ignore
-)
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/core/disco.py` & `slidge-0.1.1/slidge/core/gateway/disco.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,80 @@
 import logging
 from typing import TYPE_CHECKING, Any, Optional
 
-from slixmpp import JID
 from slixmpp.exceptions import XMPPError
+from slixmpp.plugins.xep_0030.stanza.items import DiscoItems
 from slixmpp.types import OptJid
 
-from ..util.db import user_store
-from ..util.xep_0030.stanza.info import DiscoInfo
+from ...util.db import user_store
 
 if TYPE_CHECKING:
-    from ..core.gateway import BaseGateway
+    from .base import BaseGateway
 
 
 class Disco:
     def __init__(self, xmpp: "BaseGateway"):
         self.xmpp = xmpp
 
         xmpp.plugin["xep_0030"].set_node_handler(
             "get_info",
             jid=None,
             node=None,
             handler=self.get_info,
         )
 
+        xmpp.plugin["xep_0030"].set_node_handler(
+            "get_items",
+            jid=None,
+            node=None,
+            handler=self.get_items,
+        )
+
     async def get_info(
         self, jid: OptJid, node: Optional[str], ifrom: OptJid, data: Any
     ):
-        base = self.xmpp.plugin["xep_0030"].static.get_info(jid, node, ifrom, data)
-
-        if ifrom == self.xmpp.boundjid.bare:
-            return base
-
-        if jid == self.xmpp.boundjid.bare:
-            return base
+        if ifrom == self.xmpp.boundjid.bare or jid in (self.xmpp.boundjid.bare, None):
+            return self.xmpp.plugin["xep_0030"].static.get_info(jid, node, ifrom, data)
 
         if ifrom is None:
             raise XMPPError("subscription-required")
 
         user = user_store.get_by_jid(ifrom)
         if user is None:
             raise XMPPError("registration-required")
-        session = self.xmpp.get_session_from_user(user)  # type:ignore
+        session = self.xmpp.get_session_from_user(user)
+        await session.wait_for_ready()
+
         log.debug("Looking for entity: %s", jid)
-        try:
-            entity = await session.contacts.by_jid(jid)
-        except XMPPError:
-            entity = await session.bookmarks.by_jid(jid)
-            if nick := JID(jid).resource:
-                log.debug("Returning empty disco for participant")
-                d = DiscoInfo()
-                d.set_identities([("client", "pc", None, nick)])
-                return d
 
-        log.debug("entity: %s", entity)
-        return entity.get_disco_info()
+        assert jid is not None
+        entity = await session.get_contact_or_group_or_participant(jid)
+
+        if entity is None:
+            raise XMPPError("item-not-found")
+
+        return await entity.get_disco_info(jid, node)
+
+    async def get_items(
+        self, jid: OptJid, node: Optional[str], ifrom: OptJid, data: Any
+    ):
+        if ifrom is None:
+            raise XMPPError("bad-request")
+
+        if jid != self.xmpp.boundjid.bare:
+            return DiscoItems()
+
+        user = user_store.get_by_jid(ifrom)
+        if user is None:
+            raise XMPPError("registration-required")
+
+        session = self.xmpp.get_session_from_user(user)
+        await session.wait_for_ready()
+
+        d = DiscoItems()
+        for muc in sorted(session.bookmarks, key=lambda m: m.name):
+            d.add_item(muc.jid, name=muc.name)
+
+        return d
 
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/core/gateway.py` & `slidge-0.1.1/slidge/core/gateway/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,179 +1,216 @@
 """
 This module extends slixmpp.ComponentXMPP to make writing new LegacyClients easier
 """
+
 import asyncio
 import logging
 import re
 import tempfile
-from asyncio import Future
-from typing import Callable, Generic, Iterable, Optional, Sequence, Type
+from copy import copy
+from datetime import datetime
+from typing import TYPE_CHECKING, Callable, Collection, Optional, Sequence, Union
 
+import aiohttp
 import qrcode
-from slixmpp import JID, ComponentXMPP, CoroutineCallback, Iq, Message, StanzaPath
+from slixmpp import JID, ComponentXMPP, Iq, Message, Presence
 from slixmpp.exceptions import IqError, IqTimeout, XMPPError
-from slixmpp.plugins.xep_0363 import FileUploadError
+from slixmpp.plugins.xep_0060.stanza import OwnerAffiliation
 from slixmpp.types import MessageTypes
+from slixmpp.xmlstream.xmlstream import NotConnectedError
 
-from ..util import ABCSubclassableOnceAtMost, FormField
-from ..util.db import GatewayUser, RosterBackend, user_store
-from ..util.types import AvatarType
-from ..util.xep_0292.vcard4 import VCard4Provider
-from . import config
-from .adhoc import AdhocProvider, RegistrationType
-from .chat_command import ChatCommandProvider
+from ... import command  # noqa: F401
+from ...command.adhoc import AdhocProvider
+from ...command.admin import Exec
+from ...command.base import Command, FormField
+from ...command.chat_command import ChatCommandProvider
+from ...command.register import RegistrationType
+from ...slixfix.roster import RosterBackend
+from ...slixfix.xep_0292.vcard4 import VCard4Provider
+from ...util import ABCSubclassableOnceAtMost
+from ...util.db import GatewayUser, user_store
+from ...util.sql import db
+from ...util.types import AvatarType, MessageOrPresenceTypeVar
+from .. import config
+from ..mixins import MessageMixin
+from ..pubsub import PubSubComponent
+from ..session import BaseSession
+from .caps import Caps
+from .delivery_receipt import DeliveryReceipt
 from .disco import Disco
-from .pubsub import PubSubComponent
-from .session import BaseSession, SessionType
+from .mam import Mam
+from .muc_admin import MucAdmin
+from .ping import Ping
+from .presence import PresenceHandlerMixin
+from .registration import Registration
+from .search import Search
+from .session_dispatcher import SessionDispatcher
+from .vcard_temp import VCardTemp
+
+if TYPE_CHECKING:
+    from ...group.room import LegacyMUC
 
 
 class BaseGateway(
-    Generic[SessionType], ComponentXMPP, metaclass=ABCSubclassableOnceAtMost
+    PresenceHandlerMixin,
+    ComponentXMPP,
+    MessageMixin,
+    metaclass=ABCSubclassableOnceAtMost,
 ):
     """
-    Must be subclassed by a plugin to set up various aspects of the XMPP
-    component behaviour, such as its display name or its registration process.
+    The gateway component, handling registrations and un-registrations.
 
     On slidge launch, a singleton is instantiated, and it will be made available
     to public classes such :class:`.LegacyContact` or :class:`.BaseSession` as the
     ``.xmpp`` attribute.
-    Since it inherits from :class:`slixmpp.componentxmpp.ComponentXMPP`, this gives you a hand
-    on low-level XMPP interactions via slixmpp plugins, e.g.:
+
+    Must be subclassed by a legacy module to set up various aspects of the XMPP
+    component behaviour, such as its display name or welcome message, via
+    class attributes :attr:`.COMPONENT_NAME` :attr:`.WELCOME_MESSAGE`.
+
+    Abstract methods related to the registration process must be overriden
+    for a functional :term:`Legacy Module`:
+
+    - :meth:`.validate`
+    - :meth:`.validate_two_factor_code`
+    - :meth:`.get_qr_text`
+    - :meth:`.confirm_qr`
+
+    NB: Not all of these must be overridden, it depends on the
+    :attr:`REGISTRATION_TYPE`.
+
+    The other methods, such as :meth:`.send_text` or :meth:`.react` are the same
+    as those of :class:`.LegacyContact` and :class:`.LegacyParticipant`, because
+    the component itself is also a "messaging actor", ie, an :term:`XMPP Entity`.
+    For these methods, you need to specify the JID of the recipient with the
+    `mto` parameter.
+
+    Since it inherits from :class:`slixmpp.componentxmpp.ComponentXMPP`,you also
+    have a hand on low-level XMPP interactions via slixmpp methods, e.g.:
 
     .. code-block:: python
 
         self.send_presence(
             pfrom="somebody@component.example.com",
             pto="someonwelse@anotherexample.com",
         )
 
     However, you should not need to do so often since the classes of the plugin
     API provides higher level abstractions around most commonly needed use-cases, such
     as sending messages, or displaying a custom status.
 
     """
 
-    REGISTRATION_FIELDS: Iterable[FormField] = [
+    COMPONENT_NAME: str = NotImplemented
+    """Name of the component, as seen in service discovery by XMPP clients"""
+    COMPONENT_TYPE: str = ""
+    """Type of the gateway, should follow https://xmpp.org/registrar/disco-categories.html"""
+    COMPONENT_AVATAR: Optional[AvatarType] = None
+    """
+    Path, bytes or URL used by the component as an avatar.
+    """
+
+    REGISTRATION_FIELDS: Collection[FormField] = [
         FormField(var="username", label="User name", required=True),
         FormField(var="password", label="Password", required=True, private=True),
     ]
     """
     Iterable of fields presented to the gateway user when registering using :xep:`0077`
     `extended <https://xmpp.org/extensions/xep-0077.html#extensibility>`_ by :xep:`0004`.
     """
     REGISTRATION_INSTRUCTIONS: str = "Enter your credentials"
     """
     The text presented to a user that wants to register (or modify) their legacy account
     configuration.
     """
-    REGISTRATION_TYPE = RegistrationType.SINGLE_STEP_FORM
+    REGISTRATION_TYPE: RegistrationType = RegistrationType.SINGLE_STEP_FORM
     """
-    SINGLE_STEP_FORM: 1 step, 1 form, compatible with :xep:`0077` (in-band registration)
-    
-    QRCODE: The registration requires flashing a QR code in an official client.
-    See :meth:`.BaseGateway.`
-    
-    TWO_FACTOR_CODE: The registration requires confirming login with a 2FA code
+    This attribute determines how users register to the gateway, ie, how they
+    login to the :term:`legacy service <Legacy Service>`.
+    The credentials are then stored persistently, so this process should happen
+    once per user (unless they unregister).
+
+    The registration process always start with a basic data form (:xep:`0004`)
+    presented to the user.
+    But the legacy login flow might require something more sophisticated, see
+    :class:`.RegistrationType` for more details.
     """
 
-    COMPONENT_NAME: str = NotImplemented
-    """Name of the component, as seen in service discovery by XMPP clients"""
-    COMPONENT_TYPE: Optional[str] = ""
-    """Type of the gateway, should ideally follow https://xmpp.org/registrar/disco-categories.html"""
-    COMPONENT_AVATAR: Optional[AvatarType] = None
-    """
-    Path, bytes or URL used by the component as an avatar.
-    """
+    REGISTRATION_2FA_TITLE = "Enter your 2FA code"
+    REGISTRATION_2FA_INSTRUCTIONS = (
+        "You should have received something via email or SMS, or something"
+    )
+    REGISTRATION_QR_INSTRUCTIONS = "Flash this code or follow this link"
 
     ROSTER_GROUP: str = "slidge"
     """
-    Roster entries added by the plugin in the user's roster will be part of the group specified here.
+    Name of the group assigned to a :class:`.LegacyContact` automagically
+    added to the :term:`User`'s roster with :meth:`.LegacyContact.add_to_roster`.
+    """
+    WELCOME_MESSAGE = (
+        "Thank you for registering. Type 'help' to list the available commands, "
+        "or just start messaging away!"
+    )
+    """
+    A welcome message displayed to users on registration.
+    This is useful notably for clients that don't consider component JIDs as a
+    valid recipient in their UI, yet still open a functional chat window on
+    incoming messages from components.
     """
 
     SEARCH_FIELDS: Sequence[FormField] = [
         FormField(var="first", label="First name", required=True),
         FormField(var="last", label="Last name", required=True),
-        FormField(var="phone", label="Last name", required=False),
+        FormField(var="phone", label="Phone number", required=False),
     ]
     """
     Fields used for searching items via the component, through :xep:`0055` (jabber search).
     A common use case is to allow users to search for legacy contacts by something else than
     their usernames, eg their phone number.
-    
-    Plugins should implement search by overriding :meth:`.BaseSession.search`, effectively
-    restricting search to registered users by default.
-    
+
+    Plugins should implement search by overriding :meth:`.BaseSession.search`
+    (restricted to registered users).
+
     If there is only one field, it can also be used via the ``jabber:iq:gateway`` protocol
     described in :xep:`0100`. Limitation: this only works if the search request returns
     one result item, and if this item has a 'jid' var.
     """
     SEARCH_TITLE: str = "Search for legacy contacts"
     """
     Title of the search form.
     """
     SEARCH_INSTRUCTIONS: str = ""
     """
     Instructions of the search form.
     """
 
-    _BASE_CHAT_COMMANDS = {
-        "find": "_chat_command_search",
-        "help": "_chat_command_help",
-        "register": "_chat_command_register",
-        "unregister": "_chat_command_unregister",
-        "contacts": "_chat_command_list_contacts",
-        "groups": "_chat_command_list_groups",
-    }
-    CHAT_COMMANDS: dict[str, str] = {}
-    """
-    Keys of this dict can be used to trigger a command by a simple chat message to the gateway
-    component. Extra words after the key are passed as *args to the handler. Values of the dict
-    are strings, and handlers are resolved using ``getattr()`` on the :class:`.BaseGateway`
-    instance.
-    
-    Handlers are coroutines with following signature:
-    
-    .. code-block:: python
-    
-        async def _chat_command_xxx(*args, msg: Message, session: Optional[Session] = None)
-            ...
-    
-    The original :class:`slixmpp.stanza.Message` is also passed to the handler as the
-    msg kwarg. If the command comes from a registered gateway user, its session attribute is also
-    passed to the handler.
-    
-    Refer to the :class:`slixmpp.plugins.xep_0050.XEP_0050` for more details on how to use ad-hoc
-    commands.
-    """
-
-    WELCOME_MESSAGE = (
-        "Thank you for registering. Type 'help' to list the available commands, "
-        "or just start messaging away!"
-    )
+    MARK_ALL_MESSAGES = False
     """
-    A welcome message displayed to users on registration.
-    This is useful notably for clients that don't consider component JIDs as a valid recipient in their UI,
-    yet still open a functional chat window on incoming messages from components.
+    Set this to True for :term:`legacy networks <Legacy Network>` that expects
+    read marks for *all* messages and not just the latest one that was read
+    (as most XMPP clients will only send a read mark for the latest msg).
     """
 
-    MARK_ALL_MESSAGES = False
+    PROPER_RECEIPTS = False
     """
-    Set this to True for legacy networks that expects read marks for *all* messages and not just
-    the latest one that was read (as most XMPP clients will only send a reak mark for the latest msg).
+    Set this to True if the legacy service provides a real equivalent of message delivery receipts
+    (:xep:`0184`), meaning that there is an event thrown when the actual device of a contact receives
+    a message. Make sure to call Contact.received() adequately if this is set to True.
     """
 
-    REGISTRATION_2FA_TITLE = "Enter your 2FA code"
-    REGISTRATION_2FA_INSTRUCTIONS = (
-        "You should have received something via email or SMS, or something"
-    )
-    REGISTRATION_QR_INSTRUCTIONS = "Flash this code or follow this link"
-
     GROUPS = False
 
+    mtype: MessageTypes = "chat"
+    is_group = False
+    _can_send_carbon = False
+
     def __init__(self):
+        self.datetime_started = datetime.now()
+        self.xmpp = self  # ugly hack to work with the BaseSender mixin :/
+        self.default_ns = "jabber:component:accept"
         super().__init__(
             config.JID,
             config.SECRET,
             config.SERVER,
             config.PORT,
             plugin_whitelist=SLIXMPP_PLUGINS,
             plugin_config={
@@ -186,258 +223,152 @@
                 "xep_0100": {
                     "component_name": self.COMPONENT_NAME,
                     "user_store": user_store,
                     "type": self.COMPONENT_TYPE,
                 },
                 "xep_0184": {
                     "auto_ack": False,
-                    "auto_request": True,
+                    "auto_request": False,
                 },
                 "xep_0363": {
                     "upload_service": config.UPLOAD_SERVICE,
                 },
             },
+            fix_error_ns=True,
         )
         self.loop.set_exception_handler(self.__exception_handler)
-        self.has_crashed = False
+        self.http: aiohttp.ClientSession = aiohttp.ClientSession()
+        self.has_crashed: bool = False
+        self.use_origin_id = False
 
-        self.jid_validator = re.compile(config.USER_JID_VALIDATOR)
+        self.jid_validator: re.Pattern = re.compile(config.USER_JID_VALIDATOR)
+        self.qr_pending_registrations = dict[str, asyncio.Future[bool]]()
 
-        self.session_cls: Type[SessionType] = BaseSession.get_unique_subclass()
+        self.session_cls: BaseSession = BaseSession.get_unique_subclass()
         self.session_cls.xmpp = self
 
-        self.get_session_from_stanza = self.session_cls.from_stanza
-        self.get_session_from_user = self.session_cls.from_user
+        self.get_session_from_stanza: Callable[
+            [Union[Message, Presence, Iq]], BaseSession
+        ] = self.session_cls.from_stanza  # type: ignore
+        self.get_session_from_user: Callable[[GatewayUser], BaseSession] = (
+            self.session_cls.from_user
+        )
+
         self.register_plugins()
-        self.__register_slixmpp_api()
-        self.__register_handlers()
-        self._input_futures: dict[str, Future] = {}
+        self.__register_slixmpp_events()
+        self.roster.set_backend(RosterBackend)
 
         self.register_plugin("pubsub", {"component_name": self.COMPONENT_NAME})
         self.pubsub: PubSubComponent = self["pubsub"]
         self.vcard: VCard4Provider = self["xep_0292_provider"]
+        self.delivery_receipt: DeliveryReceipt = DeliveryReceipt(self)
+
+        # with this we receive user avatar updates
+        self.plugin["xep_0030"].add_feature("urn:xmpp:avatar:metadata+notify")
+
         if self.GROUPS:
             self.plugin["xep_0030"].add_feature("http://jabber.org/protocol/muc")
+            self.plugin["xep_0030"].add_feature("urn:xmpp:mam:2")
+            self.plugin["xep_0030"].add_feature("urn:xmpp:mam:2#extended")
+            self.plugin["xep_0030"].add_feature(self.plugin["xep_0421"].namespace)
+            self.plugin["xep_0030"].add_feature(self["xep_0317"].stanza.NS)
             self.plugin["xep_0030"].add_identity(
                 category="conference",
-                name="Slidged rooms",
+                name=self.COMPONENT_NAME,
                 itype="text",
                 jid=self.boundjid,
             )
 
-        self.adhoc = AdhocProvider(self)
-        self.add_adhoc_commands()
-
-        self.disco = Disco(self)
-
-        self.chat_commands = chat = ChatCommandProvider(self)
-        self._chat_commands: dict[str, Callable] = {
-            k: getattr(self, v, None) or getattr(chat, v)
-            for k, v in (self._BASE_CHAT_COMMANDS | self.CHAT_COMMANDS).items()
-        }
-
-        self.use_origin_id = False
-
-        self.remove_handler("Ping")
-        self.register_handler(
-            CoroutineCallback(
-                "Ping",
-                StanzaPath("iq@type=get/ping"),
-                self.__handle_ping,  # type:ignore
-            )
-        )
-
-        self.qr_pending_registrations = dict[str, asyncio.Future[bool]]()
-
-    async def __handle_ping(self, iq: Iq):
-        ito = iq.get_to()
-
-        if ito == self.boundjid.bare:
-            iq.reply().send()
-
-        ifrom = iq.get_from()
-        user = user_store.get_by_jid(ifrom)
-        if user is None:
-            raise XMPPError("registration-required")
-
-        session = self.get_session_from_user(user)
-
-        try:
-            muc = await session.bookmarks.by_jid(ito)
-        except XMPPError:
-            pass
-        else:
-            muc.handle_ping(iq)
-            return
-
-        try:
-            await session.contacts.by_jid(ito)
-        except XMPPError:
-            pass
-        else:
-            iq.reply().send()
+        # why does mypy need these type annotations? no idea
+        self.__adhoc_handler: AdhocProvider = AdhocProvider(self)
+        self.__chat_commands_handler: ChatCommandProvider = ChatCommandProvider(self)
+        self.__disco_handler = Disco(self)
+
+        self.__ping_handler = Ping(self)
+        self.__mam_handler = Mam(self)
+        self.__search_handler = Search(self)
+        self.__caps_handler = Caps(self)
+        self.__vcard_temp_handler = VCardTemp(self)
+        self.__muc_admin_handler = MucAdmin(self)
+        self.__registration = Registration(self)
+        self.__dispatcher = SessionDispatcher(self)
+
+        self.__register_commands()
+
+        db.mam_launch_cleanup_task(self.loop)
+
+    def __register_commands(self):
+        for cls in Command.subclasses:
+            if any(x is NotImplemented for x in [cls.CHAT_COMMAND, cls.NODE, cls.NAME]):
+                log.debug("Not adding command '%s' because it looks abstract", cls)
+                continue
+            if cls is Exec:
+                if config.DEV_MODE:
+                    log.warning("/!\ DEV MODE ENABLED /!\\")
+                else:
+                    continue
+            c = cls(self)
+            log.debug("Registering %s", cls)
+            self.__adhoc_handler.register(c)
+            self.__chat_commands_handler.register(c)
 
     def __exception_handler(self, loop: asyncio.AbstractEventLoop, context):
         """
         Called when a task created by loop.create_task() raises an Exception
 
         :param loop:
         :param context:
         :return:
         """
-        log.debug("CONTEXT: %s", context)
+        log.debug("Context in the exception handler: %s", context)
         exc = context.get("exception")
         if exc is None:
             log.warning("No exception in this context: %s", context)
         elif isinstance(exc, SystemExit):
             log.debug("SystemExit called in an asyncio task")
         else:
-            log.exception("Crash in an asyncio task: %s", context)
+            log.error("Crash in an asyncio task: %s", context)
+            log.exception("Crash in task", exc_info=exc)
             self.has_crashed = True
             loop.stop()
 
-    def _raise_if_not_allowed_jid(self, jid: JID):
-        if not self.jid_validator.match(jid.bare):
-            raise XMPPError(
-                condition="not-allowed",
-                text="Your account is not allowed to use this gateway.",
-            )
-
-    def exception(self, exception: Exception):
-        """
-        Called when a task created by slixmpp's internal (eg, on slix events) raises an Exception.
-
-        Stop the event loop and exit on unhandled exception.
-
-        The default :class:`slixmpp.basexmpp.BaseXMPP` behaviour is just to
-        log the exception, but we want to avoid undefined behaviour.
-
-        :param exception: An unhandled :class:`Exception` object.
-        """
-        if isinstance(exception, IqError):
-            iq = exception.iq
-            log.error("%s: %s", iq["error"]["condition"], iq["error"]["text"])
-            log.warning("You should catch IqError exceptions")
-        elif isinstance(exception, IqTimeout):
-            iq = exception.iq
-            log.error("Request timed out: %s", iq)
-            log.warning("You should catch IqTimeout exceptions")
-        elif isinstance(exception, SyntaxError):
-            # Hide stream parsing errors that occur when the
-            # stream is disconnected (they've been handled, we
-            # don't need to make a mess in the logs).
-            pass
-        else:
-            self.loop.stop()
-            exit(1)
-
-    def __register_slixmpp_api(self):
-        self["xep_0077"].api.register(
-            user_store.get,
-            "user_get",
-        )
-        self["xep_0077"].api.register(
-            user_store.remove,
-            "user_remove",
-        )
-        self["xep_0077"].api.register(
-            self.make_registration_form, "make_registration_form"
-        )
-        self["xep_0077"].api.register(self._user_validate, "user_validate")
-        self["xep_0077"].api.register(self._user_modify, "user_modify")
-
-        self["xep_0055"].api.register(self.search_get_form, "search_get_form")
-        self["xep_0055"].api.register(self._search_query, "search_query")
-
-        self.roster.set_backend(RosterBackend)
-
-    def __register_handlers(self):
+    def __register_slixmpp_events(self):
         self.add_event_handler("session_start", self.__on_session_start)
         self.add_event_handler("disconnected", self.connect)
-        self.add_event_handler("gateway_message", self._on_gateway_message_private)
         self.add_event_handler("user_register", self._on_user_register)
         self.add_event_handler("user_unregister", self._on_user_unregister)
-        get_session = self.get_session_from_stanza
+        self.add_event_handler("groupchat_message_error", self.__on_group_chat_error)
 
-        # fmt: off
-        async def msg(m): await get_session(m).send_from_msg(m)
-        async def disp(m): await get_session(m).displayed_from_msg(m)
-        async def active(m): await get_session(m).active_from_msg(m)
-        async def inactive(m): await get_session(m).inactive_from_msg(m)
-        async def composing(m): await get_session(m).composing_from_msg(m)
-        async def paused(m): await get_session(m).paused_from_msg(m)
-        async def correct(m): await get_session(m).correct_from_msg(m)
-        async def react(m): await get_session(m).react_from_msg(m)
-        async def retract(m): await get_session(m).retract_from_msg(m)
-        async def groupchat_join(p): await get_session(p).join_groupchat(p)
-        # fmt: on
-
-        self.add_event_handler("legacy_message", msg)
-        self.add_event_handler("marker_displayed", disp)
-        self.add_event_handler("chatstate_active", active)
-        self.add_event_handler("chatstate_inactive", inactive)
-        self.add_event_handler("chatstate_composing", composing)
-        self.add_event_handler("chatstate_paused", paused)
-        self.add_event_handler("message_correction", correct)
-        self.add_event_handler("reactions", react)
-        self.add_event_handler("message_retract", retract)
-
-        self.add_event_handler("groupchat_join", groupchat_join)
-        self.add_event_handler("groupchat_message", msg)
-
-        self.register_handler(
-            CoroutineCallback(
-                f"muc#admin",
-                StanzaPath(f"iq/mucadmin_query"),
-                self._handle_admin,  # type: ignore
-            )
-        )
+    @property  # type: ignore
+    def jid(self):
+        # Override to avoid slixmpp deprecation warnings.
+        return self.boundjid
+
+    async def __on_group_chat_error(self, msg: Message):
+        condition = msg["error"].get_condition()
+        if condition not in KICKABLE_ERRORS:
+            return
 
-        self.plugin["xep_0030"].add_feature("jabber:iq:gateway")
-        self.register_handler(
-            CoroutineCallback(
-                f"iq:gateway",
-                StanzaPath(f"iq/gateway"),
-                self._handle_gateway_iq,  # type: ignore
+        try:
+            muc = await self.get_muc_from_stanza(msg)
+        except XMPPError as e:
+            log.debug("Not removing resource", exc_info=e)
+            return
+        mfrom = msg.get_from()
+        resource = mfrom.resource
+        try:
+            muc.user_resources.remove(resource)
+        except KeyError:
+            # this actually happens quite frequently on for both beagle and monal
+            # (not sure why?), but is of no consequence
+            log.debug("%s was not in the resources of %s", resource, muc)
+        else:
+            log.info(
+                "Removed %s from the resources of %s because of error", resource, muc
             )
-        )
-
-    async def _handle_admin(self, iq: Iq):
-        log.debug("MUC ADMIN request %s", iq)
-        raise XMPPError("not-authorized")
-
-    async def _handle_gateway_iq(self, iq: Iq):
-        user = user_store.get_by_jid(iq.get_from())
-        if user is None:
-            raise XMPPError("not-authorized", "Register to the gateway first")
-
-        if len(self.SEARCH_FIELDS) > 1:
-            raise XMPPError("not-implemented", "Use jabber search for this gateway")
-
-        field = self.SEARCH_FIELDS[0]
-
-        reply = iq.reply()
-        if iq["type"] == "get":
-            reply["gateway"]["desc"] = self.SEARCH_TITLE
-            reply["gateway"]["prompt"] = field.label
-        elif iq["type"] == "set":
-            prompt = iq["gateway"]["prompt"]
-            session = self.session_cls.from_user(user)
-            result = await session.search({field.var: prompt})
-            if result is None or not result.items:
-                raise XMPPError(
-                    "item-not-found", "No contact was found with the info you provided."
-                )
-            if len(result.items) > 1:
-                raise XMPPError(
-                    "bad-request", "Your search yielded more than one result."
-                )
-            reply["gateway"]["jid"] = result.items[0]["jid"]
-
-        reply.send()
 
     async def __on_session_start(self, event):
         log.debug("Gateway session start: %s", event)
 
         # prevents XMPP clients from considering the gateway as an HTTP upload
         disco = self.plugin["xep_0030"]
         await disco.del_feature(feature="urn:xmpp:http:upload:0", jid=self.boundjid)
@@ -448,58 +379,259 @@
         )
 
         for user in user_store.get_all():
             # TODO: before this, we should check if the user has removed us from their roster
             #       while we were offline and trigger unregister from there. Presence probe does not seem
             #       to work in this case, there must be another way. privileged entity could be used
             #       as last resort.
-            await self["xep_0100"].add_component_to_roster(user.jid)
+            try:
+                await self["xep_0100"].add_component_to_roster(user.jid)
+                await self.__add_component_to_mds_whitelist(user.jid)
+            except IqError as e:
+                # TODO: remove the user when this happens? or at least
+                # this can happen when the user has unsubscribed from the XMPP server
+                log.warning(
+                    "Error with user %s, not logging them automatically",
+                    user,
+                    exc_info=e,
+                )
+                continue
             self.send_presence(
                 pto=user.bare_jid, ptype="probe"
             )  # ensure we get all resources for user
             session = self.session_cls.from_user(user)
-            self.loop.create_task(self._login_wrap(session))
+            session.create_task(self.__login_wrap(session))
 
         log.info("Slidge has successfully started")
 
-    async def _login_wrap(self, session: "SessionType"):
+    async def __add_component_to_mds_whitelist(self, user_jid: JID):
+        # Uses privileged entity to add ourselves to the whitelist of the PEP
+        # MDS node so we receive MDS events
+        iq_creation = Iq(sto=user_jid.bare, sfrom=user_jid, stype="set")
+        iq_creation["pubsub"]["create"]["node"] = self["xep_0490"].stanza.NS
+
+        try:
+            await self["xep_0356"].send_privileged_iq(iq_creation)
+        except PermissionError:
+            log.warning(
+                "IQ privileges not granted for pubsub namespace, we cannot "
+                "create the MDS node of %s",
+                user_jid,
+            )
+        except IqError as e:
+            # conflict this means the node already exists, we can ignore that
+            if e.condition != "conflict":
+                log.exception(
+                    "Could not create the MDS node of %s", user_jid, exc_info=e
+                )
+        except Exception as e:
+            log.exception(
+                "Error while trying to create to the MDS node of %s",
+                user_jid,
+                exc_info=e,
+            )
+
+        iq_affiliation = Iq(sto=user_jid.bare, sfrom=user_jid, stype="set")
+        iq_affiliation["pubsub_owner"]["affiliations"]["node"] = self[
+            "xep_0490"
+        ].stanza.NS
+
+        aff = OwnerAffiliation()
+        aff["jid"] = self.boundjid.bare
+        aff["affiliation"] = "member"
+        iq_affiliation["pubsub_owner"]["affiliations"].append(aff)
+
+        try:
+            await self["xep_0356"].send_privileged_iq(iq_affiliation)
+        except PermissionError:
+            log.warning(
+                "IQ privileges not granted for pubsub#owner namespace, we cannot "
+                "listen to the MDS events of %s",
+                user_jid,
+            )
+        except Exception as e:
+            log.exception(
+                "Error while trying to subscribe to the MDS node of %s",
+                user_jid,
+                exc_info=e,
+            )
+
+    async def __login_wrap(self, session: "BaseSession"):
         session.send_gateway_status("Logging in…", show="dnd")
         try:
             status = await session.login()
         except Exception as e:
-            log.warning(f"Login problem for %s: %r", session.user, e)
+            log.warning("Login problem for %s", session.user, exc_info=e)
             log.exception(e)
             session.send_gateway_status(f"Could not login: {e}", show="busy")
             session.send_gateway_message(
-                f"You are not connected to this gateway! "
+                "You are not connected to this gateway! "
                 f"Maybe this message will tell you why: {e}"
             )
+            return
+
+        log.info("Login success for %s", session.user)
+        session.logged = True
+        session.send_gateway_status("Syncing contacts…", show="dnd")
+        await session.contacts.fill()
+        if not (r := session.contacts.ready).done():
+            r.set_result(True)
+        if self.GROUPS:
+            session.send_gateway_status("Syncing groups…", show="dnd")
+            await session.bookmarks.fill()
+            if not (r := session.bookmarks.ready).done():
+                r.set_result(True)
+        for c in session.contacts:
+            # we need to receive presences directed at the contacts, in
+            # order to send pubsub events for their +notify features
+            self.send_presence(pfrom=c.jid, pto=session.user.bare_jid, ptype="probe")
+        if status is None:
+            session.send_gateway_status("Logged in", show="chat")
         else:
-            log.info(f"Login success for %s", session.user)
-            session.never_logged = False
-            if status is None:
-                session.send_gateway_status("Logged in", show="chat")
+            session.send_gateway_status(status, show="chat")
+        # If we stored users avatars (or their hash) persistently across slidge
+        # restarts, we would not need to fetch it on startup
+        session.create_task(self.__fetch_user_avatar(session))
+
+    async def __fetch_user_avatar(self, session: BaseSession):
+        try:
+            iq = await self.xmpp.plugin["xep_0060"].get_items(
+                session.user.bare_jid,
+                self.xmpp.plugin["xep_0084"].stanza.MetaData.namespace,
+                ifrom=self.boundjid.bare,
+            )
+        except IqError as e:
+            session.log.debug("Failed to retrieve avatar: %r", e)
+            return
+        await self.__dispatcher.on_avatar_metadata_info(
+            session, iq["pubsub"]["items"]["item"]["avatar_metadata"]["info"]
+        )
+
+    def _send(
+        self, stanza: MessageOrPresenceTypeVar, **send_kwargs
+    ) -> MessageOrPresenceTypeVar:
+        stanza.set_from(self.boundjid.bare)
+        if mto := send_kwargs.get("mto"):
+            stanza.set_to(mto)
+        stanza.send()
+        return stanza
+
+    async def _on_user_register(self, iq: Iq):
+        session = self.get_session_from_stanza(iq)
+        for jid in config.ADMINS:
+            self.send_message(
+                mto=jid,
+                mbody=f"{iq.get_from()} has registered",
+                mtype="headline",
+                mfrom=self.boundjid.bare,
+            )
+        session.send_gateway_message(self.WELCOME_MESSAGE)
+        await self.__login_wrap(session)
+
+    async def _on_user_unregister(self, iq: Iq):
+        await self.session_cls.kill_by_jid(iq.get_from())
+
+    def raise_if_not_allowed_jid(self, jid: JID):
+        if not self.jid_validator.match(jid.bare):
+            raise XMPPError(
+                condition="not-allowed",
+                text="Your account is not allowed to use this gateway.",
+            )
+
+    def send_raw(self, data: Union[str, bytes]):
+        # overridden from XMLStream to strip base64-encoded data from the logs
+        # to make them more readable.
+        if log.isEnabledFor(level=logging.DEBUG):
+            if isinstance(data, str):
+                stripped = copy(data)
             else:
-                session.send_gateway_status(status, show="chat")
-            for c in session.contacts:
-                # we need to receive presences directed at the contacts, in
-                # order to send pubsub events for their +notify features
-                self.send_presence(
-                    pfrom=c.jid, pto=session.user.bare_jid, ptype="probe"
+                stripped = data.decode("utf-8")
+            # there is probably a way to do that in a single RE,
+            # but since it's only for debugging, the perf penalty
+            # does not matter much
+            for el in LOG_STRIP_ELEMENTS:
+                stripped = re.sub(
+                    f"(<{el}.*?>)(.*)(</{el}>)",
+                    "\1[STRIPPED]\3",
+                    stripped,
+                    flags=re.DOTALL | re.IGNORECASE,
                 )
+            log.debug("SEND: %s", stripped)
+        if not self.transport:
+            raise NotConnectedError()
+        if isinstance(data, str):
+            data = data.encode("utf-8")
+        self.transport.write(data)
+
+    def get_session_from_jid(self, j: JID):
+        try:
+            return self.session_cls.from_jid(j)
+        except XMPPError:
+            pass
+
+    async def get_muc_from_stanza(self, iq: Union[Iq, Message]) -> "LegacyMUC":
+        ito = iq.get_to()
+
+        if ito == self.boundjid.bare:
+            raise XMPPError(
+                text="No MAM on the component itself, use a JID with a resource"
+            )
+
+        ifrom = iq.get_from()
+        user = user_store.get_by_jid(ifrom)
+        if user is None:
+            raise XMPPError("registration-required")
+
+        session = self.get_session_from_user(user)
+        session.raise_if_not_logged()
 
-    def re_login(self, session: "SessionType"):
+        muc = await session.bookmarks.by_jid(ito)
+
+        return muc
+
+    def exception(self, exception: Exception):
+        # """
+        # Called when a task created by slixmpp's internal (eg, on slix events) raises an Exception.
+        #
+        # Stop the event loop and exit on unhandled exception.
+        #
+        # The default :class:`slixmpp.basexmpp.BaseXMPP` behaviour is just to
+        # log the exception, but we want to avoid undefined behaviour.
+        #
+        # :param exception: An unhandled :class:`Exception` object.
+        # """
+        if isinstance(exception, IqError):
+            iq = exception.iq
+            log.error("%s: %s", iq["error"]["condition"], iq["error"]["text"])
+            log.warning("You should catch IqError exceptions")
+        elif isinstance(exception, IqTimeout):
+            iq = exception.iq
+            log.error("Request timed out: %s", iq)
+            log.warning("You should catch IqTimeout exceptions")
+        elif isinstance(exception, SyntaxError):
+            # Hide stream parsing errors that occur when the
+            # stream is disconnected (they've been handled, we
+            # don't need to make a mess in the logs).
+            pass
+        else:
+            if exception:
+                log.exception(exception)
+            self.loop.stop()
+            exit(1)
+
+    def re_login(self, session: "BaseSession"):
         async def w():
+            session.cancel_all_tasks()
             await session.logout()
-            await self._login_wrap(session)
+            await self.__login_wrap(session)
 
-        self.loop.create_task(w())
+        session.create_task(w())
 
     async def make_registration_form(self, _jid, _node, _ifrom, iq: Iq):
-        self._raise_if_not_allowed_jid(iq.get_from())
+        self.raise_if_not_allowed_jid(iq.get_from())
         reg = iq["register"]
         user = user_store.get_by_stanza(iq)
         log.debug("User found: %s", user)
 
         form = reg["form"]
         form.add_field(
             "FORM_TYPE",
@@ -540,360 +672,224 @@
             )
 
         reply = iq.reply()
         reply.set_payload(reg)
         return reply
 
     async def user_prevalidate(self, ifrom: JID, form_dict: dict[str, Optional[str]]):
-        """
-        Pre validate a registration form using the content of self.REGISTRATION_FIELDS
-        before passing it to the plugin custom validation logic.
-        """
+        # Pre validate a registration form using the content of self.REGISTRATION_FIELDS
+        # before passing it to the plugin custom validation logic.
         for field in self.REGISTRATION_FIELDS:
             if field.required and not form_dict.get(field.var):
                 raise ValueError(f"Missing field: '{field.label}'")
 
         await self.validate(ifrom, form_dict)
 
-    async def _user_validate(self, _gateway_jid, _node, ifrom: JID, iq: Iq):
-        """
-        SliXMPP internal API stuff
-        """
-        log.debug("User validate: %s", ifrom.bare)
-        form_dict = {f.var: iq.get(f.var) for f in self.REGISTRATION_FIELDS}
-        self._raise_if_not_allowed_jid(ifrom)
-        await self.user_prevalidate(ifrom, form_dict)
-        log.info("New user: %s", ifrom.bare)
-        user_store.add(ifrom, form_dict)
-
-    async def _user_modify(
-        self, _gateway_jid, _node, ifrom: JID, form_dict: dict[str, Optional[str]]
+    async def validate(
+        self, user_jid: JID, registration_form: dict[str, Optional[str]]
     ):
         """
-        SliXMPP internal API stuff
-        """
-        user = user_store.get_by_jid(ifrom)
-        log.debug("Modify user: %s", user)
-        await self.user_prevalidate(ifrom, form_dict)
-        user_store.add(ifrom, form_dict)
+        Validate a user's initial registration form.
 
-    async def _on_user_register(self, iq: Iq):
-        session = self.get_session_from_stanza(iq)
-        for jid in config.ADMINS:
-            self.send_message(
-                mto=jid,
-                mbody=f"{iq.get_from()} has registered",
-                mtype="headline",
-                mfrom=self.boundjid.bare,
-            )
-        session.send_gateway_message(self.WELCOME_MESSAGE)
-        await self._login_wrap(session)
+        Should raise the appropriate :class:`slixmpp.exceptions.XMPPError`
+        if the registration does not allow to continue the registration process.
 
-    async def _on_user_unregister(self, iq: Iq):
-        await self.session_cls.kill_by_jid(iq.get_from())
+        If :py:attr:`REGISTRATION_TYPE` is a
+        :attr:`.RegistrationType.SINGLE_STEP_FORM`,
+        this method should raise something if it wasn't possible to successfully
+        log in to the legacy service with the registration form content.
+
+        It is also used for other types of :py:attr:`REGISTRATION_TYPE` too, since
+        the first step is always a form. If :attr:`.REGISTRATION_FIELDS` is an
+        empty list (ie, it declares no :class:`.FormField`), the "form" is
+        effectively a confirmation dialog displaying
+        :attr:`.REGISTRATION_INSTRUCTIONS`.
 
-    async def search_get_form(self, _gateway_jid, _node, ifrom: JID, iq: Iq):
-        """
-        Prepare the search form using :attr:`.BaseSession.SEARCH_FIELDS`
+        :param user_jid: JID of the user that has just registered
+        :param registration_form: A dict where keys are the :attr:`.FormField.var` attributes
+         of the :attr:`.BaseGateway.REGISTRATION_FIELDS` iterable
         """
-        user = user_store.get_by_jid(ifrom)
-        if user is None:
-            raise XMPPError(text="Search is only allowed for registered users")
-
-        reply = iq.reply()
-        form = reply["search"]["form"]
-        form["title"] = self.SEARCH_TITLE
-        form["instructions"] = self.SEARCH_INSTRUCTIONS
-        for field in self.SEARCH_FIELDS:
-            form.add_field(**field.dict())
-        return reply
+        raise NotImplementedError
 
-    async def _search_query(self, _gateway_jid, _node, ifrom: JID, iq: Iq):
-        """
-        Handles a search request
+    async def validate_two_factor_code(self, user: GatewayUser, code: str):
         """
-        user = user_store.get_by_jid(ifrom)
-        if user is None:
-            raise XMPPError(text="Search is only allowed for registered users")
-
-        result = await self.get_session_from_stanza(iq).search(
-            iq["search"]["form"].get_values()
-        )
+        Called when the user enters their 2FA code.
 
-        if not result:
-            raise XMPPError("item-not-found", text="Nothing was found")
+        Should raise the appropriate :class:`slixmpp.exceptions.XMPPError`
+        if the login fails, and return successfully otherwise.
 
-        reply = iq.reply()
-        form = reply["search"]["form"]
-        for field in result.fields:
-            form.add_reported(field.var, label=field.label, type=field.type)
-        for item in result.items:
-            form.add_item(item)
-        return reply
+        Only used when :attr:`REGISTRATION_TYPE` is
+        :attr:`.RegistrationType.TWO_FACTOR_CODE`.
 
-    def add_adhoc_commands(self):
+        :param user: The :class:`.GatewayUser` whose registration is pending
+            Use their :attr:`.GatewayUser.bare_jid` and/or
+            :attr:`.registration_form` attributes to get what you need.
+        :param code: The code they entered, either via "chatbot" message or
+            adhoc command
         """
-        Override this if you want to provide custom adhoc commands (:xep:`0050`)
-        for your plugin, using :class:`slixmpp.plugins.xep_0050.XEP_0050`
-
-        Basic example:
-
-        .. code-block:: python
-
-            def add_adhoc_commands(self):
-                self["xep_0050"].add_command(
-                    node="account_info",
-                    name="Account Information",
-                    handler=self.handle_account_info
-                )
-
-            async def handle_account_info(self, iq: Iq, adhoc_session: dict[str, Any]):
-                # beware, 'adhoc_session' is not a slidge session!
-                user = user_store.get_by_stanza(iq)
-
-                if user is None:
-                    raise XMPPError("subscription-required")
-
-                form = self["xep_0004"].make_form("result", "Account info")
-                form.add_field(
-                    label="Credits",
-                    value=await FakeLegacyClient.get_credits(user.registration_form['username']),
-                )
-
-                adhoc_session["payload"] = form
-                adhoc_session["has_next"] = False
+        raise NotImplementedError
 
-                return session
+    async def get_qr_text(self, user: GatewayUser) -> str:
         """
-        pass
+        This is where slidge gets the QR code content for the QR-based
+        registration process. It will turn it into a QR code image and send it
+        to the not-yet-fully-registered :class:`.GatewayUser`.
+
+        Only used in when :attr:`BaseGateway.REGISTRATION_TYPE` is
+        :attr:`.RegistrationType.QRCODE`.
+
+        :param user: The :class:`.GatewayUser` whose registration is pending
+            Use their :attr:`.GatewayUser.bare_jid` and/or
+            :attr:`.registration_form` attributes to get what you need.
+        """
+        raise NotImplementedError
 
-    async def validate(
-        self, user_jid: JID, registration_form: dict[str, Optional[str]]
+    async def confirm_qr(
+        self, user_bare_jid: str, exception: Optional[Exception] = None
     ):
         """
-        Validate a registration form from a user.
+        This method is meant to be called to finalize QR code-based registration
+        flows, once the legacy service confirms the QR flashing.
 
-        Since :xep:`0077` is pretty limited in terms of validation, it is OK to validate
-        anything that looks good here and continue the legacy auth process via direct messages
-        to the user (using :meth:`.BaseGateway.input` for instance).
+        Only used in when :attr:`BaseGateway.REGISTRATION_TYPE` is
+        :attr:`.RegistrationType.QRCODE`.
 
-        :param user_jid: JID of the user that has just registered
-        :param registration_form: A dict where keys are the :attr:`.FormField.var` attributes
-         of the :attr:`.BaseGateway.REGISTRATION_FIELDS` iterable
+        :param user_bare_jid: The bare JID of the almost-registered
+            :class:`GatewayUser` instance
+        :param exception: Optionally, an XMPPError to be raised to **not** confirm
+            QR code flashing.
         """
-        pass
+        fut = self.qr_pending_registrations[user_bare_jid]
+        if exception is None:
+            fut.set_result(True)
+        else:
+            fut.set_exception(exception)
+
+    async def unregister_user(self, user: GatewayUser):
+        await self.xmpp.plugin["xep_0077"].api["user_remove"](None, None, user.jid)
+        await self.xmpp.session_cls.kill_by_jid(user.jid)
 
     async def unregister(self, user: GatewayUser):
         """
         Optionally override this if you need to clean additional
         stuff after a user has been removed from the permanent user_store.
 
-        :param user:
-        """
-        pass
+        By default, this just calls :meth:`BaseSession.logout`.
 
-    async def _on_gateway_message_private(self, msg: Message):
-        """
-        Called when an XMPP user (not necessarily registered as a gateway user) sends a direct message to
-        the gateway.
-
-        If you override this and still want :meth:`.BaseGateway.input` to work, make sure to include the try/except part.
-
-        :param msg: Message sent by the XMPP user
-        """
-        try:
-            f = self._input_futures.pop(msg.get_from().bare)
-        except KeyError:
-            text = msg["body"]
-            command, *rest = text.split(" ")
-
-            user = user_store.get_by_stanza(msg)
-            if user is None:
-                session = None
-            else:
-                session = self.get_session_from_user(user)
-
-            handler = self._chat_commands.get(command)
-            if handler is None:
-                await self.on_gateway_message(msg, session=session)
-            else:
-                log.debug("Chat command handler: %s", handler)
-                await handler(*rest, msg=msg, session=session)
-        else:
-            f.set_result(msg["body"])
-
-    @staticmethod
-    async def on_gateway_message(msg: Message, session: Optional[SessionType] = None):
-        """
-        Called when the gateway component receives a direct gateway message.
-
-        Can be used to implement bot like commands, especially in conjunction with
-        :meth:`.BaseGateway.input`
-
-        :param msg:
-        :param session: If the message comes from a registered gateway user, their :.BaseSession:
+        :param user:
         """
-        if session is None:
-            r = msg.reply(
-                body="I got that, but I'm not doing anything with it. I don't even know you!"
-            )
-        else:
-            r = msg.reply(body="What? Type 'help' for the list of available commands.")
-        r["type"] = "chat"
-        r.send()
+        session = self.get_session_from_user(user)
+        await session.logout()
 
     async def input(
         self, jid: JID, text=None, mtype: MessageTypes = "chat", **msg_kwargs
     ) -> str:
         """
         Request arbitrary user input using a simple chat message, and await the result.
 
-        You shouldn't need to call directly bust instead use :meth:`.BaseSession.input`
-        to directly target a user.
-
-        NB: When using this, the next message that the user sent to the component will
-        not be transmitted to :meth:`.BaseGateway.on_gateway_message`, but rather intercepted.
-        Await the coroutine to get its content.
+        You shouldn't need to call this directly bust instead use
+        :meth:`.BaseSession.input` to directly target a user.
 
         :param jid: The JID we want input from
         :param text: A prompt to display for the user
         :param mtype: Message type
         :return: The user's reply
         """
-        if text is not None:
-            self.send_message(
-                mto=jid, mbody=text, mtype=mtype, mfrom=self.boundjid.bare, **msg_kwargs
-            )
-        f = self.loop.create_future()
-        self._input_futures[jid.bare] = f
-        await f
-        return f.result()
-
-    async def send_file(self, filename: str, **msg_kwargs):
-        """
-        Upload a file using :xep:`0363` and send the link as out of band (:xep:`0066`)
-        content in a message.
-
-        :param filename:
-        :param msg_kwargs:
-        :return:
-        """
-        msg = self.make_message(**msg_kwargs)
-        msg.set_from(self.boundjid.bare)
-        try:
-            url = await self["xep_0363"].upload_file(
-                filename=filename, ifrom=config.UPLOAD_REQUESTER
-            )
-        except FileUploadError as e:
-            log.warning(
-                "Something is wrong with the upload service, see the traceback below"
-            )
-            log.exception(e)
-            msg["body"] = (
-                "I tried to send a file, but something went wrong. "
-                "Tell your XMPP admin to check slidge logs."
-            )
-            msg.send()
-            return
-        msg["oob"]["url"] = url
-        msg["body"] = url
-        msg.send()
+        return await self.__chat_commands_handler.input(jid, text, mtype, **msg_kwargs)
 
     async def send_qr(self, text: str, **msg_kwargs):
         """
         Sends a QR Code to a JID
 
+        You shouldn't need to call directly bust instead use
+        :meth:`.BaseSession.send_qr` to directly target a user.
+
         :param text: The text that will be converted to a QR Code
-        :param msg_kwargs: Optional additional arguments to pass to :meth:`.BaseGateway.send_file`,
-            such as the recipient of the QR code.
+        :param msg_kwargs: Optional additional arguments to pass to
+            :meth:`.BaseGateway.send_file`, such as the recipient of the QR,
+            code
         """
         qr = qrcode.make(text)
-        with tempfile.NamedTemporaryFile(suffix=".png") as f:
+        with tempfile.NamedTemporaryFile(
+            suffix=".png", delete=config.NO_UPLOAD_METHOD != "move"
+        ) as f:
             qr.save(f.name)
             await self.send_file(f.name, **msg_kwargs)
 
-    def shutdown(self):
-        """
-        Called by the slidge entrypoint on normal exit.
-
-        Sends offline presences from all contacts of all user sessions and from
-        the gateway component itself.
-        No need to call this manually, :func:`slidge.__main__.main` should take care of it.
-        """
+    def shutdown(self) -> list[asyncio.Task]:
+        # """
+        # Called by the slidge entrypoint on normal exit.
+        #
+        # Sends offline presences from all contacts of all user sessions and from
+        # the gateway component itself.
+        # No need to call this manually, :func:`slidge.__main__.main` should take care of it.
+        # """
         log.debug("Shutting down")
+        tasks = []
         for user in user_store.get_all():
-            self.session_cls.from_jid(user.jid).shutdown()
+            tasks.append(self.session_cls.from_jid(user.jid).shutdown())
             self.send_presence(ptype="unavailable", pto=user.jid)
+        return tasks
 
-    async def validate_two_factor_code(self, user: GatewayUser, code: str):
-        """
-        Called when the user enters their 2FA code.
 
-        Should raise the appropriate ``XMPPError`` if the login fails
-
-        :param user: The gateway user whose registration is pending
-            Use their ``.bare_jid`` and/or``.registration_form`` attributes
-            to get what you need
-        :param code: The code they entered, either via "chatbot" message or
-            adhoc command
-        """
-        raise NotImplementedError
-
-    async def get_qr_text(self, user: GatewayUser) -> str:
-        """
-        Plugins should call this to complete registration with QR codes
-
-        :param user: The not-yet-fully-registered GatewayUser.
-            Use its ``.bare_jid`` and/or``.registration_form`` attributes
-            to get what you need
-        """
-        raise NotImplementedError
-
-    async def confirm_qr(
-        self, user_bare_jid: str, exception: Optional[Exception] = None
-    ):
-        """
-        Plugins should call this to complete registration with QR codes
-
-        :param user_bare_jid: The not-yet-fully-registered ``GatewayUser`` instance
-            Use their ``.bare_jid`` and/or``.registration_form`` attributes
-            to get what you need
-        :param exception: Optionally, an XMPPError to be raised to **not** confirm
-            QR code flashing.
-        """
-        fut = self.qr_pending_registrations[user_bare_jid]
-        if exception is None:
-            fut.set_result(True)
-        else:
-            fut.set_exception(exception)
+KICKABLE_ERRORS = {
+    "gone",
+    "internal-server-error",
+    "item-not-found",
+    "jid-malformed",
+    "recipient-unavailable",
+    "redirect",
+    "remote-server-not-found",
+    "remote-server-timeout",
+    "service-unavailable",
+    "malformed error",
+}
 
 
 SLIXMPP_PLUGINS = [
+    "link_preview",  # https://wiki.soprani.ca/CheogramApp/LinkPreviews
     "xep_0030",  # Service discovery
     "xep_0045",  # Multi-User Chat
     "xep_0050",  # Adhoc commands
+    "xep_0054",  # VCard-temp (for MUC avatars)
     "xep_0055",  # Jabber search
+    "xep_0059",  # Result Set Management
     "xep_0066",  # Out of Band Data
     "xep_0077",  # In-band registration
     "xep_0084",  # User Avatar
     "xep_0085",  # Chat state notifications
     "xep_0100",  # Gateway interaction
     "xep_0106",  # JID Escaping
     "xep_0115",  # Entity capabilities
+    "xep_0122",  # Data Forms Validation
+    "xep_0153",  # vCard-Based Avatars (for MUC avatars)
     "xep_0172",  # User nickname
     "xep_0184",  # Message Delivery Receipts
     "xep_0199",  # XMPP Ping
     "xep_0221",  # Data Forms Media Element
+    "xep_0249",  # Direct MUC Invitations
+    "xep_0264",  # Jingle Content Thumbnails
     "xep_0280",  # Carbons
     "xep_0292_provider",  # VCard4
     "xep_0308",  # Last message correction
+    "xep_0313",  # Message Archive Management
+    "xep_0317",  # Hats
     "xep_0319",  # Last User Interaction in Presence
     "xep_0333",  # Chat markers
     "xep_0334",  # Message Processing Hints
     "xep_0356",  # Privileged Entity
     "xep_0356_old",  # Privileged Entity (old namespace)
     "xep_0363",  # HTTP file upload
+    "xep_0385",  # Stateless in-line media sharing
+    "xep_0402",  # PEP Native Bookmarks
+    "xep_0421",  # Anonymous unique occupant identifiers for MUCs
     "xep_0424",  # Message retraction
+    "xep_0425",  # Message moderation
     "xep_0444",  # Message reactions
+    "xep_0447",  # Stateless File Sharing
     "xep_0461",  # Message replies
+    "xep_0490",  # Message Displayed Synchronization
 ]
+
+LOG_STRIP_ELEMENTS = ["data", "binval"]
+
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/core/mixins/message.py` & `slidge-0.1.1/slidge/core/mixins/message.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,396 +1,398 @@
 import logging
-from datetime import datetime, timezone
-from io import BytesIO
-from pathlib import Path
-from typing import IO, Iterable, Optional, Union
-
-import aiohttp
-from slixmpp import JID, Message
-from slixmpp.plugins.xep_0363 import FileUploadError
-from slixmpp.types import MessageTypes
-
-from slidge.core import config
-from slidge.util.types import LegacyMessageType
-
-from ...util.types import ChatState, Marker, ProcessingHint
-from .base import BaseSender
-
-
-class MessageMaker(BaseSender):
-    mtype: MessageTypes = NotImplemented
-    STRIP_SHORT_DELAY = False
-    USE_STANZA_ID = False
-    _is_composing = False
+import uuid
+import warnings
+from datetime import datetime
+from typing import TYPE_CHECKING, Iterable, Optional
+
+from slixmpp import Iq, Message
+
+from ...slixfix.xep_0490.mds import PUBLISH_OPTIONS
+from ...util.types import (
+    ChatState,
+    LegacyMessageType,
+    LegacyThreadType,
+    LinkPreview,
+    Marker,
+    MessageReference,
+    ProcessingHint,
+)
+from .attachment import AttachmentMixin
+from .message_maker import MessageMaker
 
-    def _make_message(
-        self,
-        state: Optional[ChatState] = None,
-        hints: Iterable[ProcessingHint] = (),
-        legacy_msg_id: Optional[LegacyMessageType] = None,
-        when: Optional[datetime] = None,
-        reply_to_msg_id: Optional[LegacyMessageType] = None,
-        reply_to_fallback_text: Optional[str] = None,
-        reply_to_jid: Optional[JID] = None,
-        carbon=False,
-        **kwargs,
-    ):
-        body = kwargs.pop("mbody", None)
-        mfrom = kwargs.pop("mfrom", self.jid)
-        mto = kwargs.pop("mto", None)
-        if carbon:
-            # the msg needs to have jabber:client as xmlns, so
-            # we don't want to associate with the XML stream
-            msg_cls = Message  # type:ignore
-        else:
-            msg_cls = self.xmpp.Message  # type:ignore
-        msg = msg_cls(sfrom=mfrom, stype=self.mtype, sto=mto, **kwargs)
-        if body:
-            if self._is_composing:
-                state = "active"
-                self._is_composing = False
-            msg["body"] = body
-        if state:
-            self._is_composing = state == "composing"
-            msg["chat_state"] = state
-        for hint in hints:
-            msg.enable(hint)
-        self._set_msg_id(msg, legacy_msg_id)
-        self._add_delay(msg, when)
-        self._add_reply_to(msg, reply_to_msg_id, reply_to_fallback_text, reply_to_jid)
-        return msg
-
-    def _set_msg_id(
-        self, msg: Message, legacy_msg_id: Optional[LegacyMessageType] = None
-    ):
-        if legacy_msg_id is not None:
-            i = self._legacy_to_xmpp(legacy_msg_id)
-            msg.set_id(i)
-            if self.USE_STANZA_ID:
-                msg["stanza_id"]["id"] = i
-                msg["stanza_id"]["by"] = self.muc.jid  # type: ignore
-
-    def _legacy_to_xmpp(self, legacy_id: LegacyMessageType):
-        return self.session.sent.get(
-            legacy_id
-        ) or self.session.legacy_msg_id_to_xmpp_msg_id(legacy_id)
-
-    def _add_delay(self, msg: Message, when: Optional[datetime]):
-        if when:
-            if when.tzinfo is None:
-                when = when.astimezone(timezone.utc)
-            if self.STRIP_SHORT_DELAY:
-                delay = datetime.now().astimezone(timezone.utc) - when
-                if delay < config.IGNORE_DELAY_THRESHOLD:
-                    return
-            msg["delay"].set_stamp(when)
-            msg["delay"].set_from(self.xmpp.boundjid.bare)
-
-    def _add_reply_to(
-        self,
-        msg: Message,
-        reply_to_msg_id: Optional[LegacyMessageType] = None,
-        reply_to_fallback_text: Optional[str] = None,
-        reply_to_author: Optional[JID] = None,
-    ):
-        if reply_to_msg_id is not None:
-            xmpp_id = self._legacy_to_xmpp(reply_to_msg_id)
-            msg["reply"]["id"] = xmpp_id
-            # FIXME: https://xmpp.org/extensions/xep-0461.html#usecases mentions that a full JID must be used here
-            if reply_to_author:
-                msg["reply"]["to"] = reply_to_author
-            if reply_to_fallback_text:
-                msg["feature_fallback"].add_quoted_fallback(reply_to_fallback_text)
+if TYPE_CHECKING:
+    from ...group import LegacyMUC
 
 
 class ChatStateMixin(MessageMaker):
-    def _chat_state(self, state: ChatState, **kwargs):
-        msg = self._make_message(
-            state=state, hints={"no-store"}, carbon=kwargs.get("carbon")
-        )
+    def __init__(self):
+        super().__init__()
+        self.__last_chat_state: Optional[ChatState] = None
+
+    def _chat_state(self, state: ChatState, forced=False, **kwargs):
+        carbon = kwargs.get("carbon", False)
+        if carbon or (state == self.__last_chat_state and not forced):
+            return
+        self.__last_chat_state = state
+        msg = self._make_message(state=state, hints={"no-store"})
         self._send(msg, **kwargs)
 
     def active(self, **kwargs):
         """
-        Send an "active" chat state (:xep:`0085`) from this contact to the user.
+        Send an "active" chat state (:xep:`0085`) from this
+        :term:`XMPP Entity`.
         """
         self._chat_state("active", **kwargs)
 
     def composing(self, **kwargs):
         """
-        Send a "composing" (ie "typing notification") chat state (:xep:`0085`) from this contact to the user.
+        Send a "composing" (ie "typing notification") chat state (:xep:`0085`)
+        from this :term:`XMPP Entity`.
         """
-        self._chat_state("composing", **kwargs)
+        self._chat_state("composing", forced=True, **kwargs)
 
     def paused(self, **kwargs):
         """
-        Send a "paused" (ie "typing paused notification") chat state (:xep:`0085`) from this contact to the user.
+        Send a "paused" (ie "typing paused notification") chat state
+        (:xep:`0085`) from this :term:`XMPP Entity`.
         """
         self._chat_state("paused", **kwargs)
 
     def inactive(self, **kwargs):
         """
-        Send an "inactive" (ie "typing paused notification") chat state (:xep:`0085`) from this contact to the user.
+        Send an "inactive" (ie "contact has not interacted with the chat session
+        interface for an intermediate period of time") chat state (:xep:`0085`)
+        from this :term:`XMPP Entity`.
         """
         self._chat_state("inactive", **kwargs)
 
     def gone(self, **kwargs):
         """
-        Send an "inactive" (ie "typing paused notification") chat state (:xep:`0085`) from this contact to the user.
+        Send a "gone" (ie "contact has not interacted with the chat session interface,
+        system, or device for a relatively long period of time") chat state
+        (:xep:`0085`) from this :term:`XMPP Entity`.
         """
         self._chat_state("gone", **kwargs)
 
 
 class MarkerMixin(MessageMaker):
     is_group: bool = NotImplemented
 
     def _make_marker(
         self, legacy_msg_id: LegacyMessageType, marker: Marker, carbon=False
     ):
         msg = self._make_message(carbon=carbon)
         msg[marker]["id"] = self._legacy_to_xmpp(legacy_msg_id)
         return msg
 
-    def _make_receipt(self, legacy_msg_id: LegacyMessageType, carbon=False):
-        msg = self._make_message(carbon=carbon)
-        msg["receipt"] = self._legacy_to_xmpp(legacy_msg_id)
-        return msg
-
     def ack(self, legacy_msg_id: LegacyMessageType, **kwargs):
         """
-        Send an "acknowledged" message marker (:xep:`0333`) from this contact to the user.
+        Send an "acknowledged" message marker (:xep:`0333`) from this :term:`XMPP Entity`.
 
         :param legacy_msg_id: The message this marker refers to
         """
         self._send(
             self._make_marker(
                 legacy_msg_id, "acknowledged", carbon=kwargs.get("carbon")
             ),
             **kwargs,
         )
 
     def received(self, legacy_msg_id: LegacyMessageType, **kwargs):
         """
-        Send a "received" message marker (:xep:`0333`) and a "message delivery receipt"
-        (:xep:`0184`)
-        from this contact to the user
+        Send a "received" message marker (:xep:`0333`) from this :term:`XMPP Entity`.
+        If called on a :class:`LegacyContact`, also send a delivery receipt
+        marker (:xep:`0184`).
 
         :param legacy_msg_id: The message this marker refers to
         """
         carbon = kwargs.get("carbon")
-        if not self.is_group:
-            # msg receipts are NOT RECOMMENDED for MUCs
-            self._send(self._make_receipt(legacy_msg_id, carbon=carbon), **kwargs)
+        if self.mtype == "chat":
+            self._send(
+                self.xmpp.delivery_receipt.make_ack(
+                    self._legacy_to_xmpp(legacy_msg_id),
+                    mfrom=self.jid,
+                    mto=self.user.jid,
+                )
+            )
         self._send(
             self._make_marker(legacy_msg_id, "received", carbon=carbon), **kwargs
         )
 
     def displayed(self, legacy_msg_id: LegacyMessageType, **kwargs):
         """
-        Send a "displayed" message marker (:xep:`0333`) from this contact to the user.
+        Send a "displayed" message marker (:xep:`0333`) from this :term:`XMPP Entity`.
 
         :param legacy_msg_id: The message this marker refers to
         """
         self._send(
             self._make_marker(legacy_msg_id, "displayed", carbon=kwargs.get("carbon")),
             **kwargs,
         )
+        if getattr(self, "is_user", False):
+            self.session.create_task(self.__send_mds(legacy_msg_id))
 
-
-class ContentMessageMixin(MessageMaker):
-    async def _upload(
-        self,
-        filename: Union[Path, str],
-        content_type: Optional[str] = None,
-        input_file: Optional[IO[bytes]] = None,
-        url: Optional[str] = None,
-    ):
-        if url is not None:
-            if input_file is not None:
-                raise TypeError("Either a URL or a file-like object")
-            async with aiohttp.ClientSession() as session:
-                async with session.get(url) as r:
-                    input_file = BytesIO(await r.read())
+    async def __send_mds(self, legacy_msg_id: LegacyMessageType):
+        # Send a MDS displayed marker on behalf of the user for a group chat
+        if muc := getattr(self, "muc", None):
+            muc_jid = muc.jid.bare
+        else:
+            # This is not implemented for 1:1 chat because it would rely on
+            # storing the XMPP-server injected stanza-id, which we don't track
+            # ATM.
+            # In practice, MDS should mostly be useful for public group chats,
+            # so it should not be an issue.
+            # We'll see if we need to implement that later
+            return
+        xmpp_msg_id = self._legacy_to_xmpp(legacy_msg_id)
+        iq = Iq(sto=self.user.bare_jid, sfrom=self.user.bare_jid, stype="set")
+        iq["pubsub"]["publish"]["node"] = self.xmpp["xep_0490"].stanza.NS
+        iq["pubsub"]["publish"]["item"]["id"] = muc_jid
+        displayed = self.xmpp["xep_0490"].stanza.Displayed()
+        displayed["stanza_id"]["id"] = xmpp_msg_id
+        displayed["stanza_id"]["by"] = muc_jid
+        iq["pubsub"]["publish"]["item"]["payload"] = displayed
+        iq["pubsub"]["publish_options"] = PUBLISH_OPTIONS
         try:
-            return await self.xmpp["xep_0363"].upload_file(
-                filename=filename,
-                content_type=content_type,
-                input_file=input_file,
-                ifrom=config.UPLOAD_REQUESTER or self.xmpp.boundjid,
-            )
-        except FileUploadError as e:
-            log.warning(
-                "Something is wrong with the upload service, see the traceback below"
-            )
-            log.exception(e)
+            await self.xmpp["xep_0356"].send_privileged_iq(iq)
+        except Exception as e:
+            self.session.log.debug("Could not MDS mark", exc_info=e)
+
+
+class ContentMessageMixin(AttachmentMixin):
+    def __default_hints(self, hints: Optional[Iterable[ProcessingHint]] = None):
+        if hints is not None:
+            return hints
+        elif self.mtype == "chat":
+            return {"markable", "store"}
+        elif self.mtype == "groupchat":
+            return {"markable"}
+
+    def __replace_id(self, legacy_msg_id: LegacyMessageType):
+        if self.mtype == "groupchat":
+            return self.session.muc_sent_msg_ids.get(
+                legacy_msg_id
+            ) or self._legacy_to_xmpp(legacy_msg_id)
+        else:
+            return self._legacy_to_xmpp(legacy_msg_id)
 
     def send_text(
         self,
         body: str,
         legacy_msg_id: Optional[LegacyMessageType] = None,
         *,
         when: Optional[datetime] = None,
-        reply_to_msg_id: Optional[LegacyMessageType] = None,
-        reply_to_fallback_text: Optional[str] = None,
-        reply_to_jid: Optional[JID] = None,
-        **kwargs,
+        reply_to: Optional[MessageReference] = None,
+        thread: Optional[LegacyThreadType] = None,
+        hints: Optional[Iterable[ProcessingHint]] = None,
+        carbon=False,
+        archive_only=False,
+        correction=False,
+        correction_event_id: Optional[LegacyMessageType] = None,
+        link_previews: Optional[list[LinkPreview]] = None,
+        **send_kwargs,
     ):
         """
-        Transmit a message from the entity to the user
+        Send a text message from this :term:`XMPP Entity`.
 
-        :param body: Context of the message
+        :param body: Content of the message
         :param legacy_msg_id: If you want to be able to transport read markers from the gateway
             user to the legacy network, specify this
         :param when: when the message was sent, for a "delay" tag (:xep:`0203`)
-        :param reply_to_msg_id: Quote another message (:xep:`0461`)
-        :param reply_to_fallback_text: Fallback text for clients not supporting :xep:`0461`
-        :param reply_to_jid: JID of the quoted message author
+        :param reply_to: Quote another message (:xep:`0461`)
+        :param hints:
+        :param thread:
+        :param carbon: (only used if called on a :class:`LegacyContact`)
+            Set this to ``True`` if this is actually a message sent **to** the
+            :class:`LegacyContact` by the :term:`User`.
+            Use this to synchronize outgoing history for legacy official apps.
+        :param correction: whether this message is a correction or not
+        :param correction_event_id: in the case where an ID is associated with the legacy
+            'correction event', specify it here to use it on the XMPP side. If not specified,
+            a random ID will be used.
+        :param link_previews: A little of sender (or server, or gateway)-generated
+            previews of URLs linked in the body.
+        :param archive_only: (only in groups) Do not send this message to user,
+            but store it in the archive. Meant to be used during ``MUC.backfill()``
         """
+        if carbon:
+            if not correction and legacy_msg_id in self.session.sent:
+                log.warning(
+                    "Carbon message for a message an XMPP has sent? This is a bug! %s",
+                    legacy_msg_id,
+                )
+                return
+            self.session.sent[legacy_msg_id] = self.session.legacy_to_xmpp_msg_id(
+                legacy_msg_id
+            )
+        hints = self.__default_hints(hints)
         msg = self._make_message(
             mbody=body,
-            legacy_msg_id=legacy_msg_id,
+            legacy_msg_id=correction_event_id if correction else legacy_msg_id,
             when=when,
-            reply_to_msg_id=reply_to_msg_id,
-            reply_to_fallback_text=reply_to_fallback_text,
-            reply_to_jid=reply_to_jid,
-            hints=kwargs.get("hints") or {"markable", "store"},
-            carbon=kwargs.get("carbon"),
+            reply_to=reply_to,
+            hints=hints or (),
+            carbon=carbon,
+            thread=thread,
+            link_previews=link_previews,
         )
-        self._send(msg, **kwargs)
+        if correction:
+            msg["replace"]["id"] = self.__replace_id(legacy_msg_id)
+        return self._send(msg, archive_only=archive_only, carbon=carbon, **send_kwargs)
 
-    async def send_file(
+    def correct(
         self,
-        filename: Union[Path, str],
-        legacy_msg_id: Optional[LegacyMessageType] = None,
+        legacy_msg_id: LegacyMessageType,
+        new_text: str,
         *,
-        content_type: Optional[str] = None,
-        input_file: Optional[IO[bytes]] = None,
-        url: Optional[str] = None,
-        reply_to_msg_id: Optional[LegacyMessageType] = None,
-        reply_to_fallback_text: Optional[str] = None,
-        reply_to_jid: Optional[JID] = None,
         when: Optional[datetime] = None,
-        caption: Optional[str] = None,
-        **kwargs,
+        reply_to: Optional[MessageReference] = None,
+        thread: Optional[LegacyThreadType] = None,
+        hints: Optional[Iterable[ProcessingHint]] = None,
+        carbon=False,
+        archive_only=False,
+        correction_event_id: Optional[LegacyMessageType] = None,
+        link_previews: Optional[list[LinkPreview]] = None,
+        **send_kwargs,
     ):
         """
-        Send a file using HTTP upload (:xep:`0363`)
+        Modify a message that was previously sent by this :term:`XMPP Entity`.
 
-        :param filename: Filename to use or location on disk to the file to upload
-        :param content_type: MIME type, inferred from filename if not given
-        :param input_file: Optionally, a file like object instead of a file on disk.
-            filename will still be used to give the uploaded file a name
-        :param legacy_msg_id: If you want to be able to transport read markers from the gateway
-            user to the legacy network, specify this
-        :param url: Optionally, a URL of a file that slidge will download and upload to the
-            default file upload service on the xmpp server it's running on. url and input_file
-            are mutually exclusive.
-        :param reply_to_msg_id: Quote another message (:xep:`0461`)
-        :param reply_to_fallback_text: Fallback text for clients not supporting :xep:`0461`
-        :param reply_to_jid: JID of the quoted message author
-        :param when: when the file was sent, for a "delay" tag (:xep:`0203`)
-        :param caption: an optional text that is linked to the file
-        """
-        carbon = kwargs.pop("carbon", False)
-        msg = self._make_message(
+        Uses last message correction (:xep:`0308`)
+
+        :param new_text: New content of the message
+        :param legacy_msg_id: The legacy message ID of the message to correct
+        :param when: when the message was sent, for a "delay" tag (:xep:`0203`)
+        :param reply_to: Quote another message (:xep:`0461`)
+        :param hints:
+        :param thread:
+        :param carbon: (only in 1:1) Reflect a message sent to this ``Contact`` by the user.
+            Use this to synchronize outgoing history for legacy official apps.
+        :param archive_only: (only in groups) Do not send this message to user,
+            but store it in the archive. Meant to be used during ``MUC.backfill()``
+        :param correction_event_id: in the case where an ID is associated with the legacy
+            'correction event', specify it here to use it on the XMPP side. If not specified,
+            a random ID will be used.
+        :param link_previews: A little of sender (or server, or gateway)-generated
+            previews of URLs linked in the body.
+        """
+        self.send_text(
+            new_text,
+            legacy_msg_id,
             when=when,
-            reply_to_msg_id=reply_to_msg_id,
-            reply_to_fallback_text=reply_to_fallback_text,
-            reply_to_jid=reply_to_jid,
+            reply_to=reply_to,
+            hints=hints,
             carbon=carbon,
+            thread=thread,
+            correction=True,
+            archive_only=archive_only,
+            correction_event_id=correction_event_id,
+            link_previews=link_previews,
+            **send_kwargs,
         )
-        uploaded_url = await self._upload(filename, content_type, input_file, url)
-        if uploaded_url is None:
-            if url is not None:
-                uploaded_url = url
-            else:
-                msg["body"] = (
-                    "I tried to send a file, but something went wrong. "
-                    "Tell your XMPP admin to check slidge logs."
-                )
-                self._set_msg_id(msg, legacy_msg_id)
-                self._send(msg, **kwargs)
-                return
-
-        msg["oob"]["url"] = uploaded_url
-        msg["body"] = uploaded_url
-        if caption:
-            self._send(msg, carbon=carbon, **kwargs)
-            self.send_text(
-                caption, legacy_msg_id=legacy_msg_id, when=when, carbon=carbon, **kwargs
-            )
-        else:
-            self._set_msg_id(msg, legacy_msg_id)
-            self._send(msg, **kwargs)
-
-    def correct(self, legacy_msg_id: LegacyMessageType, new_text: str, **kwargs):
-        """
-        Call this when a legacy contact has modified his last message content.
-
-        Uses last message correction (:xep:`0308`)
-
-        :param legacy_msg_id: Legacy message ID this correction refers to
-        :param new_text: The new text
-        """
-        msg = self._make_message(mbody=new_text, carbon=kwargs.get("carbon"))
-        msg["replace"]["id"] = self._legacy_to_xmpp(legacy_msg_id)
-        self._send(msg, **kwargs)
 
     def react(
-        self, legacy_msg_id: LegacyMessageType, emojis: Iterable[str] = (), **kwargs
+        self,
+        legacy_msg_id: LegacyMessageType,
+        emojis: Iterable[str] = (),
+        thread: Optional[LegacyThreadType] = None,
+        **kwargs,
     ):
         """
-        Call this when a legacy contact reacts to a message
+        Send a reaction (:xep:`0444`) from this :term:`XMPP Entity`.
 
         :param legacy_msg_id: The message which the reaction refers to.
-        :param emojis: A iterable of emojis used as reactions
-        :return:
+        :param emojis: An iterable of emojis used as reactions
+        :param thread:
         """
-        msg = self._make_message(hints={"store"}, carbon=kwargs.get("carbon"))
-        xmpp_id = self._legacy_to_xmpp(legacy_msg_id)
+        msg = self._make_message(
+            hints={"store"}, carbon=kwargs.get("carbon"), thread=thread
+        )
+        xmpp_id = kwargs.pop("xmpp_id", None)
+        if not xmpp_id:
+            xmpp_id = self._legacy_to_xmpp(legacy_msg_id)
         self.xmpp["xep_0444"].set_reactions(msg, to_id=xmpp_id, reactions=emojis)
         self._send(msg, **kwargs)
 
-    def retract(self, legacy_msg_id: LegacyMessageType, **kwargs):
+    def retract(
+        self,
+        legacy_msg_id: LegacyMessageType,
+        thread: Optional[LegacyThreadType] = None,
+        **kwargs,
+    ):
         """
-        Call this when a legacy contact retracts (:XEP:`0424`) a message
+        Send a message retraction (:XEP:`0424`) from this :term:`XMPP Entity`.
 
         :param legacy_msg_id: Legacy ID of the message to delete
+        :param thread:
         """
         msg = self._make_message(
             state=None,
             hints={"store"},
-            mbody=f"I have deleted the message {legacy_msg_id}, "
-            "but your XMPP client does not support that",
+            mbody=f"/me retracted the message {legacy_msg_id}",
             carbon=kwargs.get("carbon"),
+            thread=thread,
         )
         msg.enable("fallback")
-        msg["apply_to"]["id"] = self._legacy_to_xmpp(legacy_msg_id)
-        msg["apply_to"].enable("retract")
+        # namespace version mismatch between slidge and slixmpp, update me later
+        msg["fallback"]["for"] = self.xmpp["xep_0424"].namespace[:-1] + "1"
+        msg["retract"]["id"] = msg["replace"]["id"] = self.__replace_id(legacy_msg_id)
         self._send(msg, **kwargs)
 
 
 class CarbonMessageMixin(ContentMessageMixin, MarkerMixin):
     def _privileged_send(self, msg: Message):
-        self.session.ignore_messages.add(msg.get_id())
+        i = msg.get_id()
+        if not i:
+            i = str(uuid.uuid4())
+            msg.set_id(i)
+        msg.del_origin_id()
+        self.session.ignore_messages.add(i)
         try:
             self.xmpp["xep_0356"].send_privileged_message(msg)
         except PermissionError:
             try:
                 self.xmpp["xep_0356_old"].send_privileged_message(msg)
             except PermissionError:
-                log.warning(
-                    "Slidge does not have privileges to send message on behalf of user."
-                    "Refer to https://slidge.readthedocs.io/en/latest/admin/xmpp_server.html "
-                    "for more info."
+                warnings.warn(
+                    "Slidge does not have privileges to send message on behalf of"
+                    " user.Refer to"
+                    " https://slidge.readthedocs.io/en/latest/admin/xmpp_server.html"
+                    " for more info."
                 )
 
 
-class MessageMixin(ChatStateMixin, MarkerMixin, ContentMessageMixin):
+class InviteMixin(MessageMaker):
+    def invite_to(
+        self,
+        muc: "LegacyMUC",
+        reason: Optional[str] = None,
+        password: Optional[str] = None,
+        **send_kwargs,
+    ):
+        """
+        Send an invitation to join a group (:xep:`0249`) from this :term:`XMPP Entity`.
+
+        :param muc: the muc the user is invited to
+        :param reason: a text explaining why the user should join this muc
+        :param password: maybe this will make sense later? not sure
+        :param send_kwargs: additional kwargs to be passed to _send()
+            (internal use by slidge)
+        """
+        msg = self._make_message(mtype="normal")
+        msg["groupchat_invite"]["jid"] = muc.jid
+        if reason:
+            msg["groupchat_invite"]["reason"] = reason
+        if password:
+            msg["groupchat_invite"]["password"] = password
+        self._send(msg, **send_kwargs)
+
+
+class MessageMixin(InviteMixin, ChatStateMixin, MarkerMixin, ContentMessageMixin):
     pass
 
 
-class MessageCarbonMixin(ChatStateMixin, CarbonMessageMixin):
+class MessageCarbonMixin(InviteMixin, ChatStateMixin, CarbonMessageMixin):
     pass
 
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/core/pubsub.py` & `slidge-0.1.1/slidge/core/pubsub.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,120 +1,189 @@
-import asyncio
 import hashlib
 import io
 import logging
 from copy import copy
 from pathlib import Path
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Type, Union
 
 from PIL import Image, UnidentifiedImageError
-from slixmpp import JID, ComponentXMPP, CoroutineCallback, Iq, Presence, StanzaPath
+from PIL.Image import Image as PILImage
+from slixmpp import (
+    JID,
+    CoroutineCallback,
+    Iq,
+    Presence,
+    StanzaPath,
+    register_stanza_plugin,
+)
 from slixmpp.exceptions import XMPPError
 from slixmpp.plugins.base import BasePlugin, register_plugin
 from slixmpp.plugins.xep_0060.stanza import Event, EventItem, EventItems, Item
 from slixmpp.plugins.xep_0084 import Data as AvatarData
 from slixmpp.plugins.xep_0084 import MetaData as AvatarMetadata
 from slixmpp.plugins.xep_0172 import UserNick
+from slixmpp.plugins.xep_0292.stanza import VCard4
 from slixmpp.types import JidStr, OptJidStr
 
-from ..util.db import user_store
-from ..util.types import AvatarType, PepItemType
-from ..util.xep_0292.stanza import VCard4
-from . import config
-from .cache import avatar_cache
+from ..contact.contact import LegacyContact
+from ..contact.roster import ContactIsUser
+from ..util.db import GatewayUser, user_store
+from ..util.sql import db
+from ..util.types import AvatarType, LegacyFileIdType, PepItemType
+from .cache import CachedAvatar, avatar_cache
+from .mixins.lock import NamedLockMixin
+
+if TYPE_CHECKING:
+    from slidge import BaseGateway
 
 VCARD4_NAMESPACE = "urn:xmpp:vcard4"
 
 
 class PepItem:
-    def __init__(self, authorized_jid: Optional[JidStr] = None):
-        self.authorized_jid = authorized_jid
+    @staticmethod
+    def from_db(jid: JID, user: Optional[GatewayUser] = None) -> Optional["PepItem"]:
+        raise NotImplementedError
+
+    def to_db(self, jid: JID, user: Optional[GatewayUser] = None):
+        raise NotImplementedError
 
 
 class PepAvatar(PepItem):
-    def __init__(self, authorized_jid: Optional[JidStr] = None):
-        super().__init__(authorized_jid)
+    def __init__(self, jid: JID):
         self.metadata: Optional[AvatarMetadata] = None
-        self.data: Optional[AvatarData] = None
         self.id: Optional[str] = None
+        self.jid = jid
+        self._avatar_data_path: Optional[Path] = None
+
+    @property
+    def data(self) -> Optional[AvatarData]:
+        if self._avatar_data_path is None:
+            return None
+        data = AvatarData()
+        data.set_value(self._avatar_data_path.read_bytes())
+        return data
+
+    @staticmethod
+    def _sha(b: bytes):
+        return hashlib.sha1(b).hexdigest()
+
+    def _get_weak_unique_id(self, avatar: AvatarType):
+        if isinstance(avatar, str):
+            return avatar  # url
+        elif isinstance(avatar, bytes):
+            return self._sha(avatar)
+        elif isinstance(avatar, Path):
+            return self._sha(avatar.read_bytes())
 
-    async def set_avatar(self, avatar: AvatarType):
+    @staticmethod
+    async def _get_image(avatar: AvatarType) -> PILImage:
         if isinstance(avatar, str):
-            return await self.set_avatar_from_url(avatar)
+            # async with aiohttp.ClientSession() as session:
+            async with avatar_cache.http.get(avatar) as response:
+                return Image.open(io.BytesIO(await response.read()))
         elif isinstance(avatar, bytes):
-            img = Image.open(io.BytesIO(avatar))
+            return Image.open(io.BytesIO(avatar))
         elif isinstance(avatar, Path):
-            img = Image.open(avatar)
+            return Image.open(avatar)
         else:
             raise TypeError("Avatar must be bytes, a Path or a str (URL)", avatar)
 
-        metadata = AvatarMetadata()
+    async def set_avatar(
+        self, avatar: AvatarType, unique_id: Optional[LegacyFileIdType] = None
+    ):
+        if unique_id is None:
+            if isinstance(avatar, str):
+                await self._set_avatar_from_url_alone(avatar)
+                return
+            unique_id = self._get_weak_unique_id(avatar)
 
-        resampled = False
-        if (size := config.AVATAR_SIZE) and any(x > size for x in img.size):
-            img.thumbnail((size, size))
-            log.debug("Resampled image to %s", img.size)
-            resampled = True
-
-        if not resampled and img.format == "PNG" and isinstance(avatar, bytes):
-            avatar_bytes = avatar
-        elif not resampled and img.format == "PNG" and isinstance(avatar, Path):
-            with avatar.open("rb") as f:
-                avatar_bytes = f.read()
+        await self._set_avatar_from_unique_id(avatar, unique_id)
+
+    async def _set_avatar_from_unique_id(
+        self, avatar: AvatarType, unique_id: LegacyFileIdType
+    ):
+        cached_avatar = avatar_cache.get(unique_id)
+        if cached_avatar:
+            # this shouldn't be necessary but here to re-use avatars downloaded
+            # before the change introducing the JID to unique ID mapping
+            avatar_cache.store_jid(self.jid, unique_id)
         else:
-            with io.BytesIO() as f:
-                img.save(f, format="PNG")
-                avatar_bytes = f.getvalue()
+            img = await self._get_image(avatar)
+            cached_avatar = await avatar_cache.convert_and_store(
+                img, unique_id, self.jid
+            )
 
-        hash_ = hashlib.sha1(avatar_bytes).hexdigest()
-        self.id = hash_
-        metadata.add_info(
-            id=hash_,
-            itype="image/png",
-            ibytes=len(avatar_bytes),
-            height=str(img.height),
-            width=str(img.width),
-        )
-        self.metadata = metadata
+        self._set_avatar_from_cache(cached_avatar)
 
-        data = AvatarData()
-        data.set_value(avatar_bytes)
-        self.data = data
+    async def _set_avatar_from_url_alone(self, url: str):
+        cached_avatar = await avatar_cache.get_avatar_from_url_alone(url, self.jid)
+        self._set_avatar_from_cache(cached_avatar)
 
-    async def set_avatar_from_url(self, url: str):
-        avatar = await avatar_cache.get_avatar(url)
+    def _set_avatar_from_cache(self, cached_avatar: CachedAvatar):
         metadata = AvatarMetadata()
-        self.id = avatar.hash
+        self.id = cached_avatar.hash
         metadata.add_info(
-            id=avatar.hash,
+            id=cached_avatar.hash,
             itype="image/png",
-            ibytes=len(avatar.data),
-            height=str(avatar.height),
-            width=str(avatar.width),
+            ibytes=cached_avatar.path.stat().st_size,
+            height=str(cached_avatar.height),
+            width=str(cached_avatar.width),
         )
         self.metadata = metadata
+        self._avatar_data_path = cached_avatar.path
 
-        data = AvatarData()
-        data.set_value(avatar.data)
-        self.data = data
+    @staticmethod
+    def from_db(jid: JID, user: Optional[GatewayUser] = None) -> Optional["PepAvatar"]:
+        cached_id = db.avatar_get(jid)
+        if cached_id is None:
+            return None
+        item = PepAvatar(jid)
+        cached_avatar = avatar_cache.get(cached_id)
+        if cached_avatar is None:
+            raise XMPPError("internal-server-error")
+        item._set_avatar_from_cache(cached_avatar)
+        return item
+
+    def to_db(self, jid: JID, user=None):
+        cached_id = avatar_cache.get_cached_id_for(jid)
+        if cached_id is None:
+            log.warning("Could not store avatar for %s", jid)
+            return
+        db.avatar_store(jid, cached_id)
+
+    @staticmethod
+    def remove_from_db(jid: JID):
+        db.avatar_delete(jid)
 
 
 class PepNick(PepItem):
-    def __init__(
-        self, authorized_jid: Optional[JidStr] = None, nick: Optional[str] = None
-    ):
-        super().__init__(authorized_jid)
+    def __init__(self, nick: Optional[str] = None):
         nickname = UserNick()
         if nick is not None:
             nickname["nick"] = nick
         self.nick = nickname
+        self.__nick_str = nick
+
+    @staticmethod
+    def from_db(jid: JID, user: Optional[GatewayUser] = None) -> Optional["PepNick"]:
+        if user is None:
+            raise XMPPError("not-allowed")
+        nick = db.nick_get(jid, user)
+        if nick is None:
+            return None
+        return PepNick(nick)
+
+    def to_db(self, jid: JID, user: Optional[GatewayUser] = None):
+        if user is None:
+            raise XMPPError("not-allowed")
+        db.nick_store(jid, str(self.__nick_str), user)
 
 
-class PubSubComponent(BasePlugin):
-    xmpp: ComponentXMPP
+class PubSubComponent(NamedLockMixin, BasePlugin):
+    xmpp: "BaseGateway"
 
     name = "pubsub"
     description = "Pubsub component"
     dependencies = {
         "xep_0030",
         "xep_0060",
         # "xep_0084",
@@ -122,16 +191,15 @@
         "xep_0163",
     }
     default_config = {"component_name": None}
     component_name: str
 
     def __init__(self, *a, **kw):
         super(PubSubComponent, self).__init__(*a, **kw)
-        self._avatars = dict[JID, PepAvatar]()
-        self._nicks = dict[JID, PepNick]()
+        register_stanza_plugin(EventItem, UserNick)
 
     def plugin_init(self):
         self.xmpp.register_handler(
             CoroutineCallback(
                 "pubsub_get_avatar_data",
                 StanzaPath(f"iq@type=get/pubsub/items@node={AvatarData.namespace}"),
                 self._get_avatar_data,  # type:ignore
@@ -147,110 +215,143 @@
         self.xmpp.register_handler(
             CoroutineCallback(
                 "pubsub_get_vcard",
                 StanzaPath(f"iq@type=get/pubsub/items@node={VCARD4_NAMESPACE}"),
                 self._get_vcard,  # type:ignore
             )
         )
-        self.xmpp.add_event_handler("got_online", self._on_got_online)
+        self.xmpp.add_event_handler("presence_available", self._on_presence_available)
 
         disco = self.xmpp.plugin["xep_0030"]
         disco.add_identity("pubsub", "pep", self.component_name)
         disco.add_identity("account", "registered", self.component_name)
         disco.add_feature("http://jabber.org/protocol/pubsub#event")
         disco.add_feature("http://jabber.org/protocol/pubsub#retrieve-items")
         disco.add_feature("http://jabber.org/protocol/pubsub#persistent-items")
 
-    async def _on_got_online(self, p: Presence):
+    async def _on_presence_available(self, p: Presence):
+        if p.get_plugin("muc_join", check=True) is not None:
+            log.debug("Ignoring MUC presence here")
+            return
+
         from_ = p.get_from()
         ver_string = p["caps"]["ver"]
         info = None
+
+        to = p.get_to()
+
+        # we don't want to push anything for contacts that are not in the user's roster
+        if to != self.xmpp.boundjid.bare:
+            session = self.xmpp.get_session_from_stanza(p)
+
+            if session is None:
+                return
+
+            await session.contacts.ready
+            try:
+                contact = await session.contacts.by_jid(to)
+            except XMPPError as e:
+                log.debug(
+                    "Could not determine if %s was added to the roster: %s", to, e
+                )
+                return
+            except Exception as e:
+                log.warning("Could not determine if %s was added to the roster.", to)
+                log.exception(e)
+                return
+            if not contact.is_friend:
+                return
+
         if ver_string:
-            await asyncio.sleep(5)
             info = await self.xmpp.plugin["xep_0115"].get_caps(from_)
         if info is None:
-            info = await self.xmpp.plugin["xep_0030"].get_info(from_)
+            async with self.lock(from_):
+                iq = await self.xmpp.plugin["xep_0030"].get_info(from_)
+            info = iq["disco_info"]
         features = info["features"]
         if AvatarMetadata.namespace + "+notify" in features:
             try:
-                pep_avatar = self._get_authorized_avatar(p)
+                pep_avatar = await self._get_authorized_avatar(p)
             except XMPPError:
                 pass
             else:
-                self._broadcast(
+                if pep_avatar.metadata is None:
+                    raise XMPPError("internal-server-error", "Avatar but no metadata?")
+                await self._broadcast(
                     data=pep_avatar.metadata,
                     from_=p.get_to(),
                     to=from_,
                     id=pep_avatar.metadata["info"]["id"],
                 )
         if UserNick.namespace + "+notify" in features:
             try:
-                pep_nick = self._get_authorized_nick(p)
+                pep_nick = await self._get_authorized_nick(p)
             except XMPPError:
                 pass
             else:
-                self._broadcast(data=pep_nick.nick, from_=p.get_to(), to=from_)
+                await self._broadcast(data=pep_nick.nick, from_=p.get_to(), to=from_)
 
         if VCARD4_NAMESPACE + "+notify" in features:
-            self.broadcast_vcard_event(p.get_to(), to=from_)
+            await self.broadcast_vcard_event(p.get_to(), to=from_)
 
-    def broadcast_vcard_event(self, from_, to):
+    async def broadcast_vcard_event(self, from_, to):
         item = Item()
         item.namespace = VCARD4_NAMESPACE
         item["id"] = "current"
-        vcard: VCard4 = self.xmpp["xep_0292_provider"].get_vcard(from_, to)
+        vcard: VCard4 = await self.xmpp["xep_0292_provider"].get_vcard(from_, to)
         # The vcard content should NOT be in this event according to the spec:
         # https://xmpp.org/extensions/xep-0292.html#sect-idm45669698174224
         # but movim expects it to be here, and I guess
 
         log.debug("Broadcast vcard4 event: %s", vcard)
-        self._broadcast(
+        await self._broadcast(
             data=vcard,
             from_=JID(from_).bare,
             to=to,
             id="current",
             node=VCARD4_NAMESPACE,
         )
 
-    @staticmethod
-    def _get_authorized_item(
-        store: dict[JID, PepItemType], stanza: Union[Iq, Presence]
+    async def _get_authorized_item(
+        self, cls: Type[PepItemType], stanza: Union[Iq, Presence]
     ) -> PepItemType:
-        item = store.get(stanza.get_to())
+        sto = stanza.get_to()
+        user = user_store.get_by_jid(stanza.get_from())
+        item = cls.from_db(sto, user)
         if item is None:
             raise XMPPError("item-not-found")
 
-        if item.authorized_jid is not None:
-            if stanza.get_from().bare != item.authorized_jid:
-                raise XMPPError("item-not-found")
+        if sto != self.xmpp.boundjid.bare:
+            session = self.xmpp.get_session_from_stanza(stanza)
+            await session.contacts.by_jid(sto)
 
-        return item
+        return item  # type:ignore
 
-    def _get_authorized_avatar(self, stanza: Union[Iq, Presence]):
-        return self._get_authorized_item(self._avatars, stanza)
+    async def _get_authorized_avatar(self, stanza: Union[Iq, Presence]) -> PepAvatar:
+        return await self._get_authorized_item(PepAvatar, stanza)
 
-    def _get_authorized_nick(self, stanza: Union[Iq, Presence]):
-        return self._get_authorized_item(self._nicks, stanza)
+    async def _get_authorized_nick(self, stanza: Union[Iq, Presence]) -> PepNick:
+        return await self._get_authorized_item(PepNick, stanza)
 
     async def _get_avatar_data(self, iq: Iq):
-        pep_avatar = self._get_authorized_avatar(iq)
+        pep_avatar = await self._get_authorized_avatar(iq)
 
         requested_items = iq["pubsub"]["items"]
         if len(requested_items) == 0:
             self._reply_with_payload(iq, pep_avatar.data, pep_avatar.id)
         else:
             for item in requested_items:
                 if item["id"] == pep_avatar.id:
                     self._reply_with_payload(iq, pep_avatar.data, pep_avatar.id)
                     return
             else:
                 raise XMPPError("item-not-found")
 
     async def _get_avatar_metadata(self, iq: Iq):
-        pep_avatar = self._get_authorized_avatar(iq)
+        pep_avatar = await self._get_authorized_avatar(iq)
 
         requested_items = iq["pubsub"]["items"]
         if len(requested_items) == 0:
             self._reply_with_payload(iq, pep_avatar.metadata, pep_avatar.id)
         else:
             for item in requested_items:
                 if item["id"] == pep_avatar.id:
@@ -259,41 +360,59 @@
             else:
                 raise XMPPError("item-not-found")
 
     async def _get_vcard(self, iq: Iq):
         # this is not the proper way that clients should retrieve VCards, but
         # gajim does it this way.
         # https://xmpp.org/extensions/xep-0292.html#sect-idm45669698174224
-        vcard: VCard4 = self.xmpp["xep_0292_provider"].get_vcard(
+        vcard: VCard4 = await self.xmpp["xep_0292_provider"].get_vcard(
             iq.get_to().bare, iq.get_from().bare
         )
         log.debug("VCARD: %s -- %s -- %s", iq.get_to().bare, iq.get_from().bare, vcard)
         if vcard is None:
             raise XMPPError("item-not-found")
         self._reply_with_payload(iq, vcard, "current", VCARD4_NAMESPACE)
 
     @staticmethod
+    def get_avatar(jid: JID):
+        return PepAvatar.from_db(jid)
+
+    @staticmethod
     def _reply_with_payload(
         iq: Iq,
-        payload: Union[AvatarMetadata, AvatarData, VCard4],
-        id_: str,
+        payload: Optional[Union[AvatarMetadata, AvatarData, VCard4]],
+        id_: Optional[str],
         namespace: Optional[str] = None,
     ):
         result = iq.reply()
         item = Item()
         if payload:
             item.set_payload(payload.xml)
-        item["id"] = id_
-        result["pubsub"]["items"]["node"] = (
-            namespace if namespace else payload.namespace
-        )
+            item["id"] = id_
+            result["pubsub"]["items"]["node"] = (
+                namespace if namespace else payload.namespace
+            )
         result["pubsub"]["items"].append(item)
         result.send()
 
-    def _broadcast(self, data, from_: JidStr, to: OptJidStr = None, **kwargs):
+    async def _broadcast(self, data, from_: JidStr, to: OptJidStr = None, **kwargs):
+        from_ = JID(from_)
+        if from_ != self.xmpp.boundjid.bare and to is not None:
+            to = JID(to)
+            session = self.xmpp.get_session_from_jid(to)
+            if session is None:
+                return
+            await session.ready
+            try:
+                entity = await session.get_contact_or_group_or_participant(from_)
+            except ContactIsUser:
+                return
+            if isinstance(entity, LegacyContact) and not entity.is_friend:
+                return
+
         item = EventItem()
         if data:
             item.set_payload(data.xml)
         for k, v in kwargs.items():
             item[k] = v
 
         items = EventItems()
@@ -317,50 +436,90 @@
             msg.set_to(to)
             msg.send()
 
     async def set_avatar(
         self,
         jid: JidStr,
         avatar: Optional[AvatarType] = None,
-        restrict_to: OptJidStr = None,
+        broadcast_to: OptJidStr = None,
+        unique_id=None,
+        broadcast=True,
     ):
         jid = JID(jid)
         if avatar is None:
-            try:
-                del self._avatars[jid]
-            except KeyError:
-                pass
-            self._broadcast(AvatarMetadata(), jid, restrict_to)
+            PepAvatar.remove_from_db(jid)
+            await self._broadcast(AvatarMetadata(), jid, broadcast_to)
+            avatar_cache.delete_jid(jid)
         else:
-            pep_avatar = PepAvatar()
+            pep_avatar = PepAvatar(jid)
             try:
-                await pep_avatar.set_avatar(avatar)
-            except UnidentifiedImageError as e:
+                await pep_avatar.set_avatar(avatar, unique_id)
+            except (UnidentifiedImageError, FileNotFoundError) as e:
                 log.warning("Failed to set avatar for %s: %r", self, e)
                 return
-
-            pep_avatar.authorized_jid = restrict_to
-            self._avatars[jid] = pep_avatar
+            pep_avatar.to_db(jid)
             if pep_avatar.metadata is None:
                 raise RuntimeError
-            self._broadcast(
+            if not broadcast:
+                return
+            await self._broadcast(
                 pep_avatar.metadata,
                 jid,
-                restrict_to,
+                broadcast_to,
                 id=pep_avatar.metadata["info"]["id"],
             )
 
+    async def set_avatar_from_cache(
+        self, jid: JID, send_empty: bool, broadcast_to: OptJidStr = None, broadcast=True
+    ):
+        uid = avatar_cache.get_cached_id_for(jid)
+        if uid is None:
+            if not send_empty:
+                return
+            self.xmpp.loop.create_task(
+                self.set_avatar(jid, None, broadcast_to, uid, broadcast)
+            )
+            return
+        cached_avatar = avatar_cache.get(str(uid))
+        if cached_avatar is None:
+            # should not happen but well…
+            log.warning(
+                "Something is wrong with the avatar, %s won't have an "
+                "avatar because avatar not found in cache",
+                jid,
+            )
+            return
+        self.xmpp.loop.create_task(
+            self.set_avatar(jid, cached_avatar.path, broadcast_to, uid, broadcast)
+        )
+
     def set_nick(
         self,
+        user: GatewayUser,
         jid: JidStr,
         nick: Optional[str] = None,
-        restrict_to: OptJidStr = None,
     ):
         jid = JID(jid)
-        nickname = PepNick(restrict_to, nick)
-        self._nicks[jid] = nickname
-        log.debug("NICK: %s", nickname.nick)
-        self._broadcast(nickname.nick, jid, restrict_to)
+        nickname = PepNick(nick)
+        nickname.to_db(jid, user)
+        log.debug("New nickname: %s", nickname.nick)
+        self.xmpp.loop.create_task(self._broadcast(nickname.nick, jid, user.bare_jid))
+
+    async def broadcast_all(self, from_: JID, to: JID):
+        """
+        Force push avatar and nick for a stored JID.
+        """
+        a = PepAvatar.from_db(from_)
+        if a:
+            if a.metadata:
+                await self._broadcast(
+                    a.metadata, from_, to, id=a.metadata["info"]["id"]
+                )
+            else:
+                log.warning("No metadata associated to this cached avatar?!")
+        n = PepNick.from_db(from_, user_store.get_by_jid(to))
+        if n:
+            await self._broadcast(n.nick, from_, to)
 
 
 log = logging.getLogger(__name__)
 register_plugin(PubSubComponent)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slidge-0.1.0rc1/slidge/plugins/hackernews.py` & `slidge-0.1.1/slidge/command/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,209 +1,250 @@
-"""
-Hackernews slidge plugin
+# Commands available to users
+from typing import TYPE_CHECKING, Any, Optional, Union, cast
 
-Will poll replies to items you've posted.
-For every reply, the chat window '<REPLY_ITEM_ID>@<BRIDGE_JID>' should open.
-It will contain your original post (as a carbon) and its reply as a normal chat message.
-You can re-reply by replying in your XMPP client directly.
-"""
-
-import asyncio
-import logging
-import re
-from datetime import datetime
-from typing import Any, Optional
-
-import aiohttp
-from slixmpp import JID
+from slixmpp import JID  # type:ignore[attr-defined]
 from slixmpp.exceptions import XMPPError
 
-from slidge import *
-
+from ..util.types import AnyBaseSession, LegacyGroupIdType
+from .base import (
+    Command,
+    CommandAccess,
+    Confirmation,
+    Form,
+    FormField,
+    FormValues,
+    SearchResult,
+    TableResult,
+)
+from .categories import CONTACTS, GROUPS
+
+if TYPE_CHECKING:
+    pass
+
+
+class Search(Command):
+    NAME = "🔎 Search for contacts"
+    HELP = "Search for contacts via this gateway"
+    NODE = "search"
+    CHAT_COMMAND = "find"
+    ACCESS = CommandAccess.USER_LOGGED
+    CATEGORY = CONTACTS
+
+    async def run(
+        self, session: Optional[AnyBaseSession], _ifrom: JID, *args: str
+    ) -> Union[Form, SearchResult, None]:
+        if args:
+            assert session is not None
+            return await session.on_search(
+                {self.xmpp.SEARCH_FIELDS[0].var: " ".join(args)}
+            )
+        return Form(
+            title=self.xmpp.SEARCH_TITLE,
+            instructions=self.xmpp.SEARCH_INSTRUCTIONS,
+            fields=self.xmpp.SEARCH_FIELDS,
+            handler=self.search,
+        )
 
-class Gateway(BaseGateway):
-    # FIXME: implement proper login process, but we might have to do something to handle captcha
-    REGISTRATION_INSTRUCTIONS = (
-        "Enter the hackernews cookie from your browser's dev console "
-        "(something like your-user-name ampersand XXXXXXXXXXXXXXXXXXXXXXXXX)"
+    @staticmethod
+    async def search(
+        form_values: FormValues, session: Optional[AnyBaseSession], _ifrom: JID
+    ) -> SearchResult:
+        assert session is not None
+        results = await session.on_search(form_values)  # type: ignore
+        if results is None:
+            raise XMPPError("item-not-found", "No contact was found")
+
+        return results
+
+
+class SyncContacts(Command):
+    NAME = "🔄 Sync XMPP roster"
+    HELP = (
+        "Synchronize your XMPP roster with your legacy contacts. "
+        "Slidge will only add/remove/modify contacts in its dedicated roster group"
     )
-    REGISTRATION_FIELDS = [
-        FormField(var="cookie", label="'user' cookie", required=True),
-    ]
-
-    ROSTER_GROUP = "HN"  # Not used, we don't add anything to the roster
-
-    COMPONENT_NAME = "Hackernews (slidge)"
-    COMPONENT_TYPE = "hackernews"
-
-    COMPONENT_AVATAR = "https://news.ycombinator.com/favicon.ico"
-
-    async def validate(
-        self, user_jid: JID, registration_form: dict[str, Optional[str]]
-    ):
-        if registration_form["cookie"] is None:
-            raise ValueError("A cookie is required")
-        async with aiohttp.ClientSession(
-            cookies={"user": registration_form["cookie"]}
-        ) as session:
-            async with session.get(LOGIN_URL, allow_redirects=False) as r:
-                log.debug("Login response: %s - %s", r.status, await r.text())
-                if r.status != 302:
-                    raise ValueError("Cookie does not seem valid")
-
-
-class Session(BaseSession):
-    def __init__(self, user):
-        super().__init__(user)
-        self.http_session = aiohttp.ClientSession(
-            cookies={"user": self.user.registration_form["cookie"]}  # type: ignore
-        )
-        self.highest_handled_submission_id = 0
-        self.hn_username = self.user.registration_form["cookie"].split("&")[0]  # type: ignore
-
-    async def login(self):
-        kid_ids: list[int] = []
-        for submission_id in await self.get_user_submissions():
-            user_submission = await self.get_item(submission_id)
-            for kid_id in user_submission.get("kids", []):
-                kid_ids.append(kid_id)
-
-        if kid_ids:
-            self.highest_handled_submission_id = max(kid_ids)
-
-        self.xmpp.loop.create_task(self.main_loop())
-        return f"Logged as {self.hn_username}"
-
-    async def main_loop(self):
-        kid_ids: list[int] = []
-        while True:
-            kid_ids.clear()
-            for submission_id in await self.get_user_submissions():
-                try:
-                    user_submission = await self.get_item(submission_id)
-                except aiohttp.ContentTypeError as e:
-                    log.warning("Hackernews API problem: %s")
-                    log.exception(e)
-                    continue
-                for kid_id in user_submission.get("kids", []):
-                    if kid_id <= self.highest_handled_submission_id:
-                        continue
-                    await self.send_own_and_reply(user_submission, kid_id)
-                    kid_ids.append(kid_id)
-            if kid_ids:
-                self.highest_handled_submission_id = max(kid_ids)
-            await asyncio.sleep(POLL_INTERVAL)
-
-    async def get_user_submissions(self) -> list[int]:
-        log.debug("Getting user subs: %s", self.hn_username)
-        async with self.http_session.get(
-            f"{API_URL}/user/{self.hn_username}.json"
-        ) as r:
-            if r.status != 200:
-                log.warning("Bad response from API: %s", r)
-                raise RuntimeError
-            return (await r.json())["submitted"]
-
-    async def send_own_and_reply(self, user_submission, reply_id):
-        contact: LegacyContact = await self.contacts.by_legacy_id(reply_id)
-        date = datetime.fromtimestamp(user_submission["time"])
-        contact.send_text(
-            parse_comment_text(user_submission["text"]), when=date, carbon=True
-        )
-        kid = await self.get_item(reply_id)
-        contact.send_text(parse_comment_text(kid["text"]))
-
-    async def get_item(self, item_id):
-        async with self.http_session.get(f"{API_URL}/item/{item_id}.json") as r:
-            return await r.json()
-
-    async def logout(self):
-        pass
-
-    async def send_text(self, text: str, chat: LegacyContact, **k):
-        goto = f"threads?id={self.hn_username}#{chat.legacy_id}"
-        url = f"{REPLY_URL}?id={chat.legacy_id}&goto={goto}"
-        async with self.http_session.get(url) as r:
-            if r.status != 200:
-                raise XMPPError(text="Couldn't get the post reply web page from HN")
-            form_page_content = await r.text()
-        match = re.search(HMAC_RE, form_page_content)
+    NODE = CHAT_COMMAND = "sync-contacts"
+    ACCESS = CommandAccess.USER_LOGGED
+    CATEGORY = CONTACTS
+
+    async def run(self, session: Optional[AnyBaseSession], _ifrom, *_) -> Confirmation:
+        return Confirmation(
+            prompt="Are you sure you want to sync your roster?",
+            success=None,
+            handler=self.sync,
+        )
+
+    async def sync(self, session: Optional[AnyBaseSession], _ifrom: JID) -> str:
+        if session is None:
+            raise RuntimeError
+        roster_iq = await self.xmpp["xep_0356"].get_roster(session.user.bare_jid)
+
+        contacts = session.contacts.known_contacts()
+
+        added = 0
+        removed = 0
+        updated = 0
+        for item in roster_iq["roster"]:
+            groups = set(item["groups"])
+            if self.xmpp.ROSTER_GROUP in groups:
+                contact = contacts.pop(item["jid"], None)
+                if contact is None:
+                    if len(groups) == 1:
+                        await self.xmpp["xep_0356"].set_roster(
+                            session.user.jid, {item["jid"]: {"subscription": "remove"}}
+                        )
+                        removed += 1
+                    else:
+                        groups.remove(self.xmpp.ROSTER_GROUP)
+                        await self.xmpp["xep_0356"].set_roster(
+                            session.user.jid,
+                            {
+                                item["jid"]: {
+                                    "subscription": item["subscription"],
+                                    "name": item["name"],
+                                    "groups": groups,
+                                }
+                            },
+                        )
+                        updated += 1
+                else:
+                    if contact.name != item["name"]:
+                        await contact.add_to_roster(force=True)
+                        updated += 1
+
+        # we popped before so this only acts on slidge contacts not in the xmpp roster
+        for contact in contacts.values():
+            added += 1
+            await contact.add_to_roster()
+
+        return f"{added} added, {removed} removed, {updated} updated"
+
+
+class ListContacts(Command):
+    NAME = HELP = "👤 List your legacy contacts"
+    NODE = CHAT_COMMAND = "contacts"
+    ACCESS = CommandAccess.USER_LOGGED
+    CATEGORY = CONTACTS
+
+    async def run(
+        self, session: Optional[AnyBaseSession], _ifrom: JID, *_
+    ) -> TableResult:
+        assert session is not None
+        await session.contacts.fill()
+        contacts = sorted(
+            session.contacts, key=lambda c: c.name.casefold() if c.name else ""
+        )
+        return TableResult(
+            description="Your buddies",
+            fields=[FormField("name"), FormField("jid", type="jid-single")],
+            items=[{"name": c.name, "jid": c.jid.bare} for c in contacts],
+        )
+
 
-        if match is None:
+class ListGroups(Command):
+    NAME = HELP = "👥 List your legacy groups"
+    NODE = CHAT_COMMAND = "groups"
+    ACCESS = CommandAccess.USER_LOGGED
+    CATEGORY = GROUPS
+
+    async def run(self, session, _ifrom, *_):
+        assert session is not None
+        await session.bookmarks.fill()
+        groups = sorted(session.bookmarks, key=lambda g: g.DISCO_NAME.casefold())
+        return TableResult(
+            description="Your groups",
+            fields=[FormField("name"), FormField("jid", type="jid-single")],
+            items=[{"name": g.name, "jid": g.jid.bare} for g in groups],
+            jids_are_mucs=True,
+        )
+
+
+class Login(Command):
+    NAME = "🔐 Re-login to the legacy network"
+    HELP = "Login to the legacy service"
+    NODE = CHAT_COMMAND = "re-login"
+
+    ACCESS = CommandAccess.USER_NON_LOGGED
+
+    async def run(self, session: Optional[AnyBaseSession], _ifrom, *_):
+        assert session is not None
+        try:
+            msg = await session.login()
+        except Exception as e:
+            session.send_gateway_status(f"Re-login failed: {e}", show="dnd")
             raise XMPPError(
-                text="Couldn't find the HMAC hidden input on the comment reply thread"
+                "internal-server-error", etype="wait", text=f"Could not login: {e}"
             )
+        session.logged = True
+        session.send_gateway_status(msg or "Re-connected", show="chat")
+        session.send_gateway_message(msg or "Re-connected")
+        return msg
+
+
+class CreateGroup(Command):
+    NAME = "🆕 New legacy group"
+    HELP = "Create a group on the legacy service"
+    NODE = CHAT_COMMAND = "create-group"
+    CATEGORY = GROUPS
+
+    ACCESS = CommandAccess.USER_LOGGED
+
+    async def run(self, session: Optional[AnyBaseSession], _ifrom, *_):
+        assert session is not None
+        contacts = session.contacts.known_contacts(only_friends=True)
+        return Form(
+            title="Create a new group",
+            instructions="Pick contacts that should be part of this new group",
+            fields=[
+                FormField(var="group_name", label="Name of the group", required=True),
+                FormField(
+                    var="contacts",
+                    label="Contacts to add to the new group",
+                    type="list-multi",
+                    options=[
+                        {"value": str(contact.jid), "label": contact.name}
+                        for contact in sorted(contacts.values(), key=lambda c: c.name)
+                    ],
+                    required=False,
+                ),
+            ],
+            handler=self.finish,
+        )
 
-        await asyncio.sleep(SLEEP_BEFORE_POST)
+    @staticmethod
+    async def finish(form_values: FormValues, session: Optional[AnyBaseSession], *_):
+        assert session is not None
+        legacy_id: LegacyGroupIdType = await session.on_create_group(  # type:ignore
+            cast(str, form_values["group_name"]),
+            [
+                await session.contacts.by_jid(JID(j))
+                for j in form_values.get("contacts", [])  # type:ignore
+            ],
+        )
+        muc = await session.bookmarks.by_legacy_id(legacy_id)
+        return TableResult(
+            description=f"Your new group: xmpp:{muc.jid}?join",
+            fields=[FormField("name"), FormField("jid", type="jid-single")],
+            items=[{"name": muc.name, "jid": muc.jid}],
+            jids_are_mucs=True,
+        )
 
-        form_dict = {
-            "hmac": match.group(1),
-            "parent": chat.legacy_id,
-            "text": text,
-            "goto": goto,
-        }
-
-        form = aiohttp.FormData(form_dict)
-        async with self.http_session.post(REPLY_POST_URL, data=form) as r:
-            first_attempt_html_content = await r.text()
-
-        log.debug("Reply response #1: %s", r)
-        if r.status != 200:
-            raise XMPPError(text=f"Problem replying: {r}")
-
-        if REPOST_TEXT in first_attempt_html_content:
-            match = re.search(HMAC_RE, first_attempt_html_content)
-            if match is None:
-                raise XMPPError(
-                    text="We should repost but haven't found any hmac field on the repost page"
-                )
-
-            await asyncio.sleep(SLEEP_BEFORE_POST2)
-            form = aiohttp.FormData(form_dict | {"hmac": match.group(1)})
-            async with self.http_session.post(REPLY_POST_URL, data=form) as r:
-                log.debug("Reply response #2: %s", r)
-                if r.status != 200:
-                    raise XMPPError(text=f"Problem replying: {r}")
-
-    # none of the following make sense in a HN context,
-    # this is just to avoid raising NotImplementedErrors
-    async def send_file(self, *a, **k):
-        pass
-
-    async def active(self, c: LegacyContact):
-        pass
-
-    async def inactive(self, c: LegacyContact):
-        pass
-
-    async def composing(self, c: LegacyContact):
-        pass
-
-    async def paused(self, c: LegacyContact):
-        pass
-
-    async def displayed(self, legacy_msg_id: Any, c: LegacyContact):
-        pass
-
-    async def correct(self, text: str, legacy_msg_id: Any, c: LegacyContact):
-        pass
-
-    async def search(self, form_values: dict[str, str]):
-        pass
-
-
-def parse_comment_text(text: str):
-    # TODO: use regex or something more efficient here
-    return text.replace("<p>", "\n").replace("&#x27;", "'").replace("&#x2F;", "/")
-
-
-LOGIN_URL = "https://news.ycombinator.com/login"
-REPLY_URL = "https://news.ycombinator.com/reply"
-REPLY_POST_URL = "https://news.ycombinator.com/comment"
-API_URL = "https://hacker-news.firebaseio.com/v0"
-POLL_INTERVAL = 30  # seconds
-SLEEP_BEFORE_POST = 30  # seconds
-SLEEP_BEFORE_POST2 = 5  # seconds
-REPOST_TEXT = "<tr><td>Please confirm that this is your comment by submitting it one"
-HMAC_RE = re.compile(r'name="hmac" value="([a-zA-Z\d]*)"')
 
-log = logging.getLogger(__name__)
+class Unregister(Command):
+    NAME = "❌ Unregister from the gateway"
+    HELP = "Unregister from the gateway"
+    NODE = CHAT_COMMAND = "unregister"
+    ACCESS = CommandAccess.USER
+
+    async def run(
+        self, session: Optional[AnyBaseSession], _ifrom: JID, *_: Any
+    ) -> Confirmation:
+        return Confirmation(
+            prompt=f"Are you sure you want to unregister from '{self.xmpp.boundjid}'?",
+            success=f"You are not registered to '{self.xmpp.boundjid}' anymore.",
+            handler=self.unregister,
+        )
+
+    async def unregister(self, session: Optional[AnyBaseSession], _ifrom: JID) -> str:
+        assert session is not None
+        await self.xmpp.unregister_user(session.user)
+        return "OK"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slidge-0.1.0rc1/slidge/plugins/signal/session.py` & `slidge-0.1.1/slidge/core/mixins/attachment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,515 +1,506 @@
-import asyncio
 import functools
 import logging
 import os
+import re
+import shutil
+import stat
 import tempfile
+import warnings
 from datetime import datetime
+from mimetypes import guess_type
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Optional, Union, cast
+from typing import IO, Collection, Optional, Sequence, Union
+from urllib.parse import quote as urlquote
+from uuid import uuid4
+from xml.etree import ElementTree as ET
+
+import blurhash
+from PIL import Image
+from slixmpp import JID, Message
+from slixmpp.exceptions import IqError
+from slixmpp.plugins.xep_0363 import FileUploadError
+from slixmpp.plugins.xep_0385.stanza import Sims
+from slixmpp.plugins.xep_0447.stanza import StatelessFileSharing
+
+from ...util.sql import db
+from ...util.types import (
+    LegacyAttachment,
+    LegacyMessageType,
+    LegacyThreadType,
+    MessageReference,
+)
+from ...util.util import fix_suffix
+from .. import config
+from ..cache import avatar_cache
+from .message_maker import MessageMaker
+
+
+class AttachmentMixin(MessageMaker):
+    def send_text(self, *_, **k) -> Optional[Message]:
+        raise NotImplementedError
 
-import aiohttp
-import aiosignald.exc as sigexc
-import aiosignald.generated as sigapi
-from slixmpp.exceptions import XMPPError
+    async def __upload(
+        self,
+        file_path: Path,
+        file_name: Optional[str] = None,
+        content_type: Optional[str] = None,
+    ):
+        if file_name and file_path.name != file_name:
+            d = Path(tempfile.mkdtemp())
+            temp = d / file_name
+            temp.symlink_to(file_path)
+            file_path = temp
+        else:
+            d = None
+        if config.UPLOAD_SERVICE:
+            domain = None
+        else:
+            domain = re.sub(r"^.*?\.", "", self.xmpp.boundjid.bare)
+        try:
+            new_url = await self.xmpp.plugin["xep_0363"].upload_file(
+                filename=file_path,
+                content_type=content_type,
+                ifrom=config.UPLOAD_REQUESTER or self.xmpp.boundjid,
+                domain=JID(domain),
+            )
+        except (FileUploadError, IqError) as e:
+            warnings.warn(f"Something is wrong with the upload service: {e!r}")
+            return None
+        finally:
+            if d is not None:
+                file_path.unlink()
+                d.rmdir()
 
-from slidge import *
-from slidge.core.muc.room import MucType
-from slidge.util.util import is_valid_phone_number
+        return new_url
 
-if TYPE_CHECKING:
-    from .contact import Contact, Roster
-    from .gateway import Gateway
-    from .group import Bookmarks, MUC, Participant
+    @staticmethod
+    async def __no_upload(
+        file_path: Path,
+        file_name: Optional[str] = None,
+        legacy_file_id: Optional[Union[str, int]] = None,
+    ):
+        file_id = str(uuid4()) if legacy_file_id is None else str(legacy_file_id)
+        assert config.NO_UPLOAD_PATH is not None
+        assert config.NO_UPLOAD_URL_PREFIX is not None
+        destination_dir = Path(config.NO_UPLOAD_PATH) / file_id
+
+        if destination_dir.exists():
+            log.debug("Dest dir exists: %s", destination_dir)
+            files = list(f for f in destination_dir.glob("**/*") if f.is_file())
+            if len(files) == 1:
+                log.debug(
+                    "Found the legacy attachment '%s' at '%s'",
+                    legacy_file_id,
+                    files[0],
+                )
+                name = files[0].name
+                uu = files[0].parent.name  # anti-obvious url trick, see below
+                return files[0], "/".join([file_id, uu, name])
+            else:
+                log.warning(
+                    (
+                        "There are several or zero files in %s, "
+                        "slidge doesn't know which one to pick among %s. "
+                        "Removing the dir."
+                    ),
+                    destination_dir,
+                    files,
+                )
+                shutil.rmtree(destination_dir)
 
-from . import config
+        log.debug("Did not find a file in: %s", destination_dir)
+        # let's use a UUID to avoid URLs being too obvious
+        uu = str(uuid4())
+        destination_dir = destination_dir / uu
+        destination_dir.mkdir(parents=True)
+
+        name = file_name or file_path.name
+        destination = destination_dir / name
+        method = config.NO_UPLOAD_METHOD
+        if method == "copy":
+            shutil.copy2(file_path, destination)
+        elif method == "hardlink":
+            os.link(file_path, destination)
+        elif method == "symlink":
+            os.symlink(file_path, destination, target_is_directory=True)
+        elif method == "move":
+            shutil.move(file_path, destination)
+        else:
+            raise RuntimeError("No upload method not recognized", method)
 
+        if config.NO_UPLOAD_FILE_READ_OTHERS:
+            log.debug("Changing perms of %s", destination)
+            destination.chmod(destination.stat().st_mode | stat.S_IROTH)
+        uploaded_url = "/".join([file_id, uu, name])
 
-def handle_unregistered_recipient(func):
-    @functools.wraps(func)
-    async def wrapped(*a, **kw):
-        try:
-            return await func(*a, **kw)
-        except (
-            sigexc.UnregisteredUserError,
-            sigexc.IllegalArgumentException,
-            sigexc.InternalError,
-            sigexc.InvalidGroupError,
-        ) as e:
-            raise XMPPError(
-                "item-not-found",
-                text=e.message,
-            )
+        return destination, uploaded_url
 
-    return wrapped
+    async def __get_url(
+        self,
+        file_path: Optional[Path] = None,
+        data_stream: Optional[IO[bytes]] = None,
+        data: Optional[bytes] = None,
+        file_url: Optional[str] = None,
+        file_name: Optional[str] = None,
+        content_type: Optional[str] = None,
+        legacy_file_id: Optional[Union[str, int]] = None,
+    ) -> tuple[bool, Optional[Path], str]:
+        if legacy_file_id:
+            cache = db.attachment_get_url(legacy_file_id)
+            if cache is not None:
+                async with self.session.http.head(cache) as r:
+                    if r.status < 400:
+                        return False, None, cache
+                    else:
+                        db.attachment_remove(legacy_file_id)
+
+        if file_url and config.USE_ATTACHMENT_ORIGINAL_URLS:
+            return False, None, file_url
+
+        if file_name and len(file_name) > config.ATTACHMENT_MAXIMUM_FILE_NAME_LENGTH:
+            log.debug("Trimming long filename: %s", file_name)
+            base, ext = os.path.splitext(file_name)
+            file_name = (
+                base[: config.ATTACHMENT_MAXIMUM_FILE_NAME_LENGTH - len(ext)] + ext
+            )
+
+        if file_path is None:
+            file_name = str(uuid4()) if file_name is None else file_name
+            temp_dir = Path(tempfile.mkdtemp())
+            file_path = temp_dir / file_name
+            if file_url:
+                async with self.session.http.get(file_url) as r:
+                    with file_path.open("wb") as f:
+                        f.write(await r.read())
 
+            else:
+                if data_stream is not None:
+                    data = data_stream.read()
+                if data is None:
+                    raise RuntimeError
 
-class Session(
-    BaseSession["Gateway", int, "Roster", "Contact", "Bookmarks", "MUC", "Participant"]
-):
-    """
-    Represents a signal account
-    """
+                with file_path.open("wb") as f:
+                    f.write(data)
 
-    def __init__(self, user: GatewayUser):
-        """
+            is_temp = not bool(config.NO_UPLOAD_PATH)
+        else:
+            is_temp = False
 
-        :param user:
-        """
-        super().__init__(user)
-        self.phone = self.user.registration_form["phone"]
-        if self.phone is None:
-            raise RuntimeError
-        self.signal = self.xmpp.signal
-        self.xmpp.sessions_by_phone[self.phone] = self
-        self.user_uuid: asyncio.Future[str] = self.xmpp.loop.create_future()
-        self.user_nick: asyncio.Future[str] = self.xmpp.loop.create_future()
-        self.connected = self.xmpp.loop.create_future()
-        self.sent_in_muc = dict[int, "MUC"]()
+        if config.FIX_FILENAME_SUFFIX_MIME_TYPE:
+            file_name = str(fix_suffix(file_path, content_type, file_name))
 
-    @staticmethod
-    def xmpp_msg_id_to_legacy_msg_id(i: str) -> int:
-        try:
-            return int(i)
-        except ValueError:
-            raise NotImplementedError
-
-    @handle_unregistered_recipient
-    async def paused(self, c: "Contact"):
-        await (await self.signal).typing(
-            account=self.phone, typing=False, address=c.signal_address
-        )
+        if config.NO_UPLOAD_PATH:
+            local_path, new_url = await self.__no_upload(
+                file_path, file_name, legacy_file_id
+            )
+            new_url = (config.NO_UPLOAD_URL_PREFIX or "") + "/" + urlquote(new_url)
+        else:
+            local_path = file_path
+            new_url = await self.__upload(file_path, file_name, content_type)
+        if legacy_file_id:
+            db.attachment_store_url(legacy_file_id, new_url)
 
-    async def correct(self, text: str, legacy_msg_id: Any, c: "Contact"):
-        return await self.send_text("Correction: " + text, c)
+        return is_temp, local_path, new_url
 
-    async def search(self, form_values: dict[str, str]):
-        phone = form_values.get("phone")
-        if phone is None:
-            raise XMPPError("bad-request", "Please enter a phone number")
-
-        if not is_valid_phone_number(phone):
-            raise XMPPError(
-                "bad-request", "This does not look like a valid phone number"
-            )
+    async def __set_sims(
+        self,
+        msg: Message,
+        uploaded_url: str,
+        path: Optional[Path],
+        content_type: Optional[str] = None,
+        caption: Optional[str] = None,
+        file_name: Optional[str] = None,
+    ):
+        cache = db.attachment_get_sims(uploaded_url)
+        if cache:
+            msg.append(Sims(xml=ET.fromstring(cache)))
+            return
 
-        try:
-            address = await (await self.signal).resolve_address(
-                account=self.phone,
-                partial=sigapi.JsonAddressv1(number=phone),
-            )
-        except sigexc.UnregisteredUserError:
+        if not path:
             return
 
-        contact = await self.contacts.by_json_address(address)
-        # the name will be updated once c.update_and_add(), triggered by by_json_address()
-        # completes, but it's nicer to have a phone number instead of a UUID
-        # in the meantime.
-        contact.name = phone
-
-        return SearchResult(
-            fields=[FormField("phone"), FormField("jid", type="jid-single")],
-            items=[{"phone": phone, "jid": contact.jid.bare}],
+        sims = self.xmpp["xep_0385"].get_sims(
+            path, [uploaded_url], content_type, caption
         )
-
-    async def login(self):
-        await (await self.signal).subscribe(account=self.phone)
-        await self.connected
-        sig = await self.signal
-        # TODO: store the account UUID on registration so we don't have to do that
-        try:
-            # sometimes doesn't work with own phone number
-            profile = await sig.get_profile(
-                account=self.phone, address=sigapi.JsonAddressv1(number=self.phone)
-            )
-        except sigexc.ProfileUnavailableError:
-            accounts = await sig.list_accounts()
-            for a in accounts.accounts:
-                if a.address.number == self.phone:
-                    profile = await sig.get_profile(
-                        account=self.phone, address=a.address
-                    )
-                    break
+        if file_name:
+            sims["sims"]["file"]["name"] = file_name
+        if content_type is not None and content_type.startswith("image"):
+            try:
+                h, x, y = await self.xmpp.loop.run_in_executor(
+                    avatar_cache._thread_pool, get_blurhash, path
+                )
+            except Exception as e:
+                log.debug("Could not generate a blurhash", exc_info=e)
             else:
-                raise RuntimeError("Could not find the signal address of your")
-        nick: str = profile.name or profile.profile_name or "SlidgeUser"
-        if nick is not None:
-            nick = nick.replace("\u0000", " ")
-        self.user_nick.set_result(nick)
-        self.user_uuid.set_result(profile.address.uuid)
-        self.bookmarks.set_username(nick)
-        await self.add_contacts_to_roster()
-        await self.add_groups()
-        return f"Connected as {self.phone}"
+                thumbnail = sims["sims"]["file"]["thumbnail"]
+                thumbnail["width"] = x
+                thumbnail["height"] = y
+                thumbnail["media-type"] = "image/blurhash"
+                thumbnail["uri"] = "data:image/blurhash," + urlquote(h)
 
-    async def on_websocket_connection_state(
-        self, state: sigapi.WebSocketConnectionStatev1
-    ):
-        if (
-            state.state == "CONNECTED"
-            and state.socket == "IDENTIFIED"
-            and not self.connected.done()
-        ):
-            self.connected.set_result(True)
+        db.attachment_store_sims(uploaded_url, str(sims))
 
-    async def logout(self):
-        await (await self.signal).unsubscribe(account=self.phone)
+        msg.append(sims)
 
-    async def add_contacts_to_roster(self):
-        """
-        Populate a user's roster
-        """
-        profiles = await (await self.signal).list_contacts(account=self.phone)
-        for profile in profiles.profiles:
-            # contacts are added automatically if their profile could be resolved
-            await self.contacts.by_json_address(profile.address)
-
-    async def add_groups(self):
-        groups = await (await self.signal).list_groups(account=self.phone)
-        self.log.debug("GROUPS: %r", groups)
-        for group in groups.groups:
-            muc = await self.bookmarks.by_legacy_id(group.id)
-            muc.type = MucType.GROUP
-            muc.DISCO_NAME = group.title
-            muc.subject = group.description
-            muc.description = group.description
-            muc.n_participants = len(group.members)
+    def __set_sfs(
+        self,
+        msg: Message,
+        uploaded_url: str,
+        path: Optional[Path],
+        content_type: Optional[str] = None,
+        caption: Optional[str] = None,
+        file_name: Optional[str] = None,
+    ):
+        cache = db.attachment_get_sfs(uploaded_url)
+        if cache:
+            msg.append(StatelessFileSharing(xml=ET.fromstring(cache)))
+            return
 
-    async def on_signal_message(self, msg: sigapi.IncomingMessagev1):
-        """
-        User has received 'something' from signal
+        if not path:
+            return
 
-        :param msg:
-        """
-        if (sync_msg := msg.sync_message) is not None:
-            if sync_msg.contacts is not None and msg.sync_message.contactsComplete:
-                log.debug("Received a sync contact updates")
-                await self.add_contacts_to_roster()
-
-            if (sent := sync_msg.sent) is None:
-                # Probably a 'message read' marker
-                log.debug("No sent message in this sync message")
-                return
-            sent_msg = sent.message
-            if sent_msg.group or sent_msg.groupV2:
-                return
+        sfs = self.xmpp["xep_0447"].get_sfs(path, [uploaded_url], content_type, caption)
+        if file_name:
+            sfs["file"]["name"] = file_name
+        db.attachment_store_sfs(uploaded_url, str(sfs))
 
-            contact = await self.contacts.by_json_address(sent.destination)
+        msg.append(sfs)
 
-            await contact.send_attachments(
-                sent_msg.attachments, sent_msg.timestamp, carbon=True
+    def __send_url(
+        self,
+        msg: Message,
+        legacy_msg_id: LegacyMessageType,
+        uploaded_url: str,
+        caption: Optional[str] = None,
+        carbon=False,
+        when: Optional[datetime] = None,
+        **kwargs,
+    ) -> list[Message]:
+        msg["oob"]["url"] = uploaded_url
+        msg["body"] = uploaded_url
+        if caption:
+            m1 = self._send(msg, carbon=carbon, **kwargs)
+            m2 = self.send_text(
+                caption, legacy_msg_id=legacy_msg_id, when=when, carbon=carbon, **kwargs
             )
+            return [m1, m2] if m2 else [m1]
+        else:
+            self._set_msg_id(msg, legacy_msg_id)
+            return [self._send(msg, carbon=carbon, **kwargs)]
 
-            if (body := sent_msg.body) is not None:
-                contact.send_text(
-                    body=body,
-                    when=datetime.fromtimestamp(sent_msg.timestamp / 1000),
-                    legacy_id=sent_msg.timestamp,
-                    carbon=True,
-                )
-            if (reaction := sent_msg.reaction) is not None:
-                contact.react(
-                    reaction.targetSentTimestamp,
-                    () if reaction.remove else reaction.emoji,
-                    carbon=True,
-                )
-            if (delete := sent_msg.remoteDelete) is not None:
-                contact.retract(delete.target_sent_timestamp, carbon=True)
+    async def send_file(
+        self,
+        file_path: Optional[Union[Path, str]] = None,
+        legacy_msg_id: Optional[LegacyMessageType] = None,
+        *,
+        data_stream: Optional[IO[bytes]] = None,
+        data: Optional[bytes] = None,
+        file_url: Optional[str] = None,
+        file_name: Optional[str] = None,
+        content_type: Optional[str] = None,
+        reply_to: Optional[MessageReference] = None,
+        when: Optional[datetime] = None,
+        caption: Optional[str] = None,
+        legacy_file_id: Optional[Union[str, int]] = None,
+        thread: Optional[LegacyThreadType] = None,
+        **kwargs,
+    ) -> tuple[Optional[str], list[Message]]:
+        """
+        Send a single file from this :term:`XMPP Entity`.
 
-        contact = await self.contacts.by_json_address(msg.source)
+        :param file_path: Path to the attachment
+        :param data_stream: Alternatively, a stream of bytes (such as a File object)
+        :param data: Alternatively, a bytes object
+        :param file_url: Alternatively, a URL
+        :param file_name: How the file should be named.
+        :param content_type: MIME type, inferred from filename if not given
+        :param legacy_msg_id: If you want to be able to transport read markers from the gateway
+            user to the legacy network, specify this
+        :param reply_to: Quote another message (:xep:`0461`)
+        :param when: when the file was sent, for a "delay" tag (:xep:`0203`)
+        :param caption: an optional text that is linked to the file
+        :param legacy_file_id: A unique identifier for the file on the legacy network.
+             Plugins should try their best to provide it, to avoid duplicates.
+        :param thread:
+        """
+        carbon = kwargs.pop("carbon", False)
+        mto = kwargs.pop("mto", None)
+        store_multi = kwargs.pop("store_multi", True)
+        msg = self._make_message(
+            when=when,
+            reply_to=reply_to,
+            carbon=carbon,
+            mto=mto,
+            thread=thread,
+        )
 
-        if (data := msg.data_message) is not None:
-            if data.group:
-                return
-
-            if data.groupV2:
-                muc = await self.bookmarks.by_legacy_id(data.groupV2.id)
-                entity = await muc.get_participant_by_contact(contact)
-            else:
-                entity = contact
+        if content_type is None and (name := (file_name or file_path or file_url)):
+            content_type, _ = guess_type(name)
 
-            reply_self = False
-            if (quote := data.quote) is None:
-                reply_to_msg_id = None
-                reply_to_fallback_text = None
-                reply_to_author = None
-            else:
-                reply_to_msg_id = quote.id
-                reply_to_fallback_text = quote.text
-                reply_self = quote.author.uuid == msg.source.uuid
-
-                if data.groupV2:
-                    reply_to_author = await muc.get_participant(muc.user_nick)
-                else:
-                    reply_to_author = None
-
-            kwargs = dict(
-                reply_to_msg_id=reply_to_msg_id,
-                reply_to_author=reply_to_author,
-                reply_to_fallback_text=reply_to_fallback_text,
-                reply_self=reply_self,
-                when=datetime.fromtimestamp(msg.data_message.timestamp / 1000),
-            )
+        is_temp, local_path, new_url = await self.__get_url(
+            Path(file_path) if file_path else None,
+            data_stream,
+            data,
+            file_url,
+            file_name,
+            content_type,
+            legacy_file_id,
+        )
 
-            msg_id = data.timestamp
-            text = data.body
-            await entity.send_attachments(
-                data.attachments, legacy_msg_id=None if text else msg_id, **kwargs
+        if new_url is None:
+            msg["body"] = (
+                "I tried to send a file, but something went wrong. "
+                "Tell your slidge admin to check the logs."
             )
-            if text:
-                entity.send_text(body=text, legacy_msg_id=msg_id, **kwargs)
-            if (reaction := data.reaction) is not None:
-                self.log.debug("Reaction: %s", reaction)
-                if reaction.remove:
-                    entity.react(reaction.targetSentTimestamp)
-                else:
-                    entity.react(reaction.targetSentTimestamp, reaction.emoji)
-            if (delete := data.remoteDelete) is not None:
-                entity.retract(delete.target_sent_timestamp)
-
-        if (typing_message := msg.typing_message) is not None:
-            if g := typing_message.group_id:
-                muc = await self.bookmarks.by_legacy_id(g)
-                entity = await muc.get_participant_by_contact(contact)
-            else:
-                entity = contact
+            self._set_msg_id(msg, legacy_msg_id)
+            return None, [self._send(msg, **kwargs)]
 
-            action = typing_message.action
-            if action == "STARTED":
-                entity.active()
-                entity.composing()
-            elif action == "STOPPED":
-                entity.paused()
-
-        if (receipt_message := msg.receipt_message) is not None:
-            type_ = receipt_message.type
-            if type_ == "DELIVERY":
-                for t in msg.receipt_message.timestamps:
-                    entity = await self.__get_entity_by_sent_msg_id(contact, t)
-                    entity.received(t)
-            elif type_ == "READ":
-                # no need to mark all messages read, just the last one, see
-                # "8.1. Optimizations" in XEP-0333
-                t = max(msg.receipt_message.timestamps)
-                entity = await self.__get_entity_by_sent_msg_id(contact, t)
-                entity.displayed(t)
-
-    async def __get_entity_by_sent_msg_id(self, contact: "Contact", t: int):
-        self.log.debug("Looking for %s in %s", t, self.sent_in_muc)
-        group = self.sent_in_muc.get(t)
-        if group:
-            return await group.get_participant_by_contact(contact)
-        return contact
+        await self.__set_sims(
+            msg, new_url, local_path, content_type, caption, file_name
+        )
+        self.__set_sfs(msg, new_url, local_path, content_type, caption, file_name)
+        if is_temp and isinstance(local_path, Path):
+            local_path.unlink()
+            local_path.parent.rmdir()
+
+        msgs = self.__send_url(
+            msg, legacy_msg_id, new_url, caption, carbon, when, **kwargs
+        )
+        if store_multi:
+            self.__store_multi(legacy_msg_id, msgs)
+        return new_url, msgs
 
-    @handle_unregistered_recipient
-    async def send_text(
+    def __send_body(
         self,
-        text: str,
-        chat: Union["Contact", "MUC"],
-        *,
-        reply_to_msg_id=None,
-        reply_to_fallback_text=None,
-        reply_to: Optional[Union["Contact", "Participant"]] = None,
-    ) -> int:
-        address, group = self._get_args_from_entity(chat)
-        if reply_to_msg_id is None:
-            quote = None
-        elif reply_to is None:
-            quote = None
-            self.log.warning(
-                "An XMPP client did not include reply to=, so we cannot make a quote here."
+        body: Optional[str] = None,
+        legacy_msg_id: Optional[LegacyMessageType] = None,
+        reply_to: Optional[MessageReference] = None,
+        when: Optional[datetime] = None,
+        thread: Optional[LegacyThreadType] = None,
+        **kwargs,
+    ) -> Optional[Message]:
+        if body:
+            return self.send_text(
+                body,
+                legacy_msg_id,
+                reply_to=reply_to,
+                when=when,
+                thread=thread,
+                **kwargs,
             )
         else:
-            quote = sigapi.JsonQuotev1(
-                id=reply_to_msg_id,
-                author=sigapi.JsonAddressv1(uuid=await self.user_uuid)
-                if reply_to is None
-                else reply_to.signal_address,
-                text=reply_to_fallback_text or "",
-            )
-        response = await (await self.signal).send(
-            account=self.phone,
-            recipientAddress=address,
-            recipientGroupId=group,
-            messageBody=text,
-            quote=quote,
-        )
-        result = response.results[0]
-        log.debug("Result: %s", result)
-        if result.networkFailure or result.proof_required_failure:
-            raise XMPPError(str(result))
-        elif result.identityFailure:
-            chat = cast("Contact", chat)
-            s = await self.signal
-            identities = (
-                await s.get_identities(
-                    account=self.phone,
-                    address=chat.signal_address,
-                )
-            ).identities
-            ans = await self.input(
-                f"The identity of {chat.legacy_id} has changed. "
-                f"Do you want to trust all their identities and resend the message?"
-            )
-            if ans.lower().startswith("y"):
-                for i in identities:
-                    await (await self.signal).trust(
-                        account=self.phone,
-                        address=chat.signal_address,
-                        safety_number=i.safety_number,
-                    )
-                await self.send_text(text, chat, reply_to_msg_id=reply_to_msg_id)
-            else:
-                raise XMPPError(str(result))
-        legacy_msg_id = response.timestamp
-        if group:
-            self.sent_in_muc[legacy_msg_id] = cast("MUC", chat)
-        return legacy_msg_id
+            return None
 
-    @handle_unregistered_recipient
-    async def send_file(
+    async def send_files(
         self,
-        url: str,
-        chat: "Contact",
+        attachments: Collection[LegacyAttachment],
+        legacy_msg_id: Optional[LegacyMessageType] = None,
+        body: Optional[str] = None,
         *,
-        reply_to_msg_id=None,
-        reply_to_fallback_text=None,
-        reply_to: Optional[Union["Contact", "Participant"]] = None,
+        reply_to: Optional[MessageReference] = None,
+        when: Optional[datetime] = None,
+        thread: Optional[LegacyThreadType] = None,
+        body_first=False,
+        correction=False,
+        correction_event_id: Optional[LegacyMessageType] = None,
+        **kwargs,
     ):
-        s = await self.signal
-        address, group = self._get_args_from_entity(chat)
-        async with aiohttp.ClientSession() as client:
-            async with client.get(url=url) as r:
-                with tempfile.TemporaryDirectory(
-                    dir=config.SIGNALD_SOCKET.parent,
-                ) as d:
-                    os.chmod(d, 0o777)
-                    with open(Path(d) / r.url.name, "wb") as f:
-                        f.write(await r.content.read())
-                        os.chmod(
-                            f.name, 0o666
-                        )  # temp file is 0600 https://stackoverflow.com/a/10541972/5902284
-                        signal_r = await s.send(
-                            account=self.phone,
-                            recipientAddress=address,
-                            recipientGroupId=group,
-                            attachments=[sigapi.JsonAttachmentv1(filename=f.name)],
-                        )
-                        return signal_r.timestamp
-
-    async def active(self, c: "Contact"):
-        pass
-
-    async def inactive(self, c: "Contact"):
-        pass
-
-    @staticmethod
-    def _get_args_from_entity(e):
-        if e.is_group:
-            address = None
-            group = e.legacy_id
-        else:
-            address = e.signal_address
-            group = None
-        return address, group
-
-    @handle_unregistered_recipient
-    async def composing(self, c: "Contact"):
-        self.log.debug("COMPOSING %s", c)
-        address, group = self._get_args_from_entity(c)
-        await (await self.signal).typing(
-            account=self.phone,
-            address=address,
-            group=group,
-            typing=True,
-        )
-
-    @handle_unregistered_recipient
-    async def displayed(self, legacy_msg_id: int, entity: Union["Contact", "MUC"]):
-        if entity.is_group:
-            entity = cast("MUC", entity)
-            address = entity.sent.get(legacy_msg_id)
-            if address is None:
-                self.log.debug(
-                    "Ignoring read mark %s in %s", legacy_msg_id, entity.sent
-                )
-                return
-        else:
-            entity = cast("Contact", entity)
-            address = entity.signal_address
-
-        await (await self.signal).mark_read(
-            account=self.phone,
-            to=address,
-            timestamps=[legacy_msg_id],
+        # TODO: once the epic XEP-0385 vs XEP-0447 battle is over, pick
+        #       one and stop sending several attachments this way
+        # we attach the legacy_message ID to the last message we send, because
+        # we don't want several messages with the same ID (especially for MUC MAM)
+        # TODO: refactor this so we limit the number of SQL calls, ie, if
+        #       the legacy file ID is known, only fetch the row once, and if it
+        #       is new, write it all in a single call
+        if not attachments and not body:
+            # ignoring empty message
+            return
+        send_body = functools.partial(
+            self.__send_body,
+            body=body,
+            reply_to=reply_to,
+            when=when,
+            thread=thread,
+            correction=correction,
+            legacy_msg_id=legacy_msg_id,
+            correction_event_id=correction_event_id,
+            **kwargs,
         )
+        all_msgs = []
+        if body_first:
+            all_msgs.append(send_body())
+        last_attachment_i = len(attachments) - 1
+        for i, attachment in enumerate(attachments):
+            last = i == last_attachment_i
+            if last and not body:
+                legacy = legacy_msg_id
+            else:
+                legacy = None
+            _url, msgs = await self.send_file(
+                file_path=attachment.path,
+                legacy_msg_id=legacy,
+                file_url=attachment.url,
+                data_stream=attachment.stream,
+                data=attachment.data,
+                reply_to=reply_to,
+                when=when,
+                thread=thread,
+                file_name=attachment.name,
+                content_type=attachment.content_type,
+                legacy_file_id=attachment.legacy_file_id,
+                caption=attachment.caption,
+                store_multi=False,
+                **kwargs,
+            )
+            all_msgs.extend(msgs)
+        if not body_first:
+            all_msgs.append(send_body())
+        self.__store_multi(legacy_msg_id, all_msgs)
 
-    @handle_unregistered_recipient
-    async def react(
-        self, legacy_msg_id: int, emojis: list[str], c: Union["Contact", "MUC"]
+    def __store_multi(
+        self,
+        legacy_msg_id: Optional[LegacyMessageType],
+        all_msgs: Sequence[Optional[Message]],
     ):
-        address, group = self._get_args_from_entity(c)
-        if group:
+        if legacy_msg_id is None:
             return
-        c = cast("Contact", c)
+        ids = []
+        for msg in all_msgs:
+            if not msg:
+                continue
+            if stanza_id := msg.get_plugin("stanza_id", check=True):
+                ids.append(stanza_id["id"])
+            else:
+                ids.append(msg.get_id())
+        db.attachment_store_legacy_to_multi_xmpp_msg_ids(legacy_msg_id, ids)
 
-        remove = len(emojis) == 0
-        if remove:
-            try:
-                emoji = c.user_reactions.pop(legacy_msg_id)
-            except KeyError:
-                self.send_gateway_message(
-                    f"Slidge failed to remove your reactions on message '{legacy_msg_id}'"
-                )
-                self.log.warning("Could not find the emoji to remove reaction")
-                raise XMPPError(
-                    "undefined-condition",
-                    "Could not remove your reactions to this message",
-                )
-        else:
-            emoji = emojis[-1]
 
-        response = await (await self.signal).react(
-            username=self.phone,
-            recipientAddress=c.signal_address,
-            recipientGroupId=group,
-            reaction=sigapi.JsonReactionv1(
-                emoji=emoji,
-                remove=remove,
-                targetAuthor=sigapi.JsonAddressv1(number=self.phone)
-                if legacy_msg_id in self.sent
-                else c.signal_address,
-                targetSentTimestamp=legacy_msg_id,
-            ),
-        )
-        result = response.results[0]
-        if (
-            result.networkFailure
-            or result.identityFailure
-            or result.proof_required_failure
-        ):
-            raise XMPPError(str(result))
-        c.user_reactions[legacy_msg_id] = emoji
-
-    @handle_unregistered_recipient
-    async def retract(self, legacy_msg_id: int, c: "Contact"):
-        address, group = self._get_args_from_entity(c)
-        try:
-            await (await self.signal).remote_delete(
-                account=self.phone,
-                address=address,
-                group=group,
-                timestamp=legacy_msg_id,
-            )
-        except sigexc.SignaldException as e:
-            raise XMPPError(text=f"Something went wrong during remote delete: {e}")
+def get_blurhash(path: Path, n=9) -> tuple[str, int, int]:
+    img = Image.open(path)
+    width, height = img.size
+    n = min(width, height, n)
+    if width == height:
+        x = y = n
+    elif width > height:
+        x = n
+        y = round(n * height / width)
+    else:
+        x = round(n * width / height)
+        y = n
+    # There are 2 blurhash-python packages:
+    # https://github.com/woltapp/blurhash-python
+    # https://github.com/halcy/blurhash-python
+    # With this hack we're compatible with both, which is useful for packaging
+    # without using pyproject.toml, as most distro do
+    try:
+        hash_ = blurhash.encode(img, x, y)
+    except TypeError:
+        # We are using halcy's blurhash which expects
+        # the 1st argument to be a 3-dimensional array
+        import numpy  # type:ignore
 
-    async def add_device(self, uri: str):
-        try:
-            await (await self.signal).add_device(account=self.phone, uri=uri)
-        except sigexc.SignaldException as e:
-            self.send_gateway_message(f"Problem: {e}")
-        else:
-            self.send_gateway_message("Linking OK")
+        hash_ = blurhash.encode(numpy.array(img.convert("RGB")), x, y)
+    return hash_, width, height
 
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/plugins/telegram/group.py` & `slidge-0.1.1/slidge/core/mixins/message_maker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,184 +1,154 @@
+import warnings
+from copy import copy
 from datetime import datetime, timezone
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Iterable, Optional, cast
+from uuid import uuid4
 
-import aiotdlib.api as tgapi
-from slixmpp import JID
-from slixmpp.exceptions import XMPPError
+from slixmpp import Message
+from slixmpp.types import MessageTypes
 
-from slidge import *
-
-from .util import AvailableEmojisMixin, TelegramToXMPPMixin
+from ...slixfix.link_preview.stanza import LinkPreview as LinkPreviewStanza
+from ...util.db import GatewayUser
+from ...util.types import (
+    ChatState,
+    LegacyMessageType,
+    LinkPreview,
+    MessageReference,
+    ProcessingHint,
+)
+from .. import config
+from .base import BaseSender
 
 if TYPE_CHECKING:
-    from .contact import Contact
-    from .session import Session
-
-
-class Bookmarks(LegacyBookmarks):
-    @staticmethod
-    async def legacy_id_to_jid_local_part(legacy_id: int):
-        return "group" + str(legacy_id)
+    from ...group.participant import LegacyParticipant
 
-    @staticmethod
-    async def jid_local_part_to_legacy_id(local_part: str):
-        return int(local_part.replace("group", ""))
 
+class MessageMaker(BaseSender):
+    mtype: MessageTypes = NotImplemented
+    _can_send_carbon: bool = NotImplemented
+    STRIP_SHORT_DELAY = False
+    USE_STANZA_ID = False
 
-class MUC(LegacyMUC["Session", int, "Participant", int], AvailableEmojisMixin):
-    MAX_SUPER_GROUP_PARTICIPANTS = 200
-    session: "Session"
-    name = "unnamed"
-
-    async def join(self, join_presence):
-        self.user_nick = await self.session.my_name
-        await self.update_subject_from_msg()
-        await super().join(join_presence)
-
-    async def update_subject_from_msg(self, msg: Optional[tgapi.Message] = None):
-        if msg is None:
-            try:
-                msg = await self.session.tg.api.get_chat_pinned_message(self.legacy_id)
-                self.log.debug("Pinned message: %s", type(msg.content))
-            except tgapi.NotFound:
-                self.log.debug("Pinned message not found?")
-                return
-        content = msg.content
-        if not isinstance(content, (tgapi.MessagePhoto, tgapi.MessageText)):
-            return
-
-        sender_id = msg.sender_id
-        self.subject_date = datetime.fromtimestamp(msg.date, tz=timezone.utc)
-        if isinstance(sender_id, tgapi.MessageSenderUser):
-            if sender_id.user_id == await self.session.tg.get_my_id():
-                self.subject_setter = self.user_nick
-            else:
-                contact = await self.session.contacts.by_legacy_id(sender_id.user_id)
-                self.subject_setter = contact.name
+    def _make_message(
+        self,
+        state: Optional[ChatState] = None,
+        hints: Iterable[ProcessingHint] = (),
+        legacy_msg_id: Optional[LegacyMessageType] = None,
+        when: Optional[datetime] = None,
+        reply_to: Optional[MessageReference] = None,
+        carbon=False,
+        link_previews: Optional[Iterable[LinkPreview]] = None,
+        **kwargs,
+    ):
+        body = kwargs.pop("mbody", None)
+        mfrom = kwargs.pop("mfrom", self.jid)
+        mto = kwargs.pop("mto", None)
+        thread = kwargs.pop("thread", None)
+        if carbon and self._can_send_carbon:
+            # the msg needs to have jabber:client as xmlns, so
+            # we don't want to associate with the XML stream
+            msg_cls = Message
         else:
-            self.subject_setter = self.name
+            msg_cls = self.xmpp.Message  # type:ignore
+        msg = msg_cls(
+            sfrom=mfrom,
+            stype=kwargs.pop("mtype", None) or self.mtype,
+            sto=mto,
+            **kwargs,
+        )
+        if body:
+            msg["body"] = body
+            state = "active"
+        if thread:
+            known_threads = self.session.threads.inverse  # type:ignore
+            msg["thread"] = known_threads.get(thread) or str(thread)
+        if state:
+            msg["chat_state"] = state
+        for hint in hints:
+            msg.enable(hint)
+        self._set_msg_id(msg, legacy_msg_id)
+        self._add_delay(msg, when)
+        if link_previews:
+            self._add_link_previews(msg, link_previews)
+        if reply_to:
+            self._add_reply_to(msg, reply_to)
+        return msg
 
-        if isinstance(content, tgapi.MessagePhoto):
-            self.subject = content.caption.text
-        if isinstance(content, tgapi.MessageText):
-            self.subject = content.text.text
-
-    async def get_participants(self):
-        self.log.debug("Getting participants")
-        chat = await self.session.tg.get_chat(chat_id=self.legacy_id)
-        if not isinstance(
-            chat.type_, (tgapi.ChatTypeBasicGroup, tgapi.ChatTypeSupergroup)
-        ):
-            raise XMPPError("item-not-found", text="This is not a valid group ID")
-
-        info = await self.session.tg.get_chat_info(chat, full=True)
-        if isinstance(info, tgapi.BasicGroupFullInfo):
-            members = info.members
-        elif isinstance(info, tgapi.SupergroupFullInfo):
-            if info.can_get_members:
-                members = (
-                    await self.session.tg.api.get_supergroup_members(
-                        supergroup_id=chat.type_.supergroup_id,
-                        filter_=None,
-                        offset=0,
-                        limit=self.MAX_SUPER_GROUP_PARTICIPANTS,
-                        skip_validation=True,
-                    )
-                ).members
-            else:
-                members = []
-        else:
-            raise RuntimeError
-        self.log.debug("%s participants", len(members))
-        for member in members:
-            sender = member.member_id
-            if not isinstance(sender, tgapi.MessageSenderUser):
-                self.log.debug("Ignoring non-user sender")  # Does this happen?
-                continue
-            if sender.user_id == await self.session.tg.get_my_id():
-                continue
-            yield await self.participant_by_tg_user(
-                await self.session.tg.get_user(sender.user_id)
-            )
-
-    async def send_text(self, text: str) -> int:
-        result = await self.session.tg.send_text(self.legacy_id, text)
-        self.log.debug("MUC SEND RESULT: %s", result)
-        msg_id = await self.session.wait_for_tdlib_success(result.id)
-        self.log.debug("MUC SEND MSG: %s", msg_id)
-        return msg_id
-
-    async def participant_by_tg_user(self, user: tgapi.User) -> "Participant":
-        return await Participant.by_tg_user(self, user)
-
-    async def participant_system(self) -> "Participant":
-        return await self.get_participant("")
-
-    async def participant_by_tg_user_id(self, user_id: int) -> "Participant":
-        return await Participant.by_tg_user(
-            self, await self.session.tg.api.get_user(user_id)
+    def _set_msg_id(
+        self, msg: Message, legacy_msg_id: Optional[LegacyMessageType] = None
+    ):
+        if legacy_msg_id is not None:
+            i = self._legacy_to_xmpp(legacy_msg_id)
+            msg.set_id(i)
+            if self.USE_STANZA_ID:
+                msg["stanza_id"]["id"] = i
+                msg["stanza_id"]["by"] = self.muc.jid  # type: ignore
+        elif self.USE_STANZA_ID:
+            msg["stanza_id"]["id"] = str(uuid4())
+            msg["stanza_id"]["by"] = self.muc.jid  # type: ignore
+
+    def _legacy_to_xmpp(self, legacy_id: LegacyMessageType):
+        return self.session.sent.get(legacy_id) or self.session.legacy_to_xmpp_msg_id(
+            legacy_id
         )
 
-    async def get_tg_chat(self):
-        return await self.session.tg.get_chat(self.legacy_id)
+    def _add_delay(self, msg: Message, when: Optional[datetime]):
+        if when:
+            if when.tzinfo is None:
+                when = when.astimezone(timezone.utc)
+            if self.STRIP_SHORT_DELAY:
+                delay = datetime.now().astimezone(timezone.utc) - when
+                if delay < config.IGNORE_DELAY_THRESHOLD:
+                    return
+            msg["delay"].set_stamp(when)
+            msg["delay"].set_from(self.xmpp.boundjid.bare)
+
+    def _add_reply_to(self, msg: Message, reply_to: MessageReference):
+        xmpp_id = self._legacy_to_xmpp(reply_to.legacy_id)
+        msg["reply"]["id"] = xmpp_id
+
+        muc = getattr(self, "muc", None)
+
+        if entity := reply_to.author:
+            if isinstance(entity, GatewayUser):
+                if muc:
+                    jid = copy(muc.jid)
+                    jid.resource = fallback_nick = muc.user_nick
+                    msg["reply"]["to"] = jid
+                else:
+                    msg["reply"]["to"] = entity.jid
+                    # TODO: here we should use preferably use the PEP nick of the user
+                    # (but it doesn't matter much)
+                    fallback_nick = entity.jid.local
+            else:
+                if muc:
+                    if hasattr(entity, "muc"):
+                        # TODO: accept a Contact here and use muc.get_participant_by_legacy_id()
+                        # a bit of work because right now this is a sync function
+                        entity = cast("LegacyParticipant", entity)
+                        fallback_nick = entity.nickname
+                    else:
+                        warnings.warn(
+                            "The author of a message reference in a MUC must be a"
+                            " Participant instance, not a Contact"
+                        )
+                        fallback_nick = entity.name
+                else:
+                    fallback_nick = entity.name
+                msg["reply"]["to"] = entity.jid
+        else:
+            fallback_nick = None
 
-    async def fill_history(
-        self,
-        full_jid: JID,
-        maxchars: Optional[int] = None,
-        maxstanzas: Optional[int] = None,
-        seconds: Optional[int] = None,
-        since: Optional[int] = None,
-    ):
-        for m in await self.fetch_history(50):
-            part = await self.participant_by_tg_user(
-                await self.session.tg.get_user(m.sender_id.user_id)
-            )
-            await part.send_tg_message(m, full_jid=full_jid)
-
-    async def fetch_history(self, n: int):
-        tg = self.session.tg
-        chat = await self.get_tg_chat()
-        m = chat.last_message
-        if m is None:
-            return []
-
-        messages = [chat.last_message]
-        i = 0
-        last_message_id = m.id
-        while True:
-            fetched = (
-                await tg.api.get_chat_history(
-                    chat_id=self.legacy_id,
-                    from_message_id=last_message_id,
-                    offset=0,
-                    limit=10,
-                    only_local=False,
-                )
-            ).messages
-            if len(fetched) == 0:
-                break
-            messages.extend(fetched)
-            i += len(fetched)
-            if i > n:
-                break
-
-            last_message_id = fetched[-1].id
-
-        return reversed(messages)
-
-
-class Participant(LegacyParticipant[MUC], TelegramToXMPPMixin):
-    contact: "Contact"
-    session: "Session"  # type:ignore
-
-    def __init__(self, *a, **k):
-        super().__init__(*a, **k)
-        self.chat_id = self.muc.legacy_id
-        self.session.log.debug("PARTICIPANT-N: %s", self.muc.n_participants)
+        if fallback := reply_to.body:
+            msg["reply"].add_quoted_fallback(fallback, fallback_nick)
 
     @staticmethod
-    async def by_tg_user(muc: MUC, user: tgapi.User):
-        nick = " ".join((user.first_name, user.last_name)).strip()
-        p = Participant(muc, nick)
-        p.contact = await muc.session.contacts.by_legacy_id(user.id)
-        return p
+    def _add_link_previews(msg: Message, link_previews: Iterable[LinkPreview]):
+        for preview in link_previews:
+            element = LinkPreviewStanza()
+            for i, name in enumerate(preview._fields):
+                val = preview[i]
+                if not val:
+                    continue
+                element[name] = val
+            msg.append(element)
```

### Comparing `slidge-0.1.0rc1/slidge/util/db.py` & `slidge-0.1.1/slidge/util/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from io import BytesIO
 from os import PathLike
 from typing import Iterable, Optional, Union
 
 from pickle_secure import Pickler, Unpickler
 from slixmpp import JID, Iq, Message, Presence
 
+from .sql import db
+
 
 # noinspection PyUnresolvedReferences
 class EncryptedShelf(shelve.DbfilenameShelf):
     cache: dict
     dict: dict
     writeback: bool
     keyencoding: str
@@ -31,32 +33,32 @@
         self.secret_key = key
 
     def __getitem__(self, key):
         try:
             value = self.cache[key]
         except KeyError:
             f = BytesIO(self.dict[key.encode(self.keyencoding)])
-            value = Unpickler(f, key=self.secret_key).load()
+            value = Unpickler(f, key=self.secret_key).load()  # type:ignore
             if self.writeback:
                 self.cache[key] = value
         return value
 
     def __setitem__(self, key, value):
         if self.writeback:
             self.cache[key] = value
         f = BytesIO()
-        p = Pickler(f, self._protocol, key=self.secret_key)
+        p = Pickler(f, self._protocol, key=self.secret_key)  # type:ignore
         p.dump(value)
         self.dict[key.encode(self.keyencoding)] = f.getvalue()
 
 
 @dataclasses.dataclass
 class GatewayUser:
     """
-    A dataclass representing a gateway user
+    A gateway user
     """
 
     bare_jid: str
     """Bare JID of the user"""
     registration_form: dict[str, Optional[str]]
     """Content of the registration form, as a dict"""
     plugin_data: Optional[dict] = None
@@ -78,25 +80,26 @@
         The user's (bare) JID
 
         :return:
         """
         return JID(self.bare_jid)
 
     def get(self, field: str, default: str = "") -> Optional[str]:
-        """
-        Get fields from the registration form (required to comply with slixmpp backend protocol)
-
-        :param field: Name of the field
-        :param default: Default value to return if the field is not present
-
-        :return: Value of the field
-        """
+        # """
+        # Get fields from the registration form (required to comply with slixmpp backend protocol)
+        #
+        # :param field: Name of the field
+        # :param default: Default value to return if the field is not present
+        #
+        # :return: Value of the field
+        # """
         return self.registration_form.get(field, default)
 
     def commit(self):
+        db.user_store(self)
         user_store.commit(self)
 
 
 class UserStore:
     """
     Basic user store implementation using shelve from the python standard library
 
@@ -119,14 +122,16 @@
             log.info("Using existing slidge DB: %s", filename)
         else:
             log.info("Creating a new slidge DB: %s", filename)
         if secret_key:
             self._users = EncryptedShelf(filename, key=secret_key)
         else:
             self._users = shelve.open(str(filename))
+        for user in self._users.values():
+            db.user_store(user)
         log.info("Registered users in the DB: %s", list(self._users.keys()))
 
     def get_all(self) -> Iterable[GatewayUser]:
         """
         Get all users in the store
 
         :return: An iterable of GatewayUsers
@@ -140,20 +145,21 @@
         NB: there is no reason to call this manually, as this should be covered
         by slixmpp XEP-0077 and XEP-0100 plugins
 
         :param jid: JID of the gateway user
         :param registration_form: Content of the registration form (:xep:`0077`)
         """
         log.debug("Adding user %s", jid)
-        self._users[jid.bare] = GatewayUser(
+        self._users[jid.bare] = user = GatewayUser(
             bare_jid=jid.bare,
             registration_form=registration_form,
             registration_date=datetime.datetime.now(),
         )
         self._users.sync()
+        user.commit()
         log.debug("Store: %s", self._users)
 
     def commit(self, user: GatewayUser):
         self._users[user.bare_jid] = user
         self._users.sync()
 
     def get(self, _gateway_jid, _node, ifrom: JID, iq) -> Optional[GatewayUser]:
@@ -183,14 +189,15 @@
 
     def remove_by_jid(self, jid: JID):
         """
         Remove a user from the store, by JID
         """
         j = jid.bare
         log.debug("Removing user %s", j)
+        db.user_del(self._users[j])
         del self._users[j]
         self._users.sync()
 
     def get_by_jid(self, jid: JID) -> Optional[GatewayUser]:
         """
         Convenience function to get a user from their JID.
 
@@ -209,67 +216,14 @@
         return self.get_by_jid(s.get_from())
 
     def close(self):
         self._users.sync()
         self._users.close()
 
 
-class YesSet(set):
-    """
-    A pseudo-set which always test True for membership
-    """
-
-    def __contains__(self, item):
-        log.debug("Test in")
-        return True
-
-
-class RosterBackend:
-    """
-    A pseudo-roster for the gateway component.
-
-    If a user is in the user store, this will behave as if the user is part of the
-    roster with subscription "both", and "none" otherwise.
-
-    This is rudimentary but the only sane way I could come up with so far.
-    """
-
-    @staticmethod
-    def entries(_owner_jid, _default=None):
-        return YesSet()
-
-    @staticmethod
-    def save(_owner_jid, _jid, _item_state, _db_state):
-        pass
-
-    @staticmethod
-    def load(_owner_jid, jid, _db_state):
-        log.debug("Load %s", jid)
-        user = user_store.get_by_jid(JID(jid))
-        log.debug("User %s", user)
-        if user is None:
-            return {
-                "name": "",
-                "groups": [],
-                "from": False,
-                "to": False,
-                "pending_in": False,
-                "pending_out": False,
-                "whitelisted": False,
-                "subscription": "both",
-            }
-        else:
-            return {
-                "name": "",
-                "groups": [],
-                "from": True,
-                "to": True,
-                "pending_in": False,
-                "pending_out": False,
-                "whitelisted": False,
-                "subscription": "none",
-            }
-
-
 user_store = UserStore()
+"""
+A persistent store for slidge users. Not public, but I didn't find how to hide
+it from the docs!
+"""
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/util/test.py` & `slidge-0.1.1/slidge/util/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,117 +1,50 @@
 # type:ignore
 import tempfile
 import types
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 from xml.dom.minidom import parseString
 
+import xmldiff.main
 from slixmpp import (
     ElementBase,
+    Iq,
     MatcherId,
     MatchXMLMask,
     MatchXPath,
     Message,
     Presence,
     StanzaPath,
 )
+from slixmpp.stanza.error import Error
 from slixmpp.test import SlixTest, TestTransport
 from slixmpp.xmlstream import highlight, tostring
 from slixmpp.xmlstream.matcher import MatchIDSender
 
-from slidge import *
+from slidge import (
+    BaseGateway,
+    BaseSession,
+    LegacyBookmarks,
+    LegacyContact,
+    LegacyMUC,
+    LegacyParticipant,
+    LegacyRoster,
+    user_store,
+)
 
+from ..command import Command
 from ..core import config
+from ..core.config import _TimedeltaSeconds
 
 
-class SlidgeTest(SlixTest):
-    plugin: Union[types.ModuleType, dict]
-
-    class Config:
-        jid = "aim.shakespeare.lit"
-        secret = "test"
-        server = "shakespeare.lit"
-        port = 5222
-        upload_service = "upload.test"
-        home_dir = Path(tempfile.mkdtemp())
-        user_jid_validator = ".*@shakespeare.lit"
-        admins: list[str] = []
-        no_roster_push = False
-        upload_requester = None
-        ignore_delay_threshold = 300
-
-    @classmethod
-    def setUpClass(cls):
-        user_store.set_file(Path(tempfile.mkdtemp()) / "test.db")
-        for k, v in vars(cls.Config).items():
-            setattr(config, k.upper(), v)
-
+class SlixTestPlus(SlixTest):
     def setUp(self):
-        BaseGateway._subclass = find_subclass(self.plugin, BaseGateway)
-        BaseSession._subclass = find_subclass(self.plugin, BaseSession)
-        LegacyRoster._subclass = find_subclass(self.plugin, LegacyRoster, base_ok=True)
-        LegacyContact._subclass = find_subclass(
-            self.plugin, LegacyContact, base_ok=True
-        )
-        LegacyMUC._subclass = find_subclass(self.plugin, LegacyMUC, base_ok=True)
-        LegacyBookmarks._subclass = find_subclass(
-            self.plugin, LegacyBookmarks, base_ok=True
-        )
-
-        self.xmpp = BaseGateway.get_self_or_unique_subclass()()
-
-        self.xmpp._always_send_everything = True
-
-        self.xmpp.connection_made(TestTransport(self.xmpp))
-        self.xmpp.session_bind_event.set()
-        # Remove unique ID prefix to make it easier to test
-        self.xmpp._id_prefix = ""
-        self.xmpp.default_lang = None
-        self.xmpp.peer_default_lang = None
-
-        def new_id():
-            self.xmpp._id += 1
-            return str(self.xmpp._id)
-
-        self.xmpp._id = 0
-        self.xmpp.new_id = new_id
-
-        # Must have the stream header ready for xmpp.process() to work.
-        header = self.xmpp.stream_header
-
-        self.xmpp.data_received(header)
-        self.wait_for_send_queue()
-
-        self.xmpp.socket.next_sent()
-        self.xmpp.socket.next_sent()
-
-        # Some plugins require messages to have ID values. Set
-        # this to True in tests related to those plugins.
-        self.xmpp.use_message_ids = False
-        self.xmpp.use_presence_ids = False
-
-    @classmethod
-    def tearDownClass(cls):
-        BaseSession.reset_subclass()
-        BaseGateway.reset_subclass()
-        LegacyRoster.reset_subclass()
-        LegacyContact.reset_subclass()
-        LegacyMUC.reset_subclass()
-        LegacyBookmarks.reset_subclass()
-        user_store._users = None
-
-    def next_sent(self):
-        self.wait_for_send_queue()
-        sent = self.xmpp.socket.next_sent(timeout=1)
-        if sent is None:
-            return None
-        xml = self.parse_xml(sent)
-        self.fix_namespaces(xml, "jabber:component:accept")
-        sent = self.xmpp._build_stanza(xml, "jabber:component:accept")
-        return sent
+        super().setUp()
+        Error.namespace = "jabber:component:accept"
 
     def check(self, stanza, criteria, method="exact", defaults=None, use_values=True):
         """
         Create and compare several stanza objects to a correct XML string.
 
         If use_values is False, tests using stanza.values will not be used.
 
@@ -214,16 +147,110 @@
                 debug = "Two methods for creating stanzas do not match.\n"
                 debug += "Given XML:\n%s\n" % highlight(tostring(xml))
                 debug += "Given stanza:\n%s\n" % format_stanza(stanza)
                 debug += "Generated stanza:\n%s\n" % highlight(tostring(stanza2.xml))
                 result = self.compare(xml, stanza.xml, stanza2.xml)
             stanza_class.namespace = old_ns
 
+            if not result:
+                debug += str(
+                    xmldiff.main.diff_texts(tostring(xml), tostring(stanza.xml))
+                )
+                if use_values:
+                    debug += str(
+                        xmldiff.main.diff_texts(tostring(xml), tostring(stanza2.xml))
+                    )
             self.assertTrue(result, debug)
 
+    def next_sent(self, timeout=0.05) -> Optional[Union[Message, Iq, Presence]]:
+        self.wait_for_send_queue()
+        sent = self.xmpp.socket.next_sent(timeout=timeout)
+        if sent is None:
+            return None
+        xml = self.parse_xml(sent)
+        self.fix_namespaces(xml, "jabber:component:accept")
+        sent = self.xmpp._build_stanza(xml, "jabber:component:accept")
+        return sent
+
+
+class SlidgeTest(SlixTestPlus):
+    plugin: Union[types.ModuleType, dict]
+
+    class Config:
+        jid = "aim.shakespeare.lit"
+        secret = "test"
+        server = "shakespeare.lit"
+        port = 5222
+        upload_service = "upload.test"
+        home_dir = Path(tempfile.mkdtemp())
+        user_jid_validator = ".*"
+        admins: list[str] = []
+        no_roster_push = False
+        upload_requester = None
+        ignore_delay_threshold = _TimedeltaSeconds("300")
+
+    @classmethod
+    def setUpClass(cls):
+        user_store.set_file(Path(tempfile.mkdtemp()) / "test.db")
+        for k, v in vars(cls.Config).items():
+            setattr(config, k.upper(), v)
+
+    def setUp(self):
+        if hasattr(self, "plugin"):
+            BaseGateway._subclass = find_subclass(self.plugin, BaseGateway)
+            BaseSession._subclass = find_subclass(self.plugin, BaseSession)
+            LegacyRoster._subclass = find_subclass(
+                self.plugin, LegacyRoster, base_ok=True
+            )
+            LegacyContact._subclass = find_subclass(
+                self.plugin, LegacyContact, base_ok=True
+            )
+            LegacyMUC._subclass = find_subclass(self.plugin, LegacyMUC, base_ok=True)
+            LegacyBookmarks._subclass = find_subclass(
+                self.plugin, LegacyBookmarks, base_ok=True
+            )
+
+        self.xmpp = BaseGateway.get_self_or_unique_subclass()()
+
+        self.xmpp._always_send_everything = True
+
+        self.xmpp.connection_made(TestTransport(self.xmpp))
+        self.xmpp.session_bind_event.set()
+        # Remove unique ID prefix to make it easier to test
+        self.xmpp._id_prefix = ""
+        self.xmpp.default_lang = None
+        self.xmpp.peer_default_lang = None
+
+        def new_id():
+            self.xmpp._id += 1
+            return str(self.xmpp._id)
+
+        self.xmpp._id = 0
+        self.xmpp.new_id = new_id
+
+        # Must have the stream header ready for xmpp.process() to work.
+        header = self.xmpp.stream_header
+
+        self.xmpp.data_received(header)
+        self.wait_for_send_queue()
+
+        self.xmpp.socket.next_sent()
+        self.xmpp.socket.next_sent()
+
+        # Some plugins require messages to have ID values. Set
+        # this to True in tests related to those plugins.
+        self.xmpp.use_message_ids = False
+        self.xmpp.use_presence_ids = False
+        Error.namespace = "jabber:component:accept"
+
+    @classmethod
+    def tearDownClass(cls):
+        reset_subclasses()
+        user_store._users = None
+
 
 def format_stanza(stanza):
     return highlight(
         "\n".join(parseString(tostring(stanza.xml)).toprettyxml().split("\n")[1:])
     )
 
 
@@ -239,7 +266,30 @@
         except TypeError:
             pass
     else:
         if base_ok:
             return parent
         else:
             raise RuntimeError
+
+
+def reset_subclasses():
+    """
+    Reset registered subclasses between test classes.
+
+    Needed because these classes are meant to only be subclassed once and raise
+    exceptions otherwise.
+    """
+    BaseSession.reset_subclass()
+    BaseGateway.reset_subclass()
+    LegacyRoster.reset_subclass()
+    LegacyContact.reset_subclass()
+    LegacyMUC.reset_subclass()
+    LegacyBookmarks.reset_subclass()
+    LegacyParticipant.reset_subclass()
+    # reset_commands()
+
+
+def reset_commands():
+    Command.subclasses = [
+        c for c in Command.subclasses if str(c).startswith("<class 'slidge.core")
+    ]
```

### Comparing `slidge-0.1.0rc1/slidge/util/xep_0077/register.py` & `slidge-0.1.1/slidge/slixfix/xep_0077/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from .stanza import Register, RegisterFeature
 
 log = logging.getLogger(__name__)
 
 
 # noinspection PyPep8Naming
 class XEP_0077(BasePlugin):
-
     """
     XEP-0077: In-Band Registration
 
     Events:
 
     ::
 
@@ -77,15 +76,15 @@
         register_stanza_plugin(Iq, Register)
 
         if self.xmpp.is_component:
             self.xmpp["xep_0030"].add_feature("jabber:iq:register")
             self.xmpp.register_handler(
                 CoroutineCallback(
                     "registration",
-                    StanzaPath("/iq/register"),
+                    StanzaPath(f"/iq@to={self.xmpp.boundjid.bare}/register"),
                     self._handle_registration,
                 )
             )
             self._user_store = {}
             self.api.register(self._user_get, "user_get")
             self.api.register(self._user_remove, "user_remove")
             self.api.register(self._user_modify, "user_modify")
```

### Comparing `slidge-0.1.0rc1/slidge/util/xep_0100/gateway.py` & `slidge-0.1.1/slidge/slixfix/xep_0100/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
+import warnings
 
 from slixmpp import JID, Iq, Message, Presence, register_stanza_plugin
+from slixmpp.exceptions import XMPPError
 from slixmpp.plugins.base import BasePlugin
 
 from slidge.core import config
 
 from . import stanza
 
 log = logging.getLogger(__name__)
@@ -77,27 +79,28 @@
             self.xmpp.boundjid.bare: {
                 "name": self.component_name,
                 "subscription": "both",
                 "groups": ["Slidge"],
             }
         }
         try:
+            await self._set_roster(jid, items)
+        except PermissionError:
+            warnings.warn(
+                "Slidge does not have the privilege to manage users' rosters. "
+                "Users should add the slidge component to their rosters manually."
+            )
+            if config.ROSTER_PUSH_PRESENCE_SUBSCRIPTION_REQUEST_FALLBACK:
+                self.xmpp.send_presence(ptype="subscribe", pto=jid.bare)
+
+    async def _set_roster(self, jid, items):
+        try:
             await self.xmpp["xep_0356"].set_roster(jid=jid.bare, roster_items=items)
         except PermissionError:
-            try:
-                await self.xmpp["xep_0356_old"].set_roster(
-                    jid=jid.bare, roster_items=items
-                )
-            except PermissionError:
-                log.warning(
-                    "Slidge does not have the privilege to manage users' rosters. "
-                    "Users should add the slidge component to their rosters manually."
-                )
-                if config.ROSTER_PUSH_PRESENCE_SUBSCRIPTION_REQUEST_FALLBACK:
-                    self.xmpp.send_presence(ptype="subscribe", pto=jid.bare)
+            await self.xmpp["xep_0356_old"].set_roster(jid=jid.bare, roster_items=items)
 
     def on_presence_unsubscribe(self, p: Presence):
         if p.get_to() == self.xmpp.boundjid.bare:
             log.debug("REMOVE: Our roster: %s", self.xmpp.client_roster)
             self.xmpp["xep_0077"].api["user_remove"](None, None, p["from"], p)
             self.xmpp.event("user_unregister", p)
 
@@ -107,10 +110,12 @@
 
         if msg["to"] == self.xmpp.boundjid.bare:
             # It may be useful to exchange direct messages with the component
             self.xmpp.event("gateway_message", msg)
             return
 
         if self.needs_registration and await self.get_user(msg) is None:
-            return
+            raise XMPPError(
+                "registration-required", text="You are not registered to this gateway"
+            )
 
         self.xmpp.event("legacy_message", msg)
```

### Comparing `slidge-0.1.0rc1/slidge/util/xep_0292/vcard4.py` & `slidge-0.1.1/slidge/slixfix/xep_0292/vcard4.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
-from dataclasses import dataclass, field
-from typing import Optional
+from typing import TYPE_CHECKING, NamedTuple, Optional
 
-from slixmpp import JID, ComponentXMPP, CoroutineCallback, Iq, StanzaPath
+from slixmpp import JID, CoroutineCallback, Iq, StanzaPath
 from slixmpp.plugins.base import BasePlugin, register_plugin
+from slixmpp.plugins.xep_0292.stanza import NS, VCard4
 from slixmpp.types import JidStr
 
-from .stanza import NS, VCard4
+from slidge.contact import LegacyContact
 
+if TYPE_CHECKING:
+    from slidge.core.gateway import BaseGateway
 
-@dataclass
-class StoredVCard:
+
+class StoredVCard(NamedTuple):
     content: VCard4
-    authorized_jids: set[JidStr] = field(default_factory=set)
+    authorized_jids: set[JidStr]
 
 
 class VCard4Provider(BasePlugin):
-    xmpp: ComponentXMPP
+    xmpp: "BaseGateway"
 
     name = "xep_0292_provider"
     description = "VCard4 Provider"
     dependencies = {"xep_0030"}
 
     def __init__(self, *a, **k):
         super(VCard4Provider, self).__init__(*a, **k)
@@ -33,42 +35,66 @@
                 StanzaPath(f"iq@type=get/vcard"),
                 self.handle_vcard_get,  # type:ignore
             )
         )
 
         self.xmpp.plugin["xep_0030"].add_feature(NS)
 
-    def get_vcard(self, jid: JidStr, requested_by: JidStr) -> Optional[VCard4]:
+    def _get_cached_vcard(self, jid: JidStr, requested_by: JidStr) -> Optional[VCard4]:
         vcard = self._vcards.get(JID(jid).bare)
         if vcard:
             if auth := vcard.authorized_jids:
                 if JID(requested_by).bare in auth:
                     return vcard.content
             else:
                 return vcard.content
         return None
 
+    async def get_vcard(self, jid: JidStr, requested_by: JidStr) -> Optional[VCard4]:
+        if vcard := self._get_cached_vcard(jid, requested_by):
+            log.debug("Found a cached vcard")
+            return vcard
+        if not hasattr(self.xmpp, "get_session_from_jid"):
+            return None
+        jid = JID(jid)
+        requested_by = JID(requested_by)
+        session = self.xmpp.get_session_from_jid(requested_by)
+        if session is None:
+            return
+        entity = await session.get_contact_or_group_or_participant(jid)
+        if isinstance(entity, LegacyContact):
+            log.debug("Fetching vcard")
+            await entity.fetch_vcard()
+            return self._get_cached_vcard(jid, requested_by)
+        return None
+
     async def handle_vcard_get(self, iq: Iq):
         r = iq.reply()
-        if vcard := self.get_vcard(iq.get_to().bare, iq.get_from().bare):
+        if vcard := await self.get_vcard(iq.get_to().bare, iq.get_from().bare):
             r.append(vcard)
         else:
             r.enable("vcard")
         r.send()
 
     def set_vcard(
         self,
         jid: JidStr,
         vcard: VCard4,
         /,
         authorized_jids: Optional[set[JidStr]] = None,
     ):
-        self._vcards[jid] = StoredVCard(
+        cache = self._vcards.get(jid)
+        new = StoredVCard(
             vcard, authorized_jids if authorized_jids is not None else set()
         )
+        self._vcards[jid] = new
+        if cache == new:
+            return
         if self.xmpp["pubsub"] and authorized_jids:
             for to in authorized_jids:
-                self.xmpp["pubsub"].broadcast_vcard_event(jid, to)
+                self.xmpp.loop.create_task(
+                    self.xmpp["pubsub"].broadcast_vcard_event(jid, to)
+                )
 
 
 register_plugin(VCard4Provider)
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0rc1/slidge/util/xep_0356/privilege.py` & `slidge-0.1.1/slidge/slixfix/xep_0356_old/privilege.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,87 +1,94 @@
 import logging
 import typing
 from collections import defaultdict
 
 from slixmpp import JID, Iq, Message
 from slixmpp.plugins.base import BasePlugin
+from slixmpp.plugins.xep_0356.permissions import (
+    MessagePermission,
+    Permissions,
+    RosterAccess,
+)
 from slixmpp.types import JidStr
 from slixmpp.xmlstream import StanzaBase
 from slixmpp.xmlstream.handler import Callback
 from slixmpp.xmlstream.matcher import StanzaPath
 
 from . import stanza
-from .permissions import MessagePermission, Permissions, RosterAccess
 
 log = logging.getLogger(__name__)
 
 
 # noinspection PyPep8Naming
-class XEP_0356(BasePlugin):
+class XEP_0356_OLD(BasePlugin):
     """
     XEP-0356: Privileged Entity
 
     Events:
 
     ::
 
-        privileges_advertised  -- Received message/privilege from the server
+        privileges_advertised_old -- Received message/privilege from the server
     """
 
-    name = "xep_0356"
-    description = "XEP-0356: Privileged Entity (slidge)"
+    name = "xep_0356_old"
+    description = "XEP-0356: Privileged Entity (slidge - old namespace)"
     dependencies = {"xep_0297"}
     stanza = stanza
 
     granted_privileges: defaultdict[JidStr, Permissions] = defaultdict(Permissions)
 
     def plugin_init(self):
         if not self.xmpp.is_component:
             log.error("XEP 0356 is only available for components")
             return
 
         stanza.register()
 
         self.xmpp.register_handler(
             Callback(
-                "Privileges",
-                StanzaPath("message/privilege"),
+                "Privileges_old",
+                StanzaPath("message/privilege_old"),
                 self._handle_privilege,
             )
         )
 
     def plugin_end(self):
-        self.xmpp.remove_handler("Privileges")
+        self.xmpp.remove_handler("Privileges_old")
 
     def _handle_privilege(self, msg: StanzaBase):
         """
         Called when the XMPP server advertise the component's privileges.
 
         Stores the privileges in this instance's granted_privileges attribute (a dict)
         and raises the privileges_advertised event
         """
-        for perm in msg["privilege"]["perms"]:
+        for perm in msg["privilege_old"]["perms"]:
             setattr(
                 self.granted_privileges[msg.get_from()], perm["access"], perm["type"]
             )
-        log.debug(f"Privileges: {self.granted_privileges}")
-        self.xmpp.event("privileges_advertised")
+        log.debug(f"Privileges (old): {self.granted_privileges}")
+        self.xmpp.event("privileges_advertised_old")
 
     def send_privileged_message(self, msg: Message):
-        if self.granted_privileges[msg.get_from().domain].message != MessagePermission.OUTGOING:
+        if (
+            self.granted_privileges[msg.get_from().domain].message
+            != MessagePermission.OUTGOING
+        ):
             raise PermissionError(
                 "The server hasn't authorized us to send messages on behalf of other users"
             )
         else:
             self._make_privileged_message(msg).send()
 
     def _make_privileged_message(self, msg: Message):
         server = msg.get_from().domain
         wrapped = self.xmpp.make_message(mto=server, mfrom=self.xmpp.boundjid.bare)
-        wrapped["privilege"]["forwarded"].append(msg)
+        wrapped["privilege_old"]["forwarded"].append(msg)
         return wrapped
 
     def _make_get_roster(self, jid: typing.Union[JID, str], **iq_kwargs):
         return self.xmpp.make_iq_get(
             queryxmlns="jabber:iq:roster",
             ifrom=self.xmpp.boundjid.bare,
             ito=jid,
```

### Comparing `slidge-0.1.0rc1/slidge/util/xep_0356/stanza.py` & `slidge-0.1.1/slidge/slixfix/xep_0356_old/stanza.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from slixmpp.plugins.xep_0297 import Forwarded
 from slixmpp.stanza import Message
 from slixmpp.xmlstream import ElementBase, register_stanza_plugin
 
 
-class Privilege(ElementBase):
-    namespace = "urn:xmpp:privilege:2"
+class PrivilegeOld(ElementBase):
+    namespace = "urn:xmpp:privilege:1"
     name = "privilege"
-    plugin_attrib = "privilege"
+    plugin_attrib = "privilege_old"
 
     def permission(self, access):
         for perm in self["perms"]:
             if perm["access"] == access:
                 return perm["type"]
 
     def roster(self):
@@ -18,27 +18,27 @@
 
     def message(self):
         return self.permission("message")
 
     def presence(self):
         return self.permission("presence")
 
-    def add_perm(self, access, type_):
+    def add_perm(self, access, type):
         # This should only be needed for servers, so maybe out of scope for slixmpp
-        perm = Perm()
-        perm["type"] = type_
+        perm = PermOld()
+        perm["type"] = type
         perm["access"] = access
         self.append(perm)
 
 
-class Perm(ElementBase):
-    namespace = "urn:xmpp:privilege:2"
+class PermOld(ElementBase):
+    namespace = "urn:xmpp:privilege:1"
     name = "perm"
     plugin_attrib = "perm"
     plugin_multi_attrib = "perms"
     interfaces = {"type", "access"}
 
 
 def register():
-    register_stanza_plugin(Message, Privilege)
-    register_stanza_plugin(Privilege, Forwarded)
-    register_stanza_plugin(Privilege, Perm, iterable=True)
+    register_stanza_plugin(Message, PrivilegeOld)
+    register_stanza_plugin(PrivilegeOld, Forwarded)
+    register_stanza_plugin(PrivilegeOld, PermOld, iterable=True)
```

