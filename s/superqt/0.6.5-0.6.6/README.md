# Comparing `tmp/superqt-0.6.5.tar.gz` & `tmp/superqt-0.6.6.tar.gz`

## Comparing `superqt-0.6.5.tar` & `superqt-0.6.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0    24220 2020-02-02 00:00:00.000000 superqt-0.6.5/CHANGELOG.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/py.typed
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/__init__.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_catalog_combo.py
--rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_combo.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_item_delegate.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_line_edit.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/collapsible/__init__.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/collapsible/_collapsible.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/__init__.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/_color_combobox.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/_enum_combobox.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/_searchable_combo_box.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/__init__.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/_eliding.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/_eliding_label.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/_eliding_line_edit.py
--rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_animations.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_iconfont.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_plugins.py
--rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_qfont_icon.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/iconify/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/qtcompat/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/selection/__init__.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/selection/_searchable_list_widget.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/selection/_searchable_tree_widget.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/__init__.py
--rw-r--r--   0        0        0    14428 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_generic_range_slider.py
--rw-r--r--   0        0        0    20299 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_generic_slider.py
--rw-r--r--   0        0        0    26313 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_labeled.py
--rw-r--r--   0        0        0     9656 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_range_style.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_sliders.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/spinbox/__init__.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/spinbox/_intspin.py
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/spinbox/_quantity.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/__init__.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_code_syntax_highlight.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_ensure_thread.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_errormsg_context.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_img_utils.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_message_handler.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_misc.py
--rw-r--r--   0        0        0    30760 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_qthreading.py
--rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_throttler.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_util.py
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_cmap.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_code_highlight.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_collapsible.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_color_combo.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_eliding_label.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_eliding_line_edit.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_ensure_thread.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_enum_comb_box.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_iconify.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_large_int_spinbox.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_qmessage_handler.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_quantity.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_searchable_combobox.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_searchable_list.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_searchable_tree.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_threadworker.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_throttler.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_utils.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/test_fonticon.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/test_plugins.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/__init__.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/_testutil.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_float.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_generic_slider.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_labeled_slider.py
--rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_range_slider.py
--rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_single_value_sliders.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_slider.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.6.5/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.6.5/LICENSE
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 superqt-0.6.5/README.md
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 superqt-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 superqt-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    24737 2020-02-02 00:00:00.000000 superqt-0.6.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/py.typed
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/cmap/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/cmap/_catalog_combo.py
+-rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/cmap/_cmap_combo.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/cmap/_cmap_item_delegate.py
+-rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/cmap/_cmap_line_edit.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/cmap/_cmap_utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/collapsible/__init__.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/collapsible/_collapsible.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/combobox/__init__.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/combobox/_color_combobox.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/combobox/_enum_combobox.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/combobox/_searchable_combo_box.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/elidable/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/elidable/_eliding.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/elidable/_eliding_label.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/elidable/_eliding_line_edit.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/fonticon/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/fonticon/_animations.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/fonticon/_iconfont.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/fonticon/_plugins.py
+-rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/fonticon/_qfont_icon.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/iconify/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/qtcompat/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/selection/__init__.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/selection/_searchable_list_widget.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/selection/_searchable_tree_widget.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/sliders/__init__.py
+-rw-r--r--   0        0        0    14428 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/sliders/_generic_range_slider.py
+-rw-r--r--   0        0        0    20299 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/sliders/_generic_slider.py
+-rw-r--r--   0        0        0    26313 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/sliders/_labeled.py
+-rw-r--r--   0        0        0     9656 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/sliders/_range_style.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/sliders/_sliders.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/spinbox/__init__.py
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/spinbox/_intspin.py
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/spinbox/_quantity.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/__init__.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_code_syntax_highlight.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_ensure_thread.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_errormsg_context.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_img_utils.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_message_handler.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_misc.py
+-rw-r--r--   0        0        0    30760 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_qthreading.py
+-rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_throttler.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.6/src/superqt/utils/_util.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_cmap.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_code_highlight.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_collapsible.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_color_combo.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_eliding_label.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_eliding_line_edit.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_ensure_thread.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_enum_comb_box.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_iconify.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_large_int_spinbox.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_qmessage_handler.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_quantity.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_searchable_combobox.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_searchable_list.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_searchable_tree.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_threadworker.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_throttler.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_utils.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_fonticon/test_fonticon.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_fonticon/test_plugins.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_fonticon/fixtures/fake_plugin/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/__init__.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/_testutil.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/test_float.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/test_generic_slider.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/test_labeled_slider.py
+-rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/test_range_slider.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/test_single_value_sliders.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 superqt-0.6.6/tests/zz_test_sliders/test_slider.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.6.6/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.6.6/LICENSE
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 superqt-0.6.6/README.md
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 superqt-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 superqt-0.6.6/PKG-INFO
```

### Comparing `superqt-0.6.5/CHANGELOG.md` & `superqt-0.6.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Changelog
 
+## [v0.6.6](https://github.com/pyapp-kit/superqt/tree/v0.6.6) (2024-05-12)
+
+[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.6.5...v0.6.6)
+
+**Refactors:**
+
+- perf: improve paint time for QColormapLineEdit [\#245](https://github.com/pyapp-kit/superqt/pull/245) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- ci: \[pre-commit.ci\] autoupdate [\#244](https://github.com/pyapp-kit/superqt/pull/244) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+
 ## [v0.6.5](https://github.com/pyapp-kit/superqt/tree/v0.6.5) (2024-05-06)
 
 [Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.6.4...v0.6.5)
 
-**Fixed bugs:**
+**Implemented enhancements:**
 
 - fix: fix a number of issues with Labeled and Range Sliders, add LabelsOnHandle mode. [\#242](https://github.com/pyapp-kit/superqt/pull/242) ([tlambert03](https://github.com/tlambert03))
 
 **Merged pull requests:**
 
 - ci: trying to fix tests on various platforms [\#243](https://github.com/pyapp-kit/superqt/pull/243) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `superqt-0.6.5/src/superqt/__init__.py` & `superqt-0.6.6/src/superqt/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/cmap/__init__.py` & `superqt-0.6.6/src/superqt/cmap/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/cmap/_catalog_combo.py` & `superqt-0.6.6/src/superqt/cmap/_catalog_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/cmap/_cmap_combo.py` & `superqt-0.6.6/src/superqt/cmap/_cmap_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/cmap/_cmap_item_delegate.py` & `superqt-0.6.6/src/superqt/cmap/_cmap_item_delegate.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/cmap/_cmap_line_edit.py` & `superqt-0.6.6/src/superqt/cmap/_cmap_line_edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
-from qtpy.QtCore import Qt
+from qtpy.QtCore import QRect, Qt
 from qtpy.QtGui import QIcon, QPainter, QPaintEvent, QPalette
 from qtpy.QtWidgets import QApplication, QLineEdit, QStyle, QWidget
 
 from ._cmap_utils import draw_colormap, pick_font_color, try_cast_colormap
 
 if TYPE_CHECKING:
     from cmap import Colormap
@@ -99,32 +99,37 @@
         palette = self.palette()
         palette.setColor(QPalette.ColorRole.Text, text)
         self.setPalette(palette)
 
     def _cmap_is_full_width(self):
         return self._colormap_fraction >= 0.75
 
+    def _cmap_rect(self) -> QRect:
+        cmap_rect = self.rect().adjusted(2, 0, 0, 0)
+        cmap_rect.setWidth(int(cmap_rect.width() * self._colormap_fraction))
+        return cmap_rect
+
+    def resizeEvent(self, e: Any) -> None:
+        left_margin = 6
+        if not self._cmap_is_full_width():
+            # leave room for the colormap
+            left_margin += self._cmap_rect().width()
+        self.setTextMargins(left_margin, 2, 0, 0)
+        super().resizeEvent(e)
+
     def paintEvent(self, e: QPaintEvent) -> None:
         # don't draw the background
         # otherwise it will cover the colormap during super().paintEvent
         # FIXME: this appears to need to be reset during every paint event...
         # otherwise something is resetting it
         palette = self.palette()
         palette.setColor(palette.ColorRole.Base, Qt.GlobalColor.transparent)
         self.setPalette(palette)
 
-        cmap_rect = self.rect().adjusted(2, 0, 0, 0)
-        cmap_rect.setWidth(int(cmap_rect.width() * self._colormap_fraction))
-
-        left_margin = 6
-        if not self._cmap_is_full_width():
-            # leave room for the colormap
-            left_margin += cmap_rect.width()
-        self.setTextMargins(left_margin, 2, 0, 0)
-
+        cmap_rect = self._cmap_rect()
         if self._cmap:
             draw_colormap(
                 self, self._cmap, cmap_rect, checkerboard_size=self._checkerboard_size
             )
         elif not self._cmap_is_full_width():
             if self._missing_cmap:
                 draw_colormap(self, self._missing_cmap, cmap_rect)
```

### Comparing `superqt-0.6.5/src/superqt/cmap/_cmap_utils.py` & `superqt-0.6.6/src/superqt/cmap/_cmap_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/collapsible/_collapsible.py` & `superqt-0.6.6/src/superqt/collapsible/_collapsible.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/combobox/__init__.py` & `superqt-0.6.6/src/superqt/combobox/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/combobox/_color_combobox.py` & `superqt-0.6.6/src/superqt/combobox/_color_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/combobox/_enum_combobox.py` & `superqt-0.6.6/src/superqt/combobox/_enum_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/combobox/_searchable_combo_box.py` & `superqt-0.6.6/src/superqt/combobox/_searchable_combo_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/elidable/_eliding.py` & `superqt-0.6.6/src/superqt/elidable/_eliding.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/elidable/_eliding_label.py` & `superqt-0.6.6/src/superqt/elidable/_eliding_label.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/elidable/_eliding_line_edit.py` & `superqt-0.6.6/src/superqt/elidable/_eliding_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/fonticon/__init__.py` & `superqt-0.6.6/src/superqt/fonticon/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/fonticon/_animations.py` & `superqt-0.6.6/src/superqt/fonticon/_animations.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/fonticon/_iconfont.py` & `superqt-0.6.6/src/superqt/fonticon/_iconfont.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/fonticon/_plugins.py` & `superqt-0.6.6/src/superqt/fonticon/_plugins.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/fonticon/_qfont_icon.py` & `superqt-0.6.6/src/superqt/fonticon/_qfont_icon.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/iconify/__init__.py` & `superqt-0.6.6/src/superqt/iconify/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/qtcompat/__init__.py` & `superqt-0.6.6/src/superqt/qtcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/selection/_searchable_list_widget.py` & `superqt-0.6.6/src/superqt/selection/_searchable_list_widget.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/selection/_searchable_tree_widget.py` & `superqt-0.6.6/src/superqt/selection/_searchable_tree_widget.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/sliders/_generic_range_slider.py` & `superqt-0.6.6/src/superqt/sliders/_generic_range_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/sliders/_generic_slider.py` & `superqt-0.6.6/src/superqt/sliders/_generic_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/sliders/_labeled.py` & `superqt-0.6.6/src/superqt/sliders/_labeled.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/sliders/_range_style.py` & `superqt-0.6.6/src/superqt/sliders/_range_style.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/sliders/_sliders.py` & `superqt-0.6.6/src/superqt/sliders/_sliders.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/spinbox/_intspin.py` & `superqt-0.6.6/src/superqt/spinbox/_intspin.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/spinbox/_quantity.py` & `superqt-0.6.6/src/superqt/spinbox/_quantity.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/__init__.py` & `superqt-0.6.6/src/superqt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_code_syntax_highlight.py` & `superqt-0.6.6/src/superqt/utils/_code_syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_ensure_thread.py` & `superqt-0.6.6/src/superqt/utils/_ensure_thread.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_errormsg_context.py` & `superqt-0.6.6/src/superqt/utils/_errormsg_context.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_img_utils.py` & `superqt-0.6.6/src/superqt/utils/_img_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_message_handler.py` & `superqt-0.6.6/src/superqt/utils/_message_handler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_misc.py` & `superqt-0.6.6/src/superqt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_qthreading.py` & `superqt-0.6.6/src/superqt/utils/_qthreading.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_throttler.py` & `superqt-0.6.6/src/superqt/utils/_throttler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/src/superqt/utils/_util.py` & `superqt-0.6.6/src/superqt/utils/_util.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_cmap.py` & `superqt-0.6.6/tests/test_cmap.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_code_highlight.py` & `superqt-0.6.6/tests/test_code_highlight.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_collapsible.py` & `superqt-0.6.6/tests/test_collapsible.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_color_combo.py` & `superqt-0.6.6/tests/test_color_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_eliding_label.py` & `superqt-0.6.6/tests/test_eliding_label.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_eliding_line_edit.py` & `superqt-0.6.6/tests/test_eliding_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_ensure_thread.py` & `superqt-0.6.6/tests/test_ensure_thread.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_enum_comb_box.py` & `superqt-0.6.6/tests/test_enum_comb_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_iconify.py` & `superqt-0.6.6/tests/test_iconify.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_large_int_spinbox.py` & `superqt-0.6.6/tests/test_large_int_spinbox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_qmessage_handler.py` & `superqt-0.6.6/tests/test_qmessage_handler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_quantity.py` & `superqt-0.6.6/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_searchable_combobox.py` & `superqt-0.6.6/tests/test_searchable_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_searchable_list.py` & `superqt-0.6.6/tests/test_searchable_list.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_searchable_tree.py` & `superqt-0.6.6/tests/test_searchable_tree.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_threadworker.py` & `superqt-0.6.6/tests/test_threadworker.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_throttler.py` & `superqt-0.6.6/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_utils.py` & `superqt-0.6.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_fonticon/test_fonticon.py` & `superqt-0.6.6/tests/test_fonticon/test_fonticon.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_fonticon/test_plugins.py` & `superqt-0.6.6/tests/test_fonticon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf` & `superqt-0.6.6/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/zz_test_sliders/_testutil.py` & `superqt-0.6.6/tests/zz_test_sliders/_testutil.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/zz_test_sliders/test_float.py` & `superqt-0.6.6/tests/zz_test_sliders/test_float.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/zz_test_sliders/test_generic_slider.py` & `superqt-0.6.6/tests/zz_test_sliders/test_generic_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/zz_test_sliders/test_labeled_slider.py` & `superqt-0.6.6/tests/zz_test_sliders/test_labeled_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/zz_test_sliders/test_range_slider.py` & `superqt-0.6.6/tests/zz_test_sliders/test_range_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/zz_test_sliders/test_single_value_sliders.py` & `superqt-0.6.6/tests/zz_test_sliders/test_single_value_sliders.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/tests/zz_test_sliders/test_slider.py` & `superqt-0.6.6/tests/zz_test_sliders/test_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/.gitignore` & `superqt-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/LICENSE` & `superqt-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/README.md` & `superqt-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/pyproject.toml` & `superqt-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `superqt-0.6.5/PKG-INFO` & `superqt-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: superqt
-Version: 0.6.5
+Version: 0.6.6
 Summary: Missing widgets and components for PyQt/PySide
 Project-URL: Documentation, https://pyapp-kit.github.io/superqt/
 Project-URL: Source, https://github.com/pyapp-kit/superqt
 Project-URL: Tracker, https://github.com/pyapp-kit/superqt/issues
 Project-URL: Changelog, https://github.com/pyapp-kit/superqt/blob/main/CHANGELOG.md
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
```

