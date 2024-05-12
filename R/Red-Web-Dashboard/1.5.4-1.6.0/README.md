# Comparing `tmp/red_web_dashboard-1.5.4.tar.gz` & `tmp/red_web_dashboard-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_web_dashboard-1.5.4.tar", last modified: Thu May  9 14:12:24 2024, max compression
+gzip compressed data, was "red_web_dashboard-1.6.0.tar", last modified: Sun May 12 17:17:10 2024, max compression
```

## Comparing `red_web_dashboard-1.5.4.tar` & `red_web_dashboard-1.6.0.tar`

### file list

```diff
@@ -1,293 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-09 14:12:24.000000 red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-05-09 14:12:24.000000 red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:12:24.000000 red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 14:12:24.000000 red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-09 14:12:24.000000 red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 14:12:24.000000 red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.061797 red_web_dashboard-1.5.4/reddash/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.061797 red_web_dashboard-1.5.4/reddash/app/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.061797 red_web_dashboard-1.5.4/reddash/app/base/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/base/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.065797 red_web_dashboard-1.5.4/reddash/app/login/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/login/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.057797 red_web_dashboard-1.5.4/reddash/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.069797 red_web_dashboard-1.5.4/reddash/app/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/biometric-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.073797 red_web_dashboard-1.5.4/reddash/app/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   480516 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/css/argon-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/css/argon-dashboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/css/argon-dashboard.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/css/nucleo-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/css/nucleo-svg.css
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/css/simplemde.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/error-403.gif
--rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/error-404.gif
--rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/error-500.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.073797 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.eot
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/icon-documentation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.077797 red_web_dashboard-1.5.4/reddash/app/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    27144 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/argon-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/argon-dashboard.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.077797 red_web_dashboard-1.5.4/reddash/app/static/assets/js/core/
--rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/core/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/core/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/core/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.077797 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/Chart.extension.js
--rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/chartjs.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/oauth.png
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/random.svg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.077797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.085797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.093797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.093797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.097797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.101797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.101797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.101797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.101797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.101797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.101797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.105797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.057797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.105797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.109797 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/tasks_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.109797 red_web_dashboard-1.5.4/reddash/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.109797 red_web_dashboard-1.5.4/reddash/app/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/errors/blacklisted.html
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/errors/custom.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.109797 red_web_dashboard-1.5.4/reddash/app/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/includes/fixed-plugin.html
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/includes/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/includes/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/includes/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/reddash/app/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/layouts/base-fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/layouts/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/reddash/app/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/credits.html
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    30733 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/dashboard_guild.html
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/guild_profile.html
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/reddash/app/templates/pages/login/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/login/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/third_parties.html
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/third_parties_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/third_party.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:24.113797 red_web_dashboard-1.5.4/reddash/app/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14080 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/third_parties/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    27042 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/reddash/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-09 14:12:24.117797 red_web_dashboard-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 14:12:16.000000 red_web_dashboard-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.196249 red_web_dashboard-1.6.0/reddash/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.196249 red_web_dashboard-1.6.0/reddash/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.200249 red_web_dashboard-1.6.0/reddash/app/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/base/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.200249 red_web_dashboard-1.6.0/reddash/app/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/login/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.192249 red_web_dashboard-1.6.0/reddash/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.204249 red_web_dashboard-1.6.0/reddash/app/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/biometric-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.208249 red_web_dashboard-1.6.0/reddash/app/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   480562 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-svg.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/simplemde.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.208249 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/background_theme_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/background_theme_white.css
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/sidenav_theme_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/sidenav_theme_white.css
+-rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/error-403.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/error-404.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/error-500.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.212249 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/icon-documentation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.212249 red_web_dashboard-1.6.0/reddash/app/static/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.212249 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.216249 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Chart.extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/chartjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/oauth.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/random.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.216249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.220249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.228249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.232249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.232249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.192249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/tasks_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/blacklisted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/custom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/fixed-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/layouts/base-fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/layouts/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    29579 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/credits.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30814 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/dashboard_guild.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/guild_profile.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/reddash/app/templates/pages/login/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/login/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_parties.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_parties_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_party.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/reddash/app/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/third_parties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/third_parties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27042 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/setup.py
```

### Comparing `red_web_dashboard-1.5.4/LICENSE` & `red_web_dashboard-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/PKG-INFO` & `red_web_dashboard-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.5.4
+Version: 1.6.0
 Summary: An easy-to-use interactive web Dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.5.4/README.md` & `red_web_dashboard-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/PKG-INFO` & `red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.5.4
+Version: 1.6.0
 Summary: An easy-to-use interactive web Dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.5.4/Red_Web_Dashboard.egg-info/SOURCES.txt` & `red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 reddash/app/static/assets/robots.txt
 reddash/app/static/assets/css/argon-dashboard.css
 reddash/app/static/assets/css/argon-dashboard.css.map
 reddash/app/static/assets/css/argon-dashboard.min.css
 reddash/app/static/assets/css/nucleo-icons.css
 reddash/app/static/assets/css/nucleo-svg.css
 reddash/app/static/assets/css/simplemde.min.css
+reddash/app/static/assets/css/themes/background_theme_dark.css
+reddash/app/static/assets/css/themes/background_theme_white.css
+reddash/app/static/assets/css/themes/sidenav_theme_dark.css
+reddash/app/static/assets/css/themes/sidenav_theme_white.css
 reddash/app/static/assets/fonts/nucleo-icons.eot
 reddash/app/static/assets/fonts/nucleo-icons.svg
 reddash/app/static/assets/fonts/nucleo-icons.ttf
 reddash/app/static/assets/fonts/nucleo-icons.woff
 reddash/app/static/assets/fonts/nucleo-icons.woff2
 reddash/app/static/assets/fonts/nucleo.eot
 reddash/app/static/assets/fonts/nucleo.ttf
```

### Comparing `red_web_dashboard-1.5.4/pyproject.toml` & `red_web_dashboard-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/__main__.py` & `red_web_dashboard-1.6.0/reddash/__main__.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/app.py` & `red_web_dashboard-1.6.0/reddash/app/app.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/base/routes.py` & `red_web_dashboard-1.6.0/reddash/app/base/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,30 +42,30 @@
 @blueprint.route("/")
 async def index():
     return render_template("pages/index.html")
 
 
 @blueprint.route("/setcolor", methods=("POST",))
 async def set_color():
-    resp = make_response(jsonify({"status": 1}))
+    resp = make_response(jsonify({"status": 0}))
     color = request.json.get("color")
     if color is not None and color != app.data["ui"]["meta"]["default_color"]:
         resp.set_cookie(
             key="color",
             value=color,
             expires=datetime.datetime.now(tz=datetime.timezone.utc) + datetime.timedelta(days=365),
         )
     else:
         resp.delete_cookie("color")
     return resp
 
 
 @blueprint.route("/setbackgroundtheme", methods=("POST",))
 async def set_background_theme():
-    resp = make_response(jsonify({"status": 1}))
+    resp = make_response(jsonify({"status": 0}))
     background_theme = request.json.get("background_theme")
     if (
         background_theme is not None
         and background_theme != app.data["ui"]["meta"]["default_background_theme"]
     ):
         resp.set_cookie(
             key="background_theme",
@@ -73,29 +73,29 @@
             expires=datetime.datetime.now(tz=datetime.timezone.utc) + datetime.timedelta(days=365),
         )
     else:
         resp.delete_cookie("background_theme")
     return resp
 
 
-@blueprint.route("/setsidebartheme", methods=("POST",))
-async def set_sidebar_theme():
+@blueprint.route("/setsidenavtheme", methods=("POST",))
+async def set_sidenav_theme():
     resp = make_response(jsonify({"status": 1}))
-    sidebar_theme = request.json.get("sidebar_theme")
+    sidenav_theme = request.json.get("sidenav_theme")
     if (
-        sidebar_theme is not None
-        and sidebar_theme != app.data["ui"]["meta"]["default_sidebar_theme"]
+        sidenav_theme is not None
+        and sidenav_theme != app.data["ui"]["meta"]["default_sidenav_theme"]
     ):
         resp.set_cookie(
-            key="sidebar_theme",
-            value=sidebar_theme,
+            key="sidenav_theme",
+            value=sidenav_theme,
             expires=datetime.datetime.now(tz=datetime.timezone.utc) + datetime.timedelta(days=365),
         )
     else:
-        resp.delete_cookie("sidebar_theme")
+        resp.delete_cookie("sidenav_theme")
     return resp
 
 
 @blueprint.route("/sitemap.xml")
 async def sitemap():
     return app.site_mapper.generate()
 
@@ -697,15 +697,15 @@
         self.title.default = settings["title"]
         self.icon.default = settings["icon"]
         self.website_description.default = settings["website_description"]
         self.description.default = settings["description"]
         self.support_server.default = settings["support_server"]
         self.default_color.default = settings["default_color"]
         self.default_background_theme.default = settings["default_background_theme"]
-        self.default_sidebar_theme.default = settings["default_sidebar_theme"]
+        self.default_sidenav_theme.default = settings["default_sidenav_theme"]
         self.disabled_third_parties.choices = [
             (third_party, third_party) for third_party in app.variables["third_parties"]
         ]
         self.disabled_third_parties.default = settings["disabled_third_parties"].copy()
 
     title: wtforms.StringField = wtforms.StringField(_("Title:"))
     icon: wtforms.StringField = wtforms.StringField(_("Icon:"))
@@ -715,20 +715,20 @@
     default_color: wtforms.SelectField = wtforms.SelectField(
         _("Default Color:"),
         choices=[(color, color.capitalize()) for color in AVAILABLE_COLORS],
         validators=[wtforms.validators.InputRequired()],
     )
     default_background_theme: wtforms.SelectField = wtforms.SelectField(
         _("Default Background Theme:"),
-        choices=[("light", "Light"), ("dark", "Dark")],
+        choices=[("white", "White"), ("dark", "Dark")],
         validators=[wtforms.validators.InputRequired()],
     )
-    default_sidebar_theme: wtforms.SelectField = wtforms.SelectField(
-        _("Default Sidebar Theme:"),
-        choices=[("light", "Light"), ("dark", "Dark")],
+    default_sidenav_theme: wtforms.SelectField = wtforms.SelectField(
+        _("Default Sidenav Theme:"),
+        choices=[("white", "White"), ("dark", "Dark")],
         validators=[wtforms.validators.InputRequired()],
     )
     disabled_third_parties: wtforms.SelectMultipleField = wtforms.SelectMultipleField(
         _("Disabled Third Parties:"), choices=[]
     )
     submit: wtforms.SubmitField = wtforms.SubmitField(_("Save Modifications"))
 
@@ -890,15 +890,15 @@
             "title": dashboard_settings_form.title.data.strip() or None,
             "icon": dashboard_settings_form.icon.data.strip() or None,
             "website_description": dashboard_settings_form.website_description.data.strip() or None,
             "description": dashboard_settings_form.description.data.strip() or None,
             "support_server": dashboard_settings_form.support_server.data.strip() or None,
             "default_color": dashboard_settings_form.default_color.data,
             "default_background_theme": dashboard_settings_form.default_background_theme.data,
-            "default_sidebar_theme": dashboard_settings_form.default_sidebar_theme.data,
+            "default_sidenav_theme": dashboard_settings_form.default_sidenav_theme.data,
             "disabled_third_parties": dashboard_settings_form.disabled_third_parties.data,
         }
         requeststr = {
             "jsonrpc": "2.0",
             "id": 0,
             "method": "DASHBOARDRPC__SET_DASHBOARD_SETTINGS",
             "params": [
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/login/routes.py` & `red_web_dashboard-1.6.0/reddash/app/login/routes.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/pagination.py` & `red_web_dashboard-1.6.0/reddash/app/pagination.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/biometric-icon.svg` & `red_web_dashboard-1.6.0/reddash/app/static/assets/biometric-icon.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/css/argon-dashboard.css` & `red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 }
 
 h6, .h6, h5, .h5, h4, .h4, h3, .h3, h2, .h2, h1, .h1 {
   margin-top: 0;
   margin-bottom: 0.5rem;
   font-weight: 400;
   line-height: 1.2;
-  color: var(--bs-heading-color);
+  /* color: var(--bs-heading-color); */
 }
 
 h1, .h1 {
   font-size: calc(1.425rem + 2.1vw);
 }
 @media (min-width: 1200px) {
   h1, .h1 {
@@ -2113,15 +2113,15 @@
   --bs-table-striped-bg: rgba(0, 0, 0, 0.05);
   --bs-table-active-color: #67748e;
   --bs-table-active-bg: rgba(0, 0, 0, 0.1);
   --bs-table-hover-color: #67748e;
   --bs-table-hover-bg: rgba(0, 0, 0, 0.075);
   width: 100%;
   margin-bottom: 1rem;
-  color: var(--bs-table-color);
+  /* color: var(--bs-table-color); */
   vertical-align: top;
   border-color: var(--bs-table-border-color);
 }
 .table > :not(caption) > * > * {
   padding: 0.5rem 0.5rem;
   background-color: var(--bs-table-bg);
   border-bottom-width: 1px;
@@ -2327,15 +2327,15 @@
     -webkit-overflow-scrolling: touch;
   }
 }
 .form-label {
   margin-bottom: 0.5rem;
   font-size: 0.75rem;
   font-weight: 700;
-  color: #344767;
+  /* color: #344767; */
 }
 
 .col-form-label {
   padding-top: calc(0.5rem + 1px);
   padding-bottom: calc(0.5rem + 1px);
   margin-bottom: 0;
   font-size: inherit;
@@ -18335,15 +18335,15 @@
 }
 
 label,
 .form-label {
   font-size: 0.75rem;
   font-weight: 700;
   margin-bottom: 0.5rem;
-  color: #344767;
+  /* color: #344767; */
   margin-left: 0.25rem;
 }
 
 .form-control.is-invalid:focus {
   box-shadow: 0 0 0 2px rgba(253, 92, 112, 0.6);
 }
 .form-control.is-valid:focus {
@@ -20130,14 +20130,15 @@
     height: auto;
   }
 }
 .nav.nav-pills {
   background: #f8f9fa;
   border-radius: 0.75rem;
   position: relative;
+  width: fit-content;
 }
 .nav.nav-pills.nav-pills-vertical {
   border-radius: 1.1875rem;
 }
 .nav.nav-pills.nav-pills-vertical .nav-link.active {
   border-radius: 0.875rem;
 }
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/css/argon-dashboard.css.map` & `red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/css/argon-dashboard.min.css` & `red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/css/nucleo-icons.css` & `red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/css/nucleo-svg.css` & `red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-svg.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/css/simplemde.min.css` & `red_web_dashboard-1.6.0/reddash/app/static/assets/css/simplemde.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/error-403.gif` & `red_web_dashboard-1.6.0/reddash/app/static/assets/error-403.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/error-404.gif` & `red_web_dashboard-1.6.0/reddash/app/static/assets/error-404.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/error-500.gif` & `red_web_dashboard-1.6.0/reddash/app/static/assets/error-500.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.eot` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.svg` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.ttf` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.woff` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo-icons.woff2` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.eot` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.ttf` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.woff` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/fonts/nucleo.woff2` & `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/gulpfile.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/gulpfile.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/icon-documentation.svg` & `red_web_dashboard-1.6.0/reddash/app/static/assets/icon-documentation.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/argon-dashboard.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,35 @@
 "use strict";
 (function() {
-    let isWindows = navigator.platform.indexOf("Win") > -1 ? true : false;
+    let isWindows = !!(navigator.platform.indexOf("Win") > -1);
     if (isWindows) {
         // If we are on windows OS we activate the perfectScrollbar function.
         // if (document.getElementsByClassName('main-content')[0]) {
         //   let mainpanel = document.querySelector('.main-content');
         //   let ps = new PerfectScrollbar(mainpanel);
         // };
         let sidebar = document.querySelector(".sidenav");
         if (sidebar) {
-            let ps1 = new PerfectScrollbar(sidebar);
+            new PerfectScrollbar(sidebar);
         };
         let fixedplugin = document.querySelector(".navbar:not(.navbar-expand-lg) .navbar-collapse");
         if (fixedplugin) {
-            let ps2 = new PerfectScrollbar(fixedplugin);
+            new PerfectScrollbar(fixedplugin);
         };
         let fixedplugin2 = document.querySelector(".fixed-plugin");
         if (fixedplugin) {
-            let ps3 = new PerfectScrollbar(fixedplugin2);
+            new PerfectScrollbar(fixedplugin2);
         };
+        let scrollbar = document.querySelector("#sidenav-scrollbar");
+        if (scrollbar) {
+            let options = {
+                damping: "0.5"
+            }
+            Scrollbar.init(scrollbar, options);
+        }
     };
 })();
 
 // Verify navbar blur on scroll.
 if (document.getElementById("navbarBlur")) {
     navbarBlurOnScroll("navbarBlur");
 }
@@ -108,233 +115,149 @@
 
     if (navbar && (navbar.getAttribute("data-scroll") == 'true' && buttonNavbarFixed)) {
         buttonNavbarFixed.setAttribute("checked", "true");
     }
 
 }
 
-//Set Sidebar Color.
-function sidebarColor(a) {
+// Set Sidenav Color.
+function sidenavColor(a) {
     let parent = a.parentElement.children;
     let color = a.getAttribute("data-color");
-
-    let colors = [];
+    let oldColor = null;
     for (let i = 0; i < parent.length; i++) {
+        if (parent[i].classList.contains("active")) {
+            oldColor = parent[i].getAttribute("data-color");
+        }
         parent[i].classList.remove("active");
-        colors.push(parent[i].getAttribute("data-color"));
     }
-
     if (!a.classList.contains("active")) {
         a.classList.add("active");
     } else {
         a.classList.remove("active");
     }
-
-    let oldColor = null;
-    let sidebar = document.querySelector(".sidenav");
-    if (sidebar) {
-        oldColor = sidebar.getAttribute("data-color");
-    }
-    if (oldColor == null) {
-        oldColor = "success"
-    }
-    sidebar.setAttribute("data-color", color);
-
     let background = document.querySelector(".min-height-300");
-    // for (let i = 0; i < colors.length; i++) {
-    //   background.classList.remove("bg-gradient-" + colors[i]);
-    // }
     background.classList.remove("bg-gradient-" + oldColor);
     background.classList.add("bg-gradient-" + color);
-
-    // if (document.querySelector("#sidenavCard")) {
-    //   let sidenavCard = document.querySelector("#sidenavCard+.btn+.btn");
-    //   let sidenavCardClasses = ["btn", "btn-sm", "w-100", "mb-0", "bg-gradient-" + color];
-    //   sidenavCard.removeAttribute("class");
-    //   sidenavCard.classList.add(...sidenavCardClasses);
-    // }
     let buttons = document.querySelectorAll(".btn.bg-gradient-" + oldColor);
     for (let i = 0; i < buttons.length; i++) {
-        // for (let i = 0; i < colors.length; i++) {
-        //   buttons[j].classList.remove("bg-gradient-" + colors[i]);
-        // }
         if (buttons[i].tagName == "button") {
             continue
         }
         buttons[i].classList.remove("bg-gradient-" + oldColor);
         buttons[i].classList.add("bg-gradient-" + color);
     }
 }
 
-// Set Sidebar Type.
-function sidebarType(a) {
-    let parent = a.parentElement.children;
-    let color = a.getAttribute("data-class");
-    let body = document.querySelector("body");
-    let bodyWhite = document.querySelector("body:not(.dark-version)");
-    let bodyDark = body.classList.contains("dark-version");
-
-    let colors = [];
-    for (let i = 0; i < parent.length; i++) {
-        parent[i].classList.remove('active');
-        colors.push(parent[i].getAttribute('data-class'));
-    }
-
-    if (!a.classList.contains('active')) {
-        a.classList.add('active');
+// Set Background Theme.
+function backgroundTheme(a) {
+    let theme = a.checked ? "dark" : "white";
+    document.querySelector("#background_theme").href = "/static/assets/css/themes/background_theme_" + theme + ".css";
+    if (theme === "dark") {
+        document.querySelector("#sidenav-theme-select").children[1].click();
     } else {
-        a.classList.remove('active');
-    }
-
-    let sidebar = document.querySelector('.sidenav');
-
-    if (sidebar) {
-        for (let i = 0; i < colors.length; i++) {
-            sidebar.classList.remove(colors[i]);
-        }
-        sidebar.classList.add(color);
-    }
-
-    // Remove text-white/text-dark classes.
-    if (color == 'bg-white') {
-        let textWhites = document.querySelectorAll('.sidenav .text-white');
-        for (let i = 0; i < textWhites.length; i++) {
-            textWhites[i].classList.remove('text-white');
-            textWhites[i].classList.add('text-dark');
-        }
-    } else {
-        let textDarks = document.querySelectorAll('.sidenav .text-dark');
-        for (let i = 0; i < textDarks.length; i++) {
-            textDarks[i].classList.add('text-white');
-            textDarks[i].classList.remove('text-dark');
-        }
+        document.querySelector("#sidenav-theme-select").children[0].click();
     }
+}
 
-    if (color == 'bg-default' && bodyDark) {
-        let textDarks = document.querySelectorAll('.navbar-brand .text-dark');
-        for (let i = 0; i < textDarks.length; i++) {
-            textDarks[i].classList.add('text-white');
-            textDarks[i].classList.remove('text-dark');
-        }
+// Set Sidenav Theme.
+function sidenavTheme(a) {
+    let parent = a.parentElement.children;
+    let theme = a.getAttribute("data-class");
+    let themes = [];
+    for (let i = 0; i < parent.length; i++) {
+        parent[i].classList.remove("active");
+        themes.push(parent[i].getAttribute("data-class"));
     }
-
-    // Remove logo-white/logo-dark.
-
-    if ((color == 'bg-white') && bodyWhite) {
-        let navbarBrand = document.querySelector('.navbar-brand-img');
-        let navbarBrandImg = navbarBrand.src;
-
-        if (navbarBrandImg.includes('logo-ct.png')) {
-            let navbarBrandImgNew = navbarBrandImg.replace("logo-ct", "logo-ct-dark");
-            navbarBrand.src = navbarBrandImgNew;
-        }
+    if (!a.classList.contains("active")) {
+        a.classList.add("active");
     } else {
-        let navbarBrand = document.querySelector('.navbar-brand-img');
-        let navbarBrandImg = navbarBrand.src;
-        if (navbarBrandImg.includes('logo-ct-dark.png')) {
-            let navbarBrandImgNew = navbarBrandImg.replace("logo-ct-dark", "logo-ct");
-            navbarBrand.src = navbarBrandImgNew;
-        }
-    }
-
-    if (color == 'bg-white' && bodyDark) {
-        let navbarBrand = document.querySelector('.navbar-brand-img');
-        let navbarBrandImg = navbarBrand.src;
-
-        if (navbarBrandImg.includes('logo-ct.png')) {
-            let navbarBrandImgNew = navbarBrandImg.replace("logo-ct", "logo-ct-dark");
-            navbarBrand.src = navbarBrandImgNew;
-        }
+        a.classList.remove("active");
     }
+    document.querySelector("#sidenav_theme").href = "/static/assets/css/themes/sidenav_theme_" + theme + ".css";
 }
 
 // Set Navbar Fixed.
 function navbarFixed(el) {
-    let classes = ['position-sticky', 'bg-white', 'left-auto', 'top-2', 'z-index-sticky'];
-    let navbar = document.getElementById('navbarBlur');
-
+    let classes = ["position-sticky", "bg-white", "left-auto", "top-2", "z-index-sticky"];
+    let navbar = document.getElementById("navbarBlur");
     if (!el.getAttribute("checked")) {
-        toggleNavLinksColor('blur');
+        toggleNavLinksColor("blur");
         navbar.classList.add(...classes);
-        navbar.setAttribute('data-scroll', 'true');
-        navbarBlurOnScroll('navbarBlur');
+        navbar.setAttribute("data-scroll", "true");
+        navbarBlurOnScroll("navbarBlur");
         el.setAttribute("checked", "true");
     } else {
-        toggleNavLinksColor('transparent');
+        toggleNavLinksColor("transparent");
         navbar.classList.remove(...classes);
-        navbar.setAttribute('data-scroll', 'false');
-        navbarBlurOnScroll('navbarBlur');
+        navbar.setAttribute("data-scroll", "false");
+        navbarBlurOnScroll("navbarBlur");
         el.removeAttribute("checked");
     }
 };
 
 // Set Navbar Minimized.
 function navbarMinimize(el) {
-    let sidenavShow = document.getElementsByClassName('g-sidenav-show')[0];
-
+    let sidenavShow = document.getElementsByClassName("g-sidenav-show")[0];
     if (!el.getAttribute("checked")) {
-        sidenavShow.classList.remove('g-sidenav-pinned');
-        sidenavShow.classList.add('g-sidenav-hidden');
+        sidenavShow.classList.remove("g-sidenav-pinned");
+        sidenavShow.classList.add("g-sidenav-hidden");
         el.setAttribute("checked", "true");
     } else {
-        sidenavShow.classList.remove('g-sidenav-hidden');
-        sidenavShow.classList.add('g-sidenav-pinned');
+        sidenavShow.classList.remove("g-sidenav-hidden");
+        sidenavShow.classList.add("g-sidenav-pinned");
         el.removeAttribute("checked");
     }
 }
 
 function toggleNavLinksColor(type) {
-    let navLinks = document.querySelectorAll('.navbar-main .nav-link, .navbar-main .breadcrumb-item, .navbar-main .breadcrumb-item a, .navbar-main h6')
-    let navLinksToggler = document.querySelectorAll('.navbar-main .sidenav-toggler-line')
-
+    let navLinks = document.querySelectorAll(".navbar-main .nav-link, .navbar-main .breadcrumb-item, .navbar-main .breadcrumb-item a, .navbar-main h6");
+    let navLinksToggler = document.querySelectorAll(".navbar-main .sidenav-toggler-line");
     if (type === "blur") {
         navLinks.forEach(element => {
-            element.classList.remove('text-white')
+            element.classList.remove("text-white");
         });
-
         navLinksToggler.forEach(element => {
-            element.classList.add('bg-dark')
-            element.classList.remove('bg-white')
+            element.classList.add("bg-dark");
+            element.classList.remove("bg-white");
         });
     } else if (type === "transparent") {
         navLinks.forEach(element => {
-            element.classList.add('text-white')
+            element.classList.add("text-white");
         });
-
         navLinksToggler.forEach(element => {
-            element.classList.remove('bg-dark')
-            element.classList.add('bg-white')
+            element.classList.remove("bg-dark");
+            element.classList.add("bg-white");
         });
     }
 }
 
-
 // Navbar blur on scroll.
 function navbarBlurOnScroll(id) {
     let navbar = document.getElementById(id);
     let navbarScrollActive = navbar ? navbar.getAttribute("data-scroll") : false;
     let scrollDistance = 5;
     let classes = ["bg-white", "left-auto", "position-sticky"];
     let toggleClasses = ["shadow-none"];
 
-    if (navbarScrollActive == 'true') {
+    if (navbarScrollActive == "true") {
         window.onscroll = debounce(function() {
             if (window.scrollY > scrollDistance) {
                 blurNavbar();
             } else {
                 transparentNavbar();
             }
         }, 10);
     } else {
         window.onscroll = debounce(function() {
             transparentNavbar();
         }, 10);
     }
 
-    let isWindows = navigator.platform.indexOf("Win") > -1 ? true : false;
+    let isWindows = !!(navigator.platform.indexOf("Win") > -1);
 
     if (isWindows) {
         let content = document.querySelector(".main-content");
         if (navbarScrollActive == "true") {
             content.addEventListener("ps-scroll-y", debounce(function() {
                 if (content.scrollTop > scrollDistance) {
                     blurNavbar();
@@ -356,15 +279,15 @@
         toggleNavLinksColor("blur");
     }
 
     function transparentNavbar() {
         navbar.classList.remove(...classes)
         navbar.classList.add(...toggleClasses)
 
-        toggleNavLinksColor('transparent');
+        toggleNavLinksColor("transparent");
     }
 }
 
 
 // Debounce Function
 // Returns a function, that, as long as it continues to be invoked, will not
 // be triggered. The function will be called after it stops being called for
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/argon-dashboard.js.map` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9942196531791907%*

 * *Differences: {"'names'": "{insert: [(0, 'sidenav'), (44, 'sidenavColor'), (55, 'sidenavType'), (127, "*

 * *            "'sidenavWhite')], delete: [127, 55, 44, 0]}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "mappings": "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",
     "names": [
-        "sidebar",
+        "sidenav",
         "fixedplugin",
         "navigator",
         "platform",
         "indexOf",
         "document",
         "getElementsByClassName",
         "mainpanel",
@@ -41,26 +41,26 @@
         "setAttributes",
         "options",
         "Object",
         "keys",
         "forEach",
         "attr",
         "setAttribute",
-        "sidebarColor",
+        "sidenavColor",
         "a",
         "parent",
         "children",
         "color",
         "getAttribute",
         "i",
         "length",
         "sidenavCardClasses",
         "sidenavCard",
         "removeAttribute",
-        "sidebarType",
+        "sidenavType",
         "body",
         "bodyWhite",
         "bodyDark",
         "colors",
         "push",
         "navbarBrand",
         "navbarBrandImg",
@@ -124,15 +124,15 @@
         "elements",
         "total",
         "getEventTarget",
         "event",
         "srcElement",
         "darkMode",
         "hr",
-        "sidebarWhite",
+        "sidenavWhite",
         "hr_card",
         "text_btn",
         "text_span",
         "text_span_white",
         "text_strong",
         "text_strong_white",
         "text_nav_link",
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/core/bootstrap.min.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/core/jquery.min.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/core/popper.min.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/Chart.extension.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Chart.extension.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/bootstrap-notify.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/chartjs.min.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/js/plugins/utils.js` & `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/utils.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/oauth.png` & `red_web_dashboard-1.6.0/reddash/app/static/assets/oauth.png`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/pdf.svg` & `red_web_dashboard-1.6.0/reddash/app/static/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/random.svg` & `red_web_dashboard-1.6.0/reddash/app/static/assets/random.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_cards.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_forms.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_header.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_misc.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_nav.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_tables.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_typography.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/_variables.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/theme.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/static/assets/scss/argon-dashboard.scss` & `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/tasks_manager.py` & `red_web_dashboard-1.6.0/reddash/app/tasks_manager.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/errors/403.html` & `red_web_dashboard-1.6.0/reddash/app/templates/errors/403.html`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                     {% if not error_message %}
                       <p>{{ _("Looks like you're not allowed to access to this page... Strange...") }}</p>
                     {% else %}
                       <p>{{ error_message }}</p>
                     {% endif %}
                     <img src="{{ config.ASSETS_ROOT }}/error-403.gif" height="250" />
                     <br /><br />
-                    <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
+                    <a class="btn bg-gradient-{{ variables["meta"]["color"] }} mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         </div>
       </div>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/errors/404.html` & `red_web_dashboard-1.6.0/reddash/app/templates/errors/404.html`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                     {% if not error_message %}
                     <p>{{ _("Looks like that page doesn't exist... Strange...") }}</p>
                     {% else %}
                       <p>{{ error_message }}</p>
                     {% endif %}
                     <img src="{{ config.ASSETS_ROOT }}/error-404.gif" height="250" />
                     <br /><br />
-                    <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
+                    <a class="btn bg-gradient-{{ variables["meta"]["color"] }} mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         </div>
       </div>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/errors/500.html` & `red_web_dashboard-1.6.0/reddash/app/templates/errors/500.html`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                     {% if not error_message %}
                       <p>{{ _("Looks like the server ran into an issue... Strange...") }}</p>
                     {% else %}
                       <p>{{ error_message }}</p>
                     {% endif %}
                     <img src="{{ config.ASSETS_ROOT }}/error-500.gif" height="225" />
                     <br /><br />
-                    <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
+                    <a class="btn bg-gradient-{{ variables["meta"]["color"] }} mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         </div>
       </div>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/errors/blacklisted.html` & `red_web_dashboard-1.6.0/reddash/app/templates/errors/blacklisted.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/errors/custom.html` & `red_web_dashboard-1.6.0/reddash/app/templates/errors/custom.html`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 <div class="card-header">
                   <div class="card-body">
                     <h1><bold>{{ error_title }}</bold></h1>
                     {% if error_message %}
                       <p>{{ error_message }}</p>
                     {% endif %}
                     <br />
-                    <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
+                    <a class="btn bg-gradient-{{ variables["meta"]["color"] }} mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         </div>
       </div>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/includes/fixed-plugin.html` & `red_web_dashboard-1.6.0/reddash/app/templates/includes/fixed-plugin.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 <div class="fixed-plugin">
-  <!-- <a class="fixed-plugin-button text-dark position-fixed px-3 py-2"><i class="fa fa-cog py-2"></i></a> -->
+  <!-- <a class="fixed-plugin-button position-fixed px-3 py-2"><i class="fa fa-cog py-2"></i></a> -->
   <div class="card shadow-lg">
     <div class="card-header pb-0 pt-3">
       <div class="float-start">
         <h5 class="mt-3 mb-0">{{ _("Dashboard Configurator") }}</h5>
         <p>{{ _("Choose your custom options!") }}</p>
       </div>
       <div class="float-end mt-4">
-        <button class="btn btn-link text-dark p-0 fixed-plugin-close-button"><i class="fa fa-close"></i></button>
+        <button class="btn btn-link p-0 fixed-plugin-close-button"><i class="fa fa-close"></i></button>
       </div>
       <!-- End Toggle Button -->
     </div>
     <hr class="horizontal dark my-1" />
     <div class="card-body pt-sm-3 pt-0 overflow-auto">
       <!-- Theme Color -->
       <div>
         <h6 class="mb-0">{{ _("Theme Color") }}</h6>
       </div>
       <a href="javascript:void(0)" class="switch-trigger background-color" id="background-color-select">
         <div class="badge-colors my-2 text-start">
           {% for color in variables["meta"]["available_colors"] %}
-            <span class="badge filter bg-gradient-{{ color }} {% if color == variables["meta"]["color"] %}active{% endif %}" data-color="{{ color }}" onclick='sidebarColor(this); $.postData({"color": {% if color != variables["meta"]["default_color"] %}"{{ color }}"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_color") }}")'></span>
+            <span class="badge filter bg-gradient-{{ color }} {% if variables["meta"]["color"] == color %}active{% endif %}" data-color="{{ color }}" onclick='sidenavColor(this); $.postData({"color": {% if color != variables["meta"]["default_color"] %}"{{ color }}"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_color") }}")'></span>
           {% endfor %}
         </div>
       </a>
       <hr class="horizontal dark my-sm-4" />
-      <!-- Theme Light/Dark -->
+      <!-- Theme White/Dark -->
       <div class="mt-2 mb-5 d-flex">
-        <h6 class="mb-0">{{ _("Light / Dark") }}</h6>
+        <h6 class="mb-0">{{ _("White / Dark") }}</h6>
         <div class="form-check form-switch ps-0 ms-auto my-auto" id="background-theme-select">
-          <input class="form-check-input mt-1 ms-auto" type="checkbox" id="dark-version" onclick='darkMode(this); $.postData({"background_theme": this.getAttribute("checked") ? "dark" : "white"},"{{ url_for("base_blueprint.set_background_theme") }}");' />
+          <input class="form-check-input mt-1 ms-auto" type="checkbox" id="dark-version"{% if variables["meta"]["background_theme"] == "dark" %}checked="true"{% endif %} onclick='backgroundTheme(this); $.postData({"background_theme": this.checked ? "dark" : "white"},"{{ url_for("base_blueprint.set_background_theme") }}");' />
         </div>
       </div>
       <hr class="horizontal dark my-sm-4" />
       <!-- Sidenav Type -->
       <div class="mt-3">
         <h6 class="mb-0">{{ _("Sidenav Theme") }}</h6>
       </div>
-      <div class="d-flex" id="sidebar-theme-select">
-        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2 active" data-class="bg-white" onclick='sidebarType(this); $.postData({"sidebar_theme": {% if "white" != variables["meta"]["default_theme"] %}"white"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_sidebar_theme") }}")'>{{ _("White") }}</a>
-        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2" data-class="bg-default" onclick='sidebarType(this); $.postData({"sidebar_theme": {% if "dark" != variables["meta"]["default_theme"] %}"dark"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_sidebar_theme") }}")'>{{ _("Dark") }}</a>
+      <div class="d-flex" id="sidenav-theme-select">
+        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2 {% if variables["meta"]["sidenav_theme"] == "white" %}active{% endif %}" data-class="white" onclick='sidenavTheme(this); $.postData({"sidenav_theme": {% if variables["meta"]["default_theme"] != "white" %}"white"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_sidenav_theme") }}")'>{{ _("White") }}</a>
+        <a class="btn btn-outline-{{ variables["meta"]["color"] }} w-100 px-3 mb-2 me-2 {% if variables["meta"]["sidenav_theme"] == "dark" %}active{% endif %}" data-class="dark" onclick='sidenavTheme(this); $.postData({"sidenav_theme": {% if variables["meta"]["default_theme"] != "dark" %}"dark"{% else %}null{% endif %}},"{{ url_for("base_blueprint.set_sidenav_theme") }}")'>{{ _("Dark") }}</a>
       </div>
-      <p class="text-sm d-xl-none d-block mt-2">{{ _("You can change the sidenav theme just on desktop view.") }}</p>
+      <p class="text-sm d-xl-none d-block mt-2">{{ _("You can change the Sidenav theme just on desktop view.") }}</p>
       <!-- Navbar Fixed -->
       <div class="d-flex my-3">
         <h6 class="mb-0">{{ _("Navbar Fixed") }}</h6>
         <div class="form-check form-switch ps-0 ms-auto my-auto">
           <input class="form-check-input mt-1 ms-auto" type="checkbox" id="navbarFixed" onclick="navbarFixed(this)" />
         </div>
       </div>
```

#### html2text {}

```diff
@@ -1,26 +1,31 @@
 **** {{{{ __((""DDaasshhbbooaarrdd CCoonnffiigguurraattoorr"")) }}}} ****
 {{ _("Choose your custom options!") }}
 ===============================================================================
 ** {{{{ __((""TThheemmee CCoolloorr"")) }}}} **
 _{_%_ _f_o_r_ _c_o_l_o_r_ _i_n_ _v_a_r_i_a_b_l_e_s_[_"_m_e_t_a_"_]_[_"_a_v_a_i_l_a_b_l_e___c_o_l_o_r_s_"_]_ _%_}
-_}_a_c_t_i_v_e_{_%_ _e_n_d_i_f_ _%_}_"_ _d_a_t_a_-_c_o_l_o_r_=_"_{_{_ _c_o_l_o_r_ _}_}_"_ _o_n_c_l_i_c_k_=_'_s_i_d_e_b_a_r_C_o_l_o_r_(_t_h_i_s_)_;
-_$_._p_o_s_t_D_a_t_a_(_{_"_c_o_l_o_r_"_:_ _{_%_ _i_f_ _c_o_l_o_r_ _!_=_ _v_a_r_i_a_b_l_e_s_[_"_m_e_t_a_"_]_[_"_d_e_f_a_u_l_t___c_o_l_o_r_"_]_ _%_}_"_{
-_{_ _c_o_l_o_r_ _}_}_"_{_%_ _e_l_s_e_ _%_}_n_u_l_l_{_%_ _e_n_d_i_f_ _%_}_}_,_"_{_{_ _u_r_l___f_o_r_(_"_b_a_s_e___b_l_u_e_p_r_i_n_t_._s_e_t___c_o_l_o_r_"_)
-_}_}_"_)_'_>_ _{_%_ _e_n_d_f_o_r_ _%_}
+_=_ _c_o_l_o_r_ _%_}_a_c_t_i_v_e_{_%_ _e_n_d_i_f_ _%_}_"_ _d_a_t_a_-_c_o_l_o_r_=_"_{_{_ _c_o_l_o_r_ _}_}_"_ _o_n_c_l_i_c_k_=_'_s_i_d_e_n_a_v_C_o_l_o_r
+_(_t_h_i_s_)_;_ _$_._p_o_s_t_D_a_t_a_(_{_"_c_o_l_o_r_"_:_ _{_%_ _i_f_ _c_o_l_o_r_ _!_=_ _v_a_r_i_a_b_l_e_s_[_"_m_e_t_a_"_]_[_"_d_e_f_a_u_l_t___c_o_l_o_r_"_]
+_%_}_"_{_{_ _c_o_l_o_r_ _}_}_"_{_%_ _e_l_s_e_ _%_}_n_u_l_l_{_%_ _e_n_d_i_f_ _%_}_}_,_"_{_{_ _u_r_l___f_o_r
+_(_"_b_a_s_e___b_l_u_e_p_r_i_n_t_._s_e_t___c_o_l_o_r_"_)_ _}_}_"_)_'_>_ _{_%_ _e_n_d_f_o_r_ _%_}
 ===============================================================================
-** {{{{ __((""LLiigghhtt // DDaarrkk"")) }}}} **
-??
+** {{{{ __((""WWhhiittee // DDaarrkk"")) }}}} **
+% if variables["meta"]["background_theme"] == "dark" %}checked="true"{% endif
+%} onclick='backgroundTheme(this); $.postData({"background_theme": this.checked
+? "dark" : "white"},"{{ url_for("base_blueprint.set_background_theme") }}");' /
+>
 ===============================================================================
 ** {{{{ __((""SSiiddeennaavv TThheemmee"")) }}}} **
-} w-100 px-3 mb-2 me-2 active" data-class="bg-white" onclick='sidebarType
-(this); $.postData({"sidebar_theme": {% if "white" != variables["meta"]
-["default_theme"] %}"white"{% else %}null{% endif %}},"{{ url_for
-("base_blueprint.set_sidebar_theme") }}")'>{{ _("White") }}
+} w-100 px-3 mb-2 me-2 {% if variables["meta"]["sidenav_theme"] == "white"
+%}active{% endif %}" data-class="white" onclick='sidenavTheme(this); $.postData
+({"sidenav_theme": {% if variables["meta"]["default_theme"] != "white"
+%}"white"{% else %}null{% endif %}},"{{ url_for
+("base_blueprint.set_sidenav_theme") }}")'>{{ _("White") }}
 
-} w-100 px-3 mb-2 me-2" data-class="bg-default" onclick='sidebarType(this);
-$.postData({"sidebar_theme": {% if "dark" != variables["meta"]["default_theme"]
-%}"dark"{% else %}null{% endif %}},"{{ url_for
-("base_blueprint.set_sidebar_theme") }}")'>{{ _("Dark") }}
-{{ _("You can change the sidenav theme just on desktop view.") }}
+} w-100 px-3 mb-2 me-2 {% if variables["meta"]["sidenav_theme"] == "dark"
+%}active{% endif %}" data-class="dark" onclick='sidenavTheme(this); $.postData(
+{"sidenav_theme": {% if variables["meta"]["default_theme"] != "dark" %}"dark"{%
+else %}null{% endif %}},"{{ url_for("base_blueprint.set_sidenav_theme") }}")'>{
+{ _("Dark") }}
+{{ _("You can change the Sidenav theme just on desktop view.") }}
 ** {{{{ __((""NNaavvbbaarr FFiixxeedd"")) }}}} **
 ??
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/includes/footer.html` & `red_web_dashboard-1.6.0/reddash/app/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/includes/navigation.html` & `red_web_dashboard-1.6.0/reddash/app/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/includes/scripts.html` & `red_web_dashboard-1.6.0/reddash/app/templates/includes/scripts.html`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         "showMethod": "fadeIn",
         "hideMethod": "fadeOut"
     }
     toastr.danger = toastr.error;
     {% with messages = get_flashed_messages(with_categories=true) %}
         {% if messages %}
             {% for category, message in messages %}
-            toastr.{{ category }}("{{ message }}");
+                toastr.{{ category }}("{{ message|replace('\n', ' ') }}");
             {% endfor %}
         {% endif %}
     {% endwith %}
 </script>
 <script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js"></script>
 <script>
     document.addEventListener("DOMContentLoaded", (event) => {
@@ -227,18 +227,14 @@
             element.parentElement.style["background-color"] = "none";
             element.parentElement.style["border"] = "none";
             element.parentElement.querySelector("input[type=search]").remove();
         }
     });
 </script>
 <script src="https://pagination.js.org/dist/2.6.0/pagination.min.js"></script>
-<script src="https://unpkg.com/@simplewebauthn/browser/dist/bundle/index.umd.min.js"></script>
-<script>
-    const { startRegistration, startAuthentication } = SimpleWebAuthnBrowser;
-</script>
 
 <script>
     function validateInputs() {
         let inputs = document.querySelectorAll("input, textarea");
         // let previousForm = null;
         // let progressInputs = [];
         let isValid = true;
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/includes/sidenav.html` & `red_web_dashboard-1.6.0/reddash/app/templates/includes/sidenav.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 
-  <aside class="sidenav bg-white navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-4 " id="sidenav-main">
+  <aside class="sidenav bg-white navbar navbar-vertical navbar-expand-xs border-0 border-radius-xl my-3 fixed-start ms-4 " id="sidenav-main" style="scrollbar-width: none;">
     <div class="sidenav-header">
       <i class="fas fa-times p-3 cursor-pointer text-secondary opacity-5 position-absolute end-0 top-0 d-none d-xl-none" aria-hidden="true" id="iconSidenav"></i>
       <a class="navbar-brand m-0" href="/">
         <img src="{{ variables["bot"]["avatar"] }}" class="navbar-brand-img border-radius-sm h-100" alt="main_logo">
-        <span class="ms-1 text-dark font-weight-bold">{{ variables["bot"]["name"] }} {{ _("Dashboard") }}</span>
+        <span class="ms-1 font-weight-bold">{{ variables["bot"]["name"] }} {{ _("Dashboard") }}</span>
       </a>
     </div>
     <hr class="horizontal dark mt-0" style="height: 1px;">
     <div class="collapse navbar-collapse w-auto" style="height: 58%;" id="sidenav-collapse-main">
       <ul class="navbar-nav">
-        {% for item in variables["sidebar"] %}
+        {% for item in variables["sidenav"] %}
           <li class="{{ "active" if item["active"] else "" }}">
             <a class="nav-link{{ " active" if item["active"] else "" }}" href="{{ item["url"] }}"{{ ' target="blank"' if item["is_http"] }}{{ " data-scroll" if not item["active"] else "" }}>
               <div class="icon icon-shape icon-sm border-radius-md text-center me-2 d-flex align-items-center justify-content-center">
                 <i class="{{ item["icon"] }} text-primary text-lg opacity-10" style="margin-bottom: 5px;"></i>
               </div>
-              <span class="nav-link-text ms-1 text-dark">{{ item["name"] }}</span>
+              <span class="nav-link-text ms-1">{{ item["name"] }}</span>
             </a>
           </li>
         {% endfor %}
       </ul>
     </div>
     <div class="sidenav-footer mx-3">
       <div class="card card-plain shadow-none bg-transparent" id="sidenavCard">
-        <img class="w-50 mx-auto" src="{{ config.ASSETS_ROOT }}/icon-documentation.svg" alt="sidebar_illustration">
+        <img class="w-50 mx-auto" src="{{ config.ASSETS_ROOT }}/icon-documentation.svg" alt="sidenav_illustration">
         <div class="card-body text-center p-3 w-100 pt-0">
           <div class="docs-info">
-            <span class="font-weight-bold text-dark">{{ _("Need help?") }}</span><br />
+            <span class="font-weight-bold">{{ _("Need help?") }}</span><br />
             {% if variables["meta"]["support_server"] %}
-              <span class="text-xs font-weight-bold text-dark">{{ _("Please join our support server!") }}</span>
+              <span class="text-xs font-weight-bold">{{ _("Please join our support server!") }}</span>
             {% else %}
-              <span class="text-xs font-weight-bold text-dark">{{ _("Please check our docs!") }}</span>
+              <span class="text-xs font-weight-bold">{{ _("Please check our docs!") }}</span>
             {% endif %}
           </div>
         </div>
       </div>
       {% if variables["meta"]["support_server"] %}
-        <a class="btn btn-dark btn-sm w-100 mb-3" href="{{ variables["meta"]["support_server"] }}" type="button">{{ _("Join Support Server") }}</a>
+        <a class="btn bg-gradient-{{ variables["meta"]["color"] }} btn-sm w-100 mb-3" href="{{ variables["meta"]["support_server"] }}" type="button">{{ _("Join Support Server") }}</a>
       {% else %}
-        <a class="btn btn-dark btn-sm w-100 mb-3" href="{{ url_for("base_blueprint.commands") }}" type="button">{{ _("Documentation") }}</a>
+        <a class="btn bg-gradient-{{ variables["meta"]["color"] }} btn-sm w-100 mb-3" href="{{ url_for("base_blueprint.commands") }}" type="button">{{ _("Documentation") }}</a>
       {% endif %}
     </div>
   </aside>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/layouts/base-fullscreen.html` & `red_web_dashboard-1.6.0/reddash/app/templates/layouts/base-fullscreen.html`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,17 @@
      <link href="{{ config.ASSETS_ROOT }}/css/nucleo-icons.css" rel="stylesheet" />
      <link href="{{ config.ASSETS_ROOT }}/css/nucleo-svg.css" rel="stylesheet" />
      <!-- Font Awesome Icons -->
      <script src="https://kit.fontawesome.com/42d5adcbca.js" crossorigin="anonymous"></script>
      <link href="{{ config.ASSETS_ROOT }}/css/nucleo-svg.css" rel="stylesheet" />
      <!-- CSS Files -->
      <link id="pagestyle" href="{{ config.ASSETS_ROOT }}/css/argon-dashboard.css?v=2.0.4" rel="stylesheet" />
+     <link id="background_theme" href="{{ config.ASSETS_ROOT }}/css/themes/background_theme_{{ variables["meta"]["background_theme"] }}.css" rel="stylesheet" />
+     <link id="sidenav_theme" href="{{ config.ASSETS_ROOT }}/css/themes/sidenav_theme_{{ variables["meta"]["sidenav_theme"] }}.css" rel="stylesheet" />
+  
      <link href="https://cdnjs.cloudflare.com/ajax/libs/toastr.js/latest/toastr.min.css" rel="stylesheet" />
      <style>
        body #toast-container > div {
          opacity: 1;
          margin-top: 6px;
          width: 500px !important;
        }
@@ -115,22 +118,10 @@
  
      <!-- Control Center for Soft Dashboard: parallax effects, scripts for the example pages etc -->
      {% include "includes/scripts.html" %}
      <script src="{{ config.ASSETS_ROOT }}/js/argon-dashboard.js?v=2.0.4"></script>
  
      <!-- Specific JS goes HERE -->
      {% block javascripts %}{% endblock %}
- 
-     <script>
-      document.querySelector("#background-color-select").querySelector('.bg-gradient-{{ variables["meta"]["color"] }}').click();
-      {% if variables["meta"]["background_theme"] == "dark" %}
-        document.querySelector("#background-theme-select").firstElementChild.click();
-      {% endif %}
-      {% if variables["meta"]["sidebar_theme"] == "white" %}
-        document.querySelector("#sidebar-theme-select").children[0].click();
-      {% else %}
-        document.querySelector("#sidebar-theme-select").children[1].click();
-      {% endif %}
-     </script>
    </body>
  </html>
```

#### html2text {}

```diff
@@ -2,13 +2,15 @@
 }" />
 } - {{ self.title() }}" />
 }" />
 }" />
 }" />
 {% if False %}
 {% endif %}
+}.css" rel="stylesheet" />
+}.css" rel="stylesheet" />
 {% block stylesheets %}{% endblock %}
 } position-absolute w-100">
 {% include "includes/navigation.html" %} {% block content %} {% endblock %} {%
 include "includes/fixed-plugin.html" %} {% include "includes/footer.html" %}
 {% include "includes/scripts.html" %}
 {% block javascripts %}{% endblock %}
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/layouts/base.html` & `red_web_dashboard-1.6.0/reddash/app/templates/layouts/base.html`

 * *Files 14% similar despite different names*

```diff
@@ -46,14 +46,17 @@
     <link href="{{ config.ASSETS_ROOT }}/css/nucleo-icons.css" rel="stylesheet" />
     <link href="{{ config.ASSETS_ROOT }}/css/nucleo-svg.css" rel="stylesheet" />
     <!-- Font Awesome Icons -->
     <script src="https://kit.fontawesome.com/42d5adcbca.js" crossorigin="anonymous"></script>
     <link href="{{ config.ASSETS_ROOT }}/css/nucleo-svg.css" rel="stylesheet" />
     <!-- CSS Files -->
     <link id="pagestyle" href="{{ config.ASSETS_ROOT }}/css/argon-dashboard.css?v=2.0.4" rel="stylesheet" />
+    <link id="background_theme" href="{{ config.ASSETS_ROOT }}/css/themes/background_theme_{{ variables["meta"]["background_theme"] }}.css" rel="stylesheet" />
+    <link id="sidenav_theme" href="{{ config.ASSETS_ROOT }}/css/themes/sidenav_theme_{{ variables["meta"]["sidenav_theme"] }}.css" rel="stylesheet" />
+  
     <link href="https://cdnjs.cloudflare.com/ajax/libs/toastr.js/latest/toastr.min.css" rel="stylesheet" />
     <style>
       body #toast-container > div {
         opacity: 1;
         margin-top: 6px;
         width: 500px !important;
       }
@@ -117,28 +120,9 @@
 
     <!-- Control Center for Soft Dashboard: parallax effects, scripts for the example pages etc -->
     {% include "includes/scripts.html" %}
     <script src="{{ config.ASSETS_ROOT }}/js/argon-dashboard.js?v=2.0.4"></script>
 
     <!-- Specific JS goes HERE -->
     {% block javascripts %}{% endblock %}
-
-    <script>
-      let win = navigator.platform.indexOf("Win") > -1
-      if (win && document.querySelector("#sidenav-scrollbar")) {
-        let options = {
-          damping: "0.5"
-        }
-        Scrollbar.init(document.querySelector("#sidenav-scrollbar"), options);
-      }
-      document.querySelector("#background-color-select").querySelector('.bg-gradient-{{ variables["meta"]["color"] }}').click();
-      {% if variables["meta"]["background_theme"] == "dark" %}
-        document.querySelector("#background-theme-select").firstElementChild.click();
-      {% endif %}
-      {% if variables["meta"]["sidebar_theme"] == "white" %}
-        document.querySelector("#sidebar-theme-select").children[0].click();
-      {% else %}
-        document.querySelector("#sidebar-theme-select").children[1].click();
-      {% endif %}
-    </script>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,14 +2,16 @@
 }" />
 } - {{ self.title() }}" />
 }" />
 }" />
 }" />
 {% if False %}
 {% endif %}
+}.css" rel="stylesheet" />
+}.css" rel="stylesheet" />
 {% block stylesheets %}{% endblock %}
 } position-absolute w-100">
 {% include "includes/navigation.html" %} {% include "includes/sidenav.html" %}
 {% block content %} {% endblock %} {% include "includes/fixed-plugin.html" %}
 {% include "includes/footer.html" %}
 {% include "includes/scripts.html" %}
 {% block javascripts %}{% endblock %}
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/admin.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/admin.html`

 * *Files 5% similar despite different names*

```diff
@@ -103,17 +103,17 @@
                             <div class="mt-4">
                                 <p>
                                     {{ _("Webserver has been up for:") }} <code>{{ uptime_str }}</code>.<br />
                                     {% if config["RPC_CONNECTED"] %}{{ _("Connected to RPC websocket for:") }}{% else %}{{ _("Disconnected of RPC websocket for:") }}{% endif %} <code>{{ connection_str }}</code>.
                                 </p>
                                 <form action="" method="POST" role="form" enctype="multipart/form-data">
                                     {{ dashboard_actions_form.hidden_tag() }}
-                                    {{ dashboard_actions_form.lock(class="btn mb-0 bg-gradient-success btn-md my-4 mb-2", onclick="return confirmLock(event);") }}
+                                    {{ dashboard_actions_form.lock(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md my-4 mb-2", onclick="return confirmLock(event);") }}
                                     <p><i>{{ _("This will lock the dashboard and prevent anyone from accessing control panels. Website administrators will still have access, and users will still be able to login through Discord Open Authentication.") }}</i></p>
-                                    {{ dashboard_actions_form.refresh_sessions(class="btn mb-0 bg-gradient-success btn-md my-4 mb-2", onclick="return confirmRefreshSessions(event);") }}
+                                    {{ dashboard_actions_form.refresh_sessions(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md my-4 mb-2", onclick="return confirmRefreshSessions(event);") }}
                                     <p><i>{{ _("This will log out all active users and require them to re-authenticate, including website administrators.") }}</i></p>
                                 </form>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
@@ -172,28 +172,28 @@
                                             <div class="form-group">
                                                 <label class="form-group-label">{{ dashboard_settings_form.default_background_theme.label.text }}</label>
                                                 {{ dashboard_settings_form.default_background_theme(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                         <div class="col-sm-6">
                                             <div class="form-group">
-                                                <label class="form-group-label">{{ dashboard_settings_form.default_sidebar_theme.label.text }}</label>
-                                                {{ dashboard_settings_form.default_sidebar_theme(class="form-control form-control-default") }}
+                                                <label class="form-group-label">{{ dashboard_settings_form.default_sidenav_theme.label.text }}</label>
+                                                {{ dashboard_settings_form.default_sidenav_theme(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                     </div>
                                     <hr class="horizontal dark" />
                                     <div class="mb-3">
                                         <div class="form-group">
                                             <label class="form-group-label">{{ dashboard_settings_form.disabled_third_parties.label.text }}</label>
                                             {{ dashboard_settings_form.disabled_third_parties(class="form-control form-control-default") }}
                                         </div>
                                     </div>
                                     <div class="text-center">
-                                        {{ dashboard_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
+                                        {{ dashboard_settings_form.submit(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md w-100 my-4 mb-2") }}
                                     </div>
                                 </form>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
@@ -309,15 +309,15 @@
                                             <div class="form-group">
                                                 <label class="form-group-label">{{ bot_settings_form.regional_format.label.text }}</label>
                                                 {{ bot_settings_form.regional_format(class="form-control form-control-default") }}
                                             </div>
                                         </div>
                                     </div>
                                     <div class="text-center">
-                                        {{ bot_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
+                                        {{ bot_settings_form.submit(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md w-100 my-4 mb-2") }}
                                     </div>
                                 </form>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
@@ -361,15 +361,15 @@
                                 <label class="form-group-label">{{ bot_profile_form.description.label.text }}</label>
                                 {{ bot_profile_form.description(class="form-control form-control-default") }}
                             </div>
                         </div>
                     </div>
                     <div class="modal-footer">
                         <a class="btn btn-secondary" data-dismiss="modal">{{ _("Fermer") }}</a>
-                        {{ bot_profile_form.submit(class="btn mb-0 bg-gradient-success btn-md w-30 mt-2 mb-4") }}
+                        {{ bot_profile_form.submit(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md w-30 mt-2 mb-4") }}
                     </div>
                 </form>
             </div>
         </div>
     </div>
 
   </main>
```

#### html2text {}

```diff
@@ -18,21 +18,22 @@
 labelledby="overview-tab">
 ********** {{{{ __((""OOvveerrvviieeww"")) }}}} **********
 {{ _("Webserver has been up for:") }} {{ uptime_str }}.
 {% if config["RPC_CONNECTED"] %}{{ _("Connected to RPC websocket for:") }}{%
 else %}{{ _("Disconnected of RPC websocket for:") }}{% endif %} {
 { connection_str }}.
 {{ dashboard_actions_form.hidden_tag() }} {{ dashboard_actions_form.lock
-(class="btn mb-0 bg-gradient-success btn-md my-4 mb-2", onclick="return
-confirmLock(event);") }}
+(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md my-4 mb-
+2", onclick="return confirmLock(event);") }}
 {{ _("This will lock the dashboard and prevent anyone from accessing control
 panels. Website administrators will still have access, and users will still be
 able to login through Discord Open Authentication.") }}
-{{ dashboard_actions_form.refresh_sessions(class="btn mb-0 bg-gradient-success
-btn-md my-4 mb-2", onclick="return confirmRefreshSessions(event);") }}
+{{ dashboard_actions_form.refresh_sessions(class="btn mb-0 bg-gradient-" +
+variables["meta"]["color"] + " btn-md my-4 mb-2", onclick="return
+confirmRefreshSessions(event);") }}
 {{ _("This will log out all active users and require them to re-authenticate,
 including website administrators.") }}
 }show active{% endif %}" id="dashboard-settings" role="tabpanel" aria-
 labelledby="dashboard-settings-tab">
 ********** {{{{ __((""DDaasshhbbooaarrdd SSeettttiinnggss"")) }}}} **********
 {{ dashboard_settings_form.hidden_tag() }}
 {{ dashboard_settings_form.title.label.text }} {{ dashboard_settings_form.title
@@ -51,23 +52,23 @@
 ===============================================================================
 {{ dashboard_settings_form.default_color.label.text }} {
 { dashboard_settings_form.default_color(class="form-control form-control-
 default") }}
 {{ dashboard_settings_form.default_background_theme.label.text }} {
 { dashboard_settings_form.default_background_theme(class="form-control form-
 control-default") }}
-{{ dashboard_settings_form.default_sidebar_theme.label.text }} {
-{ dashboard_settings_form.default_sidebar_theme(class="form-control form-
+{{ dashboard_settings_form.default_sidenav_theme.label.text }} {
+{ dashboard_settings_form.default_sidenav_theme(class="form-control form-
 control-default") }}
 ===============================================================================
 {{ dashboard_settings_form.disabled_third_parties.label.text }} {
 { dashboard_settings_form.disabled_third_parties(class="form-control form-
 control-default") }}
-{{ dashboard_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-
-100 my-4 mb-2") }}
+{{ dashboard_settings_form.submit(class="btn mb-0 bg-gradient-" + variables
+["meta"]["color"] + " btn-md w-100 my-4 mb-2") }}
 }show active{% endif %}" id="bot-settings" role="tabpanel" aria-
 labelledby="bot-settings-tab">
 ********** {{{{ __((""BBoott SSeettttiinnggss"")) }}}} **********
 {{ bot_settings_form.hidden_tag() }}
 {{ bot_settings_form.prefixes.label.text }} {{ bot_settings_form.prefixes
 (class="form-control form-control-default select-choices") }}
 {{ bot_settings_form.invoke_error_msg.label.text }} {
@@ -102,26 +103,26 @@
 { bot_settings_form.invite_perms(class="form-control form-control-default") }}
 ===============================================================================
 {{ bot_settings_form.locale.label.text }} {{ bot_settings_form.locale
 (class="form-control form-control-default") }}
 {{ bot_settings_form.regional_format.label.text }} {
 { bot_settings_form.regional_format(class="form-control form-control-default")
 }}
-{{ bot_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100
-my-4 mb-2") }}
+{{ bot_settings_form.submit(class="btn mb-0 bg-gradient-" + variables["meta"]
+["color"] + " btn-md w-100 my-4 mb-2") }}
 **** {{{{ __((""EEddiitt DDiissccoorrdd BBoott PPrrooffiillee"")) }}}} ****
 ×
 {{ bot_profile_form.hidden_tag() }}
 }" />
 {{ bot_profile_form.avatar(class="file-upload", accept="image/png, image/jpg,
 image/jpeg, image/gif", onchange="readURL(this);", style="display: none;") }}
 % if variables["bot"]["avatar"] != variables["bot"]["default_avatar"] %}
 style="display: none;"{% endif %}>{{ _("Use default") }}
  _{_{_ ___(_"_K_e_e_p_ _c_u_r_r_e_n_t_"_)_ _}_}
 {{ bot_profile_form.username.label.text }} {{ bot_profile_form.username
 (class="form-control form-control-default") }}
 {{ bot_profile_form.description.label.text }} {{ bot_profile_form.description
 (class="form-control form-control-default") }}
-{{ _("Fermer") }} {{ bot_profile_form.submit(class="btn mb-0 bg-gradient-
-success btn-md w-30 mt-2 mb-4") }}
+{{ _("Fermer") }} {{ bot_profile_form.submit(class="btn mb-0 bg-gradient-" +
+variables["meta"]["color"] + " btn-md w-30 mt-2 mb-4") }}
 {% endblock %} {% block javascripts %}
 {% endblock %}
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/commands.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/commands.html`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                                               <div class="row">
                                                 <div class="col-ms-8">
                                                     <p class="mb-0">{{ (_("Author(s): {author}")).format(author=cogs[cog]["author"])}}</p>
                                                     <p>{{ _("Repo:") }} <a {% if cogs[cog]["repo"] != "Unknown" %}href="{{ cogs[cog]["repo"] }}"{% endif %}>{{ cogs[cog]["repo"] }}</a></p>
                                                 </div>
                                                 <div class="col-sm-4 text-left">
                                                     <div class="dropdown show">
-                                                        <a class="btn bg-gradient-success dropdown-toggle" href="#" role="button" id="prefixdrop_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                                                        <a class="btn bg-gradient-{{ variables["meta"]["color"] }} dropdown-toggle" href="#" role="button" id="prefixdrop_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                                             {{ _("Prefix") }}
                                                         </a>
                                                         <ul class="dropdown-menu prefixdiv" aria-labelledby="prefixdrop_dropdown">
                                                             {% for p in prefixes %}
                                                             <li>
                                                               <a class="dropdown-item prefix-option {% if loop.index == 1 %} active {% endif %}">{{ p }}</a>
                                                             </li>
@@ -126,15 +126,15 @@
                 <div class="row">
                   <div class="col-md-12">
                       <div class="card">
                           <div class="card-header">
                             <div class="card-body">
                               <div class="col-sm-4 text-left">
                                 <div class="dropdown show">
-                                    <a class="btn bg-gradient-success dropdown-toggle" href="#" role="button" id="prefixdrop_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+                                    <a class="btn bg-gradient-{{ variables["meta"]["color"] }} dropdown-toggle" href="#" role="button" id="prefixdrop_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                         {{ _("Prefix") }}
                                     </a>
                                     <ul class="dropdown-menu prefixdiv" aria-labelledby="prefixdrop_dropdown">
                                         {% for p in prefixes %}
                                           <li>
                                             <a class="dropdown-item prefix-option {% if loop.index == 1 %} active {% endif %}">{{ p }}</a>
                                           </li>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/credits.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/credits.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/dashboard.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/dashboard.html`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                       <a class="dropdown-item" href="{{ url_for_query(filter=None) }}">{% if not filter %}<i class="ni ni-check-bold me-2" style="vertical-align: -1.5px;"></i>{% endif %}{{ _("All guilds") }}</a>
                       <a class="dropdown-item" href="{{ url_for_query(filter="owner") }}">{% if filter == "owner" %}<i class="ni ni-check-bold me-2" style="vertical-align: -1.5px;"></i>{% endif %}{{ _("Owner") }}</a>
                       <a class="dropdown-item" href="{{ url_for_query(filter="admin") }}">{% if filter == "admin" %}<i class="ni ni-check-bold me-2" style="vertical-align: -1.5px;"></i>{% endif %}{{ _("Administrator") }}</a>
                       <a class="dropdown-item" href="{{ url_for_query(filter="mod") }}">{% if filter == "mod" %}<i class="ni ni-check-bold me-2" style="vertical-align: -1.5px;"></i>{% endif %}{{ _("Moderator") }}</a>
                   </div>
               </div>
               <div class="ms-md-auto">
-                  <a class="btn bg-gradient-success" href="{{ variables["bot"]["invite_url"] }}" target="_blank"><i class="ni ni-fat-add me-2" style="vertical-align: -2px;"></i>{{ _("Invite Me!") }}</a>
+                  <a class="btn bg-gradient-{{ variables["meta"]["color"] }}" href="{{ variables["bot"]["invite_url"] }}" target="_blank"><i class="ni ni-fat-add me-2" style="vertical-align: -2px;"></i>{{ _("Invite Me!") }}</a>
               </div>
             </div>
             <div id="guilds-container">
                 <div class="row">
                     {% for guild in guilds %}
                         <div class="col-md-3 d-flex" style="margin-bottom: 20px;">
                             <div class="card flex-fill">
```

#### html2text {}

```diff
@@ -8,15 +8,16 @@
 _{_%_ _i_f_ _n_o_t_ _f_i_l_t_e_r_ _%_}_{_%_ _e_n_d_i_f_ _%_}_{_{_ ___(_"_A_l_l_ _g_u_i_l_d_s_"_)_ _}_}
 
 }">{% if filter == "owner" %}{% endif %}{{ _("Owner") }}
 
 }">{% if filter == "admin" %}{% endif %}{{ _("Administrator") }}
 
 }">{% if filter == "mod" %}{% endif %}{{ _("Moderator") }}
-}" target="_blank">{{ _("Invite Me!") }}
+}" href="{{ variables["bot"]["invite_url"] }}" target="_blank">{{ _("Invite
+Me!") }}
 {% for guild in guilds %}
 }">
 [{{ guild.icon_url }}]
 ** {{{{ gguuiilldd..nnaammee }}}} (({{{{ gguuiilldd..iidd }}}})) **
 {{ _("Owned by") }} {{ guild.owner }}
 {% endfor %}
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/dashboard_guild.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/dashboard_guild.html`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                                                                     <div class="col-md-12 d-flex justify-content-end align-items-center">
                                                                         <a href="javascript:void(0);" onclick="this.parentElement.parentNode.remove();" class="text-danger mr-3"><i class="fa fa-minus-circle"></i> {{ _("Delete Alias") }}</a>
                                                                     </div>
                                                                 </div>
                                                             {% endfor %}
                                                             <a href="javascript:void(0);" onclick="createAlias(this);" class="text-success mr-3"><i class="fa fa-plus-circle"></i> {{ _("Create Alias") }}</a>
                                                             <div class="text-center">
-                                                                {{ aliases_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
+                                                                {{ aliases_form.submit(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md w-100 my-4 mb-2") }}
                                                             </div>
                                                         </form>
                                                     </div>
                                                 </div>
                                             </div>
                                         {% endif %}
 
@@ -132,15 +132,15 @@
                                                                     <div class="col-md-12 d-flex justify-content-end align-items-center">
                                                                         <a href="javascript:void(0);" onclick="this.parentElement.parentNode.remove();" class="text-danger mr-3"><i class="fa fa-minus-circle"></i> {{ _("Delete Custom Command") }}</a>
                                                                     </div>
                                                                 </div>
                                                             {% endfor %}
                                                             <a href="javascript:void(0);" onclick="createCustomCommand(this);" class="text-success mr-3"><i class="fa fa-plus-circle"></i> {{ _("Create Custom Command") }}</a>
                                                             <div class="text-center">
-                                                                {{ custom_commands_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
+                                                                {{ custom_commands_form.submit(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md w-100 my-4 mb-2") }}
                                                             </div>
                                                         </form>
                                                     </div>
                                                 </div>
                                             </div>
                                         {% endif %}
 
@@ -240,15 +240,15 @@
                                                     <div class="form-group">
                                                         <label class="form-group-label">{{ guild_settings_form.regional_format.label.text }}</label>
                                                         {{ guild_settings_form.regional_format(class="form-control form-control-default") }}
                                                     </div>
                                                 </div>
                                             </div>
                                             <div class="text-center">
-                                                {{ guild_settings_form.submit(class="btn mb-0 bg-gradient-success btn-md w-100 my-4 mb-2") }}
+                                                {{ guild_settings_form.submit(class="btn mb-0 bg-gradient-" + variables["meta"]["color"] + " btn-md w-100 my-4 mb-2") }}
                                             </div>
                                         </form>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </div>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/guild_profile.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/guild_profile.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
             <div class="avatar avatar-xl"><img src={% if guild.icon_animated %}"{{ guild.icon_url[:-3] + "png" }}" onmouseover='this.src = this.src.slice(0, -3) + "gif";' onmouseout='this.src = this.src.slice(0, -3) + "png";'{% else %}"{{ guild.icon_url }}"{% endif %} class="shadow-sm border-radius-lg" style="height: 170%; width: 170%;" /></div>
         </div>
         <div class="col-sm-auto col-8 my-auto">
             <div class="h-100">
                 <h3 class="col mb-1 font-weight-bolder text-center">
                     {{ guild.name }}
                     <div class="dropdown" style="display: unset;">
-                        <a class="nav-link text-lg text-dark" role="button" id="guild_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" style="display: unset; vertical-align: 2.6px; margin-left: 2px;">
+                        <a class="nav-link text-lg" role="button" id="guild_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" style="display: unset; vertical-align: 2.6px; margin-left: 2px;">
                             <i class="fa fa-ellipsis-v"></i>
                         </a>
                         <ul class="dropdown-menu" aria-labelledby="guild_dropdown">
                             <li class="nav-link"><a class="nav-item dropdown-item" onclick='copyTextToClipboard("{{ guild.id }}")'><i class="fa fa-copy" style="width: 1.3em; vertical-align: 0.2px;"></i> {{ _("Copy ID") }}</a></li>
                             {% if leave_guild_form %}
                                 <form action="" method="POST" role="form" enctype="multipart/form-data">
                                     {{ leave_guild_form.hidden_tag() }}
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/index.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,19 @@
               <div class="col-lg-3">
                 <img src="{{ variables["bot"]["avatar"] }}" style="height: 200px; width: 200px; border-radius: 50%; margin: auto; display: block;" />
               </div>
               <div class="col-lg-8">
                 <h4>{{ variables["meta"]["description"]|markdown }}</h4>
                 <br />
                 {% if variables["bot"]["invite_public"] or (current_user.is_authenticated and current_user.is_owner) %}
-                  <a class="btn btn-m bg-gradient-success" href="{{ variables["bot"]["invite_url"] }}" target="_blank" style="width: 65%;"><i class="fa fa-plus-circle me-2" style="vertical-align: -0.5px;"></i>{{ _("Invite Me!") }}</a>
+                  <a class="btn btn-m bg-gradient-{{ variables["meta"]["color"] }}" href="{{ variables["bot"]["invite_url"] }}" target="_blank" style="width: 65%;"><i class="fa fa-plus-circle me-2" style="vertical-align: -0.5px;"></i>{{ _("Invite Me!") }}</a>
                 {% endif %}
                 {% if False %}
                   <br />
-                  <a class="btn bg-gradient-success" href="{{ variables["meta"]["support_server"] }}" target="_blank">{{ _("Join support server") }}</a>
+                  <a class="btn bg-gradient-{{ variables["meta"]["color"] }}" href="{{ variables["meta"]["support_server"] }}" target="_blank">{{ _("Join support server") }}</a>
                 {% endif %}
               </div>
             </div>
         </div>
       </div>
       <br />
       <div class="row">
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/login/login.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/login/login.html`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,20 @@
                         <div class="card border-0 mb-0">
                           <div class="card-header bg-transparent">
                             <div class="text-center info mb-4">
                               <div class="icon icon-shape icon-xl rounded-circle bg-gradient-warning shadow text-center">
                                 <img src="{{ config["ASSETS_ROOT"] }}/biometric-icon.svg" style="height: 80%; margin-top: 7px;" />
                               </div>
                             </div>
-                            <h1 class="text-dark text-center mt-2 mb-3">{{ _("Authentication") }}</h1>
+                            <h1 class="text-center mt-2 mb-3">{{ _("Authentication") }}</h1>
                           </div>
                           <div class="card-body px-lg-5 pt-0">
                             <p class="text-center">{{ _("Accessing Red-Dashboard controls requires authorization for security. Authorization for Red-Dashboard uses Discord Open Authentication to identify and verify users. Please click on the Login button below to access the Dashboard.") }}</p>
                             <br />
-                            <a class="btn bg-gradient-success mb-1 w-100" href="{{ url_for("login_blueprint.discord_oauth", next=next) }}">{{ _("Login with Discord") }}</a>
+                            <a class="btn bg-gradient-{{ variables["meta"]["color"] }} mb-1 w-100" href="{{ url_for("login_blueprint.discord_oauth", next=next) }}">{{ _("Login with Discord") }}</a>
                           </div>
                         </div>
                       </div>
                     </div>
                   </div>
                 </div>
               </div>
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/oauth.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/oauth.html`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
               <div class="card">
                 <div class="card-header">
                   <div class="card-body">
                     <h1><bold>{{ provider|title }} {{ _("OAuth") }}</bold></h1>
                     <p>{{ _("Successfully forwarded your account informations. You may now close this tab and go back to Discord.") }}</p>
                     <img src="{{ config.ASSETS_ROOT }}/oauth.png" height="250" />
                     <br /><br />
-                    <a class="btn bg-gradient-success mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
+                    <a class="btn bg-gradient-{{ variables["meta"]["color"] }} mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home") }}</a>
                   </div>
                 </div>
                 <div class="card-footer">
                   {{ _('This is a Third Party integration. By using this application, you acknowledge that you have read the Third Party disclaimer found <a href="{link}">here</a>.').format(link="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/Third%20Parties%20Disclaimer.md") }}
                 </div>
               </div>
             </div>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "layouts/base.html" %} {% block title %} {{ _("Erreur 403") }} {%
 endblock %} {% block stylesheets %}{% endblock %} {% block content %}
 ************ {{{{ pprroovviiddeerr||ttiittllee }}}} {{{{ __((""OOAAuutthh"")) }}}} ************
 {{ _("Successfully forwarded your account informations. You may now close this
 tab and go back to Discord.") }}
 [{{ config.ASSETS_ROOT }}/oauth.png]
 
-}">{{ _("Back to Home") }}
+} mb-1 w-30" href="{{ url_for("base_blueprint.index") }}">{{ _("Back to Home")
+}}
 {{ _('This is a Third Party integration. By using this application, you
 acknowledge that you have read the Third Party disclaimer found _h_e_r_e.').format
 (link="https://github.com/AAA3A-AAA3A/Red-Dashboard/blob/main/documents/
 Third%20Parties%20Disclaimer.md") }}
 {% endblock %} {% block javascripts %}{% endblock %}
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/third_parties_list.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_parties_list.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/templates/pages/third_parties/third_party.html` & `red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_party.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.5.4/reddash/app/third_parties/routes.py` & `red_web_dashboard-1.6.0/reddash/app/third_parties/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             return render_template("errors/custom.html", error_title=f"Invalid argument: `{key}`.")
     for key in third_parties[name][_page]["required_kwargs"]:
         if key not in kwargs:
             return render_template("errors/custom.html", error_title=f"Missing argument: `{key}`.")
         required_kwargs[key] = kwargs.pop(key)
     for key in kwargs:
         if key in third_parties[name][_page]["optional_kwargs"]:
-            optional_kwargs[key] = kwargs[key]
+            optional_kwargs[key] = kwargs.pop(key)
     extra_kwargs = kwargs
 
     data = {}
     data["form"] = request.form.to_dict(flat=False)
     data["json"] = request.json.to_dict(flat=False) if request.method not in ("GET", "HEAD") and request.content_type == "application/json" else {}
     
     try:
```

### Comparing `red_web_dashboard-1.5.4/reddash/app/utils.py` & `red_web_dashboard-1.6.0/reddash/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,21 +355,21 @@
     def process_meta_tags() -> typing.Dict[str, typing.Any]:
         meta = deepcopy(app.data["ui"]["meta"])
         meta["color"] = request.cookies.get("color", meta["default_color"])
         meta["available_colors"]: typing.List[str] = AVAILABLE_COLORS
         meta["background_theme"] = request.cookies.get(
             "background_theme", meta["default_background_theme"]
         )
-        meta["sidebar_theme"] = request.cookies.get("sidebar_theme", meta["default_sidebar_theme"])
+        meta["sidenav_theme"] = request.cookies.get("sidenav_theme", meta["default_sidenav_theme"])
         return {"meta": meta}
 
-    def process_sidebar() -> typing.List[typing.Dict]:
-        sidebar = sorted(app.data["ui"]["sidebar"], key=lambda x: x["pos"])
+    def process_sidenav() -> typing.List[typing.Dict]:
+        sidenav = sorted(app.data["ui"]["sidenav"], key=lambda x: x["pos"])
         final = []
-        for item in sidebar:
+        for item in sidenav:
             item = dict(item.items())
             if item["session"] is True and not current_user.is_authenticated:
                 continue
             if item["session"] is False and current_user.is_authenticated:
                 continue
             if item["owner"] and not (current_user.is_authenticated and current_user.is_owner):
                 continue
@@ -465,15 +465,15 @@
 
     @app.context_processor
     def inject_variables() -> typing.Dict[str, typing.Any]:
         variables = deepcopy(app.variables)
         variables["locales"] = app.config["LOCALE_DICT"]
         variables["safelocales"] = json.dumps(app.config["LOCALE_DICT"])
         variables["selectedlocale"] = session.get("lang_code")
-        variables["sidebar"] = process_sidebar()
+        variables["sidenav"] = process_sidenav()
         uptime = datetime.datetime.fromtimestamp(
             app.variables["stats"]["uptime"]
         )
         utc_now = datetime.datetime.utcnow().replace(second=0, microsecond=0)
         real_timedelta = utc_now - uptime
         timedelta: datetime.timedelta = utc_now - uptime.replace(
             hour=utc_now.hour
```

### Comparing `red_web_dashboard-1.5.4/setup.cfg` & `red_web_dashboard-1.6.0/setup.cfg`

 * *Files identical despite different names*

