# Comparing `tmp/am2r_yams-2.0.0.tar.gz` & `tmp/am2r_yams-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "am2r_yams-2.0.0.tar", last modified: Tue Apr  9 18:54:00 2024, max compression
+gzip compressed data, was "am2r_yams-2.1.0.tar", last modified: Sun May 12 13:56:12 2024, max compression
```

## Comparing `am2r_yams-2.0.0.tar` & `am2r_yams-2.1.0.tar`

### file list

```diff
@@ -1,1097 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.391579 am2r_yams-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 18:54:00.391579 am2r_yams-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.203578 am2r_yams-2.0.0/am2r_yams/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.203578 am2r_yams-2.0.0/am2r_yams/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/__pyinstaller/hook-am2r_yams.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/
--rwxr--r--   0 runner    (1001) docker     (127)   204800 2021-09-19 09:20:24.000000 am2r_yams-2.0.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
--rwxr--r--   0 runner    (1001) docker     (127)    42496 2022-06-15 03:36:02.000000 am2r_yams-2.0.0/am2r_yams/yams/Macross.Json.Extensions.dll
--rwxr--r--   0 runner    (1001) docker     (127)    27528 2020-10-19 18:40:26.000000 am2r_yams-2.0.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (127)     6656 2023-12-07 09:32:36.000000 am2r_yams-2.0.0/am2r_yams/yams/NaturalSort.Extension.dll
--rwxr--r--   0 runner    (1001) docker     (127)     6656 2021-03-13 10:51:42.000000 am2r_yams-2.0.0/am2r_yams/yams/PropertyChanged.dll
--rwxr--r--   0 runner    (1001) docker     (127)  2088448 2024-03-05 05:20:28.000000 am2r_yams-2.0.0/am2r_yams/yams/SixLabors.ImageSharp.dll
--rwxr--r--   0 runner    (1001) docker     (127)   173432 2021-10-22 20:57:42.000000 am2r_yams-2.0.0/am2r_yams/yams/System.Drawing.Common.dll
--rw-r--r--   0 runner    (1001) docker     (127)   947200 2024-04-09 18:53:54.000000 am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.dll
--rw-r--r--   0 runner    (1001) docker     (127)   330863 2024-04-09 18:53:53.000000 am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-09 18:53:57.000000 am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.deps.json
--rw-r--r--   0 runner    (1001) docker     (127)   278016 2024-04-09 18:53:57.000000 am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.dll
--rw-r--r--   0 runner    (1001) docker     (127)    28044 2024-04-09 18:53:57.000000 am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.pdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (127)   419720 2021-10-22 20:57:34.000000 am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.187578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
--rwxr--r--   0 runner    (1001) docker     (127)    52104 2020-10-19 18:52:12.000000 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
--rwxr--r--   0 runner    (1001) docker     (127)   436600 2021-10-22 20:58:02.000000 am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.215578 am2r_yams-2.0.0/am2r_yams/yams/sprites/
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/Attribution.md
--rw-r--r--   0 runner    (1001) docker     (127)    20146 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/LICENSE-GRAPHICS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.223578 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearBulletHell.png
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearPipeHub.png
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearSave.png
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPNearTotem.png
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPRightExterior.png
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorA5EMPRobotHome.png
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_4.png
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorAnim_9.png
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorArachnus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorBlue.png
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorBomb.png
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorChargeBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPA3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorEMPActivated.png
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorGenesis.png
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorGuardian.png
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorIceBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorLocked.png
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorMissile.png
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorPBomb.png
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorPlasmaBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorQueen.png
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorScrew.png
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSerris.png
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSpazerBeam.png
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSpider.png
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorSuper.png
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTempLocked.png
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTester.png
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTorizo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorTowerEnabled.png
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/doors/sDoorWaveBeam.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.191578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.227578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/bigHealthDrop/sItemBigHealthDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.227578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/blindfold/sItemBlindfold_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.227578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/dna/sItemDNA_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.231578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/flashlight/sItemFlashlight_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.231578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileDrop/sItemMissileDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.231578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/missileLauncher/sItemMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.235578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/morph/sItemMorphBall_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.235578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/nothing/sItemNothing_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.235578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbDrop/sItemPBombDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.239578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/pbLauncher/sItemPBombLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.239578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/powerGrip/sItemPowergrip_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.239578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveJump/sItemProgressiveJump_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.243578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/progressiveSuit/sItemProgressiveSuit_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.243578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/screwAttackShiny/sItemScrewAttacker_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyHijump/sItemShinyHijump_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyIcebeam/sItemShinyIceBeam_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyMissile/sItemShinyMissile_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/shinyNothing/sItemShinyNothing_8.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.247578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/smallHealthDrop/sItemSmallHealthDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.251578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/speedboosterUpgrade/sItemSpeedBoosterUpgrade_8.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.251578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileDrop/sItemSMissileDrop_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.255578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/superMissileLauncher/sItemSMissileLauncher_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.255578 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/items/unknown/sItemUnknown_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.255578 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/bgGUIMetCountBG2ELM.png
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/bg_MapBottom2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.259579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA.png
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA0.png
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA2.png
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA3.png
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA4.png
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA5.png
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogDNA6.png
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hintsBGs/bgLogIce.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.259579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIMissileNormal.png
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIMissileNormalGreen.png
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIMissileSelected.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIPBombNormal.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIPBombNormalGreen.png
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUIPBombSelected.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUISMissileNormal.png
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUISMissileNormalGreen.png
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/hud/sGUISMissileSelected.png
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newA4Doors.png
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newA4Doors2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapBlockUnexplored.png
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/newMapTiles/sMapCornerUnexplored_9.png
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/sDisconnected.png
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/sMapHint.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadP.png
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadPClaw.png
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/skippy_bot/sAutoadPFang.png
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpDepthsEntrance.png
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpDepthsExit.png
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpHideout.png
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/tlWarpWaterfall.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/misc/wisdomSeptoggs/sWisdomSeptogg_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.195578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.191578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/caveStory/generic/sItemGenericCS_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.263579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/default/sItemRDV_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.195578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/crossBombs/sItemCrossBombsDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/diffusionBeam/sItemDiffusionBeamDread_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyPart/sItemEPartDread_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.267579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/energyTank/sItemETankDread_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.271579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/flashShift/sItemFlashShiftDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.271579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/grappleBeam/sItemGrappleBeamDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.275579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/iceMissiles/sItemIceMissilesDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.275579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTank/sItemMissileTankDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.279579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/missileTankPlus/sItemMissileTankPlusDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.283579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/morphBall/sItemMorphBallDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.283579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbLauncher/sItemPowerBombLauncherDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.287579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pbTank/sItemPowerBombTankDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.287579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/phantomCloak/sItemPhantomCloakDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.287579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/pulseRadar/sItemPulseRadarDread_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.291579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spaceJump/sItemSpaceJumpDread_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.295579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/speedBooster/sItemSpeedBoosterDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.299579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_20.png
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spiderMagnet/sItemSpiderMagnetDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.299579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_20.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/spinBoost/sItemSpinBoostDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.303579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/stormMissiles/sItemStormMissilesDread_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.303579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/varia/sItemVariaSuitDread_8.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/dread/wideBeam/sItemWideBeamDread_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.199578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.199578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/amber/sItemAmberEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/annihilator/sItemAnnihilatorEchoes_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.307579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/beamAmmo/sItemBeamAmmoEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.311579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cannonBall/sItemCannonBallEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.311579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/cobalt/sItemCobaltEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.315579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAgon/sItemDarkAgonKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.315579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkAmmo/sItemDarkAmmoEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.315579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBeam/sItemDarkBeamEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.319579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_20.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_21.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_22.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_23.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkBurst/sItemDarkburstEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.323579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkSuit/sItemDarkSuitEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.323579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkTorvus/sItemDarkTorvusKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.327579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/darkVisor/sItemDarkVisorEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.327579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/echoVisor/sItemEchoVisorEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.327579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/emerald/sItemEmeraldEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.331579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/ingHive/sItemIngHiveKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.331579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightAmmo/sItemLightAmmoEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.331579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightBeam/sItemLightBeamEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.335579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/lightSuit/sItemLightSuitEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.335579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/powerBombLauncher/sItemPowerBombLauncherEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.339579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/progressiveSuit/sItemProgressiveSuitEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.339579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/screwAttack/sItemScrewAttackEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.339579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/seekers/sItemSeekerMissileEchoes_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.343579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/skyTempleKey/sItemSkyTempleKeyEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/sonicBoom/sItemSonicBoomEchoes_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/superMissile/sItemSuperMissileEchoes_3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/echoes/violet/sItemVioletEchoes_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.203578 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.347579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/arrtifactElder/sItemArtifactElderPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifact/sItemArtifactPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactChozo/sItemArtifactChozoPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactLifegiver/sItemArtifactLifegiverPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNature/sItemArtifactNaturePrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.351579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactNewborn/sItemArtifactNewbornPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSpirit/sItemArtifactSpiritPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactStrength/sItemArtifactStrengthPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactSun/sItemArtifactSunPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.355579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactTruth/sItemArtifactTruthPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWarrior/sItemArtifactWarriorPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWild/sItemArtifactWildPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_0.png
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/artifactWorld/sItemArtifactWorldPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.359579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/bombs/sItemBombsPrime_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.363579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_17.png
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_18.png
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_19.png
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_20.png
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_21.png
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_22.png
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_23.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/boostBall/sItemBoostBallPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.367579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/combatVisor/sItemCombatVisorPrime_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.367579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/flamethrower/sItemFlamethrowerPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.367579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/grapple/sItemGrappleBeamPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.371579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/gravity/sItemGravitySuitPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.371579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceBeam/sItemIceBeamPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.371579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/iceSpreader/sItemIceSpreaderPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.375579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/morphBall/sItemMorphBallPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/phazonSuit/sItemPhazonSuitPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/plasmaBeam/sItemPlasmaBeamPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBeam/sItemPowerBeamPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.379579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/powerBombLauncher/sItemPowerBombLauncherPrime_7.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.383579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/scanVisor/sItemScanVisorPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.383579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/superMissile/sItemSuperMissilePrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.383579 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__1.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__2.png
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__3.png
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__4.png
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__5.png
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/thermalVisor/sItemThermalVisorPrime__6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_10.png
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_11.png
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_12.png
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_13.png
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_14.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_15.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_6.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_7.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_8.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/varia/sItemVariaSuitPrime_9.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBeam/sItemWaveBeamPrime_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/waveBuster/sItemWaveBusterPrime_4.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_2.png
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_3.png
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_4.png
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_5.png
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams/yams/sprites/offworld items/primes/prime1/xrayVisor/sItemXrayVisorPrime_6.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    76644 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:53:59.000000 am2r_yams-2.0.0/am2r_yams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 18:54:00.000000 am2r_yams-2.0.0/am2r_yams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:54:00.387580 am2r_yams-2.0.0/am2r_yams_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/am2r_yams_tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 18:53:24.000000 am2r_yams-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 18:54:00.391579 am2r_yams-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.072919 am2r_yams-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-12 13:55:49.000000 am2r_yams-2.1.0/LICENSE-CODE
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-12 13:56:12.072919 am2r_yams-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-12 13:55:49.000000 am2r_yams-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.060919 am2r_yams-2.1.0/am2r_yams/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-12 13:55:49.000000 am2r_yams-2.1.0/am2r_yams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-12 13:55:49.000000 am2r_yams-2.1.0/am2r_yams/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.068919 am2r_yams-2.1.0/am2r_yams/yams/
+-rwxr--r--   0 runner    (1001) docker     (127)   204800 2021-09-19 09:20:24.000000 am2r_yams-2.1.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    42496 2022-06-15 03:36:02.000000 am2r_yams-2.1.0/am2r_yams/yams/Macross.Json.Extensions.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    27528 2020-10-19 18:40:26.000000 am2r_yams-2.1.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (127)    14336 2024-04-14 16:50:48.000000 am2r_yams-2.1.0/am2r_yams/yams/NaturalSort.Extension.dll
+-rwxr--r--   0 runner    (1001) docker     (127)     6656 2021-03-13 10:51:42.000000 am2r_yams-2.1.0/am2r_yams/yams/PropertyChanged.dll
+-rwxr--r--   0 runner    (1001) docker     (127)  2091520 2024-04-11 06:51:00.000000 am2r_yams-2.1.0/am2r_yams/yams/SixLabors.ImageSharp.dll
+-rwxr--r--   0 runner    (1001) docker     (127)   173432 2021-10-22 20:57:42.000000 am2r_yams-2.1.0/am2r_yams/yams/System.Drawing.Common.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   947200 2024-05-12 13:56:07.000000 am2r_yams-2.1.0/am2r_yams/yams/UndertaleModLib.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   330863 2024-05-12 13:56:06.000000 am2r_yams-2.1.0/am2r_yams/yams/UndertaleModLib.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-12 13:56:09.000000 am2r_yams-2.1.0/am2r_yams/yams/YAMS-LIB.deps.json
+-rw-r--r--   0 runner    (1001) docker     (127)   283136 2024-05-12 13:56:09.000000 am2r_yams-2.1.0/am2r_yams/yams/YAMS-LIB.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    28592 2024-05-12 13:56:09.000000 am2r_yams-2.1.0/am2r_yams/yams/YAMS-LIB.pdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.060919 am2r_yams-2.1.0/am2r_yams/yams/runtimes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.060919 am2r_yams-2.1.0/am2r_yams/yams/runtimes/unix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.060919 am2r_yams-2.1.0/am2r_yams/yams/runtimes/unix/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.068919 am2r_yams-2.1.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (127)   419720 2021-10-22 20:57:34.000000 am2r_yams-2.1.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.060919 am2r_yams-2.1.0/am2r_yams/yams/runtimes/win/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.060919 am2r_yams-2.1.0/am2r_yams/yams/runtimes/win/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.068919 am2r_yams-2.1.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/
+-rwxr--r--   0 runner    (1001) docker     (127)    52104 2020-10-19 18:52:12.000000 am2r_yams-2.1.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll
+-rwxr--r--   0 runner    (1001) docker     (127)   436600 2021-10-22 20:58:02.000000 am2r_yams-2.1.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.072919 am2r_yams-2.1.0/am2r_yams/yams/sprites/
+-rw-r--r--   0 runner    (1001) docker     (127)   284547 2024-05-12 13:56:00.000000 am2r_yams-2.1.0/am2r_yams/yams/sprites/texturepage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74598 2024-05-12 13:56:00.000000 am2r_yams-2.1.0/am2r_yams/yams/sprites/texturepageiteminfo.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:56:12.072919 am2r_yams-2.1.0/am2r_yams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-12 13:56:12.000000 am2r_yams-2.1.0/am2r_yams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-12 13:56:12.000000 am2r_yams-2.1.0/am2r_yams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:56:12.000000 am2r_yams-2.1.0/am2r_yams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-12 13:56:12.000000 am2r_yams-2.1.0/am2r_yams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-12 13:56:12.000000 am2r_yams-2.1.0/am2r_yams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 13:56:12.000000 am2r_yams-2.1.0/am2r_yams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-12 13:55:49.000000 am2r_yams-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 13:56:12.072919 am2r_yams-2.1.0/setup.cfg
```

### Comparing `am2r_yams-2.0.0/PKG-INFO` & `am2r_yams-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 2.0.0
+Version: 2.1.0
 Summary: An open source randomizer patcher for AM2R.
-Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
+Project-URL: Repository, https://github.com/randovania/YAMS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE-CODE
 Requires-Dist: pythonnet
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 
 # Yet Another Metroid2 Shuffler (YAMS)
```

### Comparing `am2r_yams-2.0.0/README.md` & `am2r_yams-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/wrapper.py` & `am2r_yams-2.1.0/am2r_yams/wrapper.py`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll` & `am2r_yams-2.1.0/am2r_yams/yams/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/Macross.Json.Extensions.dll` & `am2r_yams-2.1.0/am2r_yams/yams/Macross.Json.Extensions.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-2.1.0/am2r_yams/yams/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/PropertyChanged.dll` & `am2r_yams-2.1.0/am2r_yams/yams/PropertyChanged.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/SixLabors.ImageSharp.dll` & `am2r_yams-2.1.0/am2r_yams/yams/SixLabors.ImageSharp.dll`

 * *Files 13% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xf9e6da3b
+	             Time stamp: 0x9fc4782e
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x001fd400
+	              Code Size: 0x001fe000
 	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x001f79d2
+	        Entry Point RVA: 0x001f867a
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00200000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -29,94 +29,94 @@
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x00204000
 	 	     Header Size: 0x00000200
-	            Checksum (0): 0x0020bfa2
+	            Checksum (0): 0x0020433e
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x001f797f [0x0000004f]
+	     Import Table: 0x001f8627 [0x0000004f]
 	   Resource Table: 0x00200000 [0x000004b8]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x00202000 [0x0000000c]
-	            Debug: 0x001f78a4 [0x00000054]
+	            Debug: 0x001f854c [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x001fd308
+	   Virtual Size: 0x001fdfb0
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x001fd400
+	  Raw Data Size: 0x001fe000
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x000004b8
 	Virtual Address: 0x00200000
 	  Raw Data Size: 0x00000600
-	   Raw Data Ptr: 0x001fd600
+	   Raw Data Ptr: 0x001fe200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x00202000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x001fdc00
+	   Raw Data Ptr: 0x001fe800
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x000d5840 [0x00121fe4]
+	         Metadata: 0x000d5d6c [0x00122760]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
-	   Strong Name at: 0x001f7824 [0x00000080]
+	   Strong Name at: 0x001f84cc [0x00000080]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name:
-	 E9 2D D9 38 5C 7F 4F AA 4C 8F 45 5B E7 4A 38 3F
-	 7E 47 C5 E2 1D BB 99 89 30 1E BD 10 6C FD 5F F3
-	 DD C8 BD 14 CC E9 57 DD F0 40 3B 24 CE ED 0F 42
-	 F2 92 65 0A 89 46 28 53 9B 0D BE E6 07 63 2E 93
-	 7C B4 E1 D3 40 43 90 87 46 71 3C 4B AC A5 B5 46
-	 9B 07 E6 D3 AC AE 93 03 EE 09 14 4F 84 55 FB 96
-	 14 68 47 5D 7E BF FA EB FF D9 58 F0 E2 0E EF EA
-	 73 CD B1 5E 66 2D 14 F7 F3 CE DF 35 12 1F 73 82
+	 48 A7 DE 10 64 A1 B9 4F 47 96 97 56 E8 28 51 49
+	 AA E1 0D DE D1 FF 16 3F DD 9F 0D 39 7D 1E CD F9
+	 71 25 65 0F 65 B2 D0 85 03 1F FE 54 4E A4 F3 D8
+	 52 7D 0D 41 AF 8A D2 E8 EC 2B C6 7D 08 32 C4 FD
+	 EA 51 26 66 F6 CC C8 CD AB FC D7 16 DE D7 41 85
+	 3D B5 32 D9 7A 80 95 D4 1A 25 DD 39 1D FC EE 52
+	 23 E3 69 67 25 85 44 DC 07 F5 45 EA 1C E0 1F ED
+	 B1 77 81 ED A6 1F 50 04 C4 AE 43 02 74 DF 8E 1C
 
 Public key:
 	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
 	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
 	 01 47 E6 FE 67 66 71 5E EC 6C FE D6 1F 1E 7D CD
 	 BF 69 74 8A 3E 35 5C 67 E9 D8 DF D9 53 AC AB 1D
 	 5E 01 2B A3 4B 23 30 81 66 FD C6 1E E1 D0 39 0D
@@ -127,41 +127,41 @@
 	 4B 0E 9A 51 71 E6 BB 13 84 B6 D2 F7 D5 4D FA 97
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x000be420 [779188 == 0x000be3b4]
-	    Strings: 0x000be420 - 0x000f0594 [205172 == 0x00032174]
-	       Blob: 0x000fba94 - 0x00121fe4 [157008 == 0x00026550]
-	User string: 0x000f0594 - 0x000fba84 [46320 == 0x0000b4f0]
-	       GUID: 0x000fba84 - 0x000fba94 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x000be814 [780200 == 0x000be7a8]
+	    Strings: 0x000be814 - 0x000f0be4 [205776 == 0x000323d0]
+	       Blob: 0x000fc170 - 0x00122760 [157168 == 0x000265f0]
+	User string: 0x000f0be4 - 0x000fc160 [46460 == 0x0000b57c]
+	       GUID: 0x000fc160 - 0x000fc170 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at d3b34)
-Table TypeRef: 256 records (10 bytes, at d3b40)
-Table TypeDef: 1591 records (18 bytes, at d4540)
-Table Field: 6613 records (10 bytes, at db51e)
-Table Method: 12252 records (18 bytes, at eb770)
-Table Param: 17805 records (8 bytes, at 1214e8)
-Table InterfaceImpl: 611 records (4 bytes, at 144150)
-Table MemberRef: 4304 records (12 bytes, at 144adc)
-Table Constant: 2187 records (10 bytes, at 15149c)
-Table CustomAttribute: 12268 records (12 bytes, at 156a0a)
-Table DeclSecurity: 1 records (8 bytes, at 17a91a)
-Table ClassLayout: 80 records (8 bytes, at 17a922)
-Table FieldLayoutt: 49 records (6 bytes, at 17aba2)
-Table StandaloneSig: 2102 records (4 bytes, at 17acc8)
-Table EventMap: 1 records (4 bytes, at 17cda0)
-Table Event: 3 records (8 bytes, at 17cda4)
-Table PropertyMap: 702 records (4 bytes, at 17cdbc)
-Table Property: 2359 records (10 bytes, at 17d8b4)
-Table MethodSemantics: 3025 records (6 bytes, at 1834da)
-Table MethodImpl: 102 records (6 bytes, at 187bc0)
-Table TypeSpec: 1297 records (4 bytes, at 187e24)
-Table FieldRVA: 348 records (6 bytes, at 189268)
-Table Assembly: 1 records (28 bytes, at 189a90)
-Table AssemblyRef: 16 records (28 bytes, at 189aac)
-Table NestedClass: 465 records (4 bytes, at 189c6c)
-Table GenericParam: 1102 records (10 bytes, at 18a3b0)
-Table MethodSpec: 2076 records (6 bytes, at 18cebc)
-Table GenericParamConstraint: 1982 records (4 bytes, at 18ff64)
+Table Module: 1 records (12 bytes, at d4060)
+Table TypeRef: 256 records (10 bytes, at d406c)
+Table TypeDef: 1591 records (18 bytes, at d4a6c)
+Table Field: 6619 records (10 bytes, at dba4a)
+Table Method: 12270 records (18 bytes, at ebcd8)
+Table Param: 17837 records (8 bytes, at 121b94)
+Table InterfaceImpl: 612 records (4 bytes, at 1448fc)
+Table MemberRef: 4304 records (12 bytes, at 14528c)
+Table Constant: 2188 records (10 bytes, at 151c4c)
+Table CustomAttribute: 12287 records (12 bytes, at 1571c4)
+Table DeclSecurity: 1 records (8 bytes, at 17b1b8)
+Table ClassLayout: 80 records (8 bytes, at 17b1c0)
+Table FieldLayoutt: 49 records (6 bytes, at 17b440)
+Table StandaloneSig: 2104 records (4 bytes, at 17b566)
+Table EventMap: 1 records (4 bytes, at 17d646)
+Table Event: 3 records (8 bytes, at 17d64a)
+Table PropertyMap: 702 records (4 bytes, at 17d662)
+Table Property: 2363 records (10 bytes, at 17e15a)
+Table MethodSemantics: 3033 records (6 bytes, at 183da8)
+Table MethodImpl: 102 records (6 bytes, at 1884be)
+Table TypeSpec: 1298 records (4 bytes, at 188722)
+Table FieldRVA: 348 records (6 bytes, at 189b6a)
+Table Assembly: 1 records (28 bytes, at 18a392)
+Table AssemblyRef: 16 records (28 bytes, at 18a3ae)
+Table NestedClass: 465 records (4 bytes, at 18a56e)
+Table GenericParam: 1103 records (10 bytes, at 18acb2)
+Table MethodSpec: 2079 records (6 bytes, at 18d7c8)
+Table GenericParamConstraint: 1983 records (4 bytes, at 190882)
```

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/System.Drawing.Common.dll` & `am2r_yams-2.1.0/am2r_yams/yams/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.dll` & `am2r_yams-2.1.0/am2r_yams/yams/UndertaleModLib.dll`

 * *Files 1% similar despite different names*

#### pedump {}

```diff
@@ -1,12 +1,12 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xd06ab7c2
+	             Time stamp: 0xefaecfdf
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2102
 
 PE Header:
 	         Magic (0x010b): 0x010b
```

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/UndertaleModLib.xml` & `am2r_yams-2.1.0/am2r_yams/yams/UndertaleModLib.xml`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.deps.json` & `am2r_yams-2.1.0/am2r_yams/yams/YAMS-LIB.deps.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9196428571428571%*

 * *Differences: {"'libraries'": "{'YAMS-LIB/2.1.0': OrderedDict([('type', 'project'), ('serviceable', False), "*

 * *                "('sha512', '')]), 'NaturalSort.Extension/4.3.0': OrderedDict([('type', "*

 * *                "'package'), ('serviceable', True), ('sha512', "*

 * *                "'sha512-NGr3z/Izk16yxEcXKsopZvfYH8hh3iY7mmLJlT8iWVWBlidqGHeq2ykoy2JposrdM6aGvqjMfso9l0N8FzxAUw=='), "*

 * *                "('path', 'naturalsort.extension/4.3.0'), ('hashPath', "*

 * *                "'naturalsort.extension.4.3.0.nupkg.sha512')]), 'SixL […]*

```diff
@@ -25,19 +25,19 @@
         "Microsoft.Win32.SystemEvents/5.0.0": {
             "hashPath": "microsoft.win32.systemevents.5.0.0.nupkg.sha512",
             "path": "microsoft.win32.systemevents/5.0.0",
             "serviceable": true,
             "sha512": "sha512-Bh6blKG8VAKvXiLe2L+sEsn62nc1Ij34MrNxepD2OCrS5cpCwQa9MeLyhVQPQ/R4Wlzwuy6wMK8hLb11QPDRsQ==",
             "type": "package"
         },
-        "NaturalSort.Extension/4.2.0": {
-            "hashPath": "naturalsort.extension.4.2.0.nupkg.sha512",
-            "path": "naturalsort.extension/4.2.0",
+        "NaturalSort.Extension/4.3.0": {
+            "hashPath": "naturalsort.extension.4.3.0.nupkg.sha512",
+            "path": "naturalsort.extension/4.3.0",
             "serviceable": true,
-            "sha512": "sha512-6aGueMxAOjclKlJ7NsuewASgPOc1Pl7Wtaz83BMUIWf8MgKWkTfcsHSnyy4xTZxzLWyfr8f6SngJdp9rmw50Jw==",
+            "sha512": "sha512-NGr3z/Izk16yxEcXKsopZvfYH8hh3iY7mmLJlT8iWVWBlidqGHeq2ykoy2JposrdM6aGvqjMfso9l0N8FzxAUw==",
             "type": "package"
         },
         "PropertyChanged.Fody/3.3.3": {
             "hashPath": "propertychanged.fody.3.3.3.nupkg.sha512",
             "path": "propertychanged.fody/3.3.3",
             "serviceable": true,
             "sha512": "sha512-2dHoq3+Y37J2g06RRyV57zMY9uVOq9JanPienXxineL1pIACCgxn8dL/f6C9I0L1hPvhoipxtP2u9jcSlVsn6Q==",
@@ -46,34 +46,34 @@
         "SharpZipLib/1.3.3": {
             "hashPath": "sharpziplib.1.3.3.nupkg.sha512",
             "path": "sharpziplib/1.3.3",
             "serviceable": true,
             "sha512": "sha512-N8+hwhsKZm25tDJfWpBSW7EGhH/R7EMuiX+KJ4C4u+fCWVc1lJ5zg1u3S1RPPVYgTqhx/C3hxrqUpi6RwK5+Tg==",
             "type": "package"
         },
-        "SixLabors.ImageSharp/3.1.3": {
-            "hashPath": "sixlabors.imagesharp.3.1.3.nupkg.sha512",
-            "path": "sixlabors.imagesharp/3.1.3",
+        "SixLabors.ImageSharp/3.1.4": {
+            "hashPath": "sixlabors.imagesharp.3.1.4.nupkg.sha512",
+            "path": "sixlabors.imagesharp/3.1.4",
             "serviceable": true,
-            "sha512": "sha512-wybtaqZQ1ZRZ4ZeU+9h+PaSeV14nyiGKIy7qRbDfSHzHq4ybqyOcjoifeaYbiKLO1u+PVxLBuy7MF/DMmwwbfg==",
+            "sha512": "sha512-lFIdxgGDA5iYkUMRFOze7BGLcdpoLFbR+a20kc1W7NepvzU7ejtxtWOg9RvgG7kb9tBoJ3ONYOK6kLil/dgF1w==",
             "type": "package"
         },
         "System.Drawing.Common/5.0.3": {
             "hashPath": "system.drawing.common.5.0.3.nupkg.sha512",
             "path": "system.drawing.common/5.0.3",
             "serviceable": true,
             "sha512": "sha512-rEQZuslijqdsO0pkJn7LtGBaMc//YVA8de0meGihkg9oLPaN+w+/Pb5d71lgp0YjPoKgBKNMvdq0IPnoW4PEng==",
             "type": "package"
         },
         "UndertaleModLib/1.0.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
-        "YAMS-LIB/2.0.0": {
+        "YAMS-LIB/2.1.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         }
     },
     "runtimeTarget": {
         "name": ".NETCoreApp,Version=v6.0",
@@ -106,19 +106,19 @@
                         "assemblyVersion": "5.0.0.0",
                         "assetType": "runtime",
                         "fileVersion": "5.0.20.51904",
                         "rid": "win"
                     }
                 }
             },
-            "NaturalSort.Extension/4.2.0": {
+            "NaturalSort.Extension/4.3.0": {
                 "runtime": {
                     "lib/net6.0/NaturalSort.Extension.dll": {
                         "assemblyVersion": "4.0.0.0",
-                        "fileVersion": "4.2.0.0"
+                        "fileVersion": "4.3.0.0"
                     }
                 }
             },
             "PropertyChanged.Fody/3.3.3": {
                 "runtime": {
                     "lib/netstandard2.1/PropertyChanged.dll": {
                         "assemblyVersion": "3.3.3.0",
@@ -130,19 +130,19 @@
                 "runtime": {
                     "lib/netstandard2.1/ICSharpCode.SharpZipLib.dll": {
                         "assemblyVersion": "1.3.3.11",
                         "fileVersion": "1.3.3.11"
                     }
                 }
             },
-            "SixLabors.ImageSharp/3.1.3": {
+            "SixLabors.ImageSharp/3.1.4": {
                 "runtime": {
                     "lib/net6.0/SixLabors.ImageSharp.dll": {
                         "assemblyVersion": "3.0.0.0",
-                        "fileVersion": "3.1.3.0"
+                        "fileVersion": "3.1.4.0"
                     }
                 }
             },
             "System.Drawing.Common/5.0.3": {
                 "dependencies": {
                     "Microsoft.Win32.SystemEvents": "5.0.0"
                 },
@@ -174,19 +174,19 @@
                     "SharpZipLib": "1.3.3",
                     "System.Drawing.Common": "5.0.3"
                 },
                 "runtime": {
                     "UndertaleModLib.dll": {}
                 }
             },
-            "YAMS-LIB/2.0.0": {
+            "YAMS-LIB/2.1.0": {
                 "dependencies": {
                     "Macross.Json.Extensions": "3.0.0",
-                    "NaturalSort.Extension": "4.2.0",
-                    "SixLabors.ImageSharp": "3.1.3",
+                    "NaturalSort.Extension": "4.3.0",
+                    "SixLabors.ImageSharp": "3.1.4",
                     "UndertaleModLib": "1.0.0"
                 },
                 "runtime": {
                     "YAMS-LIB.dll": {}
                 }
             }
         }
```

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/YAMS-LIB.dll` & `am2r_yams-2.1.0/am2r_yams/yams/YAMS-LIB.dll`

 * *Files 6% similar despite different names*

#### pedump {}

```diff
@@ -1,106 +1,106 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xc5330f13
+	             Time stamp: 0x9e2642aa
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x00043600
+	              Code Size: 0x00044a00
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0004556a
+	        Entry Point RVA: 0x000468fe
 	 	  Code Base RVA: 0x00002000
-		  Data Base RVA: 0x00046000
+		  Data Base RVA: 0x00048000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
 	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
-	 	      Image Size: 0x0004a000
+	 	      Image Size: 0x0004c000
 	 	     Header Size: 0x00000200
 	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x00045518 [0x0000004f]
-	   Resource Table: 0x00046000 [0x00000370]
+	     Import Table: 0x000468ac [0x0000004f]
+	   Resource Table: 0x00048000 [0x00000370]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
-	      Reloc Table: 0x00048000 [0x0000000c]
-	            Debug: 0x00045440 [0x00000054]
+	      Reloc Table: 0x0004a000 [0x0000000c]
+	            Debug: 0x000467d4 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00043598
+	   Virtual Size: 0x00044930
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x00043600
+	  Raw Data Size: 0x00044a00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x00000370
-	Virtual Address: 0x00046000
+	Virtual Address: 0x00048000
 	  Raw Data Size: 0x00000400
-	   Raw Data Ptr: 0x00043800
+	   Raw Data Ptr: 0x00044c00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
-	Virtual Address: 0x00048000
+	Virtual Address: 0x0004a000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x00043c00
+	   Raw Data Ptr: 0x00045000
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0000ec0c [0x00036834]
+	         Metadata: 0x0000f0d0 [0x00037704]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
@@ -109,32 +109,32 @@
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x00002b58 [10988 == 0x00002aec]
-	    Strings: 0x00002b58 - 0x00004d98 [8768 == 0x00002240]
-	       Blob: 0x000344ac - 0x00036834 [9096 == 0x00002388]
-	User string: 0x00004d98 - 0x0003449c [194308 == 0x0002f704]
-	       GUID: 0x0003449c - 0x000344ac [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x00002ba4 [11064 == 0x00002b38]
+	    Strings: 0x00002ba4 - 0x00004d74 [8656 == 0x000021d0]
+	       Blob: 0x0003530c - 0x00037704 [9208 == 0x000023f8]
+	User string: 0x00004d74 - 0x000352fc [198024 == 0x00030588]
+	       GUID: 0x000352fc - 0x0003530c [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at cedc)
-Table TypeRef: 130 records (6 bytes, at cee6)
-Table TypeDef: 42 records (14 bytes, at d1f2)
-Table Field: 262 records (6 bytes, at d43e)
-Table Method: 94 records (14 bytes, at da62)
-Table Param: 100 records (6 bytes, at df86)
-Table MemberRef: 350 records (6 bytes, at e1de)
-Table Constant: 143 records (6 bytes, at ea12)
-Table CustomAttribute: 412 records (6 bytes, at ed6c)
-Table ClassLayout: 1 records (8 bytes, at f714)
-Table StandaloneSig: 18 records (2 bytes, at f71c)
-Table TypeSpec: 66 records (2 bytes, at f740)
-Table FieldRVA: 1 records (6 bytes, at f7c4)
-Table Assembly: 1 records (22 bytes, at f7ca)
-Table AssemblyRef: 11 records (20 bytes, at f7e0)
-Table NestedClass: 9 records (4 bytes, at f8bc)
-Table GenericParam: 2 records (8 bytes, at f8e0)
-Table MethodSpec: 26 records (4 bytes, at f8f0)
-Table GenericParamConstraint: 2 records (4 bytes, at f958)
+Table Module: 1 records (10 bytes, at d3a0)
+Table TypeRef: 128 records (6 bytes, at d3aa)
+Table TypeDef: 43 records (14 bytes, at d6aa)
+Table Field: 265 records (6 bytes, at d904)
+Table Method: 95 records (14 bytes, at df3a)
+Table Param: 100 records (6 bytes, at e46c)
+Table MemberRef: 348 records (6 bytes, at e6c4)
+Table Constant: 145 records (6 bytes, at eeec)
+Table CustomAttribute: 419 records (6 bytes, at f252)
+Table ClassLayout: 1 records (8 bytes, at fc24)
+Table StandaloneSig: 18 records (2 bytes, at fc2c)
+Table TypeSpec: 67 records (2 bytes, at fc50)
+Table FieldRVA: 1 records (6 bytes, at fcd6)
+Table Assembly: 1 records (22 bytes, at fcdc)
+Table AssemblyRef: 11 records (20 bytes, at fcf2)
+Table NestedClass: 9 records (4 bytes, at fdce)
+Table GenericParam: 2 records (8 bytes, at fdf2)
+Table MethodSpec: 26 records (4 bytes, at fe02)
+Table GenericParamConstraint: 2 records (4 bytes, at fe6a)
```

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-2.1.0/am2r_yams/yams/runtimes/unix/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll` & `am2r_yams-2.1.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll` & `am2r_yams-2.1.0/am2r_yams/yams/runtimes/win/lib/netcoreapp3.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `am2r_yams-2.0.0/am2r_yams.egg-info/PKG-INFO` & `am2r_yams-2.1.0/am2r_yams.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: am2r_yams
-Version: 2.0.0
+Version: 2.1.0
 Summary: An open source randomizer patcher for AM2R.
-Home-page: https://github.com/Miepee/YAMS
 Author: Miepee
+Project-URL: Repository, https://github.com/randovania/YAMS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE-CODE
 Requires-Dist: pythonnet
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 
 # Yet Another Metroid2 Shuffler (YAMS)
```

