# Comparing `tmp/oc_ds_converter-1.0.2.tar.gz` & `tmp/oc_ds_converter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ds_converter-1.0.2.tar", max compression
+gzip compressed data, was "oc_ds_converter-1.0.3.tar", max compression
```

## Comparing `oc_ds_converter-1.0.2.tar` & `oc_ds_converter-1.0.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.455704 oc_ds_converter-1.0.2/oc_ds_converter/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.456704 oc_ds_converter-1.0.2/oc_ds_converter/crossref/__init__.py
--rw-r--r--   0        0        0    27506 2024-04-18 13:08:16.457703 oc_ds_converter-1.0.2/oc_ds_converter/crossref/crossref_processing.py
--rw-r--r--   0        0        0     4337 2024-04-18 13:08:16.458701 oc_ds_converter-1.0.2/oc_ds_converter/crossref/extract_crossref_publishers.py
--rw-r--r--   0        0        0     9101 2024-04-18 13:08:16.459704 oc_ds_converter-1.0.2/oc_ds_converter/crossref/get_not_crossref_ref.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.459704 oc_ds_converter-1.0.2/oc_ds_converter/datacite/__init__.py
--rw-r--r--   0        0        0    38522 2024-04-18 13:08:16.460703 oc_ds_converter-1.0.2/oc_ds_converter/datacite/datacite_processing.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.461708 oc_ds_converter-1.0.2/oc_ds_converter/datasource/__init__.py
--rw-r--r--   0        0        0      336 2024-04-18 13:08:16.462704 oc_ds_converter-1.0.2/oc_ds_converter/datasource/config.ini
--rw-r--r--   0        0        0     1329 2024-04-18 13:08:16.462704 oc_ds_converter-1.0.2/oc_ds_converter/datasource/datasource.py
--rw-r--r--   0        0        0     3702 2024-04-18 13:08:16.463706 oc_ds_converter-1.0.2/oc_ds_converter/datasource/redis.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.464704 oc_ds_converter-1.0.2/oc_ds_converter/jalc/__init__.py
--rw-r--r--   0        0        0    17007 2024-04-18 13:08:16.465704 oc_ds_converter-1.0.2/oc_ds_converter/jalc/jalc_processing.py
--rw-r--r--   0        0        0     1025 2024-04-18 13:08:16.466705 oc_ds_converter-1.0.2/oc_ds_converter/lib/__init__.py
--rw-r--r--   0        0        0    17248 2024-04-18 13:08:16.467705 oc_ds_converter-1.0.2/oc_ds_converter/lib/cleaner.py
--rw-r--r--   0        0        0     6083 2024-04-18 13:08:16.468706 oc_ds_converter-1.0.2/oc_ds_converter/lib/csvmanager.py
--rw-r--r--   0        0        0     9573 2024-04-18 13:08:16.469705 oc_ds_converter-1.0.2/oc_ds_converter/lib/file_manager.py
--rw-r--r--   0        0        0     6423 2024-04-18 13:08:16.470706 oc_ds_converter-1.0.2/oc_ds_converter/lib/jsonmanager.py
--rw-r--r--   0        0        0     5260 2024-04-18 13:08:16.471706 oc_ds_converter-1.0.2/oc_ds_converter/lib/master_of_regex.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.471706 oc_ds_converter-1.0.2/oc_ds_converter/medra/__init__.py
--rw-r--r--   0        0        0    12416 2024-04-18 13:08:16.472705 oc_ds_converter-1.0.2/oc_ds_converter/medra/medra_processing.py
--rw-r--r--   0        0        0     3843 2024-04-18 13:08:16.473705 oc_ds_converter-1.0.2/oc_ds_converter/metadata_manager.py
--rw-r--r--   0        0        0     1877 2024-04-18 13:08:16.474704 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/__init__.py
--rw-r--r--   0        0        0     9816 2024-04-18 13:08:16.475703 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/arxiv.py
--rw-r--r--   0        0        0     5612 2024-04-18 13:08:16.476706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/base.py
--rw-r--r--   0        0        0     5247 2024-04-18 13:08:16.477705 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/crossref.py
--rw-r--r--   0        0        0    11303 2024-04-18 13:08:16.478706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/doi.py
--rw-r--r--   0        0        0     3602 2024-04-18 13:08:16.479707 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/isbn.py
--rw-r--r--   0        0        0     3069 2024-04-18 13:08:16.479707 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/issn.py
--rw-r--r--   0        0        0     8567 2024-04-18 13:08:16.480703 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/jid.py
--rw-r--r--   0        0        0     3845 2024-04-18 13:08:16.480703 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/metadata_manager.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.481705 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/__init__.py
--rw-r--r--   0        0        0     5443 2024-04-18 13:08:16.482705 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py
--rw-r--r--   0        0        0     5011 2024-04-18 13:08:16.483705 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py
--rw-r--r--   0        0        0     5973 2024-04-18 13:08:16.484706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py
--rw-r--r--   0        0        0     2042 2024-04-18 13:08:16.485706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py
--rw-r--r--   0        0        0     7243 2024-04-18 13:08:16.485706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/openalex.py
--rw-r--r--   0        0        0     8915 2024-04-18 13:08:16.486704 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/orcid.py
--rw-r--r--   0        0        0     7317 2024-04-18 13:08:16.487704 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/pmcid.py
--rw-r--r--   0        0        0    16651 2024-04-18 13:08:16.488704 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/pmid.py
--rw-r--r--   0        0        0     5903 2024-04-18 13:08:16.489706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/ror.py
--rw-r--r--   0        0        0     2094 2024-04-18 13:08:16.489706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/support.py
--rw-r--r--   0        0        0     6081 2024-04-18 13:08:16.490705 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/url.py
--rw-r--r--   0        0        0     6637 2024-04-18 13:08:16.491703 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/viaf.py
--rw-r--r--   0        0        0     6116 2024-04-18 13:08:16.492708 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/wikidata.py
--rw-r--r--   0        0        0     6304 2024-04-18 13:08:16.493706 oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/wikipedia.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.493706 oc_ds_converter-1.0.2/oc_ds_converter/openaire/__init__.py
--rw-r--r--   0        0        0    34044 2024-04-18 13:08:16.495703 oc_ds_converter-1.0.2/oc_ds_converter/openaire/openaire_processing.py
--rw-r--r--   0        0        0        2 2024-04-18 13:08:16.495703 oc_ds_converter-1.0.2/oc_ds_converter/openaire/support_files/prefix_publishers.json
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.496704 oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/__init__.py
--rw-r--r--   0        0        0     4315 2024-04-18 13:08:16.497704 oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/base.py
--rw-r--r--   0        0        0     6110 2024-04-18 13:08:16.498704 oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/datacite.py
--rw-r--r--   0        0        0    14692 2024-04-18 13:08:16.499705 oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/jalc.py
--rw-r--r--   0        0        0     4827 2024-04-18 13:08:16.500706 oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/nih.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.500706 oc_ds_converter-1.0.2/oc_ds_converter/pubmed/__init__.py
--rw-r--r--   0        0        0     4715 2024-04-18 13:08:16.501703 oc_ds_converter-1.0.2/oc_ds_converter/pubmed/finder_nih.py
--rw-r--r--   0        0        0     7950 2024-04-18 13:08:16.502704 oc_ds_converter-1.0.2/oc_ds_converter/pubmed/get_publishers.py
--rw-r--r--   0        0        0     2428 2024-04-18 13:08:16.503704 oc_ds_converter-1.0.2/oc_ds_converter/pubmed/pubmed_dump_explorer.py
--rw-r--r--   0        0        0    35075 2024-04-18 13:08:16.504704 oc_ds_converter-1.0.2/oc_ds_converter/pubmed/pubmed_processing.py
--rw-r--r--   0        0        0      503 2024-04-18 13:08:16.505721 oc_ds_converter-1.0.2/oc_ds_converter/pubmed/support_files/issn_jour_ext.json
--rw-r--r--   0        0        0   315988 2024-04-18 13:08:16.509702 oc_ds_converter-1.0.2/oc_ds_converter/pubmed/support_files/prefix_publishers.json
--rw-r--r--   0        0        0    11903 2024-04-18 13:08:16.510702 oc_ds_converter-1.0.2/oc_ds_converter/ra_processor.py
--rw-r--r--   0        0        0        0 2024-04-18 13:08:16.511704 oc_ds_converter-1.0.2/oc_ds_converter/run/__init__.py
--rw-r--r--   0        0        0    25869 2024-04-18 13:08:16.512704 oc_ds_converter-1.0.2/oc_ds_converter/run/crossref_process.py
--rw-r--r--   0        0        0    29918 2024-04-18 13:08:16.513702 oc_ds_converter-1.0.2/oc_ds_converter/run/datacite_process.py
--rw-r--r--   0        0        0    25140 2024-04-18 13:08:16.514703 oc_ds_converter-1.0.2/oc_ds_converter/run/jalc_process.py
--rw-r--r--   0        0        0    26521 2024-04-18 13:08:16.515704 oc_ds_converter-1.0.2/oc_ds_converter/run/openaire_process.py
--rw-r--r--   0        0        0     9887 2024-04-18 13:08:16.516704 oc_ds_converter-1.0.2/oc_ds_converter/run/pubmed_process.py
--rw-r--r--   0        0        0    33527 2024-04-18 13:08:16.517704 oc_ds_converter-1.0.2/oc_ds_converter/run/pubmed_process_new.py
--rw-r--r--   0        0        0     1086 2024-04-18 13:20:23.918365 oc_ds_converter-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    23044 2024-04-18 13:08:16.450708 oc_ds_converter-1.0.2/README.md
--rw-r--r--   0        0        0    24279 1970-01-01 00:00:00.000000 oc_ds_converter-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.501975 oc_ds_converter-1.0.3/oc_ds_converter/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.502976 oc_ds_converter-1.0.3/oc_ds_converter/crossref/__init__.py
+-rw-r--r--   0        0        0    27506 2024-05-12 17:23:29.502976 oc_ds_converter-1.0.3/oc_ds_converter/crossref/crossref_processing.py
+-rw-r--r--   0        0        0     4337 2024-05-12 17:23:29.502976 oc_ds_converter-1.0.3/oc_ds_converter/crossref/extract_crossref_publishers.py
+-rw-r--r--   0        0        0     9101 2024-05-12 17:23:29.503975 oc_ds_converter-1.0.3/oc_ds_converter/crossref/get_not_crossref_ref.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.503975 oc_ds_converter-1.0.3/oc_ds_converter/datacite/__init__.py
+-rw-r--r--   0        0        0    38522 2024-05-12 17:23:29.503975 oc_ds_converter-1.0.3/oc_ds_converter/datacite/datacite_processing.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.503975 oc_ds_converter-1.0.3/oc_ds_converter/datasource/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-12 17:23:29.503975 oc_ds_converter-1.0.3/oc_ds_converter/datasource/config.ini
+-rw-r--r--   0        0        0     1329 2024-05-12 17:23:29.503975 oc_ds_converter-1.0.3/oc_ds_converter/datasource/datasource.py
+-rw-r--r--   0        0        0     3702 2024-05-12 17:23:29.504976 oc_ds_converter-1.0.3/oc_ds_converter/datasource/redis.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.504976 oc_ds_converter-1.0.3/oc_ds_converter/jalc/__init__.py
+-rw-r--r--   0        0        0    17007 2024-05-12 17:23:29.504976 oc_ds_converter-1.0.3/oc_ds_converter/jalc/jalc_processing.py
+-rw-r--r--   0        0        0     1025 2024-05-12 17:23:29.504976 oc_ds_converter-1.0.3/oc_ds_converter/lib/__init__.py
+-rw-r--r--   0        0        0    17248 2024-05-12 17:23:29.504976 oc_ds_converter-1.0.3/oc_ds_converter/lib/cleaner.py
+-rw-r--r--   0        0        0     6083 2024-05-12 17:23:29.505976 oc_ds_converter-1.0.3/oc_ds_converter/lib/csvmanager.py
+-rw-r--r--   0        0        0     9573 2024-05-12 17:23:29.505976 oc_ds_converter-1.0.3/oc_ds_converter/lib/file_manager.py
+-rw-r--r--   0        0        0     6423 2024-05-12 17:23:29.505976 oc_ds_converter-1.0.3/oc_ds_converter/lib/jsonmanager.py
+-rw-r--r--   0        0        0     5260 2024-05-12 17:23:29.505976 oc_ds_converter-1.0.3/oc_ds_converter/lib/master_of_regex.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.505976 oc_ds_converter-1.0.3/oc_ds_converter/medra/__init__.py
+-rw-r--r--   0        0        0    12416 2024-05-12 17:23:29.506976 oc_ds_converter-1.0.3/oc_ds_converter/medra/medra_processing.py
+-rw-r--r--   0        0        0     3843 2024-05-12 17:23:29.506976 oc_ds_converter-1.0.3/oc_ds_converter/metadata_manager.py
+-rw-r--r--   0        0        0     1877 2024-05-12 17:23:29.506976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-12 17:23:29.506976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/arxiv.py
+-rw-r--r--   0        0        0     5612 2024-05-12 17:23:29.506976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/base.py
+-rw-r--r--   0        0        0     5247 2024-05-12 17:23:29.507976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/crossref.py
+-rw-r--r--   0        0        0    11303 2024-05-12 17:23:29.507976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/doi.py
+-rw-r--r--   0        0        0     3602 2024-05-12 17:23:29.507976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/isbn.py
+-rw-r--r--   0        0        0     3069 2024-05-12 17:23:29.507976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/issn.py
+-rw-r--r--   0        0        0     8567 2024-05-12 17:23:29.507976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/jid.py
+-rw-r--r--   0        0        0     3845 2024-05-12 17:23:29.507976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/metadata_manager.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.508976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/__init__.py
+-rw-r--r--   0        0        0     5443 2024-05-12 17:23:29.508976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py
+-rw-r--r--   0        0        0     5011 2024-05-12 17:23:29.508976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py
+-rw-r--r--   0        0        0     5973 2024-05-12 17:23:29.508976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py
+-rw-r--r--   0        0        0     2042 2024-05-12 17:23:29.508976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py
+-rw-r--r--   0        0        0     7243 2024-05-12 17:23:29.509976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/openalex.py
+-rw-r--r--   0        0        0     8915 2024-05-12 17:23:29.509976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/orcid.py
+-rw-r--r--   0        0        0     7317 2024-05-12 17:23:29.509976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/pmcid.py
+-rw-r--r--   0        0        0    16651 2024-05-12 17:23:29.509976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/pmid.py
+-rw-r--r--   0        0        0     5903 2024-05-12 17:23:29.509976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/ror.py
+-rw-r--r--   0        0        0     2094 2024-05-12 17:23:29.510976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/support.py
+-rw-r--r--   0        0        0     6081 2024-05-12 17:23:29.510976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/url.py
+-rw-r--r--   0        0        0     6637 2024-05-12 17:23:29.510976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/viaf.py
+-rw-r--r--   0        0        0     6116 2024-05-12 17:23:29.510976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/wikidata.py
+-rw-r--r--   0        0        0     6304 2024-05-12 17:23:29.510976 oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/wikipedia.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.510976 oc_ds_converter-1.0.3/oc_ds_converter/openaire/__init__.py
+-rw-r--r--   0        0        0    34044 2024-05-12 17:23:29.511976 oc_ds_converter-1.0.3/oc_ds_converter/openaire/openaire_processing.py
+-rw-r--r--   0        0        0        2 2024-05-12 17:23:29.511976 oc_ds_converter-1.0.3/oc_ds_converter/openaire/support_files/prefix_publishers.json
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.511976 oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4315 2024-05-12 17:23:29.511976 oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/base.py
+-rw-r--r--   0        0        0     6110 2024-05-12 17:23:29.511976 oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/datacite.py
+-rw-r--r--   0        0        0    14692 2024-05-12 17:23:29.512976 oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/jalc.py
+-rw-r--r--   0        0        0     4827 2024-05-12 17:23:29.512976 oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/nih.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.512976 oc_ds_converter-1.0.3/oc_ds_converter/pubmed/__init__.py
+-rw-r--r--   0        0        0     4715 2024-05-12 17:23:29.512976 oc_ds_converter-1.0.3/oc_ds_converter/pubmed/finder_nih.py
+-rw-r--r--   0        0        0     7950 2024-05-12 17:23:29.512976 oc_ds_converter-1.0.3/oc_ds_converter/pubmed/get_publishers.py
+-rw-r--r--   0        0        0     2428 2024-05-12 17:23:29.513975 oc_ds_converter-1.0.3/oc_ds_converter/pubmed/pubmed_dump_explorer.py
+-rw-r--r--   0        0        0    35075 2024-05-12 17:23:29.513975 oc_ds_converter-1.0.3/oc_ds_converter/pubmed/pubmed_processing.py
+-rw-r--r--   0        0        0      503 2024-05-12 17:23:29.513975 oc_ds_converter-1.0.3/oc_ds_converter/pubmed/support_files/issn_jour_ext.json
+-rw-r--r--   0        0        0   315988 2024-05-12 17:23:29.514976 oc_ds_converter-1.0.3/oc_ds_converter/pubmed/support_files/prefix_publishers.json
+-rw-r--r--   0        0        0    11903 2024-05-12 17:23:29.515976 oc_ds_converter-1.0.3/oc_ds_converter/ra_processor.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:23:29.515976 oc_ds_converter-1.0.3/oc_ds_converter/run/__init__.py
+-rw-r--r--   0        0        0    25869 2024-05-12 17:23:29.515976 oc_ds_converter-1.0.3/oc_ds_converter/run/crossref_process.py
+-rw-r--r--   0        0        0    29918 2024-05-12 17:23:29.515976 oc_ds_converter-1.0.3/oc_ds_converter/run/datacite_process.py
+-rw-r--r--   0        0        0    25140 2024-05-12 17:23:29.516976 oc_ds_converter-1.0.3/oc_ds_converter/run/jalc_process.py
+-rw-r--r--   0        0        0    26521 2024-05-12 17:23:29.516976 oc_ds_converter-1.0.3/oc_ds_converter/run/openaire_process.py
+-rw-r--r--   0        0        0     9887 2024-05-12 17:23:29.516976 oc_ds_converter-1.0.3/oc_ds_converter/run/pubmed_process.py
+-rw-r--r--   0        0        0    33527 2024-05-12 17:23:29.516976 oc_ds_converter-1.0.3/oc_ds_converter/run/pubmed_process_new.py
+-rw-r--r--   0        0        0     1086 2024-05-12 17:37:18.275967 oc_ds_converter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    23044 2024-05-12 17:23:29.501975 oc_ds_converter-1.0.3/README.md
+-rw-r--r--   0        0        0    24330 1970-01-01 00:00:00.000000 oc_ds_converter-1.0.3/PKG-INFO
```

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/crossref/crossref_processing.py` & `oc_ds_converter-1.0.3/oc_ds_converter/crossref/crossref_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/crossref/extract_crossref_publishers.py` & `oc_ds_converter-1.0.3/oc_ds_converter/crossref/extract_crossref_publishers.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/crossref/get_not_crossref_ref.py` & `oc_ds_converter-1.0.3/oc_ds_converter/crossref/get_not_crossref_ref.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/datacite/datacite_processing.py` & `oc_ds_converter-1.0.3/oc_ds_converter/datacite/datacite_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/datasource/datasource.py` & `oc_ds_converter-1.0.3/oc_ds_converter/datasource/datasource.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/datasource/redis.py` & `oc_ds_converter-1.0.3/oc_ds_converter/datasource/redis.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/jalc/jalc_processing.py` & `oc_ds_converter-1.0.3/oc_ds_converter/jalc/jalc_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/lib/__init__.py` & `oc_ds_converter-1.0.3/oc_ds_converter/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/lib/cleaner.py` & `oc_ds_converter-1.0.3/oc_ds_converter/lib/cleaner.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/lib/csvmanager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/lib/csvmanager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/lib/file_manager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/lib/file_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/lib/jsonmanager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/lib/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/lib/master_of_regex.py` & `oc_ds_converter-1.0.3/oc_ds_converter/lib/master_of_regex.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/medra/medra_processing.py` & `oc_ds_converter-1.0.3/oc_ds_converter/medra/medra_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/metadata_manager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/__init__.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/arxiv.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/arxiv.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/base.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/base.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/crossref.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/crossref.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/doi.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/doi.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/isbn.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/isbn.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/issn.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/issn.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/jid.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/jid.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/metadata_manager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/metadata_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/in_memory_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/redis_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/sqlite_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/oc_data_storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/openalex.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/openalex.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/orcid.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/orcid.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/pmcid.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/pmcid.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/pmid.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/pmid.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/ror.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/ror.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/support.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/support.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/url.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/url.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/viaf.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/viaf.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/wikidata.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/wikidata.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/oc_idmanager/wikipedia.py` & `oc_ds_converter-1.0.3/oc_ds_converter/oc_idmanager/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/openaire/openaire_processing.py` & `oc_ds_converter-1.0.3/oc_ds_converter/openaire/openaire_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/base.py` & `oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/datacite.py` & `oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/datacite.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/jalc.py` & `oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/jalc.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/preprocessing/nih.py` & `oc_ds_converter-1.0.3/oc_ds_converter/preprocessing/nih.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/pubmed/finder_nih.py` & `oc_ds_converter-1.0.3/oc_ds_converter/pubmed/finder_nih.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/pubmed/get_publishers.py` & `oc_ds_converter-1.0.3/oc_ds_converter/pubmed/get_publishers.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/pubmed/pubmed_dump_explorer.py` & `oc_ds_converter-1.0.3/oc_ds_converter/pubmed/pubmed_dump_explorer.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/pubmed/pubmed_processing.py` & `oc_ds_converter-1.0.3/oc_ds_converter/pubmed/pubmed_processing.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/pubmed/support_files/prefix_publishers.json` & `oc_ds_converter-1.0.3/oc_ds_converter/pubmed/support_files/prefix_publishers.json`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/ra_processor.py` & `oc_ds_converter-1.0.3/oc_ds_converter/ra_processor.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/run/crossref_process.py` & `oc_ds_converter-1.0.3/oc_ds_converter/run/crossref_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/run/datacite_process.py` & `oc_ds_converter-1.0.3/oc_ds_converter/run/datacite_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/run/jalc_process.py` & `oc_ds_converter-1.0.3/oc_ds_converter/run/jalc_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/run/openaire_process.py` & `oc_ds_converter-1.0.3/oc_ds_converter/run/openaire_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/run/pubmed_process.py` & `oc_ds_converter-1.0.3/oc_ds_converter/run/pubmed_process.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/oc_ds_converter/run/pubmed_process_new.py` & `oc_ds_converter-1.0.3/oc_ds_converter/run/pubmed_process_new.py`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/pyproject.toml` & `oc_ds_converter-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oc-ds-converter"
-version = "1.0.2"
+version = "1.0.3"
 description = "A library for converting metadata provided by various data sources, e.g. Crossref, DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta."
 authors = ["arcangelo7 <arcangelomas@gmail.com>"]
 license = "ISC"
 readme = "README.md"
 packages = [{include = "oc_ds_converter"}]
 
 [tool.poetry.dependencies]
```

### Comparing `oc_ds_converter-1.0.2/README.md` & `oc_ds_converter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oc_ds_converter-1.0.2/PKG-INFO` & `oc_ds_converter-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: oc-ds-converter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library for converting metadata provided by various data sources, e.g. Crossref, DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta.
 License: ISC
 Author: arcangelo7
 Author-email: arcangelomas@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
 Requires-Dist: fakeredis (>=2.14.0,<3.0.0)
 Requires-Dist: filelock (>=3.12.2,<4.0.0)
 Requires-Dist: lxml (>=4.9.2,<6.0.0)
 Requires-Dist: ndjson (>=0.3.1,<0.4.0)
 Requires-Dist: packaging (>=23.1,<24.0)
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: oc-ds-converter Version: 1.0.2 Summary: A library
+Metadata-Version: 2.1 Name: oc-ds-converter Version: 1.0.3 Summary: A library
 for converting metadata provided by various data sources, e.g. Crossref,
 DataCite, JaLC, and mEDRA, into the format used by OpenCitations Meta. License:
 ISC Author: arcangelo7 Author-email: arcangelomas@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0)
-Requires-Dist: fakeredis (>=2.14.0,<3.0.0) Requires-Dist: filelock
-(>=3.12.2,<4.0.0) Requires-Dist: lxml (>=4.9.2,<6.0.0) Requires-Dist: ndjson
-(>=0.3.1,<0.4.0) Requires-Dist: packaging (>=23.1,<24.0) Requires-Dist: pandas
-(>=2.0.1,<3.0.0) Requires-Dist: pebble (>=5.0.3,<6.0.0) Requires-Dist: poetry
-(>=1.5.1,<2.0.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-Dist:
-redis (>=4.5.5,<5.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
-self (>=2020.12.3,<2021.0.0) Requires-Dist: six (>=1.16.0,<2.0.0) Requires-
-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: update (>=0.0.1,<0.0.2) Requires-
-Dist: validators (>=0.20.0,<0.21.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: beautifulsoup4 (>=4.12.1,<5.0.0) Requires-Dist: fakeredis
+(>=2.14.0,<3.0.0) Requires-Dist: filelock (>=3.12.2,<4.0.0) Requires-Dist: lxml
+(>=4.9.2,<6.0.0) Requires-Dist: ndjson (>=0.3.1,<0.4.0) Requires-Dist:
+packaging (>=23.1,<24.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist:
+pebble (>=5.0.3,<6.0.0) Requires-Dist: poetry (>=1.5.1,<2.0.0) Requires-Dist:
+python-dateutil (>=2.8.2,<3.0.0) Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: self
+(>=2020.12.3,<2021.0.0) Requires-Dist: six (>=1.16.0,<2.0.0) Requires-Dist:
+tqdm (>=4.65.0,<5.0.0) Requires-Dist: update (>=0.0.1,<0.0.2) Requires-Dist:
+validators (>=0.20.0,<0.21.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Requires-Dist: zstandard (>=0.21.0,<0.22.0) Description-Content-Type: text/
 markdown [[https://img.shields.io/badge/powered%20by-OpenCitations-
 %239931FC?labelColor=2D22DE]](http://opencitations.net) [![Run tests](https://
 github.com/opencitations/ra_processor/actions/workflows/run_tests.yml/
 badge.svg)](https://github.com/opencitations/oc_meta/actions/workflows/
 run_tests.yml) ![Coverage](https://raw.githubusercontent.com/opencitations/
 ra_processor/main/test/coverage/coverage.svg) ![GitHub code size in bytes]
```

