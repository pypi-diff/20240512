# Comparing `tmp/nef_pipelines-0.1.65.tar.gz` & `tmp/nef_pipelines-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.65.tar", last modified: Tue Apr 16 21:04:30 2024, max compression
+gzip compressed data, was "nef_pipelines-0.1.66.tar", last modified: Sun May 12 21:20:29 2024, max compression
```

## Comparing `nef_pipelines-0.1.65.tar` & `nef_pipelines-0.1.66.tar`

### file list

```diff
@@ -1,492 +1,516 @@
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.920269 nef_pipelines-0.1.65/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.420654 nef_pipelines-0.1.65/.github/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.515072 nef_pipelines-0.1.65/.github/workflows/
--rw-r--r--   0 garyt      (501) staff       (20)     1114 2024-04-16 21:02:58.000000 nef_pipelines-0.1.65/.github/workflows/test.yml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.521632 nef_pipelines-0.1.65/.idea/
--rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.65/.idea/.gitignore
--rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.65/.idea/.name
--rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.65/.idea/NFC.iml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.524590 nef_pipelines-0.1.65/.idea/inspectionProfiles/
--rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.65/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.65/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.65/.idea/modules.xml
--rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.65/.idea/vcs.xml
--rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.65/.pre-commit-config.yaml
--rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.65/.readthedocs.yml
--rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.65/AUTHORS.md
--rw-r--r--   0 garyt      (501) staff       (20)     7309 2024-04-16 20:02:09.000000 nef_pipelines-0.1.65/CHANGELOG.md
--rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.65/CONTRIBUTING.md
--rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.65/LICENSE.txt
--rw-r--r--   0 garyt      (501) staff       (20)    10243 2024-04-16 21:04:30.919717 nef_pipelines-0.1.65/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)     8849 2024-04-09 13:03:05.000000 nef_pipelines-0.1.65/README.md
--rw-r--r--   0 garyt      (501) staff       (20)      807 2023-05-21 15:23:42.000000 nef_pipelines-0.1.65/TODO.md
--rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.65/pyproject.toml
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.535272 nef_pipelines-0.1.65/references/
--rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.65/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.65/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garyt      (501) staff       (20)  1036893 2024-04-07 10:46:02.000000 nef_pipelines-0.1.65/references/kosol idps molecules-18-10802.pdf
--rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.65/release_to_pypi.sh
--rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-16 20:32:22.000000 nef_pipelines-0.1.65/requirements.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1712 2024-04-16 21:04:30.922064 nef_pipelines-0.1.65/setup.cfg
--rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.65/setup.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.422501 nef_pipelines-0.1.65/src/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.549341 nef_pipelines-0.1.65/src/nef_pipelines/
--rw-r--r--   0 garyt      (501) staff       (20)        6 2024-04-09 11:38:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/VERSION
--rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.576765 nef_pipelines-0.1.65/src/nef_pipelines/data/
--rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/ambiguity_translations.json
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.760901 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/
--rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
--rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
--rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
--rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
--rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
--rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
--rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
--rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
--rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
--rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
--rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
--rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
--rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
--rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
--rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
--rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.65/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.784751 nef_pipelines-0.1.65/src/nef_pipelines/lib/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2848 2024-04-06 16:53:23.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    20383 2024-04-09 10:57:52.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    15480 2024-04-08 08:38:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    25699 2024-04-06 13:43:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     6334 2024-03-19 22:25:46.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    14093 2024-04-09 11:03:09.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-06 16:21:33.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garyt      (501) staff       (20)    10315 2024-03-04 21:14:19.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.833014 nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/chem_comp.py
--rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/io.py
--rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/object_iter.py
--rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/translator.py
--rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garyt      (501) staff       (20)    27949 2024-03-19 22:43:06.000000 nef_pipelines-0.1.65/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     5431 2024-03-04 22:07:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/main.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.836105 nef_pipelines-0.1.65/src/nef_pipelines/nef_app/
--rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.851159 nef_pipelines-0.1.65/src/nef_pipelines/tests/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.859279 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/__init__.py
--rwxr--r--   0 garyt      (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.864830 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garyt      (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_list.py
--rwxr--r--   0 garyt      (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garyt      (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.868381 nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.874635 nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
--rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.878402 nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.883731 nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)     3621 2024-04-07 09:20:05.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.885788 nef_pipelines-0.1.65/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.891781 nef_pipelines-0.1.65/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr--r--   0 garyt      (501) staff       (20)       13 2024-04-07 09:17:12.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
--rwxr--r--   0 garyt      (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr--r--   0 garyt      (501) staff       (20)     3405 2024-04-07 09:19:50.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.906776 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.914537 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_delete.py
--rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_filter.py
--rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_rename.py
--rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_tabulate.py
--rwxr--r--   0 garyt      (501) staff       (20)    17146 2023-06-04 15:49:53.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_unassign.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.949855 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.973111 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)     8824 2024-04-16 20:00:43.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/short_co.neff
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
--rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/sparky_all.out
--rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1425 2024-04-16 20:00:44.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     6221 2024-04-07 09:31:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.995597 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.062884 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr--r--   0 garyt      (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garyt      (501) staff       (20)      840 2024-03-04 21:16:11.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     4093 2024-02-10 20:35:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr--r--   0 garyt      (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:29.428430 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrstar/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.070682 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrstar/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
--rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.086560 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.143204 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     2742 2024-02-10 18:10:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr--r--   0 garyt      (501) staff       (20)     3881 2023-08-24 07:58:35.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     3847 2024-02-10 20:35:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr--r--   0 garyt      (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.172652 nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.182347 nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr--r--   0 garyt      (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.216421 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.237370 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    29541 2023-11-21 22:17:45.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
--rw-r--r--   0 garyt      (501) staff       (20)    19578 2023-11-21 22:17:45.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     4195 2023-11-21 22:06:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2395 2023-11-21 22:06:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
--rwxr--r--   0 garyt      (501) staff       (20)     2254 2023-11-21 22:06:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
--rwxr--r--   0 garyt      (501) staff       (20)      800 2023-11-21 22:06:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
--rwxr--r--   0 garyt      (501) staff       (20)     7860 2023-12-20 18:35:13.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
--rwxr--r--   0 garyt      (501) staff       (20)     4316 2023-12-20 18:23:05.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.239813 nef_pipelines-0.1.65/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7234 2024-04-08 08:37:44.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.242057 nef_pipelines-0.1.65/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.330326 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.372893 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garyt      (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     4314 2024-04-07 09:31:37.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.386785 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.429331 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
--rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
--rw-r--r--   0 garyt      (501) staff       (20)     5638 2023-11-05 11:38:38.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_export_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     1877 2023-11-01 22:08:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_import_order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)     5825 2023-12-08 21:08:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_import_restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3282 2023-12-07 10:10:58.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_secondary_structure.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.447720 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/header.nef
--rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_header.py
--rwxr--r--   0 garyt      (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garyt      (501) staff       (20)     7636 2024-04-06 13:42:48.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_test.py
--rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/test_util.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.453403 nef_pipelines-0.1.65/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.464991 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.473177 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
--rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_data/basic.seq
--rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
--rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
--rw-r--r--   0 garyt      (501) staff       (20)     3392 2024-04-07 09:31:44.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_import_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_import_shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     8984 2024-03-27 21:18:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.484717 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.532044 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garyt      (501) staff       (20)     8138 2023-10-30 22:33:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     6577 2023-10-30 08:28:29.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    11089 2023-07-12 13:14:21.000000 nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.583414 nef_pipelines-0.1.65/src/nef_pipelines/tools/
--rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.592288 nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-03-04 21:23:23.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.595816 nef_pipelines-0.1.65/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.615713 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garyt      (501) staff       (20)      738 2024-04-06 15:19:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garyt      (501) staff       (20)     8836 2024-04-16 20:56:19.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/filter.py
--rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-02-10 20:35:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garyt      (501) staff       (20)     8044 2024-04-09 11:39:47.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garyt      (501) staff       (20)    18444 2023-06-04 15:49:53.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/unassign.py
--rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.619737 nef_pipelines-0.1.65/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-06 16:50:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/peaks/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-04-06 15:34:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.624006 nef_pipelines-0.1.65/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garyt      (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    12051 2024-04-09 11:02:16.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.65/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.626713 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.627282 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.632887 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.634923 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.636744 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15420 2024-04-07 09:21:28.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.638015 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.641339 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.662232 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     6680 2024-04-06 13:44:59.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.663478 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garyt      (501) staff       (20)      964 2023-05-24 21:21:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.672312 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5929 2024-04-06 13:45:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garyt      (501) staff       (20)     4326 2024-04-06 13:45:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garyt      (501) staff       (20)      826 2024-04-06 13:45:32.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     6096 2024-04-16 20:00:45.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.677920 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11101 2024-04-06 16:52:09.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)    11631 2024-04-06 16:51:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.681033 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.689043 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2374 2023-12-20 20:02:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22750 2023-11-19 15:24:30.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.693121 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/
--rw-r--r--   0 garyt      (501) staff       (20)      682 2024-03-19 07:46:08.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.739756 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7952 2024-04-09 11:01:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/project.py
--rw-r--r--   0 garyt      (501) staff       (20)     5993 2024-03-19 07:42:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    24119 2024-03-15 17:31:35.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.746003 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.752373 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.759949 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    16945 2023-11-21 22:15:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2313 2024-02-10 20:35:20.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     5749 2023-12-20 19:52:03.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.761843 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.764680 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.768410 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rcsb/
--rw-r--r--   0 garyt      (501) staff       (20)      454 2023-11-19 15:40:56.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rcsb/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.775941 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rcsb/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     4829 2023-12-20 18:35:13.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)    34787 2023-12-20 18:35:13.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.780767 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.785239 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.786618 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.790358 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.795640 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.798218 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.805022 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     9018 2024-03-27 21:44:50.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.808432 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/
--rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.832003 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     8157 2023-12-07 22:13:01.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.844350 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     5134 2024-03-19 07:42:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
--rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/restraints.py
--rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
--rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/talos_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.846018 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.848693 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.852360 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/
--rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.859497 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/importers/
--rw-r--r--   0 garyt      (501) staff       (20)     2923 2024-03-27 21:18:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
--rw-r--r--   0 garyt      (501) staff       (20)     2852 2023-05-21 10:57:07.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
--rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.864962 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.868461 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.915458 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-04-16 21:04:30.917085 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/
--rw-r--r--   0 garyt      (501) staff       (20)    10243 2024-04-16 21:04:29.000000 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garyt      (501) staff       (20)    21093 2024-04-16 21:04:29.000000 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2024-04-16 21:04:29.000000 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garyt      (501) staff       (20)       48 2024-04-16 21:04:29.000000 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garyt      (501) staff       (20)      440 2024-04-16 21:04:29.000000 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garyt      (501) staff       (20)       19 2024-04-16 21:04:29.000000 nef_pipelines-0.1.65/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.65/tox.ini
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.622027 nef_pipelines-0.1.66/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.374513 nef_pipelines-0.1.66/.github/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.493815 nef_pipelines-0.1.66/.github/workflows/
+-rw-r--r--   0 garyt      (501) staff       (20)     1119 2024-04-18 20:49:16.000000 nef_pipelines-0.1.66/.github/workflows/test.yml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.501798 nef_pipelines-0.1.66/.idea/
+-rw-r--r--   0 garyt      (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.66/.idea/.gitignore
+-rw-r--r--   0 garyt      (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.66/.idea/.name
+-rw-r--r--   0 garyt      (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.66/.idea/NFC.iml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.504839 nef_pipelines-0.1.66/.idea/inspectionProfiles/
+-rw-r--r--   0 garyt      (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.66/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      229 2023-10-31 09:12:23.000000 nef_pipelines-0.1.66/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.66/.idea/modules.xml
+-rw-r--r--   0 garyt      (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.66/.idea/vcs.xml
+-rw-r--r--   0 garyt      (501) staff       (20)     1330 2024-02-09 22:26:45.000000 nef_pipelines-0.1.66/.pre-commit-config.yaml
+-rw-r--r--   0 garyt      (501) staff       (20)      490 2022-11-25 17:14:46.000000 nef_pipelines-0.1.66/.readthedocs.yml
+-rw-r--r--   0 garyt      (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.66/AUTHORS.md
+-rw-r--r--   0 garyt      (501) staff       (20)     9439 2024-05-12 21:16:12.000000 nef_pipelines-0.1.66/CHANGELOG.md
+-rw-r--r--   0 garyt      (501) staff       (20)      334 2024-05-07 13:30:02.000000 nef_pipelines-0.1.66/CITATION.cff
+-rw-r--r--   0 garyt      (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.66/CONTRIBUTING.md
+-rw-r--r--   0 garyt      (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.66/LICENSE.txt
+-rw-r--r--   0 garyt      (501) staff       (20)    10359 2024-05-12 21:20:29.620655 nef_pipelines-0.1.66/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)     8849 2024-04-09 13:03:05.000000 nef_pipelines-0.1.66/README.md
+-rw-r--r--   0 garyt      (501) staff       (20)      833 2024-04-18 08:20:22.000000 nef_pipelines-0.1.66/TODO.md
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.507061 nef_pipelines-0.1.66/docs/
+-rw-r--r--   0 garyt      (501) staff       (20)    15643 2024-05-01 22:05:57.000000 nef_pipelines-0.1.66/docs/design_overview.md
+-rw-r--r--   0 garyt      (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.66/pyproject.toml
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.515587 nef_pipelines-0.1.66/references/
+-rw-r--r--   0 garyt      (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.66/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garyt      (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.66/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garyt      (501) staff       (20)  1036893 2024-04-07 10:46:02.000000 nef_pipelines-0.1.66/references/kosol idps molecules-18-10802.pdf
+-rwxr--r--   0 garyt      (501) staff       (20)     1264 2024-03-19 22:32:32.000000 nef_pipelines-0.1.66/release_to_pypi.sh
+-rw-r--r--   0 garyt      (501) staff       (20)      458 2024-05-12 19:18:18.000000 nef_pipelines-0.1.66/requirements.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1794 2024-05-12 21:20:29.623088 nef_pipelines-0.1.66/setup.cfg
+-rw-r--r--   0 garyt      (501) staff       (20)      710 2022-11-25 17:14:46.000000 nef_pipelines-0.1.66/setup.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.376374 nef_pipelines-0.1.66/src/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.527528 nef_pipelines-0.1.66/src/nef_pipelines/
+-rw-r--r--   0 garyt      (501) staff       (20)        6 2024-04-09 11:38:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/VERSION
+-rw-r--r--   0 garyt      (501) staff       (20)      577 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.542635 nef_pipelines-0.1.66/src/nef_pipelines/data/
+-rw-r--r--   0 garyt      (501) staff       (20)    16381 2024-03-04 22:17:52.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/ambiguity_translations.json
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.730945 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/
+-rw-r--r--   0 garyt      (501) staff       (20)   108495 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104358 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   118386 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102566 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json
+-rw-r--r--   0 garyt      (501) staff       (20)   108304 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)    91086 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35009 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   109165 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   105025 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119258 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102439 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96862 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99315 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    35085 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    73745 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json
+-rw-r--r--   0 garyt      (501) staff       (20)   151265 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json
+-rw-r--r--   0 garyt      (501) staff       (20)   102950 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)    96313 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    99814 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104993 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json
+-rw-r--r--   0 garyt      (501) staff       (20)   110515 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json
+-rw-r--r--   0 garyt      (501) staff       (20)    67204 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127933 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json
+-rw-r--r--   0 garyt      (501) staff       (20)   119775 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113627 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   150013 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   103831 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   112702 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89442 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)    89294 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json
+-rw-r--r--   0 garyt      (501) staff       (20)   113274 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json
+-rw-r--r--   0 garyt      (501) staff       (20)   133081 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json
+-rw-r--r--   0 garyt      (501) staff       (20)   127888 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)   104088 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    39789 2023-12-21 14:29:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json
+-rw-r--r--   0 garyt      (501) staff       (20)    18808 2024-03-04 22:17:52.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json
+-rw-r--r--   0 garyt      (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.66/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.760211 nef_pipelines-0.1.66/src/nef_pipelines/lib/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      124 2024-04-24 21:11:55.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1297 2024-02-10 20:21:35.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1128 2024-03-05 09:00:53.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2848 2024-04-06 16:53:23.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20551 2024-04-24 21:37:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15480 2024-05-01 19:23:42.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    26343 2024-05-04 20:19:37.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6451 2024-05-12 19:28:35.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14141 2024-04-24 21:12:53.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9169 2024-04-06 16:21:33.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11906 2024-04-18 08:17:45.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.770863 nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    33455 2024-03-04 22:01:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/chem_comp.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20016 2024-03-04 22:01:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/io.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4325 2024-03-04 22:00:30.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/object_iter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2494 2023-12-21 14:29:03.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/translator.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garyt      (501) staff       (20)    27862 2024-05-07 17:44:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     5594 2024-05-12 19:18:26.000000 nef_pipelines-0.1.66/src/nef_pipelines/main.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.772317 nef_pipelines-0.1.66/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garyt      (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.783160 nef_pipelines-0.1.66/src/nef_pipelines/tests/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.790725 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     5010 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.815072 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr-xr-x   0 garyt      (501) staff       (20)      473 2024-04-18 08:20:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)    10043 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10231 2024-03-04 21:31:42.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garyt      (501) staff       (20)      192 2024-04-18 08:18:10.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.818966 nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.842744 nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)       41 2024-02-10 20:33:34.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)      213 2024-02-10 20:33:03.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rwxr-xr-x   0 garyt      (501) staff       (20)      310 2024-02-10 20:33:03.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
+-rw-r--r--   0 garyt      (501) staff       (20)     3065 2024-03-19 18:41:13.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5018 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.844398 nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.846611 nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     3625 2024-04-18 08:20:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.851200 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-04-24 21:08:34.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.862501 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rw-r--r--   0 garyt      (501) staff       (20)      582 2024-04-24 21:14:16.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/3aa.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      708 2024-04-24 21:14:16.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/3aa_2_chains.nef
+-rwxr--r--   0 garyt      (501) staff       (20)       44 2024-05-03 08:09:10.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/3aa_header.fasta
+-rwxr--r--   0 garyt      (501) staff       (20)       13 2024-04-07 09:17:12.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
+-rw-r--r--   0 garyt      (501) staff       (20)      588 2024-04-24 21:14:16.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/3aa_thx.nef
+-rwxr--r--   0 garyt      (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rw-r--r--   0 garyt      (501) staff       (20)     1141 2024-05-04 17:47:19.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_export_sequence.py
+-rwxr--r--   0 garyt      (501) staff       (20)     4296 2024-05-04 17:49:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_import_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.873329 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.877229 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     5990 2023-06-03 15:00:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2560 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)      251 2023-12-20 20:04:53.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_filter.py
+-rwxr--r--   0 garyt      (501) staff       (20)     1964 2023-12-13 22:30:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr--r--   0 garyt      (501) staff       (20)     6921 2023-12-20 16:23:42.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_tabulate.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)    17207 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_unassign.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.893513 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.924807 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     8824 2024-04-16 20:00:43.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/short_co.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-23 20:39:35.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/sparky_CA-1.out
+-rw-r--r--   0 garyt      (501) staff       (20)      240 2023-05-24 21:21:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/sparky_CA.out
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-24 21:21:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/sparky_all.out
+-rw-r--r--   0 garyt      (501) staff       (20)     3331 2023-05-24 21:21:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1386 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6225 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.934735 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.978033 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garyt      (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr--r--   0 garyt      (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr--r--   0 garyt      (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr-xr-x   0 garyt      (501) staff       (20)    25195 2024-02-10 20:33:03.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)      233 2024-02-10 20:33:03.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)      814 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garyt      (501) staff       (20)      504 2023-09-13 11:17:50.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4097 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4458 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.979183 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrstar/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:50:48.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrstar/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.984269 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrstar/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)   235686 2024-03-04 22:09:35.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
+-rw-r--r--   0 garyt      (501) staff       (20)   193009 2024-03-04 22:09:35.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:28.998363 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garyt      (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garyt      (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.040897 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     1291 2023-08-23 12:07:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garyt      (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garyt      (501) staff       (20)     2172 2023-08-24 07:47:26.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garyt      (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garyt      (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garyt      (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garyt      (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garyt      (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2578 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2535 2024-04-18 08:22:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     3819 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     3851 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4675 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr--r--   0 garyt      (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.044614 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:51:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.050819 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garyt      (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2689 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     2013 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.091463 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.112440 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)    29541 2023-11-21 22:17:45.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif
+-rw-r--r--   0 garyt      (501) staff       (20)    19578 2023-11-21 22:17:45.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4795 2023-11-21 22:06:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     4195 2023-11-21 22:06:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     2395 2023-11-21 22:06:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)     2254 2023-11-21 22:06:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
+-rwxr--r--   0 garyt      (501) staff       (20)      800 2023-11-21 22:06:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4616 2024-04-18 08:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     4320 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.117999 nef_pipelines-0.1.66/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      743 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.125062 nef_pipelines-0.1.66/src/nef_pipelines/tests/simulate/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/simulate/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7057 2024-05-01 22:01:47.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/simulate/test_simulate_peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.139166 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.174151 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garyt      (501) staff       (20)      241 2023-04-26 21:06:26.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garyt      (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garyt      (501) staff       (20)    12668 2024-04-28 20:42:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4198 2024-04-18 08:20:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2665 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2370 2023-05-24 21:14:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.180537 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-28 09:23:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.200691 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)     2865 2024-02-10 20:30:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      314 2023-11-01 22:08:23.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/predS2_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/predSS_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)      817 2023-11-01 22:07:56.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1835 2023-09-13 21:31:11.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1200 2023-09-15 21:17:38.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-09-13 21:31:11.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1324 2023-11-01 22:00:48.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2870 2024-02-10 20:31:11.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/protonated_his.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/ubi_4.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2858 2024-02-10 20:30:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     5589 2024-04-28 19:39:11.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_export_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1889 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_import_order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5829 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_import_restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3306 2024-04-28 19:38:49.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_secondary_structure.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.244897 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garyt      (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/header.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1643 2024-05-06 16:49:31.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/multi.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr--r--   0 garyt      (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garyt      (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     2892 2024-02-10 20:30:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr--r--   0 garyt      (501) staff       (20)    64721 2024-03-19 22:16:54.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garyt      (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     9436 2024-04-18 18:18:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_nef_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9402 2024-05-07 20:03:52.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_save.py
+-rwxr-xr-x   0 garyt      (501) staff       (20)     7766 2024-05-04 20:18:45.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_test.py
+-rw-r--r--   0 garyt      (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/test_util.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.247583 nef_pipelines-0.1.66/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-05-04 17:51:14.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xcamshift/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1830 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.254888 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.261874 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+-rw-r--r--   0 garyt      (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_data/basic.seq
+-rw-r--r--   0 garyt      (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
+-rw-r--r--   0 garyt      (501) staff       (20)      232 2024-03-27 22:29:35.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
+-rw-r--r--   0 garyt      (501) staff       (20)     3396 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_import_peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1555 2024-04-18 08:20:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_import_shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9051 2024-04-28 20:42:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.273819 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-04-24 21:08:15.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.316126 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garyt      (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garyt      (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garyt      (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garyt      (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garyt      (501) staff       (20)     8230 2024-04-28 19:36:48.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6669 2024-04-28 19:35:07.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1987 2024-04-28 19:32:11.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1465 2024-04-18 08:18:10.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3298 2024-04-18 08:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11180 2024-04-28 19:29:44.000000 nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.329670 nef_pipelines-0.1.66/src/nef_pipelines/tools/
+-rw-r--r--   0 garyt      (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.338337 nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garyt      (501) staff       (20)      527 2023-01-02 20:40:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2614 2024-05-04 20:18:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1466 2024-02-10 20:35:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2670 2024-04-21 14:47:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9215 2024-04-21 14:47:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.364940 nef_pipelines-0.1.66/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garyt      (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.368562 nef_pipelines-0.1.66/src/nef_pipelines/tools/fit/
+-rw-r--r--   0 garyt      (501) staff       (20)      349 2024-05-12 19:22:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/fit/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4002 2024-05-12 19:23:16.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/fit/exponential.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.382005 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garyt      (501) staff       (20)      738 2024-04-06 15:19:54.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2556 2023-05-21 15:19:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8836 2024-04-16 20:56:19.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/filter.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4100 2023-12-20 19:42:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7617 2024-04-21 14:47:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8044 2024-04-09 11:39:47.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garyt      (501) staff       (20)    19382 2023-12-20 16:24:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garyt      (501) staff       (20)    18446 2024-04-21 14:59:55.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/unassign.py
+-rw-r--r--   0 garyt      (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.386011 nef_pipelines-0.1.66/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garyt      (501) staff       (20)      366 2024-04-06 16:50:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/peaks/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10891 2024-04-06 15:34:54.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garyt      (501) staff       (20)    10539 2023-11-19 15:24:30.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/res_assign.py_unused
+-rw-r--r--   0 garyt      (501) staff       (20)     8829 2024-05-07 20:12:18.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/save.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.390185 nef_pipelines-0.1.66/src/nef_pipelines/tools/series/
+-rw-r--r--   0 garyt      (501) staff       (20)      356 2024-05-12 19:20:54.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/series/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    20047 2024-05-12 19:20:55.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/series/build.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.394538 nef_pipelines-0.1.66/src/nef_pipelines/tools/simulate/
+-rw-r--r--   0 garyt      (501) staff       (20)      393 2024-05-01 21:57:12.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/simulate/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    13608 2024-05-01 21:56:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/simulate/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    26443 2024-05-01 21:52:50.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/simulate/unlabelling.py
+-rw-r--r--   0 garyt      (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garyt      (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.66/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.396857 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.397784 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garyt      (501) staff       (20)      480 2023-05-28 10:49:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.404730 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16493 2023-11-19 15:24:30.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)    14955 2024-03-27 21:45:12.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.406081 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garyt      (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.408668 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15420 2024-04-07 09:21:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.428034 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garyt      (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.430026 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4514 2024-05-03 07:54:44.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.432869 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11238 2024-05-04 20:17:59.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.434656 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garyt      (501) staff       (20)     1071 2024-05-01 17:55:31.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.442047 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5929 2024-04-06 13:45:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4326 2024-04-06 13:45:32.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2942 2024-05-01 17:53:56.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6096 2024-04-16 20:00:45.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.447942 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11101 2024-04-06 16:52:09.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2156 2024-05-01 17:55:07.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    12049 2024-05-04 20:18:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.452211 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garyt      (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.457668 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2374 2023-12-20 20:02:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3781 2023-09-13 21:22:39.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2884 2023-10-30 22:24:14.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22750 2023-11-19 15:24:30.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.460407 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/
+-rw-r--r--   0 garyt      (501) staff       (20)      682 2024-05-12 21:19:14.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.466052 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2024-03-04 22:03:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9591 2024-05-04 20:34:08.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/project.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6039 2024-05-04 20:21:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    24793 2024-05-04 20:17:59.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)      225 2024-03-19 07:46:07.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/nmrstar_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.470145 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garyt      (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.474567 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7302 2024-02-10 18:10:55.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9136 2024-03-27 21:50:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.479921 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16845 2024-04-17 08:40:33.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2359 2024-05-04 20:18:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5808 2024-05-04 20:18:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.481611 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garyt      (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.504719 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)    10943 2023-11-21 22:15:33.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garyt      (501) staff       (20)     4817 2023-11-21 22:16:36.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.509253 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rcsb/
+-rw-r--r--   0 garyt      (501) staff       (20)      454 2023-11-19 15:40:56.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rcsb/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.511092 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rcsb/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     4875 2024-04-28 20:42:25.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rcsb/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)    34787 2023-12-20 18:35:13.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.512613 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garyt      (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.515182 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    11873 2024-03-27 21:50:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.517140 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garyt      (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.519518 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9023 2024-03-27 22:18:33.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.523033 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garyt      (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.525624 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-03-18 23:32:17.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)    15801 2024-02-10 22:15:24.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.544097 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8116 2024-03-04 21:43:45.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     6470 2024-05-04 20:18:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     9064 2024-05-04 20:18:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    17455 2024-03-27 21:18:54.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.565744 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/
+-rw-r--r--   0 garyt      (501) staff       (20)      976 2023-10-31 09:11:23.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.568775 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8155 2024-04-18 19:39:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.575560 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-08-24 19:19:17.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     5150 2024-04-24 21:15:48.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/order_parameters.py
+-rw-r--r--   0 garyt      (501) staff       (20)    16249 2024-03-27 21:50:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/restraints.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3747 2024-03-19 07:42:55.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1834 2024-03-19 07:42:55.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     8576 2024-03-27 21:50:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/talos_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.576770 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garyt      (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.578821 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.600387 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garyt      (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.604609 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)     2950 2024-04-28 19:38:31.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-04-28 19:42:01.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     1865 2024-03-27 21:44:26.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
+-rw-r--r--   0 garyt      (501) staff       (20)    22539 2023-11-19 15:23:28.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.608663 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garyt      (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.611128 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     7167 2023-11-21 22:15:00.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.616896 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garyt      (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2834 2024-03-27 21:18:54.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garyt      (501) staff       (20)     2895 2024-03-27 21:50:51.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garyt      (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garyt      (501) staff       (20)    39703 2023-10-30 22:21:37.000000 nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garyt      (501) staff       (20)        0 2024-05-12 21:20:29.618403 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garyt      (501) staff       (20)    10359 2024-05-12 21:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garyt      (501) staff       (20)    22012 2024-05-12 21:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2024-05-12 21:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       48 2024-05-12 21:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garyt      (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garyt      (501) staff       (20)      532 2024-05-12 21:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garyt      (501) staff       (20)       19 2024-05-12 21:20:28.000000 nef_pipelines-0.1.66/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garyt      (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.66/tox.ini
```

### Comparing `nef_pipelines-0.1.65/.github/workflows/test.yml` & `nef_pipelines-0.1.66/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 permissions:
   contents: read
 
 jobs:
   build:
     strategy:
       matrix:
-        python-version: [ "3.9", "3.10", "3.11"] #, "3.12" ]
+        python-version: [ "3.8" , "3.9", "3.10", "3.11", "3.12" ]
         os: [ubuntu-latest, macos-latest] #windows-latest]
 
     runs-on: ${{ matrix.os }}
     steps:
 #      - name: Support longpaths
 #        run: git config --system core.longpaths true
```

### Comparing `nef_pipelines-0.1.65/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.66/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/.pre-commit-config.yaml` & `nef_pipelines-0.1.66/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/CHANGELOG.md` & `nef_pipelines-0.1.66/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -267,7 +267,40 @@
 - remove dependance on Levenshtein which was causing compilation errors
 
 ## version 0.1.64
 - update to fyeah to try to make windows installation work
 
 ## version 0.1.65
 - fixed a bug in export of CO shifts reported by Pete Simpson
+
+## version 0.1.66
+
+Major release with many new features and bug fixes
+
+- Relaxation
+  - Added initial support for fitting [using [Streamfitter](https://github.com/varioustoxins/Streamfitter)] this uses the NEF provisional data series format  [command: series build]
+  - Added a tool to build a NEF [provisional] data series format from spectra [aka peak lists] [command: series build]
+
+- Multi file streams
+  - Added the ability to save a series of NEF files from a multi entry stream [command save]
+  - Added the ability to stream multiple NEF files from BMRB entries [command nmrstar project]
+
+- Documentation & Project
+  - NEF-Pipelines has a citation record
+  - Add an initial version of design doc for NEF-Pipelines describing the internals of the pipe commands within the pipeline
+  - The project is now automatically tested on python 3.9-3.12 and Linux and MacOS as a matrix hsing GitHub Actions
+
+- MARS and Fasta
+  - Fasta output and input to NEF-Pipelines supports round tripping of chain ids [chain_codes] and chain starts via a custom header
+  - Mars has a command to read in a sequence from its Fasta file [including round tripping if written by NEF-Pipelines]  [command mars import sequence]
+  - Better support of a variety of Fasta headers (including PDB/RCSB headers)
+  - Fasta input and output the entry_id of the NEF stream is saved as the entry name of the fasta file
+  - Mars sequence exports has better error handling [command: mars export sequence]
+  - Fasta has improvement to the sequence handling [molecule type per sequence] and provides a python pipe command
+
+- Simulations
+  - The command `simulate peaks` replaces the command `shifts make_peaks` [mostly a rename]
+  - Types of spectra are now arguments to `simulate peaks` not options and the command has better error messages and case-insensitive matching of spectra names [where possible]
+  - Simulation of unlabelling spectra added [command: simulate unlabelling]
+
+- NMRStar and the BMRB
+  - Add the ability to read BMRB sequences, shifts and projects [currently shifts and sequences] [commands: nmrstar import sequences and nmrstar import shifts]
```

### Comparing `nef_pipelines-0.1.65/CONTRIBUTING.md` & `nef_pipelines-0.1.66/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/LICENSE.txt` & `nef_pipelines-0.1.66/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/PKG-INFO` & `nef_pipelines-0.1.66/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.65
+Version: 0.1.66
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -12,15 +12,16 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: click==8.1.3
-Requires-Dist: f-yeah==0.4.0
+Requires-Dist: f-yeah==0.3.0; python_version < "3.12"
+Requires-Dist: f-yeah==0.4.0; python_version >= "3.12"
 Requires-Dist: fastaparser==1.1.1
 Requires-Dist: freezegun==1.1.0
 Requires-Dist: frozendict==2.3.7
 Requires-Dist: hjson==3.1.0
 Requires-Dist: mmcif-pdbx==2.0.1
 Requires-Dist: ordered-set==4.1.0
 Requires-Dist: pydantic==2.6.3
@@ -28,14 +29,15 @@
 Requires-Dist: pyparsing==3.0.8
 Requires-Dist: pytest==7.1.3
 Requires-Dist: pytest-mock==3.12.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: StrEnum==0.4.8
 Requires-Dist: tabulate==0.8.9
 Requires-Dist: typer==0.7.0
+Requires-Dist: uncertainties==3.1.7
 Requires-Dist: urllib3==1.26.15
 Requires-Dist: wcmatch==8.5
 Requires-Dist: xmltodict==0.13.0
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
```

### Comparing `nef_pipelines-0.1.65/README.md` & `nef_pipelines-0.1.66/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/TODO.md` & `nef_pipelines-0.1.66/TODO.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,7 +21,8 @@
 * Missing tests -done
 * mars - nef2mars - done
 * renumber chains -  done
 * test hannah's problems - done
 * Fasta export - done
 * xEasy shifts - done
 release - done
+test_filter not committed
```

### Comparing `nef_pipelines-0.1.65/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.66/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.66/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/references/kosol idps molecules-18-10802.pdf` & `nef_pipelines-0.1.66/references/kosol idps molecules-18-10802.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/release_to_pypi.sh` & `nef_pipelines-0.1.66/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/setup.cfg` & `nef_pipelines-0.1.66/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	annotated-types==0.6.0
 	cachetools==5.3.3
 	click==8.1.3
-	f-yeah==0.4.0
+	f-yeah==0.3.0;python_version<'3.12'
+	f-yeah==0.4.0;python_version>='3.12'
 	fastaparser==1.1.1
 	freezegun==1.1.0
 	frozendict==2.3.7
 	hjson==3.1.0
 	mmcif-pdbx==2.0.1
 	ordered-set==4.1.0
 	pydantic==2.6.3
@@ -38,14 +39,15 @@
 	pyparsing==3.0.8
 	pytest==7.1.3
 	pytest-mock==3.12.0
 	requests==2.31.0
 	StrEnum==0.4.8
 	tabulate==0.8.9
 	typer==0.7.0
+	uncertainties==3.1.7
 	urllib3==1.26.15
 	wcmatch==8.5
 	xmltodict==0.13.0
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `nef_pipelines-0.1.65/setup.py` & `nef_pipelines-0.1.66/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/ambiguity_translations.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/ambiguity_translations.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+A+msd_ccpnRef_2007-12-11-10-13-15_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+C+msd_ccpnRef_2007-12-11-10-13-16_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+G+msd_ccpnRef_2007-12-11-10-13-16_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+I+msd_ccpnRef_2007-12-11-10-13-17_00002.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+T+msd_ccpnRef_2007-12-11-10-13-17_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+U+msd_ccpnRef_2007-12-11-10-13-17_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/DNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-969_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+A+msd_ccpnRef_2007-12-11-10-13-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+C+msd_ccpnRef_2007-12-11-10-13-18_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+G+msd_ccpnRef_2007-12-11-10-13-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+I+msd_ccpnRef_2007-12-11-10-13-19_00004.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+T+msd_ccpnRef_2007-12-11-10-13-19_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+U+msd_ccpnRef_2007-12-11-10-13-20_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/RNA+Xxx+pdbe_ccpnRef_2009-07-30-11-31-15-197_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Ala+msd_ccpnRef_2007-12-11-10-20-09_00022.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Arg+msd_ccpnRef_2007-12-11-10-20-10_00007.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Asn+msd_ccpnRef_2007-12-11-10-20-10_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Asp+msd_ccpnRef_2007-12-11-10-20-10_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Cys+msd_ccpnRef_2007-12-11-10-20-13_00005.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Gln+msd_ccpnRef_2007-12-11-10-20-15_00017.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Glu+msd_ccpnRef_2007-12-11-10-20-15_00018.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Gly+msd_ccpnRef_2007-12-11-10-20-15_00019.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+His+msd_ccpnRef_2007-12-11-10-20-16_00013.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Ile+msd_ccpnRef_2007-12-11-10-20-17_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Leu+msd_ccpnRef_2007-12-11-10-20-17_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Lys+msd_ccpnRef_2007-12-11-10-20-18_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Met+msd_ccpnRef_2007-12-11-10-20-19_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Phe+msd_ccpnRef_2007-12-11-10-20-22_00003.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Pro+msd_ccpnRef_2007-12-11-10-20-22_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Ser+msd_ccpnRef_2007-12-11-10-20-23_00016.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Thr+msd_ccpnRef_2007-12-11-10-20-24_00014.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Trp+msd_ccpnRef_2007-12-11-10-20-25_00008.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Tyr+msd_ccpnRef_2007-12-11-10-20-26_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Val+msd_ccpnRef_2007-12-11-10-20-27_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/chem_comp/protein+Xxx+pdbe_ccpnRef_2009-07-30-11-31-14-656_00001.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json` & `nef_pipelines-0.1.66/src/nef_pipelines/data/default_atom_sets_by_comp_and_linking.json`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.66/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/nef_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     get_version,
     is_float,
     is_int,
     running_in_pycharm,
     script_name,
 )
 
+NEF_PIPELINES_PREFIX = "nefpls"
+
 DEFAULT_INCREMENT_SEPARATOR = "::"
 DEFAULT_INCREMENT_END = ""
 
 NEF_TRUE = "true"
 NEF_FALSE = "false"
 NEF_NONE = "none"
 
@@ -346,26 +348,32 @@
     """
     for row in loop_row_dict_iter(loop, convert=convert):
         yield Namespace(**row)
 
 
 # TODO this partially overlaps with select_frames_by_name in this file, combine and simplify!
 def select_frames(
-    entry: Entry, selector_type: SelectionType, filters: List[str]
+    entry: Entry,
+    filters: Union[str, List[str]],
+    selector_type: SelectionType = SelectionType.ANY,
 ) -> List[Saveframe]:
     """
     select a list of frames by name of either category or name
 
     :param entry: the entry in which frames are looked for
+    :param filters: a string or list of strings to use as filters as defined by fnmatch
     :param selector_type: the matching type frame.name or frame.category or both [default, search order
            frame.name frame.category]
-    :param filters: a list of strings to use as filters as defined by fnmatch
     :return: a list of selected saveframes
     """
 
+    if isinstance(filters, str):
+        filters = [
+            filters,
+        ]
     if not filters:
         filters = ["*"]
 
     star_filters = [f"*{filter}*" for filter in filters]
     filters = list(filters)
     filters.extend(star_filters)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/peak_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/sequence_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import string
 from collections import Counter
 from dataclasses import replace
 from enum import auto
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 from ordered_set import OrderedSet
 from pynmrstar import Entry, Loop, Saveframe
 from strenum import LowercaseStrEnum
 
 from nef_pipelines.lib.constants import NEF_UNKNOWN
 from nef_pipelines.lib.nef_lib import UNUSED, loop_row_namespace_iter
@@ -33,43 +33,63 @@
     CARBOH = auto()
 
 
 NEF_CHAIN_CODE = "chain_code"
 ANY_CHAIN = "_"
 
 
-def chain_code_iter(
+class ChainCodeIterable:
+
+    ASCII_UPPERCASE = list(string.ascii_uppercase)
+
+    def __init__(self, user_chain_codes: List[str], exclude: List[str] = ()):
+
+        self._index = 0
+        self._chain_codes = []
+
+        seen_codes = set()
+        self._chain_codes = []
+        for user_chain_code in user_chain_codes:
+            seen_codes.add(user_chain_code)
+            if user_chain_code not in exclude:
+                self._chain_codes.append(user_chain_code)
+
+        for chain_code in self.ASCII_UPPERCASE:
+            if chain_code not in seen_codes and chain_code not in exclude:
+                self._chain_codes.append(chain_code)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self._index < len(self._chain_codes):
+            result = self._chain_codes[self._index]
+            self._index += 1
+            return result
+        else:
+            raise StopIteration("run out of chain names!")
+
+
+def get_chain_code_iter(
     user_chain_codes: List[str] = "", exclude: List[str] = ()
-) -> Iterable[str]:
+) -> Iterator[str]:
     """
-    Yield chain codes in user chain codes and once exhausted yield any remaining letters of the upper case alphabet
+    return an iterator thay will yield chain codes in user chain codes and
+    once exhausted yield any remaining letters of the upper case alphabet
     till they run out. A list of chain codes to not use can be provided...
 
     Args:
         user_chain_codes (str):  string of dot separated chain codes or a list of chain codes
         exclude: chain codes to not include in the iteration
 
     Returns:
         Iterable[str] single codes
     """
 
-    ascii_uppercase = list(string.ascii_uppercase)
-
-    seen_codes = set()
-
-    for chain_code in user_chain_codes:
-        seen_codes.add(chain_code)
-        if chain_code not in exclude:
-            yield chain_code
-
-    for chain_code in ascii_uppercase:
-        if chain_code not in seen_codes and chain_code not in exclude:
-            yield chain_code
-
-    raise ValueError("run out of chain names!")
+    return ChainCodeIterable(user_chain_codes, exclude).__iter__()
 
 
 def get_linking(
     target_sequence: List[SequenceResidue],
     no_chain_start=List[str],
     no_chain_end=List[str],
 ) -> List[SequenceResidue]:
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/shift_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import dataclasses
+from enum import auto
 from typing import Dict, List
 
 from pynmrstar import Loop, Saveframe
+from strenum import StrEnum
 
 from nef_pipelines.lib.nef_lib import UNUSED, loop_row_namespace_iter
 from nef_pipelines.lib.structures import (
     AtomLabel,
     Residue,
     SequenceResidue,
     ShiftData,
     ShiftList,
 )
 
 NEF_CHEMICAL_SHIFT_LOOP = "nef_chemical_shift"
 
 
+class DataType(StrEnum):
+    HEIGHT = auto()
+    VOLUME = auto()
+
+
 def nef_frames_to_shifts(frames: List[Saveframe]) -> List[ShiftData]:
     """
 
     :param frames:
     :return:
     """
     shifts = []
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/spectra_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from enum import Enum, auto
 from typing import Dict, Tuple, Union
 
 from strenum import StrEnum
 
 from nef_pipelines.lib.isotope_lib import Isotope
 
+FAKE_SPECTROMETER_FREQUENCY_600 = 600.12345678
+
 
 class NMRMassClass(Enum):
     IDP = auto()
     LOW = auto()
     HIGH = auto()
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/test_lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,64 @@
 import sys
 import traceback
 from fnmatch import fnmatch
 from io import StringIO
 from itertools import zip_longest
 from pathlib import Path
-from typing import IO, AnyStr, List, Optional
+from typing import IO, AnyStr, List, Optional, Tuple
 
 from click.testing import Result
 from pynmrstar import Entry
 from typer import Typer
 from typer.testing import CliRunner
 
 NOQA_E501 = "# noqa: E501"
 
 
-def run_and_read_pytest(args):
-
+def read_test_data(file_path: str, root_directory: Optional[str] = None) -> str:
+    """
+    Reads the content of a test data file from standard locations.
+
+    This function reads the content of a test data file located at the given file path.
+    If a root directory is provided, the function will consider the file path to be relative to this directory
+    using the function path_in_test_data for lookup.
+
+    Args:
+        file_path (str): The path to the test data file.
+        root_directory (Optional[str], optional): The root directory from which the file path is considered to be
+                                                  relative.
+                                                  If None, the file path is considered to be absolute.
+
+    Returns:
+        str: The content of the test data file.
+    """
+
+    file_path = (
+        path_in_test_data(root_directory, file_path) if root_directory else file_path
+    )
+    with open(file_path) as sequence_stream:
+        sequence_stream = sequence_stream.read()
+    return sequence_stream
+
+
+def run_and_read_pytest(args: List[str]) -> Tuple[int, str, str]:
+    """
+    Runs pytest with the provided arguments and captures the output.
+
+    This function runs pytest with the given arguments and captures the return code,
+    standard output, and standard error output. It temporarily redirects sys.stdout
+    and sys.stderr to capture the output.
+
+    Args:
+        args (List[str]): The arguments to pass to pytest.
+
+    Returns:
+        Tuple[int, str, str]: the return code, standard output,
+        and standard error output from pytest.
+    """
     from pytest import main
 
     original_output = sys.stdout
     original_error = sys.stdout
     sys.stdout = StringIO()
     sys.stderr = StringIO()
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/chem_comp.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/chem_comp.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/io.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/io.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/object_iter.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/object_iter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/translation/translator.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/translation/translator.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/translation_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/translation_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.66/src/nef_pipelines/lib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 from nef_pipelines.lib.header_lib import (
     create_header_frame,
     get_creation_time,
     get_uuid,
 )
 from nef_pipelines.lib.structures import LineInfo
 
+UNKNOWN_INPUT_SOURCE = "unknown"
+
 FOUR_SPACES = " " * 4
 
 STDIN = Path("-")
 STDOUT = Path("-")
 
 
 def _get_loop_by_category_or_none(frame: Saveframe, category: str) -> Loop:
@@ -222,15 +224,16 @@
 
     if file_name == Path("-") or not file_name:
         if sys.stdin.isatty():
             exit_error("attempting to read from a terminal")
         result = sys.stdin.read()
     else:
         try:
-            result = open(file_name).read()
+            with open(file_name) as fh:
+                result = fh.read()
         except IOError as e:
             exit_error(f"couldn't read from {file_name} because of an error", e)
 
     return result
 
 
 def get_pipe_file(args: Namespace) -> Optional[TextIO]:
@@ -340,43 +343,44 @@
         command = current_context.command_path.split()[1:]
 
     command = f"{'/'.join(command)}.py"
 
     return command
 
 
-def read_from_file_or_exit(file_name: Path, target: str = "unknown") -> str:
-    if file_name == STDIN and sys.stdin.isatty():
-        msg = f"""
-            while tring to read from {file_name} as {target} i expected to read from stdin,
-            howveer the inputs  is not a stream [did you forget to add a nef file to your pipeline?]
+def read_from_file_or_exit(file_path: Path, target: str = UNKNOWN_INPUT_SOURCE) -> str:
+
+    if file_path == STDIN and sys.stdin.isatty():
+
+        msg = """
+            while trying to read from STDIN [-] the input is not a stream
+            [did you forget to add a nef file to your pipeline?]
         """
         exit_error(msg)
-    if running_in_pycharm():
-        exit_error(
-            "reading from stdin doesn't work in pycharm debug environment as there is no shell..."
-        )
 
-    display_file_name = get_display_file_name(file_name)
+    display_file_name = get_display_file_name(file_path)
 
     fh = sys.stdin
 
-    if not file_name == STDIN:
+    if not file_path == STDIN:
         try:
-            fh = open(file_name)
+            fh = open(file_path)
         except Exception as e:
             msg = f"couldn't open {display_file_name} to read {target}"
             exit_error(msg, e)
 
     try:
         text = fh.read()
     except Exception as e:
         msg = f"couldn't read {target} from {display_file_name}"
         exit_error(msg, e)
 
+    if file_path != STDIN:
+        fh.close()
+
     return text
 
 
 def _script_to_command(script: str) -> str:
     """
     turns a script path into the equivalent nef pipelines command
     :param script: the script path
@@ -657,15 +661,15 @@
 
 
 @contextlib.contextmanager
 def smart_open(filename=None, stream_type=StdStream.STDOUT):
     f"""
     context manager to open a file or use stdout depending on the filename, stdin is defined as '-'
     by corollary a std stream won't be closed on exit only file system streams
-    :param filename: the filename to use '-' indicates a standar stream selected by stream_type
+    :param filename: the filename to use '-' indicates a standard stream selected by stream_type
     :param stream_type: how to treat the stream choices are {', '.join(StdStream.__members__)}
 
     """
 
     mode = STREAM_MODES[stream_type]
     if filename and str(filename) != "-":
         fh = open(filename, mode)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/main.py` & `nef_pipelines-0.1.66/src/nef_pipelines/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,18 +75,22 @@
     warnings = []
     try:
         # import components which will self register, this could and will be automated
         modules = [
             "nef_pipelines.tools.about",
             "nef_pipelines.tools.chains",
             "nef_pipelines.tools.entry",
+            "nef_pipelines.tools.fit",
             "nef_pipelines.tools.frames",
             "nef_pipelines.tools.header",
             "nef_pipelines.tools.peaks",
-            "nef_pipelines.tools.shifts",
+            "nef_pipelines.tools.save",
+            "nef_pipelines.tools.series",
+            "nef_pipelines.tools.simulate",
+            "nef_pipelines.tools.sink",
             "nef_pipelines.tools.stream",
             "nef_pipelines.tools.test",
             "nef_pipelines.transcoders.csv",
             "nef_pipelines.transcoders.echidna",
             "nef_pipelines.transcoders.fasta",
             "nef_pipelines.transcoders.mars",
             "nef_pipelines.transcoders.nmrpipe",
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import typer
 from typer.testing import CliRunner
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.tools.chains.clone import clone
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(clone)
 
+INPUT_3AA_NEF = read_test_data("3aa.nef", __file__)
 
-# noinspection PyUnusedLocal
-def test_clone_basic(clear_cache):
 
-    INPUT = open(path_in_test_data(__file__, "3aa.nef")).read()
+# noinspection PyUnusedLocal
+def test_clone_basic():
 
-    result = run_and_report(app, ["A", "2"], input=INPUT)
+    result = run_and_report(app, ["A", "2"], input=INPUT_3AA_NEF)
 
     EXPECTED = """\
             save_nef_molecular_system
                _nef_molecular_system.sf_category   nef_molecular_system
                _nef_molecular_system.sf_framecode  nef_molecular_system
 
                loop_
@@ -50,41 +50,35 @@
             save_
     """
 
     assert_lines_match(EXPECTED, isolate_frame(result.stdout, "nef_molecular_system"))
 
 
 # noinspection PyUnusedLocal
-def test_bad_count(clear_cache):
+def test_bad_count():
 
-    INPUT = open(path_in_test_data(__file__, "3aa.nef")).read()
-
-    result = run_and_report(app, ["A", "0"], input=INPUT, expected_exit_code=1)
+    result = run_and_report(app, ["A", "0"], input=INPUT_3AA_NEF, expected_exit_code=1)
 
     assert result.exit_code == 1
 
     assert "clone count must be > 0" in result.stdout
 
 
 # noinspection PyUnusedLocal
-def test_bad_target(clear_cache):
-
-    INPUT = open(path_in_test_data(__file__, "3aa.nef")).read()
+def test_bad_target():
 
-    result = run_and_report(app, ["B", "1"], input=INPUT, expected_exit_code=1)
+    result = run_and_report(app, ["B", "1"], input=INPUT_3AA_NEF, expected_exit_code=1)
 
     assert "couldn't find target chain B" in result.stdout
 
 
 # noinspection PyUnusedLocal
-def test_custom_chains(clear_cache):
-
-    INPUT = open(path_in_test_data(__file__, "3aa.nef")).read()
+def test_custom_chains():
 
-    result = run_and_report(app, ["A", "2", "--chains", "D,E"], input=INPUT)
+    result = run_and_report(app, ["A", "2", "--chains", "D,E"], input=INPUT_3AA_NEF)
 
     EXPECTED = """\
             save_nef_molecular_system
                _nef_molecular_system.sf_category   nef_molecular_system
                _nef_molecular_system.sf_framecode  nef_molecular_system
 
                loop_
@@ -111,17 +105,17 @@
             save_
     """
 
     assert_lines_match(EXPECTED, isolate_frame(result.stdout, "nef_molecular_system"))
 
 
 # noinspection PyUnusedLocal
-def test_clone_chain_clash(clear_cache):
+def test_clone_chain_clash():
 
-    INPUT = open(path_in_test_data(__file__, "3aa_x3.nef")).read()
+    INPUT = read_test_data("3aa_x3.nef", __file__)
 
     result = run_and_report(app, ["A", "2"], input=INPUT)
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import typer
+from pytest import fixture
 from typer.testing import CliRunner
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.tools.chains.rename import rename
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(rename)
 
 RENAME_CHAINS_B_D = ["B", "D"]
 RENAME_CHAINS_A_E = ["A", "E"]
 
 
+@fixture
+def INPUT_MULTI_CHAIN_SHIFTS_NEF():
+    return read_test_data("multi_chain_shifts.nef", __file__)
+
+
 # noinspection PyUnusedLocal
-def test_rename_basic(clear_cache):
+def test_rename_basic():
 
-    path = path_in_test_data(__file__, "multi_chain.nef")
+    INPUT = read_test_data("multi_chain.nef", __file__)
 
-    result = run_and_report(app, [*RENAME_CHAINS_B_D], input=open(path))
+    result = run_and_report(app, [*RENAME_CHAINS_B_D], input=INPUT)
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
 
     EXPECTED = """\
@@ -61,19 +67,19 @@
 
     """
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 # noinspection PyUnusedLocal
-def test_rename_multi_frame(clear_cache):
+def test_rename_multi_frame(INPUT_MULTI_CHAIN_SHIFTS_NEF):
 
-    path = path_in_test_data(__file__, "multi_chain_shifts.nef")
-
-    result = run_and_report(app, [*RENAME_CHAINS_A_E], input=open(path))
+    result = run_and_report(
+        app, [*RENAME_CHAINS_A_E], input=INPUT_MULTI_CHAIN_SHIFTS_NEF
+    )
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
 
     EXPECTED = """\
@@ -136,20 +142,18 @@
 
     """
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 # noinspection PyUnusedLocal
-def test_rename_select_frame_by_name(clear_cache):
-
-    path = path_in_test_data(__file__, "multi_chain_shifts.nef")
+def test_rename_select_frame_by_name(INPUT_MULTI_CHAIN_SHIFTS_NEF):
 
     result = run_and_report(
-        app, ["--frame", "test", *RENAME_CHAINS_A_E], input=open(path)
+        app, ["--frame", "test", *RENAME_CHAINS_A_E], input=INPUT_MULTI_CHAIN_SHIFTS_NEF
     )
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
 
@@ -209,22 +213,19 @@
 
     """
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 # noinspection PyUnusedLocal
-def test_rename_select_frame_by_category(clear_cache):
-
-    path = path_in_test_data(__file__, "multi_chain_shifts.nef")
-    input = open(path).read()
+def test_rename_select_frame_by_category(INPUT_MULTI_CHAIN_SHIFTS_NEF):
 
     command = [*RENAME_CHAINS_A_E, "--frame", "mol", "--selector-type", "category"]
 
-    result = run_and_report(app, command, input=input)
+    result = run_and_report(app, command, input=INPUT_MULTI_CHAIN_SHIFTS_NEF)
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
 
     EXPECTED = """\
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_import_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import typer
+from pytest import fixture
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.csv.importers.rdcs import rdcs
 
 app = typer.Typer()
 app.command()(rdcs)
 
 
+@fixture
+def INPUT_3A_AB_NEF():
+    return read_test_data("3a_ab.neff", __file__)
+
+
 # noinspection PyUnusedLocal
-def test_short_csv():
-    sequence_path = path_in_test_data(__file__, "3a_ab.neff")
+def test_short_csv(INPUT_3A_AB_NEF):
     csv_path = path_in_test_data(__file__, "short.csv")
 
-    nef_sequence = open(sequence_path, "r").read()
-
     args = [csv_path, "--chain-code", "AAAA"]
-    result = run_and_report(app, args, input=nef_sequence)
+    result = run_and_report(app, args, input=INPUT_3A_AB_NEF)
 
     EXPECTED = """\
         save_nef_rdc_restraint_list_rdcs
            _nef_rdc_restraint_list.sf_category           nef_rdc_restraint_list
            _nef_rdc_restraint_list.sf_framecode          nef_rdc_restraint_list_rdcs
            _nef_rdc_restraint_list.restraint_origin      .
            _nef_rdc_restraint_list.tensor_magnitude      .
@@ -67,22 +71,19 @@
 
     print(result.stdout)
     result = isolate_frame(result.stdout, "nef_rdc_restraint_list_rdcs")
 
     assert_lines_match(EXPECTED, result)
 
 
-def test_short_complete_csv():
-    sequence_path = path_in_test_data(__file__, "3a_ab.neff")
+def test_short_complete_csv(INPUT_3A_AB_NEF):
     csv_path = path_in_test_data(__file__, "short_complete.csv")
 
-    nef_sequence = open(sequence_path, "r").read()
-
     args = [csv_path]
-    result = run_and_report(app, args, input=nef_sequence)
+    result = run_and_report(app, args, input=INPUT_3A_AB_NEF)
 
     EXPECTED = """\
         save_nef_rdc_restraint_list_rdcs
            _nef_rdc_restraint_list.sf_category           nef_rdc_restraint_list
            _nef_rdc_restraint_list.sf_framecode          nef_rdc_restraint_list_rdcs
            _nef_rdc_restraint_list.restraint_origin      .
            _nef_rdc_restraint_list.tensor_magnitude      .
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     isolate_loop,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.echidna.importers.peaks import peaks
 
 app = typer.Typer()
 app.command()(peaks)
 
@@ -74,15 +75,15 @@
 """
 
 
 def test_basic():
 
     path = path_in_test_data(__file__, "echidna_peaks.txt")
 
-    data_sequence = open(path_in_test_data(__file__, "echidna_sequence.nef")).read()
+    data_sequence = read_test_data("echidna_sequence.nef", __file__)
 
     result = run_and_report(app, [path], input=data_sequence)
 
     loop = isolate_loop(result.stdout, "nef_nmr_spectrum_echidna_peaks", "nef_peak")
 
     assert_lines_match(EXPECTED, str(loop))
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/fasta/test_import_sequence.py`

 * *Files 24% similar despite different names*

```diff
@@ -129,7 +129,41 @@
 
     path = path_in_test_data(__file__, "3aa_x2.fasta")
     result = run_and_report(app, ["--starts", "1,11", path])
 
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
     assert_lines_match(EXPECTED_3A_AB_B_start_11, mol_sys_result)
+
+
+EXPECTED_3AA_HEADER_PARSING = """\
+save_nef_molecular_system
+   _nef_molecular_system.sf_category   nef_molecular_system
+   _nef_molecular_system.sf_framecode  nef_molecular_system
+
+   loop_
+      _nef_sequence.index
+      _nef_sequence.chain_code
+      _nef_sequence.sequence_code
+      _nef_sequence.residue_name
+      _nef_sequence.linking
+      _nef_sequence.residue_variant
+      _nef_sequence.cis_peptide
+
+     1   thx   -2   ALA   start    .   .
+     2   thx   -1   ALA   middle   .   .
+     3   thx    0   ALA   end      .   .
+
+   stop_
+
+save_"""
+
+
+def test_3aa_header_parsing():
+
+    path = path_in_test_data(__file__, "3aa_header.fasta")
+    result = run_and_report(app, [path])
+
+    mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
+
+    assert result.stdout.startswith("data_wibble")
+    assert_lines_match(EXPECTED_3AA_HEADER_PARSING, mol_sys_result)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_data/ubiquitin_short_unassign_single_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,62 @@
-import typer
-from typer.testing import CliRunner
+data_pales_test
 
-from nef_pipelines.lib.test_lib import (
-    assert_lines_match,
-    path_in_test_data,
-    run_and_report,
-)
-from nef_pipelines.tools.frames.delete import delete
+   save_nef_molecular_system
 
-runner = CliRunner()
-app = typer.Typer()
-app.command()(delete)
 
-EXPECTED_DELETE_CATEGORY = """\
-        data_pales_test
+      _nef_molecular_system.sf_category   nef_molecular_system
+      _nef_molecular_system.sf_framecode  nef_molecular_system
 
-        save_nef_rdc_restraint_list_test_1
-           _nef_rdc_restraint_list.sf_category     nef_rdc_restraint_list
-           _nef_rdc_restraint_list.sf_framecode    nef_rdc_restraint_list_test_1
-           _nef_rdc_restraint_list.potential_type  log-normal
 
-           loop_
-              _nef_rdc_restraint.index
-              _nef_rdc_restraint.restraint_id
-              _nef_rdc_restraint.restraint_combination_id
-              _nef_rdc_restraint.chain_code_1
-              _nef_rdc_restraint.sequence_code_1
-              _nef_rdc_restraint.residue_name_1
-              _nef_rdc_restraint.atom_name_1
-              _nef_rdc_restraint.chain_code_2
-              _nef_rdc_restraint.sequence_code_2
-              _nef_rdc_restraint.residue_name_2
-              _nef_rdc_restraint.atom_name_2
-              _nef_rdc_restraint.weight
-              _nef_rdc_restraint.target_value
-              _nef_rdc_restraint.target_value_uncertainty
+      loop_
 
-             1   1   .   A   2   TRP   H   A   21   TRP   N   2   -5.2   0.33
-             2   2   .   A   3   GLY   H   A   22   GLY   N   3   3.1    0.4
+         _nef_sequence.index
+         _nef_sequence.chain_code
+         _nef_sequence.sequence_code
+         _nef_sequence.residue_name
+         _nef_sequence.linking
+         _nef_sequence.residue_variant
+         _nef_sequence.cis_peptide
 
-           stop_
 
-        save_
-    """
+           1  AAAA  1  ALA  start      .            .
+           2  AAAA  2  TRP  middle     .            .
+           3  AAAA  3  GLY  middle     .            .
 
+      stop_
+   save_
 
-# noinspection PyUnusedLocal
-def test_delete_type(clear_cache):
 
-    path = path_in_test_data(__file__, "pales_test_1.nef")
+   save_nef_rdc_restraint_list_test_1
 
-    input_stream = open(path).read()
 
-    result = run_and_report(app, ["-c", "mol"], input=input_stream)
+      _nef_rdc_restraint_list.sf_category           nef_rdc_restraint_list
+      _nef_rdc_restraint_list.sf_framecode          nef_rdc_restraint_list_test_1
+      _nef_rdc_restraint_list.potential_type        log-normal
 
-    assert_lines_match(EXPECTED_DELETE_CATEGORY, result.stdout)
 
 
-EXPECTED_DELETE_NAME = """\
-    data_pales_test
+      loop_
 
-    save_nef_molecular_system
-       _nef_molecular_system.sf_category   nef_molecular_system
-       _nef_molecular_system.sf_framecode  nef_molecular_system
+         _nef_rdc_restraint.index
+         _nef_rdc_restraint.restraint_id
+         _nef_rdc_restraint.restraint_combination_id
+         _nef_rdc_restraint.chain_code_1
+         _nef_rdc_restraint.sequence_code_1
+         _nef_rdc_restraint.residue_name_1
+         _nef_rdc_restraint.atom_name_1
+         _nef_rdc_restraint.chain_code_2
+         _nef_rdc_restraint.sequence_code_2
+         _nef_rdc_restraint.residue_name_2
+         _nef_rdc_restraint.atom_name_2
+         _nef_rdc_restraint.weight
+         _nef_rdc_restraint.target_value
+         _nef_rdc_restraint.target_value_uncertainty
 
-       loop_
-          _nef_sequence.index
-          _nef_sequence.chain_code
-          _nef_sequence.sequence_code
-          _nef_sequence.residue_name
-          _nef_sequence.linking
-          _nef_sequence.residue_variant
-          _nef_sequence.cis_peptide
 
-         1   A   1   ALA   start    .   .
-         2   A   2   TRP   middle   .   .
-         3   A   3   GLY   middle   .   .
 
-       stop_
 
-    save_
+         1  1  .  AAAA  3  GLY  H  AAAA  22  GLY  N  3   3.1   0.4
+         2  2  .  AAAA  2  TRP  H  AAAA  21  TRP  N  2  -5.2  0.33
+      stop_
 
-"""
-
-
-# noinspection PyUnusedLocal
-def test_delete_name(clear_cache):
-
-    path = path_in_test_data(__file__, "pales_test_1.nef")
-
-    input_stream = open(path).read()
-
-    result = run_and_report(app, ["test_1"], input=input_stream)
-
-    assert_lines_match(EXPECTED_DELETE_NAME, result.stdout)
+   save_
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/frames/test_unassign.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/frames/test_unassign.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typer
+from pytest import fixture
 
 from nef_pipelines.lib.test_lib import (
     NOQA_E501,
     assert_lines_match,
     isolate_loop,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.tools.frames.unassign import unassign
 
 EXIT_ERROR = 1
 
 app = typer.Typer()
@@ -79,21 +80,23 @@
 
 stop_
 """.replace(
     NOQA_E501, ""
 )
 
 
+@fixture
+def INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN():
+    return read_test_data("ubiquitin_short_unassign_single_chain.nef", __file__)
+
+
 # noinspection PyUnusedLocal
-def test_unassign_basic():
+def test_unassign_basic(INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN):
 
-    INPUT = open(
-        path_in_test_data(__file__, "ubiquitin_short_unassign_single_chain.nef")
-    ).read()
-    result = run_and_report(app, [], input=INPUT)
+    result = run_and_report(app, [], input=INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN)
 
     loop = isolate_loop(
         result.stdout, "nef_chemical_shift_list_default", "nef_chemical_shift"
     )
     assert_lines_match(EXPECTED_BASIC_SHIFT_LIST, loop)
 
     loop = isolate_loop(result.stdout, "nef_nmr_spectrum_simnoe", "nef_peak")
@@ -165,20 +168,19 @@
 
     stop_
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_unassign_all():
+def test_unassign_all(INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN):
 
-    INPUT = open(
-        path_in_test_data(__file__, "ubiquitin_short_unassign_single_chain.nef")
-    ).read()
-    result = run_and_report(app, ["--targets", "all"], input=INPUT)
+    result = run_and_report(
+        app, ["--targets", "all"], input=INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN
+    )
 
     loop = isolate_loop(
         result.stdout, "nef_chemical_shift_list_default", "nef_chemical_shift"
     )
     assert_lines_match(loop, EXPECTED_FULL_SHIFT_LIST)
 
     loop = isolate_loop(result.stdout, "nef_nmr_spectrum_simnoe", "nef_peak")
@@ -250,21 +252,20 @@
 
     stop_
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_unassign_complete():
+def test_unassign_complete(INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN):
 
-    INPUT = open(
-        path_in_test_data(__file__, "ubiquitin_short_unassign_single_chain.nef")
-    ).read()
     result = run_and_report(
-        app, ["--targets", "all", "--sequence-mode", "unused"], input=INPUT
+        app,
+        ["--targets", "all", "--sequence-mode", "unused"],
+        input=INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN,
     )
 
     loop = isolate_loop(
         result.stdout, "nef_chemical_shift_list_default", "nef_chemical_shift"
     )
     assert_lines_match(loop, EXPECTED_UNUSED_SHIFT_LIST)
 
@@ -337,20 +338,21 @@
 
     stop_
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_unassign_ordered():
+def test_unassign_ordered(INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN):
 
-    INPUT = open(
-        path_in_test_data(__file__, "ubiquitin_short_unassign_single_chain.nef")
-    ).read()
-    result = run_and_report(app, ["--sequence-mode", "ordered"], input=INPUT)
+    result = run_and_report(
+        app,
+        ["--sequence-mode", "ordered"],
+        input=INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN,
+    )
 
     loop = isolate_loop(
         result.stdout, "nef_chemical_shift_list_default", "nef_chemical_shift"
     )
     assert_lines_match(loop, EXPECTED_ORDERED_SHIFT_LIST)
 
     loop = isolate_loop(result.stdout, "nef_nmr_spectrum_simnoe", "nef_peak")
@@ -422,19 +424,20 @@
 
     stop_
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_unassign_preserve():
-    INPUT = open(
-        path_in_test_data(__file__, "ubiquitin_short_unassign_single_chain.nef")
-    ).read()
-    result = run_and_report(app, ["--sequence-mode", "preserve"], input=INPUT)
+def test_unassign_preserve(INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN):
+    result = run_and_report(
+        app,
+        ["--sequence-mode", "preserve"],
+        input=INPUT_UBI_SHORT_UNASSIGNED_SINGLE_CHAIN,
+    )
 
     loop = isolate_loop(
         result.stdout, "nef_chemical_shift_list_default", "nef_chemical_shift"
     )
     assert_lines_match(loop, EXPECTED_PRESERVED_SHIFT_LIST)
 
     loop = isolate_loop(result.stdout, "nef_nmr_spectrum_simnoe", "nef_peak")
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/short_co.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/short_co.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_data/ubi_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.mars.exporters.shifts import shifts
 
 app = typer.Typer()
 app.command()(shifts)
 
 
 def test_export_shifts_nef5_short():
-    stream = open(path_in_test_data(__file__, "sec5_short.neff")).read()
+    input = read_test_data("sec5_short.neff", __file__)
 
-    result = run_and_report(app, ["-"], input=stream)
+    result = run_and_report(app, ["-"], input=input)
 
     EXPECTED = """\
               H      N        CA      CA-1    CB      CB-1
         PR_1  8.594  133.252  61.159  59.291  33.274  37.309
         PR_2  8.928  131.397  -       -       -       -
         PR_3  9.671  130.698  60.735  62.418  39.792  69.744
         PR_4  8.185  128.894  53.744  54.679  43.207  34.050
@@ -26,17 +26,17 @@
     """
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 def test_export_shifts_pete_co():
 
-    stream = open(path_in_test_data(__file__, "short_co.neff")).read()
+    input = read_test_data("short_co.neff", __file__)
 
-    result = run_and_report(app, ["-"], input=stream)
+    result = run_and_report(app, ["-"], input=input)
 
     EXPECTED = """\
                    H        N  CA      CA-1    CB-1    CO       CO-1
         PR_1  11.671  136.682  -       -       -       -        -
         PR_2  10.946  131.689  -       -       -       -        -
         PR_3  10.266  112.518  46.281  63.862  32.984  176.722  178.726
         PR_4   9.632  104.529  46.465  -       -       173.390  175.767
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_import_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_import_peaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_loop,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.mars.importers.peaks import peaks
 
 app = typer.Typer()
 app.command()(peaks)
 
@@ -141,15 +142,15 @@
 """.replace(
     NOQUA_E501, ""
 )
 
 
 def test_import_peaks():
 
-    sequence_stream = open(path_in_test_data(__file__, "ubi_seq.nef")).read()
+    sequence_stream = read_test_data("ubi_seq.nef", __file__)
 
     filenames = "sparky_all.out sparky_CA-1.out sparky_CA.out".split()
 
     paths = [path_in_test_data(__file__, filename) for filename in filenames]
     result = run_and_report(app, paths, input=sequence_stream)
 
     loop = isolate_loop(result.stdout, "nef_nmr_spectrum_mars_HNCA", "nef_peak")
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.nmrpipe.importers.peaks import peaks
 
-HEADER = open(path_in_test_data(__file__, "test_header_entry.txt")).read()
+HEADER = read_test_data("test_header_entry.txt", __file__)
 
 PEAKS_NMRPIPE = "nef_nmr_spectrum_nmrpipe"
 METADATA_NMRPIPE = "nef_nmr_meta_data"
 
 
 app = typer.Typer()
 app.command()(peaks)
 
 
 # noinspection PyUnusedLocal
 def test_peaks():
-    EXPECTED = open(
-        path_in_test_data(__file__, "gb3_assigned_trunc_expected.tab")
-    ).read()
+    EXPECTED = read_test_data("gb3_assigned_trunc_expected.tab", __file__)
 
     path = path_in_test_data(__file__, "gb3_assigned_trunc.tab")
     result = run_and_report(app, [path], input=HEADER)
 
     assert result.exit_code == 0
     peaks_result = isolate_frame(result.stdout, "%s" % PEAKS_NMRPIPE)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from freezegun import freeze_time
 
 from nef_pipelines.lib.nef_lib import NEF_METADATA, NEF_MOLECULAR_SYSTEM
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.lib.util import get_version
 from nef_pipelines.transcoders.nmrpipe.importers.sequence import sequence
 
-HEADER = open(path_in_test_data(__file__, "test_header_entry.txt")).read()
+HEADER = read_test_data("test_header_entry.txt", __file__)
 
 app = typer.Typer()
 app.command()(sequence)
 
 
 EXPECTED_3AA = """\
 save_nef_molecular_system
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,29 @@
     ShiftData,
     ShiftList,
 )
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.nmrpipe.importers.shifts import shifts as shifts_app
 from nef_pipelines.transcoders.nmrpipe.nmrpipe_lib import (
     read_db_file_records,
     read_shift_file,
 )
 
 app = typer.Typer()
 app.command()(shifts_app)
 
 SHIFTS_NMRPIPE = "nef_chemical_shift_list_nmrpipe"
 
-HEADER = open(path_in_test_data(__file__, "test_header_entry.txt")).read()
+HEADER = read_test_data("test_header_entry.txt", __file__)
 
 
 def test_lib_parse_shifts():
 
     EXPECTED = ShiftList(
         shifts=[
             ShiftData(
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/4peaks_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import typer
 
 from nef_pipelines.lib.structures import AtomLabel, Peak, PeakValues, SequenceResidue
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.nmrview.exporters.peaks import (
     _make_names_unique,
     _row_to_peak,
     peaks,
 )
 
 app = typer.Typer()
 app.command()(peaks)
 
-EXPECTED = open(
-    path_in_test_data(__file__, "expected_sequence_and_peaks_nmrview.txt")
-).read()
+EXPECTED = read_test_data("expected_sequence_and_peaks_nmrview.txt", __file__)
 
 EXPECTED_AXES = ["1H_1", "1H_2", "15N"]
 
 
 def test_make_names_unique():
     TEST = ["1H", "1H", "15N"]
 
@@ -88,18 +86,18 @@
         assignments=assignments,
         values=PeakValues(serial=1, volume=0.38, height=0.38),
     )
 
     assert result == EXPECTED_PEAK
 
 
-EXPECTED = open(path_in_test_data(__file__, "expected_nmr_view.xpk")).read()
+EXPECTED = read_test_data("expected_nmr_view.xpk", __file__)
 
 
 # noinspection PyUnusedLocal
-def test_3peaks(clear_cache):
+def test_3peaks():
 
-    STREAM = open(path_in_test_data(__file__, "nef_3_peaks.nef")).read()
+    STREAM = read_test_data("nef_3_peaks.nef", __file__)
 
     result = run_and_report(app, [], input=STREAM)
 
     assert_lines_match(EXPECTED, result.stdout)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 from textwrap import dedent
 
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.nmrview.exporters.sequences import sequences
 
 app = typer.Typer()
 app.command()(sequences)
 
+INPUT_MULTI_CHAIN_NEF = read_test_data("multi_chain.nef", __file__)
+
 
 # noinspection PyUnusedLocal
 def test_multi_chain():
 
-    STREAM = open(path_in_test_data(__file__, "multi_chain.nef")).read()
-
-    result = run_and_report(app, ["-o", "-"], input=STREAM)
+    result = run_and_report(app, ["-o", "-"], input=INPUT_MULTI_CHAIN_NEF)
 
     EXPECTED = """\
         ------------- A.seq -------------
         his 3
         met
         ------------- B.seq -------------
         arg 5
@@ -34,17 +34,17 @@
     """
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 def test_multi_chain_template():
 
-    STREAM = open(path_in_test_data(__file__, "multi_chain.nef")).read()
-
-    result = run_and_report(app, ["-o", "-test_{chain_code}.seq"], input=STREAM)
+    result = run_and_report(
+        app, ["-o", "-test_{chain_code}.seq"], input=INPUT_MULTI_CHAIN_NEF
+    )
 
     EXPECTED = """\
         ------------- test_A.seq -------------
         his 3
         met
         ------------- test_B.seq -------------
         arg 5
@@ -55,44 +55,41 @@
     """
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 def test_multi_chain_bad_selector():
 
-    STREAM = open(path_in_test_data(__file__, "multi_chain.nef")).read()
-
     result = run_and_report(
-        app, ["-o", "-", "AAAA"], input=STREAM, expected_exit_code=1
+        app, ["-o", "-", "AAAA"], input=INPUT_MULTI_CHAIN_NEF, expected_exit_code=1
     )
 
     assert "the chain code" in result.stdout
     assert "not in the molecular systems chain codes" in result.stdout
     assert "AAAA" in result.stdout
 
 
 def test_bad_template():
 
-    STREAM = open(path_in_test_data(__file__, "multi_chain.nef")).read()
-
     result = run_and_report(
-        app, ["-o", "test.seq", "A"], input=STREAM, expected_exit_code=1
+        app, ["-o", "test.seq", "A"], input=INPUT_MULTI_CHAIN_NEF, expected_exit_code=1
     )
 
     assert "the file name template" in result.stdout
     assert "does not contain the string" in result.stdout
     assert "{chain_code}" in result.stdout
 
 
-def test_multiple_output_files_disk(tmp_path):
-    STREAM = open(path_in_test_data(__file__, "multi_chain.nef")).read()
+def test_multiple_output_files_disk(
+    tmp_path,
+):
 
     os.chdir(tmp_path)
 
-    run_and_report(app, [], input=STREAM)
+    run_and_report(app, [], input=INPUT_MULTI_CHAIN_NEF)
 
     EXPECTED_FILES = "A.seq", "B.seq", "C.seq"
 
     for file_name in EXPECTED_FILES:
         assert (tmp_path / file_name).is_file()
 
     EXPECTED = {
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.nmrview.importers.peaks import peaks
 
 MOLECULAR_SYSTEM_NMRVIEW = "nef_spectrum_nmrview"
 
 app = typer.Typer()
 app.command()(peaks)
 
-EXPECTED_4AA = open(path_in_test_data(__file__, "nmrview_expected_4aa.txt")).read()
+
+EXPECTED_4AA = read_test_data("nmrview_expected_4aa.txt", __file__)
 
 
 # noinspection PyUnusedLocal
-def test_4_peaks(clear_cache):
+def test_4_peaks():
     peaks_path = path_in_test_data(__file__, "4peaks.xpk")
-    sequence_stream = open(path_in_test_data(__file__, "4peaks_seq.nef")).read()
+
+    sequence_stream = read_test_data("4peaks_seq.nef", __file__)
 
     args = ["--axis", "1H.1H.15N", peaks_path]
     result = run_and_report(app, args, input=sequence_stream)
 
     result = isolate_frame(result.stdout, "nef_nmr_spectrum_simnoe")
 
     assert_lines_match(EXPECTED_4AA, result)
 
 
-def test_3peaks_bad_axis_codes(clear_cache):
+def test_3peaks_bad_axis_codes():
     # reading stdin doesn't work in pytest so for a clean header
     # TODO move to conftest.py
     peaks_path = path_in_test_data(__file__, "4peaks.xpk")
-    sequence_stream = open(path_in_test_data(__file__, "4peaks_seq.nef")).read()
+
+    sequence_stream = read_test_data("4peaks_seq.nef", __file__)
 
     args = [
         "--axis",
         "1H,15N",
         peaks_path,
     ]
     result = run_and_report(app, args, expected_exit_code=1, input=sequence_stream)
@@ -109,15 +113,16 @@
     save_
 """
 
 
 # noinspection PyUnusedLocal
 def test_joe_bad_sweep_widths():
     peaks_path = path_in_test_data(__file__, "joe_clic.xpk")
-    sequence_stream = open(path_in_test_data(__file__, "4peaks_seq.nef")).read()
+
+    sequence_stream = read_test_data("4peaks_seq.nef", __file__)
 
     command = [
         "--axis",
         "1H.1H.15N",
         peaks_path,
     ]
     result = run_and_report(app, command, input=sequence_stream)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from freezegun import freeze_time
 
 from nef_pipelines.lib.nef_lib import NEF_METADATA, NEF_MOLECULAR_SYSTEM
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.lib.util import get_version
 from nef_pipelines.transcoders.nmrview.importers.sequence import sequence
 
 app = typer.Typer()
 app.command()(sequence)
@@ -78,15 +79,15 @@
     result = run_and_report(app, [path], input=HEADER)
 
     mol_sys_result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
     assert_lines_match(EXPECTED_3AA10, mol_sys_result)
 
 
-HEADER = open(path_in_test_data(__file__, "test_header_entry.txt")).read()
+HEADER = read_test_data("test_header_entry.txt", __file__)
 
 EXPECTED_HEADER = f"""\
 save_nef_nmr_meta_data
    _nef_nmr_meta_data.sf_category      nef_nmr_meta_data
    _nef_nmr_meta_data.sf_framecode     nef_nmr_meta_data
    _nef_nmr_meta_data.format_name      nmr_exchange_format
    _nef_nmr_meta_data.format_version   1.1
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ShiftData,
     ShiftList,
 )
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.nmrview.importers.shifts import shifts
 from nef_pipelines.transcoders.nmrview.nmrview_lib import parse_shifts
 
 SHIFTS_NMRVIEW = "nef_chemical_shift_list_nmrview"
 
@@ -134,30 +135,29 @@
         stop_
 
     save_
 """
 
 
 # # noinspection PyUnusedLocal
-def test_ppm_out_short_no_sequence(clear_cache):
+def test_ppm_out_short_no_sequence():
 
-    STREAM = open(path_in_test_data(__file__, "header.nef")).read()
+    STREAM = read_test_data("header.nef", __file__)
 
     path = path_in_test_data(__file__, "ppm_short.out")
     result = run_and_report(app, [path], expected_exit_code=1, input=STREAM)
 
-    print(result.stdout)
     assert "ERROR" in result.stdout
     assert "did you read a sequence?" in result.stdout
 
 
 # noinspection PyUnusedLocal
-def test_ppm_out_short(clear_cache):
+def test_ppm_out_short():
 
-    STREAM = open(path_in_test_data(__file__, "ppm_short_seq.nef")).read()
+    STREAM = read_test_data("ppm_short_seq.nef", __file__)
 
     path = path_in_test_data(__file__, "ppm_short.out")
 
     result = run_and_report(app, [path], input=STREAM)
 
     mol_sys_result = isolate_frame(result.stdout, SHIFTS_NMRVIEW)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-data_pales_test
+data_xplor
 
-   save_nef_molecular_system
+    save_nef_molecular_system
+        _nef_molecular_system.sf_category   nef_molecular_system
+        _nef_molecular_system.sf_framecode  nef_molecular_system
+
+        loop_
+            _nef_sequence.index
+            _nef_sequence.chain_code
+            _nef_sequence.sequence_code
+            _nef_sequence.residue_name
+            _nef_sequence.linking
+            _nef_sequence.residue_variant
+            _nef_sequence.cis_peptide
+
+            1   AAAA   1    ALA   start    .   .
+            2   AAAA   2    ALA   middle   .   .
+            3   AAAA   3    ALA   end      .   .
+            4   BBBB   11   ALA   start    .   .
+            5   BBBB   12   ALA   middle   .   .
+            6   BBBB   13   ALA   end      .   .
+
+        stop_
+    save_
+
+    save_nef_rdc_restraint_list_rdcs
+        _nef_rdc_restraint_list.sf_category           nef_rdc_restraint_list
+        _nef_rdc_restraint_list.sf_framecode          nef_rdc_restraint_list_rdcs
+        _nef_rdc_restraint_list.restraint_origin      .
+        _nef_rdc_restraint_list.tensor_magnitude      .
+        _nef_rdc_restraint_list.tensor_rhombicity     .
+        _nef_rdc_restraint_list.tensor_chain_code     .
+        _nef_rdc_restraint_list.tensor_sequence_code  .
+        _nef_rdc_restraint_list.tensor_residue_name   .
+
+        loop_
+            _nef_rdc_restraint.index
+            _nef_rdc_restraint.restraint_id
+            _nef_rdc_restraint.restraint_combination_id
+            _nef_rdc_restraint.chain_code_1
+            _nef_rdc_restraint.sequence_code_1
+            _nef_rdc_restraint.residue_name_1
+            _nef_rdc_restraint.atom_name_1
+            _nef_rdc_restraint.chain_code_2
+            _nef_rdc_restraint.sequence_code_2
+            _nef_rdc_restraint.residue_name_2
+            _nef_rdc_restraint.atom_name_2
+            _nef_rdc_restraint.weight
+            _nef_rdc_restraint.target_value
+            _nef_rdc_restraint.target_value_uncertainty
+            _nef_rdc_restraint.lower_linear_limit
+            _nef_rdc_restraint.lower_limit
+            _nef_rdc_restraint.upper_limit
+            _nef_rdc_restraint.upper_linear_limit
+            _nef_rdc_restraint.scale
+            _nef_rdc_restraint.distance_dependent
+
+            0   0   .   AAAA   1   ALA   HA     AAAA   1   ALA   HN   1.0   1.3   1.0   .   .   .   .   1.0   .
+            1   1   .   AAAA   1   ALA   HB     AAAA   1   ALA   HN   1.0   4.6   2.0   .   .   .   .   1.0   .
+            2   2   .   AAAA   2   ALA   HG3#   AAAA   2   ALA   HN   1.0   2.4   3.0   .   .   .   .   1.0   .
+            3   3   .   AAAA   3   ALA   HA     AAAA   3   ALA   HN   1.0   6.7   4.0   .   .   .   .   1.0   .
 
+        stop_
 
-      _nef_molecular_system.sf_category   nef_molecular_system
-      _nef_molecular_system.sf_framecode  nef_molecular_system
-
-
-      loop_
-
-         _nef_sequence.index
-         _nef_sequence.chain_code
-         _nef_sequence.sequence_code
-         _nef_sequence.residue_name
-         _nef_sequence.linking
-         _nef_sequence.residue_variant
-         _nef_sequence.cis_peptide
-
-
-           1  AAAA  1  ALA  start      .            .
-           2  AAAA  2  TRP  middle     .            .
-           3  AAAA  3  GLY  middle     .            .
-
-      stop_
-   save_
-
-
-   save_nef_rdc_restraint_list_test_1
-
-
-      _nef_rdc_restraint_list.sf_category           nef_rdc_restraint_list
-      _nef_rdc_restraint_list.sf_framecode          nef_rdc_restraint_list_test_1
-      _nef_rdc_restraint_list.potential_type        log-normal
-
-
-
-      loop_
-
-         _nef_rdc_restraint.index
-         _nef_rdc_restraint.restraint_id
-         _nef_rdc_restraint.restraint_combination_id
-         _nef_rdc_restraint.chain_code_1
-         _nef_rdc_restraint.sequence_code_1
-         _nef_rdc_restraint.residue_name_1
-         _nef_rdc_restraint.atom_name_1
-         _nef_rdc_restraint.chain_code_2
-         _nef_rdc_restraint.sequence_code_2
-         _nef_rdc_restraint.residue_name_2
-         _nef_rdc_restraint.atom_name_2
-         _nef_rdc_restraint.weight
-         _nef_rdc_restraint.target_value
-         _nef_rdc_restraint.target_value_uncertainty
-
-
-
-
-         1  1  .  AAAA  3  GLY  H  AAAA  22  GLY  N  3   3.1   0.4
-         2  2  .  AAAA  2  TRP  H  AAAA  21  TRP  N  2  -5.2  0.33
-      stop_
-
-   save_
+    save_
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from textwrap import dedent
 
 import typer
 from typer.testing import CliRunner
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.pales.exporters.rdcs import rdcs
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(rdcs)
 
-NEF_STREAM = open(path_in_test_data(__file__, "pales_test_1.nef")).read()
-NEF_STREAM_DISORDERED = open(path_in_test_data(__file__, "pales_test_2.nef")).read()
-NEF_STREAM_SEGIDS = open(path_in_test_data(__file__, "pales_test_segids.nef")).read()
+NEF_STREAM = read_test_data("pales_test_1.nef", __file__)
+NEF_STREAM_DISORDERED = read_test_data("pales_test_2.nef", __file__)
+NEF_STREAM_SEGIDS = read_test_data("pales_test_segids.nef", __file__)
 
 
 # noinspection PyUnusedLocal
-def test_rdcs(clear_cache):
+def test_rdcs():
 
     result = run_and_report(app, [], input=NEF_STREAM)
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
@@ -39,15 +39,15 @@
     """
     EXPECTED = dedent(EXPECTED)
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 # noinspection PyUnusedLocal
-def test_rdcs_disordered(clear_cache):
+def test_rdcs_disordered():
 
     result = run_and_report(app, [], input=NEF_STREAM_DISORDERED)
 
     assert result.exit_code == 0
 
     EXPECTED = """\
 
@@ -57,15 +57,15 @@
                 2        TRP        HN          21       TRP        N          -5.2    0.33   1.0
 
     """
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
-def test_rdcs_segid(clear_cache):
+def test_rdcs_segid():
 
     result = run_and_report(app, ["--segids"], input=NEF_STREAM_SEGIDS)
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/pales/test_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.pales.exporters.template import template
 
 app = typer.Typer()
 app.command()(template)
 
-SEQUENCE_STREAM = open(path_in_test_data(__file__, "tailin_seq_short.nef")).read()
+SEQUENCE_STREAM = read_test_data("tailin_seq_short.nef", __file__)
 
 
 # noinspection PyUnusedLocal
-def test_template(clear_cache):
+def test_template():
 
     result = run_and_report(app, [], input=SEQUENCE_STREAM)
 
     if result.exit_code != 0:
         print("INFO: stdout from failed read:\n", result.stdout)
 
     assert result.exit_code == 0
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.cif`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/rcsb/test_sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/rcsb/test_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import typer
 
 from nef_pipelines.lib.nef_lib import NEF_MOLECULAR_SYSTEM
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.rcsb.importers.sequence import sequence
 
 app = typer.Typer()
 app.command()(sequence)
 
-HEADER = open(path_in_test_data(__file__, "test_header_entry.txt")).read()
+HEADER = read_test_data("test_header_entry.txt", __file__)
 
 EXPECTED_3AA = """\
     save_nef_molecular_system
         _nef_molecular_system.sf_category   nef_molecular_system
         _nef_molecular_system.sf_framecode  nef_molecular_system
 
         loop_
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/simulate/test_simulate_peaks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import typer
 from typer.testing import CliRunner
 
 from nef_pipelines.lib.test_lib import (
     NOQA_E501,
     assert_lines_match,
     isolate_frame,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
-from nef_pipelines.tools.shifts.make_peaks import make_peaks
+from nef_pipelines.tools.simulate.peaks import peaks
 
 runner = CliRunner()
 app = typer.Typer()
-app.command()(make_peaks)
+app.command()(peaks)
 
 EXPECTED = """ # noqa: E501
 save_nef_nmr_spectrum_synthetic_N_HSQC
    _nef_nmr_spectrum.sf_category                nef_nmr_spectrum
    _nef_nmr_spectrum.sf_framecode               nef_nmr_spectrum_synthetic_N_HSQC
    _nef_nmr_spectrum.num_dimensions             2
    _nef_nmr_spectrum.chemical_shift_list        .
@@ -77,34 +77,38 @@
 
 save_
 """.replace(
     NOQA_E501, ""
 )
 
 
+INPUT_UBI_SHORT_NEF = read_test_data("ubiquitin_short.nef", __file__)
+
+
 # noinspection PyUnusedLocal
 def test_ubi_short():
 
-    input = open(path_in_test_data(__file__, "ubiquitin_short.nef")).read()
-    result = run_and_report(app, [], input=input)
+    result = run_and_report(app, [], input=INPUT_UBI_SHORT_NEF)
 
     new_peaks_frame = isolate_frame(result.stdout, "nef_nmr_spectrum_synthetic_N_HSQC")
     assert_lines_match(EXPECTED, new_peaks_frame)
 
 
 def test_ubi_short_different_frame_name():
-    input = open(path_in_test_data(__file__, "ubiquitin_short.nef")).read()
-    result = run_and_report(app, ["--name-template", "wibble_{spectrum}"], input=input)
+    result = run_and_report(
+        app, ["--name-template", "wibble_{spectrum}"], input=INPUT_UBI_SHORT_NEF
+    )
 
     isolate_frame(result.stdout, "nef_nmr_spectrum_wibble_N_HSQC")
 
 
 def test_ubi_short_different_spectrometer_frequency():
-    input = open(path_in_test_data(__file__, "ubiquitin_short.nef")).read()
-    result = run_and_report(app, ["--spectrometer-frequency", "800"], input=input)
+    result = run_and_report(
+        app, ["--spectrometer-frequency", "800"], input=INPUT_UBI_SHORT_NEF
+    )
 
     EXPECTED_800 = EXPECTED.replace("60.833", "81.095")
     EXPECTED_800 = EXPECTED_800.replace("600.123", "800.000")
     new_peaks_frame = isolate_frame(result.stdout, "nef_nmr_spectrum_synthetic_N_HSQC")
     assert_lines_match(EXPECTED_800, new_peaks_frame)
 
 
@@ -185,13 +189,12 @@
 """.replace(
     NOQA_E501, ""
 )
 
 
 def test_ubi_short_triple():
 
-    input = open(path_in_test_data(__file__, "ubiquitin_short.nef")).read()
-    result = run_and_report(app, ["--spectra", "HNCA"], input=input)
+    result = run_and_report(app, ["HNCA"], input=INPUT_UBI_SHORT_NEF)
 
     print(result.stdout)
     new_peaks_frame = isolate_frame(result.stdout, "nef_nmr_spectrum_synthetic_HNCA")
     assert_lines_match(EXPECTED_HNCA, new_peaks_frame)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typer
 from typer.testing import CliRunner
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.shifty.exporters.shifts import shifts
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(shifts)
@@ -17,13 +17,13 @@
 1     A   5.320  0.000  115.740  53.270  20.340  181.080
 2     G   0.000  7.310  117.940  46.770   0.000  176.920
 3     V   5.020  8.820  116.850  71.710  33.150  172.980
 """
 
 
 # noinspection PyUnusedLocal
-def test_3ab(clear_cache):
+def test_3ab():
 
-    input = open(path_in_test_data(__file__, "test_agv.neff")).read()
+    input = read_test_data("test_agv.neff", __file__)
     result = run_and_report(app, ["-"], input=input)
 
     assert_lines_match(EXPECTED, result.stdout)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.sparky.exporters.peaks import peaks
 
 SHIFTS_SPARKY = "nef_chemical_shift_list_sparky"
 
 app = typer.Typer()
@@ -22,20 +23,22 @@
   PR_65N-H       104.408  6.517       11       3
   PR_67N-H       103.504  7.048       12       4
 
 ************************************************************************************
 
 """
 
+INPUT_UBI_PEAKS_SHORT_NEF = read_test_data("ubi_peaks_short.neff", __file__)
 
-def test_ppm_out_short():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
+def test_ppm_out_short():
 
-    result = run_and_report(app, ["--file-name-template", "-"], input=STREAM)
+    result = run_and_report(
+        app, ["--file-name-template", "-"], input=INPUT_UBI_PEAKS_SHORT_NEF
+    )
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 EXPECTED_SUPPRESS_ASSIGNMENT = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
 
@@ -48,20 +51,18 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_suppress_assigment():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
-
     result = run_and_report(
         app,
         ["--file-name-template", "-", "--suppress-column", "assignment"],
-        input=STREAM,
+        input=INPUT_UBI_PEAKS_SHORT_NEF,
     )
 
     assert_lines_match(EXPECTED_SUPPRESS_ASSIGNMENT, result.stdout)
 
 
 EXPECTED_NO_HEIGHT = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
@@ -76,18 +77,18 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_no_height():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
-
     result = run_and_report(
-        app, ["--file-name-template", "-", "--suppress-column", "height"], input=STREAM
+        app,
+        ["--file-name-template", "-", "--suppress-column", "height"],
+        input=INPUT_UBI_PEAKS_SHORT_NEF,
     )
 
     assert_lines_match(EXPECTED_NO_HEIGHT, result.stdout)
 
 
 EXPECTED_NO_VOLUME = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
@@ -102,18 +103,18 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_no_volume():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
-
     result = run_and_report(
-        app, ["--file-name-template", "-", "--suppress-column", "volume"], input=STREAM
+        app,
+        ["--file-name-template", "-", "--suppress-column", "volume"],
+        input=INPUT_UBI_PEAKS_SHORT_NEF,
     )
 
     assert_lines_match(EXPECTED_NO_VOLUME, result.stdout)
 
 
 EXPECTED_NO_HEIGHT_OR_VOLUME = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
@@ -128,46 +129,42 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_no_height_or_volume():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
-
     result = run_and_report(
         app,
         [
             "--file-name-template",
             "-",
             "--suppress-column",
             "volume",
             "--suppress-column",
             "height",
         ],
-        input=STREAM,
+        input=INPUT_UBI_PEAKS_SHORT_NEF,
     )
 
     assert_lines_match(EXPECTED_NO_HEIGHT_OR_VOLUME, result.stdout)
 
 
 def test_ppm_out_short_no_height_or_volume_with_data():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
-
     result = run_and_report(
         app,
         [
             "--file-name-template",
             "-",
             "--suppress-column",
             "volume,height",
             "--add-data",
         ],
-        input=STREAM,
+        input=INPUT_UBI_PEAKS_SHORT_NEF,
     )
 
     assert_lines_match(EXPECTED_NO_HEIGHT_OR_VOLUME, result.stdout)
 
 
 EXPECTED_DIFFERENT_RESIDUES = """\
 ****************************** nef_nmr_spectrum_peaks ******************************
@@ -180,17 +177,17 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_different_residues():
 
-    STREAM = open(
-        path_in_test_data(__file__, "ubi_peaks_short_different_residues.neff")
-    ).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short_different_residues.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(app, ["--file-name-template", "-"], input=STREAM)
 
     assert_lines_match(EXPECTED_DIFFERENT_RESIDUES, result.stdout)
 
 
 EXPECTED_CHAINS = """\
@@ -203,15 +200,17 @@
 
 ************************************************************************************
 """
 
 
 def test_ppm_out_short_chains():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short_chains.neff")).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short_chains.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(app, ["--file-name-template", "-"], input=STREAM)
 
     assert_lines_match(EXPECTED_CHAINS, result.stdout)
 
 
 EXPECTED_NO_CHAINS = """\
@@ -224,15 +223,17 @@
 
 ************************************************************************************
 """
 
 
 def test_ppm_out_short_no_chains():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short_chains.neff")).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short_chains.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app, ["--file-name-template", "-", "--no-chains"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_NO_CHAINS, result.stdout)
 
@@ -250,15 +251,17 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_with_data():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app, ["--file-name-template", "-", "--add-data"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_WITH_DATA, result.stdout)
 
@@ -276,15 +279,17 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_full_assignments():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app, ["--file-name-template", "-", "--full-assignments"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_FULL_ASSIGNMENTS, result.stdout)
 
@@ -302,15 +307,17 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_discard_assignments():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_peaks_short.neff")).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app, ["--file-name-template", "-", "--discard-assignments"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_NO_ASSIGNMENTS, result.stdout)
 
@@ -329,17 +336,17 @@
 
 
 """
 
 
 def test_ppm_out_short_with_full_assignments():
 
-    STREAM = open(
-        path_in_test_data(__file__, "peaks_short_with_assignments.neff")
-    ).read()
+    file_name = path_in_test_data(__file__, "peaks_short_with_assignments.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(app, ["--file-name-template", "-"], input=STREAM)
 
     assert_lines_match(EXPECTED_WITH_FULL_ASSIGNMENTS, result.stdout)
 
 
 EXPECTED_WITH_DIFFERENT_CHAIN_SEPARATOR = """\
@@ -356,17 +363,17 @@
 ************************************************************************************
 
 """
 
 
 def test_ppm_out_short_with_different_chain_separator():
 
-    STREAM = open(
-        path_in_test_data(__file__, "peaks_short_with_assignments.neff")
-    ).read()
+    file_name = path_in_test_data(__file__, "peaks_short_with_assignments.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app, ["--file-name-template", "-", "--chain-separator", "_"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_WITH_DIFFERENT_CHAIN_SEPARATOR, result.stdout)
 
@@ -385,17 +392,17 @@
 
 
 """
 
 
 def test_ppm_out_short_3d_m1():
 
-    STREAM = open(
-        path_in_test_data(__file__, "ubi_peaks_short_i_minus_one.neff")
-    ).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short_i_minus_one.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app,
         [
             "--file-name-template",
             "-",
         ],
@@ -419,30 +426,30 @@
 
 
 """
 
 
 def test_ppm_out_short_3d_m1_no_negatives():
 
-    STREAM = open(
-        path_in_test_data(__file__, "ubi_peaks_short_i_minus_one.neff")
-    ).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short_i_minus_one.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app, ["--file-name-template", "-", "--no-negative-residues"], input=STREAM
     )
 
     assert_lines_match(EXPECTED_3D_m1_no_negatives, result.stdout)
 
 
 def test_ppm_out_short_overlapped_chains():
 
-    STREAM = open(
-        path_in_test_data(__file__, "ubi_peaks_short_overlapping_chains.neff")
-    ).read()
+    file_name = path_in_test_data(__file__, "ubi_peaks_short_overlapping_chains.neff")
+    with open(file_name) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(app, ["--no-chains"], input=STREAM, expected_exit_code=1)
 
     assert "ignore chains" in result.stdout
     assert " A " in result.stdout
     assert " B " in result.stdout
     assert "66" in result.stdout
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     NOQA_E501,
     assert_lines_match,
     isolate_loop,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.sparky.importers.peaks import peaks
 
 app = typer.Typer()
 app.command()(peaks)
 
@@ -40,24 +41,22 @@
      2   2   A   17   DT   H6    A   16   DG   H8    7.205   .   8.004   .   .   .   1680000.0    .
      3   3   A   17   DT   H7    A   16   DG   H8    1.459   .   8.008   .   .   .   20900000.0   .
      4   4   A   17   DT   H2"   A   17   DT   H1'   2.509   .   5.84    .   .   .   46800000.0   .
 
 stop_
 """
 
+DATA_SEQUENCE = read_test_data("sparky_manual_basic_sequence.nef", __file__)
+
 
 def test_basic():
 
     path = path_in_test_data(__file__, "sparky_manual_basic.peaks")
 
-    data_sequence = open(
-        path_in_test_data(__file__, "sparky_manual_basic_sequence.nef")
-    ).read()
-
-    result = run_and_report(app, ["--molecule-type", "dna", path], input=data_sequence)
+    result = run_and_report(app, ["--molecule-type", "dna", path], input=DATA_SEQUENCE)
 
     loop = isolate_loop(
         result.stdout, "nef_nmr_spectrum_sparky_sparky_manual_basic", "nef_peak"
     )
 
     assert_lines_match(EXPECTED, str(loop))
 
@@ -75,19 +74,15 @@
     assert_lines_match(EXPECTED, str(loop))
 
 
 def test_basic_no_sequence_requires_sequence():
 
     path = path_in_test_data(__file__, "sparky_manual_full_no_sequence.peaks")
 
-    sequence = open(
-        path_in_test_data(__file__, "sparky_manual_basic_sequence.nef")
-    ).read()
-
-    result = run_and_report(app, [path], input=sequence)
+    result = run_and_report(app, [path], input=DATA_SEQUENCE)
 
     loop = isolate_loop(
         result.stdout,
         "nef_nmr_spectrum_sparky_sparky_manual_full_no_sequence",
         "nef_peak",
     )
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.sparky.importers.shifts import shifts
 
 SHIFTS_SPARKY = "nef_chemical_shift_list_sparky"
 
 app = typer.Typer()
@@ -60,15 +61,15 @@
     stop_
 save_
 """
 
 
 def test_ppm_out_short():
 
-    STREAM = open(path_in_test_data(__file__, "P3a_L273R_sequence_short.neff")).read()
+    STREAM = read_test_data("P3a_L273R_sequence_short.neff", __file__)
 
     path = path_in_test_data(__file__, "test_shifts_P3a_L273R_shifts_short.txt")
 
     result = run_and_report(app, [path], input=STREAM)
 
     shifts_result = isolate_frame(result.stdout, SHIFTS_SPARKY)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/oxidised_cys.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/predSS_4.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/predSS_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/predSS_4_first_resid_2.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4_chi1.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/protonated_his.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/protonated_his.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/ubi_4.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/ubi_4.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_export_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_export_shifts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.talos.exporters.shifts import shifts
 
 app = typer.Typer()
 app.command()(shifts)
 
@@ -38,17 +39,17 @@
 4               F          C           175.32
 4               F          CB           41.48
 4               F          CA           55.21
 4               F          N           118.11
 """
 
 
-def test_4peaks(clear_cache):
+def test_4peaks():
 
-    STREAM = open(path_in_test_data(__file__, "ubi_4.nef")).read()
+    STREAM = read_test_data("ubi_4.nef", __file__)
 
     result = run_and_report(app, [], input=STREAM)
 
     assert_lines_match(EXPECTED, result.stdout)
 
 
 # TODO check filtering & bad inputs
@@ -81,17 +82,17 @@
 4               F          C           175.32
 4               F          CB           41.48
 4               F          CA           55.21
 4               F          N           118.11
 """
 
 
-def test_4peak_his_he(clear_cache):
+def test_4peak_his_he():
 
-    STREAM = open(path_in_test_data(__file__, "protonated_his.nef")).read()
+    STREAM = read_test_data("protonated_his.nef", __file__)
 
     result = run_and_report(app, [], input=STREAM)
 
     assert_lines_match(EXPECTED_PROTONATED_HIS, result.stdout)
 
 
 EXPECTED_OXIDISED_CYS = """
@@ -122,17 +123,17 @@
 4               F          C           175.32
 4               F          CB           41.48
 4               F          CA           55.21
 4               F          N           118.11
 """
 
 
-def test_4peak_cis_oxidised(clear_cache):
+def test_4peak_cis_oxidised():
 
-    STREAM = open(path_in_test_data(__file__, "oxidised_cys.nef")).read()
+    STREAM = read_test_data("oxidised_cys.nef", __file__)
 
     result = run_and_report(app, [], input=STREAM)
 
     assert_lines_match(EXPECTED_OXIDISED_CYS, result.stdout)
 
 
 EXPECTED_OFFSET_1 = """
@@ -163,13 +164,14 @@
     5               F          C           175.32
     5               F          CB           41.48
     5               F          CA           55.21
     5               F          N           118.11
 """
 
 
-def test_4peaks_offset(clear_cache):
-    STREAM = open(path_in_test_data(__file__, "ubi_4_offset_1.nef")).read()
+def test_4peaks_offset():
+    with open(path_in_test_data(__file__, "ubi_4_offset_1.nef")) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(app, [], input=STREAM)
 
     assert_lines_match(EXPECTED_OFFSET_1, result.stdout)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_import_order_parameters.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_import_order_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from fyeah import f
 
 from nef_pipelines.lib.test_lib import (
     NOQA_E501,
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.talos.importers.order_parameters import order_parameters
 
 app = typer.Typer()
 app.command()(order_parameters)
 
@@ -46,20 +47,20 @@
 
 
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_ss_4(clear_cache):
+def test_ss_4():
 
     pred_4_path = path_in_test_data(__file__, "predS2_4.tab")
     pred_4_nef_path = path_in_test_data(__file__, "pred_4_seq.nef")
 
-    STREAM = open(pred_4_nef_path).read()
+    STREAM = read_test_data(pred_4_nef_path)
 
     result = run_and_report(
         app,
         [
             pred_4_path,
         ],
         input=STREAM,
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_import_restraints.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_import_restraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from fyeah import f
 
 from nef_pipelines.lib.test_lib import (
     NOQA_E501,
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.talos.importers.restraints import restraints
 
 app = typer.Typer()
 app.command()(restraints)
 
@@ -57,20 +58,20 @@
 
 save_
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_pred4tab(clear_cache):
+def test_pred4tab():
 
     pred_4_path = path_in_test_data(__file__, "pred_4.tab")
     pred_4_nef_path = path_in_test_data(__file__, "pred_4_seq.nef")
 
-    STREAM = open(pred_4_nef_path).read()
+    STREAM = read_test_data(pred_4_nef_path)
 
     result = run_and_report(
         app,
         [
             pred_4_path,
         ],
         input=STREAM,
@@ -125,20 +126,20 @@
 save_
 
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_pred4tab_chi1(clear_cache):
+def test_pred4tab_chi1():
 
     pred_4_path = path_in_test_data(__file__, "pred_4_chi1.tab")
     pred_4_nef_path = path_in_test_data(__file__, "pred_4_seq.nef")
 
-    STREAM = open(pred_4_nef_path).read()
+    STREAM = read_test_data(pred_4_nef_path)
 
     result = run_and_report(
         app,
         [
             pred_4_path,
         ],
         input=STREAM,
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/talos/test_secondary_structure.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/talos/test_secondary_structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from fyeah import f
 
 from nef_pipelines.lib.test_lib import (
     NOQA_E501,
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.talos.importers.secondary_structure import (
     secondary_structure,
 )
 
 app = typer.Typer()
@@ -40,20 +41,20 @@
 
 save_
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_ss_4(clear_cache):
+def test_ss_4():
 
     pred_4_path = path_in_test_data(__file__, "predSS_4.tab")
     pred_4_nef_path = path_in_test_data(__file__, "pred_4_seq.nef")
 
-    STREAM = open(pred_4_nef_path).read()
+    STREAM = read_test_data(pred_4_nef_path)
 
     result = run_and_report(
         app,
         [
             pred_4_path,
         ],
         input=STREAM,
@@ -90,20 +91,21 @@
 
 save_
 """.replace(
     NOQA_E501, ""
 )
 
 
-def test_ss_4_first_resid_2(clear_cache):
+def test_ss_4_first_resid_2():
 
     pred_4_path = path_in_test_data(__file__, "predSS_4_first_resid_2.tab")
     pred_4_nef_path = path_in_test_data(__file__, "pred_4_seq_first_resid_2.nef")
 
-    STREAM = open(pred_4_nef_path).read()
+    with open(pred_4_nef_path) as fh:
+        STREAM = fh.read()
 
     result = run_and_report(
         app,
         [
             pred_4_path,
         ],
         input=STREAM,
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,23 +118,25 @@
     result = read_or_create_entry_exit_error_on_bad_file(STDIN)
     assert result == Entry.from_scratch("nef")
 
 
 def test_read_or_create_entry_exit_error_on_bad_file_exception(mocker, tmp_path):
     mocker.patch("sys.exit")
     read_or_create_entry_exit_error_on_bad_file(tmp_path / "doesnt_exists.neff")
-    assert sys.exit.called_once_with(EXIT_ERROR)
+
+    sys.exit.assert_called_once_with(EXIT_ERROR)
 
 
 def test_read_or_create_entry_exit_error_on_bad_file_bad_stdin(mocker):
     mocker.patch("sys.stdin", StringIO("wibble"))
     mocker.patch("sys.exit")
 
     read_or_create_entry_exit_error_on_bad_file(STDIN)
-    assert sys.exit.called_once_with(EXIT_ERROR)
+
+    sys.exit.assert_called_once_with(EXIT_ERROR)
 
 
 def test_read_or_create_entry_exit_error_on_bad_file(mocker):
     INPUT = """
         data_test
     """
     mocker.patch("sys.stdin", StringIO(INPUT))
@@ -220,25 +222,25 @@
     """The provided input should be the text the user inputs. It support multiple lines for multiple inputs"""
     orig = sys.stdin
     sys.stdin = StringIO(target)
     yield
     sys.stdin = orig
 
 
-def test_read_entry_stdin_or_exit_empty_stdin(clear_cache):
+def test_read_entry_stdin_or_exit_empty_stdin():
     with replace_stdin(""):
         with pytest.raises(SystemExit) as pytest_wrapped_e:
             read_entry_from_stdin_or_exit()
 
     assert pytest_wrapped_e.type == SystemExit
     assert pytest_wrapped_e.value.code == 1
 
 
 @pytest.mark.skip(reason="not currently working and deprecated")
-def test_read_entry_stdin_or_exit(clear_cache):
+def test_read_entry_stdin_or_exit():
 
     EXPECTED = """\
     data_new
 
     save_nef_nmr_meta_data
        _nef_nmr_meta_data.sf_category      nef_nmr_meta_data
        _nef_nmr_meta_data.sf_framecode     nef_nmr_meta_data
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from textwrap import dedent
 
 import pytest
 from pynmrstar import Entry, Saveframe
 
 from nef_pipelines.lib.sequence_lib import (
     BadResidue,
-    chain_code_iter,
     count_residues,
     frame_to_chains,
+    get_chain_code_iter,
     get_chain_starts,
     offset_chain_residues,
     sequence_3let_to_sequence_residues,
     sequence_from_frame,
     translate_1_to_3,
 )
 from nef_pipelines.lib.structures import SequenceResidue
@@ -219,31 +219,34 @@
     for pair in zip(EXPECTED, result):
         print(pair)
 
     assert EXPECTED == result
 
 
 def test_chain_code_iter_basic():
-    result = [chain_code for chain_code in islice(chain_code_iter(), 3)]
+    chain_code_iter = get_chain_code_iter()
+    result = [chain_code for chain_code in islice(chain_code_iter, 3)]
 
     EXPECTED = list("ABC")
 
     assert EXPECTED == result
 
 
 def test_chain_code_iter_with_user():
-    result = [chain_code for chain_code in islice(chain_code_iter("DE"), 3)]
+    chain_code_iter = get_chain_code_iter("DE")
+    result = [chain_code for chain_code in islice(chain_code_iter, 3)]
 
     EXPECTED = list("DEA")
 
     assert EXPECTED == result
 
 
 def test_chain_code_iter_with_exclude():
-    result = [chain_code for chain_code in islice(chain_code_iter(exclude="BC"), 3)]
+    chain_code_iter = get_chain_code_iter(exclude="BC")
+    result = [chain_code for chain_code in islice(chain_code_iter, 3)]
 
     EXPECTED = list("ADE")
 
     assert EXPECTED == result
 
 
 def test_sequence_from_frame():
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/test_util.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typer
 from typer.testing import CliRunner
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
-    path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.xcamshift.exporters.shifts import shifts
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(shifts)
@@ -29,13 +29,13 @@
 assign  (  segid  AAAA  and  resid  3  and  resn  VAL  and  name  CA   )   71.710
 assign  (  segid  AAAA  and  resid  3  and  resn  VAL  and  name  CB   )   33.150
 assign  (  segid  AAAA  and  resid  3  and  resn  VAL  and  name  HA   )    5.020
 """
 
 
 # noinspection PyUnusedLocal
-def test_3ab(clear_cache):
+def test_3ab():
 
-    input = open(path_in_test_data(__file__, "test_agv.neff")).read()
+    input = read_test_data("test_agv.neff", __file__)
     result = run_and_report(app, ["-"], input=input)
 
     assert_lines_match(EXPECTED, result.stdout)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_data/basic.peaks` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_data/basic.peaks`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_import_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_import_peaks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     NOQA_E501,
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.xeasy.importers.peaks import peaks
 
 app = typer.Typer()
 app.command()(peaks)
 
@@ -89,15 +90,15 @@
 """.replace(
     NOQA_E501, ""
 )
 
 
 def test_basic():
 
-    data_sequence = open(path_in_test_data(__file__, "basic_sequence.nef")).read()
+    data_sequence = read_test_data("basic_sequence.nef", __file__)
     peaks_path = path_in_test_data(__file__, "basic.peaks")
 
     result = run_and_report(app, [peaks_path], input=data_sequence)
 
     loop = isolate_frame(result.stdout, "nef_nmr_spectrum_xeasy_basic")
 
     assert_lines_match(EXPECTED, str(loop))
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_import_sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_import_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_import_shifts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     isolate_frame,
     path_in_test_data,
+    read_test_data,
     run_and_report,
 )
 from nef_pipelines.transcoders.xeasy.importers.shifts import shifts
 
 SHIFTS_XEASY = "nef_chemical_shift_list_xeasy"
 
 app = typer.Typer()
@@ -38,15 +39,15 @@
 save_
 
 """
 
 
 def test_ppm_out_short():
 
-    STREAM = open(path_in_test_data(__file__, "basic_sequence.nef")).read()
+    STREAM = read_test_data("basic_sequence.nef", __file__)
 
     path = path_in_test_data(__file__, "basic_shifts.prot")
 
     result = run_and_report(app, [path], input=STREAM)
 
     shifts_result = isolate_frame(result.stdout, SHIFTS_XEASY)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     AtomLabel,
     DimensionInfo,
     NewPeak,
     Residue,
     SequenceResidue,
     ShiftData,
 )
-from nef_pipelines.lib.test_lib import path_in_test_data
+from nef_pipelines.lib.test_lib import path_in_test_data, read_test_data
 from nef_pipelines.transcoders.xeasy.xeasy_lib import (
     parse_peaks,
     parse_sequence,
     parse_shifts,
 )
 
 EXPECTED_SEQUENCE = [
@@ -29,30 +29,31 @@
         "A 8 VAL",
         "A 9 THR",
     ]
 ]
 
 
 def test_sequence_basic():
-    sequence = open(path_in_test_data(__file__, "basic.seq")).readlines()
+    sequence = read_test_data("basic.seq", __file__).split("\n")
 
     result = parse_sequence(sequence)
     assert result == EXPECTED_SEQUENCE
 
 
 def test_sequence_basic_commented():
-    sequence = open(path_in_test_data(__file__, "basic.seq")).readlines()
+    sequence = read_test_data("basic.seq", __file__).split("\n")
     sequence = ["#a comment", *sequence]
 
     result = parse_sequence(sequence)
     assert result == EXPECTED_SEQUENCE
 
 
 def test_sequence_basic_commented_two_lines_bad():
-    sequence = open(path_in_test_data(__file__, "basic.seq")).readlines()
+    with open(path_in_test_data(__file__, "basic.seq")) as fh:
+        sequence = fh.readlines()
 
     with pytest.raises(SystemExit) as e:
         sequence = ["#a comment", "# a bad comment", *sequence]
         parse_sequence(sequence)
 
     assert e.type == SystemExit
     assert e.value.code == 1
@@ -228,15 +229,16 @@
         volume_uncertainty=0.0,
         comment="MAP    405",
     ),
 ]
 
 
 def test_basic_peaks():
-    peaks = open(path_in_test_data(__file__, "basic.peaks")).readlines()
+    with open(path_in_test_data(__file__, "basic.peaks")) as fh:
+        peaks = fh.readlines()
 
     lookup = sequence_to_residue_name_lookup(EXPECTED_SEQUENCE)
     spectrum_type, dimension_info, peaks = parse_peaks(
         peaks, source="unknown", residue_name_lookup=lookup
     )
 
     assert spectrum_type == "N15TOCSY"
@@ -343,13 +345,14 @@
         line_width_uncertainty=None,
     ),
 ]
 
 
 def test_basic_shifts():
 
-    shifts = open(path_in_test_data(__file__, "basic_shifts.prot")).readlines()
+    with open(path_in_test_data(__file__, "basic_shifts.prot")) as fh:
+        shifts = fh.readlines()
 
     lookup = sequence_to_residue_name_lookup(EXPECTED_SEQUENCE)
     shifts = parse_shifts(shifts, source="unknown", residue_lookup=lookup)
 
     assert shifts == EXPECTED_SHIFTS
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 
 # noinspection PyUnusedLocal
 def test_2_dihedrals():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     dihedrals_path = path_in_test_data(__file__, "test_2_dihedrals.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [dihedrals_path]
     result = run_and_report(app, args, input=nef_sequence)
 
     EXPECTED = """\
         save_nef_dihedral_restraint_list_test_2_dihedrals                               # noqa: E501
             _nef_dihedral_restraint_list.sf_category     nef_dihedral_restraint_list
@@ -70,28 +71,30 @@
     assert_lines_match(EXPECTED, result)
 
 
 def test_2_dihedrals_bad():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     dihedrals_path = path_in_test_data(__file__, "test_2_dihedrals_bad.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [dihedrals_path]
     result = run_and_report(app, args, input=nef_sequence, expected_exit_code=1)
 
     assert "ERROR" in result.stdout
     assert "failed to read dihedral restraints" in result.stdout
 
 
 def test_2_dihedrals_no_segids():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     dihedrals_path = path_in_test_data(__file__, "test_2_dihedrals_no_segids.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [dihedrals_path, "--chains", "AAAA"]
     result = run_and_report(app, args, input=nef_sequence)
 
     EXPECTED = """\
         save_nef_dihedral_restraint_list_test_2_dihedrals_no_segids                              # noqa: E501
             _nef_dihedral_restraint_list.sf_category     nef_dihedral_restraint_list
@@ -139,15 +142,16 @@
     assert_lines_match(EXPECTED, result)
 
 
 def test_2_dihedrals_overriding_segids():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     dihedrals_path = path_in_test_data(__file__, "test_2_dihedrals.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [dihedrals_path, "--chains", "BBBB", "--use-chains"]
     result = run_and_report(app, args, input=nef_sequence)
 
     EXPECTED = """\
         save_nef_dihedral_restraint_list_test_2_dihedrals                                     # noqa: E501
             _nef_dihedral_restraint_list.sf_category     nef_dihedral_restraint_list
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 
 # noinspection PyUnusedLocal
 def test_2_distances():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     dihedrals_path = path_in_test_data(__file__, "test_2_distances.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [dihedrals_path]
     result = run_and_report(app, args, input=nef_sequence)
 
     EXPECTED = """\
         save_nef_distance_restraint_list_test_2_distances                               # noqa: E501
             _nef_distance_restraint_list.sf_category     nef_distance_restraint_list
@@ -61,28 +62,30 @@
     assert_lines_match(EXPECTED, result)
 
 
 def test_2_distances_bad():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     distances_path = path_in_test_data(__file__, "test_2_distances_bad.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [distances_path]
     result = run_and_report(app, args, input=nef_sequence, expected_exit_code=1)
 
     assert "ERROR" in result.stdout
     assert "failed to read distance restraints" in result.stdout
 
 
 def test_2_dihstances_no_segids():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     distances_path = path_in_test_data(__file__, "test_2_distances_no_segids.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [distances_path, "--chains", "AAAA"]
     result = run_and_report(app, args, input=nef_sequence)
 
     EXPECTED = """\
         save_nef_distance_restraint_list_test_2_distances_no_segids                               # noqa: E501
             _nef_distance_restraint_list.sf_category     nef_distance_restraint_list
@@ -121,15 +124,16 @@
     assert_lines_match(EXPECTED, result)
 
 
 def test_2_distances_overriding_segids():
     sequence_path = path_in_test_data(__file__, "3a_ab.neff")
     distances_path = path_in_test_data(__file__, "test_2_distances.tbl")
 
-    nef_sequence = open(sequence_path, "r").read()
+    with open(sequence_path, "r") as fh:
+        nef_sequence = fh.read()
 
     args = [distances_path, "--chains", "BBBB", "--use-chains"]
     result = run_and_report(app, args, input=nef_sequence)
 
     EXPECTED = """\
         save_nef_distance_restraint_list_test_2_distances                               # noqa: E501
             _nef_distance_restraint_list.sf_category     nef_distance_restraint_list
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,13 +40,15 @@
         (  segid  AAAA  and  resid  3   and  resname  ALA  and  name  HA    )
         (  segid  AAAA  and  resid  3   and  resname  ALA  and  name  HN    )    6.700   1.000
 
 """
 
 
 # noinspection PyUnusedLocal
-def test_3ab(clear_cache):
+def test_3ab():
+
+    with open(path_in_test_data(__file__, "3a_ab_rdcs.neff")) as fh:
+        input = fh.read()
 
-    input = open(path_in_test_data(__file__, "3a_ab_rdcs.neff")).read()
     result = run_and_report(app, [], input=input)
 
     assert_lines_match(EXPECTED, result.stdout)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 
    stop_
 
 save_"""
 
 
 # noinspection PyUnusedLocal
-def test_3ab(clear_cache):
+def test_3ab():
 
     path = path_in_test_data(__file__, "3a_ab.psf")
     result = run_and_report(app, [path])
 
     result = isolate_frame(result.stdout, "%s" % NEF_MOLECULAR_SYSTEM)
 
     assert_lines_match(EXPECTED_3A_AB, result)
 
 
-def test_no_sequence_files(clear_cache):
+def test_no_sequence_files():
 
     result = run_and_report(app, [], expected_exit_code=1)
 
     assert "no psf files provided to read sequences from" in result.stdout
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from nef_pipelines.lib.structures import SequenceResidue
-from nef_pipelines.lib.test_lib import path_in_test_data
+from nef_pipelines.lib.test_lib import read_test_data
 from nef_pipelines.transcoders.xplor.psf_lib import PSFParseException, parse_xplor_PSF
 
-A3_AB_PSF = open(path_in_test_data(__file__, "3a_ab.psf")).read()
+A3_AB_PSF = read_test_data("3a_ab.psf", __file__)
 
 
 def test_parse_3a_ab():
     result = parse_xplor_PSF(A3_AB_PSF)
 
     assert len(result) == 6
 
@@ -22,43 +22,43 @@
             SequenceResidue(chain_code="BBBB", sequence_code=13, residue_name="ALA"),
         ]
     )
 
     assert EXPECTED == result
 
 
-EMPTY_PSF = open(path_in_test_data(__file__, "empty.psf")).read()
+EMPTY_PSF = read_test_data("empty.psf", __file__)
 
 
 def test_parse_empty():
     with pytest.raises(PSFParseException) as excinfo:
         parse_xplor_PSF(EMPTY_PSF, "test-empty-file.psf")
 
     exception_message = excinfo.value.args[0]
 
     print(exception_message)
 
     assert "test-empty-file.psf" in exception_message
     assert "the first line of a PSF file should be 'PSF'" in exception_message
 
 
-BAD_NATOM_FIELDS_PSF = open(path_in_test_data(__file__, "bad_natom.psf")).read()
+BAD_NATOM_FIELDS_PSF = read_test_data("bad_natom.psf", __file__)
 
 
 def test_parse_bad_natom():
     with pytest.raises(PSFParseException) as excinfo:
         parse_xplor_PSF(BAD_NATOM_FIELDS_PSF, "bad_natom.psf")
 
     exception_message = excinfo.value.args[0]
 
     assert "bad_natom.psf" in exception_message
     assert "can't convert natom to an int" in exception_message
 
 
-BAD_HEADER_PSF = open(path_in_test_data(__file__, "bad_header.psf")).read()
+BAD_HEADER_PSF = read_test_data("bad_header.psf", __file__)
 
 
 def test_parse_bad_header():
     with pytest.raises(PSFParseException) as excinfo:
         parse_xplor_PSF(BAD_HEADER_PSF, "bad_header.psf")
 
     exception_message = excinfo.value.args[0]
@@ -66,43 +66,43 @@
     assert "bad_header.psf" in exception_message
     assert (
         "the first line of a PSF file should be 'PSF' i got 'WIBBLE' "
         in exception_message
     )
 
 
-BAD_FIELD_COUNT = open(path_in_test_data(__file__, "bad_field_count.psf")).read()
+BAD_FIELD_COUNT = read_test_data("bad_field_count.psf", __file__)
 
 
 def test_parse_bad_field_count():
     with pytest.raises(PSFParseException) as excinfo:
         parse_xplor_PSF(BAD_FIELD_COUNT, "bad_field_count.psf")
 
     exception_message = excinfo.value.args[0]
 
     assert "8 fields" in exception_message
     assert "atom number 1" in exception_message
     assert "expected 9" in exception_message
 
 
-BAD_RESID_FIELD = open(path_in_test_data(__file__, "bad_residue_number.psf")).read()
+BAD_RESID_FIELD = read_test_data("bad_residue_number.psf", __file__)
 
 
 def test_parse_bad_resid():
     with pytest.raises(PSFParseException) as excinfo:
         parse_xplor_PSF(BAD_RESID_FIELD, "bad_residue_number.psf")
 
     exception_message = excinfo.value.args[0]
 
     assert "bad_residue_number" in exception_message
     assert "couldn't convert" in exception_message
     assert "ZZZ" in exception_message
 
 
-NO_RESIDUES_FOUND = open(path_in_test_data(__file__, "no_residues_found.psf")).read()
+NO_RESIDUES_FOUND = read_test_data("no_residues_found.psf", __file__)
 
 
 def test_parse_no_residues_found():
     with pytest.raises(PSFParseException) as excinfo:
         parse_xplor_PSF(NO_RESIDUES_FOUND, "no_residues_found.psf")
 
     exception_message = excinfo.value.args[0]
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,17 +114,16 @@
     assert result.get("angle") == 4.567
     assert result.get("range") == 7.8910
     assert result.get("exponent") == 2
 
 
 def test_read_multiple_dihedral_restraints():
 
-    TEST_DATA = open(path_in_test_data(__file__, "test_2_dihedrals.tbl")).read()
-
-    # print(TEST_DATA)
+    with open(path_in_test_data(__file__, "test_2_dihedrals.tbl")) as fh:
+        TEST_DATA = fh.read()
 
     result = _dihedral_restraints.ignore(XPLOR_COMMENT).parseString(TEST_DATA)
 
     assert len(result) == 2
 
     print(result[0].as_list())
     assert result[0].as_list() == [
@@ -196,15 +195,16 @@
         120.7,
         2,
     ]
 
 
 def test_read_3_dihedral_restraints_incomplete():
 
-    TEST_DATA = open(path_in_test_data(__file__, "test_2_dihedrals.tbl")).read()
+    with open(path_in_test_data(__file__, "test_2_dihedrals.tbl")) as fh:
+        TEST_DATA = fh.read()
 
     TEST_DATA = f"""\
         {TEST_DATA}
         assign (
     """
 
     with pytest.raises(ParseException) as e_info:
@@ -213,15 +213,16 @@
         )
 
     assert "Expected end of text, found 'assign'" in str(e_info.value)
 
 
 def test_read_multiple_noe_restraints():
 
-    TEST_DATA = open(path_in_test_data(__file__, "test_2_noes.tbl")).read()
+    with open(path_in_test_data(__file__, "test_2_noes.tbl")) as fh:
+        TEST_DATA = fh.read()
 
     result = _distance_restraints.ignore(XPLOR_COMMENT).parseString(TEST_DATA)
 
     assert len(result) == 2
 
     assert result[0].as_list() == [
         [
@@ -334,15 +335,16 @@
         "]]"
     )
 
 
 def test_get_approximate_restraint():
     dihedrals_path = path_in_test_data(__file__, "test_2_dihedrals.tbl")
 
-    dihdedral_restraints = open(dihedrals_path, "r").read()
+    with open(dihedrals_path, "r") as fh:
+        dihdedral_restraints = fh.read()
 
     result = _get_approximate_restraint_strings(dihdedral_restraints)
 
     EXPECTED = [
         """# noqa: E501 \
            assign  (segid AAAA and resid    1 and name C    ) (segid AAAA and resid    2 and name N    )
                    (segid AAAA and resid    2 and name CA   ) (segid AAAA and resid    2 and name C    )    1.0 -45.7   120.5 2
@@ -363,15 +365,16 @@
 
         assert reported == expected
 
 
 def test_get_single_atom_selection_dihderal_restraint():
     dihedrals_path = path_in_test_data(__file__, "test_2_dihedrals.tbl")
 
-    dihdedral_restraints = open(dihedrals_path, "r").read()
+    with open(dihedrals_path, "r") as fh:
+        dihdedral_restraints = fh.read()
 
     xplor_basic_restraints = _dihedral_restraints.ignore(XPLOR_COMMENT).parseString(
         dihdedral_restraints
     )
 
     restraint = xplor_basic_restraints[0].get("atoms_1")[0]
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/clone.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List
 
 import typer
 from pynmrstar import Entry
 from typer import Argument, Option
 
 from nef_pipelines.lib.sequence_lib import (
-    chain_code_iter,
     frame_to_chains,
+    get_chain_code_iter,
     sequence_from_frame,
     sequence_to_nef_frame,
 )
 from nef_pipelines.lib.util import (
     exit_error,
     get_pipe_file_or_exit,
     parse_comma_separated_options,
@@ -63,16 +63,17 @@
     # this should come from a sequence not a frame...
     existing_chain_codes = frame_to_chains(molecular_system)
 
     if target not in existing_chain_codes:
         exit_error(
             f"couldn't find target chain {target} in {', '.join(existing_chain_codes)}"
         )
-
-    useable_chain_codes = chain_code_iter(chain_codes, [target, *existing_chain_codes])
+    useable_chain_codes = get_chain_code_iter(
+        chain_codes, [target, *existing_chain_codes]
+    )
     new_chain_codes = islice(useable_chain_codes, count)
 
     target_residues = [residue for residue in sequence if residue.chain_code == target]
 
     for new_chain_code in new_chain_codes:
         for residue in target_residues:
             new_residue = replace(residue, chain_code=new_chain_code)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/rename.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     new = new_old[1]
 
     entry = read_entry_from_file_or_stdin_or_exit_error(input)
 
     changes = 0
     changed_frames = OrderedSet()
 
-    frames_to_process = select_frames(entry, selector_type, frame_selectors)
+    frames_to_process = select_frames(entry, frame_selectors, selector_type)
 
     for save_frame in frames_to_process:
         for loop in save_frame.loop_iterator():
             for tag in loop.get_tag_names():
                 tag_parts = tag.split(".")
                 if tag_parts[-1].startswith("chain_code"):
                     tag_values = loop[tag]
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/chains/renumber.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         exit_if_molecular_system_isnt_a_singleton(molecular_system_frames)
 
         molecular_system = molecular_system_frames[0]
 
         chain_offsets = chain_starts_to_offsets(molecular_system, chain_offsets)
 
-    frames = select_frames(entry, selector_type, frame_selectors)
+    frames = select_frames(entry, frame_selectors, selector_type)
 
     offset_chains_in_frames(frames, chain_offsets, starts)
 
     print(entry)
 
     # # get_help()
     #
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/filter.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/filter.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             import hashlib
 
             md5 = hashlib.md5(lines.encode("ascii")).hexdigest()
             num_lines = len(lines.split("\n"))
             print(f"    lines: {num_lines} frames: {len(entry)} checksum: {md5} [md5]")
         print()
 
-        frames = select_frames(entry, selector_type, filters)
+        frames = select_frames(entry, filters, selector_type)
 
         if verbose == 0:
             frame_names = [frame.name for frame in frames]
             if number:
                 frame_names = [
                     f"{i}. {frame_name}"
                     for i, frame_name in enumerate(frame_names, start=1)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/frames/unassign.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/frames/unassign.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             chain mappings were: {chain_mappings_msg}
         """
 
         exit_error(msg)
 
     frame_selectors = {
         (frame.category, frame.name)
-        for frame in select_frames(entry, selector_type, frame_selectors)
+        for frame in select_frames(entry, frame_selectors, selector_type)
     }
 
     entry = pipe(entry, frame_selectors, targets, sequence_mode, chain_mappings)
 
     print(entry)
 
 
@@ -461,17 +461,17 @@
                                 used_sequence_code, string.ascii_letters + "@#"
                             )
 
                             new_sequence_code = f"{prefix}PR_{i}{sequence_code}"
                             if new_sequence_code in sequence_code_map:
                                 continue
 
-                            possible_new_sequence_codes[
-                                used_sequence_code
-                            ] = new_sequence_code
+                            possible_new_sequence_codes[used_sequence_code] = (
+                                new_sequence_code
+                            )
                             break
 
                 sequence_code_map.update(possible_new_sequence_codes)
 
         for assignment, new_assignment in assignment_map.items():
 
             old_sequence_code = str(new_assignment.residue.sequence_code)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/simulate/peaks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import Counter
 from dataclasses import replace
 from pathlib import Path
 from textwrap import dedent, indent
 from typing import List
 
 import typer
 from fyeah import f
@@ -18,31 +19,31 @@
 )
 from nef_pipelines.lib.peak_lib import peaks_to_frame
 from nef_pipelines.lib.shift_lib import nef_frames_to_shifts
 from nef_pipelines.lib.spectra_lib import (
     EXPERIMENT_CLASSIFICATION_TO_SYNONYM,
     EXPERIMENT_GROUPS,
     EXPERIMENT_INFO,
+    FAKE_SPECTROMETER_FREQUENCY_600,
     SPECTRUM_TYPE_TO_CLASSIFICATION,
     ExperimentType,
     PeakInfo,
 )
 from nef_pipelines.lib.structures import NewPeak, ShiftData
 from nef_pipelines.lib.util import (
     FOUR_SPACES,
     STDIN,
     exit_error,
     flatten,
     is_int,
     parse_comma_separated_options,
     strings_to_tabulated_terminal_sensitive,
 )
-from nef_pipelines.tools.shifts import shifts_app
+from nef_pipelines.tools.simulate import simulate_app
 
-FAKE_SPECTROMETER_FREQUENCY_600 = 600.12345678
 SPECTRUM_NAME_TEMPLATE = "synthetic_{spectrum}"
 
 SHIFT_FRAMES_HELP = """\
     the names of the shift frames to use, this can be a comma separated list of name or the option can be called
     called multiple times. Wild cards are allowed. If no match is found wild cards are checked as well unless
     --exact is set
 """
@@ -52,36 +53,42 @@
     called multiple times. Possible values are: {', '.join(ExperimentType)}
 """
 NAME_TEMPLATE_HELP = """
     the name template for the new peak lists the placeholder {spectrum} will get replaced with the spectrum type
 """
 
 
-@shifts_app.command()
-def make_peaks(
+@simulate_app.command()
+def peaks(
     shift_frame_selectors: List[str] = typer.Option(
         None, "--shift-frames", help=SHIFT_FRAMES_HELP
     ),
     exact: bool = typer.Option(
         False, help="if set frames are selected by exact matches"
     ),
-    spectra: List[str] = typer.Option([ExperimentType.N_HSQC], help=SPECTRA_HELP),
     name_template: str = typer.Option(SPECTRUM_NAME_TEMPLATE, help=NAME_TEMPLATE_HELP),
     spectrometer_frequency: float = typer.Option(FAKE_SPECTROMETER_FREQUENCY_600),
     input: Path = typer.Option(
         STDIN,
         "--in",
         "-i",
         metavar="|INPUT|",
         help="input to read NEF data from [stdin = -]",
     ),
+    spectra: List[str] = typer.Argument(None, help=SPECTRA_HELP),
 ):
     """-  make a set of peaks for an hsqc, 13C direct detect or triple resonance spectrum from a list of shifts
     [alpha for non cpn peak lists and 13C detect]"""
 
+    spectra = [spectrum.replace("-", "_") for spectrum in spectra]
+    if not spectra:
+        spectra = [
+            ExperimentType.N_HSQC,
+        ]
+
     shift_frame_selectors = (
         [
             "*",
         ]
         if not shift_frame_selectors
         else parse_comma_separated_options(shift_frame_selectors)
     )
@@ -111,19 +118,37 @@
     for spectum in spectra:
 
         found = False
         if spectum in spectrum_names:
             result.append(ExperimentType[spectum])
             found = True
 
+        experiment_types_upper = [
+            experiment_type.name.upper() for experiment_type in ExperimentType
+        ]
+        upper_experiments_to_experiments = {
+            experiment_type.name.upper(): experiment_type
+            for experiment_type in ExperimentType
+        }
+        counts = Counter(experiment_types_upper)
+
         if not found:
-            spectrum_lower = spectum.lower()
-            if spectrum_lower in spectrum_names:
-                result.append(ExperimentType[spectrum_lower])
+            spectrum_upper = spectum.upper()
+            if spectrum_upper in experiment_types_upper and counts[spectrum_upper] == 1:
+                result.append(upper_experiments_to_experiments[spectrum_upper])
                 found = True
+            if spectrum_upper in experiment_types_upper and counts[spectrum_upper] > 1:
+                degenerate_spectra = [
+                    experiment_type.name
+                    for experiment_type in ExperimentType
+                    if experiment_type.upper() == spectrum_upper
+                ]
+                _exit_degnerate_spectrum_type(
+                    spectum, list(ExperimentType), degenerate_spectra
+                )
 
         if not found:
             _exit_bad_spectrum_type(spectum, list(ExperimentType))
 
     return result
 
 
@@ -151,14 +176,30 @@
     msg = dedent(msg)
 
     spectrum_types = strings_to_tabulated_terminal_sensitive(known_spectra)
     spectrum_types = indent(spectrum_types, FOUR_SPACES)
 
     exit_error(f(msg))
 
+
+def _exit_degnerate_spectrum_type(spectrum, known_spectra, degenerate_spectra):
+    degenerate_spectra = ", ".join(degenerate_spectra)
+    msg = """
+            the spectrum type {spectrum} doesn't exactly match a spectrum type in the list below
+            and has more than possible match when case is ignored [{degenerate_spectra}]
+
+            {spectrum_types}
+        """
+    msg = dedent(msg)
+
+    spectrum_types = strings_to_tabulated_terminal_sensitive(known_spectra)
+    spectrum_types = indent(spectrum_types, FOUR_SPACES)
+
+    exit_error(f(msg))
+
 
 def pipe(
     entry: Entry,
     shift_frame_selectors: List[str],
     exact_frame_selectors: bool,
     spectra: List[ExperimentType],
     name_template_string: str,
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.66/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/importers/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import sys
 from pathlib import Path
 from typing import Dict, List
 
 import typer
 
 from nef_pipelines.lib.nef_lib import (
@@ -11,15 +12,15 @@
 from nef_pipelines.lib.sequence_lib import (
     make_chunked_sequence_1let,
     sequence_from_frame,
     sequence_to_chains,
     translate_3_to_1,
 )
 from nef_pipelines.lib.structures import SequenceResidue
-from nef_pipelines.lib.util import STDOUT
+from nef_pipelines.lib.util import STDIN, STDOUT, exit_error
 from nef_pipelines.transcoders.fasta import export_app
 
 # TODO: we should be able to output *s on the ends of sequences and comments
 # TODO: we should be able to select chains by fnmatch
 
 CHAIN_CODES_HELP = """
     chains to export, to add multiple chains use repeated calls, to select all chains use * [default: 'A']
@@ -33,59 +34,75 @@
         [],
         "-c",
         "--chain_code",
         help=CHAIN_CODES_HELP,
         metavar="<CHAIN-CODE>",
     ),
     in_file: Path = typer.Option(
-        None, "-i", "--in", help="file to read nef data from", metavar="<NEF-FILE>"
+        STDIN, "-i", "--in", help="file to read nef data from", metavar="<NEF-FILE>"
     ),
     output_file: str = typer.Argument(
         None,
         help="file name to output to [default <entry_id>.fasta] for stdout use -",
         metavar="<FASTA-SEQUENCE-FILE>",
     ),
 ):
     """- convert nef sequence to fasta"""
 
     chain_codes = ["*"] if len(chain_codes) == 0 else chain_codes
 
     entry = read_entry_from_file_or_stdin_or_exit_error(in_file)
 
     output_file = f"{entry.entry_id}.fasta" if output_file is None else output_file
+    output_file = STDOUT if output_file == "-" else output_file
+
+    entry = pipe(entry, chain_codes, output_file)
+
+    if entry:
+        print(entry)
+
+
+def pipe(entry, chain_codes, output_file):
 
     fasta_records = fasta_records_from_entry(entry, chain_codes)
 
     # TODO: move to utility function and use in all outputs
-    file_h = sys.stdout if output_file == str(STDOUT) else open(output_file, "w")
+    try:
+        file_h = sys.stdout if output_file == STDOUT else open(output_file, "w")
+    except Exception as e:
+        msg = (
+            f"Error opening output file {output_file} for writing fasa file because {e}"
+        )
+        exit_error(msg, e)
 
-    # TODO we ought to output to multiple files witha template
+    # TODO we ought to be able to output to multiple files with a filename template
+    records = []
     for record in fasta_records.values():
-        print("\n\n".join(record), file=file_h)
+        records.append("\n".join(record))
+    print("\n\n".join(records), file=file_h)
 
     if output_file != STDOUT:
         file_h.close()
 
-        if not sys.stdout.isatty():
-            print(entry)
+    return entry if output_file != STDOUT else None
 
 
 def fasta_records_from_entry(entry, chain_codes):
 
     molecular_system = molecular_system_from_entry_or_exit(entry)
 
     residues = sequence_from_frame(molecular_system)
 
-    fasta_records = nef_to_fasta_records(residues, chain_codes)
+    fasta_records = nef_to_fasta_records(residues, chain_codes, entry.entry_id)
 
     return fasta_records
 
 
 def nef_to_fasta_records(
-    residues: List[SequenceResidue], target_chain_codes: List[str]
+    residues: List[SequenceResidue], target_chain_codes: List[str], entry_id: str
 ) -> Dict[str, List[str]]:
 
     all_chain_codes = sequence_to_chains(residues)
 
     chain_codes = []
     for target_chain_code in target_chain_codes:
         for chain_code in all_chain_codes:
@@ -119,13 +136,14 @@
     residue_sequences = {
         chain: make_chunked_sequence_1let(residue_sequence)
         for chain, residue_sequence in residue_sequences.items()
     }
 
     result = {}
     for chain_code, residue_sequence in residue_sequences.items():
+        entry_id = re.sub(r"\s+", "", entry_id)
         result[chain_code] = [
-            f">CHAIN: {chain_code} | START RESIDUE: {chain_starts[chain_code]}",
+            f">{entry_id} NEFPLS | CHAIN: {chain_code} | START: {chain_starts[chain_code]}",
             "\n".join(residue_sequence),
         ]
 
     return result
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 from itertools import chain, cycle, islice, zip_longest
 from pathlib import Path
-from typing import Iterable, List
+from typing import List
 
 import typer
-from fastaparser import Reader
 from ordered_set import OrderedSet
+from pynmrstar import Entry
 
+from nef_pipelines.lib.nef_lib import read_or_create_entry_exit_error_on_bad_file
 from nef_pipelines.lib.sequence_lib import (
-    BadResidue,
     MoleculeType,
-    MoleculeTypes,
-    chain_code_iter,
+    get_chain_code_iter,
     offset_chain_residues,
     sequence_3let_to_res,
     sequence_to_nef_frame,
     translate_1_to_3,
 )
 from nef_pipelines.lib.structures import SequenceResidue
-from nef_pipelines.lib.typer_utils import get_args
-from nef_pipelines.lib.util import (
-    STDIN,
-    exit_error,
-    parse_comma_separated_options,
-    process_stream_and_add_frames,
-)
-from nef_pipelines.transcoders.fasta import import_app
+from nef_pipelines.lib.util import STDIN, exit_error, parse_comma_separated_options
+from nef_pipelines.transcoders.sparky import import_app
 
 app = typer.Typer()
 
 NO_CHAIN_START_HELP = """don't include the start chain link type on a chain for the first residue [linkage will be
                          middle] for the named chains. Either use a comma joined list of chains [e.g. A,B] or call this
                          option multiple times to set chain starts for multiple chains"""
 NO_CHAIN_END_HELP = """don't include the end chain link type on a chain for the last residue [linkage will be
@@ -38,15 +31,15 @@
 
 # todo add comment to other sequences etc
 @import_app.command()
 def sequence(
     chain_codes: List[str] = typer.Option(
         [],
         "--chains",
-        help="chain codes to use for the imported chains, can be a a comma separated list or can be called "
+        help="chain codes to use for the imported chains, can be a a comma sepatared list or can be called "
         "multiple times",
         metavar="<CHAIN-CODES>",
     ),
     starts: List[str] = typer.Option(
         [],
         "--starts",
         help="first residue number of sequences can be a comma separated list or ",
@@ -54,34 +47,34 @@
     ),
     no_chain_starts: List[str] = typer.Option(
         [], "--no-chain-start", help=NO_CHAIN_START_HELP
     ),
     no_chain_ends: List[str] = typer.Option(
         [], "--no-chain-end", help=NO_CHAIN_END_HELP
     ),
-    # TODO: unused inputs!
-    entry_name: str = typer.Option("fasta", help="a name for the entry if required"),
+    entry_name: str = typer.Option("sparky", help="a name for the entry if required"),
     input: Path = typer.Option(
         STDIN,
         "-i",
         "--in",
+        metavar="|PIPE|",
         help="pipe to read NEF data from, for testing [overrides stdin !use stdin instead!]",
     ),
     molecule_types: List[MoleculeType] = typer.Option(
         [
             MoleculeType.PROTEIN,
         ],
         "--molecule-type",
         help="molecule type",
     ),
     file_names: List[Path] = typer.Argument(
-        ..., help="the file to read", metavar="<FASTA-FILE>"
+        ..., help="the file to read", metavar="<SPARKY-SEQUENCE-FILE>"
     ),
 ):
-    """- convert fasta sequence to nef"""
+    """- convert sparky sequences to nef"""
 
     chain_codes = parse_comma_separated_options(chain_codes)
     if not chain_codes:
         chain_codes = ["A"]
 
     no_chain_starts = parse_comma_separated_options(no_chain_starts)
     if not no_chain_starts:
@@ -97,49 +90,98 @@
 
     molecule_types = parse_comma_separated_options(molecule_types)
     if not molecule_types:
         molecule_types = [
             MoleculeType.PROTEIN,
         ]
 
-    args = get_args()
+    entry = read_or_create_entry_exit_error_on_bad_file(input, entry_name)
 
-    args.chain_codes = chain_codes
-    args.no_chain_starts = no_chain_starts
-    args.no_chain_ends = no_chain_ends
-    args.starts = starts
-    args.molecule_types = molecule_types
+    entry = pipe(
+        entry,
+        file_names,
+        chain_codes,
+        starts,
+        no_chain_starts,
+        no_chain_ends,
+        molecule_types,
+    )
 
-    # TODO: doesn't provide a pipe command
-    process_sequences(args)
+    print(entry)
 
 
-def process_sequences(args):
-    fasta_frames = []
+def pipe(
+    entry: Entry,
+    file_names: List[Path],
+    chain_codes: List[str],
+    starts: List[int],
+    no_chain_starts: List[bool],
+    no_chain_ends: List[bool],
+    molecule_types: List[MoleculeType],
+):
+    chain_code_iterator = get_chain_code_iter(chain_codes)
 
-    chain_code_iterator = chain_code_iter(args.chain_codes)
-    fasta_sequences = OrderedSet()
-    for file_path in args.file_names:
-        fasta_sequences.update(
-            read_sequences(file_path, chain_code_iterator, args.molecule_types)
-        )
+    chain_offsets = {}
+    chains_with_no_start = set()
+    chains_with_no_end = set()
 
-    read_chain_codes = residues_to_chain_codes(fasta_sequences)
+    sparky_sequences = set()
 
-    offsets = _get_sequence_offsets(read_chain_codes, args.starts)
+    for (
+        file_name,
+        chain_code,
+        molecule_type,
+        start,
+        no_chain_start,
+        no_chain_end,
+    ) in zip_longest(
+        file_names,
+        chain_code_iterator,
+        molecule_types,
+        starts,
+        no_chain_starts,
+        no_chain_ends,
+    ):
 
-    fasta_sequences = offset_chain_residues(fasta_sequences, offsets)
+        if file_name is None:
+            break
 
-    fasta_sequences = sorted(fasta_sequences)
+        if molecule_type is None:
+            molecule_type = MoleculeType.PROTEIN
 
-    fasta_frames.append(sequence_to_nef_frame(fasta_sequences))
+        if start is None:
+            start = 1
 
-    entry = process_stream_and_add_frames(fasta_frames, args)
+        if no_chain_start is None:
+            no_chain_start = False
 
-    print(entry)
+        if no_chain_end is None:
+            no_chain_start = False
+
+        if no_chain_start:
+            chains_with_no_start.add(chain)
+
+        if no_chain_end:
+            chains_with_no_end.add(chain)
+
+        chain_offsets[chain_code] = start
+
+        sparky_sequences.update(read_sequence(file_name, chain_code, molecule_type))
+
+    sparky_sequences = sorted(sparky_sequences)
+
+    sparky_sequences = offset_chain_residues(sparky_sequences, chain_offsets)
+
+    sparky_frame = sequence_to_nef_frame(
+        sparky_sequences, no_chain_starts, no_chain_ends
+    )
+
+    entry.add_saveframe(sparky_frame)
+
+    return entry
 
 
 def _get_sequence_offsets(chain_codes: List[str], starts: List[int]):
 
     offsets = [start - 1 for start in starts]
     cycle_starts = chain(
         offsets,
@@ -156,52 +198,26 @@
 
 def residues_to_chain_codes(residues: List[SequenceResidue]) -> List[str]:
     return list(OrderedSet([residue.chain_code for residue in residues]))
 
 
 # could do with taking a list of offsets
 # noinspection PyUnusedLocal
-def read_sequences(
-    path: Path, chain_codes: Iterable[str], molecule_types: List[MoleculeType]
+def read_sequence(
+    file_name: Path, chain_code: str, molecule_type: MoleculeType
 ) -> List[SequenceResidue]:
 
-    residues = OrderedSet()
     try:
-        with open(path) as handle:
+        with open(file_name) as handle:
             try:
-                reader = Reader(handle)
-                sequences = [sequence for sequence in reader]
+                sequence = "".join(handle.readlines())
+                sequence = "".join(sequence.split())
             except Exception as e:
-                # check if relative to os.getcwd
-                exit_error(f"Error reading fasta file {str(path)}", e)
-
-            number_sequences = len(sequences)
-
-            # read as many chain codes as there are sequences
-            # https://stackoverflow.com/questions/16188270/get-a-fixed-number-of-items-from-a-generator
-
-            chain_codes = list(islice(chain_codes, number_sequences))
-
-            for sequence, chain_code, molecule_type in zip_longest(
-                sequences, chain_codes, molecule_types, fillvalue=None
-            ):
-                if molecule_type is None:
-                    molecule_type = MoleculeTypes.PROTEIN
-
-                sequence = [letter_code.letter_code for letter_code in sequence]
-                try:
-                    sequence_3_let = translate_1_to_3(
-                        sequence, molecule_type=molecule_type
-                    )
-                except BadResidue as e:
-                    exit_error(
-                        f"Error translating sequence {sequence} to 3 letter code {e}",
-                        e,
-                    )
-                chain_residues = sequence_3let_to_res(sequence_3_let, chain_code)
+                exit_error(f"Error reading sparky sequence file {str(file_name)}", e)
 
-                residues.update(chain_residues)
+            sequence_3_let = translate_1_to_3(sequence, molecule_type=molecule_type)
+            chain_residues = sequence_3let_to_res(sequence_3_let, chain_code)
 
     except IOError as e:
-        exit_error(f"couldn't open {path} because:\n{e}", e)
+        exit_error(f"couldn't open {file_name} because:\n{e}", e)
 
-    return residues
+    return chain_residues
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import typer
 
 from nef_pipelines import nef_app
 
 app = typer.Typer()
-export_app = typer.Typer()
 import_app = typer.Typer()
+export_app = typer.Typer()
+
 
 if nef_app.app:
 
     nef_app.app.add_typer(
-        app, name="mars", help="- read and write mars [shifts and sequences]"
+        app,
+        name="talos",
+        help="-  read and write talos files [shifts & restraints]",
     )
 
     app.add_typer(
-        export_app, name="export", help="- export mars [shifts and sequences]"
+        import_app, name="import", help="-  import talos dihderal restraints "
+    )
+    app.add_typer(
+        export_app, name="export", help="-  export talos [shifts (& sequence)]"
     )
-
-    app.add_typer(import_app, name="import", help="- import mars [shifts]")
 
     # import of specific importers must be after app creation to avoid circular imports
-    import nef_pipelines.transcoders.mars.exporters.fragments  # noqa: F401
-    import nef_pipelines.transcoders.mars.exporters.input  # noqa: F401
-    import nef_pipelines.transcoders.mars.exporters.sequence  # noqa: F401
-    import nef_pipelines.transcoders.mars.exporters.shifts  # noqa: F401
-    import nef_pipelines.transcoders.mars.importers.peaks  # noqa: F401
-    import nef_pipelines.transcoders.mars.importers.shifts  # noqa: F401
+    import nef_pipelines.transcoders.talos.exporters.shifts  # noqa: F401
+    import nef_pipelines.transcoders.talos.importers.order_parameters  # noqa: F401
+    import nef_pipelines.transcoders.talos.importers.restraints  # noqa: F401
+    import nef_pipelines.transcoders.talos.importers.secondary_structure  # noqa: F401
+    import nef_pipelines.transcoders.talos.importers.sequence  # noqa: F401
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/importers/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     UNUSED,
     add_frames_to_entry,
     read_or_create_entry_exit_error_on_bad_file,
 )
 from nef_pipelines.lib.sequence_lib import (
     TRANSLATIONS_3_1_PROTEIN,
     BadResidue,
-    chain_code_iter,
+    get_chain_code_iter,
     get_residue_name_from_lookup,
     translate_1_to_3,
 )
 from nef_pipelines.lib.shift_lib import shifts_to_nef_frame
 from nef_pipelines.lib.structures import (
     AtomLabel,
     LineInfo,
@@ -121,15 +121,16 @@
     file_names,
     prefix_to_strip=DEFAULT_PSEUDO_RESIDUE_PREFIX,
     parse_residues=True,
 ):
 
     sparky_frames = []
 
-    for file_name, chain_code in zip(file_names, chain_code_iter(chain_codes)):
+    chain_code_iter = get_chain_code_iter(chain_codes)
+    for file_name, chain_code in zip(file_names, chain_code_iter):
 
         with open(file_name) as lines:
 
             sparky_shifts = _parse_shifts(
                 lines,
                 chain_code=chain_code,
                 file_name=file_name,
@@ -230,14 +231,29 @@
     string = string.upper()
     for residue_name in TRANSLATIONS_3_1_PROTEIN:
         if residue_name in string:
             result.append(residue_name)
     return result
 
 
+# TODO: remove when python 3.8 no longer supported
+def _removeprefix(target: str, prefix: str) -> str:
+    if target.startswith(prefix):
+        return target[len(prefix) :]
+    else:
+        return target
+
+
+def _removesuffix(target: str, suffix: str) -> str:
+    if target.endswith(suffix):
+        return target[: -len(suffix)]
+    else:
+        return target
+
+
 def _parse_line(
     line_info, heading_indices, chain_code, prefix_to_strip, parse_residues
 ):
     results = []
 
     fields = line_info.line.strip().split()
     pseudo_residue = fields[heading_indices[PSEUDO_RESIDUE]]
@@ -247,15 +263,15 @@
             value = fields[index]
             if value != MARS_UNDEFINED:
 
                 _exit_if_shift_is_not_float(value, line_info)
 
                 value = float(value)
 
-                pseudo_residue = pseudo_residue.removeprefix(prefix_to_strip)
+                pseudo_residue = _removeprefix(pseudo_residue, prefix_to_strip)
 
                 (
                     pseudo_pre_chars,
                     pseudo_residue_number,
                     pseudo_post_chars,
                 ) = _split_pseudo_residue(pseudo_residue)
 
@@ -286,15 +302,15 @@
     return results
 
 
 def _split_heading(heading: str):
 
     offset = ""
     if heading.endswith("-1"):
-        heading = heading.removesuffix("-1")
+        heading = _removesuffix(heading, "-1")
         offset = "-1"
     return heading, offset
 
 
 def _warn_multiple_residues(residue_names, line_info):
     msg = f"""\
                         WARNING: the pseudo residue on line {line_info.line_no} in file {line_info.file_name} contains
@@ -307,17 +323,17 @@
                                  {line_info.line}
                     """
     print(msg, files=sys.stderr)
 
 
 def _split_pseudo_residue(pseudo_residue):
     first_characters = _get_starting_alpha(pseudo_residue)
-    pseudo_residue = pseudo_residue.removeprefix(first_characters)
+    pseudo_residue = _removeprefix(pseudo_residue, first_characters)
     numbers = get_starting_number(pseudo_residue)
-    last_characters = pseudo_residue.removeprefix(numbers)
+    last_characters = _removeprefix(pseudo_residue, numbers)
 
     return first_characters, numbers, last_characters
 
 
 def _exit_if_pseudo_residue_number_missing(
     pseudo_residue_number, pseudo_residue, line_info
 ):
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/project.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/project.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,33 +6,58 @@
 
 import requests
 import typer
 from fyeah import f
 from pynmrstar import Entry
 from requests.exceptions import HTTPError
 from strenum import LowercaseStrEnum
+from tabulate import tabulate
 
 from nef_pipelines.lib.nef_lib import (
     read_entry_from_file_or_exit_error,
     read_or_create_entry_exit_error_on_bad_file,
 )
-from nef_pipelines.lib.sequence_lib import chain_code_iter
+from nef_pipelines.lib.sequence_lib import get_chain_code_iter
 from nef_pipelines.lib.util import (
     STDIN,
     exit_error,
     is_int,
     parse_comma_separated_options,
 )
 from nef_pipelines.transcoders.nmrstar import import_app
 from nef_pipelines.transcoders.nmrstar.importers.sequence import pipe as sequence_pipe
 from nef_pipelines.transcoders.nmrstar.importers.shifts import pipe as shift_pipe
 from nef_pipelines.transcoders.nmrstar.nmrstar_lib import StereoAssignmentHandling
 
 app = typer.Typer()
 
+BMRB_URL_TEMPLATE = "https://bmrb.io/ftp/pub/bmrb/entry_directories/bmr{entry_number}/bmr{entry_number}_3.str"
+
+
+class EntrySource(LowercaseStrEnum):
+    FILE = auto()
+    WEB = auto()
+    AUTO = auto()
+
+
+SHORTCUTS = {
+    "UBIQUITIN": "bmr5387",
+    "GB1": "bmr7280",
+    "GB3": "bmr25910",
+    "MBP": "bmr4354",
+    "MSG": "bmr5471",
+    "INSULIN": "bmr1000",
+}
+
+SHORTCUT_ENTRYS = {name: id.lower()[3:] for name, id in SHORTCUTS.items()}
+SHORTCUT_URLS = {
+    name: f(BMRB_URL_TEMPLATE) for name, entry_number in SHORTCUT_ENTRYS.items()
+}
+SHORTCUT_NAMES = ", ".join({name.lower(): name for name in SHORTCUTS.keys()})
+
 NO_CHAIN_START_HELP = """\
 don't include the start chain link type on a chain for the first residue [linkage will be
 middle] for the named chains. Either use a comma joined list of chains [e.g. A,B] or call this
 option multiple times to set chain starts for multiple chains
 """
 
 NO_CHAIN_END_HELP = """\
@@ -44,31 +69,25 @@
 STEREO_HELP = """\
     how to handle stereo assignments the choices are:
     - ambiguous: assume all stereo assignments are ambiguous
     - as-assigned: use the stereo assignments as they are in the file
     - auto: use as assigned if some geminal stereo assignments are present, otherwise assume all are ambiguous
 """
 
-BMRB_URL_TEMPLATE = "https://bmrb.io/ftp/pub/bmrb/entry_directories/bmr{entry_number}/bmr{entry_number}_3.str"
 
-FILE_PATH_HELP = """\
-the file to read, if it is of the form bmr<NUMBER> or just a number  or appears to be a url
-the program will attempt to fetch the entry from the bmrb or the web first before looking
+FILE_PATH_HELP = f"""\
+the file to read, if it is is one of the shortcuts {SHORTCUT_NAMES}, of the form bmr<NUMBER> or is just a number or
+appears to be a url the program will attempt to fetch the entry from the bmrb or the web first before looking
 for a file on disc unless this behaviour overridden by the --source option
 """
 
 
-class EntrySource(LowercaseStrEnum):
-    FILE = auto()
-    WEB = auto()
-    AUTO = auto()
-
-
 @import_app.command()
 def project(
+    ctx: typer.Context,
     chain_codes: List[str] = typer.Option(
         [],
         "--chains",
         help="""chain codes to use for the imported chains, can be a comma separated list or can be called
                 multiple times if no chain codes are provided they will be named A B C...""",
         metavar="<CHAIN-CODES>",
     ),
@@ -79,78 +98,109 @@
         [], "--no-chain-end", help=NO_CHAIN_END_HELP
     ),
     source: EntrySource = typer.Option(
         EntrySource.AUTO, help="the source of the entry"
     ),
     use_author: bool = typer.Option(False, help="use author field for sequence codes"),
     stereo_mode: StereoAssignmentHandling = typer.Option("auto", help=STEREO_HELP),
-    entry_name: str = typer.Option(
+    default_entry_name: str = typer.Option(
         None, help="a name for the entry (defaults to the bmrb entry number)"
     ),
     input: Path = typer.Option(
         STDIN,
         "-i",
         "--in",
         help="file to read NEF data from [- is stdin; defaults is stdin]",
     ),
     url_template: str = typer.Option(
         BMRB_URL_TEMPLATE,
         help=f"template for the bmrb url [default {BMRB_URL_TEMPLATE}]",
     ),
-    file_path: str = typer.Argument(..., help=", metavar=<NMR-STAR-FILE>"),
+    list_shortcuts: bool = typer.Option(
+        False, "--list-shortcuts", help="list the available shortcuts and exit"
+    ),
+    file_paths: List[str] = typer.Argument(None, help=FILE_PATH_HELP),
 ):
-    """-  convert as much as possible from an NMR-STAR file to NEF [shifts & sequences] [alpha]"""
+    """- convert as much as possible from an NMR-STAR file to NEF [shifts & sequences] [alpha]"""
 
-    chain_codes = parse_comma_separated_options(chain_codes)
-    if not chain_codes:
-        chain_codes = chain_code_iter()
-
-    no_chain_starts = parse_comma_separated_options(no_chain_starts)
-    if not no_chain_starts:
-        no_chain_starts = [False]
-
-    no_chain_ends = parse_comma_separated_options(no_chain_ends)
-    if no_chain_ends:
-        no_chain_ends = [False]
-
-    is_bmrb = False
-    if source in (EntrySource.AUTO, EntrySource.WEB):
-        url, is_bmrb = _get_path_as_url_or_none(file_path, url_template)
-
-        exit_on_error = True if source == EntrySource.WEB else False
-        possible_entry = _get_bmrb_entry_from_web_or_none(url, exit_on_error)
-
-        nmrstar_entry = _parse_text_to_star_or_none(possible_entry)
-
-    if (source == EntrySource.AUTO and not nmrstar_entry) or source == EntrySource.FILE:
-        nmrstar_entry = read_entry_from_file_or_exit_error(file_path)
-
-    if not nmrstar_entry:
-        msg = f"could not read entry from {file_path}"
-        exit_error(msg)
-
-    entry_name = nmrstar_entry.entry_id if not entry_name else entry_name
-    entry_name = f"bmr{entry_name}" if is_bmrb else entry_name
-
-    nef_entry = read_or_create_entry_exit_error_on_bad_file(
-        input, entry_name=entry_name
-    )
-
-    entry = pipe(
-        nef_entry,
-        nmrstar_entry,
-        chain_codes,
-        no_chain_starts,
-        no_chain_ends,
-        use_author,
-        stereo_mode,
-        file_path,
-    )
+    if list_shortcuts:
+        _list_shortcuts_and_exit()
 
-    print(entry)
+    file_paths = parse_comma_separated_options(file_paths)
+    file_paths = [
+        SHORTCUTS[file_path.upper()] if file_path.upper() in SHORTCUTS else file_path
+        for file_path in file_paths
+    ]
+
+    if not file_paths:
+        typer.echo(ctx.get_help())
+        exit_error("missing file path argument")
+
+    for file_path in file_paths:
+        chain_codes = parse_comma_separated_options(chain_codes)
+        chain_codes = get_chain_code_iter(chain_codes)
+
+        no_chain_starts = parse_comma_separated_options(no_chain_starts)
+        if not no_chain_starts:
+            no_chain_starts = [False]
+
+        no_chain_ends = parse_comma_separated_options(no_chain_ends)
+        if no_chain_ends:
+            no_chain_ends = [False]
+
+        is_bmrb = False
+        if source in (EntrySource.AUTO, EntrySource.WEB):
+            url, is_bmrb = _get_path_as_url_or_none(file_path, url_template)
+
+            exit_on_error = True if source == EntrySource.WEB else False
+            possible_entry = _get_bmrb_entry_from_web_or_none(url, exit_on_error)
+
+            nmrstar_entry = _parse_text_to_star_or_none(possible_entry)
+
+        if (
+            source == EntrySource.AUTO and not nmrstar_entry
+        ) or source == EntrySource.FILE:
+            nmrstar_entry = read_entry_from_file_or_exit_error(file_path)
+
+        if not nmrstar_entry:
+            msg = f"could not read entry from {file_path}"
+            exit_error(msg)
+
+        entry_name = (
+            nmrstar_entry.entry_id if not default_entry_name else default_entry_name
+        )
+        entry_name = f"bmr{entry_name}" if is_bmrb else entry_name
+        nef_entry = read_or_create_entry_exit_error_on_bad_file(
+            input, entry_name=entry_name
+        )
+
+        entry = pipe(
+            nef_entry,
+            nmrstar_entry,
+            chain_codes,
+            no_chain_starts,
+            no_chain_ends,
+            use_author,
+            stereo_mode,
+            file_path,
+        )
+
+        print(entry)
+
+
+def _list_shortcuts_and_exit():
+    print("The available shortcuts are:\n", file=sys.stderr)
+    shortcuts = [
+        [shortcut.lower(), entry, SHORTCUT_URLS[shortcut]]
+        for shortcut, entry in SHORTCUTS.items()
+    ]
+    HEADERS = ["name", "entry id.", "url"]
+    print(tabulate(shortcuts, headers=HEADERS), file=sys.stderr)
+    print("\nexiting...", file=sys.stderr)
+    sys.exit(0)
 
 
 def pipe(
     nef_entry,
     nmrstar_entry,
     chain_codes,
     no_chain_starts,
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/sequence.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     UNUSED,
     add_frames_to_entry,
     loop_row_namespace_iter,
     read_entry_from_file_or_exit_error,
     read_or_create_entry_exit_error_on_bad_file,
 )
 from nef_pipelines.lib.sequence_lib import (
-    chain_code_iter,
+    get_chain_code_iter,
     offset_chain_residues,
     sequence_to_nef_frame,
 )
 from nef_pipelines.lib.structures import Residue
 from nef_pipelines.lib.util import STDIN, exit_error, parse_comma_separated_options
 from nef_pipelines.transcoders.fasta.importers.sequence import (
     _get_sequence_offsets,
@@ -165,17 +165,18 @@
         residue_name = row.Comp_ID
         entity_id = row.Entity_ID
 
         entity_ids.add(entity_id)
         residue = Residue(entity_id, seq_code, residue_name)
         sequence_residues.append(residue)
 
+    chain_code_iter = get_chain_code_iter(chain_codes)
     entity_id_to_chain_code = {
         entity_id: chain_code
-        for entity_id, chain_code in zip(entity_ids, chain_code_iter(chain_codes))
+        for entity_id, chain_code in zip(entity_ids, chain_code_iter)
     }
 
     for i, residue in enumerate(sequence_residues):
         sequence_residues[i] = replace(
             residue, chain_code=entity_id_to_chain_code[residue.chain_code]
         )
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrstar/importers/shifts.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     add_frames_to_entry,
     loop_row_namespace_iter,
     read_entry_from_file_or_exit_error,
     read_entry_from_file_or_stdin_or_exit_error,
 )
-from nef_pipelines.lib.sequence_lib import chain_code_iter, sequence_from_entry_or_exit
+from nef_pipelines.lib.sequence_lib import (
+    get_chain_code_iter,
+    sequence_from_entry_or_exit,
+)
 from nef_pipelines.lib.shift_lib import shifts_to_nef_frame
 from nef_pipelines.lib.structures import AtomLabel, Residue, ShiftData, ShiftList
 from nef_pipelines.lib.translation.chem_comp import ID, ChemCompLinking
 from nef_pipelines.lib.util import (
     STDIN,
     chunks,
     exit_error,
@@ -111,15 +114,16 @@
     else:
         result = list(chem_atom_set.chemAtoms) if chem_atom_set.chemAtoms else []
 
         if chem_atom_set.chemAtomSets:
             for nested_set in chem_atom_set.chemAtomSets:
                 result.extend(chem_atom_set_by_id[nested_set].chemAtoms)
 
-    return set(result)
+    id_and_values_result = {item.ID: item for item in result}
+    return list(id_and_values_result.values())
 
 
 def _get_geminal_pairs(residue_names):
 
     ambiguity_translations_path = (
         Path(nef_pipelines_root())
         / "nef_pipelines"
@@ -277,16 +281,21 @@
             for chem_comp_var in chem_comp.chemCompVars
             if chem_comp_var.isDefaultVar
             and chem_comp_var.linking in ["start", "middle", "end"]
         ]
 
         active_chem_comp_vars_atom_sets = {}
         for chem_comp_var in active_chem_comp_vars:
-            active_chem_comp_atom_ids = set(chem_comp_var.chemAtoms)
-            for atom_set_name, atom_set_atom_ids in chem_atom_set_atoms.items():
+
+            active_chem_comp_atom_ids = set(
+                [chem_atom.ID for chem_atom in chem_comp_var.chemAtoms]
+            )
+
+            for atom_set_name, atom_set_atoms in chem_atom_set_atoms.items():
+                atom_set_atom_ids = set([atom.ID for atom in atom_set_atoms])
                 if atom_set_atom_ids.issubset(active_chem_comp_atom_ids):
                     atom_set_chem_atoms = [
                         chem_atoms_by_id[id].name for id in atom_set_atom_ids
                     ]
                     name = atom_set_name[0]
                     name = (
                         name if name != "HD*|HE*" else "QR"
@@ -376,22 +385,20 @@
 
     ambiguities = _replace_atom_dict_entity_ids_with_chain_codes(
         ambiguities, entity_id_to_chain_code
     )
 
     per_residue_ambiguities = _organise_ambiguities_by_residue(ambiguities)
 
-    _replace_atoms_with_duplicated_shifts(
+    per_residue_and_atom_shifts = _replace_atoms_with_duplicated_shifts(
         per_residue_and_atom_shifts,
         sequence_residues_by_residue,
         per_residue_ambiguities,
     )
 
-    stereo_mode = StereoAssignmentHandling.ALL_AMBIGUOUS
-
     all_stereo_pairs = _get_geminal_pairs(residue_names)
 
     _apply_stereo_assignment_ambiguities(
         per_residue_and_atom_shifts,
         all_stereo_pairs,
         sequence_residues_by_residue,
         per_residue_ambiguities,
@@ -444,15 +451,14 @@
             if len(found_pairs) == 2:
                 found_pairs = dict(
                     sorted(found_pairs.items(), key=lambda item: item[1])
                 )
                 if stereo_mode is StereoAssignmentHandling.ALL_AMBIGUOUS:
                     for before, old_shift in found_pairs.items():
                         new_atom_name = ambiguous_pair[before]
-                        # print('!', before, new)
                         atom = old_shift.atom
                         atom = replace(atom, atom_name=new_atom_name)
                         new_shift = replace(old_shift, atom=atom)
                         del chemical_shifts_by_atom_names[before]
                         chemical_shifts_by_atom_names[new_atom_name] = new_shift
 
 
@@ -515,14 +521,24 @@
                     del chemical_shifts_by_atom_names[atom]
 
                 residue_ambiguities = per_residue_ambiguities[residue]
                 residue_ambiguities[atom_set_name] = new_ambiguity
                 for atom in related_atoms:
                     del residue_ambiguities[atom]
 
+                atom_set_shift = chemical_shifts_by_atom_names[atom_set_name]
+                atom_set_shift_atom = atom_set_shift.atom
+                atom_set_shift_atom = replace(
+                    atom_set_shift_atom, atom_name=atom_set_name
+                )
+                atom_set_shift = replace(atom_set_shift, atom=atom_set_shift_atom)
+                chemical_shifts_by_atom_names[atom_set_name] = atom_set_shift
+
+    return per_residue_and_atom_shifts
+
 
 def _get_stereo_mode(ambiguities, stereo_mode):
     if stereo_mode == StereoAssignmentHandling.AUTO and any(
         [
             value == BmrbShiftAmbiguities.ALIPHATIC_GEMINAL.value
             for value in ambiguities.values()
         ]
@@ -679,17 +695,18 @@
 
 def _build_entity_ids_to_chain_codes(chain_codes, denormalised_shifts):
     entity_ids = list(
         OrderedSet(
             sorted([shift.atom.residue.chain_code for shift in denormalised_shifts])
         )
     )
+    chain_code_iter = get_chain_code_iter(chain_codes)
     entity_id_to_chain_code = {
         entity_id: chain_code
-        for entity_id, chain_code in zip(entity_ids, chain_code_iter(chain_codes))
+        for entity_id, chain_code in zip(entity_ids, chain_code_iter)
     }
     return entity_id_to_chain_code
 
 
 def _exit_error_if_missing_residues(residues, shift_residues, file_name):
 
     # could do more here and see if there is a match by sequence...
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files 7% similar despite different names*

```diff
@@ -375,41 +375,41 @@
         "folding",
         "absolute_peak_positions",
         "is_acquisition",
     )
     loop.add_tag(list_tags)
     list_data = peaks_list.peak_list_data
     for i in range(list_data.num_axis):
-        for tag in list_tags:
-            if tag == "dimension_id":
-                loop.add_data_by_tag(tag, i + 1)
-            elif tag == "axis_unit":
-                loop.add_data_by_tag(tag, "ppm")
-            elif tag == "axis_code":
-                axis_codes = args.axis_codes.split(".")
-                loop.add_data_by_tag(tag, _get_isotope_code_or_exit(i, axis_codes))
-            elif tag == "spectrometer_frequency":
-                loop.add_data_by_tag(tag, list_data.spectrometer_frequencies[i])
-            elif tag == "spectral_width":
-                if list_data.sweep_widths:
-                    loop.add_data_by_tag(tag, list_data.sweep_widths[i])
-                else:
-                    loop.add_data_by_tag(tag, NEF_UNKNOWN)
-            elif tag == "folding":
-                loop.add_data_by_tag(tag, "circular")
-            elif tag == "absolute_peak_positions":
-                loop.add_data_by_tag(tag, "true")
-            else:
-                loop.add_data_by_tag(tag, NEF_UNKNOWN)
+        row = {
+            "dimension_id": i + 1,
+            "axis_unit": "ppm",
+            "axis_code": _get_isotope_code_or_exit(i, args.axis_codes.split(".")),
+            "spectrometer_frequency": list_data.spectrometer_frequencies[i],
+            "spectral_width": (
+                list_data.sweep_widths[i] if list_data.sweep_widths else NEF_UNKNOWN
+            ),
+            "value_first_point": NEF_UNKNOWN,
+            "folding": "circular",
+            "absolute_peak_positions": "true",
+            "is_acquisition": NEF_UNKNOWN,
+        }
+        loop.add_data(
+            [
+                row,
+            ]
+        )
+
     loop = Loop.from_scratch("nef_spectrum_dimension_transfer")
     frame.add_loop(loop)
     transfer_dim_tags = ("dimension_1", "dimension_2", "transfer_type")
     loop.add_tag(transfer_dim_tags)
     loop = Loop.from_scratch("nef_peak")
     frame.add_loop(loop)
+
+    # TODO: put this in a sane order!
     peak_tags = [
         "index",
         "peak_id",
         "volume",
         "volume_uncertainty",
         "height",
         "height_uncertainty",
@@ -433,53 +433,74 @@
 
     loop.add_tag(tags)
     for i, peak in enumerate(peaks_list.peaks):
         peak_values = peak["values"]
         if peak_values.deleted:
             continue
 
+        positions = {}
         for tag in tags:
-
-            if tag == "index":
-                loop.add_data_by_tag(tag, i + 1)
-            elif tag == "peak_id":
-                loop.add_data_by_tag(tag, peak_values.serial)
-            elif tag == "volume":
-                loop.add_data_by_tag(tag, peak_values.volume)
-            elif tag == "height":
-                loop.add_data_by_tag(tag, peak_values.height)
-            elif tag.split("_")[0] == "position" and len(tag.split("_")) == 2:
+            if tag.split("_")[0] == "position" and len(tag.split("_")) == 2:
                 index = int(tag.split("_")[-1]) - 1
-                loop.add_data_by_tag(tag, peak[index].ppm)
-            elif tag.split("_")[:2] == ["chain", "code"]:
+                positions[tag] = peak[index].ppm
+
+        chain_codes = {}
+        for tag in tags:
+            if tag.split("_")[:2] == ["chain", "code"]:
                 index = int(tag.split("_")[-1]) - 1
                 chain_code = peak[index].atom_labels.residue.chain_code
                 chain_code = chain_code if chain_code is not None else args.chain_code
                 chain_code = chain_code if chain_code else "."
-                loop.add_data_by_tag(tag, chain_code)
-            elif tag.split("_")[:2] == ["sequence", "code"]:
+                chain_codes[tag] = chain_code
+
+        sequence_codes = {}
+        for tag in tags:
+            if tag.split("_")[:2] == ["sequence", "code"]:
                 index = int(tag.split("_")[-1]) - 1
                 sequence_code = peak[index].atom_labels.residue.sequence_code
                 sequence_code = sequence_code if sequence_code else "."
-                loop.add_data_by_tag(tag, sequence_code)
-            elif tag.split("_")[:2] == ["residue", "name"]:
+                sequence_codes[tag] = sequence_code
+
+        residue_names = {}
+        for tag in tags:
+            if tag.split("_")[:2] == ["residue", "name"]:
                 index = int(tag.split("_")[-1]) - 1
 
                 # TODO: there could be more than 1 atom label here and this should be a list...
                 residue_name = peak[index].atom_labels.residue.residue_name
                 residue_name = residue_name if residue_name else "."
-                loop.add_data_by_tag(tag, residue_name)
-            elif tag.split("_")[:2] == ["atom", "name"]:
+                residue_names[tag] = residue_name
+
+        atom_names = {}
+        for tag in tags:
+            if tag.split("_")[:2] == ["atom", "name"]:
                 index = int(tag.split("_")[-1]) - 1
 
                 atom_name = peak[index].atom_labels.atom_name
                 atom_name = atom_name if atom_name else "."
-                loop.add_data_by_tag(tag, atom_name)
-            else:
-                loop.add_data_by_tag(tag, constants.NEF_UNKNOWN)
+                atom_names[tag] = atom_name
+
+        row_dict = {
+            "index": i + 1,
+            "peak_id": peak_values.serial,
+            **chain_codes,
+            **sequence_codes,
+            **residue_names,
+            **atom_names,
+            **positions,
+            "volume": peak_values.volume,
+            "volume_uncertainty": NEF_UNKNOWN,
+            "height": peak_values.height,
+            "height_uncertainty": NEF_UNKNOWN,
+        }
+        loop.add_data(
+            [
+                row_dict,
+            ]
+        )
     return frame
 
 
 # TODO: can be replaced by str.removesuffix when min python version >= 3.9
 def _remove_suffix(string: str, suffix: str) -> str:
 
     result = string
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import Namespace
 from pathlib import Path
 from typing import List
 
 import typer
 
-from nef_pipelines.lib.sequence_lib import chain_code_iter, sequence_to_nef_frame
+from nef_pipelines.lib.sequence_lib import get_chain_code_iter, sequence_to_nef_frame
 from nef_pipelines.lib.typer_utils import get_args
 from nef_pipelines.lib.util import (
     STDIN,
     exit_error,
     parse_comma_separated_options,
     process_stream_and_add_frames,
 )
@@ -57,15 +57,16 @@
         exit_error(f"reading sequence failed because {e}")
 
 
 def process_sequence(args: Namespace):
     nmrview_frames = []
 
     chain_codes = parse_comma_separated_options(args.chain_codes)
-    for file_name, chain_code in zip(args.file_names, chain_code_iter(chain_codes)):
+    chain_code_iter = get_chain_code_iter(chain_codes)
+    for file_name, chain_code in zip(args.file_names, chain_code_iter):
         with open(file_name, "r") as lines:
             nmrview_sequence = read_sequence(lines, chain_code=chain_code)
 
             frame = sequence_to_nef_frame(nmrview_sequence, args.entry_name)
 
             nmrview_frames.append(frame)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from typing import Dict, List, Tuple
 
 import typer
 from pynmrstar import Entry, Saveframe
 
 from nef_pipelines.lib.constants import NEF_PIPELINES
 from nef_pipelines.lib.nef_lib import read_entry_from_file_or_stdin_or_exit_error
-from nef_pipelines.lib.sequence_lib import chain_code_iter, sequence_from_entry_or_exit
+from nef_pipelines.lib.sequence_lib import (
+    get_chain_code_iter,
+    sequence_from_entry_or_exit,
+)
 from nef_pipelines.lib.shift_lib import shifts_to_nef_frame
 from nef_pipelines.lib.structures import SequenceResidue
 from nef_pipelines.lib.util import (
     STDIN,
     exit_error,
     fixup_metadata,
     get_pipe_file_text_or_exit,
@@ -64,15 +67,16 @@
         exit_error(f"reading sequence failed because {e}", e)
 
 
 def pipe(entry, chain_codes, sequence, entry_name, file_names):
 
     nmrview_frames = []
 
-    for file_name, chain_code in zip(file_names, chain_code_iter(chain_codes)):
+    chain_code_iter = get_chain_code_iter(chain_codes)
+    for file_name, chain_code in zip(file_names, chain_code_iter):
 
         with open(file_name) as lines:
 
             chain_seqid_to_type = _sequence_to_residue_type_lookup(sequence)
 
             nmrview_shifts = parse_shifts(
                 lines, chain_seqid_to_type, chain_code=chain_code, file_name=file_name
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rcsb/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rcsb/importers/sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 from nef_pipelines.lib.structures import SequenceResidue
 from nef_pipelines.lib.typer_utils import get_args
 from nef_pipelines.lib.util import (
     exit_error,
     parse_comma_separated_options,
     process_stream_and_add_frames,
 )
-from nef_pipelines.transcoders.rcsb.rcsb_lib import parse_pdb, parse_cif, guess_cif_or_pdb, RCSBFileType
-
 from nef_pipelines.transcoders.rcsb import import_app
+from nef_pipelines.transcoders.rcsb.rcsb_lib import (
+    RCSBFileType,
+    guess_cif_or_pdb,
+    parse_cif,
+    parse_pdb,
+)
 
 app = typer.Typer()
 
 CHAINS_HELP = """chains [or segid] to read', metavar='<CHAIN-CODE>, multiple chains can be added as a comma joined list
                 [eg A.B.C] ] or by calling this option mutiple times"""
 NO_CHAIN_START_HELP = """don't include the start chain link type on a chain for the first residue [linkage will be
                          middle] for the named chains. Either use a comma joined list of chains [e.g. A,B] or call this
@@ -83,52 +87,51 @@
     )
 
     print(entry)
 
 
 def read_sequences(path, target_chain_codes, use_segids=False):
 
-    file_lines =  list(open(path).readlines())
+    with open(path) as fh:
+        lines = fh.readlines()
+    file_lines = list(lines)
     file_type = guess_cif_or_pdb(file_lines, str(path))
 
     if file_type is RCSBFileType.PDB:
         model = parse_pdb(file_lines)[0]
     elif file_type is RCSBFileType.CIF:
         model = parse_cif(file_lines)[0]
     else:
-        msg  =  \
-        f'''
+        msg = f"""
             Couldn't determine if the file {path} was a cif or pdb file...
             are you sure the file has the right format?
-        '''
+        """
         exit_error(msg)
 
     sequences = []
 
-
     if not use_segids:
 
         for chain in model:
             id = chain.chain_code
             if not id or len(id) == 0:
                 use_segids = True
 
     all_chains = len(target_chain_codes) == 0
 
-
     for chain in model:
         for residue in chain:
             chain_code = chain.segment_id if use_segids else chain.chain_code
             chain_code = chain_code.strip()
 
             if not all_chains and chain_code not in target_chain_codes:
                 continue
 
-            sequence_code =  residue.sequence_code
-            #TODO support a hetero atom flag
+            sequence_code = residue.sequence_code
+            # TODO support a hetero atom flag
             # if len(hetero_atom_flag.strip()) != 0:
             #     continue
 
             if chain_code == "":
                 exit_error(
                     f"residue with no chain code found for file {path} sequence_code is {sequence_code} \
                     residue_name is {residue.get_resname()}"
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rcsb/rcsb_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     add_frames_to_entry,
     read_entry_from_file_or_stdin_or_exit_error,
 )
 from nef_pipelines.lib.sequence_lib import (
     BadResidue,
-    chain_code_iter,
+    get_chain_code_iter,
     get_residue_name_from_lookup,
     sequence_from_entry_or_exit,
     sequence_to_residue_name_lookup,
     translate_1_to_3,
 )
 from nef_pipelines.lib.shift_lib import shifts_to_nef_frame
 from nef_pipelines.lib.structures import (
@@ -93,15 +93,16 @@
 
 def pipe(entry, chain_codes, frame_name, file_names):
 
     sequence = sequence_from_entry_or_exit(entry)
 
     sparky_frames = []
 
-    for file_name, chain_code in zip(file_names, chain_code_iter(chain_codes)):
+    chain_code_iter = get_chain_code_iter(chain_codes)
+    for file_name, chain_code in zip(file_names, chain_code_iter):
 
         with open(file_name) as lines:
 
             chain_seqid_to_type = sequence_to_residue_name_lookup(sequence)
 
             sparky_shifts = _parse_shifts(
                 lines, chain_seqid_to_type, chain_code=chain_code, file_name=file_name
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/sparky/sparky_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 import typer
 
 from nef_pipelines import nef_app
 
 app = typer.Typer()
 import_app = typer.Typer()
-export_app = typer.Typer()
+# export_app = typer.Typer()
 
 
 if nef_app.app:
 
     nef_app.app.add_typer(
         app,
-        name="talos",
-        help="-  read and write talos files [shifts & restraints]",
+        name="xeasy",
+        help="-  read xeasy files [flya dialect: sequence]",
     )
 
-    app.add_typer(
-        import_app, name="import", help="-  import talos dihderal restraints "
-    )
-    app.add_typer(
-        export_app, name="export", help="-  export talos [shifts (& sequence)]"
-    )
+    app.add_typer(import_app, name="import", help="-  import xeasy [sequence]")
 
     # import of specific importers must be after app creation to avoid circular imports
-    import nef_pipelines.transcoders.talos.exporters.shifts  # noqa: F401
-    import nef_pipelines.transcoders.talos.importers.order_parameters  # noqa: F401
-    import nef_pipelines.transcoders.talos.importers.restraints  # noqa: F401
-    import nef_pipelines.transcoders.talos.importers.secondary_structure  # noqa: F401
-    import nef_pipelines.transcoders.talos.importers.sequence  # noqa: F401
+    import nef_pipelines.transcoders.xeasy.importers.peaks  # noqa: F401
+    import nef_pipelines.transcoders.xeasy.importers.sequence  # noqa: F401
+    import nef_pipelines.transcoders.xeasy.importers.shifts  # noqa: F401
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/exporters/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/exporters/shifts.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     shifts = [
         shift
         for shift in shifts
         if shift.atom.residue.residue_name in TRANSLATIONS_3_1[MoleculeTypes.PROTEIN]
     ]
 
-    with (redirect_stdout(StringIO()) as capture):
+    with redirect_stdout(StringIO()) as capture:
         print(f"REMARK Chemical shift table for {entry.entry_id}")
         print()
         print(f"DATA CHAIN {target_chain_code}")
         print(f"DATA FIRST_RESID {start_residue}")
         print()
         for sub_sequence in chunked_sequence:
             print(f"DATA SEQUENCE {sub_sequence}")
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/order_parameters.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/order_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 
 import typer
 from fyeah import f
 from pynmrstar import Entry, Loop
 
 from nef_pipelines.lib.nef_lib import (
+    NEF_PIPELINES_PREFIX,
     UNUSED,
     create_nef_save_frame,
     read_file_or_exit,
     read_or_create_entry_exit_error_on_bad_file,
 )
 from nef_pipelines.lib.sequence_lib import (
     exit_if_chain_not_in_sequence,
@@ -22,16 +23,16 @@
 app = typer.Typer()
 
 FRAME_NAME_HELP = """\
                         name for the frame that will be created,
                         default is {chain_code}_{element_1}{isotope_number_1}_{element_2}{isotope_number_2}
                     """
 
-NEF_PIPELINES = "nefpls"
-PIPELINES_ORDER_DATA_CATEGORY = f"{NEF_PIPELINES}_order_data"
+
+PIPELINES_ORDER_DATA_CATEGORY = f"{NEF_PIPELINES_PREFIX}_order_data"
 DEFAULT_SEPARATOR = "::"
 DEFAULT_END = ""
 
 
 @import_app.command()
 def order_parameters(
     chain_code: str = typer.Option(
@@ -115,15 +116,15 @@
             "source": "estimate",
             "diffusion_model": UNUSED,
         }
 
         for tag, value in extra_tags.items():
             frame.add_tag(tag, value)
 
-        data_loop = Loop.from_scratch(f"{NEF_PIPELINES}_order_values")
+        data_loop = Loop.from_scratch(f"{NEF_PIPELINES_PREFIX}_order_values")
 
         value_types = set()
         for value in values.values():
             value_types.update(value.keys())
 
         type_strings = [f"{str(type)}  {str(type)}_err" for type in value_types]
         type_string = " ".join(type_strings)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/restraints.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/restraints.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/secondary_structure.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/talos/talos_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/talos/talos_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import typer
 
 from nef_pipelines import nef_app
 
 app = typer.Typer()
+export_app = typer.Typer()
 import_app = typer.Typer()
-# export_app = typer.Typer()
-
 
 if nef_app.app:
 
     nef_app.app.add_typer(
-        app,
-        name="xeasy",
-        help="-  read xeasy files [flya dialect: sequence]",
+        app, name="mars", help="- read and write mars [shifts and sequences]"
+    )
+
+    app.add_typer(
+        export_app, name="export", help="- export mars [shifts and sequences]"
     )
 
-    app.add_typer(import_app, name="import", help="-  import xeasy [sequence]")
+    app.add_typer(
+        import_app, name="import", help="- import mars [shifts, sequence & peaks]"
+    )
 
     # import of specific importers must be after app creation to avoid circular imports
-    import nef_pipelines.transcoders.xeasy.importers.peaks  # noqa: F401
-    import nef_pipelines.transcoders.xeasy.importers.sequence  # noqa: F401
-    import nef_pipelines.transcoders.xeasy.importers.shifts  # noqa: F401
+    import nef_pipelines.transcoders.mars.exporters.fragments  # noqa: F401
+    import nef_pipelines.transcoders.mars.exporters.input  # noqa: F401
+    import nef_pipelines.transcoders.mars.exporters.sequence  # noqa: F401
+    import nef_pipelines.transcoders.mars.exporters.shifts  # noqa: F401
+    import nef_pipelines.transcoders.mars.importers.peaks  # noqa: F401
+    import nef_pipelines.transcoders.mars.importers.sequence  # noqa: F401
+    import nef_pipelines.transcoders.mars.importers.shifts  # noqa: F401
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/importers/peaks.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/importers/peaks.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 ):
 
     xeasy_frames = []
 
     residue_type_lookup = sequence_to_residue_name_lookup(sequence)
     for file_name in file_names:
 
-        lines = file_name.open().readlines()
+        with file_name.open() as fh:
+            lines = fh.readlines()
 
         spectrum_type, dimension_info, peaks = parse_peaks(
             lines, file_name, residue_type_lookup
         )
 
         dimensions = _guess_dimensions_if_not_defined_or_throw(peaks, dimension_info)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/importers/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,8 +77,12 @@
 
     entry.add_saveframe(xeasy_frame)
 
     return entry
 
 
 def _read_sequence(file_name: Path) -> List[SequenceResidue]:
-    return parse_sequence(file_name.open().readlines())
+
+    with file_name.open() as fh:
+        lines = fh.readlines()
+
+    return parse_sequence(lines)
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/importers/shifts.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.66/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.66/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.65
+Version: 0.1.66
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -12,15 +12,16 @@
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: cachetools==5.3.3
 Requires-Dist: click==8.1.3
-Requires-Dist: f-yeah==0.4.0
+Requires-Dist: f-yeah==0.3.0; python_version < "3.12"
+Requires-Dist: f-yeah==0.4.0; python_version >= "3.12"
 Requires-Dist: fastaparser==1.1.1
 Requires-Dist: freezegun==1.1.0
 Requires-Dist: frozendict==2.3.7
 Requires-Dist: hjson==3.1.0
 Requires-Dist: mmcif-pdbx==2.0.1
 Requires-Dist: ordered-set==4.1.0
 Requires-Dist: pydantic==2.6.3
@@ -28,14 +29,15 @@
 Requires-Dist: pyparsing==3.0.8
 Requires-Dist: pytest==7.1.3
 Requires-Dist: pytest-mock==3.12.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: StrEnum==0.4.8
 Requires-Dist: tabulate==0.8.9
 Requires-Dist: typer==0.7.0
+Requires-Dist: uncertainties==3.1.7
 Requires-Dist: urllib3==1.26.15
 Requires-Dist: wcmatch==8.5
 Requires-Dist: xmltodict==0.13.0
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
```

### Comparing `nef_pipelines-0.1.65/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.66/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
+CITATION.cff
 CONTRIBUTING.md
 LICENSE.txt
 README.md
 TODO.md
 pyproject.toml
 release_to_pypi.sh
 requirements.txt
@@ -16,14 +17,15 @@
 .idea/.gitignore
 .idea/.name
 .idea/NFC.iml
 .idea/modules.xml
 .idea/vcs.xml
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
+docs/design_overview.md
 references/Nmr Experiment Nomenclature v2.docx
 references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
 references/kosol idps molecules-18-10802.pdf
 src/nef_pipelines/VERSION
 src/nef_pipelines/__init__.py
 src/nef_pipelines/__main__.py
 src/nef_pipelines/main.py
@@ -92,14 +94,15 @@
 src/nef_pipelines/lib/translation/io.py
 src/nef_pipelines/lib/translation/object_iter.py
 src/nef_pipelines/lib/translation/translator.py
 src/nef_pipelines/nef_app/__init__.py
 src/nef_pipelines/tests/conftest.py
 src/nef_pipelines/tests/test_header.py
 src/nef_pipelines/tests/test_nef_lib.py
+src/nef_pipelines/tests/test_save.py
 src/nef_pipelines/tests/test_sequence_lib.py
 src/nef_pipelines/tests/test_test.py
 src/nef_pipelines/tests/test_util.py
 src/nef_pipelines/tests/chains/__init__.py
 src/nef_pipelines/tests/chains/test_clone.py
 src/nef_pipelines/tests/chains/test_list.py
 src/nef_pipelines/tests/chains/test_rename.py
@@ -112,17 +115,23 @@
 src/nef_pipelines/tests/csv/test_data/short.csv
 src/nef_pipelines/tests/csv/test_data/short_complete.csv
 src/nef_pipelines/tests/csv/test_data/ubi_hsqc_short.csv
 src/nef_pipelines/tests/echidna/__init__.py
 src/nef_pipelines/tests/echidna/test_import_peaks.py
 src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
 src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
-src/nef_pipelines/tests/fasta/test_sequence.py
+src/nef_pipelines/tests/fasta/__init__.py
+src/nef_pipelines/tests/fasta/test_export_sequence.py
+src/nef_pipelines/tests/fasta/test_import_sequence.py
 src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+src/nef_pipelines/tests/fasta/test_data/3aa.nef
+src/nef_pipelines/tests/fasta/test_data/3aa_2_chains.nef
+src/nef_pipelines/tests/fasta/test_data/3aa_header.fasta
 src/nef_pipelines/tests/fasta/test_data/3aa_spaces.fasta
+src/nef_pipelines/tests/fasta/test_data/3aa_thx.nef
 src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
 src/nef_pipelines/tests/frames/__init__.py
 src/nef_pipelines/tests/frames/test_delete.py
 src/nef_pipelines/tests/frames/test_filter.py
 src/nef_pipelines/tests/frames/test_list.py
 src/nef_pipelines/tests/frames/test_rename.py
 src/nef_pipelines/tests/frames/test_tabulate.py
@@ -155,14 +164,15 @@
 src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
 src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
 src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
 src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
 src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
 src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
 src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+src/nef_pipelines/tests/nmrstar/__init__.py
 src/nef_pipelines/tests/nmrstar/test_data/bmr15457_3.str.txt
 src/nef_pipelines/tests/nmrstar/test_data/bmr5387_3.str.txt
 src/nef_pipelines/tests/nmrview/__init__.py
 src/nef_pipelines/tests/nmrview/tcl_diag.html
 src/nef_pipelines/tests/nmrview/test_export_peaks.py
 src/nef_pipelines/tests/nmrview/test_export_sequences.py
 src/nef_pipelines/tests/nmrview/test_import_peaks.py
@@ -180,14 +190,15 @@
 src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
 src/nef_pipelines/tests/nmrview/test_data/ppm.out
 src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
 src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
 src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
 src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
 src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+src/nef_pipelines/tests/pales/__init__.py
 src/nef_pipelines/tests/pales/test_rdcs.py
 src/nef_pipelines/tests/pales/test_template.py
 src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
 src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
 src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
 src/nef_pipelines/tests/rcsb/__init__.py
 src/nef_pipelines/tests/rcsb/test_rcsb_parsers.py
@@ -196,18 +207,18 @@
 src/nef_pipelines/tests/rcsb/test_data/1l2y_short.pdb
 src/nef_pipelines/tests/rcsb/test_data/3a_ab.pdb
 src/nef_pipelines/tests/rcsb/test_data/3a_cccc_dddd.pdb
 src/nef_pipelines/tests/rcsb/test_data/3a_no_chain_no_segid.pdb
 src/nef_pipelines/tests/rcsb/test_data/3aa.pdb
 src/nef_pipelines/tests/rcsb/test_data/3aa11_13.pdb
 src/nef_pipelines/tests/rcsb/test_data/test_header_entry.txt
-src/nef_pipelines/tests/shifts/__init__.py
-src/nef_pipelines/tests/shifts/test_make_peaks.py
 src/nef_pipelines/tests/shifty/__init__.py
 src/nef_pipelines/tests/shifty/test_export_shifts.py
+src/nef_pipelines/tests/simulate/__init__.py
+src/nef_pipelines/tests/simulate/test_simulate_peaks.py
 src/nef_pipelines/tests/sparky/__init__.py
 src/nef_pipelines/tests/sparky/test_export_peaks.py
 src/nef_pipelines/tests/sparky/test_import_peaks.py
 src/nef_pipelines/tests/sparky/test_import_sequence.py
 src/nef_pipelines/tests/sparky/test_import_shifts.py
 src/nef_pipelines/tests/sparky/test_sparky_lib.py
 src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
@@ -240,29 +251,32 @@
 src/nef_pipelines/tests/talos/test_data/pred_4_seq_first_resid_2.nef
 src/nef_pipelines/tests/talos/test_data/protonated_his.nef
 src/nef_pipelines/tests/talos/test_data/ubi_4.nef
 src/nef_pipelines/tests/talos/test_data/ubi_4_offset_1.nef
 src/nef_pipelines/tests/test_data/3a_ab.neff
 src/nef_pipelines/tests/test_data/empty.nef
 src/nef_pipelines/tests/test_data/header.nef
+src/nef_pipelines/tests/test_data/multi.nef
 src/nef_pipelines/tests/test_data/multi_chain.nef
 src/nef_pipelines/tests/test_data/nef_3_peaks.nef
 src/nef_pipelines/tests/test_data/tailin_seq_short.nef
 src/nef_pipelines/tests/test_data/test_agv.neff
 src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+src/nef_pipelines/tests/xcamshift/__init__.py
 src/nef_pipelines/tests/xcamshift/test_export_shifts.py
 src/nef_pipelines/tests/xeasy/__init__.py
 src/nef_pipelines/tests/xeasy/test_import_peaks.py
 src/nef_pipelines/tests/xeasy/test_import_sequence.py
 src/nef_pipelines/tests/xeasy/test_import_shifts.py
 src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
 src/nef_pipelines/tests/xeasy/test_data/basic.peaks
 src/nef_pipelines/tests/xeasy/test_data/basic.seq
 src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
 src/nef_pipelines/tests/xeasy/test_data/basic_shifts.prot
+src/nef_pipelines/tests/xplor/__init__.py
 src/nef_pipelines/tests/xplor/test_dihedrals.py
 src/nef_pipelines/tests/xplor/test_distances.py
 src/nef_pipelines/tests/xplor/test_export_rdcs.py
 src/nef_pipelines/tests/xplor/test_import_sequence.py
 src/nef_pipelines/tests/xplor/test_psf_lib.py
 src/nef_pipelines/tests/xplor/test_xplor_lib.py
 src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
@@ -280,36 +294,42 @@
 src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
 src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
 src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
 src/nef_pipelines/tools/about.py
 src/nef_pipelines/tools/header.py
 src/nef_pipelines/tools/offset_shifts.py
 src/nef_pipelines/tools/res_assign.py_unused
+src/nef_pipelines/tools/save.py
 src/nef_pipelines/tools/sink.py
 src/nef_pipelines/tools/stream.py
 src/nef_pipelines/tools/test.py
 src/nef_pipelines/tools/chains/__init__.py
 src/nef_pipelines/tools/chains/clone.py
 src/nef_pipelines/tools/chains/list.py
 src/nef_pipelines/tools/chains/rename.py
 src/nef_pipelines/tools/chains/renumber.py
 src/nef_pipelines/tools/entry/__init__.py
 src/nef_pipelines/tools/entry/rename.py
+src/nef_pipelines/tools/fit/__init__.py
+src/nef_pipelines/tools/fit/exponential.py
 src/nef_pipelines/tools/frames/__init__.py
 src/nef_pipelines/tools/frames/delete.py
 src/nef_pipelines/tools/frames/filter.py
 src/nef_pipelines/tools/frames/insert.py
 src/nef_pipelines/tools/frames/list.py
 src/nef_pipelines/tools/frames/rename.py
 src/nef_pipelines/tools/frames/tabulate.py
 src/nef_pipelines/tools/frames/unassign.py
 src/nef_pipelines/tools/peaks/__init__.py
 src/nef_pipelines/tools/peaks/match.py
-src/nef_pipelines/tools/shifts/__init__.py
-src/nef_pipelines/tools/shifts/make_peaks.py
+src/nef_pipelines/tools/series/__init__.py
+src/nef_pipelines/tools/series/build.py
+src/nef_pipelines/tools/simulate/__init__.py
+src/nef_pipelines/tools/simulate/peaks.py
+src/nef_pipelines/tools/simulate/unlabelling.py
 src/nef_pipelines/transcoders/__init__.py
 src/nef_pipelines/transcoders/csv/__init__.py
 src/nef_pipelines/transcoders/csv/importers/__init__.py
 src/nef_pipelines/transcoders/csv/importers/peaks.py
 src/nef_pipelines/transcoders/csv/importers/rdcs.py
 src/nef_pipelines/transcoders/echidna/__init__.py
 src/nef_pipelines/transcoders/echidna/importers/__init__.py
@@ -323,14 +343,15 @@
 src/nef_pipelines/transcoders/mars/exporters/__init__.py
 src/nef_pipelines/transcoders/mars/exporters/fragments.py
 src/nef_pipelines/transcoders/mars/exporters/input.py
 src/nef_pipelines/transcoders/mars/exporters/sequence.py
 src/nef_pipelines/transcoders/mars/exporters/shifts.py
 src/nef_pipelines/transcoders/mars/importers/__init__.py
 src/nef_pipelines/transcoders/mars/importers/peaks.py
+src/nef_pipelines/transcoders/mars/importers/sequence.py
 src/nef_pipelines/transcoders/mars/importers/shifts.py
 src/nef_pipelines/transcoders/nmrpipe/__init__.py
 src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
 src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
 src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
 src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
 src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
```

### Comparing `nef_pipelines-0.1.65/tox.ini` & `nef_pipelines-0.1.66/tox.ini`

 * *Files identical despite different names*

