# Comparing `tmp/compoundwidgets-0.4.1.tar.gz` & `tmp/compoundwidgets-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compoundwidgets-0.4.1.tar", last modified: Thu Feb 29 16:08:23 2024, max compression
+gzip compressed data, was "compoundwidgets-0.4.2.tar", last modified: Mon Apr 15 11:03:13 2024, max compression
```

## Comparing `compoundwidgets-0.4.1.tar` & `compoundwidgets-0.4.2.tar`

### file list

```diff
@@ -1,57 +1,1008 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 16:08:23.196374 compoundwidgets-0.4.1/
--rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1735 2024-02-29 16:08:23.194337 compoundwidgets-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-10-04 16:52:18.000000 compoundwidgets-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 16:08:23.115484 compoundwidgets-0.4.1/compoundwidgets/
--rw-rw-rw-   0        0        0    13086 2024-02-29 16:06:14.000000 compoundwidgets-0.4.1/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
--rw-rw-rw-   0        0        0    69664 2024-02-29 14:18:23.000000 compoundwidgets-0.4.1/compoundwidgets/COMPOUND_WIDGETS.py
--rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.4.1/compoundwidgets/CUSTOM_BUTTONS.py
--rw-rw-rw-   0        0        0    20214 2024-02-29 12:52:04.000000 compoundwidgets-0.4.1/compoundwidgets/CUSTOM_FRAMES.py
-drwxrwxrwx   0        0        0        0 2024-02-29 16:08:23.159842 compoundwidgets-0.4.1/compoundwidgets/IMAGES/
--rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/__init__.py
--rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/add_new.png
--rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/add_to_form.png
--rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/back.png
--rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/calculate.png
--rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/clear.png
--rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/edit_form.png
--rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/help.png
--rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/no.png
--rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/quit.png
--rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/remove_from_form.png
--rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/save.png
--rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/trash_can.png
--rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.4.1/compoundwidgets/IMAGES/yes.png
--rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.4.1/compoundwidgets/LED_BUTTONS.py
--rw-rw-rw-   0        0        0    13821 2024-02-29 12:55:40.000000 compoundwidgets-0.4.1/compoundwidgets/MESSAGE_BOX_WIDGETS.py
--rw-rw-rw-   0        0        0    10139 2024-02-29 16:06:14.000000 compoundwidgets-0.4.1/compoundwidgets/SCRIPTS.py
--rw-rw-rw-   0        0        0     1997 2024-02-29 16:07:26.000000 compoundwidgets-0.4.1/compoundwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 16:08:23.129438 compoundwidgets-0.4.1/compoundwidgets.egg-info/
--rw-rw-rw-   0        0        0     1735 2024-02-29 16:08:22.000000 compoundwidgets-0.4.1/compoundwidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2024-02-29 16:08:23.000000 compoundwidgets-0.4.1/compoundwidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 16:08:22.000000 compoundwidgets-0.4.1/compoundwidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-02-29 16:08:22.000000 compoundwidgets-0.4.1/compoundwidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-02-29 16:08:22.000000 compoundwidgets-0.4.1/compoundwidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 16:08:23.196374 compoundwidgets-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      676 2024-02-29 16:07:26.000000 compoundwidgets-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-29 16:08:23.193263 compoundwidgets-0.4.1/test/
--rw-rw-rw-   0        0        0      472 2023-05-31 15:58:06.000000 compoundwidgets-0.4.1/test/autocomplete_combobox_test.py
--rw-rw-rw-   0        0        0     2945 2023-11-02 09:55:54.000000 compoundwidgets-0.4.1/test/autocomplete_entry_list_test.py
--rw-rw-rw-   0        0        0     1079 2023-09-22 10:09:37.000000 compoundwidgets-0.4.1/test/autocomplete_labelcombo_test.py
--rw-rw-rw-   0        0        0     2251 2024-02-29 13:24:58.000000 compoundwidgets-0.4.1/test/compound_widgets_test_1_labelcombo.py
--rw-rw-rw-   0        0        0     2613 2024-02-29 13:50:33.000000 compoundwidgets-0.4.1/test/compound_widgets_test_2_labelentry.py
--rw-rw-rw-   0        0        0     2450 2024-02-29 13:26:18.000000 compoundwidgets-0.4.1/test/compound_widgets_test_3_labelspinbox.py
--rw-rw-rw-   0        0        0     3117 2024-02-29 13:27:31.000000 compoundwidgets-0.4.1/test/compound_widgets_test_4_labeltext.py
--rw-rw-rw-   0        0        0     4134 2024-02-29 13:28:54.000000 compoundwidgets-0.4.1/test/compound_widgets_test_5_labelentryunit.py
--rw-rw-rw-   0        0        0     1589 2024-02-29 14:18:43.000000 compoundwidgets-0.4.1/test/compound_widgets_test_6_labelentrybutton.py
--rw-rw-rw-   0        0        0     1689 2024-02-29 13:30:25.000000 compoundwidgets-0.4.1/test/compound_widgets_test_7_labelcombobutton.py
--rw-rw-rw-   0        0        0      991 2023-04-26 10:06:43.000000 compoundwidgets-0.4.1/test/custom_buttons_test.py
--rw-rw-rw-   0        0        0     2590 2023-10-08 18:33:49.000000 compoundwidgets-0.4.1/test/frames_test_1_collapsable_frames.py
--rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.4.1/test/frames_test_2_v_collapsable_frames.py
--rw-rw-rw-   0        0        0      978 2023-10-07 12:11:53.000000 compoundwidgets-0.4.1/test/frames_test_3_scrollable_frames.py
--rw-rw-rw-   0        0        0     2689 2023-09-22 10:44:22.000000 compoundwidgets-0.4.1/test/frames_test_4_scrollable_with_collapsable.py
--rw-rw-rw-   0        0        0     1329 2024-02-29 12:53:41.000000 compoundwidgets-0.4.1/test/frames_test_5_border_frames.py
--rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.4.1/test/led_buttons_test.py
--rw-rw-rw-   0        0        0     3975 2024-02-29 12:56:19.000000 compoundwidgets-0.4.1/test/message_box_test.py
--rw-rw-rw-   0        0        0      894 2023-05-10 10:34:22.000000 compoundwidgets-0.4.1/test/test_variable_tracing.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:13.243358 compoundwidgets-0.4.2/
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:10.940453 compoundwidgets-0.4.2/.venv/
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:10.878715 compoundwidgets-0.4.2/.venv/Lib/
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:10.961618 compoundwidgets-0.4.2/.venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.146495 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/
+-rw-rw-rw-   0        0        0     3602 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/BdfFontFile.py
+-rw-rw-rw-   0        0        0    16032 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/BlpImagePlugin.py
+-rw-rw-rw-   0        0        0    18205 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/BmpImagePlugin.py
+-rw-rw-rw-   0        0        0     1666 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
+-rw-rw-rw-   0        0        0     3302 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ContainerIO.py
+-rw-rw-rw-   0        0        0     1816 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/CurImagePlugin.py
+-rw-rw-rw-   0        0        0     2073 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/DcxImagePlugin.py
+-rw-rw-rw-   0        0        0    17283 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/DdsImagePlugin.py
+-rw-rw-rw-   0        0        0    16283 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/EpsImagePlugin.py
+-rw-rw-rw-   0        0        0    10134 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ExifTags.py
+-rw-rw-rw-   0        0        0     4638 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/FitsImagePlugin.py
+-rw-rw-rw-   0        0        0     4737 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/FliImagePlugin.py
+-rw-rw-rw-   0        0        0     3711 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/FontFile.py
+-rw-rw-rw-   0        0        0     7238 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/FpxImagePlugin.py
+-rw-rw-rw-   0        0        0     3581 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/FtexImagePlugin.py
+-rw-rw-rw-   0        0        0     3048 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/GbrImagePlugin.py
+-rw-rw-rw-   0        0        0     2897 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/GdImageFile.py
+-rw-rw-rw-   0        0        0    38827 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/GifImagePlugin.py
+-rw-rw-rw-   0        0        0     3567 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/GimpGradientFile.py
+-rw-rw-rw-   0        0        0     1437 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/GimpPaletteFile.py
+-rw-rw-rw-   0        0        0     1660 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/GribStubImagePlugin.py
+-rw-rw-rw-   0        0        0     1663 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
+-rw-rw-rw-   0        0        0    12396 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/IcnsImagePlugin.py
+-rw-rw-rw-   0        0        0    11998 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/IcoImagePlugin.py
+-rw-rw-rw-   0        0        0    11275 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImImagePlugin.py
+-rw-rw-rw-   0        0        0   141051 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/Image.py
+-rw-rw-rw-   0        0        0     8257 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageChops.py
+-rw-rw-rw-   0        0        0    42455 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageCms.py
+-rw-rw-rw-   0        0        0     9514 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageColor.py
+-rw-rw-rw-   0        0        0    38849 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageDraw.py
+-rw-rw-rw-   0        0        0     5728 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageDraw2.py
+-rw-rw-rw-   0        0        0     3329 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageEnhance.py
+-rw-rw-rw-   0        0        0    25218 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageFile.py
+-rw-rw-rw-   0        0        0    17598 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageFilter.py
+-rw-rw-rw-   0        0        0    61820 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageFont.py
+-rw-rw-rw-   0        0        0     6284 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageGrab.py
+-rw-rw-rw-   0        0        0    11837 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageMath.py
+-rw-rw-rw-   0        0        0     2866 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageMode.py
+-rw-rw-rw-   0        0        0     8748 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageMorph.py
+-rw-rw-rw-   0        0        0    25496 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageOps.py
+-rw-rw-rw-   0        0        0     8128 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImagePalette.py
+-rw-rw-rw-   0        0        0      391 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImagePath.py
+-rw-rw-rw-   0        0        0     6157 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageQt.py
+-rw-rw-rw-   0        0        0     2278 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageSequence.py
+-rw-rw-rw-   0        0        0     9792 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageShow.py
+-rw-rw-rw-   0        0        0     3853 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageStat.py
+-rw-rw-rw-   0        0        0     8780 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageTk.py
+-rw-rw-rw-   0        0        0     4036 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageTransform.py
+-rw-rw-rw-   0        0        0     7457 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImageWin.py
+-rw-rw-rw-   0        0        0     2761 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/ImtImagePlugin.py
+-rw-rw-rw-   0        0        0     6370 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/IptcImagePlugin.py
+-rw-rw-rw-   0        0        0    12317 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
+-rw-rw-rw-   0        0        0    30446 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/JpegImagePlugin.py
+-rw-rw-rw-   0        0        0    12664 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/JpegPresets.py
+-rw-rw-rw-   0        0        0     1979 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/McIdasImagePlugin.py
+-rw-rw-rw-   0        0        0     2722 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/MicImagePlugin.py
+-rw-rw-rw-   0        0        0     2092 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/MpegImagePlugin.py
+-rw-rw-rw-   0        0        0     5969 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/MpoImagePlugin.py
+-rw-rw-rw-   0        0        0     6028 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/MspImagePlugin.py
+-rw-rw-rw-   0        0        0     6790 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PSDraw.py
+-rw-rw-rw-   0        0        0     1215 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PaletteFile.py
+-rw-rw-rw-   0        0        0     9405 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PalmImagePlugin.py
+-rw-rw-rw-   0        0        0     1689 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PcdImagePlugin.py
+-rw-rw-rw-   0        0        0     7401 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PcfFontFile.py
+-rw-rw-rw-   0        0        0     6436 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PcxImagePlugin.py
+-rw-rw-rw-   0        0        0     9152 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PdfImagePlugin.py
+-rw-rw-rw-   0        0        0    35694 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PdfParser.py
+-rw-rw-rw-   0        0        0     1818 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PixarImagePlugin.py
+-rw-rw-rw-   0        0        0    48352 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PngImagePlugin.py
+-rw-rw-rw-   0        0        0    12579 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PpmImagePlugin.py
+-rw-rw-rw-   0        0        0     8012 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PsdImagePlugin.py
+-rw-rw-rw-   0        0        0    10284 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/PyAccess.py
+-rw-rw-rw-   0        0        0     3928 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/QoiImagePlugin.py
+-rw-rw-rw-   0        0        0     6636 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/SgiImagePlugin.py
+-rw-rw-rw-   0        0        0     9785 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/SpiderImagePlugin.py
+-rw-rw-rw-   0        0        0     4640 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/SunImagePlugin.py
+-rw-rw-rw-   0        0        0     1812 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/TarIO.py
+-rw-rw-rw-   0        0        0     7189 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/TgaImagePlugin.py
+-rw-rw-rw-   0        0        0    79378 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/TiffImagePlugin.py
+-rw-rw-rw-   0        0        0    17232 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/TiffTags.py
+-rw-rw-rw-   0        0        0     5679 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/WalImageFile.py
+-rw-rw-rw-   0        0        0    11892 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/WebPImagePlugin.py
+-rw-rw-rw-   0        0        0     4905 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/WmfImagePlugin.py
+-rw-rw-rw-   0        0        0     2162 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
+-rw-rw-rw-   0        0        0     2739 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/XbmImagePlugin.py
+-rw-rw-rw-   0        0        0     3352 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/XpmImagePlugin.py
+-rw-rw-rw-   0        0        0     2094 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/__init__.py
+-rw-rw-rw-   0        0        0      140 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/__main__.py
+-rw-rw-rw-   0        0        0     2662 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/_binary.py
+-rw-rw-rw-   0        0        0     2071 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/_deprecate.py
+-rw-rw-rw-   0        0        0      561 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/_tkinter_finder.py
+-rw-rw-rw-   0        0        0      809 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/_typing.py
+-rw-rw-rw-   0        0        0      844 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/_util.py
+-rw-rw-rw-   0        0        0       91 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/_version.py
+-rw-rw-rw-   0        0        0    10499 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/features.py
+-rw-rw-rw-   0        0        0      105 2024-04-15 11:00:53.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/PIL/report.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.151580 compoundwidgets-0.4.2/.venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     6002 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/_distutils_hack/override.py
+-rw-rw-rw-   0        0        0     4431 2024-04-15 10:59:58.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/_virtualenv.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.158088 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      355 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0      854 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.177360 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      515 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10243 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0    10370 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.200348 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6690 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     8733 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    30064 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2816 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10781 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18369 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.240265 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7944 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1782 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4287 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9766 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6777 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5335 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     3172 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4775 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3188 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    28782 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12450 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6419 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3886 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     6476 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    14006 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.250785 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1743 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      842 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6709 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1277 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    23634 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.259482 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16590 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37843 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     8688 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.267480 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    15365 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6009 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7680 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2556 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.276203 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4339 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2627 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25907 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.284507 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      135 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8297 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7456 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0    10035 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.305455 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      931 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     6889 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2486 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2818 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    20777 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4643 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     4272 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.323947 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    20541 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     3935 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6086 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18698 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1838 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.332090 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.349148 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4832 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1422 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1474 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1075 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1417 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     6806 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9816 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.356469 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1282 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0    27311 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    28128 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     7152 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.369591 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2738 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    19018 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17790 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    35460 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     4704 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24551 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.374519 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.377934 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24025 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.397327 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5173 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    21052 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    32292 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9824 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     3100 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5696 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    12592 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8378 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.455093 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     3351 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-rw-rw-   0        0        0     1015 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     3627 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     2463 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3113 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     5118 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0    11603 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    23623 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     4435 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9207 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     9312 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3456 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4499 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.467368 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18121 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5249 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11729 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22787 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    11801 2024-04-15 11:00:23.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.474475 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4993 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.493622 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      676 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1737 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     6392 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1952 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.499337 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      303 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5352 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1386 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0    18384 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     4292 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4828 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7173 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0     1417 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.505343 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.600972 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     4797 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1763 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0    10032 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3915 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     5420 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.604972 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     3242 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3732 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0      542 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-rw-   0        0        0     1860 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1683 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     4006 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12176 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3934 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1753 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1753 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1759 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    14537 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1752 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    27055 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5380 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     6077 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-rw-   0        0        0     3715 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2131 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30391 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.608497 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13560 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0      402 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-rw-   0        0        0     6400 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4137 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     4007 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    14848 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8505 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2812 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      244 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.622211 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      266 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.637540 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.673684 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      625 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41487 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51965 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20797 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51767 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14168 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5268 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39693 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18315 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    67530 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23747 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43958 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.681519 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    49330 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.700697 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.709154 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6079 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34544 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.734311 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.736311 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   109364 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.753497 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    20155 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1476 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     7211 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     7132 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     3678 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     8809 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     9573 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.785136 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2983 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.788234 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     4178 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.821360 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     5424 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4176 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5094 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35610 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     4981 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    34618 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.827387 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    12130 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    72281 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53424 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     6882 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.829422 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3700 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63223 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0    10230 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.854880 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9116 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6567 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    13387 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   224445 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.855878 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    24215 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9523 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    38646 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    26692 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13488 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10646 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     8670 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.864414 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-rw-   0        0        0      491 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-rw-   0        0        0      138 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-rw-   0        0        0    11920 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.869464 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-rw-   0        0        0      546 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-rw-   0        0        0    10927 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.910524 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5169 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1495 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    19697 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6449 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35288 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30373 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33460 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.921729 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:11.925647 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5871 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1601 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    20511 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4963 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.105339 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     6090 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8478 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2100 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0      799 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
+-rw-rw-rw-   0        0        0     9695 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     1387 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6906 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9842 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4509 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    18224 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    99218 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     8082 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1683 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9584 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5032 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14007 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14273 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11903 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    35852 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59706 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4431 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4602 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2843 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24247 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4339 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    27073 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    35173 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39684 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45525 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3777 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    29604 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.129572 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    20493 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3551 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     2179 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1682 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1562 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     2372 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     8746 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     3086 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2142 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8024 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.139950 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.154830 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/truststore/
+-rw-rw-rw-   0        0        0      403 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/truststore/__init__.py
+-rw-rw-rw-   0        0        0     9893 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/truststore/_api.py
+-rw-rw-rw-   0        0        0    17694 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/truststore/_macos.py
+-rw-rw-rw-   0        0        0     2324 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-rw-rw-   0        0        0     1130 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-rw-rw-   0        0        0    17468 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/truststore/_windows.py
+-rw-rw-rw-   0        0        0   111130 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.175990 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20300 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39990 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.191075 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.197582 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11036 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17081 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.201670 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.209585 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0     5343 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-rw-rw-   0        0        0    34665 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19752 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     6691 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30641 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.240929 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22013 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10168 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14296 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.255860 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2024-04-15 11:00:24.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.258381 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   108932 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.265386 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.269523 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/backports/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/backports/__init__.py
+-rw-rw-rw-   0        0        0   106920 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/backports/tarfile.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.291931 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     5457 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2925 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3481 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     5140 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3581 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2576 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.295931 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     9573 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.298335 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools/
+-rw-rw-rw-   0        0        0    16705 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.300806 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.308331 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0      149 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   143053 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    27548 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.333566 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      496 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     9590 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2676 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0    10347 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5292 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8208 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0    33036 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/metadata.py
+-rw-rw-rw-   0        0        0     2933 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39784 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18950 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     5268 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    16236 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.348461 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12806 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4068 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4910 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2655 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6911 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6596 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-rw-rw-   0        0        0    80078 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.349464 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2459 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.411514 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     9545 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0     9206 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_core_metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.488284 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      359 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     5440 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0     1771 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0     1453 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/_itertools.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/_log.py
+-rw-rw-rw-   0        0        0      239 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0     2411 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/_modified.py
+-rw-rw-rw-   0        0        0    19613 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8572 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14662 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    48645 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17801 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.535583 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1609 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5353 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4596 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    21717 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5575 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7686 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31793 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16539 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5536 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4912 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2595 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13007 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30128 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2757 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2788 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1180 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8408 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1933 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0    11805 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19188 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7497 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.540646 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/compat/
+-rw-rw-rw-   0        0        0      417 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/compat/__init__.py
+-rw-rw-rw-   0        0        0      567 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/compat/py38.py
+-rw-rw-rw-   0        0        0     5226 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9372 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    11945 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0      349 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     7965 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50116 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10197 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17831 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     7926 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13635 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1200 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30108 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23443 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      205 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0     1964 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3431 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18485 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12100 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15572 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18120 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12648 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5205 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     6573 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_distutils/zosccompiler.py
+-rw-rw-rw-   0        0        0     2235 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2433 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1468 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0     4567 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_normalization.py
+-rw-rw-rw-   0        0        0     1178 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_path.py
+-rw-rw-rw-   0        0        0     1112 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.549177 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.554180 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/backports/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/backports/__init__.py
+-rw-rw-rw-   0        0        0   106920 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/backports/tarfile.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.572783 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    26498 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     2454 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1859 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1165 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     1098 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-rw-rw-   0        0        0     2166 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.594236 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     5457 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2925 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3481 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     5140 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3581 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2576 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.598705 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     9570 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.601704 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/functools/
+-rw-rw-rw-   0        0        0    16696 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/functools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.604793 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.611583 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.640571 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      496 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0     3266 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-rw-rw-   0        0        0     9590 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     2676 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0    10347 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-rw-rw-   0        0        0     1431 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     5292 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-rw-rw-   0        0        0     8208 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0    33036 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/metadata.py
+-rw-rw-rw-   0        0        0     2933 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    39784 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    18950 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     5268 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    16236 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.647143 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7331 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    18740 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.703646 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     4222 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/_requirestxt.py
+-rw-rw-rw-   0        0        0     2383 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16433 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1289 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6598 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4539 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    17724 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    15127 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     6834 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     3507 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    87138 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    34488 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    26516 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5815 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2066 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3870 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2359 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0      468 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2132 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      657 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     6811 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     4927 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8101 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7821 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.711141 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/compat/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/compat/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/compat/py310.py
+-rw-rw-rw-   0        0        0      330 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/compat/py311.py
+-rw-rw-rw-   0        0        0      493 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/compat/py39.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.721528 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/
+-rw-rw-rw-   0        0        0     1499 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    14791 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.733152 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   274893 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     9160 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16456 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    17383 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25630 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      659 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5599 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    21152 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    37504 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2669 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5807 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.736152 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2556 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4852 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     4969 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1239 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0      190 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/modified.py
+-rw-rw-rw-   0        0        0     4303 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47476 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3131 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    38376 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0    14699 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      962 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      161 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     3697 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/warnings.py
+-rw-rw-rw-   0        0        0     8628 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      720 2024-04-15 11:01:49.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.776433 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/
+-rw-rw-rw-   0        0        0      396 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/__init__.py
+-rw-rw-rw-   0        0        0     8926 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/__main__.py
+-rw-rw-rw-   0        0        0     5255 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/colorutils.py
+-rw-rw-rw-   0        0        0      775 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.784037 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/dialogs/
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/dialogs/__init__.py
+-rw-rw-rw-   0        0        0    22700 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/dialogs/colorchooser.py
+-rw-rw-rw-   0        0        0     6885 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/dialogs/colordropper.py
+-rw-rw-rw-   0        0        0    64245 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/dialogs/dialogs.py
+-rw-rw-rw-   0        0        0   118811 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/icons.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.790973 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/localization/
+-rw-rw-rw-   0        0        0      675 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/localization/__init__.py
+-rw-rw-rw-   0        0        0     5594 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/localization/msgcat.py
+-rw-rw-rw-   0        0        0    15106 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/localization/msgs.py
+-rw-rw-rw-   0        0        0     2879 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/publisher.py
+-rw-rw-rw-   0        0        0    15839 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/scrolled.py
+-rw-rw-rw-   0        0        0   172335 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/style.py
+-rw-rw-rw-   0        0        0    92575 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/tableview.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.795972 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/themes/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/themes/__init__.py
+-rw-rw-rw-   0        0        0    11286 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/themes/standard.py
+-rw-rw-rw-   0        0        0       14 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/themes/user.py
+-rw-rw-rw-   0        0        0     8389 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/toast.py
+-rw-rw-rw-   0        0        0     5139 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/tooltip.py
+-rw-rw-rw-   0        0        0     3555 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/utility.py
+-rw-rw-rw-   0        0        0    10200 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/validation.py
+-rw-rw-rw-   0        0        0    40690 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/widgets.py
+-rw-rw-rw-   0        0        0    18186 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkbootstrap/window.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.800573 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkcreator/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkcreator/__init__.py
+-rw-rw-rw-   0        0        0    17276 2024-04-15 11:00:55.000000 compoundwidgets-0.4.2/.venv/Lib/site-packages/ttkcreator/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.801574 compoundwidgets-0.4.2/.venv/Scripts/
+-rw-rw-rw-   0        0        0     1332 2024-04-15 11:00:07.000000 compoundwidgets-0.4.2/.venv/Scripts/activate_this.py
+-rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1735 2024-04-15 11:03:13.240498 compoundwidgets-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-10-04 16:52:18.000000 compoundwidgets-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:12.947444 compoundwidgets-0.4.2/compoundwidgets/
+-rw-rw-rw-   0        0        0    13086 2024-02-29 16:06:14.000000 compoundwidgets-0.4.2/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
+-rw-rw-rw-   0        0        0    69664 2024-04-15 10:55:44.000000 compoundwidgets-0.4.2/compoundwidgets/COMPOUND_WIDGETS.py
+-rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.4.2/compoundwidgets/CUSTOM_BUTTONS.py
+-rw-rw-rw-   0        0        0    20758 2024-03-15 19:39:05.000000 compoundwidgets-0.4.2/compoundwidgets/CUSTOM_FRAMES.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:13.037150 compoundwidgets-0.4.2/compoundwidgets/IMAGES/
+-rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/__init__.py
+-rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/add_new.png
+-rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/add_to_form.png
+-rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/back.png
+-rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/calculate.png
+-rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/clear.png
+-rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/edit_form.png
+-rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/help.png
+-rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/no.png
+-rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/quit.png
+-rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/remove_from_form.png
+-rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/save.png
+-rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/trash_can.png
+-rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.4.2/compoundwidgets/IMAGES/yes.png
+-rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.4.2/compoundwidgets/LED_BUTTONS.py
+-rw-rw-rw-   0        0        0    13865 2024-03-28 11:25:34.000000 compoundwidgets-0.4.2/compoundwidgets/MESSAGE_BOX_WIDGETS.py
+-rw-rw-rw-   0        0        0    10139 2024-02-29 16:06:14.000000 compoundwidgets-0.4.2/compoundwidgets/SCRIPTS.py
+-rw-rw-rw-   0        0        0     1997 2024-04-15 10:56:46.000000 compoundwidgets-0.4.2/compoundwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:13.238484 compoundwidgets-0.4.2/compoundwidgets.egg-info/
+-rw-rw-rw-   0        0        0     1735 2024-04-15 11:03:10.000000 compoundwidgets-0.4.2/compoundwidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    50645 2024-04-15 11:03:10.000000 compoundwidgets-0.4.2/compoundwidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:03:10.000000 compoundwidgets-0.4.2/compoundwidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-15 11:03:10.000000 compoundwidgets-0.4.2/compoundwidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 11:03:10.000000 compoundwidgets-0.4.2/compoundwidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:03:13.243358 compoundwidgets-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      676 2024-04-15 10:56:46.000000 compoundwidgets-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:03:13.235040 compoundwidgets-0.4.2/test/
+-rw-rw-rw-   0        0        0      472 2023-05-31 15:58:06.000000 compoundwidgets-0.4.2/test/autocomplete_combobox_test.py
+-rw-rw-rw-   0        0        0     2945 2023-11-02 09:55:54.000000 compoundwidgets-0.4.2/test/autocomplete_entry_list_test.py
+-rw-rw-rw-   0        0        0     1079 2023-09-22 10:09:37.000000 compoundwidgets-0.4.2/test/autocomplete_labelcombo_test.py
+-rw-rw-rw-   0        0        0     2251 2024-02-29 13:24:58.000000 compoundwidgets-0.4.2/test/compound_widgets_test_1_labelcombo.py
+-rw-rw-rw-   0        0        0     2613 2024-02-29 13:50:33.000000 compoundwidgets-0.4.2/test/compound_widgets_test_2_labelentry.py
+-rw-rw-rw-   0        0        0     2450 2024-02-29 13:26:18.000000 compoundwidgets-0.4.2/test/compound_widgets_test_3_labelspinbox.py
+-rw-rw-rw-   0        0        0     3117 2024-02-29 13:27:31.000000 compoundwidgets-0.4.2/test/compound_widgets_test_4_labeltext.py
+-rw-rw-rw-   0        0        0     4134 2024-02-29 13:28:54.000000 compoundwidgets-0.4.2/test/compound_widgets_test_5_labelentryunit.py
+-rw-rw-rw-   0        0        0     1589 2024-02-29 14:18:43.000000 compoundwidgets-0.4.2/test/compound_widgets_test_6_labelentrybutton.py
+-rw-rw-rw-   0        0        0     1689 2024-02-29 13:30:25.000000 compoundwidgets-0.4.2/test/compound_widgets_test_7_labelcombobutton.py
+-rw-rw-rw-   0        0        0      991 2023-04-26 10:06:43.000000 compoundwidgets-0.4.2/test/custom_buttons_test.py
+-rw-rw-rw-   0        0        0     2590 2023-10-08 18:33:49.000000 compoundwidgets-0.4.2/test/frames_test_1_collapsable_frames.py
+-rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.4.2/test/frames_test_2_v_collapsable_frames.py
+-rw-rw-rw-   0        0        0      978 2023-10-07 12:11:53.000000 compoundwidgets-0.4.2/test/frames_test_3_scrollable_frames.py
+-rw-rw-rw-   0        0        0     2689 2023-09-22 10:44:22.000000 compoundwidgets-0.4.2/test/frames_test_4_scrollable_with_collapsable.py
+-rw-rw-rw-   0        0        0     1329 2024-02-29 12:53:41.000000 compoundwidgets-0.4.2/test/frames_test_5_border_frames.py
+-rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.4.2/test/led_buttons_test.py
+-rw-rw-rw-   0        0        0     3975 2024-02-29 12:56:19.000000 compoundwidgets-0.4.2/test/message_box_test.py
+-rw-rw-rw-   0        0        0      894 2023-05-10 10:34:22.000000 compoundwidgets-0.4.2/test/test_variable_tracing.py
```

### Comparing `compoundwidgets-0.4.1/LICENSE.txt` & `compoundwidgets-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/MANIFEST.in` & `compoundwidgets-0.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/PKG-INFO` & `compoundwidgets-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compoundwidgets
-Version: 0.4.1
+Version: 0.4.2
 Summary: Compound TTK Widgets with ttkbootstrap
 Home-page: https://github.com/AndreMariano100/CompoundWidgets.git
 Author: Andre Mariano
 Author-email: andremariano100@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `compoundwidgets-0.4.1/README.md` & `compoundwidgets-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/AUTOCOMPLETE_WIDGETS.py` & `compoundwidgets-0.4.2/compoundwidgets/AUTOCOMPLETE_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/COMPOUND_WIDGETS.py` & `compoundwidgets-0.4.2/compoundwidgets/COMPOUND_WIDGETS.py`

 * *Files 0% similar despite different names*

```diff
@@ -838,15 +838,15 @@
                            state='readonly')
 
     class ThermalExpansionCombo(ttk.Combobox):
         def __init__(self, parent, width):
             super().__init__(parent)
 
             self.values = ('10e-6/°C', '10e-6/°F')
-            self.conversion_values = (1, 0.55556)
+            self.conversion_values = (1, 1.79856)
             self.variable = tk.StringVar(value=self.values[0])
             self.configure(textvariable=self.variable, justify='center', width=width, values=self.values,
                            state='readonly')
 
     # Dictionary that correlates the desired unit to the appropriate class
     unit_dict = {
         'none': NoUnitCombo,
```

### Comparing `compoundwidgets-0.4.1/compoundwidgets/CUSTOM_BUTTONS.py` & `compoundwidgets-0.4.2/compoundwidgets/CUSTOM_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/CUSTOM_FRAMES.py` & `compoundwidgets-0.4.2/compoundwidgets/CUSTOM_FRAMES.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,28 +187,34 @@
                 self.style = style
 
             self.label_style = self.label_style_dict.get(style)
 
         # Main container
         if True:
             self.container = ttk.Frame(parent)
-            self.container.rowconfigure(0, weight=0)
-            self.container.rowconfigure(1, weight=1)
-            self.container.columnconfigure(0, weight=0)
-            self.container.columnconfigure(1, weight=1)
+            self.container.rowconfigure(0, weight=0)  # Internal Title
+            self.container.rowconfigure(1, weight=1)  # Main content
+            self.container.columnconfigure(0, weight=0)  # Left Title
+            self.container.columnconfigure(1, weight=1)  # Main content
 
         # Expansion frame + label
         if True:
             self.title_frame = ttk.Frame(self.container, bootstyle=style)
             self.title_frame.grid(row=0, column=0, rowspan=2, sticky='nsew')
             self.title_frame.columnconfigure(0, weight=1)
             self.title_frame.rowconfigure(0, weight=0)
             self.title_frame.rowconfigure(1, weight=1)
             self.title_frame.bind('<ButtonRelease-1>', self.check_collapse)
 
+            broken_title = '\n'.join(title.upper())
+            style = f'{style}.Inverse.TLabel'
+            self.label = ttk.Label(self.title_frame, text=broken_title, anchor='n', justify='center', style=style)
+            self.label.grid(row=1, column=0, sticky='nsew')
+            self.label.bind('<ButtonRelease-1>', self.check_collapse)
+
             self.collapse_button = ttk.Label(self.title_frame, text='-', style='primary.TButton',
                                              font=title_font, width=3, padding=0, bootstyle=self.label_style,
                                              anchor='center', justify='center',)
             self.collapse_button.grid(row=0, column=0, sticky='nsew')
             self.collapse_button.bind('<ButtonRelease-1>', self.check_collapse)
 
             Tooltip(self.title_frame, text=title)
@@ -298,20 +304,21 @@
     def disable(self):
         self.collapse_frame()
         self.disabled = True
         local_style = 'secondary'
         local_label_style = self.label_style_dict.get(local_style)
         self.title_frame.configure(bootstyle=local_style)
         self.collapse_button.configure(bootstyle=local_label_style)
+        self.label.configure(style='secondary.Inverse.TLabel')
 
     def enable(self):
         self.disabled = False
         self.title_frame.configure(bootstyle=self.style)
         self.collapse_button.configure(bootstyle=self.label_style)
-
+        self.label.configure(style=f'{self.style}.Inverse.TLabel')
 
 class ScrollableFrame(ttk.Frame):
     """
     Creates a frame with a vertical and a horizontal scrollbar.
     Scrollbars will hide if the content fits the frame dimensions.
     Parameters:
         parent: container for the frame
```

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/add_new.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/add_new.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/add_to_form.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/add_to_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/back.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/back.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/calculate.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/calculate.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/clear.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/clear.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/edit_form.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/edit_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/help.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/help.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/no.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/no.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/quit.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/quit.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/remove_from_form.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/remove_from_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/save.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/save.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/trash_can.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/trash_can.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/IMAGES/yes.png` & `compoundwidgets-0.4.2/compoundwidgets/IMAGES/yes.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/LED_BUTTONS.py` & `compoundwidgets-0.4.2/compoundwidgets/LED_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/MESSAGE_BOX_WIDGETS.py` & `compoundwidgets-0.4.2/compoundwidgets/MESSAGE_BOX_WIDGETS.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,20 +235,22 @@
         self.style = widget.winfo_toplevel().style
         self.style.configure('custom.TLabel', background=bg, foreground=fg)
         self.widget = widget
         self.text = text
         self.wait_time = wait_time
         self.wrap_length = wrap_length
 
-        self.widget.bind("<Enter>", self._enter)
-        self.widget.bind("<Leave>", self._leave)
-        self.widget.bind("<Motion>", self._move_tip)
-        self.widget.bind("<ButtonPress>", self._leave)
-        self.id = None
-        self.top_level = None
+        if not self.text:
+            self.remove_message()
+        else:
+            self.widget.bind("<Enter>", self._enter)
+            self.widget.bind("<Leave>", self._leave)
+            self.widget.bind("<Motion>", self._move_tip)
+            self.id = None
+            self.top_level = None
 
     def _enter(self, event=None):
         self.schedule()
 
     def _leave(self, event=None):
         self.unschedule()
         self.hide()
@@ -290,15 +292,16 @@
             self.top_level.destroy()
         self.top_level = None
 
     def remove_message(self):
         self.widget.unbind("<Enter>")
         self.widget.unbind("<Leave>")
         self.widget.unbind("<Motion>")
-        self.widget.unbind("<ButtonPress>")
+        self.unschedule()
+        self.hide()
 
 
 class TimedBox(tk.Toplevel):
     """
     TopLevel widget for timed message boxes.
     Input:
         parent = widget over which the progress bar will be positioned
```

### Comparing `compoundwidgets-0.4.1/compoundwidgets/SCRIPTS.py` & `compoundwidgets-0.4.2/compoundwidgets/SCRIPTS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/compoundwidgets/__init__.py` & `compoundwidgets-0.4.2/compoundwidgets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.01"
+__version__ = "0.4.02"
 __author__ = 'Andre Mariano'
 __all__ = ['AUTOCOMPLETE_WIDGETS',
            'COMPOUND_WIDGETS',
            'CUSTOM_BUTTONS',
            'CUSTOM_FRAMES',
            'MESSAGE_BOX_WIDGETS',
            'IMAGES',
```

### Comparing `compoundwidgets-0.4.1/compoundwidgets.egg-info/PKG-INFO` & `compoundwidgets-0.4.2/compoundwidgets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compoundwidgets
-Version: 0.4.1
+Version: 0.4.2
 Summary: Compound TTK Widgets with ttkbootstrap
 Home-page: https://github.com/AndreMariano100/CompoundWidgets.git
 Author: Andre Mariano
 Author-email: andremariano100@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `compoundwidgets-0.4.1/setup.py` & `compoundwidgets-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='compoundwidgets',
-    version='0.4.01',
+    version='0.4.02',
     author='Andre Mariano',
     author_email='andremariano100@gmail.com',
     url='https://github.com/AndreMariano100/CompoundWidgets.git',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license="MIT",
     description='Compound TTK Widgets with ttkbootstrap',
```

### Comparing `compoundwidgets-0.4.1/test/autocomplete_entry_list_test.py` & `compoundwidgets-0.4.2/test/autocomplete_entry_list_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/autocomplete_labelcombo_test.py` & `compoundwidgets-0.4.2/test/autocomplete_labelcombo_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/compound_widgets_test_1_labelcombo.py` & `compoundwidgets-0.4.2/test/compound_widgets_test_1_labelcombo.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/compound_widgets_test_2_labelentry.py` & `compoundwidgets-0.4.2/test/compound_widgets_test_2_labelentry.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/compound_widgets_test_3_labelspinbox.py` & `compoundwidgets-0.4.2/test/compound_widgets_test_3_labelspinbox.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/compound_widgets_test_4_labeltext.py` & `compoundwidgets-0.4.2/test/compound_widgets_test_4_labeltext.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/compound_widgets_test_5_labelentryunit.py` & `compoundwidgets-0.4.2/test/compound_widgets_test_5_labelentryunit.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/compound_widgets_test_6_labelentrybutton.py` & `compoundwidgets-0.4.2/test/compound_widgets_test_6_labelentrybutton.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/compound_widgets_test_7_labelcombobutton.py` & `compoundwidgets-0.4.2/test/compound_widgets_test_7_labelcombobutton.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/custom_buttons_test.py` & `compoundwidgets-0.4.2/test/custom_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/frames_test_1_collapsable_frames.py` & `compoundwidgets-0.4.2/test/frames_test_1_collapsable_frames.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/frames_test_2_v_collapsable_frames.py` & `compoundwidgets-0.4.2/test/frames_test_2_v_collapsable_frames.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/frames_test_3_scrollable_frames.py` & `compoundwidgets-0.4.2/test/frames_test_3_scrollable_frames.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/frames_test_4_scrollable_with_collapsable.py` & `compoundwidgets-0.4.2/test/frames_test_4_scrollable_with_collapsable.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/frames_test_5_border_frames.py` & `compoundwidgets-0.4.2/test/frames_test_5_border_frames.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/led_buttons_test.py` & `compoundwidgets-0.4.2/test/led_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/message_box_test.py` & `compoundwidgets-0.4.2/test/message_box_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.4.1/test/test_variable_tracing.py` & `compoundwidgets-0.4.2/test/test_variable_tracing.py`

 * *Files identical despite different names*

