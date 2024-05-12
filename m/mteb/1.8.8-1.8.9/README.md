# Comparing `tmp/mteb-1.8.8.tar.gz` & `tmp/mteb-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.8.8.tar", last modified: Sat May 11 09:52:28 2024, max compression
+gzip compressed data, was "mteb-1.8.9.tar", last modified: Sat May 11 13:08:04 2024, max compression
```

## Comparing `mteb-1.8.8.tar` & `mteb-1.8.9.tar`

### file list

```diff
@@ -1,1244 +1,1256 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.042079 mteb-1.8.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-11 09:52:23.000000 mteb-1.8.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    24072 2024-05-11 09:52:28.042079 mteb-1.8.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9642 2024-05-11 09:52:23.000000 mteb-1.8.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.818077 mteb-1.8.8/docs/
--rw-r--r--   0 root         (0) root         (0)     2651 2024-05-11 09:52:23.000000 mteb-1.8.8/docs/create_tasks_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.818077 mteb-1.8.8/docs/mmteb/
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-11 09:52:23.000000 mteb-1.8.8/docs/mmteb/create_points_table.py
--rw-r--r--   0 root         (0) root         (0)     2108 2024-05-11 09:52:23.000000 mteb-1.8.8/docs/mmteb/validate_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.818077 mteb-1.8.8/mteb/
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.822077 mteb-1.8.8/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     6404 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5876 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2410 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     7433 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskClusteringFast.py
--rw-r--r--   0 root         (0) root         (0)    24968 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskInstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    13422 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      562 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1897 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/MultiSubsetLoader.py
--rw-r--r--   0 root         (0) root         (0)      653 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)    10404 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7082 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/iso_15924_to_script.json
--rw-r--r--   0 root         (0) root         (0)   193114 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/iso_639_3_to_language.json
--rw-r--r--   0 root         (0) root         (0)      541 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/languages.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/benchmarks.py
--rw-r--r--   0 root         (0) root         (0)     5225 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/cmd.py
--rw-r--r--   0 root         (0) root         (0)     1702 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/encoder_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.822077 mteb-1.8.8/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13258 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5840 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8927 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     7126 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9554 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    19805 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7965 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      820 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/logging.py
--rw-r--r--   0 root         (0) root         (0)     6530 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/overview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      750 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/BitextMining/dan/
--rw-r--r--   0 root         (0) root         (0)     2246 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/BitextMining/kat/
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/kat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)    29308 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5951 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     3552 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
--rw-r--r--   0 root         (0) root         (0)    13482 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1423 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5733 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/BitextMining/srn/
--rw-r--r--   0 root         (0) root         (0)     2610 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/srn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/BitextMining/vie/
--rw-r--r--   0 root         (0) root         (0)     2889 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/CLSD/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/
--rw-r--r--   0 root         (0) root         (0)     4878 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py
--rw-r--r--   0 root         (0) root         (0)     4878 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/__init__.py
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     5167 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ara/
--rw-r--r--   0 root         (0) root         (0)     1598 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/AJGT.py
--rw-r--r--   0 root         (0) root         (0)     1719 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1907 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/TweetEmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)     3161 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ben/
--rw-r--r--   0 root         (0) root         (0)     2122 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/BengaliDocumentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/bul/
--rw-r--r--   0 root         (0) root         (0)     1947 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/bul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ces/
--rw-r--r--   0 root         (0) root         (0)     1704 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/dan/
--rw-r--r--   0 root         (0) root         (0)     1750 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     4348 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     2435 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/deu/
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ell/
--rw-r--r--   0 root         (0) root         (0)     2172 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ell/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.838077 mteb-1.8.8/mteb/tasks/Classification/eng/
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ArxivClassification.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     2072 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/DBpediaClassification.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/FrenkEnClassification.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)   241062 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/LegalBenchClassification.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/NewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     3186 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/PatentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2842 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ToxicChatClassification.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)     2290 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/YelpReviewFullClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.838077 mteb-1.8.8/mteb/tasks/Classification/est/
--rw-r--r--   0 root         (0) root         (0)     2407 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/est/estonian_valence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.838077 mteb-1.8.8/mteb/tasks/Classification/fas/
--rw-r--r--   0 root         (0) root         (0)     1714 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/fil/
--rw-r--r--   0 root         (0) root         (0)     1925 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)     2040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/fin/
--rw-r--r--   0 root         (0) root         (0)     2562 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fin/FinToxicityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/fra/
--rw-r--r--   0 root         (0) root         (0)     1468 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fra/FrenchBookReviews.py
--rw-r--r--   0 root         (0) root         (0)     1777 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/guj/
--rw-r--r--   0 root         (0) root         (0)     1285 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/guj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/hin/
--rw-r--r--   0 root         (0) root         (0)     2242 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
--rw-r--r--   0 root         (0) root         (0)     1755 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/hrv/
--rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hrv/FrenkHrClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hrv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/ind/
--rw-r--r--   0 root         (0) root         (0)     2928 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
--rw-r--r--   0 root         (0) root         (0)     3829 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ind/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/ita/
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ita/ItaCaseholdClassification.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ita/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/jav/
--rw-r--r--   0 root         (0) root         (0)     1871 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/jav/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/jpn/
--rw-r--r--   0 root         (0) root         (0)     3402 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/jpn/WRIMEClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kan/
--rw-r--r--   0 root         (0) root         (0)     1676 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kan/KannadaNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kat/
--rw-r--r--   0 root         (0) root         (0)     3016 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kor/
--rw-r--r--   0 root         (0) root         (0)     2428 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kor/KlueTC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kur/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/mal/
--rw-r--r--   0 root         (0) root         (0)     1293 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mal/MalayalamNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/mkd/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mkd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.850077 mteb-1.8.8/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2313 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     3360 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py
--rw-r--r--   0 root         (0) root         (0)     2638 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/HinDialectClassification.py
--rw-r--r--   0 root         (0) root         (0)     5163 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     3286 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/LanguageClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     6431 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MultiHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     3839 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1586 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     8376 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/SIB200Classification.py
--rw-r--r--   0 root         (0) root         (0)     2956 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py
--rw-r--r--   0 root         (0) root         (0)     3264 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/nep/
--rw-r--r--   0 root         (0) root         (0)     2770 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nep/NepaliNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nep/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/nld/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nld/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/nob/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nob/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1173 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/ory/
--rw-r--r--   0 root         (0) root         (0)     1306 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ory/OdiaNewsClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/pan/
--rw-r--r--   0 root         (0) root         (0)     1336 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/pan/PunjabiNewsClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/pol/
--rw-r--r--   0 root         (0) root         (0)     4922 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/pol/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/por/
--rw-r--r--   0 root         (0) root         (0)     2307 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/por/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/ron/
--rw-r--r--   0 root         (0) root         (0)     1579 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ron/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/san/
--rw-r--r--   0 root         (0) root         (0)     2851 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/san/SanskritShlokasClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/san/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/sin/
--rw-r--r--   0 root         (0) root         (0)     2271 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/sin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/slv/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/slv/FrenkSlClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/slv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/spa/
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/spa/SpanishNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2218 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/spa/SpanishSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/ssw/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ssw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/swe/
--rw-r--r--   0 root         (0) root         (0)     2834 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/swe/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/swe/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/swe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tam/
--rw-r--r--   0 root         (0) root         (0)     1408 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tam/TamilNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tel/
--rw-r--r--   0 root         (0) root         (0)     1382 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tha/
--rw-r--r--   0 root         (0) root         (0)     2106 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tha/WisesightSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tsn/
--rw-r--r--   0 root         (0) root         (0)     1760 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tsn/TswanaNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tsn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tur/
--rw-r--r--   0 root         (0) root         (0)     1640 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1493 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/ukr/
--rw-r--r--   0 root         (0) root         (0)     2485 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ukr/UkrFormalityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ukr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/urd/
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/urd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/vie/
--rw-r--r--   0 root         (0) root         (0)     1872 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/zho/
--rw-r--r--   0 root         (0) root         (0)     6571 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zho/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)     1883 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/zul/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1644 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Clustering/deu/
--rw-r--r--   0 root         (0) root         (0)     1179 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1984 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1477 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.866078 mteb-1.8.8/mteb/tasks/Clustering/eng/
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.866078 mteb-1.8.8/mteb/tasks/Clustering/fra/
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1607 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3055 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     3202 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     2687 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3442 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/nob/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/nob/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/pol/
--rw-r--r--   0 root         (0) root         (0)     3352 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/pol/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/rom/
--rw-r--r--   0 root         (0) root         (0)     1089 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/spa/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/swe/
--rw-r--r--   0 root         (0) root         (0)     4765 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/swe/SwednClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4094 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/swe/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/zho/
--rw-r--r--   0 root         (0) root         (0)     3639 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/zho/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/InstructionRetrieval/
--rw-r--r--   0 root         (0) root         (0)      176 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1547 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1547 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1556 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/deu/
--rw-r--r--   0 root         (0) root         (0)     2862 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/eng/
--rw-r--r--   0 root         (0) root         (0)     4650 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/LegalBenchPC.py
--rw-r--r--   0 root         (0) root         (0)     1152 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/hye/
--rw-r--r--   0 root         (0) root         (0)     1439 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/hye/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2780 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)     6426 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/XNLI.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/pol/
--rw-r--r--   0 root         (0) root         (0)     3577 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/pol/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/zho/
--rw-r--r--   0 root         (0) root         (0)     1849 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3054 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/fra/
--rw-r--r--   0 root         (0) root         (0)     1195 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/fra/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/fra/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1269 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/zho/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/zho/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     3751 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Retrieval/ara/
--rw-r--r--   0 root         (0) root         (0)     2367 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ara/SadeemQuestionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ara/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Retrieval/code/
--rw-r--r--   0 root         (0) root         (0)     3275 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3377 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.882078 mteb-1.8.8/mteb/tasks/Retrieval/dan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2574 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.882078 mteb-1.8.8/mteb/tasks/Retrieval/deu/
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2891 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.882078 mteb-1.8.8/mteb/tasks/Retrieval/ell/
--rw-r--r--   0 root         (0) root         (0)     2683 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ell/GreekCivicsQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ell/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.890078 mteb-1.8.8/mteb/tasks/Retrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1175 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1151 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3648 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3641 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.890078 mteb-1.8.8/mteb/tasks/Retrieval/est/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/est/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/est/estqa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/fra/
--rw-r--r--   0 root         (0) root         (0)     2144 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3184 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2148 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/hun/
--rw-r--r--   0 root         (0) root         (0)     2589 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/hun/HunSum2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/jpn/
--rw-r--r--   0 root         (0) root         (0)     2853 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/kat/
--rw-r--r--   0 root         (0) root         (0)     2568 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/kor/
--rw-r--r--   0 root         (0) root         (0)      906 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kor/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3776 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3277 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     6239 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3731 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3771 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3145 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     4217 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3943 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/nob/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2699 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/nob/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/pol/
--rw-r--r--   0 root         (0) root         (0)      967 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/slk/
--rw-r--r--   0 root         (0) root         (0)     2891 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/slk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/spa/
--rw-r--r--   0 root         (0) root         (0)     2125 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2610 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/tur/
--rw-r--r--   0 root         (0) root         (0)     3883 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/tur/TurHistQuad.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/tur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/vie/
--rw-r--r--   0 root         (0) root         (0)     3798 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/zho/
--rw-r--r--   0 root         (0) root         (0)    10384 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      787 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/STS/deu/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/eng/
--rw-r--r--   0 root         (0) root         (0)     1184 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1184 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1208 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/fao/
--rw-r--r--   0 root         (0) root         (0)     2015 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fao/FaroeseSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/fin/
--rw-r--r--   0 root         (0) root         (0)     3422 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fin/FinParaSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/fra/
--rw-r--r--   0 root         (0) root         (0)     1472 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fra/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/jpn/
--rw-r--r--   0 root         (0) root         (0)     3034 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/jpn/JSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/kor/
--rw-r--r--   0 root         (0) root         (0)     2504 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/kor/KlueSTS.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/kor/KorSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     4131 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1600 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2712 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/pol/
--rw-r--r--   0 root         (0) root         (0)     2268 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/pol/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/ron/
--rw-r--r--   0 root         (0) root         (0)     1896 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/ron/RonSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/STS/spa/
--rw-r--r--   0 root         (0) root         (0)     1486 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/spa/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/STS/zho/
--rw-r--r--   0 root         (0) root         (0)     7122 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/zho/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/Summarization/eng/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/Summarization/fra/
--rw-r--r--   0 root         (0) root         (0)     1304 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/fra/__init__.py
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.042079 mteb-1.8.8/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    24072 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    73769 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      258 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2752 2024-05-11 09:52:24.000000 mteb-1.8.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.814077 mteb-1.8.8/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/results/GritLM__GritLM-7B/
--rw-r--r--   0 root         (0) root         (0)     2342 2024-05-11 09:52:23.000000 mteb-1.8.8/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/
--rw-r--r--   0 root         (0) root         (0)     1154 2024-05-11 09:52:23.000000 mteb-1.8.8/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.810077 mteb-1.8.8/results/dangvantuan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.914078 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      634 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      675 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
--rw-r--r--   0 root         (0) root         (0)      676 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
--rw-r--r--   0 root         (0) root         (0)      332 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      335 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
--rw-r--r--   0 root         (0) root         (0)     1242 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2992 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)     2801 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      820 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SICKFr.json
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/STS22.json
--rw-r--r--   0 root         (0) root         (0)      921 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
--rw-r--r--   0 root         (0) root         (0)     1099 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1245 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.810077 mteb-1.8.8/results/intfloat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.918078 mteb-1.8.8/results/intfloat/multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/HinDialectClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/MalayalamNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/OdiaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1294 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/SadeemQuestionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/SouthAfricanLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      367 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/TamilNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/TeluguAndhraJyotiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/TswanaNewsClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.918078 mteb-1.8.8/results/intfloat__e5-small/
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small/TurkishProductSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.918078 mteb-1.8.8/results/intfloat__e5-small-v2/
--rw-r--r--   0 root         (0) root         (0)     2512 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2540 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2550 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.922078 mteb-1.8.8/results/intfloat__multilingual-e5-base/
--rw-r--r--   0 root         (0) root         (0)      758 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     2281 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json
--rw-r--r--   0 root         (0) root         (0)     2293 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json
--rw-r--r--   0 root         (0) root         (0)      733 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      757 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.970079 mteb-1.8.8/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/AJGT.json
--rw-r--r--   0 root         (0) root         (0)      375 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/AfriSentiLangClassification.json
--rw-r--r--   0 root         (0) root         (0)     1422 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ArxivClassification.json
--rw-r--r--   0 root         (0) root         (0)      517 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json
--rw-r--r--   0 root         (0) root         (0)     1161 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BSARDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BengaliDocumentClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BengaliSentimentAnalysis.json
--rw-r--r--   0 root         (0) root         (0)   336719 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1081 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicensorLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAntiAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAuditRightsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADCapOnLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADChangeOfControlLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADCovenantNotToSueLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADEffectiveDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADExclusivityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADExpirationDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADGoverningLawLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADIPOwnershipAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      468 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADInsuranceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADJointIPOwnershipLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADLicenseGrantLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADLiquidatedDamagesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADMinimumCommitmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      396 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADMostFavoredNationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNoSolicitOfCustomersLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNoSolicitOfEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNonCompeteLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      424 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNonDisparagementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      425 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNonTransferableLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADPostTerminationServicesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADPriceRestrictionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADRenewalTermLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      461 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADRevenueProfitSharingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADRofrRofoRofnLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADSourceCodeEscrowLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADTerminationForConvenienceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADThirdPartyBeneficiaryLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADUncappedLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADVolumeRestrictionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADWarrantyDurationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CanadaTaxCourtOutcomesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      616 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json
--rw-r--r--   0 root         (0) root         (0)    13681 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     5524 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      492 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIExplicitIdentificationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      483 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLILimitedUseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLINoLicensingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      492 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      422 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissibleCopyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      461 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLISharingWithEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLISurvivalOfObligationsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CorporateLobbyingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     2305 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json
--rw-r--r--   0 root         (0) root         (0)     2309 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json
--rw-r--r--   0 root         (0) root         (0)      738 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DBpediaClassification.json
--rw-r--r--   0 root         (0) root         (0)     1016 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DefinitionClassificationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity1LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity2LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      408 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity3LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity4LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity5LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity6LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      463 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2105 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FaroeseSTS.json
--rw-r--r--   0 root         (0) root         (0)      733 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      827 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FinParaSTS.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FinToxicityClassification.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FinancialPhrasebankClassification.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenchBookReviews.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenkEnClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenkHrClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenkSlClassification.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FunctionOfDecisionSectionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     1168 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GeorgianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GermanDPR.json
--rw-r--r--   0 root         (0) root         (0)      401 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GermanPoliticiansTwitterSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekCivicsQA.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HateSpeechPortugueseClassification.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1289 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      604 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     4319 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)    11798 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     4273 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     3924 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      644 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/InsurancePolicyInterpretationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/InternationalCitizenshipQuestionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ItaCaseholdClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JCrewBlockerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JavaneseIMDBClassification.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KLUE-TC.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KannadaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1163 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7814 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7703 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1169 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LanguageClassification.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsBenefitsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsBusinessLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsConsumerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsCourtsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsCrimeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsDivorceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsDomesticViolenceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsEducationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsEmploymentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsEstatesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsFamilyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsHealthLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsHousingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsImmigrationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsTortsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsTrafficLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LegalBenchPC.json
--rw-r--r--   0 root         (0) root         (0)      420 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LegalReasoningCausalityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     2360 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MLQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     3894 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      749 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3151 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MultiHateClassification.json
--rw-r--r--   0 root         (0) root         (0)     8513 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)   417235 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NTREXBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NepaliNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     3386 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3392 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NordicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PatentClassification.json
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      514 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      513 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PunjabiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      403 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)    42700 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SIB200Classification.json
--rw-r--r--   0 root         (0) root         (0)      298 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      584 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      592 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SentimentAnalysisHindi.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SinhalaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SinhalaNewsSourceClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SlovakSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      375 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SpanishNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SpanishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1015 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      304 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)      893 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      524 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json
--rw-r--r--   0 root         (0) root         (0)     1116 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      629 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      597 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      522 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ToxicConversationsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1166 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TurkishProductSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1827 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetTopicSingleClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      734 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/UrduRomanSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1028 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      368 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)     2184 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/WisesightSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)    38759 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLI.json
--rw-r--r--   0 root         (0) root         (0)    18115 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLIV2.json
--rw-r--r--   0 root         (0) root         (0)    12839 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/XQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/YahooAnswersTopicsClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/YelpReviewFullClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.814077 mteb-1.8.8/results/sentence-transformers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.974079 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/HinDialectClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MalayalamNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/OdiaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1295 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SadeemQuestionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SouthAfricanLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TamilNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)    21290 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json
--rw-r--r--   0 root         (0) root         (0)    21291 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TeluguAndhraJyotiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TswanaNewsClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.978079 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)   387673 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1014 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      302 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/model.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.030079 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AJGT.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AfriSentiLangClassification.json
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClassification.json
--rw-r--r--   0 root         (0) root         (0)      520 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json
--rw-r--r--   0 root         (0) root         (0)     1160 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliDocumentClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      444 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliSentimentAnalysis.json
--rw-r--r--   0 root         (0) root         (0)   338028 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1088 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      344 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      398 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)      462 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicensorLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAntiAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAuditRightsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCapOnLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADChangeOfControlLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCovenantNotToSueLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADEffectiveDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExclusivityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExpirationDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADGoverningLawLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIPOwnershipAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADInsuranceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADJointIPOwnershipLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      415 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLicenseGrantLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLiquidatedDamagesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMinimumCommitmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMostFavoredNationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfCustomersLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonCompeteLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      390 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonDisparagementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonTransferableLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      444 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPostTerminationServicesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPriceRestrictionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRenewalTermLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRevenueProfitSharingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRofrRofoRofnLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADSourceCodeEscrowLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADTerminationForConvenienceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADThirdPartyBeneficiaryLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUncappedLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADVolumeRestrictionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      398 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADWarrantyDurationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CanadaTaxCourtOutcomesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      641 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json
--rw-r--r--   0 root         (0) root         (0)    13663 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     5535 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIExplicitIdentificationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLILimitedUseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoLicensingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleCopyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISurvivalOfObligationsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CorporateLobbyingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     2340 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json
--rw-r--r--   0 root         (0) root         (0)     2295 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DBpediaClassification.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DefinitionClassificationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity1LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity2LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity3LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity4LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity5LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity6LegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2108 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FaroeseSTS.json
--rw-r--r--   0 root         (0) root         (0)      746 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      835 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinToxicityClassification.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinancialPhrasebankClassification.json
--rw-r--r--   0 root         (0) root         (0)      291 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenchBookReviews.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkEnClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkHrClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkSlClassification.json
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FunctionOfDecisionSectionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GermanPoliticiansTwitterSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1157 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HateSpeechPortugueseClassification.json
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1317 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     4370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)    11833 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     4276 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     3921 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      641 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InsurancePolicyInterpretationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InternationalCitizenshipQuestionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      342 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaCaseholdClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JCrewBlockerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JavaneseIMDBClassification.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-TC.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KannadaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1167 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7839 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7915 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1152 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LanguageClassification.json
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBenefitsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBusinessLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsConsumerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCourtsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCrimeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDivorceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      425 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDomesticViolenceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEducationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEmploymentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEstatesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsFamilyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHealthLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHousingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsImmigrationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTortsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTrafficLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     1443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalReasoningCausalityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)   104611 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     3877 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     3884 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      748 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3151 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json
--rw-r--r--   0 root         (0) root         (0)     1332 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json
--rw-r--r--   0 root         (0) root         (0)     8537 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)   421556 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NepaliNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     3382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NordicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)    16669 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PatentClassification.json
--rw-r--r--   0 root         (0) root         (0)    18247 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      741 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      517 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PunjabiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)    42635 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1011 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SentimentAnalysisHindi.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsSourceClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)      898 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      523 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1022 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      637 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      523 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicChatClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicConversationsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1822 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetTopicSingleClassification.json
--rw-r--r--   0 root         (0) root         (0)     1035 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UrduRomanSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
--rw-r--r--   0 root         (0) root         (0)     2186 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WisesightSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)    38547 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json
--rw-r--r--   0 root         (0) root         (0)    17971 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLIV2.json
--rw-r--r--   0 root         (0) root         (0)    12890 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YahooAnswersTopicsClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YelpReviewFullClassification.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)      176 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5924 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2133 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/medicalqaretrieval/
--rw-r--r--   0 root         (0) root         (0)     1884 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/medicalqaretrieval/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/multilingual_sentiment_classification/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/multilingual_sentiment_classification/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/scala_classification/
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/scala_classification/create_multiling_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2435 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/toxic_conversations_50k/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/xnli2/
--rw-r--r--   0 root         (0) root         (0)      688 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/xnli2/create_multilang_ds.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5216 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/mteb_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.814077 mteb-1.8.8/scripts/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      673 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1017 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_law.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 09:52:28.042079 mteb-1.8.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.042079 mteb-1.8.8/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1418 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     2602 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_all_abstasks.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_encoder_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_mteb.py
--rw-r--r--   0 root         (0) root         (0)     7159 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_mteb_rerank.py
--rw-r--r--   0 root         (0) root         (0)     3013 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_overview.py
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_retrieval_abstask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.528482 mteb-1.8.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-11 13:08:00.000000 mteb-1.8.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    24072 2024-05-11 13:08:04.528482 mteb-1.8.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9642 2024-05-11 13:08:00.000000 mteb-1.8.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.308481 mteb-1.8.9/docs/
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-11 13:08:00.000000 mteb-1.8.9/docs/create_tasks_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.308481 mteb-1.8.9/docs/mmteb/
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-11 13:08:00.000000 mteb-1.8.9/docs/mmteb/create_points_table.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-05-11 13:08:00.000000 mteb-1.8.9/docs/mmteb/validate_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.308481 mteb-1.8.9/mteb/
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.316481 mteb-1.8.9/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     6404 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5876 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     7433 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskClusteringFast.py
+-rw-r--r--   0 root         (0) root         (0)    24968 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskInstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     6769 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskMultilabelClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    13422 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/MultiSubsetLoader.py
+-rw-r--r--   0 root         (0) root         (0)      653 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)    10411 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      512 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/iso_15924_to_script.json
+-rw-r--r--   0 root         (0) root         (0)   193114 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/iso_639_3_to_language.json
+-rw-r--r--   0 root         (0) root         (0)      541 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/abstasks/languages.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/cmd.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/encoder_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.316481 mteb-1.8.9/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13258 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.316481 mteb-1.8.9/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11003 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    19805 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      820 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/logging.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/overview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.316481 mteb-1.8.9/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.316481 mteb-1.8.9/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.320481 mteb-1.8.9/mteb/tasks/BitextMining/dan/
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.320481 mteb-1.8.9/mteb/tasks/BitextMining/kat/
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.320481 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)    29308 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)    13482 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.320481 mteb-1.8.9/mteb/tasks/BitextMining/srn/
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/srn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.320481 mteb-1.8.9/mteb/tasks/BitextMining/vie/
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/BitextMining/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.324481 mteb-1.8.9/mteb/tasks/CLSD/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.324481 mteb-1.8.9/mteb/tasks/CLSD/WMT1921/
+-rw-r--r--   0 root         (0) root         (0)     4878 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py
+-rw-r--r--   0 root         (0) root         (0)     4878 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/CLSD/WMT1921/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/CLSD/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.324481 mteb-1.8.9/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     5212 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.324481 mteb-1.8.9/mteb/tasks/Classification/ara/
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ara/AJGT.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ara/TweetEmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ara/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.324481 mteb-1.8.9/mteb/tasks/Classification/ben/
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ben/BengaliDocumentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ben/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.324481 mteb-1.8.9/mteb/tasks/Classification/bul/
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/bul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.324481 mteb-1.8.9/mteb/tasks/Classification/ces/
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.328481 mteb-1.8.9/mteb/tasks/Classification/dan/
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/dan/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/dan/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.328481 mteb-1.8.9/mteb/tasks/Classification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.328481 mteb-1.8.9/mteb/tasks/Classification/ell/
+-rw-r--r--   0 root         (0) root         (0)     2172 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.332481 mteb-1.8.9/mteb/tasks/Classification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/ArxivClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/DBpediaClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/FrenkEnClassification.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)   241062 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/LegalBenchClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/PatentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/ToxicChatClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/YelpReviewFullClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.332481 mteb-1.8.9/mteb/tasks/Classification/est/
+-rw-r--r--   0 root         (0) root         (0)     2407 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/est/estonian_valence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.332481 mteb-1.8.9/mteb/tasks/Classification/fas/
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.332481 mteb-1.8.9/mteb/tasks/Classification/fil/
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.332481 mteb-1.8.9/mteb/tasks/Classification/fin/
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fin/FinToxicityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/fra/
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fra/FrenchBookReviews.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/guj/
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/guj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/hin/
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/hin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/hrv/
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/hrv/FrenkHrClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/hrv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/ind/
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3829 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ind/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/ita/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ita/ItaCaseholdClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ita/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/jav/
+-rw-r--r--   0 root         (0) root         (0)     1871 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/jav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3402 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/jpn/WRIMEClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/kan/
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/kan/KannadaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/kan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.336481 mteb-1.8.9/mteb/tasks/Classification/kat/
+-rw-r--r--   0 root         (0) root         (0)     3016 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.340481 mteb-1.8.9/mteb/tasks/Classification/kor/
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/kor/KlueTC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.340481 mteb-1.8.9/mteb/tasks/Classification/kur/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/kur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.340481 mteb-1.8.9/mteb/tasks/Classification/mal/
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/mal/MalayalamNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/mal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.340481 mteb-1.8.9/mteb/tasks/Classification/mar/
+-rw-r--r--   0 root         (0) root         (0)     1328 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/mar/MarathiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/mar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.340481 mteb-1.8.9/mteb/tasks/Classification/mkd/
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/mkd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.344481 mteb-1.8.9/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/HinDialectClassification.py
+-rw-r--r--   0 root         (0) root         (0)     5163 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/IndicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/LanguageClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/MultiHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3839 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     8376 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/SIB200Classification.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.344481 mteb-1.8.9/mteb/tasks/Classification/nep/
+-rw-r--r--   0 root         (0) root         (0)     2770 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/nep/NepaliNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/nep/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.344481 mteb-1.8.9/mteb/tasks/Classification/nld/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/nld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.344481 mteb-1.8.9/mteb/tasks/Classification/nob/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/nob/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/nob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.344481 mteb-1.8.9/mteb/tasks/Classification/ory/
+-rw-r--r--   0 root         (0) root         (0)     1306 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ory/OdiaNewsClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.344481 mteb-1.8.9/mteb/tasks/Classification/pan/
+-rw-r--r--   0 root         (0) root         (0)     1336 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/pan/PunjabiNewsClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.344481 mteb-1.8.9/mteb/tasks/Classification/pol/
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/pol/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/por/
+-rw-r--r--   0 root         (0) root         (0)     2307 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/por/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/ron/
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ron/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/san/
+-rw-r--r--   0 root         (0) root         (0)     2851 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/san/SanskritShlokasClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/san/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/sin/
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/sin/SinhalaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/sin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/slv/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/slv/FrenkSlClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/slv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/spa/
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/spa/SpanishNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/spa/SpanishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/ssw/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ssw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/swe/
+-rw-r--r--   0 root         (0) root         (0)     2834 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/swe/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/swe/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/swe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.348481 mteb-1.8.9/mteb/tasks/Classification/tam/
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tam/TamilNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/tel/
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/tha/
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tha/WisesightSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/tsn/
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tsn/TswanaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tsn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/tur/
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/ukr/
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ukr/UkrFormalityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/ukr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/urd/
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/urd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/vie/
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/zho/
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/zho/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Classification/zul/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Classification/zul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.352481 mteb-1.8.9/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.356481 mteb-1.8.9/mteb/tasks/Clustering/deu/
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.360481 mteb-1.8.9/mteb/tasks/Clustering/eng/
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.360481 mteb-1.8.9/mteb/tasks/Clustering/fra/
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.360481 mteb-1.8.9/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.360481 mteb-1.8.9/mteb/tasks/Clustering/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/nob/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/nob/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.360481 mteb-1.8.9/mteb/tasks/Clustering/pol/
+-rw-r--r--   0 root         (0) root         (0)     3352 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/pol/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.360481 mteb-1.8.9/mteb/tasks/Clustering/rom/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.360481 mteb-1.8.9/mteb/tasks/Clustering/spa/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/Clustering/swe/
+-rw-r--r--   0 root         (0) root         (0)     4765 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/swe/SwednClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/swe/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/Clustering/zho/
+-rw-r--r--   0 root         (0) root         (0)     3639 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/zho/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Clustering/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/InstructionRetrieval/
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/InstructionRetrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/MultiLabelClassification/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/MultiLabelClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/MultiLabelClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2593 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/MultiLabelClassification/multilingual/MultiEURLEXMultilabelClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/PairClassification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/PairClassification/eng/
+-rw-r--r--   0 root         (0) root         (0)     4650 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/eng/LegalBenchPC.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.364481 mteb-1.8.9/mteb/tasks/PairClassification/hye/
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/hye/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2780 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/multilingual/XNLI.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/PairClassification/pol/
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/pol/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/PairClassification/zho/
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/PairClassification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/Reranking/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/eng/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/eng/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/Reranking/fra/
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/fra/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/fra/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/Reranking/zho/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/zho/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Reranking/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.368481 mteb-1.8.9/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     3751 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.372481 mteb-1.8.9/mteb/tasks/Retrieval/ara/
+-rw-r--r--   0 root         (0) root         (0)     2367 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/ara/SadeemQuestionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/ara/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.372481 mteb-1.8.9/mteb/tasks/Retrieval/code/
+-rw-r--r--   0 root         (0) root         (0)     3275 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.372481 mteb-1.8.9/mteb/tasks/Retrieval/dan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/dan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/dan/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/dan/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.372481 mteb-1.8.9/mteb/tasks/Retrieval/deu/
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.372481 mteb-1.8.9/mteb/tasks/Retrieval/ell/
+-rw-r--r--   0 root         (0) root         (0)     2683 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/ell/GreekCivicsQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.380481 mteb-1.8.9/mteb/tasks/Retrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.380481 mteb-1.8.9/mteb/tasks/Retrieval/est/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/est/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/est/estqa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.384482 mteb-1.8.9/mteb/tasks/Retrieval/fra/
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.384482 mteb-1.8.9/mteb/tasks/Retrieval/hun/
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/hun/HunSum2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.384482 mteb-1.8.9/mteb/tasks/Retrieval/jpn/
+-rw-r--r--   0 root         (0) root         (0)     2853 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.384482 mteb-1.8.9/mteb/tasks/Retrieval/kat/
+-rw-r--r--   0 root         (0) root         (0)     2568 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.384482 mteb-1.8.9/mteb/tasks/Retrieval/kor/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/kor/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.384482 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     6239 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.388481 mteb-1.8.9/mteb/tasks/Retrieval/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/nob/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/nob/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.388481 mteb-1.8.9/mteb/tasks/Retrieval/pol/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.388481 mteb-1.8.9/mteb/tasks/Retrieval/slk/
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/slk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.388481 mteb-1.8.9/mteb/tasks/Retrieval/spa/
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.388481 mteb-1.8.9/mteb/tasks/Retrieval/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/Retrieval/tur/
+-rw-r--r--   0 root         (0) root         (0)     3883 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/tur/TurHistQuad.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/Retrieval/vie/
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/Retrieval/zho/
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Retrieval/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      787 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/STS/deu/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/STS/eng/
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/STS/fao/
+-rw-r--r--   0 root         (0) root         (0)     2015 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/fao/FaroeseSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.392481 mteb-1.8.9/mteb/tasks/STS/fin/
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/fin/FinParaSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/fin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/fra/
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/fra/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/jpn/JSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/kor/
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/kor/KlueSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/kor/KorSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     4131 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/pol/
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/pol/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/ron/
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/ron/RonSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/spa/
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/spa/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/STS/zho/
+-rw-r--r--   0 root         (0) root         (0)     7122 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/zho/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/STS/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.396482 mteb-1.8.9/mteb/tasks/Summarization/eng/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Summarization/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.400482 mteb-1.8.9/mteb/tasks/Summarization/fra/
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/Summarization/fra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      348 2024-05-11 13:08:00.000000 mteb-1.8.9/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.524482 mteb-1.8.9/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24072 2024-05-11 13:08:04.000000 mteb-1.8.9/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    74415 2024-05-11 13:08:04.000000 mteb-1.8.9/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 13:08:04.000000 mteb-1.8.9/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-11 13:08:04.000000 mteb-1.8.9/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-05-11 13:08:04.000000 mteb-1.8.9/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-11 13:08:04.000000 mteb-1.8.9/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-05-11 13:08:01.000000 mteb-1.8.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.304481 mteb-1.8.9/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.400482 mteb-1.8.9/results/GritLM__GritLM-7B/
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-05-11 13:08:00.000000 mteb-1.8.9/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-05-11 13:08:00.000000 mteb-1.8.9/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-05-11 13:08:00.000000 mteb-1.8.9/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.400482 mteb-1.8.9/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-05-11 13:08:00.000000 mteb-1.8.9/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.300481 mteb-1.8.9/results/dangvantuan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.404482 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
+-rw-r--r--   0 root         (0) root         (0)      676 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
+-rw-r--r--   0 root         (0) root         (0)      332 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      335 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)     2801 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      820 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/SICKFr.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/STS22.json
+-rw-r--r--   0 root         (0) root         (0)      921 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
+-rw-r--r--   0 root         (0) root         (0)      221 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-05-11 13:08:00.000000 mteb-1.8.9/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.300481 mteb-1.8.9/results/intfloat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.404482 mteb-1.8.9/results/intfloat/multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/HinDialectClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/MalayalamNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/MarathiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/OdiaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/SadeemQuestionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/SouthAfricanLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/TamilNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/TeluguAndhraJyotiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat/multilingual-e5-small/TswanaNewsClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.404482 mteb-1.8.9/results/intfloat__e5-small/
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__e5-small/TurkishProductSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.404482 mteb-1.8.9/results/intfloat__e5-small-v2/
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.408481 mteb-1.8.9/results/intfloat__multilingual-e5-base/
+-rw-r--r--   0 root         (0) root         (0)      758 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2281 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json
+-rw-r--r--   0 root         (0) root         (0)     2293 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-base/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.456482 mteb-1.8.9/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/AJGT.json
+-rw-r--r--   0 root         (0) root         (0)      375 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/AfriSentiLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ArxivClassification.json
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BengaliDocumentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BengaliSentimentAnalysis.json
+-rw-r--r--   0 root         (0) root         (0)   336719 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicensorLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADAntiAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADAuditRightsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADCapOnLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADChangeOfControlLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADCovenantNotToSueLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADEffectiveDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADExclusivityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADExpirationDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADGoverningLawLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADIPOwnershipAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADInsuranceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADJointIPOwnershipLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADLicenseGrantLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADLiquidatedDamagesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADMinimumCommitmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      396 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADMostFavoredNationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADNoSolicitOfCustomersLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADNoSolicitOfEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADNonCompeteLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      424 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADNonDisparagementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADNonTransferableLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADPostTerminationServicesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADPriceRestrictionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADRenewalTermLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADRevenueProfitSharingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADRofrRofoRofnLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADSourceCodeEscrowLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADTerminationForConvenienceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADThirdPartyBeneficiaryLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADUncappedLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADVolumeRestrictionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CUADWarrantyDurationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CanadaTaxCourtOutcomesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      616 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json
+-rw-r--r--   0 root         (0) root         (0)    13681 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIExplicitIdentificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      483 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLILimitedUseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLINoLicensingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      422 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIPermissibleCopyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLISharingWithEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ContractNLISurvivalOfObligationsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CorporateLobbyingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json
+-rw-r--r--   0 root         (0) root         (0)      738 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/DBpediaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/DefinitionClassificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/Diversity1LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/Diversity2LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/Diversity3LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/Diversity4LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/Diversity5LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/Diversity6LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FaroeseSTS.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      827 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FinToxicityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FinancialPhrasebankClassification.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FrenchBookReviews.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FrenkEnClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FrenkHrClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FrenkSlClassification.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/FunctionOfDecisionSectionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/GeorgianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/GermanDPR.json
+-rw-r--r--   0 root         (0) root         (0)      401 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/GermanPoliticiansTwitterSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/GreekCivicsQA.json
+-rw-r--r--   0 root         (0) root         (0)      606 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/HateSpeechPortugueseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     4319 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)    11798 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     4273 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3924 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      644 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/InsurancePolicyInterpretationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/InternationalCitizenshipQuestionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ItaCaseholdClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/JCrewBlockerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/JavaneseIMDBClassification.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/KLUE-TC.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/KannadaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7814 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7703 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LanguageClassification.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsBenefitsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsBusinessLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsConsumerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsCourtsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsCrimeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsDivorceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsDomesticViolenceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsEducationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsEmploymentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsEstatesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsFamilyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsHealthLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsHousingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsImmigrationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsTortsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LearnedHandsTrafficLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LegalBenchPC.json
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/LegalReasoningCausalityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2360 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MLQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3894 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     6649 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MultiEURLEXMultilabelClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MultiHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)     8513 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)   417235 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NepaliNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NordicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/PatentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      513 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/PunjabiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)    42700 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SIB200Classification.json
+-rw-r--r--   0 root         (0) root         (0)      298 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      584 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SentimentAnalysisHindi.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SinhalaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SinhalaNewsSourceClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SlovakSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      375 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SpanishNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SpanishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      304 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      893 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      629 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      522 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/ToxicConversationsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1166 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TweetTopicSingleClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/UrduRomanSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      368 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/WisesightSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    38759 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/XNLI.json
+-rw-r--r--   0 root         (0) root         (0)    18115 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/XNLIV2.json
+-rw-r--r--   0 root         (0) root         (0)    12839 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/XQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/YahooAnswersTopicsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/YelpReviewFullClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-11 13:08:00.000000 mteb-1.8.9/results/intfloat__multilingual-e5-small/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.304481 mteb-1.8.9/results/sentence-transformers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.456482 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/HinDialectClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MalayalamNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      368 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MarathiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/OdiaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SadeemQuestionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SouthAfricanLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TamilNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)    21290 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json
+-rw-r--r--   0 root         (0) root         (0)    21291 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TeluguAndhraJyotiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TswanaNewsClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.460482 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)   387673 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/model.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.516482 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AJGT.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AfriSentiLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClassification.json
+-rw-r--r--   0 root         (0) root         (0)      520 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliDocumentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliSentimentAnalysis.json
+-rw-r--r--   0 root         (0) root         (0)   338028 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      344 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicensorLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAntiAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAuditRightsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCapOnLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADChangeOfControlLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCovenantNotToSueLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADEffectiveDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExclusivityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExpirationDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADGoverningLawLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIPOwnershipAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADInsuranceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADJointIPOwnershipLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLicenseGrantLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLiquidatedDamagesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMinimumCommitmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMostFavoredNationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfCustomersLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonCompeteLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonDisparagementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonTransferableLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPostTerminationServicesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPriceRestrictionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRenewalTermLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRevenueProfitSharingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRofrRofoRofnLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADSourceCodeEscrowLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADTerminationForConvenienceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADThirdPartyBeneficiaryLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUncappedLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADVolumeRestrictionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADWarrantyDurationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CanadaTaxCourtOutcomesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json
+-rw-r--r--   0 root         (0) root         (0)    13663 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIExplicitIdentificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLILimitedUseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoLicensingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleCopyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISurvivalOfObligationsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CorporateLobbyingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json
+-rw-r--r--   0 root         (0) root         (0)     2295 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DBpediaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DefinitionClassificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity1LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity2LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity3LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity4LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity5LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity6LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FaroeseSTS.json
+-rw-r--r--   0 root         (0) root         (0)      746 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      835 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinToxicityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinancialPhrasebankClassification.json
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenchBookReviews.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkEnClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkHrClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkSlClassification.json
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FunctionOfDecisionSectionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GermanPoliticiansTwitterSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HateSpeechPortugueseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     4370 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     4276 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InsurancePolicyInterpretationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InternationalCitizenshipQuestionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      342 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaCaseholdClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JCrewBlockerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JavaneseIMDBClassification.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-TC.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KannadaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7839 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7915 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LanguageClassification.json
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBenefitsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBusinessLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsConsumerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCourtsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCrimeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDivorceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDomesticViolenceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEducationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEmploymentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEstatesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsFamilyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHealthLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHousingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsImmigrationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTortsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTrafficLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1443 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalReasoningCausalityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)   104611 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3884 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      748 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     6739 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiEURLEXMultilabelClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     8537 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)   421556 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NepaliNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3382 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3376 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NordicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)    16669 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PatentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    18247 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      741 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PunjabiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)    42635 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SentimentAnalysisHindi.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsSourceClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      637 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicChatClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicConversationsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetTopicSingleClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UrduRomanSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WisesightSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    38547 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json
+-rw-r--r--   0 root         (0) root         (0)    17971 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLIV2.json
+-rw-r--r--   0 root         (0) root         (0)    12890 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YahooAnswersTopicsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YelpReviewFullClassification.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-11 13:08:00.000000 mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.516482 mteb-1.8.9/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.516482 mteb-1.8.9/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.516482 mteb-1.8.9/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/medicalqaretrieval/
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/medicalqaretrieval/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/multilingual_sentiment_classification/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/multilingual_sentiment_classification/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/scala_classification/
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/scala_classification/create_multiling_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.520482 mteb-1.8.9/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.524482 mteb-1.8.9/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/toxic_conversations_50k/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.524482 mteb-1.8.9/scripts/data/xnli2/
+-rw-r--r--   0 root         (0) root         (0)      688 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/data/xnli2/create_multilang_ds.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/mteb_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.308481 mteb-1.8.9/scripts/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.524482 mteb-1.8.9/scripts/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.524482 mteb-1.8.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      673 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-11 13:08:00.000000 mteb-1.8.9/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 13:08:04.528482 mteb-1.8.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 13:08:04.524482 mteb-1.8.9/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_all_abstasks.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_encoder_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_mteb.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_mteb_rerank.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_overview.py
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-11 13:08:00.000000 mteb-1.8.9/tests/test_retrieval_abstask.py
```

### Comparing `mteb-1.8.8/LICENSE` & `mteb-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/PKG-INFO` & `mteb-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.8.8
+Version: 1.8.9
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.8.8/README.md` & `mteb-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/docs/create_tasks_table.py` & `mteb-1.8.9/docs/create_tasks_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/docs/mmteb/create_points_table.py` & `mteb-1.8.9/docs/mmteb/create_points_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/docs/mmteb/validate_points.py` & `mteb-1.8.9/docs/mmteb/validate_points.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTask.py` & `mteb-1.8.9/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskClusteringFast.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskClusteringFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskInstructionRetrieval.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskInstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.8.9/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/CrosslingualTask.py` & `mteb-1.8.9/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/LangMapping.py` & `mteb-1.8.9/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/MultiSubsetLoader.py` & `mteb-1.8.9/mteb/abstasks/MultiSubsetLoader.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/MultilingualTask.py` & `mteb-1.8.9/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/TaskMetadata.py` & `mteb-1.8.9/mteb/abstasks/TaskMetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from __future__ import annotations
 
 import logging
 from datetime import date
 from typing import List, Mapping, Union
 
-from pydantic import (
-    AnyUrl,
-    BaseModel,
-    BeforeValidator,
-    TypeAdapter,
-    field_validator,
-)
+from pydantic import AnyUrl, BaseModel, BeforeValidator, TypeAdapter, field_validator
 from typing_extensions import Annotated, Literal
 
 from .languages import (
     ISO_TO_LANGUAGE,
     ISO_TO_SCRIPT,
     path_to_lang_codes,
     path_to_lang_scripts,
@@ -76,14 +70,15 @@
     "low",
     "mixed",
 ]
 
 TASK_TYPE = Literal[
     "BitextMining",
     "Classification",
+    "MultilabelClassification",
     "Clustering",
     "PairClassification",
     "Reranking",
     "Retrieval",
     "STS",
     "Summarization",
     "InstructionRetrieval",
```

### Comparing `mteb-1.8.8/mteb/abstasks/iso_15924_to_script.json` & `mteb-1.8.9/mteb/abstasks/iso_15924_to_script.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/iso_639_3_to_language.json` & `mteb-1.8.9/mteb/abstasks/iso_639_3_to_language.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/abstasks/languages.py` & `mteb-1.8.9/mteb/abstasks/languages.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/benchmarks.py` & `mteb-1.8.9/mteb/benchmarks.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/cmd.py` & `mteb-1.8.9/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/encoder_interface.py` & `mteb-1.8.9/mteb/encoder_interface.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/MTEB.py` & `mteb-1.8.9/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,88 @@
 from __future__ import annotations
 
 import logging
 
 import numpy as np
 import torch
 from sklearn.linear_model import LogisticRegression
-from sklearn.metrics import accuracy_score, average_precision_score, f1_score
+from sklearn.metrics import (
+    accuracy_score,
+    average_precision_score,
+    f1_score,
+    label_ranking_average_precision_score,
+)
 from sklearn.neighbors import KNeighborsClassifier
 from torch import Tensor
 
 from .Evaluator import Evaluator
 
 logger = logging.getLogger(__name__)
 
 
+def dot_distance(a: np.ndarray, b: np.ndarray) -> float:
+    return -np.dot(a, b)
+
+
+class kNNMultiLabelClassificationEvaluator(Evaluator):
+    def __init__(
+        self,
+        embeddings_train,
+        y_train,
+        embeddings_test,
+        y_test,
+        k=1,
+        batch_size=32,
+        limit=None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        if limit is not None:
+            embeddings_train = embeddings_train[:limit]
+            y_train = y_train[:limit]
+            embeddings_test = embeddings_test[:limit]
+            y_test = y_test[:limit]
+        self.embeddings_train = embeddings_train
+        self.y_train = y_train
+        self.embeddings_test = embeddings_test
+        self.y_test = y_test
+
+        self.batch_size = batch_size
+
+        self.k = k
+
+    def __call__(self, model, test_cache=None):
+        scores = {}
+        max_accuracy = 0
+        max_f1 = 0
+        max_ap = 0
+        for metric_name in ["cosine", "euclidean", "dot"]:
+            if metric_name == "dot":
+                metric = dot_distance
+            else:
+                metric = metric_name
+            classifier = KNeighborsClassifier(n_neighbors=self.k, metric=metric)
+            classifier.fit(self.embeddings_train, self.y_train)
+            y_pred = classifier.predict(self.embeddings_test)
+            accuracy = classifier.score(self.embeddings_test, self.y_test)
+            f1 = f1_score(self.y_test, y_pred, average="macro")
+            scores["accuracy_" + metric_name] = accuracy
+            scores["f1_" + metric_name] = f1
+            max_accuracy = max(max_accuracy, accuracy)
+            max_f1 = max(max_f1, f1)
+            lrap = label_ranking_average_precision_score(self.y_test, y_pred)
+            scores["lrap_" + metric_name] = lrap
+            max_ap = max(max_ap, lrap)
+        scores["accuracy"] = max_accuracy
+        scores["f1"] = max_f1
+        if len(np.unique(self.y_train)) == 2:
+            scores["lrap"] = max_ap
+        return scores, test_cache
+
+
 class kNNClassificationEvaluator(Evaluator):
     def __init__(
         self,
         sentences_train,
         y_train,
         sentences_test,
         y_test,
```

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.8.9/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/evaluation/evaluators/utils.py` & `mteb-1.8.9/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/logging.py` & `mteb-1.8.9/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/overview.py` & `mteb-1.8.9/mteb/overview.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/__init__.py` & `mteb-1.8.9/mteb/tasks/BitextMining/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py` & `mteb-1.8.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py` & `mteb-1.8.9/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py` & `mteb-1.8.9/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/__init__.py` & `mteb-1.8.9/mteb/tasks/Classification/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from .ita.ItalianLinguistAcceptabilityClassification import *
 from .jav.JavaneseIMDBClassification import *
 from .jpn.WRIMEClassification import *
 from .kan.KannadaNewsClassification import *
 from .kor.KlueTC import *
 from .kur.KurdishSentimentClassification import *
 from .mal.MalayalamNewsClassification import *
+from .mar.MarathiNewsClassification import *
 from .mkd.MacedonianTweetSentimentClassification import *
 from .multilingual.AfriSentiLangClassification import *
 from .multilingual.AmazonCounterfactualClassification import *
 from .multilingual.AmazonReviewsClassification import *
 from .multilingual.HinDialectClassification import *
 from .multilingual.IndicLangClassification import *
 from .multilingual.IndicSentimentClassification import *
```

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ara/AJGT.py` & `mteb-1.8.9/mteb/tasks/Classification/ara/AJGT.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ara/TweetEmotionClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ara/TweetEmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ara/TweetSarcasmClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ara/TweetSarcasmClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ben/BengaliDocumentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ben/BengaliDocumentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py` & `mteb-1.8.9/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py` & `mteb-1.8.9/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/dan/DKHateClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/dan/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/dan/LccSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/dan/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/ArxivClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/ArxivClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/Banking77Classification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/DBpediaClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/DBpediaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/EmotionClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/FrenkEnClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/FrenkEnClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/ImdbClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/LegalBenchClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/LegalBenchClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/NewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/NewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/PatentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/PatentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/ToxicChatClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/ToxicChatClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/eng/YelpReviewFullClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/eng/YelpReviewFullClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/est/estonian_valence.py` & `mteb-1.8.9/mteb/tasks/Classification/est/estonian_valence.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/fin/FinToxicityClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/fin/FinToxicityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/fra/FrenchBookReviews.py` & `mteb-1.8.9/mteb/tasks/Classification/fra/FrenchBookReviews.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/guj/GujaratiNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/guj/GujaratiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py` & `mteb-1.8.9/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/hrv/FrenkHrClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/hrv/FrenkHrClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ita/ItaCaseholdClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ita/ItaCaseholdClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/jpn/WRIMEClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/jpn/WRIMEClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/kan/KannadaNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/kan/KannadaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/kor/KlueTC.py` & `mteb-1.8.9/mteb/tasks/Classification/kor/KlueTC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/kur/KurdishSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/kur/KurdishSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/mal/MalayalamNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/mal/MalayalamNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/HinDialectClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/HinDialectClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicLangClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/IndicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/LanguageClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/LanguageClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/MultiHateClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/MultiHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/SIB200Classification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/SIB200Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/nep/NepaliNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/nep/NepaliNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/nob/NoRecClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/nob/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ory/OdiaNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ory/OdiaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/pan/PunjabiNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/pan/PunjabiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/pol/PolishClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/pol/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ron/RomanianSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ron/RomanianSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/san/SanskritShlokasClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/san/SanskritShlokasClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/sin/SinhalaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/slv/FrenkSlClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/slv/FrenkSlClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/spa/SpanishNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/spa/SpanishNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/spa/SpanishSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/spa/SpanishSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/swe/DalajClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/swe/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/swe/SweRecClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/swe/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/tam/TamilNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/tam/TamilNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/tha/WisesightSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/tha/WisesightSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/tsn/TswanaNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/tsn/TswanaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/ukr/UkrFormalityClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/ukr/UkrFormalityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/zho/CMTEBClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/zho/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py` & `mteb-1.8.9/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/__init__.py` & `mteb-1.8.9/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py` & `mteb-1.8.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/BigPatentClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/nob/snl_clustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/nob/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/nob/vg_clustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/nob/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/pol/PolishClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/pol/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/rom/RomaniBibleClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/rom/RomaniBibleClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py` & `mteb-1.8.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py` & `mteb-1.8.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/swe/SwednClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/swe/SwednClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/swe/swedn_clustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/swe/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Clustering/zho/CMTEBClustering.py` & `mteb-1.8.9/mteb/tasks/Clustering/zho/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py` & `mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py` & `mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py` & `mteb-1.8.9/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/eng/LegalBenchPC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/eng/LegalBenchPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.8.9/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/multilingual/XNLI.py` & `mteb-1.8.9/mteb/tasks/PairClassification/multilingual/XNLI.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/pol/PolishPC.py` & `mteb-1.8.9/mteb/tasks/PairClassification/pol/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py` & `mteb-1.8.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py` & `mteb-1.8.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/eng/MindSmallReranking.py` & `mteb-1.8.9/mteb/tasks/Reranking/eng/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/eng/SciDocsReranking.py` & `mteb-1.8.9/mteb/tasks/Reranking/eng/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py` & `mteb-1.8.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/fra/AlloprofReranking.py` & `mteb-1.8.9/mteb/tasks/Reranking/fra/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/fra/SyntecReranking.py` & `mteb-1.8.9/mteb/tasks/Reranking/fra/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.8.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Reranking/zho/CMTEBReranking.py` & `mteb-1.8.9/mteb/tasks/Reranking/zho/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/__init__.py` & `mteb-1.8.9/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/ara/SadeemQuestionRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/ara/SadeemQuestionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/dan/dan_fever.py` & `mteb-1.8.9/mteb/tasks/Retrieval/dan/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/dan/twitterhjerne.py` & `mteb-1.8.9/mteb/tasks/Retrieval/dan/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/ell/GreekCivicsQA.py` & `mteb-1.8.9/mteb/tasks/Retrieval/ell/GreekCivicsQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/NQRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/est/estqa.py` & `mteb-1.8.9/mteb/tasks/Retrieval/est/estqa.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/fra/FQuADRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/fra/FQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/hun/HunSum2.py` & `mteb-1.8.9/mteb/tasks/Retrieval/hun/HunSum2.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/kor/KoMiracl.py` & `mteb-1.8.9/mteb/tasks/Retrieval/kor/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py` & `mteb-1.8.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/nob/norquad.py` & `mteb-1.8.9/mteb/tasks/Retrieval/nob/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/nob/snl_retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/nob/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py` & `mteb-1.8.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py` & `mteb-1.8.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/tur/TurHistQuad.py` & `mteb-1.8.9/mteb/tasks/Retrieval/tur/TurHistQuad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py` & `mteb-1.8.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/__init__.py` & `mteb-1.8.9/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py` & `mteb-1.8.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/BiossesSTS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/STS12STS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/STS13STS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/STS14STS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/STS15STS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/STS16STS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/eng/SickrSTS.py` & `mteb-1.8.9/mteb/tasks/STS/eng/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/fao/FaroeseSTS.py` & `mteb-1.8.9/mteb/tasks/STS/fao/FaroeseSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/fin/FinParaSTS.py` & `mteb-1.8.9/mteb/tasks/STS/fin/FinParaSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/fra/SickFrSTS.py` & `mteb-1.8.9/mteb/tasks/STS/fra/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/jpn/JSTS.py` & `mteb-1.8.9/mteb/tasks/STS/jpn/JSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/kor/KlueSTS.py` & `mteb-1.8.9/mteb/tasks/STS/kor/KlueSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/kor/KorSTS.py` & `mteb-1.8.9/mteb/tasks/STS/kor/KorSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py` & `mteb-1.8.9/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.8.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.8.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.8.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/pol/PolishSTS.py` & `mteb-1.8.9/mteb/tasks/STS/pol/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/ron/RonSTS.py` & `mteb-1.8.9/mteb/tasks/STS/ron/RonSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/spa/STSES.py` & `mteb-1.8.9/mteb/tasks/STS/spa/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/STS/zho/CMTEBSTS.py` & `mteb-1.8.9/mteb/tasks/STS/zho/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py` & `mteb-1.8.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py` & `mteb-1.8.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/mteb.egg-info/PKG-INFO` & `mteb-1.8.9/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.8.8
+Version: 1.8.9
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.8.8/mteb.egg-info/SOURCES.txt` & `mteb-1.8.9/mteb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 mteb.egg-info/top_level.txt
 mteb/abstasks/AbsTask.py
 mteb/abstasks/AbsTaskBitextMining.py
 mteb/abstasks/AbsTaskClassification.py
 mteb/abstasks/AbsTaskClustering.py
 mteb/abstasks/AbsTaskClusteringFast.py
 mteb/abstasks/AbsTaskInstructionRetrieval.py
+mteb/abstasks/AbsTaskMultilabelClassification.py
 mteb/abstasks/AbsTaskPairClassification.py
 mteb/abstasks/AbsTaskReranking.py
 mteb/abstasks/AbsTaskRetrieval.py
 mteb/abstasks/AbsTaskSTS.py
 mteb/abstasks/AbsTaskSummarization.py
 mteb/abstasks/CrosslingualTask.py
 mteb/abstasks/LangMapping.py
@@ -151,14 +152,16 @@
 mteb/tasks/Classification/kat/GeorgianSentimentClassification.py
 mteb/tasks/Classification/kat/__init__.py
 mteb/tasks/Classification/kor/KlueTC.py
 mteb/tasks/Classification/kur/KurdishSentimentClassification.py
 mteb/tasks/Classification/kur/__init__.py
 mteb/tasks/Classification/mal/MalayalamNewsClassification.py
 mteb/tasks/Classification/mal/__init__.py
+mteb/tasks/Classification/mar/MarathiNewsClassification.py
+mteb/tasks/Classification/mar/__init__.py
 mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
 mteb/tasks/Classification/mkd/__init__.py
 mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py
 mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
 mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
 mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py
 mteb/tasks/Classification/multilingual/HinDialectClassification.py
@@ -282,14 +285,16 @@
 mteb/tasks/Clustering/zho/CMTEBClustering.py
 mteb/tasks/Clustering/zho/__init__.py
 mteb/tasks/InstructionRetrieval/__init__.py
 mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
 mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
 mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
 mteb/tasks/InstructionRetrieval/eng/__init__.py
+mteb/tasks/MultiLabelClassification/__init__.py
+mteb/tasks/MultiLabelClassification/multilingual/MultiEURLEXMultilabelClassification.py
 mteb/tasks/PairClassification/__init__.py
 mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
 mteb/tasks/PairClassification/deu/__init__.py
 mteb/tasks/PairClassification/eng/LegalBenchPC.py
 mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
 mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
 mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
@@ -497,14 +502,15 @@
 results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
 results/dangvantuan/sentence-camembert-base/SummEvalFr.json
 results/dangvantuan/sentence-camembert-base/SyntecReranking.json
 results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
 results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
 results/intfloat/multilingual-e5-small/HinDialectClassification.json
 results/intfloat/multilingual-e5-small/MalayalamNewsClassification.json
+results/intfloat/multilingual-e5-small/MarathiNewsClassification.json
 results/intfloat/multilingual-e5-small/OdiaNewsClassification.json
 results/intfloat/multilingual-e5-small/SadeemQuestionRetrieval.json
 results/intfloat/multilingual-e5-small/SouthAfricanLangClassification.json
 results/intfloat/multilingual-e5-small/TamilNewsClassification.json
 results/intfloat/multilingual-e5-small/TeluguAndhraJyotiNewsClassification.json
 results/intfloat/multilingual-e5-small/TswanaNewsClassification.json
 results/intfloat__e5-small/TurkishProductSentimentClassification.json
@@ -684,14 +690,15 @@
 results/intfloat__multilingual-e5-small/LegalReasoningCausalityLegalBenchClassification.json
 results/intfloat__multilingual-e5-small/MLQARetrieval.json
 results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json
 results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json
 results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
 results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
 results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
+results/intfloat__multilingual-e5-small/MultiEURLEXMultilabelClassification.json
 results/intfloat__multilingual-e5-small/MultiHateClassification.json
 results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json
 results/intfloat__multilingual-e5-small/NTREXBitextMining.json
 results/intfloat__multilingual-e5-small/NepaliNewsClassification.json
 results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
 results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
 results/intfloat__multilingual-e5-small/NewsClassification.json
@@ -756,14 +763,15 @@
 results/intfloat__multilingual-e5-small/XQuADRetrieval.json
 results/intfloat__multilingual-e5-small/YahooAnswersTopicsClassification.json
 results/intfloat__multilingual-e5-small/YelpReviewFullClassification.json
 results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
 results/intfloat__multilingual-e5-small/model_meta.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/HinDialectClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MalayalamNewsClassification.json
+results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MarathiNewsClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/OdiaNewsClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SadeemQuestionRetrieval.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SouthAfricanLangClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TamilNewsClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TeluguAndhraJyotiNewsClassification.json
@@ -946,14 +954,15 @@
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalReasoningCausalityLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiEURLEXMultilabelClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NepaliNewsClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
```

### Comparing `mteb-1.8.8/pyproject.toml` & `mteb-1.8.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.8.8"
+version = "1.8.9"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.8.8/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json` & `mteb-1.8.9/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/GritLM__GritLM-7B/News21InstructionRetrieval.json` & `mteb-1.8.9/results/GritLM__GritLM-7B/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json` & `mteb-1.8.9/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json` & `mteb-1.8.9/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/PawsX.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SICKFr.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/SICKFr.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json` & `mteb-1.8.9/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat/multilingual-e5-small/SadeemQuestionRetrieval.json` & `mteb-1.8.9/results/intfloat/multilingual-e5-small/SadeemQuestionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json` & `mteb-1.8.9/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__e5-small-v2/News21InstructionRetrieval.json` & `mteb-1.8.9/results/intfloat__e5-small-v2/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json` & `mteb-1.8.9/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/BSARDRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/BSARDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/DanFEVER.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/EstQA.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/FQuADRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/FinParaSTS.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/FinParaSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/GermanDPR.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/GermanDPR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekCivicsQA.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/GreekCivicsQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicQARetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/LegalBenchPC.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/LegalBenchPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/MLQARetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/MLQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/MultiHateClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/MultiHateClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/NTREXBitextMining.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/NTREXBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SIB200Classification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SIB200Classification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/SyntecRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLI.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/XNLI.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLIV2.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/XNLIV2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/intfloat__multilingual-e5-small/XQuADRetrieval.json` & `mteb-1.8.9/results/intfloat__multilingual-e5-small/XQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SadeemQuestionRetrieval.json` & `mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SadeemQuestionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json` & `mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json` & `mteb-1.8.9/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLIV2.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLIV2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json` & `mteb-1.8.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/amazon_polarity/create_data.py` & `mteb-1.8.9/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.8.9/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/arxiv/script_clustering.py` & `mteb-1.8.9/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/arxiv/script_raw.py` & `mteb-1.8.9/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/biorxiv/script_clustering.py` & `mteb-1.8.9/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/biorxiv/script_raw.py` & `mteb-1.8.9/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/bucc/create_data.py` & `mteb-1.8.9/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/create_task_table.py` & `mteb-1.8.9/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/germanquad/process_data.py` & `mteb-1.8.9/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/hal/create_data.py` & `mteb-1.8.9/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/imdb/create_data.py` & `mteb-1.8.9/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/medicalqaretrieval/create_data.py` & `mteb-1.8.9/scripts/data/medicalqaretrieval/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/medrxiv/script_clustering.py` & `mteb-1.8.9/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/medrxiv/script_raw.py` & `mteb-1.8.9/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/mind/prepare_data.py` & `mteb-1.8.9/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/multilingual_sentiment_classification/create_data.py` & `mteb-1.8.9/scripts/data/multilingual_sentiment_classification/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/redditp2p/script_clustering.py` & `mteb-1.8.9/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.8.9/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.8.9/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/summeval_fr/create_data.py` & `mteb-1.8.9/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.8.9/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/data/xnli2/create_multilang_ds.py` & `mteb-1.8.9/scripts/data/xnli2/create_multilang_ds.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/merge_cqadupstack.py` & `mteb-1.8.9/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/mteb_meta.py` & `mteb-1.8.9/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/run_mteb_chinese.py` & `mteb-1.8.9/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/run_mteb_english.py` & `mteb-1.8.9/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/run_mteb_french.py` & `mteb-1.8.9/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/run_mteb_german.py` & `mteb-1.8.9/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/run_mteb_korean.py` & `mteb-1.8.9/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/run_mteb_law.py` & `mteb-1.8.9/scripts/run_mteb_law.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/scripts/run_mteb_polish.py` & `mteb-1.8.9/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_ClusteringEvaluator.py` & `mteb-1.8.9/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_InstructionRetrievalEvaluator.py` & `mteb-1.8.9/tests/test_InstructionRetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_PairClassificationEvaluator.py` & `mteb-1.8.9/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_RerankingEvaluator.py` & `mteb-1.8.9/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_RetrievalEvaluator.py` & `mteb-1.8.9/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_TaskMetadata.py` & `mteb-1.8.9/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_all_abstasks.py` & `mteb-1.8.9/tests/test_all_abstasks.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_encoder_interfaces.py` & `mteb-1.8.9/tests/test_encoder_interfaces.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_mteb.py` & `mteb-1.8.9/tests/test_mteb.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_mteb_rerank.py` & `mteb-1.8.9/tests/test_mteb_rerank.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.8/tests/test_overview.py` & `mteb-1.8.9/tests/test_overview.py`

 * *Files identical despite different names*

