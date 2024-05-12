# Comparing `tmp/aksharamukha-2.2.1.tar.gz` & `tmp/aksharamukha-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharamukha-2.2.1.tar", last modified: Fri May 10 19:14:47 2024, max compression
+gzip compressed data, was "aksharamukha-2.2.2.tar", last modified: Sun May 12 16:32:29 2024, max compression
```

## Comparing `aksharamukha-2.2.1.tar` & `aksharamukha-2.2.2.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.283116 aksharamukha-2.2.1/
--rw-rw-rw-   0        0        0     4648 2024-05-10 19:14:47.283116 aksharamukha-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3255 2022-05-26 09:31:49.000000 aksharamukha-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.108475 aksharamukha-2.2.1/aksharamukha/
--rw-rw-rw-   0        0        0    13357 2024-03-19 23:12:33.000000 aksharamukha-2.2.1/aksharamukha/Convert.py
--rw-rw-rw-   0        0        0   131047 2024-05-10 16:16:47.000000 aksharamukha-2.2.1/aksharamukha/ConvertFix.py
--rw-rw-rw-   0        0        0    24800 2024-05-09 22:03:51.000000 aksharamukha-2.2.1/aksharamukha/FallBack.py
--rw-rw-rw-   0        0        0    16360 2024-05-10 18:04:10.000000 aksharamukha-2.2.1/aksharamukha/GeneralMap.py
--rw-rw-rw-   0        0        0     3372 2024-05-09 13:36:31.000000 aksharamukha-2.2.1/aksharamukha/PostOptions.py
--rw-rw-rw-   0        0        0   107098 2024-05-09 23:05:19.000000 aksharamukha-2.2.1/aksharamukha/PostProcess.py
--rw-rw-rw-   0        0        0      494 2022-05-07 22:19:20.000000 aksharamukha-2.2.1/aksharamukha/PreOptions.py
--rw-rw-rw-   0        0        0    58079 2024-05-10 16:11:23.000000 aksharamukha-2.2.1/aksharamukha/PreProcess.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.136474 aksharamukha-2.2.1/aksharamukha/ScriptMap/
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.181495 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/
--rw-rw-rw-   0        0        0     3918 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Balinese.py
--rw-rw-rw-   0        0        0     4147 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakKaro.py
--rw-rw-rw-   0        0        0     4207 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakManda.py
--rw-rw-rw-   0        0        0     4171 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py
--rw-rw-rw-   0        0        0     4165 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakSima.py
--rw-rw-rw-   0        0        0     4183 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakToba.py
--rw-rw-rw-   0        0        0     4301 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buginese.py
--rw-rw-rw-   0        0        0     4321 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buhid.py
--rw-rw-rw-   0        0        0     3947 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Burmese.py
--rw-rw-rw-   0        0        0     4178 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Cham.py
--rw-rw-rw-   0        0        0     4565 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/DivesAkuru.py
--rw-rw-rw-   0        0        0     4338 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Hanunoo.py
--rw-rw-rw-   0        0        0     3962 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Javanese.py
--rw-rw-rw-   0        0        0     4446 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Kawi.py
--rw-rw-rw-   0        0        0     3958 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhamtiShan.py
--rw-rw-rw-   0        0        0     3944 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Khmer.py
--rw-rw-rw-   0        0        0     3944 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhmerLoC.py
--rw-rw-rw-   0        0        0     4138 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhomThai.py
--rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhuenTham.py
--rw-rw-rw-   0        0        0     4354 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao.py
--rw-rw-rw-   0        0        0     4348 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao2.py
--rw-rw-rw-   0        0        0     4162 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LaoPali.py
--rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LaoTham.py
--rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LueTham.py
--rw-rw-rw-   0        0        0     4792 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Makasar.py
--rw-rw-rw-   0        0        0     4805 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Marchen.py
--rw-rw-rw-   0        0        0     3923 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Mon.py
--rw-rw-rw-   0        0        0     3988 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Pallava.py
--rw-rw-rw-   0        0        0     4324 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/PhagsPa.py
--rw-rw-rw-   0        0        0     4136 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Rejang.py
--rw-rw-rw-   0        0        0     3967 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Shan.py
--rw-rw-rw-   0        0        0     3967 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ShanLoC.py
--rw-rw-rw-   0        0        0     4175 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Siddham.py
--rw-rw-rw-   0        0        0     2391 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py
--rw-rw-rw-   0        0        0     4530 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Soyombo.py
--rw-rw-rw-   0        0        0     4093 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Sundanese.py
--rw-rw-rw-   0        0        0     4386 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tagalog.py
--rw-rw-rw-   0        0        0     4326 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py
--rw-rw-rw-   0        0        0     3977 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TaiLaing.py
--rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TaiTham.py
--rw-rw-rw-   0        0        0     4540 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thaana.py
--rw-rw-rw-   0        0        0     4122 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thai.py
--rw-rw-rw-   0        0        0     4094 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ThamLoC.py
--rw-rw-rw-   0        0        0     4045 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tibetan.py
--rw-rw-rw-   0        0        0     3997 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TibetanLoC.py
--rw-rw-rw-   0        0        0     4644 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.229598 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/
--rw-rw-rw-   0        0        0     4809 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ahom.py
--rw-rw-rw-   0        0        0     3870 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Assamese.py
--rw-rw-rw-   0        0        0     3869 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bengali.py
--rw-rw-rw-   0        0        0     3863 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/BengaliRaBa.py
--rw-rw-rw-   0        0        0     4541 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py
--rw-rw-rw-   0        0        0     3679 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Brahmi.py
--rw-rw-rw-   0        0        0     4641 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Chakma.py
--rw-rw-rw-   0        0        0     3747 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Devanagari.py
--rw-rw-rw-   0        0        0     4444 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Dogra.py
--rw-rw-rw-   0        0        0     4336 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Grantha.py
--rw-rw-rw-   0        0        0     3989 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py
--rw-rw-rw-   0        0        0     3875 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py
--rw-rw-rw-   0        0        0     3853 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gujarati.py
--rw-rw-rw-   0        0        0     4503 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py
--rw-rw-rw-   0        0        0     3982 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py
--rw-rw-rw-   0        0        0     3982 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GurmukhiLoC.py
--rw-rw-rw-   0        0        0     4138 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kaithi.py
--rw-rw-rw-   0        0        0     3845 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kannada.py
--rw-rw-rw-   0        0        0     3907 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kharoshthi.py
--rw-rw-rw-   0        0        0     4548 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khojki.py
--rw-rw-rw-   0        0        0     4230 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khudawadi.py
--rw-rw-rw-   0        0        0     4195 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Lepcha.py
--rw-rw-rw-   0        0        0     4191 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Limbu.py
--rw-rw-rw-   0        0        0     4237 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/LimbuLoC.py
--rw-rw-rw-   0        0        0     4612 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Mahajani.py
--rw-rw-rw-   0        0        0     3839 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Malayalam.py
--rw-rw-rw-   0        0        0     4545 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py
--rw-rw-rw-   0        0        0     4159 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py
--rw-rw-rw-   0        0        0     4323 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Modi.py
--rw-rw-rw-   0        0        0     4546 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Multani.py
--rw-rw-rw-   0        0        0     4316 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Nandinagari.py
--rw-rw-rw-   0        0        0     4293 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Newa.py
--rw-rw-rw-   0        0        0     3864 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Oriya.py
--rw-rw-rw-   0        0        0     3881 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ranjana.py
--rw-rw-rw-   0        0        0     3877 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Saurashtra.py
--rw-rw-rw-   0        0        0     4562 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py
--rw-rw-rw-   0        0        0     4449 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sharada.py
--rw-rw-rw-   0        0        0     3828 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py
--rw-rw-rw-   0        0        0     3786 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sinhala.py
--rw-rw-rw-   0        0        0     4011 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SylotiNagri.py
--rw-rw-rw-   0        0        0     3743 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py
--rw-rw-rw-   0        0        0     4284 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Takri.py
--rw-rw-rw-   0        0        0     4181 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tamil.py
--rw-rw-rw-   0        0        0     4668 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py
--rw-rw-rw-   0        0        0     3765 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilExtended.py
--rw-rw-rw-   0        0        0     3864 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py
--rw-rw-rw-   0        0        0     3880 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Telugu.py
--rw-rw-rw-   0        0        0     4289 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tirhuta.py
--rw-rw-rw-   0        0        0     4581 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Urdu.py
--rw-rw-rw-   0        0        0     4095 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.232596 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/
--rw-rw-rw-   0        0        0     4155 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/Hebrew.py
--rw-rw-rw-   0        0        0     4427 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/OldPersian.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/__init__.py
--rw-rw-rw-   0        0        0    24451 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/kana2roman.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.274114 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/
--rw-rw-rw-   0        0        0     3109 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Aksharaa.py
--rw-rw-rw-   0        0        0     2991 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Ariyaka.py
--rw-rw-rw-   0        0        0     3359 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/AssameseRomanLoC.py
--rw-rw-rw-   0        0        0     3843 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Avestan.py
--rw-rw-rw-   0        0        0     3288 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseRomanLoC.py
--rw-rw-rw-   0        0        0     3263 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseSimpleRomanLoC.py
--rw-rw-rw-   0        0        0     2950 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaNorth.py
--rw-rw-rw-   0        0        0     2950 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaSouth.py
--rw-rw-rw-   0        0        0     3364 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BengaliRomanLoC.py
--rw-rw-rw-   0        0        0     3369 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BurmeseRomanLoC.py
--rw-rw-rw-   0        0        0     3351 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/DevanagariRomanLoC.py
--rw-rw-rw-   0        0        0     3408 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GreekModern.py
--rw-rw-rw-   0        0        0     3353 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GujaratiRomanLoC.py
--rw-rw-rw-   0        0        0     3336 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GurmukhiLoCRomanLoC.py
--rw-rw-rw-   0        0        0     3409 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HK.py
--rw-rw-rw-   0        0        0     3962 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HanifiRohingya.py
--rw-rw-rw-   0        0        0     3361 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IAST.py
--rw-rw-rw-   0        0        0     3371 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IASTPali.py
--rw-rw-rw-   0        0        0     3516 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IPA.py
--rw-rw-rw-   0        0        0     3374 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ISO.py
--rw-rw-rw-   0        0        0     3380 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ISOPali.py
--rw-rw-rw-   0        0        0     1202 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Inter.py
--rw-rw-rw-   0        0        0     3412 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Itrans.py
--rw-rw-rw-   0        0        0     3271 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseRomanLoC.py
--rw-rw-rw-   0        0        0     3278 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseSimpleRomanLoC.py
--rw-rw-rw-   0        0        0     3368 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/KannadaRomanLoC.py
--rw-rw-rw-   0        0        0     3358 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/KhmerLoCRomanLoC.py
--rw-rw-rw-   0        0        0     3352 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/LimbuLoCRomanLoC.py
--rw-rw-rw-   0        0        0     3241 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mongolian.py
--rw-rw-rw-   0        0        0     3928 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mro.py
--rw-rw-rw-   0        0        0     3354 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/OriyaRomanLoC.py
--rw-rw-rw-   0        0        0     2991 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanColloquial.py
--rw-rw-rw-   0        0        0     2944 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanKana.py
--rw-rw-rw-   0        0        0     3016 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanReadable.py
--rw-rw-rw-   0        0        0     3457 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanSemitic.py
--rw-rw-rw-   0        0        0     3526 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RussianCyrillic.py
--rw-rw-rw-   0        0        0     2992 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SLP1.py
--rw-rw-rw-   0        0        0     3486 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Santali.py
--rw-rw-rw-   0        0        0     3328 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ShanLoCRomanLoC.py
--rw-rw-rw-   0        0        0     3360 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SinhalaRomanLoC.py
--rw-rw-rw-   0        0        0     4110 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SoraSompeng.py
--rw-rw-rw-   0        0        0     3365 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TeluguRomanLoC.py
--rw-rw-rw-   0        0        0     3371 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ThamLoCRomanLoC.py
--rw-rw-rw-   0        0        0     3276 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TibetanLoCRomanLoC.py
--rw-rw-rw-   0        0        0     3378 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Titus.py
--rw-rw-rw-   0        0        0     3532 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TolongSiki.py
--rw-rw-rw-   0        0        0     3543 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Velthuis.py
--rw-rw-rw-   0        0        0     3273 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX-kok.py
--rw-rw-rw-   0        0        0     3422 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX.py
--rw-rw-rw-   0        0        0     3802 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Wancho.py
--rw-rw-rw-   0        0        0     4040 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WarangCiti.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/__init__.py
--rw-rw-rw-   0        0        0     2426 2023-01-03 15:36:17.000000 aksharamukha-2.2.1/aksharamukha/demo.py
--rw-rw-rw-   0        0        0     5103 2023-06-19 19:15:40.000000 aksharamukha-2.2.1/aksharamukha/gimeltra.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.275114 aksharamukha-2.2.1/aksharamukha/json/
--rw-rw-rw-   0        0        0    77047 2024-01-12 16:16:19.000000 aksharamukha-2.2.1/aksharamukha/json/gimeltra_data.json
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.280114 aksharamukha-2.2.1/aksharamukha/test/
--rw-rw-rw-   0        0        0        0 2023-04-02 22:00:18.000000 aksharamukha-2.2.1/aksharamukha/test/__init__.py
--rw-rw-rw-   0        0        0     8192 2024-03-06 18:30:06.000000 aksharamukha-2.2.1/aksharamukha/test/loc_burmese_test_cases.py
--rw-rw-rw-   0        0        0     6118 2024-05-08 23:03:10.000000 aksharamukha-2.2.1/aksharamukha/test/loc_indic_test_cases.py
--rw-rw-rw-   0        0        0     2843 2024-03-18 16:22:08.000000 aksharamukha-2.2.1/aksharamukha/test/loc_khmer_test_cases.py
--rw-rw-rw-   0        0        0     3605 2024-03-07 16:31:45.000000 aksharamukha-2.2.1/aksharamukha/test/loc_shan_test_cases.py
--rw-rw-rw-   0        0        0     1674 2024-04-16 15:17:16.000000 aksharamukha-2.2.1/aksharamukha/test/loc_tham_test_cases.py
--rw-rw-rw-   0        0        0      664 2023-04-02 23:36:09.000000 aksharamukha-2.2.1/aksharamukha/test/test_file_generator.py
--rw-rw-rw-   0        0        0     6403 2024-05-09 23:05:02.000000 aksharamukha-2.2.1/aksharamukha/test/testsuite.py
--rw-rw-rw-   0        0        0    35363 2024-05-10 18:36:41.000000 aksharamukha-2.2.1/aksharamukha/transliterate.py
--rw-rw-rw-   0        0        0     4664 2024-05-10 19:07:52.000000 aksharamukha-2.2.1/aksharamukha/transliterate_file.py
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.283116 aksharamukha-2.2.1/aksharamukha/yaml/
--rw-rw-rw-   0        0        0     8250 2022-05-19 16:05:38.000000 aksharamukha-2.2.1/aksharamukha/yaml/aksharamukha-scripts.yaml
--rw-rw-rw-   0        0        0   189327 2022-05-19 15:32:30.000000 aksharamukha-2.2.1/aksharamukha/yaml/wikitra2-data.yaml
-drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.134472 aksharamukha-2.2.1/aksharamukha.egg-info/
--rw-rw-rw-   0        0        0     4648 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7895 2024-05-10 19:14:47.000000 aksharamukha-2.2.1/aksharamukha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-10 19:14:47.285662 aksharamukha-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     4561 2024-05-10 19:14:41.000000 aksharamukha-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.280284 aksharamukha-2.2.2/
+-rw-rw-rw-   0        0        0     4663 2024-05-12 16:32:29.280284 aksharamukha-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2024-05-12 16:03:09.000000 aksharamukha-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.070208 aksharamukha-2.2.2/aksharamukha/
+-rw-rw-rw-   0        0        0    13357 2024-03-19 23:12:33.000000 aksharamukha-2.2.2/aksharamukha/Convert.py
+-rw-rw-rw-   0        0        0   131254 2024-05-12 16:01:27.000000 aksharamukha-2.2.2/aksharamukha/ConvertFix.py
+-rw-rw-rw-   0        0        0    24800 2024-05-09 22:03:51.000000 aksharamukha-2.2.2/aksharamukha/FallBack.py
+-rw-rw-rw-   0        0        0    16360 2024-05-10 18:04:10.000000 aksharamukha-2.2.2/aksharamukha/GeneralMap.py
+-rw-rw-rw-   0        0        0     3372 2024-05-09 13:36:31.000000 aksharamukha-2.2.2/aksharamukha/PostOptions.py
+-rw-rw-rw-   0        0        0   107253 2024-05-11 22:41:40.000000 aksharamukha-2.2.2/aksharamukha/PostProcess.py
+-rw-rw-rw-   0        0        0      494 2022-05-07 22:19:20.000000 aksharamukha-2.2.2/aksharamukha/PreOptions.py
+-rw-rw-rw-   0        0        0    58079 2024-05-10 16:11:23.000000 aksharamukha-2.2.2/aksharamukha/PreProcess.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.108470 aksharamukha-2.2.2/aksharamukha/ScriptMap/
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.157612 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/
+-rw-rw-rw-   0        0        0     3918 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Balinese.py
+-rw-rw-rw-   0        0        0     4147 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakKaro.py
+-rw-rw-rw-   0        0        0     4207 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakManda.py
+-rw-rw-rw-   0        0        0     4171 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py
+-rw-rw-rw-   0        0        0     4165 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakSima.py
+-rw-rw-rw-   0        0        0     4183 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakToba.py
+-rw-rw-rw-   0        0        0     4301 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Buginese.py
+-rw-rw-rw-   0        0        0     4321 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Buhid.py
+-rw-rw-rw-   0        0        0     3947 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Burmese.py
+-rw-rw-rw-   0        0        0     4178 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Cham.py
+-rw-rw-rw-   0        0        0     4565 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/DivesAkuru.py
+-rw-rw-rw-   0        0        0     4338 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Hanunoo.py
+-rw-rw-rw-   0        0        0     3962 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Javanese.py
+-rw-rw-rw-   0        0        0     4446 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Kawi.py
+-rw-rw-rw-   0        0        0     3958 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhamtiShan.py
+-rw-rw-rw-   0        0        0     3944 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Khmer.py
+-rw-rw-rw-   0        0        0     3944 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhmerLoC.py
+-rw-rw-rw-   0        0        0     4138 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhomThai.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhuenTham.py
+-rw-rw-rw-   0        0        0     4354 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Lao.py
+-rw-rw-rw-   0        0        0     4348 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Lao2.py
+-rw-rw-rw-   0        0        0     4162 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/LaoPali.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/LaoTham.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/LueTham.py
+-rw-rw-rw-   0        0        0     4792 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Makasar.py
+-rw-rw-rw-   0        0        0     4805 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Marchen.py
+-rw-rw-rw-   0        0        0     3923 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Mon.py
+-rw-rw-rw-   0        0        0     3988 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Pallava.py
+-rw-rw-rw-   0        0        0     4324 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/PhagsPa.py
+-rw-rw-rw-   0        0        0     4136 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Rejang.py
+-rw-rw-rw-   0        0        0     3967 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Shan.py
+-rw-rw-rw-   0        0        0     3967 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/ShanLoC.py
+-rw-rw-rw-   0        0        0     4175 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Siddham.py
+-rw-rw-rw-   0        0        0     2391 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py
+-rw-rw-rw-   0        0        0     4530 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Soyombo.py
+-rw-rw-rw-   0        0        0     4093 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Sundanese.py
+-rw-rw-rw-   0        0        0     4386 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Tagalog.py
+-rw-rw-rw-   0        0        0     4326 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py
+-rw-rw-rw-   0        0        0     3977 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/TaiLaing.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/TaiTham.py
+-rw-rw-rw-   0        0        0     4540 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Thaana.py
+-rw-rw-rw-   0        0        0     4122 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Thai.py
+-rw-rw-rw-   0        0        0     4094 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/ThamLoC.py
+-rw-rw-rw-   0        0        0     4045 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Tibetan.py
+-rw-rw-rw-   0        0        0     3997 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/TibetanLoC.py
+-rw-rw-rw-   0        0        0     4644 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.211210 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/
+-rw-rw-rw-   0        0        0     4809 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Ahom.py
+-rw-rw-rw-   0        0        0     3870 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Assamese.py
+-rw-rw-rw-   0        0        0     3869 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Bengali.py
+-rw-rw-rw-   0        0        0     3863 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/BengaliRaBa.py
+-rw-rw-rw-   0        0        0     4541 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py
+-rw-rw-rw-   0        0        0     3679 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Brahmi.py
+-rw-rw-rw-   0        0        0     4641 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Chakma.py
+-rw-rw-rw-   0        0        0     3747 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Devanagari.py
+-rw-rw-rw-   0        0        0     4444 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Dogra.py
+-rw-rw-rw-   0        0        0     4336 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Grantha.py
+-rw-rw-rw-   0        0        0     3989 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py
+-rw-rw-rw-   0        0        0     3875 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py
+-rw-rw-rw-   0        0        0     3853 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Gujarati.py
+-rw-rw-rw-   0        0        0     4503 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py
+-rw-rw-rw-   0        0        0     3982 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py
+-rw-rw-rw-   0        0        0     3982 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GurmukhiLoC.py
+-rw-rw-rw-   0        0        0     4138 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Kaithi.py
+-rw-rw-rw-   0        0        0     3845 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Kannada.py
+-rw-rw-rw-   0        0        0     3907 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Kharoshthi.py
+-rw-rw-rw-   0        0        0     4548 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Khojki.py
+-rw-rw-rw-   0        0        0     4230 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Khudawadi.py
+-rw-rw-rw-   0        0        0     4195 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Lepcha.py
+-rw-rw-rw-   0        0        0     4191 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Limbu.py
+-rw-rw-rw-   0        0        0     4237 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/LimbuLoC.py
+-rw-rw-rw-   0        0        0     4612 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Mahajani.py
+-rw-rw-rw-   0        0        0     3839 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Malayalam.py
+-rw-rw-rw-   0        0        0     4545 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py
+-rw-rw-rw-   0        0        0     4159 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py
+-rw-rw-rw-   0        0        0     4323 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Modi.py
+-rw-rw-rw-   0        0        0     4546 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Multani.py
+-rw-rw-rw-   0        0        0     4316 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Nandinagari.py
+-rw-rw-rw-   0        0        0     4293 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Newa.py
+-rw-rw-rw-   0        0        0     3864 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Oriya.py
+-rw-rw-rw-   0        0        0     3881 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Ranjana.py
+-rw-rw-rw-   0        0        0     3877 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Saurashtra.py
+-rw-rw-rw-   0        0        0     4562 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py
+-rw-rw-rw-   0        0        0     4449 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Sharada.py
+-rw-rw-rw-   0        0        0     3828 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py
+-rw-rw-rw-   0        0        0     3786 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Sinhala.py
+-rw-rw-rw-   0        0        0     4011 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/SylotiNagri.py
+-rw-rw-rw-   0        0        0     3743 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py
+-rw-rw-rw-   0        0        0     4284 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Takri.py
+-rw-rw-rw-   0        0        0     4181 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Tamil.py
+-rw-rw-rw-   0        0        0     4668 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py
+-rw-rw-rw-   0        0        0     3765 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/TamilExtended.py
+-rw-rw-rw-   0        0        0     3864 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py
+-rw-rw-rw-   0        0        0     3880 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Telugu.py
+-rw-rw-rw-   0        0        0     4289 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Tirhuta.py
+-rw-rw-rw-   0        0        0     4581 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Urdu.py
+-rw-rw-rw-   0        0        0     4095 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.214218 aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/
+-rw-rw-rw-   0        0        0     4155 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/Hebrew.py
+-rw-rw-rw-   0        0        0     4427 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/OldPersian.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/__init__.py
+-rw-rw-rw-   0        0        0    24451 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/kana2roman.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.266499 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/
+-rw-rw-rw-   0        0        0     3109 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Aksharaa.py
+-rw-rw-rw-   0        0        0     2991 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Ariyaka.py
+-rw-rw-rw-   0        0        0     3359 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/AssameseRomanLoC.py
+-rw-rw-rw-   0        0        0     3843 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Avestan.py
+-rw-rw-rw-   0        0        0     3288 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BalineseRomanLoC.py
+-rw-rw-rw-   0        0        0     3263 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BalineseSimpleRomanLoC.py
+-rw-rw-rw-   0        0        0     2950 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BarahaNorth.py
+-rw-rw-rw-   0        0        0     2950 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BarahaSouth.py
+-rw-rw-rw-   0        0        0     3364 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BengaliRomanLoC.py
+-rw-rw-rw-   0        0        0     3369 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BurmeseRomanLoC.py
+-rw-rw-rw-   0        0        0     3351 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/DevanagariRomanLoC.py
+-rw-rw-rw-   0        0        0     3408 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/GreekModern.py
+-rw-rw-rw-   0        0        0     3353 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/GujaratiRomanLoC.py
+-rw-rw-rw-   0        0        0     3336 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/GurmukhiLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3409 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/HK.py
+-rw-rw-rw-   0        0        0     3962 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/HanifiRohingya.py
+-rw-rw-rw-   0        0        0     3361 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/IAST.py
+-rw-rw-rw-   0        0        0     3371 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/IASTPali.py
+-rw-rw-rw-   0        0        0     3516 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/IPA.py
+-rw-rw-rw-   0        0        0     3374 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ISO.py
+-rw-rw-rw-   0        0        0     3380 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ISOPali.py
+-rw-rw-rw-   0        0        0     1202 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Inter.py
+-rw-rw-rw-   0        0        0     3412 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Itrans.py
+-rw-rw-rw-   0        0        0     3271 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/JavaneseRomanLoC.py
+-rw-rw-rw-   0        0        0     3278 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/JavaneseSimpleRomanLoC.py
+-rw-rw-rw-   0        0        0     3368 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/KannadaRomanLoC.py
+-rw-rw-rw-   0        0        0     3358 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/KhmerLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3352 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/LimbuLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3241 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Mongolian.py
+-rw-rw-rw-   0        0        0     3928 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Mro.py
+-rw-rw-rw-   0        0        0     3354 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/OriyaRomanLoC.py
+-rw-rw-rw-   0        0        0     2991 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanColloquial.py
+-rw-rw-rw-   0        0        0     2944 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanKana.py
+-rw-rw-rw-   0        0        0     3016 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanReadable.py
+-rw-rw-rw-   0        0        0     3457 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanSemitic.py
+-rw-rw-rw-   0        0        0     3526 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RussianCyrillic.py
+-rw-rw-rw-   0        0        0     2992 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/SLP1.py
+-rw-rw-rw-   0        0        0     3486 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Santali.py
+-rw-rw-rw-   0        0        0     3328 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ShanLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3360 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/SinhalaRomanLoC.py
+-rw-rw-rw-   0        0        0     4110 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/SoraSompeng.py
+-rw-rw-rw-   0        0        0     3365 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/TeluguRomanLoC.py
+-rw-rw-rw-   0        0        0     3371 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ThamLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3276 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/TibetanLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3378 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Titus.py
+-rw-rw-rw-   0        0        0     3532 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/TolongSiki.py
+-rw-rw-rw-   0        0        0     3543 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Velthuis.py
+-rw-rw-rw-   0        0        0     3273 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/WX-kok.py
+-rw-rw-rw-   0        0        0     3422 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/WX.py
+-rw-rw-rw-   0        0        0     3802 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Wancho.py
+-rw-rw-rw-   0        0        0     4040 2024-05-10 18:21:32.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/WarangCiti.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/ScriptMap/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.2/aksharamukha/__init__.py
+-rw-rw-rw-   0        0        0     2426 2023-01-03 15:36:17.000000 aksharamukha-2.2.2/aksharamukha/demo.py
+-rw-rw-rw-   0        0        0     5103 2023-06-19 19:15:40.000000 aksharamukha-2.2.2/aksharamukha/gimeltra.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.267506 aksharamukha-2.2.2/aksharamukha/json/
+-rw-rw-rw-   0        0        0    77047 2024-01-12 16:16:19.000000 aksharamukha-2.2.2/aksharamukha/json/gimeltra_data.json
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.274989 aksharamukha-2.2.2/aksharamukha/test/
+-rw-rw-rw-   0        0        0        0 2023-04-02 22:00:18.000000 aksharamukha-2.2.2/aksharamukha/test/__init__.py
+-rw-rw-rw-   0        0        0     8192 2024-03-06 18:30:06.000000 aksharamukha-2.2.2/aksharamukha/test/loc_burmese_test_cases.py
+-rw-rw-rw-   0        0        0     6118 2024-05-08 23:03:10.000000 aksharamukha-2.2.2/aksharamukha/test/loc_indic_test_cases.py
+-rw-rw-rw-   0        0        0     2843 2024-03-18 16:22:08.000000 aksharamukha-2.2.2/aksharamukha/test/loc_khmer_test_cases.py
+-rw-rw-rw-   0        0        0     3605 2024-03-07 16:31:45.000000 aksharamukha-2.2.2/aksharamukha/test/loc_shan_test_cases.py
+-rw-rw-rw-   0        0        0     1674 2024-04-16 15:17:16.000000 aksharamukha-2.2.2/aksharamukha/test/loc_tham_test_cases.py
+-rw-rw-rw-   0        0        0      664 2023-04-02 23:36:09.000000 aksharamukha-2.2.2/aksharamukha/test/test_file_generator.py
+-rw-rw-rw-   0        0        0     6403 2024-05-09 23:05:02.000000 aksharamukha-2.2.2/aksharamukha/test/testsuite.py
+-rw-rw-rw-   0        0        0    35458 2024-05-10 21:51:25.000000 aksharamukha-2.2.2/aksharamukha/transliterate.py
+-rw-rw-rw-   0        0        0     4664 2024-05-10 19:07:52.000000 aksharamukha-2.2.2/aksharamukha/transliterate_file.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.279315 aksharamukha-2.2.2/aksharamukha/yaml/
+-rw-rw-rw-   0        0        0     8250 2022-05-19 16:05:38.000000 aksharamukha-2.2.2/aksharamukha/yaml/aksharamukha-scripts.yaml
+-rw-rw-rw-   0        0        0   189327 2022-05-19 15:32:30.000000 aksharamukha-2.2.2/aksharamukha/yaml/wikitra2-data.yaml
+drwxrwxrwx   0        0        0        0 2024-05-12 16:32:29.106945 aksharamukha-2.2.2/aksharamukha.egg-info/
+-rw-rw-rw-   0        0        0     4663 2024-05-12 16:32:28.000000 aksharamukha-2.2.2/aksharamukha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7895 2024-05-12 16:32:28.000000 aksharamukha-2.2.2/aksharamukha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:32:28.000000 aksharamukha-2.2.2/aksharamukha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-12 16:32:28.000000 aksharamukha-2.2.2/aksharamukha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-12 16:32:28.000000 aksharamukha-2.2.2/aksharamukha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-12 16:32:29.281790 aksharamukha-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     4561 2024-05-12 16:31:57.000000 aksharamukha-2.2.2/setup.py
```

### Comparing `aksharamukha-2.2.1/PKG-INFO` & `aksharamukha-2.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharamukha
-Version: 2.2.1
+Version: 2.2.2
 Summary: Provides script conversion (a.k.a transliteration) between various scripts
 Home-page: https://github.com/virtualvinodh/aksharamukha-python
 Author: Vinodh Rajan
 Author-email: vinodh@virtualvindh.com
 License: GNU AGPL 3.0
 Keywords: unicode semitic arabic syriac hebrew indic indian language script brahmi brahmic asian transliteration conversion writing alphabet romanization
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,26 +30,28 @@
 
 # Aksharamukha Python Package
 
 Aksharamukha aims to provide transliteration a.k.a script conversion between various scripts within the Indic cultural sphere.  These include historic scripts, contemporary Brahmi-derived/inspired scripts, scripts invented for minority Indian languages, scripts that have co-existed with Indic scripts (like Avestan) or linguistically related scripts like Old Persian. It also specifically provides lossless transliteration between the main Indian scripts (along with Sinhala).
 
 Apart from the simple mapping of characters, Askharamukha also attempts to implement various script/language-specific orthographic conventions (where known) such as vowel lengths, gemination and nasalization. It also provides several customization options to fine-tune and get the desired orthography.
 
-Aksharamukha as of now supports 120 scripts and 21 romanization methods. The scripts supported are:
-
-*Ahom, Arabic, Ariyaka, Assamese, Avestan, Balinese, Batak Karo, Batak Mandailing, Batak Pakpak, Batak Simalungun, Batak Toba, Bengali (Bangla), Bhaiksuki, Brahmi, Buginese (Lontara), Buhid, Burmese (Myanmar), Chakma, Cham, Cyrillic (Russian), Devanagari, Dogra, Elymaic, Ethiopic (Abjad), Gondi (Gunjala), Gondi (Masaram), Grantha, Grantha (Pandya), Gujarati, Hanunoo, Hatran, Hebrew, Hebrew (Judeo-Arabic), Imperial Aramaic, Inscriptional Pahlavi, Inscriptional Parthian, Japanese (Hiragana), Japanese (Katakana), Javanese, Kaithi, Kannada, Kawi, Khamti Shan, Kharoshthi, Khmer (Cambodian), Khojki, Khom Thai, Khudawadi, Lao, Lao (Pali), Lepcha, Limbu, Mahajani, Makasar, Malayalam, Manichaean, Marchen, Meetei Mayek (Manipuri), Modi, Mon, Mongolian (Ali Gali), Mro, Multani, Nabataean, Nandinagari, Newa (Nepal Bhasa), Old North Arabian, Old Persian, Old Sogdian, Old South Arabian, Oriya (Odia), Pallava, Palmyrene, Persian, PhagsPa, Phoenician, Psalter Pahlavi, Punjabi (Gurmukhi), Ranjana (Lantsa), Rejang, Rohingya (Hanifi), Roman (IPA Indic), Samaritan, Santali (Ol Chiki), Saurashtra, Shahmukhi, Shan, Sharada, Siddham, Sinhala, Sogdian, Sora Sompeng, Soyombo, Sundanese, Syloti Nagari, Syriac (Eastern), Syriac (Estrangela), Syriac (Western), Tagalog, Tagbanwa, Tai Laing, Takri, Tamil, Tamil (Extended), Tamil Brahmi, Telugu, Thaana (Dhivehi), Thai, Tham (Lanna), Tham (Lao), Tham (Tai Khuen), Tham (Tai Lue), Tibetan, Tirhuta (Maithili), Ugaritic, Urdu, Vatteluttu, Wancho, Warang Citi, Zanabazar Square*
-
-The Indic Romanization Formats supported are: *Harvard-Kyoto, ITRANS, Velthuis, IAST, IAST (Pāḷi), ISO, ISO (Pāḷi), Titus, SLP1, WX, Roman (Readable), Roman (Colloquial)* . The Semitic Romanization Formats supported are: *Semitic (Aksharamukha), Semitic Typeable (Aksharamukha), ISO 259 Hebrew, SBL Hebrew, ISO 233 Arabic, DMG Persian*
-
 ## Usage and Examples
 
 Please use `pip aksharamukha` to install the Python package.
 
-Please find the usage instructions and relevant documentation [here](http://aksharamukha.appspot.com/#/python).
+Please find the usage instructions and relevant documentation [here](https://www.aksharamukha.com/python).
 
 ## Online Version
 
-The package as an online tool with a pretty web interface is available [here](http://aksharamukha.appspot.com/).
+The package as an online tool with a pretty web interface is available [here](https://www.aksharamukha.com).
 
 ## Contact
 
 If you have any questions please head to [Github](https://github.com/virtualvinodh/aksharamukha-python) or mail vinodh@virtualvinodh.com
+
+## Scripts Supported
+
+Aksharamukha as of now supports 120 scripts and 21 romanization methods. The scripts supported are:
+
+*Ahom, Arabic, Ariyaka, Assamese, Avestan, Balinese, Batak Karo, Batak Mandailing, Batak Pakpak, Batak Simalungun, Batak Toba, Bengali (Bangla), Bhaiksuki, Brahmi, Buginese (Lontara), Buhid, Burmese (Myanmar), Chakma, Cham, Cyrillic (Russian), Devanagari, Dogra, Elymaic, Ethiopic (Abjad), Gondi (Gunjala), Gondi (Masaram), Grantha, Grantha (Pandya), Gujarati, Hanunoo, Hatran, Hebrew, Hebrew (Judeo-Arabic), Imperial Aramaic, Inscriptional Pahlavi, Inscriptional Parthian, Japanese (Hiragana), Japanese (Katakana), Javanese, Kaithi, Kannada, Kawi, Khamti Shan, Kharoshthi, Khmer (Cambodian), Khojki, Khom Thai, Khudawadi, Lao, Lao (Pali), Lepcha, Limbu, Mahajani, Makasar, Malayalam, Manichaean, Marchen, Meetei Mayek (Manipuri), Modi, Mon, Mongolian (Ali Gali), Mro, Multani, Nabataean, Nandinagari, Newa (Nepal Bhasa), Old North Arabian, Old Persian, Old Sogdian, Old South Arabian, Oriya (Odia), Pallava, Palmyrene, Persian, PhagsPa, Phoenician, Psalter Pahlavi, Punjabi (Gurmukhi), Ranjana (Lantsa), Rejang, Rohingya (Hanifi), Roman (IPA Indic), Samaritan, Santali (Ol Chiki), Saurashtra, Shahmukhi, Shan, Sharada, Siddham, Sinhala, Sogdian, Sora Sompeng, Soyombo, Sundanese, Syloti Nagari, Syriac (Eastern), Syriac (Estrangela), Syriac (Western), Tagalog, Tagbanwa, Tai Laing, Takri, Tamil, Tamil (Extended), Tamil Brahmi, Telugu, Thaana (Dhivehi), Thai, Tham (Lanna), Tham (Lao), Tham (Tai Khuen), Tham (Tai Lue), Tibetan, Tirhuta (Maithili), Ugaritic, Urdu, Vatteluttu, Wancho, Warang Citi, Zanabazar Square*
+
+The Indic Romanization Formats supported are: *Harvard-Kyoto, ITRANS, Velthuis, IAST, IAST (Pāḷi), ISO, ISO (Pāḷi), Titus, SLP1, WX, Roman (Readable), Roman (Colloquial)* . The Semitic Romanization Formats supported are: *Semitic (Aksharamukha), Semitic Typeable (Aksharamukha), ISO 259 Hebrew, SBL Hebrew, ISO 233 Arabic, DMG Persian*
```

### Comparing `aksharamukha-2.2.1/README.md` & `aksharamukha-2.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # Aksharamukha Python Package
 
 Aksharamukha aims to provide transliteration a.k.a script conversion between various scripts within the Indic cultural sphere.  These include historic scripts, contemporary Brahmi-derived/inspired scripts, scripts invented for minority Indian languages, scripts that have co-existed with Indic scripts (like Avestan) or linguistically related scripts like Old Persian. It also specifically provides lossless transliteration between the main Indian scripts (along with Sinhala).
 
 Apart from the simple mapping of characters, Askharamukha also attempts to implement various script/language-specific orthographic conventions (where known) such as vowel lengths, gemination and nasalization. It also provides several customization options to fine-tune and get the desired orthography.
 
-Aksharamukha as of now supports 120 scripts and 21 romanization methods. The scripts supported are:
-
-*Ahom, Arabic, Ariyaka, Assamese, Avestan, Balinese, Batak Karo, Batak Mandailing, Batak Pakpak, Batak Simalungun, Batak Toba, Bengali (Bangla), Bhaiksuki, Brahmi, Buginese (Lontara), Buhid, Burmese (Myanmar), Chakma, Cham, Cyrillic (Russian), Devanagari, Dogra, Elymaic, Ethiopic (Abjad), Gondi (Gunjala), Gondi (Masaram), Grantha, Grantha (Pandya), Gujarati, Hanunoo, Hatran, Hebrew, Hebrew (Judeo-Arabic), Imperial Aramaic, Inscriptional Pahlavi, Inscriptional Parthian, Japanese (Hiragana), Japanese (Katakana), Javanese, Kaithi, Kannada, Kawi, Khamti Shan, Kharoshthi, Khmer (Cambodian), Khojki, Khom Thai, Khudawadi, Lao, Lao (Pali), Lepcha, Limbu, Mahajani, Makasar, Malayalam, Manichaean, Marchen, Meetei Mayek (Manipuri), Modi, Mon, Mongolian (Ali Gali), Mro, Multani, Nabataean, Nandinagari, Newa (Nepal Bhasa), Old North Arabian, Old Persian, Old Sogdian, Old South Arabian, Oriya (Odia), Pallava, Palmyrene, Persian, PhagsPa, Phoenician, Psalter Pahlavi, Punjabi (Gurmukhi), Ranjana (Lantsa), Rejang, Rohingya (Hanifi), Roman (IPA Indic), Samaritan, Santali (Ol Chiki), Saurashtra, Shahmukhi, Shan, Sharada, Siddham, Sinhala, Sogdian, Sora Sompeng, Soyombo, Sundanese, Syloti Nagari, Syriac (Eastern), Syriac (Estrangela), Syriac (Western), Tagalog, Tagbanwa, Tai Laing, Takri, Tamil, Tamil (Extended), Tamil Brahmi, Telugu, Thaana (Dhivehi), Thai, Tham (Lanna), Tham (Lao), Tham (Tai Khuen), Tham (Tai Lue), Tibetan, Tirhuta (Maithili), Ugaritic, Urdu, Vatteluttu, Wancho, Warang Citi, Zanabazar Square*
-
-The Indic Romanization Formats supported are: *Harvard-Kyoto, ITRANS, Velthuis, IAST, IAST (Pāḷi), ISO, ISO (Pāḷi), Titus, SLP1, WX, Roman (Readable), Roman (Colloquial)* . The Semitic Romanization Formats supported are: *Semitic (Aksharamukha), Semitic Typeable (Aksharamukha), ISO 259 Hebrew, SBL Hebrew, ISO 233 Arabic, DMG Persian*
-
 ## Usage and Examples
 
 Please use `pip aksharamukha` to install the Python package.
 
-Please find the usage instructions and relevant documentation [here](http://aksharamukha.appspot.com/#/python).
+Please find the usage instructions and relevant documentation [here](https://www.aksharamukha.com/python).
 
 ## Online Version
 
-The package as an online tool with a pretty web interface is available [here](http://aksharamukha.appspot.com/).
+The package as an online tool with a pretty web interface is available [here](https://www.aksharamukha.com).
 
 ## Contact
 
 If you have any questions please head to [Github](https://github.com/virtualvinodh/aksharamukha-python) or mail vinodh@virtualvinodh.com
+
+## Scripts Supported
+
+Aksharamukha as of now supports 120 scripts and 21 romanization methods. The scripts supported are:
+
+*Ahom, Arabic, Ariyaka, Assamese, Avestan, Balinese, Batak Karo, Batak Mandailing, Batak Pakpak, Batak Simalungun, Batak Toba, Bengali (Bangla), Bhaiksuki, Brahmi, Buginese (Lontara), Buhid, Burmese (Myanmar), Chakma, Cham, Cyrillic (Russian), Devanagari, Dogra, Elymaic, Ethiopic (Abjad), Gondi (Gunjala), Gondi (Masaram), Grantha, Grantha (Pandya), Gujarati, Hanunoo, Hatran, Hebrew, Hebrew (Judeo-Arabic), Imperial Aramaic, Inscriptional Pahlavi, Inscriptional Parthian, Japanese (Hiragana), Japanese (Katakana), Javanese, Kaithi, Kannada, Kawi, Khamti Shan, Kharoshthi, Khmer (Cambodian), Khojki, Khom Thai, Khudawadi, Lao, Lao (Pali), Lepcha, Limbu, Mahajani, Makasar, Malayalam, Manichaean, Marchen, Meetei Mayek (Manipuri), Modi, Mon, Mongolian (Ali Gali), Mro, Multani, Nabataean, Nandinagari, Newa (Nepal Bhasa), Old North Arabian, Old Persian, Old Sogdian, Old South Arabian, Oriya (Odia), Pallava, Palmyrene, Persian, PhagsPa, Phoenician, Psalter Pahlavi, Punjabi (Gurmukhi), Ranjana (Lantsa), Rejang, Rohingya (Hanifi), Roman (IPA Indic), Samaritan, Santali (Ol Chiki), Saurashtra, Shahmukhi, Shan, Sharada, Siddham, Sinhala, Sogdian, Sora Sompeng, Soyombo, Sundanese, Syloti Nagari, Syriac (Eastern), Syriac (Estrangela), Syriac (Western), Tagalog, Tagbanwa, Tai Laing, Takri, Tamil, Tamil (Extended), Tamil Brahmi, Telugu, Thaana (Dhivehi), Thai, Tham (Lanna), Tham (Lao), Tham (Tai Khuen), Tham (Tai Lue), Tibetan, Tirhuta (Maithili), Ugaritic, Urdu, Vatteluttu, Wancho, Warang Citi, Zanabazar Square*
+
+The Indic Romanization Formats supported are: *Harvard-Kyoto, ITRANS, Velthuis, IAST, IAST (Pāḷi), ISO, ISO (Pāḷi), Titus, SLP1, WX, Roman (Readable), Roman (Colloquial)* . The Semitic Romanization Formats supported are: *Semitic (Aksharamukha), Semitic Typeable (Aksharamukha), ISO 259 Hebrew, SBL Hebrew, ISO 233 Arabic, DMG Persian*
```

### Comparing `aksharamukha-2.2.1/aksharamukha/Convert.py` & `aksharamukha-2.2.2/aksharamukha/Convert.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ConvertFix.py` & `aksharamukha-2.2.2/aksharamukha/ConvertFix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1880,14 +1880,17 @@
     ListC = [Tibetan.ViramaMap[0]+chr(x) for x in range(0x0F40,0x0F68)] # Consonants
     ListSubC = [chr(x+80) for x in range(0x0F40,0x0F68)] # Subjoined Consonants
 
     SubC = ["ཝྭ","ཡྱ","རྱ","རྭ", "ྺྭ"]
     SubMinC = ["ཝྺ","ཡྻ","ཪྻ","ཪྺ", "ྺྺ"]
 
     if not reverse:
+        #introduce virama for Jihva/Upadh
+        Strng = re.sub('([ྈྉ])', r'\1' + '\u0f84',  Strng)
+
         for x,y in zip(ListC,ListSubC):
             Strng = Strng.replace(x,y)
 
         for x,y in zip(SubC,SubMinC):
             Strng = Strng.replace(x,y)
 
         Strng = Strng.replace(' ', '\u0F0B')
@@ -1923,14 +1926,17 @@
 
         Strng = Strng.replace("༺", "(")
         Strng = Strng.replace("༻", ")")
 
         Strng = Strng.replace("༼", "{")
         Strng = Strng.replace("༽", "}")
 
+        #remove virama from Jihva/Upadh
+        Strng = re.sub('([ྈྉ])(\u0f84)', r'\1',  Strng)
+
         if swapNative:
             Strng = Strng.replace('ཇྷ', 'ཛྷ') ## JHA -> DZHA
             Strng = Strng.replace("ཇ", "ཛ")
             Strng = Strng.replace('ཅ', 'ཙ')
             Strng = Strng.replace('ཆ', 'ཚ')
             Strng = Strng.replace("ཞ", "ཛྷ༹")
             Strng = Strng.replace("འ", "ཨ")
```

### Comparing `aksharamukha-2.2.1/aksharamukha/FallBack.py` & `aksharamukha-2.2.2/aksharamukha/FallBack.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/GeneralMap.py` & `aksharamukha-2.2.2/aksharamukha/GeneralMap.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/PostOptions.py` & `aksharamukha-2.2.2/aksharamukha/PostOptions.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/PostProcess.py` & `aksharamukha-2.2.2/aksharamukha/PostProcess.py`

 * *Files 1% similar despite different names*

```diff
@@ -2535,14 +2535,16 @@
 
     for ch, chvir in zip(chilluArch, chilluArchhVir):
         Strng = re.sub('(?<!' + vir + ')' + chvir + '(?!' + ListC + ')', ch, Strng)
 
     return Strng
 
 def MalayalamLineVirama(Strng):
+    #ListC = '(' + '|'.join(GM.CrunchSymbols(GM.CharactersNV,'Malayalam') + ['ഽ']) + ')'
+    #Strng = re.sub('\u0D4D'+'(?!'+ListC +')', '\u0D3B', Strng)
     Strng = Strng.replace('\u0D4D', '\u0D3B')
 
     return Strng
 
 def MalayalamCircVirama(Strng):
     Strng = Strng.replace('\u0D4D', '\u0D3C')
```

### Comparing `aksharamukha-2.2.1/aksharamukha/PreProcess.py` & `aksharamukha-2.2.2/aksharamukha/PreProcess.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Balinese.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Balinese.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakKaro.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakKaro.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakManda.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakManda.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakSima.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakSima.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakToba.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/BatakToba.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buginese.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Buginese.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buhid.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Buhid.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Burmese.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Burmese.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Cham.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Cham.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/DivesAkuru.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/DivesAkuru.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Hanunoo.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Hanunoo.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Javanese.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Javanese.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Kawi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Kawi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhamtiShan.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhamtiShan.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Khmer.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Khmer.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhmerLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhmerLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhomThai.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhomThai.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhuenTham.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/KhuenTham.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Lao.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao2.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Lao2.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LaoPali.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/LaoPali.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LaoTham.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/LaoTham.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LueTham.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/LueTham.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Makasar.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Makasar.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Marchen.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Marchen.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Mon.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Mon.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Pallava.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Pallava.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/PhagsPa.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/PhagsPa.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Rejang.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Rejang.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Shan.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Shan.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ShanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/ShanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Siddham.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Siddham.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Soyombo.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Soyombo.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Sundanese.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Sundanese.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tagalog.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Tagalog.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TaiLaing.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/TaiLaing.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TaiTham.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/TaiTham.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thaana.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Thaana.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thai.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Thai.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ThamLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/ThamLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tibetan.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/Tibetan.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TibetanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/TibetanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ahom.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Ahom.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Assamese.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Assamese.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bengali.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Bengali.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/BengaliRaBa.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/BengaliRaBa.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Brahmi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Brahmi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Chakma.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Chakma.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Devanagari.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Devanagari.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Dogra.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Dogra.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Grantha.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Grantha.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gujarati.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Gujarati.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GurmukhiLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/GurmukhiLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kaithi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Kaithi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kannada.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Kannada.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kharoshthi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Kharoshthi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khojki.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Khojki.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khudawadi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Khudawadi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Lepcha.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Lepcha.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Limbu.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Limbu.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/LimbuLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/LimbuLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Mahajani.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Mahajani.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Malayalam.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Malayalam.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Modi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Modi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Multani.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Multani.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Nandinagari.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Nandinagari.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Newa.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Newa.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Oriya.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Oriya.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ranjana.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Ranjana.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Saurashtra.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Saurashtra.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sharada.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Sharada.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sinhala.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Sinhala.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SylotiNagri.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/SylotiNagri.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Takri.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Takri.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tamil.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Tamil.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilExtended.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/TamilExtended.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Telugu.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Telugu.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tirhuta.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Tirhuta.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Urdu.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Urdu.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/Hebrew.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/Hebrew.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/OldPersian.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/OldPersian.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/kana2roman.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/NonIndic/kana2roman.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Aksharaa.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Aksharaa.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Ariyaka.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Ariyaka.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/AssameseRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/AssameseRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Avestan.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Avestan.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BalineseRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseSimpleRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BalineseSimpleRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaNorth.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BarahaNorth.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaSouth.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BarahaSouth.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BengaliRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BengaliRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BurmeseRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/BurmeseRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/DevanagariRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/DevanagariRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GreekModern.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/GreekModern.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GujaratiRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/GujaratiRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GurmukhiLoCRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/GurmukhiLoCRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HK.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/HK.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HanifiRohingya.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/HanifiRohingya.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IAST.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/IAST.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IASTPali.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/IASTPali.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IPA.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/IPA.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ISO.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ISO.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ISOPali.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ISOPali.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Inter.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Inter.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Itrans.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Itrans.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/JavaneseRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseSimpleRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/JavaneseSimpleRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/KannadaRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/KannadaRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/KhmerLoCRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/KhmerLoCRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/LimbuLoCRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/LimbuLoCRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mongolian.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Mongolian.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mro.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Mro.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/OriyaRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/OriyaRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanColloquial.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanColloquial.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanKana.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanKana.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanReadable.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanReadable.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanSemitic.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RomanSemitic.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RussianCyrillic.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/RussianCyrillic.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SLP1.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/SLP1.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Santali.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Santali.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ShanLoCRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ShanLoCRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SinhalaRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/SinhalaRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SoraSompeng.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/SoraSompeng.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TeluguRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/TeluguRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ThamLoCRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/ThamLoCRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TibetanLoCRomanLoC.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/TibetanLoCRomanLoC.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Titus.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Titus.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TolongSiki.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/TolongSiki.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Velthuis.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Velthuis.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX-kok.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/WX-kok.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/WX.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Wancho.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/Wancho.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WarangCiti.py` & `aksharamukha-2.2.2/aksharamukha/ScriptMap/Roman/WarangCiti.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/demo.py` & `aksharamukha-2.2.2/aksharamukha/demo.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/gimeltra.py` & `aksharamukha-2.2.2/aksharamukha/gimeltra.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/json/gimeltra_data.json` & `aksharamukha-2.2.2/aksharamukha/json/gimeltra_data.json`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/test/loc_burmese_test_cases.py` & `aksharamukha-2.2.2/aksharamukha/test/loc_burmese_test_cases.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/test/loc_indic_test_cases.py` & `aksharamukha-2.2.2/aksharamukha/test/loc_indic_test_cases.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/test/loc_khmer_test_cases.py` & `aksharamukha-2.2.2/aksharamukha/test/loc_khmer_test_cases.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/test/loc_shan_test_cases.py` & `aksharamukha-2.2.2/aksharamukha/test/loc_shan_test_cases.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/test/loc_tham_test_cases.py` & `aksharamukha-2.2.2/aksharamukha/test/loc_tham_test_cases.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/test/test_file_generator.py` & `aksharamukha-2.2.2/aksharamukha/test/test_file_generator.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/test/testsuite.py` & `aksharamukha-2.2.2/aksharamukha/test/testsuite.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/transliterate.py` & `aksharamukha-2.2.2/aksharamukha/transliterate.py`

 * *Files 1% similar despite different names*

```diff
@@ -865,8 +865,13 @@
     from pathlib import Path
     cwd = Path(Path(__file__).parent)
     with open(Path(cwd, "json/gimeltra_data.json"), "r", encoding="utf-8") as f:
         data = json.load(f)
 
     return data
 
+@functools.lru_cache(maxsize=None)
+def getOptions(script):
+    #json.load('')
+    return
+
 ## add the new libraries to requiesments.txt in both folders
```

### Comparing `aksharamukha-2.2.1/aksharamukha/transliterate_file.py` & `aksharamukha-2.2.2/aksharamukha/transliterate_file.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/yaml/aksharamukha-scripts.yaml` & `aksharamukha-2.2.2/aksharamukha/yaml/aksharamukha-scripts.yaml`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha/yaml/wikitra2-data.yaml` & `aksharamukha-2.2.2/aksharamukha/yaml/wikitra2-data.yaml`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/aksharamukha.egg-info/PKG-INFO` & `aksharamukha-2.2.2/aksharamukha.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharamukha
-Version: 2.2.1
+Version: 2.2.2
 Summary: Provides script conversion (a.k.a transliteration) between various scripts
 Home-page: https://github.com/virtualvinodh/aksharamukha-python
 Author: Vinodh Rajan
 Author-email: vinodh@virtualvindh.com
 License: GNU AGPL 3.0
 Keywords: unicode semitic arabic syriac hebrew indic indian language script brahmi brahmic asian transliteration conversion writing alphabet romanization
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,26 +30,28 @@
 
 # Aksharamukha Python Package
 
 Aksharamukha aims to provide transliteration a.k.a script conversion between various scripts within the Indic cultural sphere.  These include historic scripts, contemporary Brahmi-derived/inspired scripts, scripts invented for minority Indian languages, scripts that have co-existed with Indic scripts (like Avestan) or linguistically related scripts like Old Persian. It also specifically provides lossless transliteration between the main Indian scripts (along with Sinhala).
 
 Apart from the simple mapping of characters, Askharamukha also attempts to implement various script/language-specific orthographic conventions (where known) such as vowel lengths, gemination and nasalization. It also provides several customization options to fine-tune and get the desired orthography.
 
-Aksharamukha as of now supports 120 scripts and 21 romanization methods. The scripts supported are:
-
-*Ahom, Arabic, Ariyaka, Assamese, Avestan, Balinese, Batak Karo, Batak Mandailing, Batak Pakpak, Batak Simalungun, Batak Toba, Bengali (Bangla), Bhaiksuki, Brahmi, Buginese (Lontara), Buhid, Burmese (Myanmar), Chakma, Cham, Cyrillic (Russian), Devanagari, Dogra, Elymaic, Ethiopic (Abjad), Gondi (Gunjala), Gondi (Masaram), Grantha, Grantha (Pandya), Gujarati, Hanunoo, Hatran, Hebrew, Hebrew (Judeo-Arabic), Imperial Aramaic, Inscriptional Pahlavi, Inscriptional Parthian, Japanese (Hiragana), Japanese (Katakana), Javanese, Kaithi, Kannada, Kawi, Khamti Shan, Kharoshthi, Khmer (Cambodian), Khojki, Khom Thai, Khudawadi, Lao, Lao (Pali), Lepcha, Limbu, Mahajani, Makasar, Malayalam, Manichaean, Marchen, Meetei Mayek (Manipuri), Modi, Mon, Mongolian (Ali Gali), Mro, Multani, Nabataean, Nandinagari, Newa (Nepal Bhasa), Old North Arabian, Old Persian, Old Sogdian, Old South Arabian, Oriya (Odia), Pallava, Palmyrene, Persian, PhagsPa, Phoenician, Psalter Pahlavi, Punjabi (Gurmukhi), Ranjana (Lantsa), Rejang, Rohingya (Hanifi), Roman (IPA Indic), Samaritan, Santali (Ol Chiki), Saurashtra, Shahmukhi, Shan, Sharada, Siddham, Sinhala, Sogdian, Sora Sompeng, Soyombo, Sundanese, Syloti Nagari, Syriac (Eastern), Syriac (Estrangela), Syriac (Western), Tagalog, Tagbanwa, Tai Laing, Takri, Tamil, Tamil (Extended), Tamil Brahmi, Telugu, Thaana (Dhivehi), Thai, Tham (Lanna), Tham (Lao), Tham (Tai Khuen), Tham (Tai Lue), Tibetan, Tirhuta (Maithili), Ugaritic, Urdu, Vatteluttu, Wancho, Warang Citi, Zanabazar Square*
-
-The Indic Romanization Formats supported are: *Harvard-Kyoto, ITRANS, Velthuis, IAST, IAST (Pāḷi), ISO, ISO (Pāḷi), Titus, SLP1, WX, Roman (Readable), Roman (Colloquial)* . The Semitic Romanization Formats supported are: *Semitic (Aksharamukha), Semitic Typeable (Aksharamukha), ISO 259 Hebrew, SBL Hebrew, ISO 233 Arabic, DMG Persian*
-
 ## Usage and Examples
 
 Please use `pip aksharamukha` to install the Python package.
 
-Please find the usage instructions and relevant documentation [here](http://aksharamukha.appspot.com/#/python).
+Please find the usage instructions and relevant documentation [here](https://www.aksharamukha.com/python).
 
 ## Online Version
 
-The package as an online tool with a pretty web interface is available [here](http://aksharamukha.appspot.com/).
+The package as an online tool with a pretty web interface is available [here](https://www.aksharamukha.com).
 
 ## Contact
 
 If you have any questions please head to [Github](https://github.com/virtualvinodh/aksharamukha-python) or mail vinodh@virtualvinodh.com
+
+## Scripts Supported
+
+Aksharamukha as of now supports 120 scripts and 21 romanization methods. The scripts supported are:
+
+*Ahom, Arabic, Ariyaka, Assamese, Avestan, Balinese, Batak Karo, Batak Mandailing, Batak Pakpak, Batak Simalungun, Batak Toba, Bengali (Bangla), Bhaiksuki, Brahmi, Buginese (Lontara), Buhid, Burmese (Myanmar), Chakma, Cham, Cyrillic (Russian), Devanagari, Dogra, Elymaic, Ethiopic (Abjad), Gondi (Gunjala), Gondi (Masaram), Grantha, Grantha (Pandya), Gujarati, Hanunoo, Hatran, Hebrew, Hebrew (Judeo-Arabic), Imperial Aramaic, Inscriptional Pahlavi, Inscriptional Parthian, Japanese (Hiragana), Japanese (Katakana), Javanese, Kaithi, Kannada, Kawi, Khamti Shan, Kharoshthi, Khmer (Cambodian), Khojki, Khom Thai, Khudawadi, Lao, Lao (Pali), Lepcha, Limbu, Mahajani, Makasar, Malayalam, Manichaean, Marchen, Meetei Mayek (Manipuri), Modi, Mon, Mongolian (Ali Gali), Mro, Multani, Nabataean, Nandinagari, Newa (Nepal Bhasa), Old North Arabian, Old Persian, Old Sogdian, Old South Arabian, Oriya (Odia), Pallava, Palmyrene, Persian, PhagsPa, Phoenician, Psalter Pahlavi, Punjabi (Gurmukhi), Ranjana (Lantsa), Rejang, Rohingya (Hanifi), Roman (IPA Indic), Samaritan, Santali (Ol Chiki), Saurashtra, Shahmukhi, Shan, Sharada, Siddham, Sinhala, Sogdian, Sora Sompeng, Soyombo, Sundanese, Syloti Nagari, Syriac (Eastern), Syriac (Estrangela), Syriac (Western), Tagalog, Tagbanwa, Tai Laing, Takri, Tamil, Tamil (Extended), Tamil Brahmi, Telugu, Thaana (Dhivehi), Thai, Tham (Lanna), Tham (Lao), Tham (Tai Khuen), Tham (Tai Lue), Tibetan, Tirhuta (Maithili), Ugaritic, Urdu, Vatteluttu, Wancho, Warang Citi, Zanabazar Square*
+
+The Indic Romanization Formats supported are: *Harvard-Kyoto, ITRANS, Velthuis, IAST, IAST (Pāḷi), ISO, ISO (Pāḷi), Titus, SLP1, WX, Roman (Readable), Roman (Colloquial)* . The Semitic Romanization Formats supported are: *Semitic (Aksharamukha), Semitic Typeable (Aksharamukha), ISO 259 Hebrew, SBL Hebrew, ISO 233 Arabic, DMG Persian*
```

### Comparing `aksharamukha-2.2.1/aksharamukha.egg-info/SOURCES.txt` & `aksharamukha-2.2.2/aksharamukha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.2.1/setup.py` & `aksharamukha-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
   name='aksharamukha',
 
   # Versions should comply with PEP440.  For a discussion on single-sourcing
   # the version across setup.py and the project code, see
   # https://packaging.python.org/en/latest/single_source_version.html
-  version='2.2.1',
+  version='2.2.2',
 
   description='Provides script conversion (a.k.a transliteration) between various scripts',
   long_description=long_description,
   long_description_content_type='text/markdown',
 
   # The project's main homepage.
   url='https://github.com/virtualvinodh/aksharamukha-python',
```

