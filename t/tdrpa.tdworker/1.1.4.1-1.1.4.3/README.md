# Comparing `tmp/tdrpa.tdworker-1.1.4.1-py3-none-any.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 418482 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1170944 b- defN 24-May-12 18:32 tdrpa/tdworker.cp38-win_amd64.pyd
+Zip file size: 419608 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1172992 b- defN 24-May-12 18:59 tdrpa/tdworker.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    15621 b- defN 24-May-06 14:11 tdrpa/tdworker/WinElement.pyi
 -rw-rw-rw-  2.0 fat     4815 b- defN 24-May-06 06:22 tdrpa/tdworker/WinKeyboard.pyi
 -rw-rw-rw-  2.0 fat     6966 b- defN 24-May-06 06:18 tdrpa/tdworker/WinMouse.pyi
 -rw-rw-rw-  2.0 fat     3672 b- defN 24-May-06 06:25 tdrpa/tdworker/WinWindow.pyi
 -rw-rw-rw-  2.0 fat       60 b- defN 24-May-06 07:35 tdrpa/tdworker/__init__.pyi
--rw-rw-rw-  2.0 fat      663 b- defN 24-May-12 18:32 tdrpa.tdworker-1.1.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 18:32 tdrpa.tdworker-1.1.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-12 18:32 tdrpa.tdworker-1.1.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      850 b- defN 24-May-12 18:32 tdrpa.tdworker-1.1.4.1.dist-info/RECORD
-10 files, 1203689 bytes uncompressed, 417024 bytes compressed:  65.4%
+-rw-rw-rw-  2.0 fat      663 b- defN 24-May-12 18:59 tdrpa.tdworker-1.1.4.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 18:59 tdrpa.tdworker-1.1.4.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-12 18:59 tdrpa.tdworker-1.1.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      850 b- defN 24-May-12 18:59 tdrpa.tdworker-1.1.4.3.dist-info/RECORD
+10 files, 1205737 bytes uncompressed, 418150 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tdrpa/tdworker/WinWindow.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/__init__.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.1.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.1.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.1.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.1.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tdrpa.tdworker-1.1.4.1.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.1
+Version: 1.1.4.3
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
```

## Comparing `tdrpa.tdworker-1.1.4.1.dist-info/RECORD` & `tdrpa.tdworker-1.1.4.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tdrpa/tdworker.cp38-win_amd64.pyd,sha256=TiWGODH69HhHrwOET3Kh89nwZnNLMJLqXY86IGKAudM,1170944
+tdrpa/tdworker.cp38-win_amd64.pyd,sha256=ZZA40eZP8UrxK81Jc8UGUXJRTQzK6xKq53IqSDU_bbs,1172992
 tdrpa/tdworker/WinElement.pyi,sha256=Y6OBYXLr3w1xmRnnVGvbWtlX46v5d87NiOBkq-01O4s,15621
 tdrpa/tdworker/WinKeyboard.pyi,sha256=bRdaR6rM4FNzbIATUXRmt36fm3BhFarzpKruAJHklME,4815
 tdrpa/tdworker/WinMouse.pyi,sha256=H_59kcbqkJwoSfGQxte2Uo_f7J7n1ys2p9MKeZ1tnhU,6966
 tdrpa/tdworker/WinWindow.pyi,sha256=8X9FLtPKbw2rK2Wgc9z2ZmmWUAbogbNK6lmYhQ84dHU,3672
 tdrpa/tdworker/__init__.pyi,sha256=p5gNrSuSvmBtCSEM133tD7XSlW_2LyUB4svpQTlndv8,60
-tdrpa.tdworker-1.1.4.1.dist-info/METADATA,sha256=fL417IE3Xho_WN6PpPu8nKf5-vjshHDDzCupmfGiNI0,663
-tdrpa.tdworker-1.1.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdworker-1.1.4.1.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdworker-1.1.4.1.dist-info/RECORD,,
+tdrpa.tdworker-1.1.4.3.dist-info/METADATA,sha256=uL0Ua6odwGaODAfL6g8I8B2bpeP5D9N8z8_TTXyDU-U,663
+tdrpa.tdworker-1.1.4.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdworker-1.1.4.3.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdworker-1.1.4.3.dist-info/RECORD,,
```

