# Comparing `tmp/dashport-0.7.4.tar.gz` & `tmp/dashport-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashport-0.7.4.tar", last modified: Sat May 11 22:01:17 2024, max compression
+gzip compressed data, was "dashport-0.7.5.tar", last modified: Sun May 12 06:26:28 2024, max compression
```

## Comparing `dashport-0.7.4.tar` & `dashport-0.7.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.284086 dashport-0.7.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.272086 dashport-0.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.272086 dashport-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-11 22:01:13.000000 dashport-0.7.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-11 22:01:13.000000 dashport-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    34459 2024-05-11 22:01:13.000000 dashport-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-11 22:01:17.284086 dashport-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-11 22:01:13.000000 dashport-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.276086 dashport-0.7.4/dashport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/borders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.276086 dashport-0.7.4/dashport/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/resources/block_elements_table.json
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/resources/box_drawing_table.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-11 22:01:13.000000 dashport-0.7.4/dashport/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.284086 dashport-0.7.4/dashport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-11 22:01:17.000000 dashport-0.7.4/dashport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-11 22:01:17.000000 dashport-0.7.4/dashport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:01:17.000000 dashport-0.7.4/dashport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 22:01:17.000000 dashport-0.7.4/dashport.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.276086 dashport-0.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/buttons.md
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/colors.md
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/dashport.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.280086 dashport-0.7.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/examples/boilerplate.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/examples/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/examples/layouts.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/examples/util.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/examples/views.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.280086 dashport-0.7.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   110554 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/images/Layout_quadrants.png
--rw-r--r--   0 runner    (1001) docker     (127)    66901 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/images/Layout_split_screen_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)    76578 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/images/Layout_split_screen_vert.png
--rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/images/Layout_three_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)   107025 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/images/Layout_three_vert.png
--rw-r--r--   0 runner    (1001) docker     (127)   558852 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/images/color_palette.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/layouts.md
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/panels.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/strings.md
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-11 22:01:13.000000 dashport-0.7.4/docs/widgets.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.280086 dashport-0.7.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.280086 dashport-0.7.4/examples/boilerplate/
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/boilerplate/basic_window.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/boilerplate/boilerplate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/boilerplate/color_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/boilerplate/rectangle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2089 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/boilerplate/using_buttons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.284086 dashport-0.7.4/examples/layouts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/layouts/arbitrary_panels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/layouts/custom_borders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      578 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/layouts/split_screen_columns.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1896 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/layouts/split_screen_quad.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/layouts/split_screen_rows.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/layouts/split_screen_three_horizontal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/layouts/split_screen_three_vert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.284086 dashport-0.7.4/examples/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/util/all_ascii_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/util/all_attributes_curses.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4797 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/util/all_box_drawing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/util/color_palette.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1080 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/util/explore_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:01:17.284086 dashport-0.7.4/examples/views/
--rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/views/interactive_prompt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2541 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/views/multiple_views.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/views/scroll_panels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      703 2024-05-11 22:01:13.000000 dashport-0.7.4/examples/views/scroll_text.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:01:17.284086 dashport-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 22:01:13.000000 dashport-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.080959 dashport-0.7.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.064959 dashport-0.7.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.068959 dashport-0.7.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-12 06:26:23.000000 dashport-0.7.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-12 06:26:23.000000 dashport-0.7.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    34459 2024-05-12 06:26:23.000000 dashport-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-12 06:26:28.080959 dashport-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-12 06:26:23.000000 dashport-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.068959 dashport-0.7.5/dashport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/borders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.072959 dashport-0.7.5/dashport/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/resources/block_elements_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/resources/box_drawing_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-12 06:26:23.000000 dashport-0.7.5/dashport/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.080959 dashport-0.7.5/dashport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-12 06:26:28.000000 dashport-0.7.5/dashport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-12 06:26:28.000000 dashport-0.7.5/dashport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 06:26:28.000000 dashport-0.7.5/dashport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-12 06:26:28.000000 dashport-0.7.5/dashport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.072959 dashport-0.7.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/buttons.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/colors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/dashport.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.072959 dashport-0.7.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/examples/boilerplate.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/examples/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/examples/layouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/examples/util.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/examples/views.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.076959 dashport-0.7.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   110554 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/images/Layout_quadrants.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66901 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/images/Layout_split_screen_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76578 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/images/Layout_split_screen_vert.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92502 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/images/Layout_three_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107025 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/images/Layout_three_vert.png
+-rw-r--r--   0 runner    (1001) docker     (127)   558852 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/images/color_palette.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/layouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/panels.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/strings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-12 06:26:23.000000 dashport-0.7.5/docs/widgets.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.076959 dashport-0.7.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.076959 dashport-0.7.5/examples/boilerplate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/boilerplate/basic_window.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/boilerplate/boilerplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/boilerplate/color_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/boilerplate/rectangle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2089 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/boilerplate/using_buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.076959 dashport-0.7.5/examples/layouts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/layouts/arbitrary_panels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/layouts/custom_borders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      578 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/layouts/split_screen_columns.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1896 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/layouts/split_screen_quad.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/layouts/split_screen_rows.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/layouts/split_screen_three_horizontal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1260 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/layouts/split_screen_three_vert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.076959 dashport-0.7.5/examples/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1166 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/util/all_ascii_constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1010 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/util/all_attributes_curses.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4797 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/util/all_box_drawing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/util/color_palette.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1080 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/util/explore_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 06:26:28.080959 dashport-0.7.5/examples/views/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/views/interactive_prompt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2541 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/views/multiple_views.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/views/scroll_panels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      703 2024-05-12 06:26:23.000000 dashport-0.7.5/examples/views/scroll_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 06:26:28.080959 dashport-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-12 06:26:23.000000 dashport-0.7.5/setup.py
```

### Comparing `dashport-0.7.4/.github/workflows/publish-to-pypi.yml` & `dashport-0.7.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/.gitignore` & `dashport-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/LICENSE` & `dashport-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/PKG-INFO` & `dashport-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashport
-Version: 0.7.4
+Version: 0.7.5
 Summary: Dashport curses wrapper for Python
 Home-page: https://github.com/numbertheory/dashport
 Author: JP Etcheber
 Author-email: jetcheber@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dashport.svg)](https://badge.fury.io/py/dashport) [![Documentation Status](https://readthedocs.org/projects/dashport/badge/?version=latest)](https://dashport.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dashport-0.7.4/dashport/borders.py` & `dashport-0.7.5/dashport/borders.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/characters.py` & `dashport-0.7.5/dashport/characters.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/colors.py` & `dashport-0.7.5/dashport/colors.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/dash.py` & `dashport-0.7.5/dashport/dash.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/layout.py` & `dashport-0.7.5/dashport/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,16 +107,16 @@
     app.panel_coords = [[0, 0], [0, 0], [0, 0], [0, 0]]
     app.panel_dimensions = [win1.getmaxyx(), win2.getmaxyx(),
                             win3.getmaxyx(), win4.getmaxyx()]
     return [win1, win2, win3, win4, panel1, panel2, panel3, panel4]
 
 
 def three_panels_vert(app, **kwargs):
-    split_rows = int(app.rows / 2) - app.title_offset
-    split_cols = int(app.cols / 2)
+    split_rows = kwargs.get("split_rows", int(app.rows / 2) - app.title_offset)
+    split_cols = kwargs.get("split_cols", int(app.cols / 2))
     long_side = kwargs.get("long_side", "right")
     border = kwargs.get("border", False)
     border_styles = kwargs.get("border_styles", [0, 0, 0])
     if isinstance(border, bool):
         border = [border] * 3
     long_side_width = kwargs.get("long_side_width", None)
     if not long_side_width:
```

### Comparing `dashport-0.7.4/dashport/prompt.py` & `dashport-0.7.5/dashport/prompt.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/resources/block_elements_table.json` & `dashport-0.7.5/dashport/resources/block_elements_table.json`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/resources/box_drawing_table.json` & `dashport-0.7.5/dashport/resources/box_drawing_table.json`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/run.py` & `dashport-0.7.5/dashport/run.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport/widgets.py` & `dashport-0.7.5/dashport/widgets.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/dashport.egg-info/PKG-INFO` & `dashport-0.7.5/dashport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashport
-Version: 0.7.4
+Version: 0.7.5
 Summary: Dashport curses wrapper for Python
 Home-page: https://github.com/numbertheory/dashport
 Author: JP Etcheber
 Author-email: jetcheber@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/dashport.svg)](https://badge.fury.io/py/dashport) [![Documentation Status](https://readthedocs.org/projects/dashport/badge/?version=latest)](https://dashport.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dashport-0.7.4/dashport.egg-info/SOURCES.txt` & `dashport-0.7.5/dashport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/Makefile` & `dashport-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/buttons.md` & `dashport-0.7.5/docs/buttons.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/colors.md` & `dashport-0.7.5/docs/colors.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/conf.py` & `dashport-0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/dashport.md` & `dashport-0.7.5/docs/dashport.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/examples/boilerplate.md` & `dashport-0.7.5/docs/examples/boilerplate.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/examples/layouts.md` & `dashport-0.7.5/docs/examples/layouts.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/examples/views.md` & `dashport-0.7.5/docs/examples/views.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/images/Layout_quadrants.png` & `dashport-0.7.5/docs/images/Layout_quadrants.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/images/Layout_split_screen_horizontal.png` & `dashport-0.7.5/docs/images/Layout_split_screen_horizontal.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/images/Layout_split_screen_vert.png` & `dashport-0.7.5/docs/images/Layout_split_screen_vert.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/images/Layout_three_horizontal.png` & `dashport-0.7.5/docs/images/Layout_three_horizontal.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/images/Layout_three_vert.png` & `dashport-0.7.5/docs/images/Layout_three_vert.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/images/color_palette.png` & `dashport-0.7.5/docs/images/color_palette.png`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/index.rst` & `dashport-0.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/layouts.md` & `dashport-0.7.5/docs/layouts.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/panels.md` & `dashport-0.7.5/docs/panels.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/strings.md` & `dashport-0.7.5/docs/strings.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/docs/widgets.md` & `dashport-0.7.5/docs/widgets.md`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/boilerplate/basic_window.py` & `dashport-0.7.5/examples/boilerplate/basic_window.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/boilerplate/rectangle.py` & `dashport-0.7.5/examples/boilerplate/rectangle.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/boilerplate/using_buttons.py` & `dashport-0.7.5/examples/boilerplate/using_buttons.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/layouts/arbitrary_panels.py` & `dashport-0.7.5/examples/layouts/arbitrary_panels.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/layouts/custom_borders.py` & `dashport-0.7.5/examples/layouts/custom_borders.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/layouts/split_screen_columns.py` & `dashport-0.7.5/examples/layouts/split_screen_columns.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/layouts/split_screen_quad.py` & `dashport-0.7.5/examples/layouts/split_screen_quad.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/layouts/split_screen_rows.py` & `dashport-0.7.5/examples/layouts/split_screen_rows.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/layouts/split_screen_three_horizontal.py` & `dashport-0.7.5/examples/layouts/split_screen_three_horizontal.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/layouts/split_screen_three_vert.py` & `dashport-0.7.5/examples/layouts/split_screen_three_vert.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/util/all_ascii_constants.py` & `dashport-0.7.5/examples/util/all_ascii_constants.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/util/all_attributes_curses.py` & `dashport-0.7.5/examples/util/all_attributes_curses.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/util/all_box_drawing.py` & `dashport-0.7.5/examples/util/all_box_drawing.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/util/color_palette.py` & `dashport-0.7.5/examples/util/color_palette.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/util/explore_screen.py` & `dashport-0.7.5/examples/util/explore_screen.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/views/interactive_prompt.py` & `dashport-0.7.5/examples/views/interactive_prompt.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/views/multiple_views.py` & `dashport-0.7.5/examples/views/multiple_views.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/views/scroll_panels.py` & `dashport-0.7.5/examples/views/scroll_panels.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/examples/views/scroll_text.py` & `dashport-0.7.5/examples/views/scroll_text.py`

 * *Files identical despite different names*

### Comparing `dashport-0.7.4/setup.py` & `dashport-0.7.5/setup.py`

 * *Files identical despite different names*

