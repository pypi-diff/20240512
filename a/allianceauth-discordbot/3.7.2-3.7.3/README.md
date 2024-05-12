# Comparing `tmp/allianceauth_discordbot-3.7.2.tar.gz` & `tmp/allianceauth_discordbot-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth_discordbot-3.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "allianceauth_discordbot-3.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth_discordbot-3.7.2.tar` & `allianceauth_discordbot-3.7.3.tar`

### file list

```diff
@@ -1,67 +1,72 @@
--rw-r--r--   0        0        0     1322 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/.github/workflows/main.yml
--rw-r--r--   0        0        0      719 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      339 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/.gitignore
--rw-r--r--   0        0        0      179 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/.isort.cfg
--rw-r--r--   0        0        0     1164 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      267 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/.tx/transifex.yml
--rw-r--r--   0        0        0     3233 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     1077 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/LICENSE
--rw-r--r--   0        0        0      109 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/MANIFEST.in
--rw-r--r--   0        0        0      636 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/Makefile
--rw-r--r--   0        0        0    15369 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/README.md
--rw-r--r--   0        0        0      176 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/__init__.py
--rw-r--r--   0        0        0     1977 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/admin.py
--rw-r--r--   0        0        0     4370 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/app_settings.py
--rw-r--r--   0        0        0      263 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/apps.py
--rw-r--r--   0        0        0      928 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/auth_hooks.py
--rw-r--r--   0        0        0    17002 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/bot.py
--rw-r--r--   0        0        0     4774 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/bot_tasks.py
--rw-r--r--   0        0        0        0 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/__init__.py
--rw-r--r--   0        0        0     3261 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/about.py
--rw-r--r--   0        0        0     2931 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/abuse.py
--rw-r--r--   0        0        0     1093 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/abuse_two.py
--rw-r--r--   0        0        0    16421 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/admin.py
--rw-r--r--   0        0        0     2694 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/auth.py
--rw-r--r--   0        0        0      909 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/eastereggs.py
--rw-r--r--   0        0        0     1459 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/eightball.py
--rw-r--r--   0        0        0     3827 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/facwar.py
--rw-r--r--   0        0        0    12709 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/members.py
--rw-r--r--   0        0        0     3531 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/models.py
--rw-r--r--   0        0        0     5703 2024-01-31 09:29:21.807413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/price_check.py
--rw-r--r--   0        0        0     1495 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/prom_export.py
--rw-r--r--   0        0        0     5180 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/quote.py
--rw-r--r--   0        0        0     6214 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/reaction_roles.py
--rw-r--r--   0        0        0     1201 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/remind.py
--rw-r--r--   0        0        0     6532 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/services.py
--rw-r--r--   0        0        0    15830 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/sov.py
--rw-r--r--   0        0        0     4650 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/tickets.py
--rw-r--r--   0        0        0     1396 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/time.py
--rw-r--r--   0        0        0     2171 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/timers.py
--rw-r--r--   0        0        0        0 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/utils/__init__.py
--rw-r--r--   0        0        0      207 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/utils/context.py
--rw-r--r--   0        0        0     3883 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/utils/decorators.py
--rw-r--r--   0        0        0      437 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/utils/exceptions.py
--rw-r--r--   0        0        0     4373 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/cogs/welcomegoodbye.py
--rw-r--r--   0        0        0      235 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/launcher.py
--rw-r--r--   0        0        0      380 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1027 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1621 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0001_initial.py
--rw-r--r--   0        0        0     1410 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
--rw-r--r--   0        0        0      636 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0003_authbotconfiguration.py
--rw-r--r--   0        0        0      485 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0004_settings.py
--rw-r--r--   0        0        0      759 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
--rw-r--r--   0        0        0     1773 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
--rw-r--r--   0        0        0     1219 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0007_quotemessage.py
--rw-r--r--   0        0        0      413 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0008_channels_deleted.py
--rw-r--r--   0        0        0      507 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0009_alter_quotemessage_options.py
--rw-r--r--   0        0        0     1056 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
--rw-r--r--   0        0        0      805 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
--rw-r--r--   0        0        0        0 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/migrations/__init__.py
--rw-r--r--   0        0        0     5148 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/models.py
--rw-r--r--   0        0        0      317 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/providers.py
--rw-r--r--   0        0        0     3667 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/tasks.py
--rw-r--r--   0        0        0       45 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/urls.py
--rw-r--r--   0        0        0       15 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/aadiscordbot/views.py
--rw-r--r--   0        0        0      315 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/bot_conf.py
--rw-r--r--   0        0        0      866 2024-01-31 09:29:21.811413 allianceauth_discordbot-3.7.2/pyproject.toml
--rw-r--r--   0        0        0    16137 1970-01-01 00:00:00.000000 allianceauth_discordbot-3.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1322 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0      719 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      339 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.gitignore
+-rw-r--r--   0        0        0      179 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.isort.cfg
+-rw-r--r--   0        0        0     2553 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/.tx/transifex.yml
+-rw-r--r--   0        0        0     3318 2024-05-12 08:25:35.969976 allianceauth_discordbot-3.7.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1077 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/LICENSE
+-rw-r--r--   0        0        0      109 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/MANIFEST.in
+-rw-r--r--   0        0        0      636 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/Makefile
+-rw-r--r--   0        0        0    16093 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/README.md
+-rw-r--r--   0        0        0      176 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/__init__.py
+-rw-r--r--   0        0        0     2069 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/admin.py
+-rw-r--r--   0        0        0     4370 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/app_settings.py
+-rw-r--r--   0        0        0      263 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/apps.py
+-rw-r--r--   0        0        0      928 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/auth_hooks.py
+-rw-r--r--   0        0        0    17002 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/bot.py
+-rw-r--r--   0        0        0     4774 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/bot_tasks.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/__init__.py
+-rw-r--r--   0        0        0     3261 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/about.py
+-rw-r--r--   0        0        0     2931 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse.py
+-rw-r--r--   0        0        0     1093 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse_two.py
+-rw-r--r--   0        0        0    16421 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/admin.py
+-rw-r--r--   0        0        0     2694 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/auth.py
+-rw-r--r--   0        0        0      909 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eastereggs.py
+-rw-r--r--   0        0        0     1459 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eightball.py
+-rw-r--r--   0        0        0     3827 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/facwar.py
+-rw-r--r--   0        0        0    12709 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/members.py
+-rw-r--r--   0        0        0     3531 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/models.py
+-rw-r--r--   0        0        0     5703 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/price_check.py
+-rw-r--r--   0        0        0     1495 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/prom_export.py
+-rw-r--r--   0        0        0     5180 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/quote.py
+-rw-r--r--   0        0        0     6214 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/reaction_roles.py
+-rw-r--r--   0        0        0     1201 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/remind.py
+-rw-r--r--   0        0        0     6532 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/services.py
+-rw-r--r--   0        0        0    15830 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/sov.py
+-rw-r--r--   0        0        0     4650 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/tickets.py
+-rw-r--r--   0        0        0     1396 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/time.py
+-rw-r--r--   0        0        0     2171 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/timers.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/context.py
+-rw-r--r--   0        0        0     3883 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/decorators.py
+-rw-r--r--   0        0        0      437 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/exceptions.py
+-rw-r--r--   0        0        0     4831 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/cogs/welcomegoodbye.py
+-rw-r--r--   0        0        0      235 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/launcher.py
+-rw-r--r--   0        0        0     1235 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1027 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1621 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1410 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
+-rw-r--r--   0        0        0      636 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0003_authbotconfiguration.py
+-rw-r--r--   0        0        0      485 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0004_settings.py
+-rw-r--r--   0        0        0      759 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
+-rw-r--r--   0        0        0     1773 2024-05-12 08:25:35.973976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
+-rw-r--r--   0        0        0     1219 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0007_quotemessage.py
+-rw-r--r--   0        0        0      413 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0008_channels_deleted.py
+-rw-r--r--   0        0        0      507 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0009_alter_quotemessage_options.py
+-rw-r--r--   0        0        0     1056 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py
+-rw-r--r--   0        0        0      805 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py
+-rw-r--r--   0        0        0      437 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0012_welcomemessage_guild_id.py
+-rw-r--r--   0        0        0      425 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0013_goodbyemessage_guild_id.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/migrations/__init__.py
+-rw-r--r--   0        0        0     5294 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/models.py
+-rw-r--r--   0        0        0      317 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/providers.py
+-rw-r--r--   0        0        0     3667 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/tasks.py
+-rw-r--r--   0        0        0       45 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/urls.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/utils/__init__.py
+-rw-r--r--   0        0        0     3349 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/utils/auth.py
+-rw-r--r--   0        0        0       15 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/aadiscordbot/views.py
+-rw-r--r--   0        0        0      315 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/bot_conf.py
+-rw-r--r--   0        0        0     2174 2024-05-12 08:25:35.977976 allianceauth_discordbot-3.7.3/pyproject.toml
+-rw-r--r--   0        0        0    17687 1970-01-01 00:00:00.000000 allianceauth_discordbot-3.7.3/PKG-INFO
```

### Comparing `allianceauth_discordbot-3.7.2/.github/workflows/main.yml` & `allianceauth_discordbot-3.7.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/.github/workflows/publish.yml` & `allianceauth_discordbot-3.7.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/CHANGELOG.md` & `allianceauth_discordbot-3.7.3/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,175 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [3.7.3]
+
+- Maintenance release
+
 ## [3.3.0]
 
 ### New
+
 * WelcomeGoodbye Cog, responds to User Leave and Join events with customizable messages.
 
 ## [3.2.0]
 
 ### New
+
 * Reworked the task consumer to alow tasks to persist a gracefull restart
+
 - Added a configurable global rate limit option on tasks
 
 ## [3.1.2]
 
 ### New
+
 * Added ability to run bot on its own tokens
 
 ## [3.1.1]
 
 ### Fixes
+
 * Added very verbose logging to any startup errors
+
 + Added a 2 min cool down on hard failures at startup
 
 ## [3.1.0]
 
 ### Added
+
 * Updated Discord lib
+
 + Added startup checks to ensure admins know if there is an iuus with their bot
-+ Moved more commands to slash
+- Moved more commands to slash
 
 ## [3.0.1] - [3.0.5]
+
 + Updated things, fixed odd bugs
 
 ## [3.0.0]
 
 ### Added
+
 * Moved to new Discord library
+
 + Swapped many commands to Slash
-+ Full Reaction Roles support with public member access
+- Full Reaction Roles support with public member access
 
 ## [0.5.2] 2021-07-09
 
 ### Added
+
 * More Permission Decorators
+
 ### Fixes
+
 * Corrected a typo in the in_channel permissions decorater
+
 ## [0.5.1] 2021-07-09
+
 ### Added
+
 * Allows Prefix to be set as a setting
+
 ### Fixed
+
 * Documents all settings in readme
+
 ## [0.5.0] 2021-07-09
+
 ### Fixes
+
 * Mostly internal changes
-* Logging is cleaned and documented
-* Permissions are moved into Decorators and consistent across all cogs (and can be used my others)
-* All app settings are properly sanitized and defaulted
-* Prefix and Access Denied reacc can be configured
+- Logging is cleaned and documented
+- Permissions are moved into Decorators and consistent across all cogs (and can be used my others)
+- All app settings are properly sanitized and defaulted
+- Prefix and Access Denied reacc can be configured
 
 ## [0.4.0] 2021-05-05
+
 ### Added
+
 * Price Check Cog, PR #40 (@ppfeufer)
+
 ### Fixes
+
 * Use the Django Application Registry instead of reading INSTALLED_APPS, @ErikKalkoken
 
 ## [0.3.1] 2021-02-06
+
 ### Added
+
 * Added PyPi Deployment stuffs
+
 ### Fixes
+
 * Lookup cog doesnt throw error on not found. PR #33 (@ppfeufer)
 
 ## [0.3.0] 2021-02-05
+
 First Non-Alpha Release, AA-Discord bot has been heavily tested by the community now, many thanks to all involved.
+
 ### Added
+
 * App Cogs can now be customized to load external cogs
-* New shiny Time cog, using AA-Timezones
+- New shiny Time cog, using AA-Timezones
+
 ### Fixes
+
 * Use AA-Statistics, the rebranded authanalitics
 
 ### Docs
+
 Notated Integrations
+
 ## [0.2.5a Alpha] 2021-01-05
+
 ### Fixes
+
 * Readme reflects new settings formats
-* Cogs are configurable by Settings
-* Docker Support (again)
-* Refactor Channel/Direct message tasks to be more AA aware, adds shims to old tasks.
+- Cogs are configurable by Settings
+- Docker Support (again)
+- Refactor Channel/Direct message tasks to be more AA aware, adds shims to old tasks.
 
 ## [0.2.4a Alpha] 2021-01-02
+
 ### Fixes
+
 * Removes Click dependency for better Python 3.6 support
-* Server model was returning invalid server_name as its string
+- Server model was returning invalid server_name as its string
 
 ## [0.2.1a Alpha] 2021-01-02
+
 ### Fixes
+
 * Adds some logging
 
 ## [0.2.0a Alpha] 2021-01-02
+
 The initial migration was edited here, be aware you might need to migrate zero before you update
+
 ### Added
+
 * Documented all Cogs. Plenty changed here to polish them just read the readme...
-* Adds tasks to send Direct and Private Messages
+- Adds tasks to send Direct and Private Messages
+
 ### Fixes
+
 * Postgres Compatability
-* Module Compatability, only imports features if they are installed.
+- Module Compatability, only imports features if they are installed.
 
 ## [0.1.13a PreRelease]
+
 * A lot of things happened here, we suck at changelogs
 
 ## [0.0.2a1 PreRelease] - 2020-09-21
 
 ### Added
+
 * !Auth Cog
-* Requirements to Setup.py
-* Install Documentation
+- Requirements to Setup.py
+- Install Documentation
```

### Comparing `allianceauth_discordbot-3.7.2/LICENSE` & `allianceauth_discordbot-3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/Makefile` & `allianceauth_discordbot-3.7.3/Makefile`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/README.md` & `allianceauth_discordbot-3.7.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,18 +46,17 @@
     * promote_role_to_god/demote_role_to_god - promote/demote a role to/from full admin so for when you need it
     * empty_roles - list all roles on server with no members
     * clear_empty_roles - remove all empty roles from the server
     * orphans - find any user in discord with no auth user attached
     * get_webhooks - returns any webhooks setup in this current channel, or creates one for you and returns that
     * uptime - how long the bot has been up for
 
-
 ## Installation
 
-* Ensure you have installed and configured the Alliance Auth Discord Service, https://allianceauth.readthedocs.io/en/latest/features/services/discord.html
+* Ensure you have installed and configured the Alliance Auth Discord Service, <https://allianceauth.readthedocs.io/en/latest/features/services/discord.html>
 
 * Update your [Discord Developer Application](https://discord.com/developers/applications) to include the Privileged Intents that we call. Please enable all intents.
 
 ![screenshot](https://i.imgur.com/A1yA24P.png)
 
 * Install the app with your venv active
 
@@ -114,14 +113,50 @@
 
 * Fetch `bot_conf.py` from the Git Repo into the root of your AA install, beside `manage.py`
 
 ```bash
 wget https://raw.githubusercontent.com/pvyParts/allianceauth-discordbot/master/bot_conf.py
 ```
 
+## Running Discordbot with Docker
+
+Update base image to have bot_conf.py mapped
+
+```dockerfile
+x-allianceauth-base:
+
+# image: ${AA_DOCKER_TAG?err}
+
+  &allianceauth-base
+  build:
+    context: .
+    dockerfile: custom.dockerfile
+    args:
+      AA_DOCKER_TAG: ${AA_DOCKER_TAG?err}
+  restart: always
+  env_file:
+    - ./.env
+  volumes:
+...
+    - ./conf/bot_conf.py:/home/allianceauth/myauth/bot_conf.py
+...
+```
+
+Add a service to run the Discordbot
+
+```dockerfile
+  allianceauth_discordbot:
+    container_name: allianceauth_discordbot
+    <<: [ *allianceauth-base ]
+    restart: on-failure:1
+    entrypoint: [ "python", "/home/allianceauth/myauth/bot_conf.py" ]
+```
+
+## Running DiscordBot with Supervisor
+
 * Amend your supervisor.conf, correcting paths as required and add `authbot` to the launch group at the end of the conf
 
 ```ini
 [program:authbot]
 command=/home/allianceserver/venv/auth/bin/python /home/allianceserver/myauth/bot_conf.py
 directory=/home/allianceserver/myauth
 user=allianceserver
@@ -138,22 +173,24 @@
 [group:myauth]
 programs=beat,worker,gunicorn,authbot
 priority=999
 ```
 
 Go to admin and configure your admin users in the bot config model.
 
-
 > Enable groups/states/users to utilize the lookup command by adding permissions under **corputils | corp stats |**
+
 ```ini
 corputils.view_alliance_corpstats
 ```
 
 ## Optional Settings
+
 ### Built in Cogs
+
  ```python
 # Change the bots default Cogs, add or remove if you want to use any of the extra cogs.
 
 DISCORD_BOT_COGS = [
   "aadiscordbot.cogs.about", # about the bot
   "aadiscordbot.cogs.admin", # Discord server admin helpers
   "aadiscordbot.cogs.members", # Member lookup commands
@@ -172,65 +209,77 @@
   "aadiscordbot.cogs.quote", # Save and recall messages
   "aadiscordbot.cogs.prom_export", # Admin Level Logging cog
   "aadiscordbot.cogs.tickets", # Private thread ticket system with pingable groups.
   ]
 ```
 
 ### Additional Rate Limiting
+
 ```python
 # configure the optional rate limited
 # this is a bot_task function and how many / time period
 # 100/s equates to 100 per second max
 # 10/m equates to 10 per minute or 1 every 6 seconds max
 # 60/h equates to 60 per hour or one per minute max
 DISCORD_BOT_TASK_RATE_LIMITS = {
         "send_channel_message_by_discord_id": "100/s",
         "send_direct_message_by_discord_id": "1/s",
         "send_direct_message_by_user_id": "1/s"
         }
 ```
 
 ## Reaction Roles
+>
 > ❗❗❗ **This will bypass the Group Leadership/Join Request System**: This is intended for open groups but not limited to it! ❗❗❗
 
 The bot is able to run a reaction roles system that is compatible with auth and public users on a discord.
- - If a member is part of auth it will do auth syncing of roles
- - If a member is not found in auth and the reaction role message has the public flag set it will assign roles to anyone who reacts
 
-### How To Reaction Role!
+* If a member is part of auth it will do auth syncing of roles
+* If a member is not found in auth and the reaction role message has the public flag set it will assign roles to anyone who reacts
+
+### How To Reaction Role
+
  1. Setup the inital Message you wish to use buy using the command `!rr`
-   - *Optional* Edit the name and settings of this message in `Admin > Discord Bot > Reaction Role Messages`
+
+    * _Optional_ Edit the name and settings of this message in `Admin > Discord Bot > Reaction Role Messages`
+
  2. React to the message with the reactions you wish to use.
  3. The bot will counter react to the reactions when it creates the binding in auth.
  4. Goto `Admin > Discord Bot > Reaction Role Bindings`
  5. Assign the groups you want for each reaction
 
 #### Messages Admin
+
 ![https://cdn.discordapp.com/attachments/639369068930924546/936082605156237332/unknown.png](https://cdn.discordapp.com/attachments/639369068930924546/936082605156237332/unknown.png)
+
 #### Reactions Admin
+
 ![https://cdn.discordapp.com/attachments/639369068930924546/936084126379962378/unknown.png](https://cdn.discordapp.com/attachments/639369068930924546/936084126379962378/unknown.png)
 
 ## Integrations
+
 * [Statistics](https://github.com/pvyParts/aa-statistics)
   * Adds zkill Monthly/Yearly stats to !lookup
 * [timezones](https://github.com/ppfeufer/aa-timezones)
   * Updates the `time` command to have all timezones configured in auth.
 
 ## Welcome Messaages
+
 `
 With the WelcomeGoodbye Cog activated, Discordbot will grab a random message from the Welcome or Goodbye Message Model and send it to the Guild System channel
 
 These can be configured in admin under `/admin/aadiscordbot/welcomemessage/` and `/admin/aadiscordbot/goodbyemessage/`
 
 The messages support some string formatting
 
 * `{user_mention} - A Discord @ Mention
 * `{guild_name} - The name of the Discord Server
 * `{auth_url} - A link to Auth
-```
+
+```text
 Welcome {user_mention} to {guild_name}, I hope you enjoy your stay.
 
 You can Authenticate for more access {auth_url}
 ```
 
 ## Private Thread Ticket System
 
@@ -238,31 +287,34 @@
 
 With the `aadiscordbot.cogs.tickets` Cog activated, users wll be able to issue the `/help` command to pick a group to get help from.
 
 The groups available for selection are configurable in the site admin under
 `Discord Bot > Ticket Cog Configuration`
 
 You also need to choose a channel to create the threads in from the site admin `Discord Bot > Ticket Cog Configuration`:
-  - Anyone who can use the `/help` command must have View and Send Message permissions on this channel otherwise they will not be able to see the tickets authbot creates for them
-  - Authbot must have the permissions to create private threads in this channel
-  - Authbot must have the permissions to send messages to this channel
 
+* Anyone who can use the `/help` command must have View and Send Message permissions on this channel otherwise they will not be able to see the tickets authbot creates for them
+* Authbot must have the permissions to create private threads in this channel
+* Authbot must have the permissions to send messages to this channel
 
 ## Using AA-Discordbot from my project
 
 ### Send Messages
+
 You can use the send_message helper to send a message with text/embed to:
-  - Discord user_id
-  - Discord channel_id
-  - Auth User Model Object
-  - Auth user_pk
+
+* Discord user_id
+* Discord channel_id
+* Auth User Model Object
+* Auth user_pk
 
 [aadiscordbot/tasks.py](https://github.com/pvyParts/allianceauth-discordbot/blob/master/aadiscordbot/tasks.py)
 
 ### Example Usage
+
 ```python
 from django.contrib.auth.models import User
 from django.apps import apps
 
 ## Use a small helper to check if AA-Discordbot is installs
 def discord_bot_active():
     return apps.is_installed('aadiscordbot')
@@ -331,39 +383,44 @@
                 message=msg,
                 embed=e)
 ```
 
 ### Registering 3rd Party Cogs (Handling Commands)
 
 In `auth_hooks.py`, define a function that returns an array of cog modules, and register it as a `discord_cogs_hook`:
+
 ```python
 @hooks.register('discord_cogs_hook')
 def register_cogs():
     return ["yourapp.cogs.cog_a", "yourapp.cogs.cog_b"]
 ```
 
-## Optional Settings
+## Optional Settings continued
+
 ### Isolate AuthBot from Auth's Discord Service
+
 ```python
 AUTHBOT_DISCORD_APP_ID = 'App ID for dedicated bot'
 AUTHBOT_DISCORD_BOT_TOKEN = 'Token for dedicated bot'
 ```
 
 ## Issues
 
 Please remember to report any aa-discordbot related issues using the issues on **this** repository.
 
 ## Troubleshooting
 
 ### Py-Cord and discord.py fighting in venv
+
 **Problem:**
 
 Something has gone funny with my venv after i installed another app that wanted `discord.py`
 
 **Reason:**
 
 This is due to the Py-cord lib sharing the `discord` namespace. Py-Cord is however a drop in replacement. So no issues should arise from using it over the now legacy discord.py lib. **YMMV**
 
 **Fix:**
+
  1. Uninstall `discord.py` by running `pip uninstall discord.py` with your venv active.
  2. Reinstall `py-cord` by running `pip install -U py-cord==2.0.0b3` with your venv active.
  3. Approach the dev from the app that overrode your py-cord to update to a maintained lib.
```

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/admin.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,18 +66,18 @@
         except:
             b = ob.emoji_text
         return b
 
 
 @admin.register(WelcomeMessage)
 class WelcomeMessageAdmin(admin.ModelAdmin):
-    list_display = ('id', )
+    list_display = ('guild_id', 'id', "authenticated", "unauthenticated")
 
 
 @admin.register(GoodbyeMessage)
 class GoodbyeMessageAdmin(admin.ModelAdmin):
-    list_display = ('id', )
+    list_display = ('guild_id', 'id', "authenticated", "unauthenticated")
 
 
 @admin.register(TicketGroups)
 class TicketGroupAdmin(admin.ModelAdmin):
     filter_horizontal = ['groups']
```

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/app_settings.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/auth_hooks.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/bot.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/bot.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/bot_tasks.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/bot_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/about.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/about.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/abuse.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/abuse_two.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/abuse_two.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/admin.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/auth.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/eastereggs.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eastereggs.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/eightball.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/eightball.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/facwar.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/facwar.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/members.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/members.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/models.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/price_check.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/price_check.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/prom_export.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/prom_export.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/quote.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/quote.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/reaction_roles.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/reaction_roles.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/remind.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/remind.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/services.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/services.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/sov.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/sov.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/tickets.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/tickets.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/time.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/timers.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/cogs/utils/decorators.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/cogs/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/locale/en/LC_MESSAGES/django.po` & `allianceauth_discordbot-3.7.3/aadiscordbot/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0001_initial.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0003_authbotconfiguration.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0003_authbotconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0007_quotemessage.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0007_quotemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0010_alter_discordbot_options_ticketgroups.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/migrations/0011_alter_ticketgroups_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/models.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,26 +103,28 @@
 
 
 class WelcomeMessage(models.Model):
     message = models.TextField(_("Welcome Message"))
     authenticated = models.BooleanField(_("Valid for Authenticated Users"))
     unauthenticated = models.BooleanField(
         _("Valid for Un-Authenticated Users"))
+    guild_id = models.BigIntegerField(default=settings.DISCORD_GUILD_ID)
 
     class Meta:
         default_permissions = ()
         verbose_name = 'Welcome Message'
         verbose_name_plural = 'Welcome Messages'
 
 
 class GoodbyeMessage(models.Model):
     message = models.TextField(_("Goodbye Message"))
     authenticated = models.BooleanField(_("Valid for Authenticated Users"))
     unauthenticated = models.BooleanField(
         _("Valid for Un-Authenticated Users"))
+    guild_id = models.BigIntegerField(default=settings.DISCORD_GUILD_ID)
 
     class Meta:
         default_permissions = ()
         verbose_name = 'Goodbye Message'
         verbose_name_plural = 'Goodbye Messages'
```

### Comparing `allianceauth_discordbot-3.7.2/aadiscordbot/tasks.py` & `allianceauth_discordbot-3.7.3/aadiscordbot/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_discordbot-3.7.2/PKG-INFO` & `allianceauth_discordbot-3.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,36 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.7.2
+Version: 3.7.3
 Summary: Alliance Auth Modular Discord Bot
+Keywords: allianceauth,eveonline
 Author-email: AaronKable <aaronkable@gmail.com>
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Celery
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: allianceauth>=2.9.0
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Requires-Dist: allianceauth>=3.0.0,<5.0.0
 Requires-Dist: py-cord>2.0.0,<3.0.0
-Requires-Dist: pendulum>=2.1.2,<3.0.0
+Requires-Dist: pendulum>=2.1.2,<4.0.0
 Requires-Dist: redis>=4.2.0,<5.0.0
 Requires-Dist: django-solo>=2.1.0,<3.0.0
 Project-URL: Home, https://github.com/Solar-Helix-Independent-Transport/allianceauth-discordbot
 Project-URL: Source, https://github.com/Solar-Helix-Independent-Transport/allianceauth-discordbot
 Project-URL: Tracker, https://github.com/Solar-Helix-Independent-Transport/allianceauth-discordbot/issues
 
 # AA-Discordbot
@@ -63,18 +81,17 @@
     * promote_role_to_god/demote_role_to_god - promote/demote a role to/from full admin so for when you need it
     * empty_roles - list all roles on server with no members
     * clear_empty_roles - remove all empty roles from the server
     * orphans - find any user in discord with no auth user attached
     * get_webhooks - returns any webhooks setup in this current channel, or creates one for you and returns that
     * uptime - how long the bot has been up for
 
-
 ## Installation
 
-* Ensure you have installed and configured the Alliance Auth Discord Service, https://allianceauth.readthedocs.io/en/latest/features/services/discord.html
+* Ensure you have installed and configured the Alliance Auth Discord Service, <https://allianceauth.readthedocs.io/en/latest/features/services/discord.html>
 
 * Update your [Discord Developer Application](https://discord.com/developers/applications) to include the Privileged Intents that we call. Please enable all intents.
 
 ![screenshot](https://i.imgur.com/A1yA24P.png)
 
 * Install the app with your venv active
 
@@ -131,14 +148,50 @@
 
 * Fetch `bot_conf.py` from the Git Repo into the root of your AA install, beside `manage.py`
 
 ```bash
 wget https://raw.githubusercontent.com/pvyParts/allianceauth-discordbot/master/bot_conf.py
 ```
 
+## Running Discordbot with Docker
+
+Update base image to have bot_conf.py mapped
+
+```dockerfile
+x-allianceauth-base:
+
+# image: ${AA_DOCKER_TAG?err}
+
+  &allianceauth-base
+  build:
+    context: .
+    dockerfile: custom.dockerfile
+    args:
+      AA_DOCKER_TAG: ${AA_DOCKER_TAG?err}
+  restart: always
+  env_file:
+    - ./.env
+  volumes:
+...
+    - ./conf/bot_conf.py:/home/allianceauth/myauth/bot_conf.py
+...
+```
+
+Add a service to run the Discordbot
+
+```dockerfile
+  allianceauth_discordbot:
+    container_name: allianceauth_discordbot
+    <<: [ *allianceauth-base ]
+    restart: on-failure:1
+    entrypoint: [ "python", "/home/allianceauth/myauth/bot_conf.py" ]
+```
+
+## Running DiscordBot with Supervisor
+
 * Amend your supervisor.conf, correcting paths as required and add `authbot` to the launch group at the end of the conf
 
 ```ini
 [program:authbot]
 command=/home/allianceserver/venv/auth/bin/python /home/allianceserver/myauth/bot_conf.py
 directory=/home/allianceserver/myauth
 user=allianceserver
@@ -155,22 +208,24 @@
 [group:myauth]
 programs=beat,worker,gunicorn,authbot
 priority=999
 ```
 
 Go to admin and configure your admin users in the bot config model.
 
-
 > Enable groups/states/users to utilize the lookup command by adding permissions under **corputils | corp stats |**
+
 ```ini
 corputils.view_alliance_corpstats
 ```
 
 ## Optional Settings
+
 ### Built in Cogs
+
  ```python
 # Change the bots default Cogs, add or remove if you want to use any of the extra cogs.
 
 DISCORD_BOT_COGS = [
   "aadiscordbot.cogs.about", # about the bot
   "aadiscordbot.cogs.admin", # Discord server admin helpers
   "aadiscordbot.cogs.members", # Member lookup commands
@@ -189,65 +244,77 @@
   "aadiscordbot.cogs.quote", # Save and recall messages
   "aadiscordbot.cogs.prom_export", # Admin Level Logging cog
   "aadiscordbot.cogs.tickets", # Private thread ticket system with pingable groups.
   ]
 ```
 
 ### Additional Rate Limiting
+
 ```python
 # configure the optional rate limited
 # this is a bot_task function and how many / time period
 # 100/s equates to 100 per second max
 # 10/m equates to 10 per minute or 1 every 6 seconds max
 # 60/h equates to 60 per hour or one per minute max
 DISCORD_BOT_TASK_RATE_LIMITS = {
         "send_channel_message_by_discord_id": "100/s",
         "send_direct_message_by_discord_id": "1/s",
         "send_direct_message_by_user_id": "1/s"
         }
 ```
 
 ## Reaction Roles
+>
 > ❗❗❗ **This will bypass the Group Leadership/Join Request System**: This is intended for open groups but not limited to it! ❗❗❗
 
 The bot is able to run a reaction roles system that is compatible with auth and public users on a discord.
- - If a member is part of auth it will do auth syncing of roles
- - If a member is not found in auth and the reaction role message has the public flag set it will assign roles to anyone who reacts
 
-### How To Reaction Role!
+* If a member is part of auth it will do auth syncing of roles
+* If a member is not found in auth and the reaction role message has the public flag set it will assign roles to anyone who reacts
+
+### How To Reaction Role
+
  1. Setup the inital Message you wish to use buy using the command `!rr`
-   - *Optional* Edit the name and settings of this message in `Admin > Discord Bot > Reaction Role Messages`
+
+    * _Optional_ Edit the name and settings of this message in `Admin > Discord Bot > Reaction Role Messages`
+
  2. React to the message with the reactions you wish to use.
  3. The bot will counter react to the reactions when it creates the binding in auth.
  4. Goto `Admin > Discord Bot > Reaction Role Bindings`
  5. Assign the groups you want for each reaction
 
 #### Messages Admin
+
 ![https://cdn.discordapp.com/attachments/639369068930924546/936082605156237332/unknown.png](https://cdn.discordapp.com/attachments/639369068930924546/936082605156237332/unknown.png)
+
 #### Reactions Admin
+
 ![https://cdn.discordapp.com/attachments/639369068930924546/936084126379962378/unknown.png](https://cdn.discordapp.com/attachments/639369068930924546/936084126379962378/unknown.png)
 
 ## Integrations
+
 * [Statistics](https://github.com/pvyParts/aa-statistics)
   * Adds zkill Monthly/Yearly stats to !lookup
 * [timezones](https://github.com/ppfeufer/aa-timezones)
   * Updates the `time` command to have all timezones configured in auth.
 
 ## Welcome Messaages
+
 `
 With the WelcomeGoodbye Cog activated, Discordbot will grab a random message from the Welcome or Goodbye Message Model and send it to the Guild System channel
 
 These can be configured in admin under `/admin/aadiscordbot/welcomemessage/` and `/admin/aadiscordbot/goodbyemessage/`
 
 The messages support some string formatting
 
 * `{user_mention} - A Discord @ Mention
 * `{guild_name} - The name of the Discord Server
 * `{auth_url} - A link to Auth
-```
+
+```text
 Welcome {user_mention} to {guild_name}, I hope you enjoy your stay.
 
 You can Authenticate for more access {auth_url}
 ```
 
 ## Private Thread Ticket System
 
@@ -255,31 +322,34 @@
 
 With the `aadiscordbot.cogs.tickets` Cog activated, users wll be able to issue the `/help` command to pick a group to get help from.
 
 The groups available for selection are configurable in the site admin under
 `Discord Bot > Ticket Cog Configuration`
 
 You also need to choose a channel to create the threads in from the site admin `Discord Bot > Ticket Cog Configuration`:
-  - Anyone who can use the `/help` command must have View and Send Message permissions on this channel otherwise they will not be able to see the tickets authbot creates for them
-  - Authbot must have the permissions to create private threads in this channel
-  - Authbot must have the permissions to send messages to this channel
 
+* Anyone who can use the `/help` command must have View and Send Message permissions on this channel otherwise they will not be able to see the tickets authbot creates for them
+* Authbot must have the permissions to create private threads in this channel
+* Authbot must have the permissions to send messages to this channel
 
 ## Using AA-Discordbot from my project
 
 ### Send Messages
+
 You can use the send_message helper to send a message with text/embed to:
-  - Discord user_id
-  - Discord channel_id
-  - Auth User Model Object
-  - Auth user_pk
+
+* Discord user_id
+* Discord channel_id
+* Auth User Model Object
+* Auth user_pk
 
 [aadiscordbot/tasks.py](https://github.com/pvyParts/allianceauth-discordbot/blob/master/aadiscordbot/tasks.py)
 
 ### Example Usage
+
 ```python
 from django.contrib.auth.models import User
 from django.apps import apps
 
 ## Use a small helper to check if AA-Discordbot is installs
 def discord_bot_active():
     return apps.is_installed('aadiscordbot')
@@ -348,40 +418,45 @@
                 message=msg,
                 embed=e)
 ```
 
 ### Registering 3rd Party Cogs (Handling Commands)
 
 In `auth_hooks.py`, define a function that returns an array of cog modules, and register it as a `discord_cogs_hook`:
+
 ```python
 @hooks.register('discord_cogs_hook')
 def register_cogs():
     return ["yourapp.cogs.cog_a", "yourapp.cogs.cog_b"]
 ```
 
-## Optional Settings
+## Optional Settings continued
+
 ### Isolate AuthBot from Auth's Discord Service
+
 ```python
 AUTHBOT_DISCORD_APP_ID = 'App ID for dedicated bot'
 AUTHBOT_DISCORD_BOT_TOKEN = 'Token for dedicated bot'
 ```
 
 ## Issues
 
 Please remember to report any aa-discordbot related issues using the issues on **this** repository.
 
 ## Troubleshooting
 
 ### Py-Cord and discord.py fighting in venv
+
 **Problem:**
 
 Something has gone funny with my venv after i installed another app that wanted `discord.py`
 
 **Reason:**
 
 This is due to the Py-cord lib sharing the `discord` namespace. Py-Cord is however a drop in replacement. So no issues should arise from using it over the now legacy discord.py lib. **YMMV**
 
 **Fix:**
+
  1. Uninstall `discord.py` by running `pip uninstall discord.py` with your venv active.
  2. Reinstall `py-cord` by running `pip install -U py-cord==2.0.0b3` with your venv active.
  3. Approach the dev from the app that overrode your py-cord to update to a maintained lib.
```

