# Comparing `tmp/notolog-0.9.1b3.tar.gz` & `tmp/notolog-0.9.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.1b3.tar", last modified: Sat May 11 12:50:34 2024, max compression
+gzip compressed data, was "notolog-0.9.1b4.tar", last modified: Sun May 12 16:48:59 2024, max compression
```

## Comparing `notolog-0.9.1b3.tar` & `notolog-0.9.1b4.tar`

### file list

```diff
@@ -1,350 +1,352 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.238985 notolog-0.9.1b3/
--rw-r--r--   0 vadikus    (501) staff       (20)     6779 2024-05-11 12:47:23.000000 notolog-0.9.1b3/CHANGELOG.md
--rw-r--r--   0 vadikus    (501) staff       (20)     3490 2024-05-11 12:17:28.000000 notolog-0.9.1b3/CODE_OF_CONDUCT.md
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b3/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      433 2024-05-11 12:17:28.000000 notolog-0.9.1b3/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    17100 2024-05-11 12:50:34.238299 notolog-0.9.1b3/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    15048 2024-05-11 12:17:28.000000 notolog-0.9.1b3/README.md
--rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b3/app_config.toml
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.073611 notolog-0.9.1b3/docs/
--rw-r--r--   0 vadikus    (501) staff       (20)     8631 2024-05-11 12:17:28.000000 notolog-0.9.1b3/docs/Examples.md
--rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b3/docs/notolog-ui-settings.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.110060 notolog-0.9.1b3/notolog/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-11 12:47:08.000000 notolog-0.9.1b3/notolog/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.140620 notolog-0.9.1b3/notolog/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.052247 notolog-0.9.1b3/notolog/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.200484 notolog-0.9.1b3/notolog/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2311 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      885 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6818 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.227442 notolog-0.9.1b3/notolog/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.922423 notolog-0.9.1b3/notolog/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2363 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      721 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     8472 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.934207 notolog-0.9.1b3/notolog/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2480 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6935 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.959532 notolog-0.9.1b3/notolog/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2408 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      753 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     8451 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.968075 notolog-0.9.1b3/notolog/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4341 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.973459 notolog-0.9.1b3/notolog/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1433 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5624 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1125 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/enums/enum_base.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1367 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)      451 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4516 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.974678 notolog-0.9.1b3/notolog/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.979874 notolog-0.9.1b3/notolog/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.984679 notolog-0.9.1b3/notolog/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9213 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    51699 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9909 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/image_downloader.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:33.986676 notolog-0.9.1b3/notolog/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.003270 notolog-0.9.1b3/notolog/lexemes/de/
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6586 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.015977 notolog-0.9.1b3/notolog/lexemes/en/
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6051 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.024652 notolog-0.9.1b3/notolog/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6560 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.033063 notolog-0.9.1b3/notolog/lexemes/fi/
--rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fi/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fi/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6292 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/fi/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fi/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fi/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fi/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fi/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.046644 notolog-0.9.1b3/notolog/lexemes/fr/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6716 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.062248 notolog-0.9.1b3/notolog/lexemes/ge/
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9735 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.070281 notolog-0.9.1b3/notolog/lexemes/gr/
--rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/gr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/gr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8668 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/gr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/gr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/gr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/gr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/gr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.079564 notolog-0.9.1b3/notolog/lexemes/in/
--rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/in/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/in/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10078 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/in/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/in/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/in/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/in/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/in/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.089648 notolog-0.9.1b3/notolog/lexemes/it/
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6366 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.115459 notolog-0.9.1b3/notolog/lexemes/ja/
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7248 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.126774 notolog-0.9.1b3/notolog/lexemes/ko/
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6775 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.133933 notolog-0.9.1b3/notolog/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6245 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.140779 notolog-0.9.1b3/notolog/lexemes/nl/
--rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/nl/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/nl/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6475 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/nl/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/nl/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/nl/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/nl/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/nl/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.158398 notolog-0.9.1b3/notolog/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6357 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.167643 notolog-0.9.1b3/notolog/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7938 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.177178 notolog-0.9.1b3/notolog/lexemes/se/
--rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/se/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/se/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6253 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/se/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/se/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/se/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/se/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/se/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.187645 notolog-0.9.1b3/notolog/lexemes/tr/
--rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/tr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/tr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6154 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/tr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/tr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/tr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/tr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/tr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.201010 notolog-0.9.1b3/notolog/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5777 2024-05-11 12:17:28.000000 notolog-0.9.1b3/notolog/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2860 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/main.py
--rw-r--r--   0 vadikus    (501) staff       (20)   177588 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.223500 notolog-0.9.1b3/notolog/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    37284 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)    12804 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-11 09:19:41.000000 notolog-0.9.1b3/notolog/view_widget.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.237420 notolog-0.9.1b3/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    17100 2024-05-11 12:50:32.000000 notolog-0.9.1b3/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    11426 2024-05-11 12:50:32.000000 notolog-0.9.1b3/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-11 12:50:32.000000 notolog-0.9.1b3/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       46 2024-05-11 12:50:32.000000 notolog-0.9.1b3/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-11 12:50:32.000000 notolog-0.9.1b3/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-05-11 12:50:32.000000 notolog-0.9.1b3/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-06 20:09:20.000000 notolog-0.9.1b3/requirements.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-11 12:50:34.239102 notolog-0.9.1b3/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     2377 2024-05-11 12:47:38.000000 notolog-0.9.1b3/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:50:34.236704 notolog-0.9.1b3/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b3/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9888 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5839 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1943 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_pkg_integration.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1178 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4484 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6226 2024-05-11 09:19:41.000000 notolog-0.9.1b3/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.310927 notolog-0.9.1b4/
+-rw-r--r--   0 vadikus    (501) staff       (20)     7403 2024-05-12 16:16:12.000000 notolog-0.9.1b4/CHANGELOG.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     3490 2024-05-11 12:17:28.000000 notolog-0.9.1b4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b4/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      433 2024-05-11 12:17:28.000000 notolog-0.9.1b4/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    17439 2024-05-12 16:48:59.232380 notolog-0.9.1b4/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    15349 2024-05-12 14:50:00.000000 notolog-0.9.1b4/README.md
+-rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b4/app_config.toml
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.838428 notolog-0.9.1b4/docs/
+-rw-r--r--   0 vadikus    (501) staff       (20)     8631 2024-05-11 12:17:28.000000 notolog-0.9.1b4/docs/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b4/docs/notolog-ui-settings.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.866873 notolog-0.9.1b4/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-12 14:50:00.000000 notolog-0.9.1b4/notolog/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.875902 notolog-0.9.1b4/notolog/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.824162 notolog-0.9.1b4/notolog/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.886726 notolog-0.9.1b4/notolog/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2311 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      885 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6818 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.901661 notolog-0.9.1b4/notolog/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.955776 notolog-0.9.1b4/notolog/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2363 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      721 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8472 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.973013 notolog-0.9.1b4/notolog/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2480 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6935 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.984706 notolog-0.9.1b4/notolog/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2408 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      753 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8451 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.990144 notolog-0.9.1b4/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4341 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:58.996856 notolog-0.9.1b4/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1433 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5624 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1125 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/enum_base.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1367 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      451 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4516 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.001391 notolog-0.9.1b4/notolog/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.014476 notolog-0.9.1b4/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.026023 notolog-0.9.1b4/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9213 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    51699 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10614 2024-05-12 16:23:25.000000 notolog-0.9.1b4/notolog/image_downloader.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.029491 notolog-0.9.1b4/notolog/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.037097 notolog-0.9.1b4/notolog/lexemes/de/
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6586 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.045950 notolog-0.9.1b4/notolog/lexemes/en/
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6051 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.060050 notolog-0.9.1b4/notolog/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6560 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.065996 notolog-0.9.1b4/notolog/lexemes/fi/
+-rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6292 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/fi/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fi/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.073713 notolog-0.9.1b4/notolog/lexemes/fr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6716 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.079264 notolog-0.9.1b4/notolog/lexemes/ge/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9735 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.085114 notolog-0.9.1b4/notolog/lexemes/gr/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8668 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/gr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/gr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.089773 notolog-0.9.1b4/notolog/lexemes/in/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10078 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/in/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/in/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.099736 notolog-0.9.1b4/notolog/lexemes/it/
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6366 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.109845 notolog-0.9.1b4/notolog/lexemes/ja/
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7248 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.116368 notolog-0.9.1b4/notolog/lexemes/ko/
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6775 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.123756 notolog-0.9.1b4/notolog/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6245 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.129926 notolog-0.9.1b4/notolog/lexemes/nl/
+-rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6475 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/nl/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/nl/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.136130 notolog-0.9.1b4/notolog/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6357 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.142253 notolog-0.9.1b4/notolog/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7938 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.154224 notolog-0.9.1b4/notolog/lexemes/se/
+-rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6253 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/se/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/se/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.161795 notolog-0.9.1b4/notolog/lexemes/tr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6154 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/tr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/tr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.170044 notolog-0.9.1b4/notolog/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5777 2024-05-11 12:17:28.000000 notolog-0.9.1b4/notolog/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2860 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/main.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   178083 2024-05-12 16:26:17.000000 notolog-0.9.1b4/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.187675 notolog-0.9.1b4/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    37284 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    12804 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-11 09:19:41.000000 notolog-0.9.1b4/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.230873 notolog-0.9.1b4/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    17439 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    11469 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       46 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      320 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-05-12 16:48:58.000000 notolog-0.9.1b4/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      320 2024-05-12 14:50:00.000000 notolog-0.9.1b4/requirements.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-12 16:48:59.311224 notolog-0.9.1b4/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2377 2024-05-12 14:50:00.000000 notolog-0.9.1b4/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-12 16:48:59.228632 notolog-0.9.1b4/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b4/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9888 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5839 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-12 14:50:00.000000 notolog-0.9.1b4/tests/test_pkg_integration.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3948 2024-05-12 16:42:21.000000 notolog-0.9.1b4/tests/test_qt_async.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2919 2024-05-12 16:16:12.000000 notolog-0.9.1b4/tests/test_qt_ui.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1178 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4484 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6226 2024-05-11 09:19:41.000000 notolog-0.9.1b4/tests/test_themes.py
```

### Comparing `notolog-0.9.1b3/CHANGELOG.md` & `notolog-0.9.1b4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 # Changelog
 All notologable changes to this project will be documented in this file.
 
+## [0.9.1b4] - 2024-05-12
+
+### Added
+- Introduced the pytest-asyncio package to support testing of asyncio code with pytest, enhancing the robustness and reliability of unit tests.
+- Added the `.gitattributes` file that was previously omitted to ensure consistent Git configurations across various environments.
+
+### Updated
+- Improved the processing and completion of tasks in the asynchronous syntax highlighter, enhancing efficiency and stability.
+- Expanded the `.gitignore` file with additional entries to better manage the files included in version control, such as ignoring more temporary files and build artifacts.
+
 ## [0.9.1b3] - 2024-05-11
 
 ### Added
 - Introduced the CODE_OF_CONDUCT.md file to promote a respectful and positive environment for all contributors and participants. This document outlines our commitment to providing a harassment-free experience for everyone and offers guidelines for respectful communication practices.
 - Support for highlighting tables in markdown edit mode, enhancing the editing experience.
 - A new EnumBase class to incorporate common methods across enums, improving code reusability.
 - Additional tests to increase coverage and ensure the stability of new features.
```

### Comparing `notolog-0.9.1b3/CODE_OF_CONDUCT.md` & `notolog-0.9.1b4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/LICENSE` & `notolog-0.9.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/PKG-INFO` & `notolog-0.9.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b3
+Version: 0.9.1b4
 Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Keywords: notolog,python,markdown,editor,ai,text
@@ -42,30 +42,34 @@
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.18.0
 Requires-Dist: PySide6==6.7.0
 Requires-Dist: PySide6_Addons==6.7.0
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
+Requires-Dist: pytest-asyncio==0.23.6
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: qasync==0.27.1
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-11 11:15:29.656338"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-12 13:57:34.333369"}} -->
 # Notolog
 
-![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
-## Overview
+## Python Markdown Editor
 
-Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
+![PyPI - License](https://img.shields.io/pypi/l/notolog)&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog)&nbsp;![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+
+Notolog is an open-source markdown editor developed with Python and PySide6. Born from a personal endeavor to tackle daily programming challenges and deepen Python proficiency, Notolog serves as a proof-of-concept that seamlessly blends simplicity with functionality. It offers an intuitive user experience across various platforms, ensuring users can efficiently manage and edit markdown files with ease.
 
 ---
-![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
+
+![Notolog UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
 
 ## Features
 
 * Notolog is open-sourced under the MIT license, promoting full transparency and encouraging collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
@@ -231,15 +235,15 @@
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
 ## License
 
-The Notolog project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+The Notolog project is licensed under the MIT License - see the [LICENSE](https://github.com/notolog/notolog-editor/blob/main/LICENSE) file for details.
 
 ## Third-Party Components
 
 ### Libraries and Licenses
 
 This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
 
@@ -266,14 +270,18 @@
 - **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
 - **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
 - **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
 - **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
 - **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
 - **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
+#### Apache License 2.0
+
+- **pytest-asyncio**: A library that provides support for testing asyncio code with pytest. [License Details](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE) , [PyPI](https://pypi.org/project/pytest-asyncio/)
+
 #### Other Dual Licensed
 
 - **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
 - **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
 
 #### Python Standard Library
```

### Comparing `notolog-0.9.1b3/README.md` & `notolog-0.9.1b4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-11 11:15:29.656338"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-12 13:57:34.333369"}} -->
 # Notolog
 
-![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
-## Overview
+## Python Markdown Editor
 
-Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
+![PyPI - License](https://img.shields.io/pypi/l/notolog)&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog)&nbsp;![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+
+Notolog is an open-source markdown editor developed with Python and PySide6. Born from a personal endeavor to tackle daily programming challenges and deepen Python proficiency, Notolog serves as a proof-of-concept that seamlessly blends simplicity with functionality. It offers an intuitive user experience across various platforms, ensuring users can efficiently manage and edit markdown files with ease.
 
 ---
-![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
+
+![Notolog UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
 
 ## Features
 
 * Notolog is open-sourced under the MIT license, promoting full transparency and encouraging collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
@@ -178,15 +181,15 @@
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
 ## License
 
-The Notolog project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+The Notolog project is licensed under the MIT License - see the [LICENSE](https://github.com/notolog/notolog-editor/blob/main/LICENSE) file for details.
 
 ## Third-Party Components
 
 ### Libraries and Licenses
 
 This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
 
@@ -213,14 +216,18 @@
 - **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
 - **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
 - **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
 - **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
 - **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
 - **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
+#### Apache License 2.0
+
+- **pytest-asyncio**: A library that provides support for testing asyncio code with pytest. [License Details](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE) , [PyPI](https://pypi.org/project/pytest-asyncio/)
+
 #### Other Dual Licensed
 
 - **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
 - **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
 
 #### Python Standard Library
```

### Comparing `notolog-0.9.1b3/docs/Examples.md` & `notolog-0.9.1b4/docs/Examples.md`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/docs/notolog-ui-settings.png` & `notolog-0.9.1b4/docs/notolog-ui-settings.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/app_config.py` & `notolog-0.9.1b4/notolog/app_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tomli
 
 toml_base_app_config = """
 [app]
 name = "Notolog"
-version = "0.9.1b3"
+version = "0.9.1b4"
 license = "MIT"
 date = "2024"
 website = "https://notolog.app"
 repository = "https://github.com/notolog/notolog-editor"
 pypi = "https://pypi.org/project/notolog"
 author = "Vadim Bakhrenkov"
```

### Comparing `notolog-0.9.1b3/notolog/assets/notolog-example-image.png` & `notolog-0.9.1b4/notolog/assets/notolog-example-image.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/notolog-logo.png` & `notolog-0.9.1b4/notolog/assets/notolog-logo.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.1b4/notolog/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/calligraphy/default.ini` & `notolog-0.9.1b4/notolog/assets/themes/calligraphy/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/calligraphy/md.ini` & `notolog-0.9.1b4/notolog/assets/themes/calligraphy/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.1b4/notolog/assets/themes/calligraphy/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/calligraphy/styles.css` & `notolog-0.9.1b4/notolog/assets/themes/calligraphy/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.1b4/notolog/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/about_popup.css` & `notolog-0.9.1b4/notolog/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/default.ini` & `notolog-0.9.1b4/notolog/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/LICENSE` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/balloon.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/folder.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/github.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/quote.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/robot.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/star.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/trash3.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.1b4/notolog/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/md.ini` & `notolog-0.9.1b4/notolog/assets/themes/default/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/settings_dialog.css` & `notolog-0.9.1b4/notolog/assets/themes/default/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/styles.css` & `notolog-0.9.1b4/notolog/assets/themes/default/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/default/tree_view.css` & `notolog-0.9.1b4/notolog/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.1b4/notolog/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/noir_dark/default.ini` & `notolog-0.9.1b4/notolog/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/noir_dark/md.ini` & `notolog-0.9.1b4/notolog/assets/themes/noir_dark/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.1b4/notolog/assets/themes/noir_dark/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/noir_dark/styles.css` & `notolog-0.9.1b4/notolog/assets/themes/noir_dark/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.1b4/notolog/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/strawberry/about_popup.css` & `notolog-0.9.1b4/notolog/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/strawberry/default.ini` & `notolog-0.9.1b4/notolog/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/strawberry/md.ini` & `notolog-0.9.1b4/notolog/assets/themes/strawberry/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.1b4/notolog/assets/themes/strawberry/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/strawberry/styles.css` & `notolog-0.9.1b4/notolog/assets/themes/strawberry/styles.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/assets/themes/strawberry/tree_view.css` & `notolog-0.9.1b4/notolog/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/edit_widget.py` & `notolog-0.9.1b4/notolog/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/editor_state.py` & `notolog-0.9.1b4/notolog/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/encrypt/enc_helper.py` & `notolog-0.9.1b4/notolog/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/encrypt/enc_new_password_dialog.py` & `notolog-0.9.1b4/notolog/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/encrypt/enc_password.py` & `notolog-0.9.1b4/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/encrypt/enc_password_dialog.py` & `notolog-0.9.1b4/notolog/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.1b4/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/enums/ai_model_names.py` & `notolog-0.9.1b4/notolog/enums/ai_model_names.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/enums/colors.py` & `notolog-0.9.1b4/notolog/enums/colors.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/enums/enum_base.py` & `notolog-0.9.1b4/notolog/enums/enum_base.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/enums/languages.py` & `notolog-0.9.1b4/notolog/enums/languages.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/etree_extension.py` & `notolog-0.9.1b4/notolog/etree_extension.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/file_header.py` & `notolog-0.9.1b4/notolog/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/file_system_watcher.py` & `notolog-0.9.1b4/notolog/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/helpers/file_helper.py` & `notolog-0.9.1b4/notolog/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/helpers/theme_helper.py` & `notolog-0.9.1b4/notolog/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/helpers/tooltip_helper.py` & `notolog-0.9.1b4/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/helpers/update_helper.py` & `notolog-0.9.1b4/notolog/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/highlight/main_highlighter.py` & `notolog-0.9.1b4/notolog/highlight/main_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/highlight/md_highlighter.py` & `notolog-0.9.1b4/notolog/highlight/md_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/highlight/view_highlighter.py` & `notolog-0.9.1b4/notolog/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/image_downloader.py` & `notolog-0.9.1b4/notolog/image_downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -165,26 +165,22 @@
 
     @asyncSlot()
     async def download_resource_in_queue(self, resource_url) -> None:
         if self.debug:
             self.logger.debug('Downloading resource %d tasks in queue' % len(self.resource_tasks))
 
         task = asyncio.ensure_future(self.resource_download_async(resource_url))
-        task.add_done_callback(
-            lambda _task:
-            (self.logger.debug('%s from total %d completed with callback'
-                               % (_task.get_name(), len(self.resource_tasks))) if self.debug else None,
-             # Remove finished task from the queue
-             self.resource_tasks.remove(_task))
-        )
+        # Add task to the local pool first
         self.resource_tasks.append(task)
+        # Callback method to set up further actions
+        task.add_done_callback(lambda _task: self.resource_task_callback(_task))
 
         done, pending = await asyncio.wait(
             self.resource_tasks,
-            return_when=asyncio.ALL_COMPLETED,  # no pending tasks check
+            return_when=asyncio.ALL_COMPLETED,  # There is no pending tasks check
             # timeout = 1.5  # to return after the timeout, some task could be pending
         )
 
         if self.debug:
             self.logger.debug(f'Downloading resource tasks progress. Done {len(done)}, pending {len(pending)}')
 
         if len(self.resource_tasks) <= 1:
@@ -192,20 +188,39 @@
             # typically ahead.
             await asyncio.sleep(0.25, self.event_loop)
             if self.downloaded_cnt > 0:
                 # All tasks in queue have finished
                 self.finished.emit(self.downloaded_cnt)
                 self.downloaded_cnt = 0
 
+    def resource_task_callback(self, task):
+        if self.debug:
+            self.logger.debug('%s from total %d completed with callback'
+                              % (task.get_name(), len(self.resource_tasks)))
+
+        # Remove finished task from the queue
+        self.resource_tasks.remove(task)
+
     async def resource_download_async(self, image_url) -> None:
         """
-        Downloading resource which is will be processed by resource_downloaded_handler() then.
+        Downloading resource which will be processed by resource_downloaded_handler() then.
         """
         self.download_image(image_url)
 
+    async def cancel_tasks(self):
+        tasks_total = len(self.resource_tasks)
+        for i, task in enumerate(self.resource_tasks):
+            if not task.done():
+                task_res = task.cancel()
+                if self.logging:
+                    self.logger.info(
+                        f'[{i + 1}/{tasks_total}] Pending task "{task.get_name()}" canceled with result "{task_res}"')
+                # Gather all tasks to ensure they are completed before closing
+                await asyncio.gather(*self.resource_tasks, return_exceptions=True)
+
     @staticmethod
     def is_external_url(url, base_domain='example.com'):
         """
         Determine if the given URL is an external URL.
         """
         parsed_url = urlparse(url)
         return not (parsed_url.netloc == '' or parsed_url.netloc.endswith(base_domain))
```

### Comparing `notolog-0.9.1b3/notolog/lexemes/de/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/de/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/de/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/de/common.py` & `notolog-0.9.1b4/notolog/lexemes/de/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/de/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/de/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/de/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/de/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/de/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/en/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/en/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/en/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/en/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/en/common.py` & `notolog-0.9.1b4/notolog/lexemes/en/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/en/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/en/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/en/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/en/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/en/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/en/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/es/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/es/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/es/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/es/common.py` & `notolog-0.9.1b4/notolog/lexemes/es/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/es/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/es/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/es/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/es/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/es/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fi/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/fi/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fi/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/fi/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fi/common.py` & `notolog-0.9.1b4/notolog/lexemes/fi/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fi/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/fi/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fi/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/fi/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fi/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/fi/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fi/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/fi/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fr/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/fr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fr/common.py` & `notolog-0.9.1b4/notolog/lexemes/fr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fr/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fr/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/fr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fr/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/fr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/fr/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ge/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ge/common.py` & `notolog-0.9.1b4/notolog/lexemes/ge/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ge/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ge/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ge/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ge/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/ge/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ge/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/gr/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/gr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/gr/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/gr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/gr/common.py` & `notolog-0.9.1b4/notolog/lexemes/gr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/gr/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/gr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/gr/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/gr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/gr/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/gr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/gr/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/gr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/in/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/in/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/in/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/in/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/in/common.py` & `notolog-0.9.1b4/notolog/lexemes/in/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/in/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/in/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/in/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/in/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/in/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/in/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/in/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/in/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/it/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/it/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/it/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/it/common.py` & `notolog-0.9.1b4/notolog/lexemes/it/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/it/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/it/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/it/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/it/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/it/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/it/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/it/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ja/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/ja/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ja/common.py` & `notolog-0.9.1b4/notolog/lexemes/ja/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ja/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/ja/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ja/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ja/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ja/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/ja/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ja/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ko/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/ko/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ko/common.py` & `notolog-0.9.1b4/notolog/lexemes/ko/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ko/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/ko/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ko/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ko/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ko/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ko/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/la/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/la/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/la/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/la/common.py` & `notolog-0.9.1b4/notolog/lexemes/la/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/la/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/la/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/la/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/la/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/la/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/la/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/lexemes.py` & `notolog-0.9.1b4/notolog/lexemes/lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/nl/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/nl/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/nl/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/nl/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/nl/common.py` & `notolog-0.9.1b4/notolog/lexemes/nl/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/nl/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/nl/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/nl/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/nl/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/nl/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/nl/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/nl/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/nl/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/pt/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/pt/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/pt/common.py` & `notolog-0.9.1b4/notolog/lexemes/pt/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/pt/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/pt/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/pt/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/pt/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/pt/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/pt/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ru/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/ru/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ru/common.py` & `notolog-0.9.1b4/notolog/lexemes/ru/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ru/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ru/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/ru/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ru/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/ru/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/ru/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/se/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/se/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/se/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/se/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/se/common.py` & `notolog-0.9.1b4/notolog/lexemes/se/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/se/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/se/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/se/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/se/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/se/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/se/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/se/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/se/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/tr/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/tr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/tr/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/tr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/tr/common.py` & `notolog-0.9.1b4/notolog/lexemes/tr/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/tr/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/tr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/tr/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/tr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/tr/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/tr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/tr/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/tr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/zh/ai_assistant.py` & `notolog-0.9.1b4/notolog/lexemes/zh/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/zh/common.py` & `notolog-0.9.1b4/notolog/lexemes/zh/common.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/zh/main_menu.py` & `notolog-0.9.1b4/notolog/lexemes/zh/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/zh/settings_dialog.py` & `notolog-0.9.1b4/notolog/lexemes/zh/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/zh/statusbar.py` & `notolog-0.9.1b4/notolog/lexemes/zh/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/lexemes/zh/toolbar.py` & `notolog-0.9.1b4/notolog/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/main.py` & `notolog-0.9.1b4/notolog/main.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/notolog_editor.py` & `notolog-0.9.1b4/notolog/notolog_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1708,68 +1708,82 @@
 
     @asyncClose
     async def closeEvent(self, event):
         if self.logging:
             self.logger.info('Stopping events loop, closing the app... Sayonara!')
 
         # Cancel all pending tasks if exist
-        if hasattr(self, 're_tasks'):
+        if hasattr(self, 'rehighlight_tasks'):
             tasks_total = len(self.rehighlight_tasks)
             for i, task in enumerate(self.rehighlight_tasks):
                 if not task.done():
                     task_res = task.cancel()
                     if self.logging:
                         self.logger.info(f'[{i+1}/{tasks_total}] Pending task "{task.get_name()}" canceled with result "{task_res}"')
+                    # Gather all tasks to ensure they are completed before closing
+                    await asyncio.gather(*self.rehighlight_tasks, return_exceptions=True)
+
+        # Cancel all resource downloading tasks if they are exist
+        if hasattr(self, 'resource_downloader'):
+            await self.resource_downloader.cancel_tasks()
 
         if self.get_mode() == Mode.EDIT:
             # Save any unsaved changes
             self.save_active_file(clear_after=False)
         else:
             # Save cursor position (block start)
             self.store_doc_cursor_pos(self.get_mode())
 
         self.settings.mode = self.get_mode().value
         self.settings.source = self.get_source().value
 
         event.accept()
 
     @asyncSlot()
-    async def rehighlight_in_queue(self, full_rehighlight: bool = False) -> None:
+    async def rehighlight_in_queue(self, full_rehighlight: bool = False) -> Any:
         """
         More info about asyncio tasks: https://docs.python.org/3/library/asyncio-task.html
         """
         if self.debug:
             self.logger.debug('Re-highlight %d tasks in queue' % len(self.rehighlight_tasks))
 
         postpone = False if len(self.rehighlight_tasks) == 0 else True
         if self.debug:
             self.logger.debug('Re-highlight is to postpone "%r"' % postpone)
 
+        task = None
         # To keep only a few tasks in queue
         if len(self.rehighlight_tasks) < 3:
             task = asyncio.ensure_future(self.rehighlight_async(full_rehighlight, postpone))
             # task = asyncio.create_task(self.rehighlight_async(full_rehighlight, postpone))
-            task.add_done_callback(
-                lambda _task:
-                    (self.logger.info('%s from total %d completed with callback'
-                                      % (_task.get_name(), len(self.rehighlight_tasks))) if self.debug else None,
-                        self.rehighlight_tasks.remove(_task),
-                        QTimer.singleShot(750,
-                            lambda: self.rehighlight_editor(True)) if len(self.rehighlight_tasks) == 0 else None)
-            )
+            # Add task to the local pool first
             self.rehighlight_tasks.append(task)
+            # Callback method to set up further actions
+            task.add_done_callback(lambda _task: self.rehighlight_task_callback(_task))
 
         done, pending = await asyncio.wait(
             self.rehighlight_tasks,
-            return_when=asyncio.ALL_COMPLETED,  # no pending tasks check
+            return_when=asyncio.ALL_COMPLETED,  # There is no pending tasks check
         )
 
         if self.debug:
             self.logger.debug(f'Re-highlight tasks progress. Done {len(done)}, pending {len(pending)}')
 
+        return task
+
+    def rehighlight_task_callback(self, task) -> None:
+        if self.debug:
+            self.logger.debug('%s from total %d completed with callback'
+                              % (task.get_name(), len(self.rehighlight_tasks)))
+
+        self.rehighlight_tasks.remove(task)
+
+        if len(self.rehighlight_tasks) == 0:
+            QTimer.singleShot(750, lambda: self.rehighlight_editor(True))
+
     async def rehighlight_async(self, full_rehighlight: bool = False, postpone: bool = False) -> None:
         """
         Run this method not too often to avoid overwhelming the system.
         """
         # First of all check it's necessary
         if self.get_mode() == Mode.EDIT and self.get_source() == Source.MARKDOWN:
             # Postpone before re-highlighting if a few tasks
```

### Comparing `notolog-0.9.1b3/notolog/settings.py` & `notolog-0.9.1b4/notolog/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/text_block_data.py` & `notolog-0.9.1b4/notolog/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/theme.py` & `notolog-0.9.1b4/notolog/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/about_popup.py` & `notolog-0.9.1b4/notolog/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/ai_assistant.py` & `notolog-0.9.1b4/notolog/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/color_picker_dialog.py` & `notolog-0.9.1b4/notolog/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/common_dialog.py` & `notolog-0.9.1b4/notolog/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/enum_combo_box.py` & `notolog-0.9.1b4/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/file_system_model.py` & `notolog-0.9.1b4/notolog/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/line_numbers.py` & `notolog-0.9.1b4/notolog/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/rename_file_dialog.py` & `notolog-0.9.1b4/notolog/ui/rename_file_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/rotating_label.py` & `notolog-0.9.1b4/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/settings_dialog.py` & `notolog-0.9.1b4/notolog/ui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/sort_filter_proxy_model.py` & `notolog-0.9.1b4/notolog/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/statusbar.py` & `notolog-0.9.1b4/notolog/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/ui/toolbar.py` & `notolog-0.9.1b4/notolog/ui/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/view_decorator.py` & `notolog-0.9.1b4/notolog/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/view_processor.py` & `notolog-0.9.1b4/notolog/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog/view_widget.py` & `notolog-0.9.1b4/notolog/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/notolog.egg-info/PKG-INFO` & `notolog-0.9.1b4/notolog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b3
+Version: 0.9.1b4
 Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
 Keywords: notolog,python,markdown,editor,ai,text
@@ -42,30 +42,34 @@
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.18.0
 Requires-Dist: PySide6==6.7.0
 Requires-Dist: PySide6_Addons==6.7.0
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
+Requires-Dist: pytest-asyncio==0.23.6
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: qasync==0.27.1
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-11 11:15:29.656338"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-12 13:57:34.333369"}} -->
 # Notolog
 
-![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+![Notolog - Python Markdown Editor](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)
 
-## Overview
+## Python Markdown Editor
 
-Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
+![PyPI - License](https://img.shields.io/pypi/l/notolog)&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog)&nbsp;![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+
+Notolog is an open-source markdown editor developed with Python and PySide6. Born from a personal endeavor to tackle daily programming challenges and deepen Python proficiency, Notolog serves as a proof-of-concept that seamlessly blends simplicity with functionality. It offers an intuitive user experience across various platforms, ensuring users can efficiently manage and edit markdown files with ease.
 
 ---
-![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
+
+![Notolog UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
 
 
 ## Features
 
 * Notolog is open-sourced under the MIT license, promoting full transparency and encouraging collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
@@ -231,15 +235,15 @@
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to [open an issue](https://github.com/notolog/notolog-editor/issues) or submit a [pull request](https://github.com/notolog/notolog-editor/pulls) on the project's [GitHub page](https://github.com/notolog/notolog-editor).
 
 ## License
 
-The Notolog project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+The Notolog project is licensed under the MIT License - see the [LICENSE](https://github.com/notolog/notolog-editor/blob/main/LICENSE) file for details.
 
 ## Third-Party Components
 
 ### Libraries and Licenses
 
 This project utilizes numerous third-party libraries, each with its own licensing terms. Below is a detailed list of these libraries grouped by license type to help clarify what each license permits and requires. This categorization aids in ensuring compliance with legal terms for use, modification, and distribution of these software components.
 
@@ -266,14 +270,18 @@
 - **Python-Markdown**: Markdown to HTML conversion. [Project Details](https://python-markdown.github.io/), [BSD 3-Clause License](https://github.com/Python-Markdown/markdown/blob/master/LICENSE.md)
 - **Emoji library**: Converts emoji text-code to emojis. [New BSD License](https://github.com/carpedm20/emoji/blob/master/LICENSE.txt), [PyPI](https://pypi.org/project/emoji/)
 - **qasync**: Async support for Python. [BSD 2-Clause "Simplified" License](https://github.com/CabbageDevelopment/qasync/blob/master/LICENSE), [PyPI](https://pypi.org/project/qasync/)
 - **Pygments**: Syntax highlighting for programming languages. [Project Details](https://pygments.org/), [BSD 2-Clause "Simplified" License](https://github.com/pygments/pygments/blob/master/LICENSE)
 - **click**: Used for creating command-line interfaces. [Project Details](https://palletsprojects.com/p/click/), [BSD-3-Clause License](https://click.palletsprojects.com/en/8.1.x/license/)
 - **pycparser**: C code parser and for generating Abstract Syntax Trees (AST) in Python. [BSD 3-Clause License](https://github.com/eliben/pycparser/blob/main/LICENSE), [PyPI](https://pypi.org/project/pycparser/)
 
+#### Apache License 2.0
+
+- **pytest-asyncio**: A library that provides support for testing asyncio code with pytest. [License Details](https://github.com/pytest-dev/pytest-asyncio/blob/main/LICENSE) , [PyPI](https://pypi.org/project/pytest-asyncio/)
+
 #### Other Dual Licensed
 
 - **cryptography**: Provides cryptographic functions and primitives. [Apache License 2.0](https://github.com/pyca/cryptography/blob/main/LICENSE.APACHE) and [BSD 3-Clause License](https://github.com/pyca/cryptography/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/cryptography/)
 - **packaging**: Python package metadata and distribution utilities. [Apache License 2.0](https://github.com/pypa/packaging/blob/main/LICENSE.APACHE) and [BSD 2-Clause "Simplified" License](https://github.com/pypa/packaging/blob/main/LICENSE.BSD), [PyPI](https://pypi.org/project/packaging/)
 
 #### Python Standard Library
```

### Comparing `notolog-0.9.1b3/notolog.egg-info/SOURCES.txt` & `notolog-0.9.1b4/notolog.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -301,11 +301,13 @@
 tests/test_enc_helper.py
 tests/test_enc_password.py
 tests/test_file_header.py
 tests/test_html_view.py
 tests/test_lexemes.py
 tests/test_notolog_editor.py
 tests/test_pkg_integration.py
+tests/test_qt_async.py
+tests/test_qt_ui.py
 tests/test_settings.py
 tests/test_text_block_data.py
 tests/test_theme_helper.py
 tests/test_themes.py
```

### Comparing `notolog-0.9.1b3/setup.py` & `notolog-0.9.1b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.1b3',
+    version='0.9.1b4',
     description='Notolog - Python Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
     license='MIT',
     # py_modules=['main'],  # This refers to the standalone 'main.py' at the top-level directory
```

### Comparing `notolog-0.9.1b3/tests/test_enc_helper.py` & `notolog-0.9.1b4/tests/test_enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_enc_password.py` & `notolog-0.9.1b4/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_file_header.py` & `notolog-0.9.1b4/tests/test_file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_html_view.py` & `notolog-0.9.1b4/tests/test_html_view.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_lexemes.py` & `notolog-0.9.1b4/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_notolog_editor.py` & `notolog-0.9.1b4/tests/test_notolog_editor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_pkg_integration.py` & `notolog-0.9.1b4/tests/test_qt_ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,77 @@
 from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QApplication  # Sync with main.py
+from PySide6.QtWidgets import QApplication
 from PySide6.QtTest import QTest
 
 from notolog.notolog_editor import NotologEditor
+from notolog.enums.languages import Languages
+from notolog.settings import Settings
 
 import os
 import sys
 import pytest
 
 
-@pytest.fixture(scope="session")
-def qt_application():
-    # Force Qt style override
-    """
-    QApplication: invalid style override 'kvantum' passed, ignoring it.
-        Available styles: Windows, Fusion
-    """
-    os.environ["QT_STYLE_OVERRIDE"] = "Fusion"
-    # Fixture to initialize QApplication.
-    return QApplication(sys.argv)
-
-
-@pytest.fixture
-def main_window(qt_application):
-    # Fixture to create and return main window instance
-    window = NotologEditor(screen=qt_application.screens()[0])
-    yield window
-
-
-def test_editor_state(main_window):
-    # Check default window title
-    assert main_window.windowTitle() == "Notolog Editor"
-
-    assert main_window.statusbar['mode_label'].text() == 'View mode'
-    assert main_window.statusbar['source_label'].text() == 'HTML'
-    assert main_window.statusbar['encryption_label'].text() == 'Plain 🔓'
-
-    # Test that clicking the edit button updates the editor state
-    QTest.mouseClick(main_window.toolbar.toolbar_edit_button, Qt.MouseButton.LeftButton)
-
-    assert main_window.statusbar['mode_label'].text() == 'Edit mode'
-    assert main_window.statusbar['source_label'].text() == 'Markdown'
-    assert main_window.statusbar['encryption_label'].text() == 'Plain 🔓'
-
-
-def test_search_elements(main_window):
-    assert hasattr(main_window.toolbar, 'search_input')
-    main_window.toolbar.search_input.setText('Test search')
-    assert main_window.toolbar.search_input.text() == 'Test search'
-
-    assert hasattr(main_window.toolbar, 'btn_search_clear')
-    # Test that clicking the button updates the search field
-    QTest.mouseClick(main_window.toolbar.btn_search_clear, Qt.MouseButton.LeftButton)
-    assert main_window.toolbar.search_input.text() == ''
+class TestQtUi:
 
+    @pytest.fixture(autouse=True, scope="session")
+    def qt_app(self):
+        # Check to avoid:
+        # RuntimeError: Please destroy the QApplication singleton before creating a new QApplication instance.
+        app = QApplication.instance()
+        if not app:
+            # Force Qt style override
+            """
+            QApplication: invalid style override 'kvantum' passed, ignoring it.
+                Available styles: Windows, Fusion
+            """
+            os.environ["QT_STYLE_OVERRIDE"] = "Fusion"
+            # Fixture to initialize QApplication.
+            app = QApplication(sys.argv)
+
+        yield app
+
+        # Properly close the QApplication after each test
+        app.quit()
+
+    @pytest.fixture
+    def settings_obj(self, qt_app):
+        # Fixture to create and return settings instance
+        settings = Settings()
+        yield settings
+
+    @pytest.fixture
+    def main_window(self, mocker, qt_app):
+        # Force to override system language as a default
+        mocker.patch.object(Languages, 'default', return_value='la')
+
+        # Fixture to create and return main window instance
+        window = NotologEditor(screen=qt_app.screens()[0])
+        yield window
+
+    def test_editor_state(self, main_window, settings_obj):
+        # Check app language set correctly
+        assert settings_obj.app_language == 'la'
+
+        # Check default window title
+        assert main_window.windowTitle() == "Editorium Notolog"
+
+        assert main_window.statusbar['mode_label'].text() == 'Modus Visum'
+        assert main_window.statusbar['source_label'].text() == 'HTML'
+        assert main_window.statusbar['encryption_label'].text() == 'Simplicitas 🔓'
+
+        # Test that clicking the edit button updates the editor state
+        QTest.mouseClick(main_window.toolbar.toolbar_edit_button, Qt.MouseButton.LeftButton)
+
+        assert main_window.statusbar['mode_label'].text() == 'Modus Editio'
+        assert main_window.statusbar['source_label'].text() == 'Markdown'
+        assert main_window.statusbar['encryption_label'].text() == 'Simplicitas 🔓'
+
+    def test_search_elements(self, main_window):
+        assert hasattr(main_window.toolbar, 'search_input')
+        main_window.toolbar.search_input.setText('Test search')
+        assert main_window.toolbar.search_input.text() == 'Test search'
+
+        assert hasattr(main_window.toolbar, 'btn_search_clear')
+        # Test that clicking the button updates the search field
+        QTest.mouseClick(main_window.toolbar.btn_search_clear, Qt.MouseButton.LeftButton)
+        assert main_window.toolbar.search_input.text() == ''
```

### Comparing `notolog-0.9.1b3/tests/test_settings.py` & `notolog-0.9.1b4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_text_block_data.py` & `notolog-0.9.1b4/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_theme_helper.py` & `notolog-0.9.1b4/tests/test_theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b3/tests/test_themes.py` & `notolog-0.9.1b4/tests/test_themes.py`

 * *Files identical despite different names*

