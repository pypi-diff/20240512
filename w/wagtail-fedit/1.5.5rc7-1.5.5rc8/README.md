# Comparing `tmp/wagtail_fedit-1.5.5rc7.tar.gz` & `tmp/wagtail_fedit-1.5.5rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.5rc7.tar", last modified: Fri May 10 13:02:03 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.5rc8.tar", last modified: Fri May 10 17:00:45 2024, max compression
```

## Comparing `wagtail_fedit-1.5.5rc7.tar` & `wagtail_fedit-1.5.5rc8.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.461602 wagtail_fedit-1.5.5rc7/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/MANIFEST.in
--rw-rw-rw-   0        0        0     3013 2024-05-10 13:02:03.462604 wagtail_fedit-1.5.5rc7/PKG-INFO
--rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.5rc7/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-05-10 13:02:03.463603 wagtail_fedit-1.5.5rc7/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.341659 wagtail_fedit-1.5.5rc7/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.362425 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    14469 2024-04-25 18:57:33.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     6545 2024-04-25 18:29:05.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/apps.py
--rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.368428 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.316636 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.316636 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.371240 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.371240 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.372248 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.319127 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.320129 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.375889 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5745 2024-05-08 11:26:45.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.377068 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    51061 2024-05-08 13:42:06.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/edit.js
--rw-rw-rw-   0        0        0    26914 2024-05-07 17:43:52.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.378075 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/licenses/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.321128 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.380070 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.381069 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.384942 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      571 2024-05-08 11:29:32.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.397329 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.404320 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.407347 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.408540 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.410532 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.412534 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    13140 2024-05-08 09:22:37.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    10310 2024-05-07 21:59:17.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.415532 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.421320 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.424174 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.439129 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.444444 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    18101 2024-04-25 13:15:30.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.450602 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8490 2024-04-25 13:06:47.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.460610 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1832 2024-05-10 12:39:02.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:02:03.348335 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     3013 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4466 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 13:02:03.000000 wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.386934 wagtail_fedit-1.5.5rc8/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3013 2024-05-10 17:00:45.386934 wagtail_fedit-1.5.5rc8/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-28 14:18:11.000000 wagtail_fedit-1.5.5rc8/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-05-10 17:00:45.388934 wagtail_fedit-1.5.5rc8/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.276858 wagtail_fedit-1.5.5rc8/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.295900 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      532 2024-04-22 21:01:35.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    14469 2024-04-25 18:57:33.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     6545 2024-04-25 18:29:05.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     8652 2024-04-23 18:12:26.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     5607 2024-05-07 18:13:59.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0     1595 2024-04-18 20:22:37.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/apps.py
+-rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.298896 wagtail_fedit-1.5.5rc8/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     4617 2024-04-21 02:08:33.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.243802 wagtail_fedit-1.5.5rc8/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.244808 wagtail_fedit-1.5.5rc8/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.301145 wagtail_fedit-1.5.5rc8/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7262 2024-04-23 15:50:58.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    15296 2024-04-25 14:19:13.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.302150 wagtail_fedit-1.5.5rc8/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.303151 wagtail_fedit-1.5.5rc8/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.246808 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.247648 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.308152 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5745 2024-05-08 11:26:45.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5098 2024-04-17 20:40:49.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.310151 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    53927 2024-05-10 17:00:41.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/edit.js
+-rw-rw-rw-   0        0        0    26914 2024-05-07 17:43:52.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.311640 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/licenses/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.248653 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.312646 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.313646 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.315646 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      571 2024-05-08 11:29:32.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.327161 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      555 2024-04-21 21:13:45.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      330 2024-04-21 00:12:14.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5271 2024-04-21 00:11:24.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.332286 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.334285 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.336291 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.338287 wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.341804 wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13140 2024-05-08 09:22:37.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10310 2024-05-07 21:59:17.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.344307 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.349815 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.353836 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.365883 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    28117 2024-04-25 18:07:06.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.372379 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3625 2024-04-15 20:14:41.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1196 2024-04-23 17:25:08.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    18101 2024-04-25 13:15:30.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.377416 wagtail_fedit-1.5.5rc8/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8490 2024-04-25 13:06:47.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17778 2024-04-25 09:19:32.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.385935 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      184 2024-04-16 10:03:02.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1832 2024-05-10 12:39:02.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0      328 2024-04-21 16:44:33.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     3100 2024-05-07 18:11:10.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:00:45.283373 wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     3013 2024-05-10 17:00:45.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4466 2024-05-10 17:00:45.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 17:00:45.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-10 17:00:45.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 17:00:45.000000 wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.5rc7/LICENSE` & `wagtail_fedit-1.5.5rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/PKG-INFO` & `wagtail_fedit-1.5.5rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.5rc7
+Version: 1.5.5rc8
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.5rc7/README.md` & `wagtail_fedit-1.5.5rc8/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/setup.cfg` & `wagtail_fedit-1.5.5rc8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3572 6337 0d0a 6465 7363 7269 7074 696f  5rc7..descriptio
+00000030: 3572 6338 0d0a 6465 7363 7269 7074 696f  5rc8..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/__init__.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/errors.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/errors.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/models.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/edit.js` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/edit.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,20 @@
 (() => {
     "use strict";
     var t = {
             2: (t, e, n) => {
+                n.d(e, {
+                    A: () => s
+                });
                 var i = n(601),
                     r = n.n(i),
-                    o = n(314);
-                n.n(o)()(r()).push([t.id, '.tippy-box[data-animation=fade][data-state=hidden]{opacity:0}[data-tippy-root]{max-width:calc(100vw - 10px)}.tippy-box{position:relative;background-color:#333;color:#fff;border-radius:4px;font-size:14px;line-height:1.4;white-space:normal;outline:0;transition-property:transform,visibility,opacity}.tippy-box[data-placement^=top]>.tippy-arrow{bottom:0}.tippy-box[data-placement^=top]>.tippy-arrow:before{bottom:-7px;left:0;border-width:8px 8px 0;border-top-color:initial;transform-origin:center top}.tippy-box[data-placement^=bottom]>.tippy-arrow{top:0}.tippy-box[data-placement^=bottom]>.tippy-arrow:before{top:-7px;left:0;border-width:0 8px 8px;border-bottom-color:initial;transform-origin:center bottom}.tippy-box[data-placement^=left]>.tippy-arrow{right:0}.tippy-box[data-placement^=left]>.tippy-arrow:before{border-width:8px 0 8px 8px;border-left-color:initial;right:-7px;transform-origin:center left}.tippy-box[data-placement^=right]>.tippy-arrow{left:0}.tippy-box[data-placement^=right]>.tippy-arrow:before{left:-7px;border-width:8px 8px 8px 0;border-right-color:initial;transform-origin:center right}.tippy-box[data-inertia][data-state=visible]{transition-timing-function:cubic-bezier(.54,1.5,.38,1.11)}.tippy-arrow{width:16px;height:16px;color:#333}.tippy-arrow:before{content:"";position:absolute;border-color:transparent;border-style:solid}.tippy-content{position:relative;padding:5px 9px;z-index:1}', ""])
+                    o = n(314),
+                    a = n.n(o)()(r());
+                a.push([t.id, '.tippy-box[data-animation=fade][data-state=hidden]{opacity:0}[data-tippy-root]{max-width:calc(100vw - 10px)}.tippy-box{position:relative;background-color:#333;color:#fff;border-radius:4px;font-size:14px;line-height:1.4;white-space:normal;outline:0;transition-property:transform,visibility,opacity}.tippy-box[data-placement^=top]>.tippy-arrow{bottom:0}.tippy-box[data-placement^=top]>.tippy-arrow:before{bottom:-7px;left:0;border-width:8px 8px 0;border-top-color:initial;transform-origin:center top}.tippy-box[data-placement^=bottom]>.tippy-arrow{top:0}.tippy-box[data-placement^=bottom]>.tippy-arrow:before{top:-7px;left:0;border-width:0 8px 8px;border-bottom-color:initial;transform-origin:center bottom}.tippy-box[data-placement^=left]>.tippy-arrow{right:0}.tippy-box[data-placement^=left]>.tippy-arrow:before{border-width:8px 0 8px 8px;border-left-color:initial;right:-7px;transform-origin:center left}.tippy-box[data-placement^=right]>.tippy-arrow{left:0}.tippy-box[data-placement^=right]>.tippy-arrow:before{left:-7px;border-width:8px 8px 8px 0;border-right-color:initial;transform-origin:center right}.tippy-box[data-inertia][data-state=visible]{transition-timing-function:cubic-bezier(.54,1.5,.38,1.11)}.tippy-arrow{width:16px;height:16px;color:#333}.tippy-arrow:before{content:"";position:absolute;border-color:transparent;border-style:solid}.tippy-content{position:relative;padding:5px 9px;z-index:1}', ""]);
+                const s = a
             },
             314: t => {
                 t.exports = function(t) {
                     var e = [];
                     return e.toString = function() {
                         return this.map((function(e) {
                             var n = "",
@@ -33,14 +38,147 @@
                     }, e
                 }
             },
             601: t => {
                 t.exports = function(t) {
                     return t[1]
                 }
+            },
+            72: t => {
+                var e = [];
+
+                function n(t) {
+                    for (var n = -1, i = 0; i < e.length; i++)
+                        if (e[i].identifier === t) {
+                            n = i;
+                            break
+                        } return n
+                }
+
+                function i(t, i) {
+                    for (var o = {}, a = [], s = 0; s < t.length; s++) {
+                        var c = t[s],
+                            l = i.base ? c[0] + i.base : c[0],
+                            d = o[l] || 0,
+                            p = "".concat(l, " ").concat(d);
+                        o[l] = d + 1;
+                        var u = n(p),
+                            f = {
+                                css: c[1],
+                                media: c[2],
+                                sourceMap: c[3],
+                                supports: c[4],
+                                layer: c[5]
+                            };
+                        if (-1 !== u) e[u].references++, e[u].updater(f);
+                        else {
+                            var h = r(f, i);
+                            i.byIndex = s, e.splice(s, 0, {
+                                identifier: p,
+                                updater: h,
+                                references: 1
+                            })
+                        }
+                        a.push(p)
+                    }
+                    return a
+                }
+
+                function r(t, e) {
+                    var n = e.domAPI(e);
+                    return n.update(t),
+                        function(e) {
+                            if (e) {
+                                if (e.css === t.css && e.media === t.media && e.sourceMap === t.sourceMap && e.supports === t.supports && e.layer === t.layer) return;
+                                n.update(t = e)
+                            } else n.remove()
+                        }
+                }
+                t.exports = function(t, r) {
+                    var o = i(t = t || [], r = r || {});
+                    return function(t) {
+                        t = t || [];
+                        for (var a = 0; a < o.length; a++) {
+                            var s = n(o[a]);
+                            e[s].references--
+                        }
+                        for (var c = i(t, r), l = 0; l < o.length; l++) {
+                            var d = n(o[l]);
+                            0 === e[d].references && (e[d].updater(), e.splice(d, 1))
+                        }
+                        o = c
+                    }
+                }
+            },
+            659: t => {
+                var e = {};
+                t.exports = function(t, n) {
+                    var i = function(t) {
+                        if (void 0 === e[t]) {
+                            var n = document.querySelector(t);
+                            if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                                n = n.contentDocument.head
+                            } catch (t) {
+                                n = null
+                            }
+                            e[t] = n
+                        }
+                        return e[t]
+                    }(t);
+                    if (!i) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                    i.appendChild(n)
+                }
+            },
+            540: t => {
+                t.exports = function(t) {
+                    var e = document.createElement("style");
+                    return t.setAttributes(e, t.attributes), t.insert(e, t.options), e
+                }
+            },
+            56: (t, e, n) => {
+                t.exports = function(t) {
+                    var e = n.nc;
+                    e && t.setAttribute("nonce", e)
+                }
+            },
+            825: t => {
+                t.exports = function(t) {
+                    if ("undefined" == typeof document) return {
+                        update: function() {},
+                        remove: function() {}
+                    };
+                    var e = t.insertStyleElement(t);
+                    return {
+                        update: function(n) {
+                            ! function(t, e, n) {
+                                var i = "";
+                                n.supports && (i += "@supports (".concat(n.supports, ") {")), n.media && (i += "@media ".concat(n.media, " {"));
+                                var r = void 0 !== n.layer;
+                                r && (i += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), i += n.css, r && (i += "}"), n.media && (i += "}"), n.supports && (i += "}");
+                                var o = n.sourceMap;
+                                o && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), e.styleTagTransform(i, t, e.options)
+                            }(e, t, n)
+                        },
+                        remove: function() {
+                            ! function(t) {
+                                if (null === t.parentNode) return !1;
+                                t.parentNode.removeChild(t)
+                            }(e)
+                        }
+                    }
+                }
+            },
+            113: t => {
+                t.exports = function(t, e) {
+                    if (e.styleSheet) e.styleSheet.cssText = t;
+                    else {
+                        for (; e.firstChild;) e.removeChild(e.firstChild);
+                        e.appendChild(document.createTextNode(t))
+                    }
+                }
             }
         },
         e = {};
 
     function n(i) {
         var r = e[i];
         if (void 0 !== r) return r.exports;
@@ -56,15 +194,15 @@
             a: e
         }), e
     }, n.d = (t, e) => {
         for (var i in e) n.o(e, i) && !n.o(t, i) && Object.defineProperty(t, i, {
             enumerable: !0,
             get: e[i]
         })
-    }, n.o = (t, e) => Object.prototype.hasOwnProperty.call(t, e), (() => {
+    }, n.o = (t, e) => Object.prototype.hasOwnProperty.call(t, e), n.nc = void 0, (() => {
         function t(t) {
             if (null == t) return window;
             if ("[object Window]" !== t.toString()) {
                 var e = t.ownerDocument;
                 return e && e.defaultView || window
             }
             return t
@@ -241,21 +379,21 @@
             M = "left",
             S = "auto",
             D = [A, T, C, M],
             k = "start",
             j = "end",
             P = "viewport",
             N = "popper",
-            W = D.reduce((function(t, e) {
+            H = D.reduce((function(t, e) {
                 return t.concat([e + "-" + k, e + "-" + j])
             }), []),
-            H = [].concat(D, [S]).reduce((function(t, e) {
+            R = [].concat(D, [S]).reduce((function(t, e) {
                 return t.concat([e, e + "-" + k, e + "-" + j])
             }), []),
-            R = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
+            W = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
 
         function B(t) {
             var e = new Map,
                 n = new Set,
                 i = [];
 
             function r(t) {
@@ -268,40 +406,40 @@
             }
             return t.forEach((function(t) {
                 e.set(t.name, t)
             })), t.forEach((function(t) {
                 n.has(t.name) || r(t)
             })), i
         }
-        var _ = {
+        var I = {
             placement: "bottom",
             modifiers: [],
             strategy: "absolute"
         };
 
-        function F() {
+        function _() {
             for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
             return !e.some((function(t) {
                 return !(t && "function" == typeof t.getBoundingClientRect)
             }))
         }
 
-        function V(t) {
+        function F(t) {
             void 0 === t && (t = {});
             var n = t,
                 i = n.defaultModifiers,
                 r = void 0 === i ? [] : i,
                 o = n.defaultOptions,
-                a = void 0 === o ? _ : o;
+                a = void 0 === o ? I : o;
             return function(t, n, i) {
                 void 0 === i && (i = a);
                 var o, s, c = {
                         placement: "bottom",
                         orderedModifiers: [],
-                        options: Object.assign({}, _, a),
+                        options: Object.assign({}, I, a),
                         modifiersData: {},
                         elements: {
                             reference: t,
                             popper: n
                         },
                         attributes: {},
                         styles: {}
@@ -314,15 +452,15 @@
                             var o = "function" == typeof i ? i(c.options) : i;
                             u(), c.options = Object.assign({}, a, c.options, o), c.scrollParents = {
                                 reference: e(t) ? x(t) : t.contextElement ? x(t.contextElement) : [],
                                 popper: x(n)
                             };
                             var s, d, f = function(t) {
                                 var e = B(t);
-                                return R.reduce((function(t, n) {
+                                return W.reduce((function(t, n) {
                                     return t.concat(e.filter((function(t) {
                                         return t.phase === n
                                     })))
                                 }), [])
                             }((s = [].concat(r, c.options.modifiers), d = s.reduce((function(t, e) {
                                 var n = t[e.name];
                                 return t[e.name] = n ? Object.assign({}, n, e, {
@@ -351,15 +489,15 @@
                             })), p.update()
                         },
                         forceUpdate: function() {
                             if (!d) {
                                 var t = c.elements,
                                     e = t.reference,
                                     n = t.popper;
-                                if (F(e, n)) {
+                                if (_(e, n)) {
                                     c.rects = {
                                         reference: g(e, L(n), "fixed" === c.options.strategy),
                                         popper: w(n)
                                     }, c.reset = !1, c.placement = c.options.placement, c.orderedModifiers.forEach((function(t) {
                                         return c.modifiersData[t.name] = Object.assign({}, t.data)
                                     }));
                                     for (var i = 0; i < c.orderedModifiers.length; i++)
@@ -390,48 +528,74 @@
                                 }))
                             }))), s
                         }),
                         destroy: function() {
                             u(), d = !0
                         }
                     };
-                if (!F(t, n)) return p;
+                if (!_(t, n)) return p;
 
                 function u() {
                     l.forEach((function(t) {
                         return t()
                     })), l = []
                 }
                 return p.setOptions(i).then((function(t) {
                     !d && i.onFirstUpdate && i.onFirstUpdate(t)
                 })), p
             }
         }
         var q = {
             passive: !0
         };
+        const V = {
+            name: "eventListeners",
+            enabled: !0,
+            phase: "write",
+            fn: function() {},
+            effect: function(e) {
+                var n = e.state,
+                    i = e.instance,
+                    r = e.options,
+                    o = r.scroll,
+                    a = void 0 === o || o,
+                    s = r.resize,
+                    c = void 0 === s || s,
+                    l = t(n.elements.popper),
+                    d = [].concat(n.scrollParents.reference, n.scrollParents.popper);
+                return a && d.forEach((function(t) {
+                        t.addEventListener("scroll", i.update, q)
+                    })), c && l.addEventListener("resize", i.update, q),
+                    function() {
+                        a && d.forEach((function(t) {
+                            t.removeEventListener("scroll", i.update, q)
+                        })), c && l.removeEventListener("resize", i.update, q)
+                    }
+            },
+            data: {}
+        };
 
-        function I(t) {
+        function U(t) {
             return t.split("-")[0]
         }
 
-        function U(t) {
+        function $(t) {
             return t.split("-")[1]
         }
 
-        function $(t) {
+        function z(t) {
             return ["top", "bottom"].indexOf(t) >= 0 ? "x" : "y"
         }
 
-        function z(t) {
+        function X(t) {
             var e, n = t.reference,
                 i = t.element,
                 r = t.placement,
-                o = r ? I(r) : null,
-                a = r ? U(r) : null,
+                o = r ? U(r) : null,
+                a = r ? $(r) : null,
                 s = n.x + n.width / 2 - i.width / 2,
                 c = n.y + n.height / 2 - i.height / 2;
             switch (o) {
                 case A:
                     e = {
                         x: s,
                         y: n.y - i.height
@@ -457,35 +621,35 @@
                     break;
                 default:
                     e = {
                         x: n.x,
                         y: n.y
                     }
             }
-            var l = o ? $(o) : null;
+            var l = o ? z(o) : null;
             if (null != l) {
                 var d = "y" === l ? "height" : "width";
                 switch (a) {
                     case k:
                         e[l] = e[l] - (n[d] / 2 - i[d] / 2);
                         break;
                     case j:
                         e[l] = e[l] + (n[d] / 2 - i[d] / 2)
                 }
             }
             return e
         }
-        var X = {
+        var Y = {
             top: "auto",
             right: "auto",
             bottom: "auto",
             left: "auto"
         };
 
-        function Y(e) {
+        function G(e) {
             var n, i = e.popper,
                 r = e.popperRect,
                 o = e.placement,
                 a = e.variation,
                 c = e.offsets,
                 l = e.position,
                 d = e.gpuAcceleration,
@@ -511,127 +675,199 @@
                 D = window;
             if (p) {
                 var k = L(i),
                     P = "clientHeight",
                     N = "clientWidth";
                 k === t(i) && "static" !== m(k = f(i)).position && "absolute" === l && (P = "scrollHeight", N = "scrollWidth"), (o === A || (o === M || o === C) && a === j) && (S = T, y -= (h && k === D && D.visualViewport ? D.visualViewport.height : k[P]) - r.height, y *= d ? 1 : -1), o !== M && (o !== A && o !== T || a !== j) || (O = C, g -= (h && k === D && D.visualViewport ? D.visualViewport.width : k[N]) - r.width, g *= d ? 1 : -1)
             }
-            var W, H = Object.assign({
+            var H, R = Object.assign({
                     position: l
-                }, p && X),
-                R = !0 === u ? function(t, e) {
+                }, p && Y),
+                W = !0 === u ? function(t, e) {
                     var n = t.x,
                         i = t.y,
                         r = e.devicePixelRatio || 1;
                     return {
                         x: s(n * r) / r || 0,
                         y: s(i * r) / r || 0
                     }
                 }({
                     x: g,
                     y
                 }, t(i)) : {
                     x: g,
                     y
                 };
-            return g = R.x, y = R.y, d ? Object.assign({}, H, ((W = {})[S] = E ? "0" : "", W[O] = x ? "0" : "", W.transform = (D.devicePixelRatio || 1) <= 1 ? "translate(" + g + "px, " + y + "px)" : "translate3d(" + g + "px, " + y + "px, 0)", W)) : Object.assign({}, H, ((n = {})[S] = E ? y + "px" : "", n[O] = x ? g + "px" : "", n.transform = "", n))
+            return g = W.x, y = W.y, d ? Object.assign({}, R, ((H = {})[S] = E ? "0" : "", H[O] = x ? "0" : "", H.transform = (D.devicePixelRatio || 1) <= 1 ? "translate(" + g + "px, " + y + "px)" : "translate3d(" + g + "px, " + y + "px, 0)", H)) : Object.assign({}, R, ((n = {})[S] = E ? y + "px" : "", n[O] = x ? g + "px" : "", n.transform = "", n))
         }
-        const G = {
-            name: "applyStyles",
-            enabled: !0,
-            phase: "write",
-            fn: function(t) {
-                var e = t.state;
-                Object.keys(e.elements).forEach((function(t) {
-                    var n = e.styles[t] || {},
-                        r = e.attributes[t] || {},
-                        o = e.elements[t];
-                    i(o) && u(o) && (Object.assign(o.style, n), Object.keys(r).forEach((function(t) {
-                        var e = r[t];
-                        !1 === e ? o.removeAttribute(t) : o.setAttribute(t, !0 === e ? "" : e)
-                    })))
-                }))
+        const J = {
+                name: "computeStyles",
+                enabled: !0,
+                phase: "beforeWrite",
+                fn: function(t) {
+                    var e = t.state,
+                        n = t.options,
+                        i = n.gpuAcceleration,
+                        r = void 0 === i || i,
+                        o = n.adaptive,
+                        a = void 0 === o || o,
+                        s = n.roundOffsets,
+                        c = void 0 === s || s,
+                        l = {
+                            placement: U(e.placement),
+                            variation: $(e.placement),
+                            popper: e.elements.popper,
+                            popperRect: e.rects.popper,
+                            gpuAcceleration: r,
+                            isFixed: "fixed" === e.options.strategy
+                        };
+                    null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, G(Object.assign({}, l, {
+                        offsets: e.modifiersData.popperOffsets,
+                        position: e.options.strategy,
+                        adaptive: a,
+                        roundOffsets: c
+                    })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, G(Object.assign({}, l, {
+                        offsets: e.modifiersData.arrow,
+                        position: "absolute",
+                        adaptive: !1,
+                        roundOffsets: c
+                    })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
+                        "data-popper-placement": e.placement
+                    })
+                },
+                data: {}
             },
-            effect: function(t) {
-                var e = t.state,
-                    n = {
-                        popper: {
-                            position: e.options.strategy,
-                            left: "0",
-                            top: "0",
-                            margin: "0"
-                        },
-                        arrow: {
-                            position: "absolute"
-                        },
-                        reference: {}
-                    };
-                return Object.assign(e.elements.popper.style, n.popper), e.styles = n, e.elements.arrow && Object.assign(e.elements.arrow.style, n.arrow),
-                    function() {
-                        Object.keys(e.elements).forEach((function(t) {
-                            var r = e.elements[t],
-                                o = e.attributes[t] || {},
-                                a = Object.keys(e.styles.hasOwnProperty(t) ? e.styles[t] : n[t]).reduce((function(t, e) {
-                                    return t[e] = "", t
-                                }), {});
-                            i(r) && u(r) && (Object.assign(r.style, a), Object.keys(o).forEach((function(t) {
-                                r.removeAttribute(t)
-                            })))
-                        }))
-                    }
+            K = {
+                name: "applyStyles",
+                enabled: !0,
+                phase: "write",
+                fn: function(t) {
+                    var e = t.state;
+                    Object.keys(e.elements).forEach((function(t) {
+                        var n = e.styles[t] || {},
+                            r = e.attributes[t] || {},
+                            o = e.elements[t];
+                        i(o) && u(o) && (Object.assign(o.style, n), Object.keys(r).forEach((function(t) {
+                            var e = r[t];
+                            !1 === e ? o.removeAttribute(t) : o.setAttribute(t, !0 === e ? "" : e)
+                        })))
+                    }))
+                },
+                effect: function(t) {
+                    var e = t.state,
+                        n = {
+                            popper: {
+                                position: e.options.strategy,
+                                left: "0",
+                                top: "0",
+                                margin: "0"
+                            },
+                            arrow: {
+                                position: "absolute"
+                            },
+                            reference: {}
+                        };
+                    return Object.assign(e.elements.popper.style, n.popper), e.styles = n, e.elements.arrow && Object.assign(e.elements.arrow.style, n.arrow),
+                        function() {
+                            Object.keys(e.elements).forEach((function(t) {
+                                var r = e.elements[t],
+                                    o = e.attributes[t] || {},
+                                    a = Object.keys(e.styles.hasOwnProperty(t) ? e.styles[t] : n[t]).reduce((function(t, e) {
+                                        return t[e] = "", t
+                                    }), {});
+                                i(r) && u(r) && (Object.assign(r.style, a), Object.keys(o).forEach((function(t) {
+                                    r.removeAttribute(t)
+                                })))
+                            }))
+                        }
+                },
+                requires: ["computeStyles"]
             },
-            requires: ["computeStyles"]
-        };
-        var J = {
+            Q = {
+                name: "offset",
+                enabled: !0,
+                phase: "main",
+                requires: ["popperOffsets"],
+                fn: function(t) {
+                    var e = t.state,
+                        n = t.options,
+                        i = t.name,
+                        r = n.offset,
+                        o = void 0 === r ? [0, 0] : r,
+                        a = R.reduce((function(t, n) {
+                            return t[n] = function(t, e, n) {
+                                var i = U(t),
+                                    r = [M, A].indexOf(i) >= 0 ? -1 : 1,
+                                    o = "function" == typeof n ? n(Object.assign({}, e, {
+                                        placement: t
+                                    })) : n,
+                                    a = o[0],
+                                    s = o[1];
+                                return a = a || 0, s = (s || 0) * r, [M, C].indexOf(i) >= 0 ? {
+                                    x: s,
+                                    y: a
+                                } : {
+                                    x: a,
+                                    y: s
+                                }
+                            }(n, e.rects, o), t
+                        }), {}),
+                        s = a[e.placement],
+                        c = s.x,
+                        l = s.y;
+                    null != e.modifiersData.popperOffsets && (e.modifiersData.popperOffsets.x += c, e.modifiersData.popperOffsets.y += l), e.modifiersData[i] = a
+                }
+            };
+        var Z = {
             left: "right",
             right: "left",
             bottom: "top",
             top: "bottom"
         };
 
-        function K(t) {
+        function tt(t) {
             return t.replace(/left|right|bottom|top/g, (function(t) {
-                return J[t]
+                return Z[t]
             }))
         }
-        var Q = {
+        var et = {
             start: "end",
             end: "start"
         };
 
-        function Z(t) {
+        function nt(t) {
             return t.replace(/start|end/g, (function(t) {
-                return Q[t]
+                return et[t]
             }))
         }
 
-        function tt(t, e) {
+        function it(t, e) {
             var n = e.getRootNode && e.getRootNode();
             if (t.contains(e)) return !0;
             if (n && r(n)) {
                 var i = e;
                 do {
                     if (i && t.isSameNode(i)) return !0;
                     i = i.parentNode || i.host
                 } while (i)
             }
             return !1
         }
 
-        function et(t) {
+        function rt(t) {
             return Object.assign({}, t, {
                 left: t.x,
                 top: t.y,
                 right: t.x + t.width,
                 bottom: t.y + t.height
             })
         }
 
-        function nt(n, i, r) {
-            return i === P ? et(function(e, n) {
+        function ot(n, i, r) {
+            return i === P ? rt(function(e, n) {
                 var i = t(e),
                     r = f(e),
                     o = i.visualViewport,
                     a = r.clientWidth,
                     s = r.clientHeight,
                     c = 0,
                     d = 0;
@@ -645,15 +881,15 @@
                     height: s,
                     x: c + h(e),
                     y: d
                 }
             }(n, r)) : e(i) ? function(t, e) {
                 var n = d(t, !1, "fixed" === e);
                 return n.top = n.top + t.clientTop, n.left = n.left + t.clientLeft, n.bottom = n.top + t.clientHeight, n.right = n.left + t.clientWidth, n.width = t.clientWidth, n.height = t.clientHeight, n.x = n.left, n.y = n.top, n
-            }(i, r) : et(function(t) {
+            }(i, r) : rt(function(t) {
                 var e, n = f(t),
                     i = p(t),
                     r = null == (e = t.ownerDocument) ? void 0 : e.body,
                     a = o(n.scrollWidth, n.clientWidth, r ? r.scrollWidth : 0, r ? r.clientWidth : 0),
                     s = o(n.scrollHeight, n.clientHeight, r ? r.scrollHeight : 0, r ? r.clientHeight : 0),
                     c = -i.scrollLeft + h(t),
                     l = -i.scrollTop;
@@ -662,30 +898,30 @@
                     height: s,
                     x: c,
                     y: l
                 }
             }(f(n)))
         }
 
-        function it(t) {
+        function at(t) {
             return Object.assign({}, {
                 top: 0,
                 right: 0,
                 bottom: 0,
                 left: 0
             }, t)
         }
 
-        function rt(t, e) {
+        function st(t, e) {
             return e.reduce((function(e, n) {
                 return e[n] = t, e
             }), {})
         }
 
-        function ot(t, n) {
+        function ct(t, n) {
             void 0 === n && (n = {});
             var r = n,
                 s = r.placement,
                 c = void 0 === s ? t.placement : s,
                 l = r.strategy,
                 p = void 0 === l ? t.strategy : l,
                 h = r.boundary,
@@ -694,583 +930,491 @@
                 w = void 0 === g ? P : g,
                 b = r.elementContext,
                 E = void 0 === b ? N : b,
                 O = r.altBoundary,
                 M = void 0 !== O && O,
                 S = r.padding,
                 k = void 0 === S ? 0 : S,
-                j = it("number" != typeof k ? k : rt(k, D)),
-                W = E === N ? "reference" : N,
-                H = t.rects.popper,
-                R = t.elements[M ? W : E],
+                j = at("number" != typeof k ? k : st(k, D)),
+                H = E === N ? "reference" : N,
+                R = t.rects.popper,
+                W = t.elements[M ? H : E],
                 B = function(t, n, r, s) {
                     var c = "clippingParents" === n ? function(t) {
                             var n = x(y(t)),
                                 r = ["absolute", "fixed"].indexOf(m(t).position) >= 0 && i(t) ? L(t) : t;
                             return e(r) ? n.filter((function(t) {
-                                return e(t) && tt(t, r) && "body" !== u(t)
+                                return e(t) && it(t, r) && "body" !== u(t)
                             })) : []
                         }(t) : [].concat(n),
                         l = [].concat(c, [r]),
                         d = l[0],
                         p = l.reduce((function(e, n) {
-                            var i = nt(t, n, s);
+                            var i = ot(t, n, s);
                             return e.top = o(i.top, e.top), e.right = a(i.right, e.right), e.bottom = a(i.bottom, e.bottom), e.left = o(i.left, e.left), e
-                        }), nt(t, d, s));
+                        }), ot(t, d, s));
                     return p.width = p.right - p.left, p.height = p.bottom - p.top, p.x = p.left, p.y = p.top, p
-                }(e(R) ? R : R.contextElement || f(t.elements.popper), v, w, p),
-                _ = d(t.elements.reference),
-                F = z({
-                    reference: _,
-                    element: H,
+                }(e(W) ? W : W.contextElement || f(t.elements.popper), v, w, p),
+                I = d(t.elements.reference),
+                _ = X({
+                    reference: I,
+                    element: R,
                     strategy: "absolute",
                     placement: c
                 }),
-                V = et(Object.assign({}, H, F)),
-                q = E === N ? V : _,
-                I = {
+                F = rt(Object.assign({}, R, _)),
+                q = E === N ? F : I,
+                V = {
                     top: B.top - q.top + j.top,
                     bottom: q.bottom - B.bottom + j.bottom,
                     left: B.left - q.left + j.left,
                     right: q.right - B.right + j.right
                 },
                 U = t.modifiersData.offset;
             if (E === N && U) {
                 var $ = U[c];
-                Object.keys(I).forEach((function(t) {
+                Object.keys(V).forEach((function(t) {
                     var e = [C, T].indexOf(t) >= 0 ? 1 : -1,
                         n = [A, T].indexOf(t) >= 0 ? "y" : "x";
-                    I[t] += $[n] * e
+                    V[t] += $[n] * e
                 }))
             }
-            return I
+            return V
         }
+        const lt = {
+            name: "flip",
+            enabled: !0,
+            phase: "main",
+            fn: function(t) {
+                var e = t.state,
+                    n = t.options,
+                    i = t.name;
+                if (!e.modifiersData[i]._skip) {
+                    for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = e.options.placement, g = U(v), w = c || (g !== v && h ? function(t) {
+                            if (U(t) === S) return [];
+                            var e = tt(t);
+                            return [nt(t), e, nt(e)]
+                        }(v) : [tt(v)]), y = [v].concat(w).reduce((function(t, n) {
+                            return t.concat(U(n) === S ? function(t, e) {
+                                void 0 === e && (e = {});
+                                var n = e,
+                                    i = n.placement,
+                                    r = n.boundary,
+                                    o = n.rootBoundary,
+                                    a = n.padding,
+                                    s = n.flipVariations,
+                                    c = n.allowedAutoPlacements,
+                                    l = void 0 === c ? R : c,
+                                    d = $(i),
+                                    p = d ? s ? H : H.filter((function(t) {
+                                        return $(t) === d
+                                    })) : D,
+                                    u = p.filter((function(t) {
+                                        return l.indexOf(t) >= 0
+                                    }));
+                                0 === u.length && (u = p);
+                                var f = u.reduce((function(e, n) {
+                                    return e[n] = ct(t, {
+                                        placement: n,
+                                        boundary: r,
+                                        rootBoundary: o,
+                                        padding: a
+                                    })[U(n)], e
+                                }), {});
+                                return Object.keys(f).sort((function(t, e) {
+                                    return f[t] - f[e]
+                                }))
+                            }(e, {
+                                placement: n,
+                                boundary: d,
+                                rootBoundary: p,
+                                padding: l,
+                                flipVariations: h,
+                                allowedAutoPlacements: m
+                            }) : n)
+                        }), []), b = e.rects.reference, x = e.rects.popper, E = new Map, O = !0, L = y[0], j = 0; j < y.length; j++) {
+                        var P = y[j],
+                            N = U(P),
+                            W = $(P) === k,
+                            B = [A, T].indexOf(N) >= 0,
+                            I = B ? "width" : "height",
+                            _ = ct(e, {
+                                placement: P,
+                                boundary: d,
+                                rootBoundary: p,
+                                altBoundary: u,
+                                padding: l
+                            }),
+                            F = B ? W ? C : M : W ? T : A;
+                        b[I] > x[I] && (F = tt(F));
+                        var q = tt(F),
+                            V = [];
+                        if (o && V.push(_[N] <= 0), s && V.push(_[F] <= 0, _[q] <= 0), V.every((function(t) {
+                                return t
+                            }))) {
+                            L = P, O = !1;
+                            break
+                        }
+                        E.set(P, V)
+                    }
+                    if (O)
+                        for (var z = function(t) {
+                                var e = y.find((function(e) {
+                                    var n = E.get(e);
+                                    if (n) return n.slice(0, t).every((function(t) {
+                                        return t
+                                    }))
+                                }));
+                                if (e) return L = e, "break"
+                            }, X = h ? 3 : 1; X > 0 && "break" !== z(X); X--);
+                    e.placement !== L && (e.modifiersData[i]._skip = !0, e.placement = L, e.reset = !0)
+                }
+            },
+            requiresIfExists: ["offset"],
+            data: {
+                _skip: !1
+            }
+        };
 
-        function at(t, e, n) {
+        function dt(t, e, n) {
             return o(t, a(e, n))
         }
+        const pt = {
+                name: "preventOverflow",
+                enabled: !0,
+                phase: "main",
+                fn: function(t) {
+                    var e = t.state,
+                        n = t.options,
+                        i = t.name,
+                        r = n.mainAxis,
+                        s = void 0 === r || r,
+                        c = n.altAxis,
+                        l = void 0 !== c && c,
+                        d = n.boundary,
+                        p = n.rootBoundary,
+                        u = n.altBoundary,
+                        f = n.padding,
+                        h = n.tether,
+                        m = void 0 === h || h,
+                        v = n.tetherOffset,
+                        g = void 0 === v ? 0 : v,
+                        y = ct(e, {
+                            boundary: d,
+                            rootBoundary: p,
+                            padding: f,
+                            altBoundary: u
+                        }),
+                        b = U(e.placement),
+                        x = $(e.placement),
+                        E = !x,
+                        O = z(b),
+                        S = "x" === O ? "y" : "x",
+                        D = e.modifiersData.popperOffsets,
+                        j = e.rects.reference,
+                        P = e.rects.popper,
+                        N = "function" == typeof g ? g(Object.assign({}, e.rects, {
+                            placement: e.placement
+                        })) : g,
+                        H = "number" == typeof N ? {
+                            mainAxis: N,
+                            altAxis: N
+                        } : Object.assign({
+                            mainAxis: 0,
+                            altAxis: 0
+                        }, N),
+                        R = e.modifiersData.offset ? e.modifiersData.offset[e.placement] : null,
+                        W = {
+                            x: 0,
+                            y: 0
+                        };
+                    if (D) {
+                        if (s) {
+                            var B, I = "y" === O ? A : M,
+                                _ = "y" === O ? T : C,
+                                F = "y" === O ? "height" : "width",
+                                q = D[O],
+                                V = q + y[I],
+                                X = q - y[_],
+                                Y = m ? -P[F] / 2 : 0,
+                                G = x === k ? j[F] : P[F],
+                                J = x === k ? -P[F] : -j[F],
+                                K = e.elements.arrow,
+                                Q = m && K ? w(K) : {
+                                    width: 0,
+                                    height: 0
+                                },
+                                Z = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : {
+                                    top: 0,
+                                    right: 0,
+                                    bottom: 0,
+                                    left: 0
+                                },
+                                tt = Z[I],
+                                et = Z[_],
+                                nt = dt(0, j[F], Q[F]),
+                                it = E ? j[F] / 2 - Y - nt - tt - H.mainAxis : G - nt - tt - H.mainAxis,
+                                rt = E ? -j[F] / 2 + Y + nt + et + H.mainAxis : J + nt + et + H.mainAxis,
+                                ot = e.elements.arrow && L(e.elements.arrow),
+                                at = ot ? "y" === O ? ot.clientTop || 0 : ot.clientLeft || 0 : 0,
+                                st = null != (B = null == R ? void 0 : R[O]) ? B : 0,
+                                lt = q + rt - st,
+                                pt = dt(m ? a(V, q + it - st - at) : V, q, m ? o(X, lt) : X);
+                            D[O] = pt, W[O] = pt - q
+                        }
+                        if (l) {
+                            var ut, ft = "x" === O ? A : M,
+                                ht = "x" === O ? T : C,
+                                mt = D[S],
+                                vt = "y" === S ? "height" : "width",
+                                gt = mt + y[ft],
+                                wt = mt - y[ht],
+                                yt = -1 !== [A, M].indexOf(b),
+                                bt = null != (ut = null == R ? void 0 : R[S]) ? ut : 0,
+                                xt = yt ? gt : mt - j[vt] - P[vt] - bt + H.altAxis,
+                                Et = yt ? mt + j[vt] + P[vt] - bt - H.altAxis : wt,
+                                Ot = m && yt ? function(t, e, n) {
+                                    var i = dt(t, e, n);
+                                    return i > n ? n : i
+                                }(xt, mt, Et) : dt(m ? xt : gt, mt, m ? Et : wt);
+                            D[S] = Ot, W[S] = Ot - mt
+                        }
+                        e.modifiersData[i] = W
+                    }
+                },
+                requiresIfExists: ["offset"]
+            },
+            ut = {
+                name: "arrow",
+                enabled: !0,
+                phase: "main",
+                fn: function(t) {
+                    var e, n = t.state,
+                        i = t.name,
+                        r = t.options,
+                        o = n.elements.arrow,
+                        a = n.modifiersData.popperOffsets,
+                        s = U(n.placement),
+                        c = z(s),
+                        l = [M, C].indexOf(s) >= 0 ? "height" : "width";
+                    if (o && a) {
+                        var d = function(t, e) {
+                                return at("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
+                                    placement: e.placement
+                                })) : t) ? t : st(t, D))
+                            }(r.padding, n),
+                            p = w(o),
+                            u = "y" === c ? A : M,
+                            f = "y" === c ? T : C,
+                            h = n.rects.reference[l] + n.rects.reference[c] - a[c] - n.rects.popper[l],
+                            m = a[c] - n.rects.reference[c],
+                            v = L(o),
+                            g = v ? "y" === c ? v.clientHeight || 0 : v.clientWidth || 0 : 0,
+                            y = h / 2 - m / 2,
+                            b = d[u],
+                            x = g - p[l] - d[f],
+                            E = g / 2 - p[l] / 2 + y,
+                            O = dt(b, E, x),
+                            S = c;
+                        n.modifiersData[i] = ((e = {})[S] = O, e.centerOffset = O - E, e)
+                    }
+                },
+                effect: function(t) {
+                    var e = t.state,
+                        n = t.options.element,
+                        i = void 0 === n ? "[data-popper-arrow]" : n;
+                    null != i && ("string" != typeof i || (i = e.elements.popper.querySelector(i))) && it(e.elements.popper, i) && (e.elements.arrow = i)
+                },
+                requires: ["popperOffsets"],
+                requiresIfExists: ["preventOverflow"]
+            };
 
-        function st(t, e, n) {
+        function ft(t, e, n) {
             return void 0 === n && (n = {
                 x: 0,
                 y: 0
             }), {
                 top: t.top - e.height - n.y,
                 right: t.right - e.width + n.x,
                 bottom: t.bottom - e.height + n.y,
                 left: t.left - e.width - n.x
             }
         }
 
-        function ct(t) {
+        function ht(t) {
             return [A, C, T, M].some((function(e) {
                 return t[e] >= 0
             }))
         }
-        var lt = V({
-                defaultModifiers: [{
-                    name: "eventListeners",
-                    enabled: !0,
-                    phase: "write",
-                    fn: function() {},
-                    effect: function(e) {
-                        var n = e.state,
-                            i = e.instance,
-                            r = e.options,
-                            o = r.scroll,
-                            a = void 0 === o || o,
-                            s = r.resize,
-                            c = void 0 === s || s,
-                            l = t(n.elements.popper),
-                            d = [].concat(n.scrollParents.reference, n.scrollParents.popper);
-                        return a && d.forEach((function(t) {
-                                t.addEventListener("scroll", i.update, q)
-                            })), c && l.addEventListener("resize", i.update, q),
-                            function() {
-                                a && d.forEach((function(t) {
-                                    t.removeEventListener("scroll", i.update, q)
-                                })), c && l.removeEventListener("resize", i.update, q)
-                            }
-                    },
-                    data: {}
-                }, {
+        var mt = F({
+                defaultModifiers: [V, {
                     name: "popperOffsets",
                     enabled: !0,
                     phase: "read",
                     fn: function(t) {
                         var e = t.state,
                             n = t.name;
-                        e.modifiersData[n] = z({
+                        e.modifiersData[n] = X({
                             reference: e.rects.reference,
                             element: e.rects.popper,
                             strategy: "absolute",
                             placement: e.placement
                         })
                     },
                     data: {}
-                }, {
-                    name: "computeStyles",
-                    enabled: !0,
-                    phase: "beforeWrite",
-                    fn: function(t) {
-                        var e = t.state,
-                            n = t.options,
-                            i = n.gpuAcceleration,
-                            r = void 0 === i || i,
-                            o = n.adaptive,
-                            a = void 0 === o || o,
-                            s = n.roundOffsets,
-                            c = void 0 === s || s,
-                            l = {
-                                placement: I(e.placement),
-                                variation: U(e.placement),
-                                popper: e.elements.popper,
-                                popperRect: e.rects.popper,
-                                gpuAcceleration: r,
-                                isFixed: "fixed" === e.options.strategy
-                            };
-                        null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, Y(Object.assign({}, l, {
-                            offsets: e.modifiersData.popperOffsets,
-                            position: e.options.strategy,
-                            adaptive: a,
-                            roundOffsets: c
-                        })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, Y(Object.assign({}, l, {
-                            offsets: e.modifiersData.arrow,
-                            position: "absolute",
-                            adaptive: !1,
-                            roundOffsets: c
-                        })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
-                            "data-popper-placement": e.placement
-                        })
-                    },
-                    data: {}
-                }, G, {
-                    name: "offset",
-                    enabled: !0,
-                    phase: "main",
-                    requires: ["popperOffsets"],
-                    fn: function(t) {
-                        var e = t.state,
-                            n = t.options,
-                            i = t.name,
-                            r = n.offset,
-                            o = void 0 === r ? [0, 0] : r,
-                            a = H.reduce((function(t, n) {
-                                return t[n] = function(t, e, n) {
-                                    var i = I(t),
-                                        r = [M, A].indexOf(i) >= 0 ? -1 : 1,
-                                        o = "function" == typeof n ? n(Object.assign({}, e, {
-                                            placement: t
-                                        })) : n,
-                                        a = o[0],
-                                        s = o[1];
-                                    return a = a || 0, s = (s || 0) * r, [M, C].indexOf(i) >= 0 ? {
-                                        x: s,
-                                        y: a
-                                    } : {
-                                        x: a,
-                                        y: s
-                                    }
-                                }(n, e.rects, o), t
-                            }), {}),
-                            s = a[e.placement],
-                            c = s.x,
-                            l = s.y;
-                        null != e.modifiersData.popperOffsets && (e.modifiersData.popperOffsets.x += c, e.modifiersData.popperOffsets.y += l), e.modifiersData[i] = a
-                    }
-                }, {
-                    name: "flip",
-                    enabled: !0,
-                    phase: "main",
-                    fn: function(t) {
-                        var e = t.state,
-                            n = t.options,
-                            i = t.name;
-                        if (!e.modifiersData[i]._skip) {
-                            for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = e.options.placement, g = I(v), w = c || (g !== v && h ? function(t) {
-                                    if (I(t) === S) return [];
-                                    var e = K(t);
-                                    return [Z(t), e, Z(e)]
-                                }(v) : [K(v)]), y = [v].concat(w).reduce((function(t, n) {
-                                    return t.concat(I(n) === S ? function(t, e) {
-                                        void 0 === e && (e = {});
-                                        var n = e,
-                                            i = n.placement,
-                                            r = n.boundary,
-                                            o = n.rootBoundary,
-                                            a = n.padding,
-                                            s = n.flipVariations,
-                                            c = n.allowedAutoPlacements,
-                                            l = void 0 === c ? H : c,
-                                            d = U(i),
-                                            p = d ? s ? W : W.filter((function(t) {
-                                                return U(t) === d
-                                            })) : D,
-                                            u = p.filter((function(t) {
-                                                return l.indexOf(t) >= 0
-                                            }));
-                                        0 === u.length && (u = p);
-                                        var f = u.reduce((function(e, n) {
-                                            return e[n] = ot(t, {
-                                                placement: n,
-                                                boundary: r,
-                                                rootBoundary: o,
-                                                padding: a
-                                            })[I(n)], e
-                                        }), {});
-                                        return Object.keys(f).sort((function(t, e) {
-                                            return f[t] - f[e]
-                                        }))
-                                    }(e, {
-                                        placement: n,
-                                        boundary: d,
-                                        rootBoundary: p,
-                                        padding: l,
-                                        flipVariations: h,
-                                        allowedAutoPlacements: m
-                                    }) : n)
-                                }), []), b = e.rects.reference, x = e.rects.popper, E = new Map, O = !0, L = y[0], j = 0; j < y.length; j++) {
-                                var P = y[j],
-                                    N = I(P),
-                                    R = U(P) === k,
-                                    B = [A, T].indexOf(N) >= 0,
-                                    _ = B ? "width" : "height",
-                                    F = ot(e, {
-                                        placement: P,
-                                        boundary: d,
-                                        rootBoundary: p,
-                                        altBoundary: u,
-                                        padding: l
-                                    }),
-                                    V = B ? R ? C : M : R ? T : A;
-                                b[_] > x[_] && (V = K(V));
-                                var q = K(V),
-                                    $ = [];
-                                if (o && $.push(F[N] <= 0), s && $.push(F[V] <= 0, F[q] <= 0), $.every((function(t) {
-                                        return t
-                                    }))) {
-                                    L = P, O = !1;
-                                    break
-                                }
-                                E.set(P, $)
-                            }
-                            if (O)
-                                for (var z = function(t) {
-                                        var e = y.find((function(e) {
-                                            var n = E.get(e);
-                                            if (n) return n.slice(0, t).every((function(t) {
-                                                return t
-                                            }))
-                                        }));
-                                        if (e) return L = e, "break"
-                                    }, X = h ? 3 : 1; X > 0 && "break" !== z(X); X--);
-                            e.placement !== L && (e.modifiersData[i]._skip = !0, e.placement = L, e.reset = !0)
-                        }
-                    },
-                    requiresIfExists: ["offset"],
-                    data: {
-                        _skip: !1
-                    }
-                }, {
-                    name: "preventOverflow",
-                    enabled: !0,
-                    phase: "main",
-                    fn: function(t) {
-                        var e = t.state,
-                            n = t.options,
-                            i = t.name,
-                            r = n.mainAxis,
-                            s = void 0 === r || r,
-                            c = n.altAxis,
-                            l = void 0 !== c && c,
-                            d = n.boundary,
-                            p = n.rootBoundary,
-                            u = n.altBoundary,
-                            f = n.padding,
-                            h = n.tether,
-                            m = void 0 === h || h,
-                            v = n.tetherOffset,
-                            g = void 0 === v ? 0 : v,
-                            y = ot(e, {
-                                boundary: d,
-                                rootBoundary: p,
-                                padding: f,
-                                altBoundary: u
-                            }),
-                            b = I(e.placement),
-                            x = U(e.placement),
-                            E = !x,
-                            O = $(b),
-                            S = "x" === O ? "y" : "x",
-                            D = e.modifiersData.popperOffsets,
-                            j = e.rects.reference,
-                            P = e.rects.popper,
-                            N = "function" == typeof g ? g(Object.assign({}, e.rects, {
-                                placement: e.placement
-                            })) : g,
-                            W = "number" == typeof N ? {
-                                mainAxis: N,
-                                altAxis: N
-                            } : Object.assign({
-                                mainAxis: 0,
-                                altAxis: 0
-                            }, N),
-                            H = e.modifiersData.offset ? e.modifiersData.offset[e.placement] : null,
-                            R = {
-                                x: 0,
-                                y: 0
-                            };
-                        if (D) {
-                            if (s) {
-                                var B, _ = "y" === O ? A : M,
-                                    F = "y" === O ? T : C,
-                                    V = "y" === O ? "height" : "width",
-                                    q = D[O],
-                                    z = q + y[_],
-                                    X = q - y[F],
-                                    Y = m ? -P[V] / 2 : 0,
-                                    G = x === k ? j[V] : P[V],
-                                    J = x === k ? -P[V] : -j[V],
-                                    K = e.elements.arrow,
-                                    Q = m && K ? w(K) : {
-                                        width: 0,
-                                        height: 0
-                                    },
-                                    Z = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : {
-                                        top: 0,
-                                        right: 0,
-                                        bottom: 0,
-                                        left: 0
-                                    },
-                                    tt = Z[_],
-                                    et = Z[F],
-                                    nt = at(0, j[V], Q[V]),
-                                    it = E ? j[V] / 2 - Y - nt - tt - W.mainAxis : G - nt - tt - W.mainAxis,
-                                    rt = E ? -j[V] / 2 + Y + nt + et + W.mainAxis : J + nt + et + W.mainAxis,
-                                    st = e.elements.arrow && L(e.elements.arrow),
-                                    ct = st ? "y" === O ? st.clientTop || 0 : st.clientLeft || 0 : 0,
-                                    lt = null != (B = null == H ? void 0 : H[O]) ? B : 0,
-                                    dt = q + rt - lt,
-                                    pt = at(m ? a(z, q + it - lt - ct) : z, q, m ? o(X, dt) : X);
-                                D[O] = pt, R[O] = pt - q
-                            }
-                            if (l) {
-                                var ut, ft = "x" === O ? A : M,
-                                    ht = "x" === O ? T : C,
-                                    mt = D[S],
-                                    vt = "y" === S ? "height" : "width",
-                                    gt = mt + y[ft],
-                                    wt = mt - y[ht],
-                                    yt = -1 !== [A, M].indexOf(b),
-                                    bt = null != (ut = null == H ? void 0 : H[S]) ? ut : 0,
-                                    xt = yt ? gt : mt - j[vt] - P[vt] - bt + W.altAxis,
-                                    Et = yt ? mt + j[vt] + P[vt] - bt - W.altAxis : wt,
-                                    Ot = m && yt ? function(t, e, n) {
-                                        var i = at(t, e, n);
-                                        return i > n ? n : i
-                                    }(xt, mt, Et) : at(m ? xt : gt, mt, m ? Et : wt);
-                                D[S] = Ot, R[S] = Ot - mt
-                            }
-                            e.modifiersData[i] = R
-                        }
-                    },
-                    requiresIfExists: ["offset"]
-                }, {
-                    name: "arrow",
-                    enabled: !0,
-                    phase: "main",
-                    fn: function(t) {
-                        var e, n = t.state,
-                            i = t.name,
-                            r = t.options,
-                            o = n.elements.arrow,
-                            a = n.modifiersData.popperOffsets,
-                            s = I(n.placement),
-                            c = $(s),
-                            l = [M, C].indexOf(s) >= 0 ? "height" : "width";
-                        if (o && a) {
-                            var d = function(t, e) {
-                                    return it("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
-                                        placement: e.placement
-                                    })) : t) ? t : rt(t, D))
-                                }(r.padding, n),
-                                p = w(o),
-                                u = "y" === c ? A : M,
-                                f = "y" === c ? T : C,
-                                h = n.rects.reference[l] + n.rects.reference[c] - a[c] - n.rects.popper[l],
-                                m = a[c] - n.rects.reference[c],
-                                v = L(o),
-                                g = v ? "y" === c ? v.clientHeight || 0 : v.clientWidth || 0 : 0,
-                                y = h / 2 - m / 2,
-                                b = d[u],
-                                x = g - p[l] - d[f],
-                                E = g / 2 - p[l] / 2 + y,
-                                O = at(b, E, x),
-                                S = c;
-                            n.modifiersData[i] = ((e = {})[S] = O, e.centerOffset = O - E, e)
-                        }
-                    },
-                    effect: function(t) {
-                        var e = t.state,
-                            n = t.options.element,
-                            i = void 0 === n ? "[data-popper-arrow]" : n;
-                        null != i && ("string" != typeof i || (i = e.elements.popper.querySelector(i))) && tt(e.elements.popper, i) && (e.elements.arrow = i)
-                    },
-                    requires: ["popperOffsets"],
-                    requiresIfExists: ["preventOverflow"]
-                }, {
+                }, J, K, Q, lt, pt, ut, {
                     name: "hide",
                     enabled: !0,
                     phase: "main",
                     requiresIfExists: ["preventOverflow"],
                     fn: function(t) {
                         var e = t.state,
                             n = t.name,
                             i = e.rects.reference,
                             r = e.rects.popper,
                             o = e.modifiersData.preventOverflow,
-                            a = ot(e, {
+                            a = ct(e, {
                                 elementContext: "reference"
                             }),
-                            s = ot(e, {
+                            s = ct(e, {
                                 altBoundary: !0
                             }),
-                            c = st(a, i),
-                            l = st(s, r, o),
-                            d = ct(c),
-                            p = ct(l);
+                            c = ft(a, i),
+                            l = ft(s, r, o),
+                            d = ht(c),
+                            p = ht(l);
                         e.modifiersData[n] = {
                             referenceClippingOffsets: c,
                             popperEscapeOffsets: l,
                             isReferenceHidden: d,
                             hasPopperEscaped: p
                         }, e.attributes.popper = Object.assign({}, e.attributes.popper, {
                             "data-popper-reference-hidden": d,
                             "data-popper-escaped": p
                         })
                     }
                 }]
             }),
-            dt = "tippy-content",
-            pt = "tippy-backdrop",
-            ut = "tippy-arrow",
-            ft = "tippy-svg-arrow",
-            ht = {
+            vt = "tippy-content",
+            gt = "tippy-backdrop",
+            wt = "tippy-arrow",
+            yt = "tippy-svg-arrow",
+            bt = {
                 passive: !0,
                 capture: !0
             },
-            mt = function() {
+            xt = function() {
                 return document.body
             };
 
-        function vt(t, e, n) {
+        function Et(t, e, n) {
             if (Array.isArray(t)) {
                 var i = t[e];
                 return null == i ? Array.isArray(n) ? n[e] : n : i
             }
             return t
         }
 
-        function gt(t, e) {
+        function Ot(t, e) {
             var n = {}.toString.call(t);
             return 0 === n.indexOf("[object") && n.indexOf(e + "]") > -1
         }
 
-        function wt(t, e) {
+        function Lt(t, e) {
             return "function" == typeof t ? t.apply(void 0, e) : t
         }
 
-        function yt(t, e) {
+        function At(t, e) {
             return 0 === e ? t : function(i) {
                 clearTimeout(n), n = setTimeout((function() {
                     t(i)
                 }), e)
             };
             var n
         }
 
-        function bt(t) {
+        function Tt(t) {
             return [].concat(t)
         }
 
-        function xt(t, e) {
+        function Ct(t, e) {
             -1 === t.indexOf(e) && t.push(e)
         }
 
-        function Et(t) {
+        function Mt(t) {
             return [].slice.call(t)
         }
 
-        function Ot(t) {
+        function St(t) {
             return Object.keys(t).reduce((function(e, n) {
                 return void 0 !== t[n] && (e[n] = t[n]), e
             }), {})
         }
 
-        function Lt() {
+        function Dt() {
             return document.createElement("div")
         }
 
-        function At(t) {
+        function kt(t) {
             return ["Element", "Fragment"].some((function(e) {
-                return gt(t, e)
+                return Ot(t, e)
             }))
         }
 
-        function Tt(t, e) {
+        function jt(t, e) {
             t.forEach((function(t) {
                 t && (t.style.transitionDuration = e + "ms")
             }))
         }
 
-        function Ct(t, e) {
+        function Pt(t, e) {
             t.forEach((function(t) {
                 t && t.setAttribute("data-state", e)
             }))
         }
 
-        function Mt(t, e, n) {
+        function Nt(t, e, n) {
             var i = e + "EventListener";
             ["transitionend", "webkitTransitionEnd"].forEach((function(e) {
                 t[i](e, n)
             }))
         }
 
-        function St(t, e) {
+        function Ht(t, e) {
             for (var n = e; n;) {
                 var i;
                 if (t.contains(n)) return !0;
                 n = null == n.getRootNode || null == (i = n.getRootNode()) ? void 0 : i.host
             }
             return !1
         }
-        var Dt = {
+        var Rt = {
                 isTouch: !1
             },
-            kt = 0;
+            Wt = 0;
 
-        function jt() {
-            Dt.isTouch || (Dt.isTouch = !0, window.performance && document.addEventListener("mousemove", Pt))
+        function Bt() {
+            Rt.isTouch || (Rt.isTouch = !0, window.performance && document.addEventListener("mousemove", It))
         }
 
-        function Pt() {
+        function It() {
             var t = performance.now();
-            t - kt < 20 && (Dt.isTouch = !1, document.removeEventListener("mousemove", Pt)), kt = t
+            t - Wt < 20 && (Rt.isTouch = !1, document.removeEventListener("mousemove", It)), Wt = t
         }
 
-        function Nt() {
+        function _t() {
             var t, e = document.activeElement;
             if ((t = e) && t._tippy && t._tippy.reference === t) {
                 var n = e._tippy;
                 e.blur && !n.state.isVisible && e.blur()
             }
         }
-        var Wt = !("undefined" == typeof window || "undefined" == typeof document || !window.msCrypto),
-            Ht = Object.assign({
-                appendTo: mt,
+        var Ft = !("undefined" == typeof window || "undefined" == typeof document || !window.msCrypto),
+            qt = Object.assign({
+                appendTo: xt,
                 aria: {
                     content: "auto",
                     expanded: "auto"
                 },
                 delay: 0,
                 duration: [300, 250],
                 getReferenceClientRect: null,
@@ -1313,121 +1457,121 @@
                 content: "",
                 inertia: !1,
                 maxWidth: 350,
                 role: "tooltip",
                 theme: "",
                 zIndex: 9999
             }),
-            Rt = Object.keys(Ht);
+            Vt = Object.keys(qt);
 
-        function Bt(t) {
+        function Ut(t) {
             var e = (t.plugins || []).reduce((function(e, n) {
                 var i, r = n.name,
                     o = n.defaultValue;
-                return r && (e[r] = void 0 !== t[r] ? t[r] : null != (i = Ht[r]) ? i : o), e
+                return r && (e[r] = void 0 !== t[r] ? t[r] : null != (i = qt[r]) ? i : o), e
             }), {});
             return Object.assign({}, t, e)
         }
 
-        function _t(t, e) {
+        function $t(t, e) {
             var n = Object.assign({}, e, {
-                content: wt(e.content, [t])
+                content: Lt(e.content, [t])
             }, e.ignoreAttributes ? {} : function(t, e) {
-                return (e ? Object.keys(Bt(Object.assign({}, Ht, {
+                return (e ? Object.keys(Ut(Object.assign({}, qt, {
                     plugins: e
-                }))) : Rt).reduce((function(e, n) {
+                }))) : Vt).reduce((function(e, n) {
                     var i = (t.getAttribute("data-tippy-" + n) || "").trim();
                     if (!i) return e;
                     if ("content" === n) e[n] = i;
                     else try {
                         e[n] = JSON.parse(i)
                     } catch (t) {
                         e[n] = i
                     }
                     return e
                 }), {})
             }(t, e.plugins));
-            return n.aria = Object.assign({}, Ht.aria, n.aria), n.aria = {
+            return n.aria = Object.assign({}, qt.aria, n.aria), n.aria = {
                 expanded: "auto" === n.aria.expanded ? e.interactive : n.aria.expanded,
                 content: "auto" === n.aria.content ? e.interactive ? null : "describedby" : n.aria.content
             }, n
         }
-        var Ft = function() {
+        var zt = function() {
             return "innerHTML"
         };
 
-        function Vt(t, e) {
-            t[Ft()] = e
+        function Xt(t, e) {
+            t[zt()] = e
         }
 
-        function qt(t) {
-            var e = Lt();
-            return !0 === t ? e.className = ut : (e.className = ft, At(t) ? e.appendChild(t) : Vt(e, t)), e
+        function Yt(t) {
+            var e = Dt();
+            return !0 === t ? e.className = wt : (e.className = yt, kt(t) ? e.appendChild(t) : Xt(e, t)), e
         }
 
-        function It(t, e) {
-            At(e.content) ? (Vt(t, ""), t.appendChild(e.content)) : "function" != typeof e.content && (e.allowHTML ? Vt(t, e.content) : t.textContent = e.content)
+        function Gt(t, e) {
+            kt(e.content) ? (Xt(t, ""), t.appendChild(e.content)) : "function" != typeof e.content && (e.allowHTML ? Xt(t, e.content) : t.textContent = e.content)
         }
 
-        function Ut(t) {
+        function Jt(t) {
             var e = t.firstElementChild,
-                n = Et(e.children);
+                n = Mt(e.children);
             return {
                 box: e,
                 content: n.find((function(t) {
-                    return t.classList.contains(dt)
+                    return t.classList.contains(vt)
                 })),
                 arrow: n.find((function(t) {
-                    return t.classList.contains(ut) || t.classList.contains(ft)
+                    return t.classList.contains(wt) || t.classList.contains(yt)
                 })),
                 backdrop: n.find((function(t) {
-                    return t.classList.contains(pt)
+                    return t.classList.contains(gt)
                 }))
             }
         }
 
-        function $t(t) {
-            var e = Lt(),
-                n = Lt();
+        function Kt(t) {
+            var e = Dt(),
+                n = Dt();
             n.className = "tippy-box", n.setAttribute("data-state", "hidden"), n.setAttribute("tabindex", "-1");
-            var i = Lt();
+            var i = Dt();
 
             function r(n, i) {
-                var r = Ut(e),
+                var r = Jt(e),
                     o = r.box,
                     a = r.content,
                     s = r.arrow;
-                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || It(a, t.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(qt(i.arrow))) : o.appendChild(qt(i.arrow)) : s && o.removeChild(s)
+                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || Gt(a, t.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(Yt(i.arrow))) : o.appendChild(Yt(i.arrow)) : s && o.removeChild(s)
             }
-            return i.className = dt, i.setAttribute("data-state", "hidden"), It(i, t.props), e.appendChild(n), n.appendChild(i), r(t.props, t.props), {
+            return i.className = vt, i.setAttribute("data-state", "hidden"), Gt(i, t.props), e.appendChild(n), n.appendChild(i), r(t.props, t.props), {
                 popper: e,
                 onUpdate: r
             }
         }
-        $t.$$tippy = !0;
-        var zt = 1,
-            Xt = [],
-            Yt = [];
+        Kt.$$tippy = !0;
+        var Qt = 1,
+            Zt = [],
+            te = [];
 
-        function Gt(t, e) {
-            var n, i, r, o, a, s, c, l, d = _t(t, Object.assign({}, Ht, Bt(Ot(e)))),
+        function ee(t, e) {
+            var n, i, r, o, a, s, c, l, d = $t(t, Object.assign({}, qt, Ut(St(e)))),
                 p = !1,
                 u = !1,
                 f = !1,
                 h = !1,
                 m = [],
-                v = yt(X, d.interactiveDebounce),
-                g = zt++,
+                v = At(X, d.interactiveDebounce),
+                g = Qt++,
                 w = (l = d.plugins).filter((function(t, e) {
                     return l.indexOf(t) === e
                 })),
                 y = {
                     id: g,
                     reference: t,
-                    popper: Lt(),
+                    popper: Dt(),
                     popperInstance: null,
                     props: d,
                     state: {
                         isEnabled: !0,
                         isVisible: !1,
                         isDestroyed: !1,
                         isMounted: !1,
@@ -1437,91 +1581,91 @@
                     clearDelayTimeouts: function() {
                         clearTimeout(n), clearTimeout(i), cancelAnimationFrame(r)
                     },
                     setProps: function(e) {
                         if (!y.state.isDestroyed) {
                             P("onBeforeUpdate", [y, e]), $();
                             var n = y.props,
-                                i = _t(t, Object.assign({}, n, Ot(e), {
+                                i = $t(t, Object.assign({}, n, St(e), {
                                     ignoreAttributes: !0
                                 }));
-                            y.props = i, U(), n.interactiveDebounce !== i.interactiveDebounce && (H(), v = yt(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? bt(n.triggerTarget).forEach((function(t) {
+                            y.props = i, U(), n.interactiveDebounce !== i.interactiveDebounce && (R(), v = At(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? Tt(n.triggerTarget).forEach((function(t) {
                                 t.removeAttribute("aria-expanded")
-                            })) : i.triggerTarget && t.removeAttribute("aria-expanded"), W(), j(), E && E(n, i), y.popperInstance && (K(), Z().forEach((function(t) {
+                            })) : i.triggerTarget && t.removeAttribute("aria-expanded"), H(), j(), E && E(n, i), y.popperInstance && (K(), Z().forEach((function(t) {
                                 requestAnimationFrame(t._tippy.popperInstance.forceUpdate)
                             }))), P("onAfterUpdate", [y, e])
                         }
                     },
                     setContent: function(t) {
                         y.setProps({
                             content: t
                         })
                     },
                     show: function() {
                         var t = y.state.isVisible,
                             e = y.state.isDestroyed,
                             n = !y.state.isEnabled,
-                            i = Dt.isTouch && !y.props.touch,
-                            r = vt(y.props.duration, 0, Ht.duration);
+                            i = Rt.isTouch && !y.props.touch,
+                            r = Et(y.props.duration, 0, qt.duration);
                         if (!(t || e || n || i || M().hasAttribute("disabled") || (P("onShow", [y], !1), !1 === y.props.onShow(y)))) {
-                            if (y.state.isVisible = !0, C() && (x.style.visibility = "visible"), j(), F(), y.state.isMounted || (x.style.transition = "none"), C()) {
+                            if (y.state.isVisible = !0, C() && (x.style.visibility = "visible"), j(), _(), y.state.isMounted || (x.style.transition = "none"), C()) {
                                 var o = D();
-                                Tt([o.box, o.content], 0)
+                                jt([o.box, o.content], 0)
                             }
                             var a, c, l;
                             s = function() {
                                 var t;
                                 if (y.state.isVisible && !h) {
                                     if (h = !0, x.offsetHeight, x.style.transition = y.props.moveTransition, C() && y.props.animation) {
                                         var e = D(),
                                             n = e.box,
                                             i = e.content;
-                                        Tt([n, i], r), Ct([n, i], "visible")
+                                        jt([n, i], r), Pt([n, i], "visible")
                                     }
-                                    N(), W(), xt(Yt, y), null == (t = y.popperInstance) || t.forceUpdate(), P("onMount", [y]), y.props.animation && C() && function(t, e) {
+                                    N(), H(), Ct(te, y), null == (t = y.popperInstance) || t.forceUpdate(), P("onMount", [y]), y.props.animation && C() && function(t, e) {
                                         q(t, (function() {
                                             y.state.isShown = !0, P("onShown", [y])
                                         }))
                                     }(r)
                                 }
-                            }, c = y.props.appendTo, l = M(), (a = y.props.interactive && c === mt || "parent" === c ? l.parentNode : wt(c, [l])).contains(x) || a.appendChild(x), y.state.isMounted = !0, K()
+                            }, c = y.props.appendTo, l = M(), (a = y.props.interactive && c === xt || "parent" === c ? l.parentNode : Lt(c, [l])).contains(x) || a.appendChild(x), y.state.isMounted = !0, K()
                         }
                     },
                     hide: function() {
                         var t = !y.state.isVisible,
                             e = y.state.isDestroyed,
                             n = !y.state.isEnabled,
-                            i = vt(y.props.duration, 1, Ht.duration);
+                            i = Et(y.props.duration, 1, qt.duration);
                         if (!(t || e || n) && (P("onHide", [y], !1), !1 !== y.props.onHide(y))) {
-                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, C() && (x.style.visibility = "hidden"), H(), V(), j(!0), C()) {
+                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, C() && (x.style.visibility = "hidden"), R(), F(), j(!0), C()) {
                                 var r = D(),
                                     o = r.box,
                                     a = r.content;
-                                y.props.animation && (Tt([o, a], i), Ct([o, a], "hidden"))
+                                y.props.animation && (jt([o, a], i), Pt([o, a], "hidden"))
                             }
-                            N(), W(), y.props.animation ? C() && function(t, e) {
+                            N(), H(), y.props.animation ? C() && function(t, e) {
                                 q(t, (function() {
                                     !y.state.isVisible && x.parentNode && x.parentNode.contains(x) && e()
                                 }))
                             }(i, y.unmount) : y.unmount()
                         }
                     },
                     hideWithInteractivity: function(t) {
-                        S().addEventListener("mousemove", v), xt(Xt, v), v(t)
+                        S().addEventListener("mousemove", v), Ct(Zt, v), v(t)
                     },
                     enable: function() {
                         y.state.isEnabled = !0
                     },
                     disable: function() {
                         y.hide(), y.state.isEnabled = !1
                     },
                     unmount: function() {
                         y.state.isVisible && y.hide(), y.state.isMounted && (Q(), Z().forEach((function(t) {
                             t._tippy.unmount()
-                        })), x.parentNode && x.parentNode.removeChild(x), Yt = Yt.filter((function(t) {
+                        })), x.parentNode && x.parentNode.removeChild(x), te = te.filter((function(t) {
                             return t !== y
                         })), y.state.isMounted = !1, P("onHidden", [y]))
                     },
                     destroy: function() {
                         y.state.isDestroyed || (y.clearDelayTimeouts(), y.unmount(), $(), delete t._tippy, y.state.isDestroyed = !0, P("onDestroy", [y]))
                     }
                 };
@@ -1530,15 +1674,15 @@
                 x = b.popper,
                 E = b.onUpdate;
             x.setAttribute("data-tippy-root", ""), x.id = "tippy-" + y.id, y.popper = x, t._tippy = y, x._tippy = y;
             var O = w.map((function(t) {
                     return t.fn(y)
                 })),
                 L = t.hasAttribute("aria-expanded");
-            return U(), W(), j(), P("onCreate", [y]), d.showOnCreate && tt(), x.addEventListener("mouseenter", (function() {
+            return U(), H(), j(), P("onCreate", [y]), d.showOnCreate && tt(), x.addEventListener("mouseenter", (function() {
                 y.props.interactive && y.state.isVisible && y.clearDelayTimeouts()
             })), x.addEventListener("mouseleave", (function() {
                 y.props.interactive && y.props.trigger.indexOf("mouseenter") >= 0 && S().addEventListener("mousemove", v)
             })), y;
 
             function A() {
                 var t = y.props.touch;
@@ -1556,23 +1700,23 @@
 
             function M() {
                 return c || t
             }
 
             function S() {
                 var t, e, n = M().parentNode;
-                return n ? null != (e = bt(n)[0]) && null != (t = e.ownerDocument) && t.body ? e.ownerDocument : document : document
+                return n ? null != (e = Tt(n)[0]) && null != (t = e.ownerDocument) && t.body ? e.ownerDocument : document : document
             }
 
             function D() {
-                return Ut(x)
+                return Jt(x)
             }
 
             function k(t) {
-                return y.state.isMounted && !y.state.isVisible || Dt.isTouch || o && "focus" === o.type ? 0 : vt(y.props.delay, t ? 0 : 1, Ht.delay)
+                return y.state.isMounted && !y.state.isVisible || Rt.isTouch || o && "focus" === o.type ? 0 : Et(y.props.delay, t ? 0 : 1, qt.delay)
             }
 
             function j(t) {
                 void 0 === t && (t = !1), x.style.pointerEvents = y.props.interactive && !t ? "" : "none", x.style.zIndex = "" + y.props.zIndex
             }
 
             function P(t, e, n) {
@@ -1583,109 +1727,109 @@
             }
 
             function N() {
                 var e = y.props.aria;
                 if (e.content) {
                     var n = "aria-" + e.content,
                         i = x.id;
-                    bt(y.props.triggerTarget || t).forEach((function(t) {
+                    Tt(y.props.triggerTarget || t).forEach((function(t) {
                         var e = t.getAttribute(n);
                         if (y.state.isVisible) t.setAttribute(n, e ? e + " " + i : i);
                         else {
                             var r = e && e.replace(i, "").trim();
                             r ? t.setAttribute(n, r) : t.removeAttribute(n)
                         }
                     }))
                 }
             }
 
-            function W() {
-                !L && y.props.aria.expanded && bt(y.props.triggerTarget || t).forEach((function(t) {
+            function H() {
+                !L && y.props.aria.expanded && Tt(y.props.triggerTarget || t).forEach((function(t) {
                     y.props.interactive ? t.setAttribute("aria-expanded", y.state.isVisible && t === M() ? "true" : "false") : t.removeAttribute("aria-expanded")
                 }))
             }
 
-            function H() {
-                S().removeEventListener("mousemove", v), Xt = Xt.filter((function(t) {
+            function R() {
+                S().removeEventListener("mousemove", v), Zt = Zt.filter((function(t) {
                     return t !== v
                 }))
             }
 
-            function R(e) {
-                if (!Dt.isTouch || !f && "mousedown" !== e.type) {
+            function W(e) {
+                if (!Rt.isTouch || !f && "mousedown" !== e.type) {
                     var n = e.composedPath && e.composedPath()[0] || e.target;
-                    if (!y.props.interactive || !St(x, n)) {
-                        if (bt(y.props.triggerTarget || t).some((function(t) {
-                                return St(t, n)
+                    if (!y.props.interactive || !Ht(x, n)) {
+                        if (Tt(y.props.triggerTarget || t).some((function(t) {
+                                return Ht(t, n)
                             }))) {
-                            if (Dt.isTouch) return;
+                            if (Rt.isTouch) return;
                             if (y.state.isVisible && y.props.trigger.indexOf("click") >= 0) return
                         } else P("onClickOutside", [y, e]);
                         !0 === y.props.hideOnClick && (y.clearDelayTimeouts(), y.hide(), u = !0, setTimeout((function() {
                             u = !1
-                        })), y.state.isMounted || V())
+                        })), y.state.isMounted || F())
                     }
                 }
             }
 
             function B() {
                 f = !0
             }
 
-            function _() {
+            function I() {
                 f = !1
             }
 
-            function F() {
+            function _() {
                 var t = S();
-                t.addEventListener("mousedown", R, !0), t.addEventListener("touchend", R, ht), t.addEventListener("touchstart", _, ht), t.addEventListener("touchmove", B, ht)
+                t.addEventListener("mousedown", W, !0), t.addEventListener("touchend", W, bt), t.addEventListener("touchstart", I, bt), t.addEventListener("touchmove", B, bt)
             }
 
-            function V() {
+            function F() {
                 var t = S();
-                t.removeEventListener("mousedown", R, !0), t.removeEventListener("touchend", R, ht), t.removeEventListener("touchstart", _, ht), t.removeEventListener("touchmove", B, ht)
+                t.removeEventListener("mousedown", W, !0), t.removeEventListener("touchend", W, bt), t.removeEventListener("touchstart", I, bt), t.removeEventListener("touchmove", B, bt)
             }
 
             function q(t, e) {
                 var n = D().box;
 
                 function i(t) {
-                    t.target === n && (Mt(n, "remove", i), e())
+                    t.target === n && (Nt(n, "remove", i), e())
                 }
                 if (0 === t) return e();
-                Mt(n, "remove", a), Mt(n, "add", i), a = i
+                Nt(n, "remove", a), Nt(n, "add", i), a = i
             }
 
-            function I(e, n, i) {
-                void 0 === i && (i = !1), bt(y.props.triggerTarget || t).forEach((function(t) {
+            function V(e, n, i) {
+                void 0 === i && (i = !1), Tt(y.props.triggerTarget || t).forEach((function(t) {
                     t.addEventListener(e, n, i), m.push({
                         node: t,
                         eventType: e,
                         handler: n,
                         options: i
                     })
                 }))
             }
 
             function U() {
                 var t;
-                T() && (I("touchstart", z, {
+                T() && (V("touchstart", z, {
                     passive: !0
-                }), I("touchend", Y, {
+                }), V("touchend", Y, {
                     passive: !0
                 })), (t = y.props.trigger, t.split(/\s+/).filter(Boolean)).forEach((function(t) {
-                    if ("manual" !== t) switch (I(t, z), t) {
+                    if ("manual" !== t) switch (V(t, z), t) {
                         case "mouseenter":
-                            I("mouseleave", Y);
+                            V("mouseleave", Y);
                             break;
                         case "focus":
-                            I(Wt ? "focusout" : "blur", G);
+                            V(Ft ? "focusout" : "blur", G);
                             break;
                         case "focusin":
-                            I("focusout", G)
+                            V("focusout", G)
                     }
                 }))
             }
 
             function $() {
                 m.forEach((function(t) {
                     var e = t.node,
@@ -1696,15 +1840,15 @@
                 })), m = []
             }
 
             function z(t) {
                 var e, n = !1;
                 if (y.state.isEnabled && !J(t) && !u) {
                     var i = "focus" === (null == (e = o) ? void 0 : e.type);
-                    o = t, c = t.currentTarget, W(), !y.state.isVisible && gt(t, "MouseEvent") && Xt.forEach((function(e) {
+                    o = t, c = t.currentTarget, H(), !y.state.isVisible && Ot(t, "MouseEvent") && Zt.forEach((function(e) {
                         return e(t)
                     })), "click" === t.type && (y.props.trigger.indexOf("mouseenter") < 0 || p) && !1 !== y.props.hideOnClick && y.state.isVisible ? n = !0 : tt(t), "click" === t.type && (p = !n), n && !i && et(t)
                 }
             }
 
             function X(t) {
                 var e = t.target,
@@ -1734,39 +1878,39 @@
                                 p = "left" === a ? s.right.x : 0,
                                 u = e.top - i + c > o,
                                 f = i - e.bottom - l > o,
                                 h = e.left - n + d > o,
                                 m = n - e.right - p > o;
                             return u || f || h || m
                         }))
-                    })(i, t) && (H(), et(t))
+                    })(i, t) && (R(), et(t))
                 }
             }
 
             function Y(t) {
                 J(t) || y.props.trigger.indexOf("click") >= 0 && p || (y.props.interactive ? y.hideWithInteractivity(t) : et(t))
             }
 
             function G(t) {
                 y.props.trigger.indexOf("focusin") < 0 && t.target !== M() || y.props.interactive && t.relatedTarget && x.contains(t.relatedTarget) || et(t)
             }
 
             function J(t) {
-                return !!Dt.isTouch && T() !== t.type.indexOf("touch") >= 0
+                return !!Rt.isTouch && T() !== t.type.indexOf("touch") >= 0
             }
 
             function K() {
                 Q();
                 var e = y.props,
                     n = e.popperOptions,
                     i = e.placement,
                     r = e.offset,
                     o = e.getReferenceClientRect,
                     a = e.moveTransition,
-                    c = C() ? Ut(x).arrow : null,
+                    c = C() ? Jt(x).arrow : null,
                     l = o ? {
                         getBoundingClientRect: o,
                         contextElement: o.contextElement || M()
                     } : t,
                     d = [{
                         name: "offset",
                         options: {
@@ -1809,74 +1953,74 @@
                     }];
                 C() && c && d.push({
                     name: "arrow",
                     options: {
                         element: c,
                         padding: 3
                     }
-                }), d.push.apply(d, (null == n ? void 0 : n.modifiers) || []), y.popperInstance = lt(l, x, Object.assign({}, n, {
+                }), d.push.apply(d, (null == n ? void 0 : n.modifiers) || []), y.popperInstance = mt(l, x, Object.assign({}, n, {
                     placement: i,
                     onFirstUpdate: s,
                     modifiers: d
                 }))
             }
 
             function Q() {
                 y.popperInstance && (y.popperInstance.destroy(), y.popperInstance = null)
             }
 
             function Z() {
-                return Et(x.querySelectorAll("[data-tippy-root]"))
+                return Mt(x.querySelectorAll("[data-tippy-root]"))
             }
 
             function tt(t) {
-                y.clearDelayTimeouts(), t && P("onTrigger", [y, t]), F();
+                y.clearDelayTimeouts(), t && P("onTrigger", [y, t]), _();
                 var e = k(!0),
                     i = A(),
                     r = i[0],
                     o = i[1];
-                Dt.isTouch && "hold" === r && o && (e = o), e ? n = setTimeout((function() {
+                Rt.isTouch && "hold" === r && o && (e = o), e ? n = setTimeout((function() {
                     y.show()
                 }), e) : y.show()
             }
 
             function et(t) {
                 if (y.clearDelayTimeouts(), P("onUntrigger", [y, t]), y.state.isVisible) {
                     if (!(y.props.trigger.indexOf("mouseenter") >= 0 && y.props.trigger.indexOf("click") >= 0 && ["mouseleave", "mousemove"].indexOf(t.type) >= 0 && p)) {
                         var e = k(!1);
                         e ? i = setTimeout((function() {
                             y.state.isVisible && y.hide()
                         }), e) : r = requestAnimationFrame((function() {
                             y.hide()
                         }))
                     }
-                } else V()
+                } else F()
             }
         }
 
-        function Jt(t, e) {
+        function ne(t, e) {
             void 0 === e && (e = {});
-            var n = Ht.plugins.concat(e.plugins || []);
-            document.addEventListener("touchstart", jt, ht), window.addEventListener("blur", Nt);
+            var n = qt.plugins.concat(e.plugins || []);
+            document.addEventListener("touchstart", Bt, bt), window.addEventListener("blur", _t);
             var i, r = Object.assign({}, e, {
                     plugins: n
                 }),
-                o = (i = t, At(i) ? [i] : function(t) {
-                    return gt(t, "NodeList")
-                }(i) ? Et(i) : Array.isArray(i) ? i : Et(document.querySelectorAll(i))).reduce((function(t, e) {
-                    var n = e && Gt(e, r);
+                o = (i = t, kt(i) ? [i] : function(t) {
+                    return Ot(t, "NodeList")
+                }(i) ? Mt(i) : Array.isArray(i) ? i : Mt(document.querySelectorAll(i))).reduce((function(t, e) {
+                    var n = e && ee(e, r);
                     return n && t.push(n), t
                 }), []);
-            return At(t) ? o[0] : o
+            return kt(t) ? o[0] : o
         }
-        Jt.defaultProps = Ht, Jt.setDefaultProps = function(t) {
+        ne.defaultProps = qt, ne.setDefaultProps = function(t) {
             Object.keys(t).forEach((function(e) {
-                Ht[e] = t[e]
+                qt[e] = t[e]
             }))
-        }, Jt.currentInput = Dt, Object.assign({}, G, {
+        }, ne.currentInput = Rt, Object.assign({}, K, {
             effect: function(t) {
                 var e = t.state,
                     n = {
                         popper: {
                             position: e.options.strategy,
                             left: "0",
                             top: "0",
@@ -1885,68 +2029,82 @@
                         arrow: {
                             position: "absolute"
                         },
                         reference: {}
                     };
                 Object.assign(e.elements.popper.style, n.popper), e.styles = n, e.elements.arrow && Object.assign(e.elements.arrow.style, n.arrow)
             }
-        }), Jt.setDefaultProps({
-            render: $t
+        }), ne.setDefaultProps({
+            render: Kt
         });
-        const Kt = Jt;
-        n(2);
-        class Qt {
+        const ie = ne;
+        var re = n(72),
+            oe = n.n(re),
+            ae = n(825),
+            se = n.n(ae),
+            ce = n(659),
+            le = n.n(ce),
+            de = n(56),
+            pe = n.n(de),
+            ue = n(540),
+            fe = n.n(ue),
+            he = n(113),
+            me = n.n(he),
+            ve = n(2),
+            ge = {};
+        ge.styleTagTransform = me(), ge.setAttributes = pe(), ge.insert = le().bind(null, "head"), ge.domAPI = se(), ge.insertStyleElement = fe(), oe()(ve.A, ge), ve.A && ve.A.locals && ve.A.locals;
+        class we {
             constructor(t) {
                 this.element = t, this.tooltipConfig = this.makeConfig(), this.init()
             }
             init() {
-                Kt(this.element, this.tooltipConfig)
+                ie(this.element, this.tooltipConfig)
             }
             makeConfig() {
                 const t = {
                     content: this.element.getAttribute("title")
                 };
                 for (let e = 0; e < this.element.attributes.length; e++) {
                     const n = this.element.attributes[e];
                     n.name.startsWith("data-tooltip-") && (t[n.name.replace("data-tooltip-", "")] = n.value)
                 }
                 return this.tooltipConfig = t, t
             }
         }
 
-        function Zt(t) {
+        function ye(t) {
             const e = t.dataset.feditConstructor;
             if (e) return window.wagtailFedit.editors[e];
             throw new Error("No editor class found for element")
         }
 
-        function te(t = document) {
+        function be(t = document) {
             let e;
             e = t instanceof HTMLElement && t.classList.contains("wagtail-fedit-adapter-wrapper") && !t.classList.contains("wagtail-fedit-initialized") ? [t] : t.querySelectorAll(".wagtail-fedit-adapter-wrapper");
             for (let n = 0; n < e.length; n++) {
                 const i = e[n];
                 if (!i.classList.contains("wagtail-fedit-initialized")) {
                     i.classList.add("wagtail-fedit-initialized");
-                    const t = Zt(i);
+                    const t = ye(i);
                     t ? new t(i) : console.error("No editor class found for element", i)
                 }
                 const r = t.querySelectorAll("[data-tooltip='true']");
                 for (let t = 0; t < r.length; t++) {
                     const e = r[t];
-                    "true" == e.dataset.tooltip && (new Qt(e), delete e.dataset.tooltip)
+                    "true" == e.dataset.tooltip && (new we(e), delete e.dataset.tooltip)
                 }
             }
         }
 
-        function ee(t) {
+        function xe(t) {
             if (!t) return;
             const e = new URL(t.href);
             window.scrollY > 100 && e.searchParams.set("scrollY", `${window.scrollY}`), window.scrollX > 100 && e.searchParams.set("scrollX", `${window.scrollX}`), t.href = e.toString()
         }
-        class ne {
+        class Ee {
             constructor(t) {
                 this.editor = t
             }
             openModal() {
                 this.editor.makeModal()
             }
             closeModal() {
@@ -1977,30 +2135,30 @@
             refetch() {
                 return this.editor.refetch()
             }
             execRelated(t) {
                 for (const e of this.editor.relatedWrappers) t(e.editorAPI)
             }
         }
-        const ie = "wagtail-fedit-modal",
-            re = `\n<div class="${ie}-wrapper">\n    <div class="${ie}" id="${ie}-__ID__-modal">\n    </div>\n</div>`;
-        class oe {
+        const Oe = "wagtail-fedit-modal",
+            Le = `\n<div class="${Oe}-wrapper">\n    <div class="${Oe}" id="${Oe}-__ID__-modal">\n    </div>\n</div>`;
+        class Ae {
             constructor(t) {
-                this.options = t, this.modalHtml = re.replace("__ID__", this.options.modalId)
+                this.options = t, this.modalHtml = Le.replace("__ID__", this.options.modalId)
             }
             static get modalWrapper() {
-                var t = document.querySelector(`#${ie}-wrapper`);
-                return t || ((t = document.createElement("div")).id = `${ie}-wrapper`, t.classList.add(`${ie}-wrapper`), document.body.appendChild(t), t)
+                var t = document.querySelector(`#${Oe}-wrapper`);
+                return t || ((t = document.createElement("div")).id = `${Oe}-wrapper`, t.classList.add(`${Oe}-wrapper`), document.body.appendChild(t), t)
             }
             get wrapper() {
                 return this.constructor.modalWrapper
             }
             get modal() {
-                var t = this.wrapper.querySelector(`.${ie}`);
-                t && t.id !== `${ie}-${this.options.modalId}-modal` && (t.remove(), t = null), t || (t = this.buildModal());
+                var t = this.wrapper.querySelector(`.${Oe}`);
+                t && t.id !== `${Oe}-${this.options.modalId}-modal` && (t.remove(), t = null), t || (t = this.buildModal());
                 var e = t;
                 return e.modal = this, e
             }
             get innerHTML() {
                 return this.modal.innerHTML
             }
             set innerHTML(t) {
@@ -2013,16 +2171,16 @@
                 return this.modal.classList
             }
             get children() {
                 return this.modal.children
             }
             buildModal() {
                 var t = this.wrapper,
-                    e = t.querySelector(`.${ie}`);
-                return e || (t.innerHTML = this.modalHtml, e = t.querySelector(`.${ie}`)), e.modal || (e.modal = this), e
+                    e = t.querySelector(`.${Oe}`);
+                return e || (t.innerHTML = this.modalHtml, e = t.querySelector(`.${Oe}`)), e.modal || (e.modal = this), e
             }
             addClass(t) {
                 this.modal.classList.add(t)
             }
             removeClass(t) {
                 this.modal.classList.remove(t)
             }
@@ -2052,15 +2210,15 @@
             addEventListener(t, e) {
                 this.modal.addEventListener(t, e)
             }
             removeEventListener(t, e) {
                 this.modal.removeEventListener(t, e)
             }
         }
-        class ae {
+        class Te {
             constructor(t) {
                 const {
                     id: e,
                     className: n,
                     srcdoc: i = null,
                     url: r = null,
                     onLoad: o = (() => {}),
@@ -2107,15 +2265,15 @@
                         newFrame: r
                     })
                 }, r.onerror = () => {
                     i()
                 }, r
             }
         }
-        var se = function(t, e, n, i) {
+        var Ce = function(t, e, n, i) {
             return new(n || (n = Promise))((function(r, o) {
                 function a(t) {
                     try {
                         c(i.next(t))
                     } catch (t) {
                         o(t)
                     }
@@ -2134,17 +2292,17 @@
                     t.done ? r(t.value) : (e = t.value, e instanceof n ? e : new n((function(t) {
                         t(e)
                     }))).then(a, s)
                 }
                 c((i = i.apply(t, e || [])).next())
             }))
         };
-        class ce extends EventTarget {
+        class Me extends EventTarget {
             constructor(t) {
-                super(), this.api = new ne(this), this.initialTitle = document.title, this.wrapperElement = t, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), this.modal = new oe({
+                super(), this.api = new Ee(this), this.initialTitle = document.title, this.wrapperElement = t, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), this.modal = new Ae({
                     modalId: this.wrapperElement.id,
                     onClose: () => {
                         window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.executeEvent(window.wagtailFedit.EVENTS.MODAL_CLOSE)
                     }
                 }), window.location.hash === `#${this.wrapperElement.id}` && (this.makeModal(), this.focus())
             }
             get editUrl() {
@@ -2155,20 +2313,20 @@
             }
             get relatedWrappers() {
                 const t = this.wrapperElement.dataset.wrapperId,
                     e = document.querySelectorAll(`[data-wrapper-id="${t}"]`);
                 return Array.from(e).filter((t => t !== this.wrapperElement))
             }
             init() {
-                this.sharedContext = this.wrapperElement.dataset.sharedContext, this.wrapperElement.editorAPI = this.api, this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button"), this.editBtn.addEventListener("click", (t => se(this, void 0, void 0, (function*() {
+                this.sharedContext = this.wrapperElement.dataset.sharedContext, this.wrapperElement.editorAPI = this.api, this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button"), this.editBtn.addEventListener("click", (t => Ce(this, void 0, void 0, (function*() {
                     t.preventDefault(), t.stopPropagation(), yield this.makeModal()
                 }))))
             }
             initNewEditors() {
-                te(this.wrapperElement)
+                be(this.wrapperElement)
             }
             focus() {
                 this.wrapperElement.focus()
             }
             refetch() {
                 return new Promise(((t, e) => {
                     fetch(this.getRefetchUrl()).then((t => t.json())).then((e => {
@@ -2186,16 +2344,16 @@
                 return t.pathname = this.editUrl, this.sharedContext && t.searchParams.set("shared_context", this.sharedContext), t.toString()
             }
             getRefetchUrl() {
                 const t = new URL(window.location.href);
                 return t.pathname = this.refetchUrl, this.sharedContext && t.searchParams.set("shared_context", this.sharedContext), t.toString()
             }
             makeModal() {
-                return se(this, void 0, void 0, (function*() {
-                    this.iframe = new ae({
+                return Ce(this, void 0, void 0, (function*() {
+                    this.iframe = new Te({
                         url: this.getEditUrl(),
                         id: "wagtail-fedit-iframe",
                         className: null,
                         onLoad: () => {
                             const t = e => {
                                 e.preventDefault();
                                 const n = new FormData(this.iframe.formElement);
@@ -2263,15 +2421,15 @@
                 t.startsWith(`${window.wagtailFedit.NAMESPACE}:`) || (n = `${window.wagtailFedit.NAMESPACE}:${t}`);
                 const i = new CustomEvent(n, {
                     detail: e
                 });
                 super.dispatchEvent(i), this.wrapperElement.dispatchEvent(i), document.dispatchEvent(i)
             }
         }
-        class le {
+        class Se {
             constructor(t) {
                 this.publishButton = t, this.publishButtonsWrapper = t.parentElement.querySelector(".wagtail-fedit-form-buttons");
                 const e = this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button");
                 let n = !1;
                 for (let t = 0; t < e.length; t++)
                     if (e[t].classList.contains("initially-hidden")) {
                         n = !0;
@@ -2307,15 +2465,15 @@
                         easing: "ease-in-out"
                     }).onfinish = () => {
                         this.publishButtonsWrapper.classList.add("open")
                     })
                 }))
             }
         }
-        class de extends ce {
+        class De extends Me {
             static get funcMap() {
                 return window
             }
             onResponse(t) {
                 const e = t.func.name,
                     n = t.func.target;
                 if (!e || !n) return void console.error("Invalid response", t);
@@ -2323,20 +2481,20 @@
                 if (!i) return void console.error("Target element not found", n);
                 const r = this.constructor.funcMap[e];
                 if (r) return r(i, t);
                 console.error("Function not found", e)
             }
         }
 
-        function pe() {
-            te(), new MutationObserver((t => {
+        function ke() {
+            be(), new MutationObserver((t => {
                 for (const e of t)
                     for (let t = 0; t < e.addedNodes.length; t++) {
                         const n = e.addedNodes[t];
-                        1 === n.nodeType && te(n)
+                        1 === n.nodeType && be(n)
                     }
             })).observe(document.body, {
                 childList: !0,
                 subtree: !0
             });
             const t = new URL(window.location.href),
                 e = t.searchParams.get("scrollY") || 0,
@@ -2347,36 +2505,36 @@
                 const t = i.shadowRoot.querySelector("#wagtail-fedit-editor-button"),
                     e = i.shadowRoot.querySelector("#wagtail-fedit-live-button"),
                     n = i.shadowRoot.querySelector("#wagtail-fedit-publish-menu");
                 if (t || e) {
                     let n;
                     window.addEventListener("scroll", (() => {
                         n && clearTimeout(n), n = setTimeout((() => {
-                            ee(t), ee(e);
+                            xe(t), xe(e);
                             const n = new URL(window.location.href);
                             n.searchParams.set("scrollY", `${window.scrollY}`), n.searchParams.set("scrollX", `${window.scrollX}`), window.history.replaceState(null, "", n.toString())
                         }), 50)
                     }))
                 }
-                n && new le(n)
+                n && new Se(n)
             }
         }
         window.wagtailFedit = {
             NAMESPACE: "wagtail-fedit",
             EVENTS: {
                 SUBMIT: "wagtail-fedit:submit",
                 CHANGE: "wagtail-fedit:change",
                 MODAL_OPEN: "wagtail-fedit:modalOpen",
                 MODAL_LOAD: "wagtail-fedit:modalLoad",
                 MODAL_CLOSE: "wagtail-fedit:modalClose",
                 SUBMIT_ERROR: "wagtail-fedit:submitError"
             },
             editors: {
-                "wagtail_fedit.editors.BaseFuncEditor": de,
-                "wagtail_fedit.editors.BlockFieldEditor": class extends ce {
+                "wagtail_fedit.editors.BaseFuncEditor": De,
+                "wagtail_fedit.editors.BlockFieldEditor": class extends Me {
                     onResponse(t) {
                         return this.api.updateHtml((e => {
                             this.wrapperElement.animate([{
                                 opacity: 1
                             }, {
                                 opacity: 0
                             }], {
@@ -2396,15 +2554,15 @@
                                 }).onfinish = () => {
                                     n.style.opacity = "1"
                                 }
                             }
                         }))
                     }
                 },
-                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends de {
+                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends De {
                     static get funcMap() {
                         return window.wagtailFedit.funcs
                     }
                 }
             },
             funcs: {
                 "wagtail_fedit.funcs.backgroundImageFunc": function(t, e) {
@@ -2415,10 +2573,10 @@
             },
             register: function(t, e) {
                 this.editors[t] = e
             },
             registerFunc: function(t, e) {
                 this.funcs[t] = e
             }
-        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", pe) : pe()
+        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", ke) : ke()
     })()
 })();
```

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.5rc8/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.5rc7
+Version: 1.5.5rc8
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.5rc7/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.5rc8/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

