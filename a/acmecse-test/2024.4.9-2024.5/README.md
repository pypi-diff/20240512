# Comparing `tmp/acmecse_test-2024.4.9-py3-none-any.whl.zip` & `tmp/acmecse_test-2024.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,269 @@
-Zip file size: 6384 bytes, number of entries: 8
--rw-r--r--  2.0 unx      228 b- defN 23-Oct-22 10:32 acme/__init__.py
--rw-r--r--  2.0 unx     6439 b- defN 24-May-03 09:42 acme/__main__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-04 11:05 acmecse_test-2024.4.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     3853 b- defN 24-May-04 11:05 acmecse_test-2024.4.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-04 11:05 acmecse_test-2024.4.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 24-May-04 11:05 acmecse_test-2024.4.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-04 11:05 acmecse_test-2024.4.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      673 b- defN 24-May-04 11:05 acmecse_test-2024.4.9.dist-info/RECORD
-8 files, 12859 bytes uncompressed, 5196 bytes compressed:  59.6%
+Zip file size: 1022771 bytes, number of entries: 267
+-rw-r--r--  2.0 unx      228 b- defN 24-May-12 11:51 acmecse/__init__.py
+-rw-r--r--  2.0 unx     6439 b- defN 24-May-12 11:51 acmecse/__main__.py
+-rw-r--r--  2.0 unx    13656 b- defN 24-May-12 11:51 acmecse/databases/DBBinding.py
+-rw-r--r--  2.0 unx    29567 b- defN 24-May-12 11:51 acmecse/databases/PostgreSQLBinding.py
+-rw-r--r--  2.0 unx    24419 b- defN 24-May-12 11:51 acmecse/databases/TinyDBBinding.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-12 11:51 acmecse/databases/__init__.py
+-rw-r--r--  2.0 unx    21130 b- defN 24-May-12 11:51 acmecse/etc/ACMEUtils.py
+-rw-r--r--  2.0 unx     5368 b- defN 24-May-12 11:51 acmecse/etc/Constants.py
+-rw-r--r--  2.0 unx    13243 b- defN 24-May-12 11:51 acmecse/etc/DateUtils.py
+-rw-r--r--  2.0 unx     4770 b- defN 24-May-12 11:51 acmecse/etc/GeoTools.py
+-rw-r--r--  2.0 unx    11717 b- defN 24-May-12 11:51 acmecse/etc/RequestUtils.py
+-rw-r--r--  2.0 unx    23264 b- defN 24-May-12 11:51 acmecse/etc/ResponseStatusCodes.py
+-rw-r--r--  2.0 unx    82053 b- defN 24-May-12 11:51 acmecse/etc/Types.py
+-rw-r--r--  2.0 unx     5292 b- defN 24-May-12 11:51 acmecse/etc/Utils.py
+-rw-r--r--  2.0 unx       67 b- defN 24-May-12 11:51 acmecse/etc/__init__.py
+-rw-r--r--  2.0 unx     2635 b- defN 24-May-12 11:51 acmecse/helpers/ACMEIntEnum.py
+-rw-r--r--  2.0 unx    30479 b- defN 24-May-12 11:51 acmecse/helpers/BackgroundWorker.py
+-rw-r--r--  2.0 unx    13186 b- defN 24-May-12 11:51 acmecse/helpers/CoapDissector.py
+-rw-r--r--  2.0 unx     6839 b- defN 24-May-12 11:51 acmecse/helpers/EventManager.py
+-rw-r--r--  2.0 unx   116610 b- defN 24-May-12 11:51 acmecse/helpers/Interpreter.py
+-rw-r--r--  2.0 unx    17600 b- defN 24-May-12 11:51 acmecse/helpers/KeyHandler.py
+-rw-r--r--  2.0 unx    20897 b- defN 24-May-12 11:51 acmecse/helpers/MQTTConnection.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-12 11:51 acmecse/helpers/NetworkTools.py
+-rw-r--r--  2.0 unx     2061 b- defN 24-May-12 11:51 acmecse/helpers/OAuth.py
+-rw-r--r--  2.0 unx      562 b- defN 24-May-12 11:51 acmecse/helpers/OrderedSet.py
+-rw-r--r--  2.0 unx     4761 b- defN 24-May-12 11:51 acmecse/helpers/ReadWriteLock.py
+-rw-r--r--  2.0 unx     3894 b- defN 24-May-12 11:51 acmecse/helpers/ResourceSemaphore.py
+-rw-r--r--  2.0 unx    15579 b- defN 24-May-12 11:51 acmecse/helpers/TextTools.py
+-rw-r--r--  2.0 unx     1180 b- defN 24-May-12 11:51 acmecse/helpers/ThreadSafeCounter.py
+-rw-r--r--  2.0 unx     2385 b- defN 24-May-12 11:51 acmecse/helpers/TinyDBBetterTable.py
+-rw-r--r--  2.0 unx     4219 b- defN 24-May-12 11:51 acmecse/helpers/TinyDBBufferedStorage.py
+-rw-r--r--  2.0 unx     9991 b- defN 24-May-12 11:51 acmecse/helpers/UDPServer.py
+-rw-r--r--  2.0 unx      104 b- defN 24-May-12 11:51 acmecse/helpers/__init__.py
+-rw-r--r--  2.0 unx     1741 b- defN 24-May-12 11:51 acmecse/init/ASFunctions.as
+-rw-r--r--  2.0 unx    21001 b- defN 24-May-12 11:51 acmecse/init/acme.ini.default
+-rw-r--r--  2.0 unx      758 b- defN 24-May-12 11:51 acmecse/init/action.as_
+-rw-r--r--  2.0 unx      437 b- defN 24-May-12 11:51 acmecse/init/action2.as
+-rw-r--r--  2.0 unx       85 b- defN 24-May-12 11:51 acmecse/init/action3.as_
+-rw-r--r--  2.0 unx     2207 b- defN 24-May-12 11:51 acmecse/init/agd-dev.fcp
+-rw-r--r--  2.0 unx     2719 b- defN 24-May-12 11:51 acmecse/init/agd-mc.fcp
+-rw-r--r--  2.0 unx    66620 b- defN 24-May-12 11:51 acmecse/init/attributePolicies.ap
+-rw-r--r--  2.0 unx     9646 b- defN 24-May-12 11:51 acmecse/init/attributePolicies.fcp
+-rw-r--r--  2.0 unx     1329 b- defN 24-May-12 11:51 acmecse/init/bla.as
+-rw-r--r--  2.0 unx    18313 b- defN 24-May-12 11:51 acmecse/init/cid-dev.fcp
+-rw-r--r--  2.0 unx    38892 b- defN 24-May-12 11:51 acmecse/init/cod-dev.fcp
+-rw-r--r--  2.0 unx   397091 b- defN 24-May-12 11:51 acmecse/init/cod-mc.fcp
+-rw-r--r--  2.0 unx     1292 b- defN 24-May-12 11:51 acmecse/init/cod-sdev.fcp
+-rw-r--r--  2.0 unx    34667 b- defN 24-May-12 11:51 acmecse/init/complexTypePolicies.ap
+-rw-r--r--  2.0 unx    40517 b- defN 24-May-12 11:51 acmecse/init/configurations.docmd
+-rw-r--r--  2.0 unx     1304 b- defN 24-May-12 11:51 acmecse/init/covid.fcp
+-rw-r--r--  2.0 unx      793 b- defN 24-May-12 11:51 acmecse/init/curve.as
+-rw-r--r--  2.0 unx    13849 b- defN 24-May-12 11:51 acmecse/init/enumTypesPolicies.ep
+-rw-r--r--  2.0 unx      538 b- defN 24-May-12 11:51 acmecse/init/getConfigurationUT.as
+-rw-r--r--  2.0 unx    10163 b- defN 24-May-12 11:51 acmecse/init/hed-dev.fcp
+-rw-r--r--  2.0 unx       90 b- defN 24-May-12 11:51 acmecse/init/hed-mc.fcp
+-rw-r--r--  2.0 unx     1147 b- defN 24-May-12 11:51 acmecse/init/hed-sdev.fcp
+-rw-r--r--  2.0 unx    67896 b- defN 24-May-12 11:51 acmecse/init/hod-dev.fcp
+-rw-r--r--  2.0 unx       88 b- defN 24-May-12 11:51 acmecse/init/hod-mc.fcp
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 11:51 acmecse/init/ind-dev.fcp
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 11:51 acmecse/init/ind-mc.fcp
+-rw-r--r--  2.0 unx     1849 b- defN 24-May-12 11:51 acmecse/init/init.as
+-rw-r--r--  2.0 unx      850 b- defN 24-May-12 11:51 acmecse/init/iotOrchestrator.fcp
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-12 11:51 acmecse/init/mad-dev.fcp
+-rw-r--r--  2.0 unx    68005 b- defN 24-May-12 11:51 acmecse/init/mad-mc.fcp
+-rw-r--r--  2.0 unx      999 b- defN 24-May-12 11:51 acmecse/init/mad-sdev.fcp
+-rw-r--r--  2.0 unx    11467 b- defN 24-May-12 11:51 acmecse/init/mdd-mc.fcp
+-rw-r--r--  2.0 unx      255 b- defN 24-May-12 11:51 acmecse/init/melodyImperial.as
+-rw-r--r--  2.0 unx      254 b- defN 24-May-12 11:51 acmecse/init/melodyTheme.as
+-rw-r--r--  2.0 unx     3795 b- defN 24-May-12 11:51 acmecse/init/psd-dev.fcp
+-rw-r--r--  2.0 unx    20221 b- defN 24-May-12 11:51 acmecse/init/psd-mc.fcp
+-rw-r--r--  2.0 unx      403 b- defN 24-May-12 11:51 acmecse/init/query.as
+-rw-r--r--  2.0 unx    14074 b- defN 24-May-12 11:51 acmecse/init/rad-dev.fcp
+-rw-r--r--  2.0 unx     2385 b- defN 24-May-12 11:51 acmecse/init/rad-mc.fcp
+-rw-r--r--  2.0 unx      243 b- defN 24-May-12 11:51 acmecse/init/rebootWemos.as
+-rw-r--r--  2.0 unx     2317 b- defN 24-May-12 11:51 acmecse/init/ved-dev.fcp
+-rw-r--r--  2.0 unx       93 b- defN 24-May-12 11:51 acmecse/init/ved-mc.fcp
+-rw-r--r--  2.0 unx      954 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/hacksterIO.as
+-rw-r--r--  2.0 unx      685 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/init.as
+-rw-r--r--  2.0 unx      918 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/jupyterNotebooksLive.as
+-rw-r--r--  2.0 unx      750 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/jupyterNotebooksWiki.as
+-rw-r--r--  2.0 unx      840 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/oneM2MHomePage.as
+-rw-r--r--  2.0 unx      774 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/oneM2MIntroduction.as
+-rw-r--r--  2.0 unx      776 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/oneM2MSpecifications.as
+-rw-r--r--  2.0 unx      887 b- defN 24-May-12 11:51 acmecse/init/demoDocumentationTutorials/stackOverflow.as
+-rw-r--r--  2.0 unx     4544 b- defN 24-May-12 11:51 acmecse/init/demoLightbulb/init.as
+-rw-r--r--  2.0 unx     3225 b- defN 24-May-12 11:51 acmecse/init/demoLightbulb/lighbulb.as
+-rw-r--r--  2.0 unx     4329 b- defN 24-May-12 11:51 acmecse/init/demoLightbulb/toggleLightswitch.as
+-rw-r--r--  2.0 unx      492 b- defN 24-May-12 11:51 acmecse/init/system.scripts/utReset.as
+-rw-r--r--  2.0 unx      350 b- defN 24-May-12 11:51 acmecse/init/system.scripts/utStatus.as
+-rw-r--r--  2.0 unx      464 b- defN 24-May-12 11:51 acmecse/init/testing.scripts/testCaseEnd.as
+-rw-r--r--  2.0 unx      512 b- defN 24-May-12 11:51 acmecse/init/testing.scripts/testCaseStart.as
+-rw-r--r--  2.0 unx      478 b- defN 24-May-12 11:51 acmecse/init/testing.scripts/testsDisableShortRequestExpiration.as
+-rw-r--r--  2.0 unx      526 b- defN 24-May-12 11:51 acmecse/init/testing.scripts/testsDisableShortResourceExpiration.as
+-rw-r--r--  2.0 unx      601 b- defN 24-May-12 11:51 acmecse/init/testing.scripts/testsEnableShortRequestExpiration.as
+-rw-r--r--  2.0 unx      800 b- defN 24-May-12 11:51 acmecse/init/testing.scripts/testsEnableShortResourceExpiration.as
+-rw-r--r--  2.0 unx      665 b- defN 24-May-12 11:51 acmecse/init/utilities.scripts/utilAttributeInfo.as
+-rw-r--r--  2.0 unx    17392 b- defN 24-May-12 11:51 acmecse/protocols/CoAPServer.py
+-rw-r--r--  2.0 unx    34997 b- defN 24-May-12 11:51 acmecse/protocols/HttpServer.py
+-rw-r--r--  2.0 unx    21875 b- defN 24-May-12 11:51 acmecse/protocols/MQTTClient.py
+-rw-r--r--  2.0 unx    24687 b- defN 24-May-12 11:51 acmecse/protocols/WebSocketServer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-12 11:51 acmecse/protocols/__init__.py
+-rw-r--r--  2.0 unx     8566 b- defN 24-May-12 11:51 acmecse/resources/ACP.py
+-rw-r--r--  2.0 unx     2327 b- defN 24-May-12 11:51 acmecse/resources/ACPAnnc.py
+-rw-r--r--  2.0 unx     9144 b- defN 24-May-12 11:51 acmecse/resources/ACTR.py
+-rw-r--r--  2.0 unx     1376 b- defN 24-May-12 11:51 acmecse/resources/ACTRAnnc.py
+-rw-r--r--  2.0 unx     5613 b- defN 24-May-12 11:51 acmecse/resources/AE.py
+-rw-r--r--  2.0 unx     1982 b- defN 24-May-12 11:51 acmecse/resources/AEAnnc.py
+-rw-r--r--  2.0 unx     1411 b- defN 24-May-12 11:51 acmecse/resources/ANDI.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-12 11:51 acmecse/resources/ANDIAnnc.py
+-rw-r--r--  2.0 unx     1309 b- defN 24-May-12 11:51 acmecse/resources/ANI.py
+-rw-r--r--  2.0 unx     1254 b- defN 24-May-12 11:51 acmecse/resources/ANIAnnc.py
+-rw-r--r--  2.0 unx    11189 b- defN 24-May-12 11:51 acmecse/resources/AnnounceableResource.py
+-rw-r--r--  2.0 unx     1767 b- defN 24-May-12 11:51 acmecse/resources/AnnouncedResource.py
+-rw-r--r--  2.0 unx     1471 b- defN 24-May-12 11:51 acmecse/resources/BAT.py
+-rw-r--r--  2.0 unx     1244 b- defN 24-May-12 11:51 acmecse/resources/BATAnnc.py
+-rw-r--r--  2.0 unx     4679 b- defN 24-May-12 11:51 acmecse/resources/CIN.py
+-rw-r--r--  2.0 unx     1389 b- defN 24-May-12 11:51 acmecse/resources/CINAnnc.py
+-rw-r--r--  2.0 unx    10133 b- defN 24-May-12 11:51 acmecse/resources/CNT.py
+-rw-r--r--  2.0 unx     1731 b- defN 24-May-12 11:51 acmecse/resources/CNTAnnc.py
+-rw-r--r--  2.0 unx     4729 b- defN 24-May-12 11:51 acmecse/resources/CNT_LA.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-12 11:51 acmecse/resources/CNT_OL.py
+-rw-r--r--  2.0 unx    17628 b- defN 24-May-12 11:51 acmecse/resources/CRS.py
+-rw-r--r--  2.0 unx     4663 b- defN 24-May-12 11:51 acmecse/resources/CSEBase.py
+-rw-r--r--  2.0 unx     1590 b- defN 24-May-12 11:51 acmecse/resources/CSEBaseAnnc.py
+-rw-r--r--  2.0 unx     3705 b- defN 24-May-12 11:51 acmecse/resources/CSR.py
+-rw-r--r--  2.0 unx     2096 b- defN 24-May-12 11:51 acmecse/resources/CSRAnnc.py
+-rw-r--r--  2.0 unx     2766 b- defN 24-May-12 11:51 acmecse/resources/ContainerResource.py
+-rw-r--r--  2.0 unx     2180 b- defN 24-May-12 11:51 acmecse/resources/DATC.py
+-rw-r--r--  2.0 unx     1186 b- defN 24-May-12 11:51 acmecse/resources/DATCAnnc.py
+-rw-r--r--  2.0 unx     3424 b- defN 24-May-12 11:51 acmecse/resources/DEPR.py
+-rw-r--r--  2.0 unx     1276 b- defN 24-May-12 11:51 acmecse/resources/DEPRAnnc.py
+-rw-r--r--  2.0 unx     2578 b- defN 24-May-12 11:51 acmecse/resources/DVC.py
+-rw-r--r--  2.0 unx     1175 b- defN 24-May-12 11:51 acmecse/resources/DVCAnnc.py
+-rw-r--r--  2.0 unx     1396 b- defN 24-May-12 11:51 acmecse/resources/DVI.py
+-rw-r--r--  2.0 unx     1389 b- defN 24-May-12 11:51 acmecse/resources/DVIAnnc.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-12 11:51 acmecse/resources/EVL.py
+-rw-r--r--  2.0 unx     1162 b- defN 24-May-12 11:51 acmecse/resources/EVLAnnc.py
+-rw-r--r--  2.0 unx     1385 b- defN 24-May-12 11:51 acmecse/resources/FCI.py
+-rw-r--r--  2.0 unx    13218 b- defN 24-May-12 11:51 acmecse/resources/FCNT.py
+-rw-r--r--  2.0 unx     1694 b- defN 24-May-12 11:51 acmecse/resources/FCNTAnnc.py
+-rw-r--r--  2.0 unx     3776 b- defN 24-May-12 11:51 acmecse/resources/FCNT_LA.py
+-rw-r--r--  2.0 unx     3780 b- defN 24-May-12 11:51 acmecse/resources/FCNT_OL.py
+-rw-r--r--  2.0 unx     1391 b- defN 24-May-12 11:51 acmecse/resources/FWR.py
+-rw-r--r--  2.0 unx     1043 b- defN 24-May-12 11:51 acmecse/resources/FWRAnnc.py
+-rw-r--r--  2.0 unx    17068 b- defN 24-May-12 11:51 acmecse/resources/Factory.py
+-rw-r--r--  2.0 unx     2742 b- defN 24-May-12 11:51 acmecse/resources/GRP.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-12 11:51 acmecse/resources/GRPAnnc.py
+-rw-r--r--  2.0 unx     2220 b- defN 24-May-12 11:51 acmecse/resources/GRP_FOPT.py
+-rw-r--r--  2.0 unx     7838 b- defN 24-May-12 11:51 acmecse/resources/LCP.py
+-rw-r--r--  2.0 unx     1485 b- defN 24-May-12 11:51 acmecse/resources/LCPAnnc.py
+-rw-r--r--  2.0 unx     1104 b- defN 24-May-12 11:51 acmecse/resources/MEM.py
+-rw-r--r--  2.0 unx     1115 b- defN 24-May-12 11:51 acmecse/resources/MEMAnnc.py
+-rw-r--r--  2.0 unx     1271 b- defN 24-May-12 11:51 acmecse/resources/MNWK.py
+-rw-r--r--  2.0 unx     1270 b- defN 24-May-12 11:51 acmecse/resources/MNWKAnnc.py
+-rw-r--r--  2.0 unx      767 b- defN 24-May-12 11:51 acmecse/resources/MgmtObj.py
+-rw-r--r--  2.0 unx      794 b- defN 24-May-12 11:51 acmecse/resources/MgmtObjAnnc.py
+-rw-r--r--  2.0 unx     2082 b- defN 24-May-12 11:51 acmecse/resources/NOD.py
+-rw-r--r--  2.0 unx     1353 b- defN 24-May-12 11:51 acmecse/resources/NODAnnc.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-May-12 11:51 acmecse/resources/NYCFC.py
+-rw-r--r--  2.0 unx     1141 b- defN 24-May-12 11:51 acmecse/resources/NYCFCAnnc.py
+-rw-r--r--  2.0 unx     4262 b- defN 24-May-12 11:51 acmecse/resources/PCH.py
+-rw-r--r--  2.0 unx     5899 b- defN 24-May-12 11:51 acmecse/resources/PCH_PCU.py
+-rw-r--r--  2.0 unx     6751 b- defN 24-May-12 11:51 acmecse/resources/PRMR.py
+-rw-r--r--  2.0 unx     2399 b- defN 24-May-12 11:51 acmecse/resources/RBO.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-12 11:51 acmecse/resources/RBOAnnc.py
+-rw-r--r--  2.0 unx     3582 b- defN 24-May-12 11:51 acmecse/resources/REQ.py
+-rw-r--r--  2.0 unx    38258 b- defN 24-May-12 11:51 acmecse/resources/Resource.py
+-rw-r--r--  2.0 unx     4554 b- defN 24-May-12 11:51 acmecse/resources/SCH.py
+-rw-r--r--  2.0 unx     1324 b- defN 24-May-12 11:51 acmecse/resources/SCHAnnc.py
+-rw-r--r--  2.0 unx     1165 b- defN 24-May-12 11:51 acmecse/resources/SIM.py
+-rw-r--r--  2.0 unx     1165 b- defN 24-May-12 11:51 acmecse/resources/SIMAnnc.py
+-rw-r--r--  2.0 unx     4761 b- defN 24-May-12 11:51 acmecse/resources/SMD.py
+-rw-r--r--  2.0 unx     1168 b- defN 24-May-12 11:51 acmecse/resources/SMDAnnc.py
+-rw-r--r--  2.0 unx     1285 b- defN 24-May-12 11:51 acmecse/resources/STTE.py
+-rw-r--r--  2.0 unx    13263 b- defN 24-May-12 11:51 acmecse/resources/SUB.py
+-rw-r--r--  2.0 unx     1811 b- defN 24-May-12 11:51 acmecse/resources/SWR.py
+-rw-r--r--  2.0 unx     1271 b- defN 24-May-12 11:51 acmecse/resources/SWRAnnc.py
+-rw-r--r--  2.0 unx    17184 b- defN 24-May-12 11:51 acmecse/resources/TS.py
+-rw-r--r--  2.0 unx     1356 b- defN 24-May-12 11:51 acmecse/resources/TSAnnc.py
+-rw-r--r--  2.0 unx     4725 b- defN 24-May-12 11:51 acmecse/resources/TSB.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-12 11:51 acmecse/resources/TSBAnnc.py
+-rw-r--r--  2.0 unx     1592 b- defN 24-May-12 11:51 acmecse/resources/TSI.py
+-rw-r--r--  2.0 unx     1156 b- defN 24-May-12 11:51 acmecse/resources/TSIAnnc.py
+-rw-r--r--  2.0 unx     3704 b- defN 24-May-12 11:51 acmecse/resources/TS_LA.py
+-rw-r--r--  2.0 unx     3654 b- defN 24-May-12 11:51 acmecse/resources/TS_OL.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-12 11:51 acmecse/resources/Unknown.py
+-rw-r--r--  2.0 unx     1712 b- defN 24-May-12 11:51 acmecse/resources/VirtualResource.py
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-12 11:51 acmecse/resources/WIFIC.py
+-rw-r--r--  2.0 unx     1271 b- defN 24-May-12 11:51 acmecse/resources/WIFICAnnc.py
+-rw-r--r--  2.0 unx       69 b- defN 24-May-12 11:51 acmecse/resources/__init__.py
+-rw-r--r--  2.0 unx    16051 b- defN 24-May-12 11:51 acmecse/runtime/CSE.py
+-rw-r--r--  2.0 unx    56759 b- defN 24-May-12 11:51 acmecse/runtime/Configuration.py
+-rw-r--r--  2.0 unx    59065 b- defN 24-May-12 11:51 acmecse/runtime/Console.py
+-rw-r--r--  2.0 unx    27163 b- defN 24-May-12 11:51 acmecse/runtime/Importer.py
+-rw-r--r--  2.0 unx    24779 b- defN 24-May-12 11:51 acmecse/runtime/Logging.py
+-rw-r--r--  2.0 unx    18463 b- defN 24-May-12 11:51 acmecse/runtime/Onboarding.py
+-rw-r--r--  2.0 unx    71323 b- defN 24-May-12 11:51 acmecse/runtime/ScriptManager.py
+-rw-r--r--  2.0 unx    17617 b- defN 24-May-12 11:51 acmecse/runtime/Statistics.py
+-rw-r--r--  2.0 unx    25899 b- defN 24-May-12 11:51 acmecse/runtime/Storage.py
+-rw-r--r--  2.0 unx     5753 b- defN 24-May-12 11:51 acmecse/runtime/TextUI.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-12 11:51 acmecse/runtime/__init__.py
+-rw-r--r--  2.0 unx    12149 b- defN 24-May-12 11:51 acmecse/services/ActionManager.py
+-rw-r--r--  2.0 unx    20537 b- defN 24-May-12 11:51 acmecse/services/AnnouncementManager.py
+-rw-r--r--  2.0 unx    71700 b- defN 24-May-12 11:51 acmecse/services/Dispatcher.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-12 11:51 acmecse/services/EventManager.py
+-rw-r--r--  2.0 unx    11963 b- defN 24-May-12 11:51 acmecse/services/GroupManager.py
+-rw-r--r--  2.0 unx    13602 b- defN 24-May-12 11:51 acmecse/services/LocationManager.py
+-rw-r--r--  2.0 unx    52183 b- defN 24-May-12 11:51 acmecse/services/NotificationManager.py
+-rw-r--r--  2.0 unx    16021 b- defN 24-May-12 11:51 acmecse/services/RegistrationManager.py
+-rw-r--r--  2.0 unx    35391 b- defN 24-May-12 11:51 acmecse/services/RemoteCSEManager.py
+-rw-r--r--  2.0 unx    68573 b- defN 24-May-12 11:51 acmecse/services/RequestManager.py
+-rw-r--r--  2.0 unx    24356 b- defN 24-May-12 11:51 acmecse/services/SecurityManager.py
+-rw-r--r--  2.0 unx    22665 b- defN 24-May-12 11:51 acmecse/services/SemanticManager.py
+-rw-r--r--  2.0 unx     7061 b- defN 24-May-12 11:51 acmecse/services/TimeManager.py
+-rw-r--r--  2.0 unx    10985 b- defN 24-May-12 11:51 acmecse/services/TimeSeriesManager.py
+-rw-r--r--  2.0 unx    37526 b- defN 24-May-12 11:51 acmecse/services/Validator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-12 11:51 acmecse/services/__init__.py
+-rw-r--r--  2.0 unx     5234 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerAbout.py
+-rw-r--r--  2.0 unx     4713 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerConfigurations.py
+-rw-r--r--  2.0 unx     4095 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerDelete.py
+-rw-r--r--  2.0 unx    10050 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerDiagram.py
+-rw-r--r--  2.0 unx     1230 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerInfo.py
+-rw-r--r--  2.0 unx      948 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerRegistrations.py
+-rw-r--r--  2.0 unx     9741 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerRequests.py
+-rw-r--r--  2.0 unx     7435 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerResourceServices.py
+-rw-r--r--  2.0 unx    13802 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerTools.py
+-rw-r--r--  2.0 unx    14558 b- defN 24-May-12 11:51 acmecse/textui/ACMEContainerTree.py
+-rw-r--r--  2.0 unx     4292 b- defN 24-May-12 11:51 acmecse/textui/ACMEFieldOriginator.py
+-rw-r--r--  2.0 unx     1732 b- defN 24-May-12 11:51 acmecse/textui/ACMEHeader.py
+-rw-r--r--  2.0 unx     1215 b- defN 24-May-12 11:51 acmecse/textui/ACMETUI.css
+-rw-r--r--  2.0 unx     8215 b- defN 24-May-12 11:51 acmecse/textui/ACMETuiApp.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-12 11:51 acmecse/textui/__init__.py
+-rw-r--r--  2.0 unx       69 b- defN 24-May-12 11:51 acmecse/webui/__init__.py
+-rw-r--r--  2.0 unx    13775 b- defN 24-May-12 11:51 acmecse/webui/webUI.py
+-rw-r--r--  2.0 unx     4003 b- defN 24-May-12 11:51 acmecse/webui/web/index-sl.html
+-rw-r--r--  2.0 unx     8894 b- defN 24-May-12 11:51 acmecse/webui/web/index.html
+-rwxr-xr-x  2.0 unx     1645 b- defN 24-May-12 11:51 acmecse/webui/web/css/contextmenu.css
+-rw-r--r--  2.0 unx    57352 b- defN 24-May-12 11:51 acmecse/webui/web/css/picnic.css
+-rw-r--r--  2.0 unx     2157 b- defN 24-May-12 11:51 acmecse/webui/web/css/style.css
+-rw-r--r--  2.0 unx     1440 b- defN 24-May-12 11:51 acmecse/webui/web/css/treejs.css
+-rw-r--r--  2.0 unx    31485 b- defN 24-May-12 11:51 acmecse/webui/web/img/acme.png
+-rw-r--r--  2.0 unx     4302 b- defN 24-May-12 11:51 acmecse/webui/web/img/acme.t2d
+-rw-r--r--  2.0 unx    15106 b- defN 24-May-12 11:51 acmecse/webui/web/img/acme_sm.png
+-rw-r--r--  2.0 unx    41918 b- defN 24-May-12 11:51 acmecse/webui/web/img/acme_sq.png
+-rw-r--r--  2.0 unx    43352 b- defN 24-May-12 11:51 acmecse/webui/web/img/acme_sq_white.png
+-rw-r--r--  2.0 unx     3198 b- defN 24-May-12 11:51 acmecse/webui/web/img/badge-acme.png
+-rw-r--r--  2.0 unx     1911 b- defN 24-May-12 11:51 acmecse/webui/web/img/favicon.png
+-rw-r--r--  2.0 unx   126976 b- defN 24-May-12 11:51 acmecse/webui/web/img/badge-acme.pxd/metadata.info
+-rw-r--r--  2.0 unx     5016 b- defN 24-May-12 11:51 acmecse/webui/web/img/badge-acme.pxd/QuickLook/Icon.tiff
+-rw-r--r--  2.0 unx     5616 b- defN 24-May-12 11:51 acmecse/webui/web/img/badge-acme.pxd/QuickLook/Thumbnail.tiff
+-rw-r--r--  2.0 unx   131072 b- defN 24-May-12 11:51 acmecse/webui/web/img/favicon.pxd/metadata.info
+-rw-r--r--  2.0 unx    10768 b- defN 24-May-12 11:51 acmecse/webui/web/img/favicon.pxd/QuickLook/Icon.tiff
+-rw-r--r--  2.0 unx   200980 b- defN 24-May-12 11:51 acmecse/webui/web/img/favicon.pxd/QuickLook/Thumbnail.tiff
+-rw-r--r--  2.0 unx    12713 b- defN 24-May-12 11:51 acmecse/webui/web/js/attributes.js
+-rwxr-xr-x  2.0 unx     6386 b- defN 24-May-12 11:51 acmecse/webui/web/js/contextmenu.js
+-rw-r--r--  2.0 unx     9383 b- defN 24-May-12 11:51 acmecse/webui/web/js/main.js
+-rw-r--r--  2.0 unx     1974 b- defN 24-May-12 11:51 acmecse/webui/web/js/menu.js
+-rw-r--r--  2.0 unx     8995 b- defN 24-May-12 11:51 acmecse/webui/web/js/resourceTree.js
+-rw-r--r--  2.0 unx     1986 b- defN 24-May-12 11:51 acmecse/webui/web/js/rest.js
+-rw-r--r--  2.0 unx    15492 b- defN 24-May-12 11:51 acmecse/webui/web/js/restui.js
+-rw-r--r--  2.0 unx    14539 b- defN 24-May-12 11:51 acmecse/webui/web/js/tree.js
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-12 11:51 acmecse_test-2024.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2174 b- defN 24-May-12 11:51 acmecse_test-2024.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 11:51 acmecse_test-2024.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 24-May-12 11:51 acmecse_test-2024.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx      152 b- defN 24-May-12 11:51 acmecse_test-2024.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    23508 b- defN 24-May-12 11:51 acmecse_test-2024.5.dist-info/RECORD
+267 files, 3445253 bytes uncompressed, 985793 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -1,25 +1,802 @@
-Filename: acme/__init__.py
+Filename: acmecse/__init__.py
 Comment: 
 
-Filename: acme/__main__.py
+Filename: acmecse/__main__.py
 Comment: 
 
-Filename: acmecse_test-2024.4.9.dist-info/LICENSE
+Filename: acmecse/databases/DBBinding.py
 Comment: 
 
-Filename: acmecse_test-2024.4.9.dist-info/METADATA
+Filename: acmecse/databases/PostgreSQLBinding.py
 Comment: 
 
-Filename: acmecse_test-2024.4.9.dist-info/WHEEL
+Filename: acmecse/databases/TinyDBBinding.py
 Comment: 
 
-Filename: acmecse_test-2024.4.9.dist-info/entry_points.txt
+Filename: acmecse/databases/__init__.py
 Comment: 
 
-Filename: acmecse_test-2024.4.9.dist-info/top_level.txt
+Filename: acmecse/etc/ACMEUtils.py
 Comment: 
 
-Filename: acmecse_test-2024.4.9.dist-info/RECORD
+Filename: acmecse/etc/Constants.py
+Comment: 
+
+Filename: acmecse/etc/DateUtils.py
+Comment: 
+
+Filename: acmecse/etc/GeoTools.py
+Comment: 
+
+Filename: acmecse/etc/RequestUtils.py
+Comment: 
+
+Filename: acmecse/etc/ResponseStatusCodes.py
+Comment: 
+
+Filename: acmecse/etc/Types.py
+Comment: 
+
+Filename: acmecse/etc/Utils.py
+Comment: 
+
+Filename: acmecse/etc/__init__.py
+Comment: 
+
+Filename: acmecse/helpers/ACMEIntEnum.py
+Comment: 
+
+Filename: acmecse/helpers/BackgroundWorker.py
+Comment: 
+
+Filename: acmecse/helpers/CoapDissector.py
+Comment: 
+
+Filename: acmecse/helpers/EventManager.py
+Comment: 
+
+Filename: acmecse/helpers/Interpreter.py
+Comment: 
+
+Filename: acmecse/helpers/KeyHandler.py
+Comment: 
+
+Filename: acmecse/helpers/MQTTConnection.py
+Comment: 
+
+Filename: acmecse/helpers/NetworkTools.py
+Comment: 
+
+Filename: acmecse/helpers/OAuth.py
+Comment: 
+
+Filename: acmecse/helpers/OrderedSet.py
+Comment: 
+
+Filename: acmecse/helpers/ReadWriteLock.py
+Comment: 
+
+Filename: acmecse/helpers/ResourceSemaphore.py
+Comment: 
+
+Filename: acmecse/helpers/TextTools.py
+Comment: 
+
+Filename: acmecse/helpers/ThreadSafeCounter.py
+Comment: 
+
+Filename: acmecse/helpers/TinyDBBetterTable.py
+Comment: 
+
+Filename: acmecse/helpers/TinyDBBufferedStorage.py
+Comment: 
+
+Filename: acmecse/helpers/UDPServer.py
+Comment: 
+
+Filename: acmecse/helpers/__init__.py
+Comment: 
+
+Filename: acmecse/init/ASFunctions.as
+Comment: 
+
+Filename: acmecse/init/acme.ini.default
+Comment: 
+
+Filename: acmecse/init/action.as_
+Comment: 
+
+Filename: acmecse/init/action2.as
+Comment: 
+
+Filename: acmecse/init/action3.as_
+Comment: 
+
+Filename: acmecse/init/agd-dev.fcp
+Comment: 
+
+Filename: acmecse/init/agd-mc.fcp
+Comment: 
+
+Filename: acmecse/init/attributePolicies.ap
+Comment: 
+
+Filename: acmecse/init/attributePolicies.fcp
+Comment: 
+
+Filename: acmecse/init/bla.as
+Comment: 
+
+Filename: acmecse/init/cid-dev.fcp
+Comment: 
+
+Filename: acmecse/init/cod-dev.fcp
+Comment: 
+
+Filename: acmecse/init/cod-mc.fcp
+Comment: 
+
+Filename: acmecse/init/cod-sdev.fcp
+Comment: 
+
+Filename: acmecse/init/complexTypePolicies.ap
+Comment: 
+
+Filename: acmecse/init/configurations.docmd
+Comment: 
+
+Filename: acmecse/init/covid.fcp
+Comment: 
+
+Filename: acmecse/init/curve.as
+Comment: 
+
+Filename: acmecse/init/enumTypesPolicies.ep
+Comment: 
+
+Filename: acmecse/init/getConfigurationUT.as
+Comment: 
+
+Filename: acmecse/init/hed-dev.fcp
+Comment: 
+
+Filename: acmecse/init/hed-mc.fcp
+Comment: 
+
+Filename: acmecse/init/hed-sdev.fcp
+Comment: 
+
+Filename: acmecse/init/hod-dev.fcp
+Comment: 
+
+Filename: acmecse/init/hod-mc.fcp
+Comment: 
+
+Filename: acmecse/init/ind-dev.fcp
+Comment: 
+
+Filename: acmecse/init/ind-mc.fcp
+Comment: 
+
+Filename: acmecse/init/init.as
+Comment: 
+
+Filename: acmecse/init/iotOrchestrator.fcp
+Comment: 
+
+Filename: acmecse/init/mad-dev.fcp
+Comment: 
+
+Filename: acmecse/init/mad-mc.fcp
+Comment: 
+
+Filename: acmecse/init/mad-sdev.fcp
+Comment: 
+
+Filename: acmecse/init/mdd-mc.fcp
+Comment: 
+
+Filename: acmecse/init/melodyImperial.as
+Comment: 
+
+Filename: acmecse/init/melodyTheme.as
+Comment: 
+
+Filename: acmecse/init/psd-dev.fcp
+Comment: 
+
+Filename: acmecse/init/psd-mc.fcp
+Comment: 
+
+Filename: acmecse/init/query.as
+Comment: 
+
+Filename: acmecse/init/rad-dev.fcp
+Comment: 
+
+Filename: acmecse/init/rad-mc.fcp
+Comment: 
+
+Filename: acmecse/init/rebootWemos.as
+Comment: 
+
+Filename: acmecse/init/ved-dev.fcp
+Comment: 
+
+Filename: acmecse/init/ved-mc.fcp
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/hacksterIO.as
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/init.as
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/jupyterNotebooksLive.as
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/jupyterNotebooksWiki.as
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/oneM2MHomePage.as
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/oneM2MIntroduction.as
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/oneM2MSpecifications.as
+Comment: 
+
+Filename: acmecse/init/demoDocumentationTutorials/stackOverflow.as
+Comment: 
+
+Filename: acmecse/init/demoLightbulb/init.as
+Comment: 
+
+Filename: acmecse/init/demoLightbulb/lighbulb.as
+Comment: 
+
+Filename: acmecse/init/demoLightbulb/toggleLightswitch.as
+Comment: 
+
+Filename: acmecse/init/system.scripts/utReset.as
+Comment: 
+
+Filename: acmecse/init/system.scripts/utStatus.as
+Comment: 
+
+Filename: acmecse/init/testing.scripts/testCaseEnd.as
+Comment: 
+
+Filename: acmecse/init/testing.scripts/testCaseStart.as
+Comment: 
+
+Filename: acmecse/init/testing.scripts/testsDisableShortRequestExpiration.as
+Comment: 
+
+Filename: acmecse/init/testing.scripts/testsDisableShortResourceExpiration.as
+Comment: 
+
+Filename: acmecse/init/testing.scripts/testsEnableShortRequestExpiration.as
+Comment: 
+
+Filename: acmecse/init/testing.scripts/testsEnableShortResourceExpiration.as
+Comment: 
+
+Filename: acmecse/init/utilities.scripts/utilAttributeInfo.as
+Comment: 
+
+Filename: acmecse/protocols/CoAPServer.py
+Comment: 
+
+Filename: acmecse/protocols/HttpServer.py
+Comment: 
+
+Filename: acmecse/protocols/MQTTClient.py
+Comment: 
+
+Filename: acmecse/protocols/WebSocketServer.py
+Comment: 
+
+Filename: acmecse/protocols/__init__.py
+Comment: 
+
+Filename: acmecse/resources/ACP.py
+Comment: 
+
+Filename: acmecse/resources/ACPAnnc.py
+Comment: 
+
+Filename: acmecse/resources/ACTR.py
+Comment: 
+
+Filename: acmecse/resources/ACTRAnnc.py
+Comment: 
+
+Filename: acmecse/resources/AE.py
+Comment: 
+
+Filename: acmecse/resources/AEAnnc.py
+Comment: 
+
+Filename: acmecse/resources/ANDI.py
+Comment: 
+
+Filename: acmecse/resources/ANDIAnnc.py
+Comment: 
+
+Filename: acmecse/resources/ANI.py
+Comment: 
+
+Filename: acmecse/resources/ANIAnnc.py
+Comment: 
+
+Filename: acmecse/resources/AnnounceableResource.py
+Comment: 
+
+Filename: acmecse/resources/AnnouncedResource.py
+Comment: 
+
+Filename: acmecse/resources/BAT.py
+Comment: 
+
+Filename: acmecse/resources/BATAnnc.py
+Comment: 
+
+Filename: acmecse/resources/CIN.py
+Comment: 
+
+Filename: acmecse/resources/CINAnnc.py
+Comment: 
+
+Filename: acmecse/resources/CNT.py
+Comment: 
+
+Filename: acmecse/resources/CNTAnnc.py
+Comment: 
+
+Filename: acmecse/resources/CNT_LA.py
+Comment: 
+
+Filename: acmecse/resources/CNT_OL.py
+Comment: 
+
+Filename: acmecse/resources/CRS.py
+Comment: 
+
+Filename: acmecse/resources/CSEBase.py
+Comment: 
+
+Filename: acmecse/resources/CSEBaseAnnc.py
+Comment: 
+
+Filename: acmecse/resources/CSR.py
+Comment: 
+
+Filename: acmecse/resources/CSRAnnc.py
+Comment: 
+
+Filename: acmecse/resources/ContainerResource.py
+Comment: 
+
+Filename: acmecse/resources/DATC.py
+Comment: 
+
+Filename: acmecse/resources/DATCAnnc.py
+Comment: 
+
+Filename: acmecse/resources/DEPR.py
+Comment: 
+
+Filename: acmecse/resources/DEPRAnnc.py
+Comment: 
+
+Filename: acmecse/resources/DVC.py
+Comment: 
+
+Filename: acmecse/resources/DVCAnnc.py
+Comment: 
+
+Filename: acmecse/resources/DVI.py
+Comment: 
+
+Filename: acmecse/resources/DVIAnnc.py
+Comment: 
+
+Filename: acmecse/resources/EVL.py
+Comment: 
+
+Filename: acmecse/resources/EVLAnnc.py
+Comment: 
+
+Filename: acmecse/resources/FCI.py
+Comment: 
+
+Filename: acmecse/resources/FCNT.py
+Comment: 
+
+Filename: acmecse/resources/FCNTAnnc.py
+Comment: 
+
+Filename: acmecse/resources/FCNT_LA.py
+Comment: 
+
+Filename: acmecse/resources/FCNT_OL.py
+Comment: 
+
+Filename: acmecse/resources/FWR.py
+Comment: 
+
+Filename: acmecse/resources/FWRAnnc.py
+Comment: 
+
+Filename: acmecse/resources/Factory.py
+Comment: 
+
+Filename: acmecse/resources/GRP.py
+Comment: 
+
+Filename: acmecse/resources/GRPAnnc.py
+Comment: 
+
+Filename: acmecse/resources/GRP_FOPT.py
+Comment: 
+
+Filename: acmecse/resources/LCP.py
+Comment: 
+
+Filename: acmecse/resources/LCPAnnc.py
+Comment: 
+
+Filename: acmecse/resources/MEM.py
+Comment: 
+
+Filename: acmecse/resources/MEMAnnc.py
+Comment: 
+
+Filename: acmecse/resources/MNWK.py
+Comment: 
+
+Filename: acmecse/resources/MNWKAnnc.py
+Comment: 
+
+Filename: acmecse/resources/MgmtObj.py
+Comment: 
+
+Filename: acmecse/resources/MgmtObjAnnc.py
+Comment: 
+
+Filename: acmecse/resources/NOD.py
+Comment: 
+
+Filename: acmecse/resources/NODAnnc.py
+Comment: 
+
+Filename: acmecse/resources/NYCFC.py
+Comment: 
+
+Filename: acmecse/resources/NYCFCAnnc.py
+Comment: 
+
+Filename: acmecse/resources/PCH.py
+Comment: 
+
+Filename: acmecse/resources/PCH_PCU.py
+Comment: 
+
+Filename: acmecse/resources/PRMR.py
+Comment: 
+
+Filename: acmecse/resources/RBO.py
+Comment: 
+
+Filename: acmecse/resources/RBOAnnc.py
+Comment: 
+
+Filename: acmecse/resources/REQ.py
+Comment: 
+
+Filename: acmecse/resources/Resource.py
+Comment: 
+
+Filename: acmecse/resources/SCH.py
+Comment: 
+
+Filename: acmecse/resources/SCHAnnc.py
+Comment: 
+
+Filename: acmecse/resources/SIM.py
+Comment: 
+
+Filename: acmecse/resources/SIMAnnc.py
+Comment: 
+
+Filename: acmecse/resources/SMD.py
+Comment: 
+
+Filename: acmecse/resources/SMDAnnc.py
+Comment: 
+
+Filename: acmecse/resources/STTE.py
+Comment: 
+
+Filename: acmecse/resources/SUB.py
+Comment: 
+
+Filename: acmecse/resources/SWR.py
+Comment: 
+
+Filename: acmecse/resources/SWRAnnc.py
+Comment: 
+
+Filename: acmecse/resources/TS.py
+Comment: 
+
+Filename: acmecse/resources/TSAnnc.py
+Comment: 
+
+Filename: acmecse/resources/TSB.py
+Comment: 
+
+Filename: acmecse/resources/TSBAnnc.py
+Comment: 
+
+Filename: acmecse/resources/TSI.py
+Comment: 
+
+Filename: acmecse/resources/TSIAnnc.py
+Comment: 
+
+Filename: acmecse/resources/TS_LA.py
+Comment: 
+
+Filename: acmecse/resources/TS_OL.py
+Comment: 
+
+Filename: acmecse/resources/Unknown.py
+Comment: 
+
+Filename: acmecse/resources/VirtualResource.py
+Comment: 
+
+Filename: acmecse/resources/WIFIC.py
+Comment: 
+
+Filename: acmecse/resources/WIFICAnnc.py
+Comment: 
+
+Filename: acmecse/resources/__init__.py
+Comment: 
+
+Filename: acmecse/runtime/CSE.py
+Comment: 
+
+Filename: acmecse/runtime/Configuration.py
+Comment: 
+
+Filename: acmecse/runtime/Console.py
+Comment: 
+
+Filename: acmecse/runtime/Importer.py
+Comment: 
+
+Filename: acmecse/runtime/Logging.py
+Comment: 
+
+Filename: acmecse/runtime/Onboarding.py
+Comment: 
+
+Filename: acmecse/runtime/ScriptManager.py
+Comment: 
+
+Filename: acmecse/runtime/Statistics.py
+Comment: 
+
+Filename: acmecse/runtime/Storage.py
+Comment: 
+
+Filename: acmecse/runtime/TextUI.py
+Comment: 
+
+Filename: acmecse/runtime/__init__.py
+Comment: 
+
+Filename: acmecse/services/ActionManager.py
+Comment: 
+
+Filename: acmecse/services/AnnouncementManager.py
+Comment: 
+
+Filename: acmecse/services/Dispatcher.py
+Comment: 
+
+Filename: acmecse/services/EventManager.py
+Comment: 
+
+Filename: acmecse/services/GroupManager.py
+Comment: 
+
+Filename: acmecse/services/LocationManager.py
+Comment: 
+
+Filename: acmecse/services/NotificationManager.py
+Comment: 
+
+Filename: acmecse/services/RegistrationManager.py
+Comment: 
+
+Filename: acmecse/services/RemoteCSEManager.py
+Comment: 
+
+Filename: acmecse/services/RequestManager.py
+Comment: 
+
+Filename: acmecse/services/SecurityManager.py
+Comment: 
+
+Filename: acmecse/services/SemanticManager.py
+Comment: 
+
+Filename: acmecse/services/TimeManager.py
+Comment: 
+
+Filename: acmecse/services/TimeSeriesManager.py
+Comment: 
+
+Filename: acmecse/services/Validator.py
+Comment: 
+
+Filename: acmecse/services/__init__.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerAbout.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerConfigurations.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerDelete.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerDiagram.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerInfo.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerRegistrations.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerRequests.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerResourceServices.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerTools.py
+Comment: 
+
+Filename: acmecse/textui/ACMEContainerTree.py
+Comment: 
+
+Filename: acmecse/textui/ACMEFieldOriginator.py
+Comment: 
+
+Filename: acmecse/textui/ACMEHeader.py
+Comment: 
+
+Filename: acmecse/textui/ACMETUI.css
+Comment: 
+
+Filename: acmecse/textui/ACMETuiApp.py
+Comment: 
+
+Filename: acmecse/textui/__init__.py
+Comment: 
+
+Filename: acmecse/webui/__init__.py
+Comment: 
+
+Filename: acmecse/webui/webUI.py
+Comment: 
+
+Filename: acmecse/webui/web/index-sl.html
+Comment: 
+
+Filename: acmecse/webui/web/index.html
+Comment: 
+
+Filename: acmecse/webui/web/css/contextmenu.css
+Comment: 
+
+Filename: acmecse/webui/web/css/picnic.css
+Comment: 
+
+Filename: acmecse/webui/web/css/style.css
+Comment: 
+
+Filename: acmecse/webui/web/css/treejs.css
+Comment: 
+
+Filename: acmecse/webui/web/img/acme.png
+Comment: 
+
+Filename: acmecse/webui/web/img/acme.t2d
+Comment: 
+
+Filename: acmecse/webui/web/img/acme_sm.png
+Comment: 
+
+Filename: acmecse/webui/web/img/acme_sq.png
+Comment: 
+
+Filename: acmecse/webui/web/img/acme_sq_white.png
+Comment: 
+
+Filename: acmecse/webui/web/img/badge-acme.png
+Comment: 
+
+Filename: acmecse/webui/web/img/favicon.png
+Comment: 
+
+Filename: acmecse/webui/web/img/badge-acme.pxd/metadata.info
+Comment: 
+
+Filename: acmecse/webui/web/img/badge-acme.pxd/QuickLook/Icon.tiff
+Comment: 
+
+Filename: acmecse/webui/web/img/badge-acme.pxd/QuickLook/Thumbnail.tiff
+Comment: 
+
+Filename: acmecse/webui/web/img/favicon.pxd/metadata.info
+Comment: 
+
+Filename: acmecse/webui/web/img/favicon.pxd/QuickLook/Icon.tiff
+Comment: 
+
+Filename: acmecse/webui/web/img/favicon.pxd/QuickLook/Thumbnail.tiff
+Comment: 
+
+Filename: acmecse/webui/web/js/attributes.js
+Comment: 
+
+Filename: acmecse/webui/web/js/contextmenu.js
+Comment: 
+
+Filename: acmecse/webui/web/js/main.js
+Comment: 
+
+Filename: acmecse/webui/web/js/menu.js
+Comment: 
+
+Filename: acmecse/webui/web/js/resourceTree.js
+Comment: 
+
+Filename: acmecse/webui/web/js/rest.js
+Comment: 
+
+Filename: acmecse/webui/web/js/restui.js
+Comment: 
+
+Filename: acmecse/webui/web/js/tree.js
+Comment: 
+
+Filename: acmecse_test-2024.5.dist-info/LICENSE
+Comment: 
+
+Filename: acmecse_test-2024.5.dist-info/METADATA
+Comment: 
+
+Filename: acmecse_test-2024.5.dist-info/WHEEL
+Comment: 
+
+Filename: acmecse_test-2024.5.dist-info/entry_points.txt
+Comment: 
+
+Filename: acmecse_test-2024.5.dist-info/top_level.txt
+Comment: 
+
+Filename: acmecse_test-2024.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `acme/__main__.py` & `acmecse/__main__.py`

 * *Files identical despite different names*

## Comparing `acmecse_test-2024.4.9.dist-info/LICENSE` & `acmecse_test-2024.5.dist-info/LICENSE`

 * *Files identical despite different names*

