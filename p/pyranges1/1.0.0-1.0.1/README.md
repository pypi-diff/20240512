# Comparing `tmp/pyranges1-1.0.0.tar.gz` & `tmp/pyranges1-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyranges1-1.0.0.tar", last modified: Sun May  5 12:02:17 2024, max compression
+gzip compressed data, was "pyranges1-1.0.1.tar", last modified: Sun May 12 12:37:17 2024, max compression
```

## Comparing `pyranges1-1.0.0.tar` & `pyranges1-1.0.1.tar`

### file list

```diff
@@ -1,170 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.747028 pyranges1-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.711028 pyranges1-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.715028 pyranges1-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 12:02:12.000000 pyranges1-1.0.0/.github/workflows/all_checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-05 12:02:12.000000 pyranges1-1.0.0/.github/workflows/build_the_book.yml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-05 12:02:12.000000 pyranges1-1.0.0/.github/workflows/build_wheels_and_upload_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-05 12:02:12.000000 pyranges1-1.0.0/.github/workflows/hypothesis_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-05 12:02:12.000000 pyranges1-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 12:02:12.000000 pyranges1-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 12:02:12.000000 pyranges1-1.0.0/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-05 12:02:12.000000 pyranges1-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-05 12:02:17.747028 pyranges1-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-05 12:02:12.000000 pyranges1-1.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-05 12:02:12.000000 pyranges1-1.0.0/check_typing_linting_and_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-05 12:02:12.000000 pyranges1-1.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.719028 pyranges1-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/extension_orfs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/extension_seqs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/extension_stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_columns.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_create.rst
--rw-r--r--   0 runner    (1001) docker     (127)    33804 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_genomic_ops.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_pages.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_rows.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_sequences.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/how_to_write.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/pyranges_extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/pyranges_module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/pyranges_objects.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/range_frame.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/todos.rst
--rw-r--r--   0 runner    (1001) docker     (127)    46805 2024-05-05 12:02:12.000000 pyranges1-1.0.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.723028 pyranges1-1.0.0/pyranges/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.727028 pyranges1-1.0.0/pyranges/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/loci_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/multioverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/out.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/pyranges_groupby.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/pyranges_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   212529 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/pyranges_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/tostring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.731028 pyranges1-1.0.0/pyranges/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/aorta.bed
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/aorta2.bed
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/bigwig.bw
--rw-r--r--   0 runner    (1001) docker     (127)   309369 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/chipseq.bed
--rw-r--r--   0 runner    (1001) docker     (127)   309045 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/chipseq_background.bed
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/chromsizes.bed
--rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/cpg.bed
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/ensembl.gtf
--rw-r--r--   0 runner    (1001) docker     (127)    35943 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/ensembl_human.gtf.gz
--rw-r--r--   0 runner    (1001) docker     (127)    64417 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/exons.bed
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/f1.bed
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/f2.bed
--rw-r--r--   0 runner    (1001) docker     (127)    81253 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/gencode_human.gtf.gz
--rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/lamina.bed
--rw-r--r--   0 runner    (1001) docker     (127)   387402 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/ncbi.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/ncbi.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/ncbi.gff.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/smaller.bam
--rw-r--r--   0 runner    (1001) docker     (127)    62555 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/data/ucsc_human.bed.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/docs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.731028 pyranges1-1.0.0/pyranges/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/ext/orfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/ext/seqs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/ext/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.735028 pyranges1-1.0.0/pyranges/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/boundaries.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/combine_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/itergrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/join.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/max_disjoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/merge_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/nearest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/spliced_subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/subtraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/tile_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/to_rle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/methods/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/orfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.735028 pyranges1-1.0.0/pyranges/range_frame/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/range_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/range_frame/range_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/range_frame/range_frame_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22547 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/seqs.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 12:02:12.000000 pyranges1-1.0.0/pyranges/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.743028 pyranges1-1.0.0/pyranges1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-05 12:02:17.000000 pyranges1-1.0.0/pyranges1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-05 12:02:17.000000 pyranges1-1.0.0/pyranges1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:02:17.000000 pyranges1-1.0.0/pyranges1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-05 12:02:17.000000 pyranges1-1.0.0/pyranges1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 12:02:17.000000 pyranges1-1.0.0/pyranges1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:02:17.747028 pyranges1-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-05 12:02:12.000000 pyranges1-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.739028 pyranges1-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/.fuse_hidden0000017200000002
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/hi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.739028 pyranges1-1.0.0/tests/property_based/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/property_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/property_based/hypothesis_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/property_based/new.py
--rw-r--r--   0 runner    (1001) docker     (127)    17767 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/property_based/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/property_based/test_do_not_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/property_based/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/run_doctest_tutorial_howto.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/test_calculate_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/test_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.739028 pyranges1-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/chip_10.bed
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/f1.bed
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/f2.bed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.739028 pyranges1-1.0.0/tests/unit/getitem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/getitem/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/hi
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/k_nearest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.739028 pyranges1-1.0.0/tests/unit/new_position/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/new_position/test_new_position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.743028 pyranges1-1.0.0/tests/unit/out/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/out/test_out.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.743028 pyranges1-1.0.0/tests/unit/spliced_subsequence/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/spliced_subsequence/test_spliced_subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_count_overlaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.743028 pyranges1-1.0.0/tests/unit/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_data/ensembl.gtf
--rw-r--r--   0 runner    (1001) docker     (127)    71593 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_data/test_sorted.bam
--rw-r--r--   0 runner    (1001) docker     (127)  1706448 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_data/test_sorted.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_guessers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_pandas_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/test_tostring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:17.743028 pyranges1-1.0.0/tests/unit/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:02:12.000000 pyranges1-1.0.0/tests/unit/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.480606 pyranges1-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.448606 pyranges1-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.452606 pyranges1-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-12 12:37:13.000000 pyranges1-1.0.1/.github/workflows/all_checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-12 12:37:13.000000 pyranges1-1.0.1/.github/workflows/build_the_book.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-12 12:37:13.000000 pyranges1-1.0.1/.github/workflows/build_wheels_and_upload_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-12 12:37:13.000000 pyranges1-1.0.1/.github/workflows/hypothesis_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-12 12:37:13.000000 pyranges1-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-12 12:37:13.000000 pyranges1-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-12 12:37:13.000000 pyranges1-1.0.1/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-12 12:37:13.000000 pyranges1-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-12 12:37:17.480606 pyranges1-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-12 12:37:13.000000 pyranges1-1.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-12 12:37:13.000000 pyranges1-1.0.1/check_typing_linting_and_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-12 12:37:13.000000 pyranges1-1.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.456606 pyranges1-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.456606 pyranges1-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.456606 pyranges1-1.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/_templates/custom_method_summary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13243 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/extension_orfs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/extension_seqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/extension_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_columns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33804 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_genomic_ops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    47854 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_overlap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_pages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_rows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_sequences.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/how_to_write.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/migration_cheatsheet.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/migration_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/pyranges_extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/pyranges_module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/pyranges_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/range_frame.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/todos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46805 2024-05-12 12:37:13.000000 pyranges1-1.0.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.460606 pyranges1-1.0.1/pyranges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.460606 pyranges1-1.0.1/pyranges/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/loci_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/multioverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/pyranges_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/pyranges_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225407 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/pyranges_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/tostring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.464606 pyranges1-1.0.1/pyranges/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/aorta.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/aorta2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/bigwig.bw
+-rw-r--r--   0 runner    (1001) docker     (127)   309369 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/chipseq.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   309045 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/chipseq_background.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/chromsizes.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/cpg.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    35943 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/ensembl_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    64417 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/exons.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/f2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    81253 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/gencode_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/lamina.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   387402 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/ncbi.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/ncbi.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/ncbi.gff.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/smaller.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    62555 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/data/ucsc_human.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/docs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.468606 pyranges1-1.0.1/pyranges/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/ext/orfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/ext/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/ext/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.468606 pyranges1-1.0.1/pyranges/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/combine_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/itergrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/max_disjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/merge_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/nearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/tile_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/to_rle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/methods/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/orfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.472606 pyranges1-1.0.1/pyranges/range_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/range_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/range_frame/range_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/range_frame/range_frame_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-12 12:37:13.000000 pyranges1-1.0.1/pyranges/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.480606 pyranges1-1.0.1/pyranges1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-12 12:37:17.000000 pyranges1-1.0.1/pyranges1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-12 12:37:17.000000 pyranges1-1.0.1/pyranges1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:37:17.000000 pyranges1-1.0.1/pyranges1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-12 12:37:17.000000 pyranges1-1.0.1/pyranges1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 12:37:17.000000 pyranges1-1.0.1/pyranges1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 12:37:17.480606 pyranges1-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-12 12:37:13.000000 pyranges1-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.472606 pyranges1-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/.fuse_hidden0000017200000002
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/hi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.472606 pyranges1-1.0.1/tests/property_based/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/property_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/property_based/hypothesis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/property_based/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17767 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/property_based/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/property_based/test_do_not_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/property_based/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/run_doctest_tutorial_howto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/test_calculate_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/test_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.476606 pyranges1-1.0.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/chip_10.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/f2.bed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.476606 pyranges1-1.0.1/tests/unit/getitem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/getitem/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/hi
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/k_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.476606 pyranges1-1.0.1/tests/unit/new_position/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/new_position/test_new_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.476606 pyranges1-1.0.1/tests/unit/out/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/out/test_out.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.476606 pyranges1-1.0.1/tests/unit/spliced_subsequence/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/spliced_subsequence/test_spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_count_overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.476606 pyranges1-1.0.1/tests/unit/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    71593 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_data/test_sorted.bam
+-rw-r--r--   0 runner    (1001) docker     (127)  1706448 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_data/test_sorted.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_guessers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_pandas_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/test_tostring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:17.480606 pyranges1-1.0.1/tests/unit/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 12:37:13.000000 pyranges1-1.0.1/tests/unit/unit/__init__.py
```

### Comparing `pyranges1-1.0.0/.github/workflows/all_checks.yml` & `pyranges1-1.0.1/.github/workflows/all_checks.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/.github/workflows/build_the_book.yml` & `pyranges1-1.0.1/.github/workflows/build_the_book.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/.github/workflows/build_wheels_and_upload_to_pypi.yml` & `pyranges1-1.0.1/.github/workflows/build_wheels_and_upload_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/.github/workflows/hypothesis_tests.yml` & `pyranges1-1.0.1/.github/workflows/hypothesis_tests.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/LICENSE` & `pyranges1-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/PKG-INFO` & `pyranges1-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 1.0.0
+Version: 1.0.1
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyranges1-1.0.0/README.md` & `pyranges1-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/check_typing_linting_and_formatting.py` & `pyranges1-1.0.1/check_typing_linting_and_formatting.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/conftest.py` & `pyranges1-1.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/Makefile` & `pyranges1-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/api_reference.rst` & `pyranges1-1.0.1/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/conf.py` & `pyranges1-1.0.1/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-import os
-import sys
+from docutils import nodes, utils
+
 # sys.path.insert(0, os.path.abspath('.'))
 
 # sys.path.insert(0, os.path.abspath('..'))  # Adjust this as necessary
 #
 # sys.path.insert(0, os.path.abspath('../pyranges'))  # Adjust this as necessary
 #
 # sys.path.insert(0, os.path.abspath('.'))  # Adjust this as necessary
 
 # -- Project information -----------------------------------------------------
 
 project = "pyranges"
-copyright = "2020, Endre Bakken Stovner"
-author = "Endre Bakken Stovner"
+copyright = "2024, Endre Bakken Stovner, Marco Mariotti"
+author = "Endre Bakken Stovner, Marco Mariotti"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -56,15 +56,15 @@
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = []
+exclude_patterns = ['_generated_hidden*']
 
 master_doc = "index"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
@@ -73,7 +73,25 @@
 html_theme = 'sphinx_rtd_theme'
 
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
+
+
+
+def monospaced_link(name, rawtext, text, lineno, inliner, options={}, content=[]):
+    url = text.split(' ')[-1].strip('<>')
+    clickable_text = ' '.join(text.split(' ')[:-1])
+    # Create a reference node, which is the docutils node for hyperlinks
+    unescaped_text = utils.unescape(text)
+
+    node = nodes.reference(rawtext, clickable_text, refuri=url, **options)
+
+    # Add a special class to this node
+    node['classes'].append('monospaced-link')
+    return [node], []
+
+def setup(app):
+    app.add_role('mslink', monospaced_link)
+    app.add_css_file('custom.css')
```

### Comparing `pyranges1-1.0.0/docs/developer_guide.rst` & `pyranges1-1.0.1/docs/developer_guide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 .. _task_sequence:
 
 Task sequence
 ~~~~~~~~~~~~~
 
 1. Create and download your own Pyranges fork
-------------------------------------------
+---------------------------------------------
 
 The easiest way to do this is through github. Login into the github website if you aren't already,
 then visit the Pyranges page on github, click "Fork" on the top right. 
 Fill the form and confirm. In the page of your new fork, find the
 **<> Code** button, and copy the https address. On your computer, create a new folder dedicated
 to the project, then clone your fork inside it:
 
@@ -291,15 +291,15 @@
 	git push
 
 You will be requested your github credentials. Note that your online password may not work; in this
 case, google how to set up a github token that you can use.
 
 
 10. Open a pull request
-----------------------
+-----------------------
 
 The easiest way to open a pull request is through the github website. Go to **your**
 Pyranges fork on github, then find the "Contribute" button (near the **<> Code** button). Click
 it, and select **Open pull request**.
 
 In the newly opened page, carefully check that source and destination are correctly selected. The
 Base repository should be pyranges/pyranges (i.e. the main pyranges repo), and the Head repository
@@ -311,15 +311,15 @@
 
 Github will run a "check" workflow which basically replicates the steps above. If all checks are ok, 
 Pyranges administrators will inspect the pull request, comment it if necessary, and potentially accept it.
 
 
 
 11. Core team only: upload to PyPI
----------------------------------
+----------------------------------
 
 Every now and then, the core development team considers that a new pyranges version should be
 released. To do so:
 
 - Update the version number in the pyproject.toml file
 - Find the "Build and upload to PyPI" workflow in the left menu of the github actions at `https://github.com/pyranges/pyranges_1.x/actions/ <https://github.com/pyranges/pyranges_1.x/actions/>`_
 - Click the "Run workflow" button on the right
@@ -343,9 +343,11 @@
 If you want to run tests in parallel, use the -n flag (only gives a speedup for the long-running
 property-based tests):
 
 .. code:: bash
 
     pytest -n 4 tests/property_based
 
+Other useful tools:
+
 * [rg](https://github.com/BurntSushi/ripgrep): ripgrep recursively searches directories for a regex pattern while respecting your gitignore
 * [fd](https://github.com/sharkdp/fd): A simple, fast and user-friendly alternative to 'find'
```

### Comparing `pyranges1-1.0.0/docs/how_to_columns.rst` & `pyranges1-1.0.1/docs/how_to_columns.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/how_to_create.rst` & `pyranges1-1.0.1/docs/how_to_create.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/how_to_genomic_ops.rst` & `pyranges1-1.0.1/docs/how_to_genomic_ops.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/how_to_inspect.rst` & `pyranges1-1.0.1/docs/how_to_inspect.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/how_to_rows.rst` & `pyranges1-1.0.1/docs/how_to_rows.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/how_to_sequences.rst` & `pyranges1-1.0.1/docs/how_to_sequences.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/how_to_write.rst` & `pyranges1-1.0.1/docs/how_to_write.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/index.rst` & `pyranges1-1.0.1/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 Pyranges is open source, and hosted at github: https://github.com/pyranges/pyranges_1.x/
 
 Pyranges is developed by Endre Bakken Stovner and by
 `Marco Mariotti's lab <https://www.mariottigenomicslab.com/>`_.
 
 **This documentation refers to the version 1 of pyranges**, which introduces a new API and a new data structure
-compared to version 0, still the 'default', soon to be deprecated. **Version 0** is available at
-https://github.com/pyranges/pyranges and https://pyranges.readthedocs.io/
+compared to version 0, still the 'default', soon to be deprecated. If you are a pyranges v0 user,
+check :doc:`this guide to migrate to v1 <./migration_guide>`.
 
 
 Citation
 ~~~~~~~~
 
 Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. *Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
 
@@ -30,14 +30,15 @@
 ~~~~~~~~~~~~~~~~~~~~~
 
 #. 🚀 :doc:`Installation instructions <./installation>`
 #. 🚀 :doc:`The tutorial <./tutorial>`,  recommended for all new users
 #. 🚀 :doc:`The how-to pages <./how_to_pages>`, further below, where functionalities are grouped by topic
 #. 🚀 :doc:`The API reference <./api_reference>`, where all methods are explained in detail
 #. 🚀 :doc:`The developer guide <./developer_guide>`, to follow in order to contribute to PyRanges
+#. 🚀 :doc:`The guide to migrate to v1 <./migration_guide>`, for existing users of pyranges v0
 
 
 
 .. toctree::
    :maxdepth: 1
    :hidden:
    :caption: Contents:
@@ -45,13 +46,12 @@
    installation
    tutorial
    how_to_pages
    api_reference
    developer_guide
 
 
-Indices and tables
-==================
+Indices
+=======
 
 * :ref:`genindex`
 * :ref:`modindex`
-* :ref:`search`
```

### Comparing `pyranges1-1.0.0/docs/installation.rst` & `pyranges1-1.0.1/docs/installation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     conda activate pr
 
 
 The preferred way to install pyranges is via pip::
 
     pip install pyranges1
 
-The command above will install a minimal version of pyranges.
+The command above will install a **minimal version** of pyranges.
 Pyranges has several optional dependencies, required for certain functionalities.
 
-To install all optional dependencies, use::
+To **install all optional dependencies**, use::
 
     pip install pyranges1[all]
 
 Here you can see the optional dependencies grouped by functionality::
 
     # user add-ons: to fetch sequences, read BAM files, parallelize execution ...
     pip install pyranges1[add-ons]
```

### Comparing `pyranges1-1.0.0/docs/make.bat` & `pyranges1-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/pyranges_module.rst` & `pyranges1-1.0.1/docs/pyranges_module.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/requirements.txt` & `pyranges1-1.0.1/docs/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 platformdirs==4.2.1
 pluggy==1.5.0
 pockets==0.9.1
 pyBigWig==0.3.22
 pyfaidx==0.8.1.1
 Pygments==2.17.2
 pyproject-api==1.6.1
-pyranges
 pyright==1.1.361
 pyrle
 pysam==0.22.1
 pytest==8.2.0
 pytest-watcher==0.4.2
 pytest-xdist==3.6.1
 python-dateutil==2.9.0.post0
```

### Comparing `pyranges1-1.0.0/docs/todos.rst` & `pyranges1-1.0.1/docs/todos.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/docs/tutorial.rst` & `pyranges1-1.0.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyproject.toml` & `pyranges1-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "cython", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyranges1"
-version = "1.0.0"
+version = "1.0.1"
 description = "GenomicRanges for Python."
 requires-python = ">=3.12.0"
 readme = "README.md"
 authors = [{ name = "Endre Bakken Stovner", email = "endbak@pm.me" }]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `pyranges1-1.0.0/pyranges/__init__.py` & `pyranges1-1.0.1/pyranges/__init__.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/empty.py` & `pyranges1-1.0.1/pyranges/core/empty.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/example_data.py` & `pyranges1-1.0.1/pyranges/core/example_data.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/loci_getter.py` & `pyranges1-1.0.1/pyranges/core/loci_getter.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/multioverlap.py` & `pyranges1-1.0.1/pyranges/core/multioverlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/names.py` & `pyranges1-1.0.1/pyranges/core/names.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 JOIN_INNER: Final = "inner"
 JOIN_RIGHT: Final = "right"
 JOIN_LEFT: Final = "left"
 VALID_JOIN_TYPE = Literal["inner", "left", "outer", "right"]
 VALID_JOIN_OPTIONS = [JOIN_INNER, JOIN_LEFT, JOIN_OUTER, JOIN_RIGHT]
 
 JOIN_SUFFIX = "_b"
-VALID_COMBINE_OPTIONS = Literal["intersect", "union"]
+VALID_COMBINE_OPTIONS = Literal["intersect", "union", "swap"]
 
 NEAREST_ANY_DIRECTION: Final = "any"
 NEAREST_UPSTREAM: Final = "upstream"
 NEAREST_DOWNSTREAM: Final = "downstream"
 VALID_NEAREST_TYPE = Literal["any", "upstream", "downstream"]
 VALID_NEAREST_OPTIONS = [
     NEAREST_ANY_DIRECTION,
```

### Comparing `pyranges1-1.0.0/pyranges/core/options.py` & `pyranges1-1.0.1/pyranges/core/options.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/out.py` & `pyranges1-1.0.1/pyranges/core/out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/parallelism.py` & `pyranges1-1.0.1/pyranges/core/parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/pyranges_groupby.py` & `pyranges1-1.0.1/pyranges/core/pyranges_groupby.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/pyranges_helpers.py` & `pyranges1-1.0.1/pyranges/core/pyranges_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     REVERSE_STRAND,
     STRAND_BEHAVIOR_AUTO,
     STRAND_BEHAVIOR_IGNORE,
     STRAND_BEHAVIOR_OPPOSITE,
     STRAND_BEHAVIOR_SAME,
     STRAND_COL,
     STRICT_STRAND_BEHAVIOR_TYPE,
-    TEMP_STRAND_COL,
     USE_STRAND_AUTO,
     VALID_BY_OPTIONS,
     VALID_STRAND_BEHAVIOR_OPTIONS,
     VALID_STRAND_BEHAVIOR_TYPE,
     VALID_USE_STRAND_OPTIONS,
     VALID_USE_STRAND_TYPE,
 )
@@ -115,25 +114,25 @@
 def group_keys_from_validated_strand_behavior(
     strand_behavior: VALID_STRAND_BEHAVIOR_TYPE,
     by: VALID_BY_OPTIONS = None,
 ) -> list[str]:
     """Return group keys based on strand behavior.
 
     If strand_behavior is 'same', return [CHROM_COL, STRAND_COL].
-    If strand_behavior is 'opposite', return [CHROM_COL, TEMP_STRAND_COL].
+    If strand_behavior is 'opposite', return [CHROM_COL, STRAND_COL].
     If strand_behavior is 'ignore', return [CHROM_COL].
 
     In each case, if a by argument is provided, it is appended/extended to the list of group keys.
 
     """
-    strand_cols = (
-        [STRAND_COL]
-        if strand_behavior == STRAND_BEHAVIOR_SAME
-        else ([TEMP_STRAND_COL] if strand_behavior == STRAND_BEHAVIOR_OPPOSITE else [])
-    )
+    if strand_behavior == STRAND_BEHAVIOR_AUTO:
+        msg = "this function must be called with a validated strand_behavior"
+        raise ValueError(msg)
+
+    strand_cols = [STRAND_COL] if strand_behavior in [STRAND_BEHAVIOR_SAME, STRAND_BEHAVIOR_OPPOSITE] else []
 
     return [CHROM_COL, *strand_cols, *arg_to_list(by)]
 
 
 def strand_behavior_from_validated_use_strand(
     df: "PyRanges",
     use_strand: VALID_USE_STRAND_TYPE,
```

### Comparing `pyranges1-1.0.0/pyranges/core/pyranges_main.py` & `pyranges1-1.0.1/pyranges/core/pyranges_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import sys
 from collections.abc import Callable, Iterable
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Optional, cast
 
+import numpy as np
 import pandas as pd
 from natsort import natsort, natsorted  # type: ignore[import]
 
 import pyranges as pr
 from pyranges.core.loci_getter import LociGetter
 from pyranges.core.names import (
     CHROM_AND_STRAND_COLS,
@@ -21,19 +22,22 @@
     JOIN_SUFFIX,
     NEAREST_DOWNSTREAM,
     NEAREST_UPSTREAM,
     OVERLAP_CONTAINMENT,
     OVERLAP_FIRST,
     PANDAS_COMPRESSION_TYPE,
     RANGE_COLS,
+    REVERSE_STRAND,
     SKIP_IF_EMPTY_LEFT,
     START_COL,
+    STRAND_BEHAVIOR_IGNORE,
     STRAND_BEHAVIOR_OPPOSITE,
     STRAND_COL,
     TEMP_END_SLACK_COL,
+    TEMP_ID_COL,
     TEMP_NAME_COL,
     TEMP_NUM_COL,
     TEMP_START_SLACK_COL,
     TEMP_STRAND_COL,
     USE_STRAND_DEFAULT,
     VALID_BY_TYPES,
     VALID_COMBINE_OPTIONS,
@@ -586,57 +590,78 @@
 
     def apply_pair(  # type: ignore[override]
         self: "PyRanges",
         other: "PyRanges",
         function: BinaryOperation,
         strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
         by: VALID_BY_TYPES = None,
+        *,
+        preserve_order: bool = False,
         **kwargs,
     ) -> "pr.PyRanges":
         """Apply function to pairs of overlapping intervals, by chromosome and optionally strand.
 
         Parameters
         ----------
         other : PyRanges
             Second PyRanges to apply function to.
 
         function : Callable
             Function that takes two PyRanges  and returns a PyRanges.
-            The function shouldb accept a **kwargs argument. It may be used to extract useful information:
+            The function should accept a **kwargs argument, which may be used to extract useful information:
             group = kwargs.get("__by__", {})
             # e.g. chromosome = group.get("Chromosome", None)
             # e.g. strand = group.get("Strand", "+")
 
         strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
             Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
             information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
             otherwise ignore the strand information.
 
         by : str or list of str or None
             Additional columns - in addition to chromosome and strand - to group by.
 
+        copy_self : bool, default False
+            Whether to copy the first PyRanges before operations. Use False if copied beforehand.
+
+        preserve_order : bool, default False
+            Preserve the order of the intervals in the first PyRanges in output.
+
         kwargs : dict
             Other arguments passed along to the function.
 
         """
         strand_behavior = validate_and_convert_strand_behavior(self, other, strand_behavior)
         by = arg_to_list(by)
 
         if strand_behavior == STRAND_BEHAVIOR_OPPOSITE:
-            self[TEMP_STRAND_COL] = self[STRAND_COL].replace({"+": "-", "-": "+"})
-            other[TEMP_STRAND_COL] = other[STRAND_COL]
+            # swap strands in STRAND_COL, but keep original values in TEMP_STRAND_COL
+            self = mypy_ensure_pyranges(
+                self.assign(**{TEMP_STRAND_COL: self[STRAND_COL]}).assign(
+                    **{
+                        STRAND_COL: self[STRAND_COL].replace(
+                            {FORWARD_STRAND: REVERSE_STRAND, REVERSE_STRAND: FORWARD_STRAND},
+                        ),
+                    },
+                ),
+            )
 
         grpby_ks = group_keys_from_validated_strand_behavior(strand_behavior, by=by)
 
         res = mypy_ensure_pyranges(super().apply_pair(other, function, by=grpby_ks, **kwargs))
 
         if strand_behavior == STRAND_BEHAVIOR_OPPOSITE:
-            res = res.drop_and_return(TEMP_STRAND_COL, axis="columns")
+            # swap back strands in STRAND_COL
+            res = res.drop_and_return(STRAND_COL, axis="columns").rename(columns={TEMP_STRAND_COL: STRAND_COL})
+
+        if preserve_order:
+            common_index = self.index.intersection(res.index)
+            res = res.reindex(common_index)
 
-        return res
+        return mypy_ensure_pyranges(res)
 
     def boundaries(
         self,
         transcript_id: str | list[str] | None = None,
         agg: dict[str, str | Callable] | None = None,
     ) -> "PyRanges":
         """Return the boundaries of groups of intervals (e.g. transcripts).
@@ -763,118 +788,152 @@
             Whether to cluster only intervals on the same strand.
             The default "auto" means True if PyRanges has valid strands (see .strand_valid).
 
         match_by : str or list, default None
             If provided, only intervals with an equal value in column(s) `match_by` may be considered as overlapping.
 
         slack : int, default 0
-            Consider intervals separated by less than `slack` to be in the same cluster. If `slack`
-            is negative, intervals overlapping less than `slack` are not considered to be in the
-            same cluster.
+            Length by which the criteria of overlap are loosened.
+            A value of 1 clusters also bookended intervals.
+            Higher slack values cluster more distant intervals (with a maximum distance of slack-1 between them).
 
         cluster_column:
             Name the cluster column added in output. Default: "Cluster"
 
         count_column:
             If a value is provided, add a column of counts with this name.
 
         Returns
         -------
         PyRanges
             PyRanges with an ID-column "Cluster" added.
 
-        Warning
-        -------
-
-        Bookended intervals (i.e. the End of a PyRanges interval is the Start of
-        another one) are by default considered to overlap.
-        Avoid this with slack=-1.
-
         See Also
         --------
         PyRanges.merge: combine overlapping intervals into one
 
         Examples
         --------
-        >>> gr = pr.PyRanges({"Chromosome": [1, 1, 2, 1, 1], "Start": [1, 2, 0, 3, 9],
-        ...                    "End": [3, 3, 4, 10, 12], "Gene": [1, 2, 6, 3, 3]})
+        >>> gr = pr.PyRanges(dict(Chromosome=1, Start=[5, 6, 12, 16, 20, 22, 24], End=[9, 8, 16, 18, 23, 25, 27]))
         >>> gr
-          index  |      Chromosome    Start      End     Gene
-          int64  |           int64    int64    int64    int64
-        -------  ---  ------------  -------  -------  -------
-              0  |               1        1        3        1
-              1  |               1        2        3        2
-              2  |               2        0        4        6
-              3  |               1        3       10        3
-              4  |               1        9       12        3
-        PyRanges with 5 rows, 4 columns, and 1 index columns.
-        Contains 2 chromosomes.
+          index  |      Chromosome    Start      End
+          int64  |           int64    int64    int64
+        -------  ---  ------------  -------  -------
+              0  |               1        5        9
+              1  |               1        6        8
+              2  |               1       12       16
+              3  |               1       16       18
+              4  |               1       20       23
+              5  |               1       22       25
+              6  |               1       24       27
+        PyRanges with 7 rows, 3 columns, and 1 index columns.
+        Contains 1 chromosomes.
 
-        >>> gr.cluster(cluster_column="ClusterId").sort_ranges()
-          index  |      Chromosome    Start      End     Gene    ClusterId
-          int64  |           int64    int64    int64    int64        int64
-        -------  ---  ------------  -------  -------  -------  -----------
-              0  |               1        1        3        1            0
-              1  |               1        2        3        2            0
-              3  |               1        3       10        3            0
-              4  |               1        9       12        3            0
-              2  |               2        0        4        6            1
-        PyRanges with 5 rows, 5 columns, and 1 index columns.
-        Contains 2 chromosomes.
+        >>> gr.cluster()
+          index  |      Chromosome    Start      End    Cluster
+          int64  |           int64    int64    int64      int64
+        -------  ---  ------------  -------  -------  ---------
+              0  |               1        5        9          0
+              1  |               1        6        8          0
+              2  |               1       12       16          1
+              3  |               1       16       18          2
+              4  |               1       20       23          3
+              5  |               1       22       25          3
+              6  |               1       24       27          3
+        PyRanges with 7 rows, 4 columns, and 1 index columns.
+        Contains 1 chromosomes.
 
-        >>> gr.cluster(match_by=["Gene"], count_column="Counts")
-          index  |      Chromosome    Start      End     Gene    Cluster    Counts
-          int64  |           int64    int64    int64    int64      int64     int64
-        -------  ---  ------------  -------  -------  -------  ---------  --------
-              0  |               1        1        3        1          0         1
-              1  |               1        2        3        2          1         1
-              2  |               2        0        4        6          2         1
-              3  |               1        3       10        3          3         2
-              4  |               1        9       12        3          3         2
-        PyRanges with 5 rows, 6 columns, and 1 index columns.
-        Contains 2 chromosomes.
+        Slack=1 will cluster also bookended intervals:
+
+        >>> gr.cluster(slack=1)
+          index  |      Chromosome    Start      End    Cluster
+          int64  |           int64    int64    int64      int64
+        -------  ---  ------------  -------  -------  ---------
+              0  |               1        5        9          0
+              1  |               1        6        8          0
+              2  |               1       12       16          1
+              3  |               1       16       18          1
+              4  |               1       20       23          2
+              5  |               1       22       25          2
+              6  |               1       24       27          2
+        PyRanges with 7 rows, 4 columns, and 1 index columns.
+        Contains 1 chromosomes.
+
+        Higher values of slack will cluster more distant intervals:
+
+        >>> gr.cluster(slack=3)
+          index  |      Chromosome    Start      End    Cluster
+          int64  |           int64    int64    int64      int64
+        -------  ---  ------------  -------  -------  ---------
+              0  |               1        5        9          0
+              1  |               1        6        8          0
+              2  |               1       12       16          1
+              3  |               1       16       18          1
+              4  |               1       20       23          1
+              5  |               1       22       25          1
+              6  |               1       24       27          1
+        PyRanges with 7 rows, 4 columns, and 1 index columns.
+        Contains 1 chromosomes.
+
+        >>> gr.cluster(slack=3, count_column="Count")
+          index  |      Chromosome    Start      End    Cluster    Count
+          int64  |           int64    int64    int64      int64    int64
+        -------  ---  ------------  -------  -------  ---------  -------
+              0  |               1        5        9          0        2
+              1  |               1        6        8          0        2
+              2  |               1       12       16          1        5
+              3  |               1       16       18          1        5
+              4  |               1       20       23          1        5
+              5  |               1       22       25          1        5
+              6  |               1       24       27          1        5
+        PyRanges with 7 rows, 5 columns, and 1 index columns.
+        Contains 1 chromosomes.
 
         """
         from pyranges.methods.cluster import _cluster
 
         if not len(self):
             # returning empty PyRanges with consistent columns
-            cols_to_add = {cluster_column: None}
+            cols_to_add = {cluster_column: 0}
             if count_column:
-                cols_to_add[count_column] = None
+                cols_to_add[count_column] = 0
             return mypy_ensure_pyranges(self.copy().assign(**cols_to_add))
 
-        strand = validate_and_convert_use_strand(self, use_strand=use_strand)
         _self = mypy_ensure_pyranges(self.sort_values(START_COL))
 
-        _by = [match_by] if isinstance(match_by, str) else ([*match_by] if match_by is not None else [])
+        use_strand = validate_and_convert_use_strand(_self, use_strand)
+
         gr = _self.apply_single(
             _cluster,
             by=match_by,
-            use_strand=strand,
+            use_strand=use_strand,
             slack=slack,
             count_column=count_column,
             cluster_column=cluster_column,
             preserve_index=True,
         )
 
+        by_split_groups = (
+            (CHROM_AND_STRAND_COLS if use_strand else [CHROM_COL]) + arg_to_list(match_by) + [cluster_column]
+        )
         gr = gr.reindex(self.index)
-        gr[cluster_column] = gr.groupby(self.loc_columns + _by + [cluster_column], sort=False).ngroup()
+        gr[cluster_column] = gr.groupby(by_split_groups, sort=False).ngroup()
         return mypy_ensure_pyranges(gr)
 
     def copy(self, *args, **kwargs) -> "pr.PyRanges":
         """Return a copy of the PyRanges."""
         return mypy_ensure_pyranges(super().copy(*args, **kwargs))
 
     def count_overlaps(
         self,
         other: "PyRanges",
         strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
         *,
         match_by: str | list[str] | None = None,
+        slack: int = 0,
         overlap_col: str = "NumberOverlaps",
         keep_nonoverlapping: bool = True,
         calculate_coverage: bool = False,
         coverage_col: str = "CoverageOverlaps",
     ) -> "PyRanges":
         """Count number of overlaps per interval.
 
@@ -889,14 +948,17 @@
             If provided, only intervals with an equal value in column(s) `match_by` may be considered as overlapping.
 
         strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
             Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
             information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
             otherwise ignore the strand information.
 
+        slack : int, default 0
+            Temporarily lengthen intervals in self before searching for overlaps.
+
         keep_nonoverlapping : bool, default True
             Keep intervals without overlaps.
 
         overlap_col : str, default "NumberOverlaps"
             Name of column with overlap counts.
 
         calculate_coverage : bool, default False
@@ -938,29 +1000,39 @@
         Contains 1 chromosomes and 2 strands.
 
         >>> f1.count_overlaps(f2, overlap_col="Count")
           index  |    Chromosome      Start      End  Strand        Count
           int64  |    category        int64    int64  category      int64
         -------  ---  ------------  -------  -------  ----------  -------
               0  |    chr1                3        6  +                 0
-              2  |    chr1                8        9  +                 0
               1  |    chr1                5        7  -                 1
+              2  |    chr1                8        9  +                 0
         PyRanges with 3 rows, 5 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
-        >>> f1.count_overlaps(f2, overlap_col="C", calculate_coverage=True, coverage_col="F")
-          index  |    Chromosome      Start      End  Strand              F
-          int64  |    category        int64    int64  category      float64
-        -------  ---  ------------  -------  -------  ----------  ---------
-              0  |    chr1                3        6  +                 0
+        >>> f1.count_overlaps(f2, overlap_col="Count", slack=1, strand_behavior="ignore")
+          index  |    Chromosome      Start      End  Strand        Count
+          int64  |    category        int64    int64  category      int64
+        -------  ---  ------------  -------  -------  ----------  -------
+              0  |    chr1                3        6  +                 1
+              1  |    chr1                5        7  -                 1
               2  |    chr1                8        9  +                 0
-              1  |    chr1                5        7  -                 0.5
         PyRanges with 3 rows, 5 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
+        >>> f1.count_overlaps(f2, overlap_col="C", calculate_coverage=True, coverage_col="F")
+          index  |    Chromosome      Start      End  Strand            C          F
+          int64  |    category        int64    int64  category      int64    float64
+        -------  ---  ------------  -------  -------  ----------  -------  ---------
+              0  |    chr1                3        6  +                 0        0
+              1  |    chr1                5        7  -                 1        0.5
+              2  |    chr1                8        9  +                 0        0
+        PyRanges with 3 rows, 6 columns, and 1 index columns.
+        Contains 1 chromosomes and 2 strands.
+
         >>> annotation = pr.example_data.ensembl_gtf.get_with_loc_columns(['transcript_id', 'Feature'])
         >>> reads = pr.random(1000, chromsizes={'1':150000}, strand=False, seed=123)
         >>> annotation.count_overlaps(reads)
         index    |    Chromosome    Start    End      Strand      transcript_id    Feature     NumberOverlaps
         int64    |    category      int64    int64    category    object           category    int64
         -------  ---  ------------  -------  -------  ----------  ---------------  ----------  ----------------
         0        |    1             11868    14409    +           nan              gene        20
@@ -976,18 +1048,31 @@
         Contains 1 chromosomes and 2 strands.
 
         """
         from pyranges.methods.coverage import _number_overlapping
 
         strand_behavior = validate_and_convert_strand_behavior(self, other, strand_behavior)
         if coverage_col != "CoverageOverlaps" and not calculate_coverage:
-            msg = "coverage_col can only be provided if calculate_coverage is True."
+            msg = "coverage_col can only be provided with calculate_coverage=True."
             raise ValueError(msg)
 
-        result = self.apply_pair(
+        if slack and calculate_coverage:
+            msg = "calculate_coverage can only be computed with slack=0."
+            raise ValueError(msg)
+
+        if slack:
+            _self = self.copy()
+            _self[TEMP_START_SLACK_COL] = _self.Start
+            _self[TEMP_END_SLACK_COL] = _self.End
+
+            _self = _self.extend(slack, use_strand=False)
+        else:
+            _self = self
+
+        result = _self.apply_pair(
             other,
             _number_overlapping,
             strand_behavior=strand_behavior,
             by=match_by,
             keep_nonoverlapping=keep_nonoverlapping,
             overlap_col=overlap_col,
             skip_if_empty=not keep_nonoverlapping,
@@ -995,25 +1080,31 @@
 
         if calculate_coverage:
             from pyranges.methods.coverage import _coverage
 
             use_strand = use_strand_from_validated_strand_behavior(self, other, strand_behavior)
             other = other.merge_overlaps(use_strand=use_strand, match_by=match_by, count_col="Count")
 
-            result = self.copy().apply_pair(
+            result = result.apply_pair(
                 other,
                 _coverage,
                 strand_behavior=strand_behavior,
                 by=match_by,
                 fraction_col=coverage_col,
                 keep_nonoverlapping=keep_nonoverlapping,
                 overlap_col=overlap_col,
                 skip_if_empty=not keep_nonoverlapping,
             )
-        return result
+        if slack and len(result) > 0:
+            result[START_COL] = result[TEMP_START_SLACK_COL]
+            result[END_COL] = result[TEMP_END_SLACK_COL]
+            result = result.drop_and_return([TEMP_START_SLACK_COL, TEMP_END_SLACK_COL], axis=1)
+
+        # reindex to original order
+        return mypy_ensure_pyranges(result.reindex(self.index))
 
     # to do: optimize, doesn't need to split by chromosome, only strand and only if ext_3/5
     def extend(
         self,
         ext: int | None = None,
         ext_3: int | None = None,
         ext_5: int | None = None,
@@ -1266,36 +1357,32 @@
         match_by : str or list, default None
             If provided, only intervals with an equal value in column(s) `match_by` may be joined.
 
         report_overlap : bool, default False
             Report amount of overlap in base pairs.
 
         slack : int, default 0
-            Lengthen intervals in self before joining.
+            Before joining, temporarily extend intervals in self by this much on both ends.
 
         suffix : str or tuple, default "_b"
             Suffix to give overlapping columns in other.
 
-        apply_strand_suffix : bool, default None
-            If first pyranges is unstranded, but the second is not, the first will be given a strand column.
-            apply_strand_suffix makes the added strand column a regular data column instead by adding a suffix.
 
         Returns
         -------
         PyRanges
 
             A PyRanges appended with columns of another.
 
         Note
         ----
-        The chromosome from other will never be reported as it is always the same as in self.
+        The indices of the two input PyRanges are not preserved in output.
+        The chromosome column from other will never be reported as it is always the same as in self.
+        Whether the strand column from other is reported depends on the strand_behavior.
 
-        As pandas did not have NaN for non-float datatypes until recently, "left" and "right" join
-        give non-overlapping rows the value -1 to avoid promoting columns to object. This will
-        change to NaN in a future version as general NaN becomes stable in pandas.
 
         See Also
         --------
         PyRanges.combine_interval_columns : give joined PyRanges new coordinates
 
         Examples
         --------
@@ -1322,42 +1409,42 @@
         PyRanges with 2 rows, 4 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         >>> f1.join_ranges(f2)
           index  |    Chromosome      Start      End  Name         Start_b    End_b  Name_b
           int64  |    object          int64    int64  object         int64    int64  object
         -------  ---  ------------  -------  -------  ---------  ---------  -------  --------
-              2  |    chr1                5        7  interval2          6        7  b
+              0  |    chr1                5        7  interval2          6        7  b
         PyRanges with 1 rows, 7 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         Note that since some start and end columns are nan, a regular DataFrame is returned.
 
         >>> f1.join_ranges(f2, join_type="left")
           index  |    Chromosome      Start      End  Name         Start_b      End_b  Name_b
           int64  |    object          int64    int64  object       float64    float64  object
         -------  ---  ------------  -------  -------  ---------  ---------  ---------  --------
-              2  |    chr1                5        7  interval2          6          7  b
               0  |    chr1                3        6  interval1        nan        nan  nan
               1  |    chr1                8        9  interval3        nan        nan  nan
+              2  |    chr1                5        7  interval2          6          7  b
         PyRanges with 3 rows, 7 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         >>> f1.join_ranges(f2, join_type="outer")
           index  |    Chromosome        Start        End  Name         Start_b      End_b  Name_b
           int64  |    object          float64    float64  object       float64    float64  object
         -------  ---  ------------  ---------  ---------  ---------  ---------  ---------  --------
-              1  |    chr1                  5          7  interval2          6          7  b
               0  |    chr1                  3          6  interval1        nan        nan  nan
               1  |    chr1                  8          9  interval3        nan        nan  nan
-              0  |    nan                 nan        nan  nan                1          2  a
-        PyRanges with 4 rows, 7 columns, and 1 index columns (with 2 index duplicates).
+              2  |    chr1                  5          7  interval2          6          7  b
+              3  |    nan                 nan        nan  nan                1          2  a
+        PyRanges with 4 rows, 7 columns, and 1 index columns.
         Contains 1 chromosomes.
         Invalid ranges:
-          * 1 starts or ends are nan. See indexes: 0
+          * 1 starts or ends are nan. See indexes: 3
 
 
         >>> gr = pr.PyRanges({"Chromosome": ["chr1", "chr2", "chr1", "chr3"], "Start": [1, 4, 10, 0],
         ...                   "End": [3, 9, 11, 1], "ID": ["a", "b", "c", "d"]})
         >>> gr
           index  |    Chromosome      Start      End  ID
           int64  |    object          int64    int64  object
@@ -1382,17 +1469,17 @@
         Contains 1 chromosomes.
 
         >>> gr.join_ranges(gr2)
           index  |    Chromosome      Start      End  ID          Start_b    End_b  ID_b
           int64  |    object          int64    int64  object        int64    int64  object
         -------  ---  ------------  -------  -------  --------  ---------  -------  --------
               0  |    chr1                1        3  a                 1       10  c
-              0  |    chr1                1        3  a                 2        9  b
-              0  |    chr1                1        3  a                 2        3  a
-        PyRanges with 3 rows, 7 columns, and 1 index columns (with 2 index duplicates).
+              1  |    chr1                1        3  a                 2        9  b
+              2  |    chr1                1        3  a                 2        3  a
+        PyRanges with 3 rows, 7 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         >>> gr.join_ranges(gr2, match_by="ID")
           index  |    Chromosome      Start      End  ID          Start_b    End_b
           int64  |    object          int64    int64  object        int64    int64
         -------  ---  ------------  -------  -------  --------  ---------  -------
               0  |    chr1                1        3  a                 2        3
@@ -1400,107 +1487,111 @@
         Contains 1 chromosomes.
 
         >>> bad = f1.join_ranges(f2, join_type="right")
         >>> bad
           index  |    Chromosome        Start        End  Name         Start_b    End_b  Name_b
           int64  |    object          float64    float64  object         int64    int64  object
         -------  ---  ------------  ---------  ---------  ---------  ---------  -------  --------
-              1  |    chr1                  5          7  interval2          6        7  b
-              0  |    nan                 nan        nan  nan                1        2  a
+              0  |    chr1                  5          7  interval2          6        7  b
+              1  |    nan                 nan        nan  nan                1        2  a
         PyRanges with 2 rows, 7 columns, and 1 index columns.
         Contains 1 chromosomes.
         Invalid ranges:
-          * 1 starts or ends are nan. See indexes: 0
+          * 1 starts or ends are nan. See indexes: 1
 
         >>> f2.join_ranges(bad)  # bad.join_ranges(f2) would not work either.
         Traceback (most recent call last):
         ...
         ValueError: Cannot perform function on invalid ranges (function was _both_dfs).
 
         With slack 1, bookended features are joined (see row 1):
 
         >>> f1.join_ranges(f2, slack=1)
           index  |    Chromosome      Start      End  Name         Start_b    End_b  Name_b
           int64  |    object          int64    int64  object         int64    int64  object
         -------  ---  ------------  -------  -------  ---------  ---------  -------  --------
               0  |    chr1                3        6  interval1          6        7  b
-              2  |    chr1                5        7  interval2          6        7  b
+              1  |    chr1                5        7  interval2          6        7  b
         PyRanges with 2 rows, 7 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         >>> f1.join_ranges(f2, report_overlap=True)
           index  |    Chromosome      Start      End  Name         Start_b    End_b  Name_b      Overlap
           int64  |    object          int64    int64  object         int64    int64  object        int64
         -------  ---  ------------  -------  -------  ---------  ---------  -------  --------  ---------
-              2  |    chr1                5        7  interval2          6        7  b                 1
+              0  |    chr1                5        7  interval2          6        7  b                 1
         PyRanges with 1 rows, 8 columns, and 1 index columns.
         Contains 1 chromosomes.
 
 
         >>> f1.join_ranges(f2, report_overlap=True)
           index  |    Chromosome      Start      End  Name         Start_b    End_b  Name_b      Overlap
           int64  |    object          int64    int64  object         int64    int64  object        int64
         -------  ---  ------------  -------  -------  ---------  ---------  -------  --------  ---------
-              2  |    chr1                5        7  interval2          6        7  b                 1
+              0  |    chr1                5        7  interval2          6        7  b                 1
         PyRanges with 1 rows, 8 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         Allowing slack in overlaps may result in 0 or negative Overlap values:
 
         >>> f1.join_ranges(f2, report_overlap=True, slack=2)
           index  |    Chromosome      Start      End  Name         Start_b    End_b  Name_b      Overlap
           int64  |    object          int64    int64  object         int64    int64  object        int64
         -------  ---  ------------  -------  -------  ---------  ---------  -------  --------  ---------
               0  |    chr1                3        6  interval1          1        2  a                -1
-              0  |    chr1                3        6  interval1          6        7  b                 0
-              1  |    chr1                8        9  interval3          6        7  b                -1
-              2  |    chr1                5        7  interval2          6        7  b                 1
-        PyRanges with 4 rows, 8 columns, and 1 index columns (with 1 index duplicates).
+              1  |    chr1                3        6  interval1          6        7  b                 0
+              2  |    chr1                8        9  interval3          6        7  b                -1
+              3  |    chr1                5        7  interval2          6        7  b                 1
+        PyRanges with 4 rows, 8 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         """
         from pyranges.methods.join import _both_dfs
 
         _self = self.copy()
         if slack:
             _self[TEMP_START_SLACK_COL] = _self.Start
             _self[TEMP_END_SLACK_COL] = _self.End
+            _self = _self.extend(slack, use_strand=False)
+        _self[TEMP_ID_COL] = np.arange(len(_self))
 
-            _self = _self.extend(slack)
-
-        gr: pd.DataFrame | PyRanges = _self.apply_pair(
+        gr: PyRanges = _self.apply_pair(
             other,
             _both_dfs,
             strand_behavior=strand_behavior,
             by=match_by,
             join_type=join_type,
             report_overlap=report_overlap,
             suffix=suffix,
         )
 
         # even if empty, make sure the object returned has consistent columns
         if gr.empty:
             use_strand = use_strand_from_validated_strand_behavior(self, other, strand_behavior)
-            empty_with_cols = self.head(0).merge(
-                other.head(0),
-                how="inner",
-                suffixes=("", suffix),
-                on=(([CHROM_COL, STRAND_COL] if use_strand else [CHROM_COL]) + arg_to_list(match_by)),
+            gr = mypy_ensure_pyranges(
+                self.head(0).merge(
+                    other.head(0),
+                    how="inner",
+                    suffixes=("", suffix),
+                    on=(([CHROM_COL, STRAND_COL] if use_strand else [CHROM_COL]) + arg_to_list(match_by)),
+                ),
             )
-            return mypy_ensure_pyranges(empty_with_cols)
 
         if slack and len(gr) > 0:
             gr[START_COL] = gr[TEMP_START_SLACK_COL]
             gr[END_COL] = gr[TEMP_END_SLACK_COL]
             gr = gr.drop_and_return([TEMP_START_SLACK_COL, TEMP_END_SLACK_COL], axis=1)
 
         if report_overlap:
             gr["Overlap"] = gr[["End", "End" + suffix]].min(axis=1) - gr[["Start", "Start" + suffix]].max(axis=1)
 
-        return gr
+        # preserving order. I can't use the reindex syntax as in other functions because of potential duplicates
+        gr = mypy_ensure_pyranges(gr.sort_values(TEMP_ID_COL).reset_index(drop=True))
+
+        return gr.drop_and_return(TEMP_ID_COL, axis=1)
 
     @property
     def length(self) -> int:
         """Return the total length of the intervals.
 
         See Also
         --------
@@ -1591,29 +1682,31 @@
         Parameters
         ----------
         use_strand: {"auto", True, False}, default: "auto"
             Find the max disjoint set separately for each strand.
             The default "auto" means True if PyRanges has valid strands (see .strand_valid).
 
         slack : int, default 0
-            Consider intervals within a distance of slack to be overlapping.
+            Length by which the criteria of overlap are loosened.
+            A value of 1 implies that bookended intervals are considered overlapping.
+            Higher slack values allow more distant intervals (with a maximum distance of slack-1 between them).
 
         match_by : str or list, default None
             If provided, only intervals with an equal value in column(s) `match_by` may be considered as overlapping.
 
         Returns
         -------
         PyRanges
-
             PyRanges with maximal disjoint set of intervals.
 
         See Also
         --------
         PyRanges.merge_overlaps : merge intervals into non-overlapping superintervals
         PyRanges.split : split intervals into non-overlapping subintervals
+        PyRanges.cluster : annotate overlapping intervals with common ID
 
         Examples
         --------
         >>> gr = pr.example_data.f1
         >>> gr
           index  |    Chromosome      Start      End  Name         Score  Strand
           int64  |    category        int64    int64  object       int64  category
@@ -1651,14 +1744,17 @@
         *,
         count_col: str | None = None,
         match_by: VALID_BY_TYPES = None,
         slack: int = 0,
     ) -> "PyRanges":
         """Merge overlapping intervals into one.
 
+        Returns a PyRanges with superintervals that are the union of overlapping intervals.
+        Bookended intervals are merged by default.
+
         Parameters
         ----------
         use_strand: {"auto", True, False}, default: "auto"
             Only merge intervals on same strand.
             The default "auto" means True if PyRanges has valid strands (see .strand_valid).
 
         count : bool, default False
@@ -1672,25 +1768,26 @@
 
         slack : int, default 0
             Allow this many nucleotides between each interval to merge.
 
         Returns
         -------
         PyRanges
-
-            PyRanges with superintervals.
+            PyRanges with superintervals. Metadata columns, index, and order are not preserved.
 
         Note
         ----
         To avoid losing metadata, use cluster instead. If you want to perform a reduction function
         on the metadata, use pandas groupby.
 
         See Also
         --------
         PyRanges.cluster : annotate overlapping intervals with common ID
+        PyRanges.max_disjoint : find the maximal disjoint set of intervals
+        PyRanges.split : split intervals into non-overlapping subintervals
 
         Examples
         --------
         >>> gr = pr.example_data.ensembl_gtf.get_with_loc_columns(["Feature", "gene_name"])
         >>> gr
         index    |    Chromosome    Start    End      Strand      Feature     gene_name
         int64    |    category      int64    int64    category    category    object
@@ -1733,19 +1830,20 @@
         use_strand = validate_and_convert_use_strand(self, use_strand)
 
         return self.apply_single(_merge, by=match_by, use_strand=use_strand, count_col=count_col, slack=slack)
 
     def nearest(
         self,
         other: "PyRanges",
-        strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "ignore",
+        strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
         direction: VALID_NEAREST_TYPE = "any",
         *,
+        match_by: VALID_BY_TYPES = None,
         suffix: str = JOIN_SUFFIX,
-        overlap: bool = True,
+        exclude_overlaps: bool = False,
     ) -> "PyRanges":
         """Find closest interval.
 
         For each interval in self PyRanges, the columns of the nearest interval in other PyRanges are appended.
 
         Parameters
         ----------
@@ -1753,20 +1851,22 @@
             PyRanges to find nearest interval in.
 
         strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
             Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
             information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
             otherwise ignore the strand information.
 
-        overlap : bool, default True
-            Whether to include overlaps.
+        exclude_overlaps : bool, default True
+            Whether to not report intervals of others that overlap with self as the nearest ones.
 
         direction : {"any", "upstream", "downstream"}, default "any", i.e. both directions
-            Whether to only look for nearest in one direction. Always with respect to the PyRanges
-            it is called on.
+            Whether to only look for nearest in one direction.
+
+        match_by : str or list, default None
+            If provided, only intervals with an equal value in column(s) `match_by` may be matched.
 
         suffix : str, default "_b"
             Suffix to give columns with shared name in other.
 
         Returns
         -------
         PyRanges
@@ -1786,64 +1886,125 @@
         -------  ---  ------------  -------  -------  ----------
               0  |    chr1                3        6  +
               1  |    chr1                5        7  -
               2  |    chr1                8        9  +
         PyRanges with 3 rows, 4 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
-        >>> f2 = pr.example_data.f2.remove_nonloc_columns()
+        >>> f2 = pr.PyRanges(dict(Chromosome="chr1", Start=[1, 6, 20], End=[2, 7, 22], Strand=["+", "-", "+"]))
         >>> f2
           index  |    Chromosome      Start      End  Strand
-          int64  |    category        int64    int64  category
-        -------  ---  ------------  -------  -------  ----------
+          int64  |    object          int64    int64  object
+        -------  ---  ------------  -------  -------  --------
               0  |    chr1                1        2  +
               1  |    chr1                6        7  -
-        PyRanges with 2 rows, 4 columns, and 1 index columns.
+              2  |    chr1               20       22  +
+        PyRanges with 3 rows, 4 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
         >>> f1.nearest(f2)
+          index  |    Chromosome      Start      End  Strand        Start_b    End_b    Distance
+          int64  |    category        int64    int64  category        int64    int64       int64
+        -------  ---  ------------  -------  -------  ----------  ---------  -------  ----------
+              0  |    chr1                3        6  +                   1        2           2
+              1  |    chr1                5        7  -                   6        7           0
+              2  |    chr1                8        9  +                   1        2           7
+        PyRanges with 3 rows, 7 columns, and 1 index columns.
+        Contains 1 chromosomes and 2 strands.
+
+        >>> f1.nearest(f2, strand_behavior='ignore')
           index  |    Chromosome      Start      End  Strand        Start_b    End_b  Strand_b      Distance
-          int64  |    category        int64    int64  category        int64    int64  category         int64
+          int64  |    category        int64    int64  category        int64    int64  object           int64
         -------  ---  ------------  -------  -------  ----------  ---------  -------  ----------  ----------
-              1  |    chr1                5        7  -                   6        7  -                    0
               0  |    chr1                3        6  +                   6        7  -                    1
-              1  |    chr1                8        9  +                   6        7  -                    2
-        PyRanges with 3 rows, 8 columns, and 1 index columns (with 1 index duplicates).
+              1  |    chr1                5        7  -                   6        7  -                    0
+              2  |    chr1                8        9  +                   6        7  -                    2
+        PyRanges with 3 rows, 8 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
-        >>> f1.nearest(f2, direction="upstream")
+        >>> f1.nearest(f2, strand_behavior='ignore', exclude_overlaps=True)
           index  |    Chromosome      Start      End  Strand        Start_b    End_b  Strand_b      Distance
-          int64  |    category        int64    int64  category        int64    int64  category         int64
+          int64  |    category        int64    int64  category        int64    int64  object           int64
         -------  ---  ------------  -------  -------  ----------  ---------  -------  ----------  ----------
-              1  |    chr1                5        7  -                   6        7  -                    0
-              0  |    chr1                3        6  +                   1        2  +                    2
-              1  |    chr1                8        9  +                   6        7  -                    2
-        PyRanges with 3 rows, 8 columns, and 1 index columns (with 1 index duplicates).
+              0  |    chr1                3        6  +                   6        7  -                    1
+              1  |    chr1                5        7  -                   1        2  +                    4
+              2  |    chr1                8        9  +                   6        7  -                    2
+        PyRanges with 3 rows, 8 columns, and 1 index columns.
+        Contains 1 chromosomes and 2 strands.
+
+        >>> f1.nearest(f2, direction='downstream')
+          index  |    Chromosome      Start      End  Strand        Start_b    End_b    Distance
+          int64  |    category        int64    int64  category        int64    int64       int64
+        -------  ---  ------------  -------  -------  ----------  ---------  -------  ----------
+              0  |    chr1                3        6  +                  20       22          15
+              1  |    chr1                5        7  -                   6        7           0
+              2  |    chr1                8        9  +                  20       22          12
+        PyRanges with 3 rows, 7 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
+        If an input interval has no suitable nearest interval, these rows are dropped:
+
+        >>> f1.nearest(f2, direction='upstream', exclude_overlaps=True)
+          index  |    Chromosome      Start      End  Strand        Start_b      End_b    Distance
+          int64  |    category        int64    int64  category      float64    float64       int64
+        -------  ---  ------------  -------  -------  ----------  ---------  ---------  ----------
+              0  |    chr1                3        6  +                   1          2           2
+              2  |    chr1                8        9  +                   1          2           7
+        PyRanges with 2 rows, 7 columns, and 1 index columns.
+        Contains 1 chromosomes and 1 strands.
+
         """
         from pyranges.methods.nearest import _nearest
 
-        if direction in {NEAREST_UPSTREAM, NEAREST_DOWNSTREAM} and not other.strand_valid:
-            msg = "If doing upstream or downstream nearest, other pyranges must be stranded"
+        strand_behavior = validate_and_convert_strand_behavior(self, other, strand_behavior)
+        if direction in {NEAREST_UPSTREAM, NEAREST_DOWNSTREAM} and strand_behavior == STRAND_BEHAVIOR_IGNORE:
+            msg = "For upstream or downstream nearest, strands must be valid and strand_behavior cannot be 'ignore'"
             raise AssertionError(msg)
 
-        return self.apply_pair(
-            other,
-            _nearest,
-            strand_behavior=strand_behavior,
-            how=direction,
-            overlap=overlap,
-            suffix=suffix,
+        if strand_behavior == STRAND_BEHAVIOR_OPPOSITE:
+            # swap strands in STRAND_COL, but keep original values in TEMP_STRAND_COL
+            self = mypy_ensure_pyranges(
+                self.assign(**{TEMP_STRAND_COL: self[STRAND_COL]}).assign(
+                    **{
+                        STRAND_COL: self[STRAND_COL].replace(
+                            {FORWARD_STRAND: REVERSE_STRAND, REVERSE_STRAND: FORWARD_STRAND},
+                        ),
+                    },
+                ),
+            )
+            # switch direction
+            if direction == NEAREST_UPSTREAM:
+                direction = NEAREST_DOWNSTREAM
+            elif direction == NEAREST_DOWNSTREAM:
+                direction = NEAREST_UPSTREAM
+
+        res = mypy_ensure_pyranges(
+            self.apply_pair(
+                other,
+                _nearest,
+                strand_behavior=strand_behavior,
+                how=direction,
+                by=match_by,
+                overlap=not exclude_overlaps,
+                suffix=suffix,
+                preserve_order=True,
+            ),
         )
 
+        if strand_behavior == STRAND_BEHAVIOR_OPPOSITE:
+            # swap back strands in STRAND_COL
+            res = res.drop_and_return(STRAND_COL, axis="columns").rename(columns={TEMP_STRAND_COL: STRAND_COL})
+
+        return mypy_ensure_pyranges(res)
+
     def overlap(  # type: ignore[override]
         self,
         other: "PyRanges",
         strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
+        slack: int = 0,
         *,
         match_by: VALID_BY_TYPES = None,
         invert: bool = False,
         contained: bool = False,
     ) -> "PyRanges":
         """Return overlapping intervals.
 
@@ -1855,14 +2016,19 @@
             PyRanges to find overlaps with.
 
         strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
             Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
             information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
             otherwise ignore the strand information.
 
+        slack : int, default 0
+            Intervals in self are temporarily extended by slack on both ends before overlap is calculated, so that
+            we allow non-overlapping intervals to be considered overlapping if they are within less than slack distance
+            e.g. slack=1 reports bookended intervals.
+
         invert : bool, default False
             Whether to return the intervals without overlaps.
 
         contained : bool, default False
             Whether to report only intervals that are entirely contained in an interval of 'other'.
 
         match_by : str or list, default None
@@ -1890,14 +2056,26 @@
         -------  ---  ------------  -------  -------  --------
               0  |    chr1                1        3  A
               1  |    chr1                1        3  a
               2  |    chr2                4        9  b
         PyRanges with 3 rows, 4 columns, and 1 index columns.
         Contains 2 chromosomes.
 
+        >>> gr.overlap(gr2, slack=2)
+          index  |    Chromosome      Start      End  ID
+          int64  |    object          int64    int64  object
+        -------  ---  ------------  -------  -------  --------
+              0  |    chr1                1        3  A
+              1  |    chr1                1        3  a
+              2  |    chr1               10       11  c
+              3  |    chr2                4        9  b
+        PyRanges with 4 rows, 4 columns, and 1 index columns.
+        Contains 2 chromosomes.
+
+
         >>> gr.overlap(gr2, contained=True)
           index  |    Chromosome      Start      End  ID
           int64  |    object          int64    int64  object
         -------  ---  ------------  -------  -------  --------
               2  |    chr2                4        9  b
         PyRanges with 1 rows, 4 columns, and 1 index columns.
         Contains 1 chromosomes.
@@ -1942,24 +2120,38 @@
         Contains 1 chromosomes and 1 strands.
 
         """
         from pyranges.methods.overlap import _overlap
 
         how = OVERLAP_CONTAINMENT if contained else OVERLAP_FIRST
 
-        return self.apply_pair(
+        _self = self.copy()
+        if slack:
+            _self[TEMP_START_SLACK_COL] = _self.Start
+            _self[TEMP_END_SLACK_COL] = _self.End
+            _self = _self.extend(slack, use_strand=False)
+
+        gr = _self.apply_pair(
             other,
             _overlap,
             strand_behavior=strand_behavior,
             by=match_by,
+            preserve_order=True,
             invert=invert,
             skip_if_empty=False if invert else SKIP_IF_EMPTY_LEFT,
             how=how,
         )
 
+        if slack and len(gr) > 0:
+            gr[START_COL] = gr[TEMP_START_SLACK_COL]
+            gr[END_COL] = gr[TEMP_END_SLACK_COL]
+            gr = gr.drop_and_return([TEMP_START_SLACK_COL, TEMP_END_SLACK_COL], axis=1)
+
+        return mypy_ensure_pyranges(gr)
+
     def set_intersect(
         self,
         other: "PyRanges",
         strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
         multiple: VALID_OVERLAP_TYPE = "all",
     ) -> "PyRanges":
         """Return set-theoretical intersection.
@@ -1974,28 +2166,30 @@
         strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
             Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
             information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
             otherwise ignore the strand information.
 
         multiple : {"all", "first", "last"}, default "all"
             What to report when multiple merged intervals in 'other' overlap with the same merged interval in self.
-            The default "all" reports all overlapping subintervals, which will have duplicate indices.
+            The default "all" reports all overlapping subintervals.
             "first" reports only, for each merged self interval, the overlapping 'other' subinterval with smallest Start
             "last" reports only the overlapping subinterval with the biggest End in 'other'
 
         Returns
         -------
         PyRanges
-
-            A PyRanges with overlapping subintervals.
+            A PyRanges with overlapping subintervals. Input index is not preserved.
+            No columns other than Chromosome, Start, End, and optionally Strand are returned.
 
         See Also
         --------
+        PyRanges.set_union : set-theoretical union
         PyRanges.intersect : find overlapping subintervals
         PyRanges.overlap : report overlapping intervals
+        PyRanges.merge_overlaps : merge overlapping intervals
 
         Examples
         --------
         >>> r1 = pr.PyRanges({"Chromosome": ["chr1"] * 3, "Start": [5, 20, 40],"End": [10, 30, 50], "ID": ["a", "b", "c"]})
         >>> r1
           index  |    Chromosome      Start      End  ID
           int64  |    object          int64    int64  object
@@ -2053,34 +2247,38 @@
                 how=multiple,
             ).reset_index(drop=True),
         )
 
     def set_union(self, other: "PyRanges", strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto") -> "PyRanges":
         """Return set-theoretical union.
 
+        Returns the regions present in either self or other.
+        Both PyRanges are merged first.
+
         Parameters
         ----------
         other : PyRanges
             PyRanges to do union with.
 
         strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
             Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
             information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
             otherwise ignore the strand information.
 
         Returns
         -------
         PyRanges
-
-            A PyRanges with the union of intervals.
+            A PyRanges with the union of intervals. Input index is not preserved.
+            No columns other than Chromosome, Start, End, and optionally Strand are returned.
 
         See Also
         --------
         PyRanges.set_intersect : set-theoretical intersection
         PyRanges.overlap : report overlapping intervals
+        PyRanges.merge_overlaps : merge overlapping intervals
 
         Examples
         --------
         >>> gr = pr.PyRanges({"Chromosome": ["chr1"] * 3, "Start": [1, 4, 10],
         ...                    "End": [3, 9, 11], "ID": ["a", "b", "c"]})
         >>> gr
           index  |    Chromosome      Start      End  ID
@@ -2103,28 +2301,51 @@
         PyRanges with 3 rows, 3 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         >>> gr.set_union(gr2)
           index  |    Chromosome      Start      End
           int64  |    object          int64    int64
         -------  ---  ------------  -------  -------
+              0  |    chr1                1        9
+              1  |    chr1                9       10
+              2  |    chr1               10       11
+        PyRanges with 3 rows, 3 columns, and 1 index columns.
+        Contains 1 chromosomes.
+
+        Merging bookended intervals:
+
+        >>> gr.set_union(gr2).merge_overlaps(slack=1)
+          index  |    Chromosome      Start      End
+          int64  |    object          int64    int64
+        -------  ---  ------------  -------  -------
               0  |    chr1                1       11
         PyRanges with 1 rows, 3 columns, and 1 index columns.
         Contains 1 chromosomes.
 
+
         """
         if self.empty and other.empty:
             return mypy_ensure_pyranges(self.copy())
 
         strand_behavior = validate_and_convert_strand_behavior(self, other, strand_behavior)
         use_strand = use_strand_from_validated_strand_behavior(self, other, strand_behavior)
 
         if not use_strand:
             self = self.remove_strand()
             other = other.remove_strand()
+        elif strand_behavior == STRAND_BEHAVIOR_OPPOSITE:
+            other = mypy_ensure_pyranges(
+                other.assign(
+                    **{
+                        STRAND_COL: other[STRAND_COL].replace(
+                            {FORWARD_STRAND: REVERSE_STRAND, REVERSE_STRAND: FORWARD_STRAND},
+                        ),
+                    },
+                ),
+            )
 
         gr = pr.concat([self, other])
 
         return gr.merge_overlaps(use_strand=use_strand)
 
     def sort_ranges(
         self,
@@ -2536,15 +2757,18 @@
         -------
         PyRanges
 
             PyRanges with intervals split at overlap points.
 
         See Also
         --------
-        pyranges.multioverlap : find overlaps with multiple PyRanges
+        PyRanges.merge_overlaps : merge overlapping intervals
+        PyRanges.max_disjoint : find the maximal disjoint set of intervals
+        PyRanges.split : split intervals into non-overlapping subintervals
+
 
         Examples
         --------
         >>> gr = pr.PyRanges({'Chromosome': ['chr1', 'chr1', 'chr1', 'chr1'], 'Start': [3, 5, 5, 11],
         ...                   'End': [6, 9, 7, 12], 'Strand': ['+', '+', '-', '-']})
         >>> gr
           index  |    Chromosome      Start      End  Strand
@@ -2937,14 +3161,20 @@
             How to handle strand information. "auto" means use "same" if both PyRanges are stranded,
             otherwise ignore the strand information. "same" means only subtract intervals on the same strand.
             "opposite" means only subtract intervals on the opposite strand. "ignore" means ignore strand
 
         match_by : str or list, default None
             If provided, only intervals with an equal value in column(s) `match_by` may be considered as overlapping.
 
+        Returns
+        -------
+        PyRanges
+            PyRanges with subintervals from self that do not overlap with any interval in other.
+            Columns and index are preserved.
+
         Warning
         -------
         The returned Pyranges may have index duplicates. Call .reset_index(drop=True) to fix it.
 
         See Also
         --------
         PyRanges.overlap : use with invert=True to return all intervals without overlap
@@ -3014,36 +3244,41 @@
               2  |    chr1               10       11  c         z
         PyRanges with 3 rows, 5 columns, and 1 index columns.
         Contains 1 chromosomes.
 
         """
         from pyranges.methods.subtraction import _subtraction
 
+        strand_behavior = validate_and_convert_strand_behavior(self, other, strand_behavior)
         use_strand = use_strand_from_validated_strand_behavior(self, other, strand_behavior)
 
         other_clusters = other.merge_overlaps(use_strand=use_strand, match_by=match_by)
 
         grpby_ks = group_keys_from_validated_strand_behavior(strand_behavior, match_by)
 
         gr = self.count_overlaps(
             other_clusters,
             strand_behavior=strand_behavior,
             overlap_col=TEMP_NUM_COL,
             match_by=grpby_ks,
         )
+        gr[TEMP_ID_COL] = np.arange(len(gr))
 
         result = gr.apply_pair(
             other_clusters,
             strand_behavior=strand_behavior,
             function=_subtraction,
             by=grpby_ks,
             skip_if_empty=False,
         )
 
-        return result.drop_and_return(TEMP_NUM_COL, axis=1)
+        return mypy_ensure_pyranges(result.sort_values(TEMP_ID_COL)).drop_and_return(
+            [TEMP_NUM_COL, TEMP_ID_COL],
+            axis=1,
+        )
 
     def summary(
         self,
         *,
         return_df: bool = False,
     ) -> pd.DataFrame | None:
         """Return info.
@@ -4167,16 +4402,15 @@
 
         match_by : str or list, default None
             If provided, only intervals with an equal value in column(s) `match_by` may be considered as overlapping.
 
         Returns
         -------
         PyRanges
-
-            A PyRanges with overlapping intervals.
+            A PyRanges with overlapping intervals. Input index is preserved, but may contain duplicates.
 
         See Also
         --------
         PyRanges.overlap : report overlapping (unmodified) intervals
         PyRanges.subtract_ranges : report non-overlapping subintervals
         PyRanges.set_intersect : set-intersect PyRanges
 
@@ -4237,40 +4471,48 @@
 
         """
         from pyranges.methods.overlap import _intersect
 
         # note: argument multiple = 'containment' is formally accepted but omitted in docstring since the result
         # will be always the same as self.overlap(other, contained=True), no intersect is done in that case
 
-        return self.apply_pair(
+        _self = self.copy()
+        _self[TEMP_ID_COL] = np.arange(len(_self))
+
+        gr = _self.apply_pair(
             other,
             _intersect,
             strand_behavior=strand_behavior,
             by=match_by,
             how=multiple,
         )
 
+        # preserving order. I can't use the reindex syntax as in other functions because of potential duplicates
+        gr = mypy_ensure_pyranges(gr.sort_values(TEMP_ID_COL))
+        return gr.drop_and_return(TEMP_ID_COL, axis=1)
+
     def combine_interval_columns(
         self,
         function: VALID_COMBINE_OPTIONS | CombineIntervalColumnsOperation = "intersect",
         *,
         start: str = START_COL,
         end: str = END_COL,
         start2: str = START_COL + JOIN_SUFFIX,
         end2: str = END_COL + JOIN_SUFFIX,
         drop_old_columns: bool = True,
     ) -> "pr.PyRanges":
         """Use two pairs of columns representing intervals to create a new start and end column.
 
+        The function is designed as post-processing after join_ranges to aggregate the coordinates of the two intervals.
         By default, the new start and end columns will be the intersection of the intervals.
 
         Parameters
         ----------
-        function : {"intersect", "union"} or Callable, default "intersect"
-            How to combine the intervals: "intersect" or "union".
+        function : {"intersect", "union", "swap"} or Callable, default "intersect"
+            How to combine the self and other intervals: "intersect", "union", or "swap"
             If a callable is passed, it should take four Series arguments: start1, end1, start2, end2;
             and return a tuple of two integers: (new_starts, new_ends).
 
         start : str, default "Start"
             Column name for Start of first interval
         end : str, default "End"
             Column name for End of first interval
@@ -4285,72 +4527,91 @@
         --------
         >>> gr1, gr2 = pr.example_data.aorta.head(3).remove_nonloc_columns(), pr.example_data.aorta2.head(3).remove_nonloc_columns()
         >>> j = gr1.join_ranges(gr2)
         >>> j
           index  |    Chromosome      Start      End  Strand        Start_b    End_b
           int64  |    category        int64    int64  category        int64    int64
         -------  ---  ------------  -------  -------  ----------  ---------  -------
-              1  |    chr1             9939    10138  +               10073    10272
               0  |    chr1             9916    10115  -                9988    10187
-              0  |    chr1             9916    10115  -               10079    10278
-              2  |    chr1             9951    10150  -                9988    10187
-              2  |    chr1             9951    10150  -               10079    10278
-        PyRanges with 5 rows, 6 columns, and 1 index columns (with 2 index duplicates).
+              1  |    chr1             9916    10115  -               10079    10278
+              2  |    chr1             9939    10138  +               10073    10272
+              3  |    chr1             9951    10150  -                9988    10187
+              4  |    chr1             9951    10150  -               10079    10278
+        PyRanges with 5 rows, 6 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
         The default operation is to intersect the intervals:
 
         >>> j.combine_interval_columns()
           index  |    Chromosome      Start      End  Strand
           int64  |    category        int64    int64  category
         -------  ---  ------------  -------  -------  ----------
-              1  |    chr1            10073    10138  +
               0  |    chr1             9988    10115  -
-              0  |    chr1            10079    10115  -
-              2  |    chr1             9988    10150  -
-              2  |    chr1            10079    10150  -
-        PyRanges with 5 rows, 4 columns, and 1 index columns (with 2 index duplicates).
+              1  |    chr1            10079    10115  -
+              2  |    chr1            10073    10138  +
+              3  |    chr1             9988    10150  -
+              4  |    chr1            10079    10150  -
+        PyRanges with 5 rows, 4 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
         Take the union instead:
 
         >>> j.combine_interval_columns('union')
           index  |    Chromosome      Start      End  Strand
           int64  |    category        int64    int64  category
         -------  ---  ------------  -------  -------  ----------
-              1  |    chr1             9939    10272  +
               0  |    chr1             9916    10187  -
-              0  |    chr1             9916    10278  -
-              2  |    chr1             9951    10187  -
-              2  |    chr1             9951    10278  -
-        PyRanges with 5 rows, 4 columns, and 1 index columns (with 2 index duplicates).
+              1  |    chr1             9916    10278  -
+              2  |    chr1             9939    10272  +
+              3  |    chr1             9951    10187  -
+              4  |    chr1             9951    10278  -
+        PyRanges with 5 rows, 4 columns, and 1 index columns.
+        Contains 1 chromosomes and 2 strands.
+
+        >>> j.combine_interval_columns('swap')
+          index  |    Chromosome      Start      End  Strand
+          int64  |    category        int64    int64  category
+        -------  ---  ------------  -------  -------  ----------
+              0  |    chr1             9988    10187  -
+              1  |    chr1            10079    10278  -
+              2  |    chr1            10073    10272  +
+              3  |    chr1             9988    10187  -
+              4  |    chr1            10079    10278  -
+        PyRanges with 5 rows, 4 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
+
         Use a custom function that keeps the start of the first interval and the end of the second:
 
         >>> def custom_combine(s1, e1, s2, e2): return (s1, e2)
         >>> j.combine_interval_columns(custom_combine)
           index  |    Chromosome      Start      End  Strand
           int64  |    category        int64    int64  category
         -------  ---  ------------  -------  -------  ----------
-              1  |    chr1             9939    10272  +
               0  |    chr1             9916    10187  -
-              0  |    chr1             9916    10278  -
-              2  |    chr1             9951    10187  -
-              2  |    chr1             9951    10278  -
-        PyRanges with 5 rows, 4 columns, and 1 index columns (with 2 index duplicates).
+              1  |    chr1             9916    10278  -
+              2  |    chr1             9939    10272  +
+              3  |    chr1             9951    10187  -
+              4  |    chr1             9951    10278  -
+        PyRanges with 5 rows, 4 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
         """
-        from pyranges.methods.combine_positions import _intersect_interval_columns, _union_interval_columns
+        from pyranges.methods.combine_positions import (
+            _intersect_interval_columns,
+            _swap_interval_columns,
+            _union_interval_columns,
+        )
 
         if function == "intersect":
             function = _intersect_interval_columns
         elif function == "union":
             function = _union_interval_columns
+        elif function == "swap":
+            function = _swap_interval_columns
 
         new_starts, new_ends = function(self[start], self[end], self[start2], self[end2])
 
         z = self.copy()
         z[START_COL] = new_starts
         z[END_COL] = new_ends
```

### Comparing `pyranges1-1.0.0/pyranges/core/random.py` & `pyranges1-1.0.1/pyranges/core/random.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/tostring.py` & `pyranges1-1.0.1/pyranges/core/tostring.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/core/version.py` & `pyranges1-1.0.1/pyranges/core/version.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/bigwig.bw` & `pyranges1-1.0.1/pyranges/data/bigwig.bw`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/chipseq.bed` & `pyranges1-1.0.1/pyranges/data/chipseq.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/chipseq_background.bed` & `pyranges1-1.0.1/pyranges/data/chipseq_background.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/cpg.bed` & `pyranges1-1.0.1/pyranges/data/cpg.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/ensembl.gtf` & `pyranges1-1.0.1/pyranges/data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/ensembl_human.gtf.gz` & `pyranges1-1.0.1/pyranges/data/ensembl_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/exons.bed` & `pyranges1-1.0.1/pyranges/data/exons.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/gencode_human.gtf.gz` & `pyranges1-1.0.1/pyranges/data/gencode_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/lamina.bed` & `pyranges1-1.0.1/pyranges/data/lamina.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/ncbi.fasta` & `pyranges1-1.0.1/pyranges/data/ncbi.fasta`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/ncbi.gff.gz` & `pyranges1-1.0.1/pyranges/data/ncbi.gff.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/smaller.bam` & `pyranges1-1.0.1/pyranges/data/smaller.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/data/ucsc_human.bed.gz` & `pyranges1-1.0.1/pyranges/data/ucsc_human.bed.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/ext/orfs.py` & `pyranges1-1.0.1/pyranges/ext/orfs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/ext/seqs.py` & `pyranges1-1.0.1/pyranges/ext/seqs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/ext/stats.py` & `pyranges1-1.0.1/pyranges/ext/stats.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/boundaries.py` & `pyranges1-1.0.1/pyranges/methods/boundaries.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/combine_positions.py` & `pyranges1-1.0.1/pyranges/methods/combine_positions.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     starts2: pd.Series,
     ends2: pd.Series,
 ) -> tuple[pd.Series, pd.Series]:
     new_starts = pd.Series(
         np.where(starts > starts2.to_numpy(), starts, starts2),
         index=starts.index,
     )
-
     new_ends = pd.Series(
         np.where(ends < ends2.to_numpy(), ends, ends2),
         index=ends.index,
     )
     return new_starts, new_ends
 
 
@@ -26,14 +25,21 @@
     starts2: pd.Series,
     ends2: pd.Series,
 ) -> tuple[pd.Series, pd.Series]:
     new_starts = pd.Series(
         np.where(starts < starts2.to_numpy(), starts, starts2),
         index=starts.index,
     )
-
     new_ends = pd.Series(
         np.where(ends > ends2.to_numpy(), ends, ends2),
         index=ends.index,
     )
-
     return new_starts, new_ends
+
+
+def _swap_interval_columns(
+    starts: pd.Series,  # noqa: ARG001
+    ends: pd.Series,  # noqa: ARG001
+    starts2: pd.Series,
+    ends2: pd.Series,
+) -> tuple[pd.Series, pd.Series]:
+    return starts2, ends2
```

### Comparing `pyranges1-1.0.0/pyranges/methods/concat.py` & `pyranges1-1.0.1/pyranges/methods/concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/coverage.py` & `pyranges1-1.0.1/pyranges/methods/coverage.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/join.py` & `pyranges1-1.0.1/pyranges/methods/join.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/merge.py` & `pyranges1-1.0.1/pyranges/methods/merge.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,18 @@
         return df
 
     slack = kwargs.get("slack", 0)
     by = kwargs["by"]
 
     cdf = df.sort_values(START_COL)
 
-    starts, ends, number = find_clusters(cdf.Start.values, cdf.End.values, slack)
+    # important: sorted_nearest interprets slack differently than pyranges
+    # 0 slack in sorted_nearest means that bookended intervals are considered overlapping
+    # together, while in pyranges it means that they are not.
+    starts, ends, number = find_clusters(cdf.Start.values, cdf.End.values, slack - 1)
 
     by_values = df.head(1).squeeze()[by].to_dict()
 
     cluster_df = pd.DataFrame(
         {
             START_COL: starts,
             END_COL: ends,
```

### Comparing `pyranges1-1.0.0/pyranges/methods/nearest.py` & `pyranges1-1.0.1/pyranges/methods/nearest.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,23 @@
     nearest_next_nonoverlapping,
     nearest_nonoverlapping,
     nearest_previous_nonoverlapping,
 )
 
 import pyranges.core.empty
 from pyranges import PyRanges
-from pyranges.core.names import END_COL, START_COL
+from pyranges.core.names import (
+    BY_ENTRY_IN_KWARGS,
+    END_COL,
+    FORWARD_STRAND,
+    GENOME_LOC_COLS_WITH_STRAND,
+    REVERSE_STRAND,
+    START_COL,
+    STRAND_COL,
+)
 from pyranges.methods.sort import sort_one_by_one
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, NDArray
     from pandas import DataFrame
 
 
@@ -35,15 +43,15 @@
         pd.Series(dist, index=df2.index).fillna(-1).astype(int),
     )
 
     return df2
 
 
 def _overlapping_for_nearest(df: pd.DataFrame, df2: pd.DataFrame, suffix: str) -> tuple[pd.DataFrame, pd.DataFrame]:
-    nearest_df = pd.DataFrame(columns="Chromosome Start End Strand".split())
+    nearest_df = pd.DataFrame(columns=GENOME_LOC_COLS_WITH_STRAND)
 
     it = NCLS(df2.Start.to_numpy(), df2.End.to_numpy(), df2.index.to_numpy())
 
     idx_self, idx_other = it.first_overlap_both(
         df[START_COL].to_numpy(),
         df[END_COL].to_numpy(),
         df.index.to_numpy(),
@@ -99,38 +107,42 @@
     return r_idx, dist
 
 
 def _nearest(df: "DataFrame", df2: "DataFrame", **kwargs) -> pd.DataFrame:
     if df.empty or df2.empty:
         return PyRanges()
 
+    columns_used_for_by = kwargs.get(BY_ENTRY_IN_KWARGS, {}).keys()
     overlap = kwargs["overlap"]
     how = kwargs["how"]
     suffix = kwargs["suffix"]
+    strand = kwargs.get(BY_ENTRY_IN_KWARGS, {}).get(STRAND_COL)
 
     if how == "upstream":
-        strand = df.Strand.iloc[0]
-        how = {"+": "previous", "-": "next"}[strand]
+        how = {FORWARD_STRAND: "previous", REVERSE_STRAND: "next"}[strand]
     elif how == "downstream":
-        strand = df.Strand.iloc[0]
-        how = {"+": "next", "-": "previous"}[strand]
+        how = {FORWARD_STRAND: "next", REVERSE_STRAND: "previous"}[strand]
 
-    df2 = df2.reset_index(drop=True)
+    df2 = df2.drop(columns=columns_used_for_by).reset_index(drop=True)
 
     if overlap:
         nearest_df, df_to_find_nearest_in = _overlapping_for_nearest(df, df2, suffix)
     else:
         df_to_find_nearest_in = df
         nearest_df = pyranges.core.empty.empty()
 
     df = pyranges.core.empty.empty_df()
     if not df_to_find_nearest_in.empty:
-        df_to_find_nearest_in = sort_one_by_one(df_to_find_nearest_in, "Start", "End")
-        df2 = sort_one_by_one(df2, "Start", "End")
-        df_to_find_nearest_in.index = pd.Index(range(len(df_to_find_nearest_in)))
+        df_to_find_nearest_in = sort_one_by_one(df_to_find_nearest_in, START_COL, END_COL)
+        df2 = sort_one_by_one(df2, START_COL, END_COL)
+
+        # preserving index name
+        original_index_names = df_to_find_nearest_in.index.names
+        index_names = [name if name is not None else f"__index{i}" for i, name in enumerate(original_index_names)]
+        df_to_find_nearest_in = df_to_find_nearest_in.reset_index(names=index_names)
 
         if how == "next":
             r_idx, dist = _next_nonoverlapping(df_to_find_nearest_in.End, df2.Start, df2.index.to_numpy())
         elif how == "previous":
             r_idx, dist = _previous_nonoverlapping(df_to_find_nearest_in.Start, df2.End)
         else:
             previous_r_idx, previous_dist = _previous_nonoverlapping(df_to_find_nearest_in.Start, df2.End)
@@ -146,13 +158,17 @@
         df2 = _insert_distance(df2, dist, suffix)
 
         _r_idx = pd.Series(r_idx, index=df2.index)
         df_to_find_nearest_in = df_to_find_nearest_in.drop(_r_idx[_r_idx == -1].index)
 
         df = df_to_find_nearest_in.join(df2, rsuffix=suffix)
 
-    if overlap and "df" in locals() and not df.empty and not nearest_df.empty:
+        # restoring index and index names
+        df = df.set_index(index_names)
+        df.index.names = original_index_names
+
+    if overlap and not df.empty and not nearest_df.empty:
         df = pd.concat([nearest_df, df], sort=False)
     elif overlap and not nearest_df.empty:
         df = nearest_df
 
-    return PyRanges(df.drop("Chromosome" + suffix, axis=1))
+    return df
```

### Comparing `pyranges1-1.0.0/pyranges/methods/overlap.py` & `pyranges1-1.0.1/pyranges/methods/overlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/spliced_subsequence.py` & `pyranges1-1.0.1/pyranges/methods/spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/split.py` & `pyranges1-1.0.1/pyranges/methods/split.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/statistics.py` & `pyranges1-1.0.1/pyranges/methods/statistics.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/subsequence.py` & `pyranges1-1.0.1/pyranges/methods/subsequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     orig_order = df.index.copy()
     df.insert(0, TEMP_INDEX_COL, orig_order)
 
     by = [col for col in by if col not in [CHROM_COL, STRAND_COL]]
     by_argument_given = bool(by)
     by = by or [TEMP_INDEX_COL]
 
-    strand = kwargs.get(BY_ENTRY_IN_KWARGS, {}).get("Strand")
+    strand = kwargs.get(BY_ENTRY_IN_KWARGS, {}).get(STRAND_COL)
 
     # at this point, strand is False if 1. spliced_subsequence was called with use_strand=False or
     #                                   2. it was called with use_strand='auto' and not self.valid_strand
     # or it can be '+' or '-' if:
     #  1. it was input as True to spliced_subsequence and passed  to pyrange_apply_single as True,
     #     which updates it to '-' or '+' before calling _spliced_subseq, or
     #  2. it was called with strand=None and self is stranded
```

### Comparing `pyranges1-1.0.0/pyranges/methods/subtraction.py` & `pyranges1-1.0.1/pyranges/methods/subtraction.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/summary.py` & `pyranges1-1.0.1/pyranges/methods/summary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/tile_genome.py` & `pyranges1-1.0.1/pyranges/methods/tile_genome.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/to_rle.py` & `pyranges1-1.0.1/pyranges/methods/to_rle.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/methods/windows.py` & `pyranges1-1.0.1/pyranges/methods/windows.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/range_frame/range_frame.py` & `pyranges1-1.0.1/pyranges/range_frame/range_frame.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/range_frame/range_frame_validator.py` & `pyranges1-1.0.1/pyranges/range_frame/range_frame_validator.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/pyranges/readers.py` & `pyranges1-1.0.1/pyranges/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,14 +632,18 @@
     f : str
         Path to bw file.
 
     Returns
     -------
     PyRanges
 
+    Note
+    ----
+    This function requires the library pyBigWig, it can be installed with pip install pyBigWig
+
     Examples
     --------
     >>> import pyranges as pr
     >>> path = pr.example_data.files["bigwig.bw"]
     >>> pr.read_bigwig(path)
       index  |      Chromosome    Start      End      Value
       int64  |          object    int64    int64    float64
```

### Comparing `pyranges1-1.0.0/pyranges1.egg-info/PKG-INFO` & `pyranges1-1.0.1/pyranges1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 1.0.0
+Version: 1.0.1
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyranges1-1.0.0/pyranges1.egg-info/SOURCES.txt` & `pyranges1-1.0.1/pyranges1.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,33 @@
 docs/extension_orfs.rst
 docs/extension_seqs.rst
 docs/extension_stats.rst
 docs/how_to_columns.rst
 docs/how_to_create.rst
 docs/how_to_genomic_ops.rst
 docs/how_to_inspect.rst
+docs/how_to_overlap.rst
 docs/how_to_pages.rst
 docs/how_to_rows.rst
 docs/how_to_sequences.rst
 docs/how_to_write.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/migration_cheatsheet.tsv
+docs/migration_guide.rst
 docs/pyranges_extensions.rst
 docs/pyranges_module.rst
 docs/pyranges_objects.rst
 docs/range_frame.rst
 docs/requirements.txt
 docs/todos.rst
 docs/tutorial.rst
+docs/_static/custom.css
+docs/_templates/custom_method_summary.rst
 pyranges/__init__.py
 pyranges/docs
 pyranges/orfs.py
 pyranges/readers.py
 pyranges/seqs.py
 pyranges/stats.py
 pyranges/core/__init__.py
```

### Comparing `pyranges1-1.0.0/tests/.fuse_hidden0000017200000002` & `pyranges1-1.0.1/tests/.fuse_hidden0000017200000002`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/helpers.py` & `pyranges1-1.0.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/hi` & `pyranges1-1.0.1/tests/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/property_based/hypothesis_helper.py` & `pyranges1-1.0.1/tests/property_based/hypothesis_helper.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/property_based/new.py` & `pyranges1-1.0.1/tests/property_based/new.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/property_based/test_binary.py` & `pyranges1-1.0.1/tests/property_based/test_binary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/property_based/test_do_not_error.py` & `pyranges1-1.0.1/tests/property_based/test_do_not_error.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/property_based/test_unary.py` & `pyranges1-1.0.1/tests/property_based/test_unary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/test_parallelism.py` & `pyranges1-1.0.1/tests/test_parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/chip_10.bed` & `pyranges1-1.0.1/tests/unit/chip_10.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/conftest.py` & `pyranges1-1.0.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/hi` & `pyranges1-1.0.1/tests/unit/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/k_nearest.py` & `pyranges1-1.0.1/tests/unit/k_nearest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/out/test_out.py` & `pyranges1-1.0.1/tests/unit/out/test_out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/spliced_subsequence/test_spliced_subsequence.py` & `pyranges1-1.0.1/tests/unit/spliced_subsequence/test_spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/test_concat.py` & `pyranges1-1.0.1/tests/unit/test_concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/test_count_overlaps.py` & `pyranges1-1.0.1/tests/unit/test_count_overlaps.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/test_data/ensembl.gtf` & `pyranges1-1.0.1/tests/unit/test_data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/test_data/test_sorted.bam` & `pyranges1-1.0.1/tests/unit/test_data/test_sorted.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/test_data/test_sorted.bam.bai` & `pyranges1-1.0.1/tests/unit/test_data/test_sorted.bam.bai`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/test_guessers.py` & `pyranges1-1.0.1/tests/unit/test_guessers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-1.0.0/tests/unit/test_join.py` & `pyranges1-1.0.1/tests/unit/test_join.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             "Chromosome": ["chr1", "chr1"],
             "Start": [795, 795],
             "End": [895, 895],
             "Strand": ["-", "-"],
             "Start_b": [731, 821],
             "End_b": [831, 921],
         },
-        index=[3, 3],
+        index=[0, 1],
     )
 
     assert j.equals(expected_result)
 
 
 def test_join_issue_8_right():
     gd = {
@@ -70,10 +70,10 @@
             "Chromosome": ["chr1", "chr1", nan, nan],
             "Start": [795.0, 795.0, nan, nan],
             "End": [895.0, 895.0, nan, nan],
             "Strand": ["-", "-", nan, nan],
             "Start_b": [731, 821, 157, 584],
             "End_b": [831, 921, 257, 684],
         },
-        index=[2, 3, 0, 1],
+        index=[0, 1, 2, 3],
     )
     assert j.equals(expected_result)
```

### Comparing `pyranges1-1.0.0/tests/unit/test_pandas_overrides.py` & `pyranges1-1.0.1/tests/unit/test_pandas_overrides.py`

 * *Files identical despite different names*

