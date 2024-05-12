# Comparing `tmp/pythainlp-5.0.2.tar.gz` & `tmp/pythainlp-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythainlp-5.0.2.tar", last modified: Wed Apr  3 10:21:15 2024, max compression
+gzip compressed data, was "pythainlp-5.0.3.tar", last modified: Sun May 12 10:30:24 2024, max compression
```

## Comparing `pythainlp-5.0.2.tar` & `pythainlp-5.0.3.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.857493 pythainlp-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-03 10:21:04.000000 pythainlp-5.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 10:21:04.000000 pythainlp-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 10:21:04.000000 pythainlp-5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-03 10:21:15.857493 pythainlp-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-03 10:21:04.000000 pythainlp-5.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17911 2024-04-03 10:21:04.000000 pythainlp-5.0.2/README_TH.md
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.829493 pythainlp-5.0.2/pythainlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.829493 pythainlp-5.0.2/pythainlp/ancient/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/ancient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/ancient/aksonhan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.829493 pythainlp-5.0.2/pythainlp/augment/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/augment/lm/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/lm/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/lm/phayathaibert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/lm/wangchanberta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/augment/word2vec/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/word2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/word2vec/bpemb_wv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/word2vec/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/word2vec/ltw2v.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/word2vec/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/augment/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/benchmarks/word_tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/chat/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/chat/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/classify/param_free.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/cli/soundex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/cli/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/cli/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/cls/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/cls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.833493 pythainlp-5.0.2/pythainlp/coref/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/coref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/coref/_fastcoref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/coref/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/coref/han_coref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.837493 pythainlp-5.0.2/pythainlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/icu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/oscar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/th_en_translit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/tnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/ttc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/volubilis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/corpus/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.837493 pythainlp-5.0.2/pythainlp/el/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/el/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/el/_multiel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/el/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.837493 pythainlp-5.0.2/pythainlp/generate/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/generate/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/generate/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/generate/wangchanglm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.837493 pythainlp-5.0.2/pythainlp/khavee/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/khavee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25046 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/khavee/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/khavee/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.837493 pythainlp-5.0.2/pythainlp/morpheme/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/morpheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/morpheme/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/morpheme/word_formation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.837493 pythainlp-5.0.2/pythainlp/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/parse/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/parse/esupar_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/parse/spacy_thai_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/parse/transformers_ud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/parse/ud_goeswith.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.837493 pythainlp-5.0.2/pythainlp/phayathaibert/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/phayathaibert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15435 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/phayathaibert/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.841493 pythainlp-5.0.2/pythainlp/soundex/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/soundex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/soundex/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/soundex/lk82.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/soundex/metasound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/soundex/prayut_and_somchaip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/soundex/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/soundex/udom83.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.841493 pythainlp-5.0.2/pythainlp/spell/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/spell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/spell/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/spell/phunspell.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/spell/pn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/spell/symspellpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/spell/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/spell/wanchanberta_thai_grammarly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.841493 pythainlp-5.0.2/pythainlp/summarize/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/summarize/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/summarize/freq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/summarize/keybert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/summarize/mt5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.845493 pythainlp-5.0.2/pythainlp/tag/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/_tag_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/crfchunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/orchid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/pos_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/thai_nner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/thainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/unigram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tag/wangchanberta_onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.845493 pythainlp-5.0.2/pythainlp/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/attacut.py
--rw-r--r--   0 runner    (1001) docker     (127)    31383 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/crfcls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/crfcut.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/deepcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/etcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/han_solo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/longest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/multi_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/nercut.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/newmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/nlpo3.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/oskut.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/sefr_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/ssg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/tcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/tcc_p.py
--rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/thaisumcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tokenize/wtsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.845493 pythainlp-5.0.2/pythainlp/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tools/misspell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/tools/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.849493 pythainlp-5.0.2/pythainlp/translate/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/translate/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/translate/en_th.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/translate/small100.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/translate/th_fr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/translate/tokenization_small100.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/translate/zh_th.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.849493 pythainlp-5.0.2/pythainlp/transliterate/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/iso_11940.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/royin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/spoonerism.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/thai2rom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/thai2rom_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/thaig2p.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/tltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/w2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/transliterate/wunsen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.849493 pythainlp-5.0.2/pythainlp/ulmfit/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/ulmfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/ulmfit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/ulmfit/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/ulmfit/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.853493 pythainlp-5.0.2/pythainlp/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/abbreviation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/digitconv.py
--rw-r--r--   0 runner    (1001) docker     (127)    93458 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/emojiconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/morse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/numtoword.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/phoneme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/pronounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/remove_trailing_repeat_consonants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/spell_words.py
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/strftime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/syllable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/thai.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/util/wordtonum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.853493 pythainlp-5.0.2/pythainlp/wangchanberta/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/wangchanberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/wangchanberta/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.853493 pythainlp-5.0.2/pythainlp/word_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/word_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/word_vector/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.853493 pythainlp-5.0.2/pythainlp/wsd/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/wsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-03 10:21:04.000000 pythainlp-5.0.2/pythainlp/wsd/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.829493 pythainlp-5.0.2/pythainlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-03 10:21:15.000000 pythainlp-5.0.2/pythainlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-03 10:21:15.000000 pythainlp-5.0.2/pythainlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:21:15.000000 pythainlp-5.0.2/pythainlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 10:21:15.000000 pythainlp-5.0.2/pythainlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:21:15.000000 pythainlp-5.0.2/pythainlp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-03 10:21:15.000000 pythainlp-5.0.2/pythainlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 10:21:15.000000 pythainlp-5.0.2/pythainlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-03 10:21:15.861493 pythainlp-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-03 10:21:04.000000 pythainlp-5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.857493 pythainlp-5.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:21:15.857493 pythainlp-5.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/data/eval-details-input.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/data/eval-input.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/data/input.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/data/sentences.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_ancient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_coref.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_el.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_khavee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_misspell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_morpheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_soundex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_spell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    58154 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_transliterate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_ulmfit.py
--rw-r--r--   0 runner    (1001) docker     (127)    38788 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_wangchanberta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_word_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 10:21:04.000000 pythainlp-5.0.2/tests/test_wsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.645979 pythainlp-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-05-12 10:30:16.000000 pythainlp-5.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 10:30:16.000000 pythainlp-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 10:30:16.000000 pythainlp-5.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-12 10:30:24.645979 pythainlp-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-05-12 10:30:16.000000 pythainlp-5.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17911 2024-05-12 10:30:16.000000 pythainlp-5.0.3/README_TH.md
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/ancient/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/ancient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/ancient/aksonhan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/augment/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/augment/lm/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/lm/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/lm/phayathaibert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/lm/wangchanberta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/augment/word2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/word2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/word2vec/bpemb_wv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/word2vec/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/word2vec/ltw2v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/word2vec/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/augment/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/benchmarks/word_tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/chat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/classify/param_free.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.621979 pythainlp-5.0.3/pythainlp/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/cli/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/cli/soundex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/cli/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/cli/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.621979 pythainlp-5.0.3/pythainlp/cls/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/cls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.621979 pythainlp-5.0.3/pythainlp/coref/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/coref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/coref/_fastcoref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/coref/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/coref/han_coref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.621979 pythainlp-5.0.3/pythainlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18455 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/icu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/oscar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/th_en_translit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/tnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/ttc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/volubilis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/corpus/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.621979 pythainlp-5.0.3/pythainlp/el/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/el/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/el/_multiel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/el/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.621979 pythainlp-5.0.3/pythainlp/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/generate/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/generate/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/generate/wangchanglm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.621979 pythainlp-5.0.3/pythainlp/khavee/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/khavee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25046 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/khavee/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/khavee/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.625979 pythainlp-5.0.3/pythainlp/morpheme/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/morpheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/morpheme/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/morpheme/word_formation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.625979 pythainlp-5.0.3/pythainlp/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/parse/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/parse/esupar_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/parse/spacy_thai_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/parse/transformers_ud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/parse/ud_goeswith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.625979 pythainlp-5.0.3/pythainlp/phayathaibert/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/phayathaibert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15435 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/phayathaibert/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.625979 pythainlp-5.0.3/pythainlp/soundex/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/soundex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/soundex/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/soundex/lk82.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/soundex/metasound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/soundex/prayut_and_somchaip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/soundex/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/soundex/udom83.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.625979 pythainlp-5.0.3/pythainlp/spell/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/spell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/spell/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/spell/phunspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/spell/pn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/spell/symspellpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/spell/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/spell/wanchanberta_thai_grammarly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.625979 pythainlp-5.0.3/pythainlp/summarize/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/summarize/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/summarize/freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/summarize/keybert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/summarize/mt5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.629979 pythainlp-5.0.3/pythainlp/tag/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/_tag_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/crfchunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/orchid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/pos_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/thai_nner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/thainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/unigram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tag/wangchanberta_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.633979 pythainlp-5.0.3/pythainlp/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/attacut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31383 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/crfcls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/crfcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/deepcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/etcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/han_solo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/longest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/multi_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/nercut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/newmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/nlpo3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/oskut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/sefr_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/ssg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/tcc_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/thaisumcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tokenize/wtsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.633979 pythainlp-5.0.3/pythainlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tools/misspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/tools/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.633979 pythainlp-5.0.3/pythainlp/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/translate/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/translate/en_th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/translate/small100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/translate/th_fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/translate/tokenization_small100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/translate/zh_th.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.633979 pythainlp-5.0.3/pythainlp/transliterate/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/iso_11940.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/royin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/spoonerism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/thai2rom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/thai2rom_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/thaig2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/w2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/transliterate/wunsen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.637979 pythainlp-5.0.3/pythainlp/ulmfit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/ulmfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/ulmfit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/ulmfit/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/ulmfit/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.637979 pythainlp-5.0.3/pythainlp/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/abbreviation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/digitconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93458 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/emojiconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/morse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/numtoword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/phoneme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/pronounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/remove_trailing_repeat_consonants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/spell_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/syllable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/thai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/util/wordtonum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.637979 pythainlp-5.0.3/pythainlp/wangchanberta/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/wangchanberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/wangchanberta/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.637979 pythainlp-5.0.3/pythainlp/word_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/word_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/word_vector/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.641979 pythainlp-5.0.3/pythainlp/wsd/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/wsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-12 10:30:16.000000 pythainlp-5.0.3/pythainlp/wsd/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.617979 pythainlp-5.0.3/pythainlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-12 10:30:24.000000 pythainlp-5.0.3/pythainlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-12 10:30:24.000000 pythainlp-5.0.3/pythainlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 10:30:24.000000 pythainlp-5.0.3/pythainlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 10:30:24.000000 pythainlp-5.0.3/pythainlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 10:30:24.000000 pythainlp-5.0.3/pythainlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-12 10:30:24.000000 pythainlp-5.0.3/pythainlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 10:30:24.000000 pythainlp-5.0.3/pythainlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-12 10:30:24.645979 pythainlp-5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-05-12 10:30:16.000000 pythainlp-5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.641979 pythainlp-5.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:30:24.645979 pythainlp-5.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/data/eval-details-input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/data/eval-input.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/data/input.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/data/sentences.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_ancient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_coref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_el.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_khavee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_morpheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_soundex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_spell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58154 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_ulmfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38788 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_wangchanberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_word_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-12 10:30:16.000000 pythainlp-5.0.3/tests/test_wsd.py
```

### Comparing `pythainlp-5.0.2/CONTRIBUTING.md` & `pythainlp-5.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/LICENSE` & `pythainlp-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/PKG-INFO` & `pythainlp-5.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 5.0.2
+Version: 5.0.3
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pythainlp.github.io/docs/5.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
```

### Comparing `pythainlp-5.0.2/README.md` & `pythainlp-5.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ## News
 
 > Now, You can contact with or ask any questions of the PyThaiNLP team. <a href="https://matrix.to/#/#thainlp:matrix.org" rel="noopener" target="_blank"><img src="https://matrix.to/img/matrix-badge.svg" alt="Chat on Matrix"></a>
 
 | Version | Description | Status |
 |:------:|:--:|:------:|
-| [5.0.2](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [5.0.3](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
 | [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.1 | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/900) |
 
 ## Getting Started
 
 - PyThaiNLP 2 requires Python 3.7+. Python 2.7 users can use PyThaiNLP 1.6. See [2.0 change log](https://github.com/PyThaiNLP/pythainlp/issues/118) | [Upgrading from 1.7](https://pythainlp.github.io/docs/2.0/notes/pythainlp-1_7-2_0.html) | [Upgrading ThaiNER from 1.7](https://github.com/PyThaiNLP/pythainlp/wiki/Upgrade-ThaiNER-from-PyThaiNLP-1.7-to-PyThaiNLP-2.0)
 - [PyThaiNLP Get Started notebook](https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html) | [API document](https://pythainlp.github.io/docs) | [Tutorials](https://pythainlp.github.io/tutorials)
 - [Official website](https://pythainlp.github.io/) | [PyPI](https://pypi.org/project/pythainlp/) | [Facebook page](https://www.facebook.com/pythainlp/)
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 PyThaiNLP
 à¹à¸à¹à¸à¹à¸¥à¸à¸²à¸£à¸µà¸ à¸²à¸©à¸²à¹à¸à¸à¸­à¸à¸ªà¸³à¸«à¸£à¸±à¸à¸à¸£à¸°à¸¡à¸§à¸¥à¸à¸¥à¸ à¸²à¸©à¸²à¸à¸£à¸£à¸¡à¸à¸²à¸à¸´
 à¸à¸¥à¹à¸²à¸¢à¸à¸±à¸ NLTK à¹à¸à¸¢à¹à¸à¹à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢
 [à¸à¸¹à¸£à¸²à¸¢à¸¥à¸°à¹à¸­à¸µà¸¢à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢à¹à¸à¹à¸à¸µà¹
 README_TH.MD](https://github.com/PyThaiNLP/pythainlp/blob/dev/README_TH.md) ##
 News > Now, You can contact with or ask any questions of the PyThaiNLP team.
 _[_C_h_a_t_ _o_n_ _M_a_t_r_i_x_]| Version | Description | Status | |:------:|:--:|:------:| |
-[5.0.2](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change
+[5.0.3](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change
 Log](https://github.com/PyThaiNLP/pythainlp/issues/788) | | [`dev`](https://
 github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.1 | [Change
 Log](https://github.com/PyThaiNLP/pythainlp/issues/900) | ## Getting Started -
 PyThaiNLP 2 requires Python 3.7+. Python 2.7 users can use PyThaiNLP 1.6. See
 [2.0 change log](https://github.com/PyThaiNLP/pythainlp/issues/118) |
 [Upgrading from 1.7](https://pythainlp.github.io/docs/2.0/notes/pythainlp-1_7-
 2_0.html) | [Upgrading ThaiNER from 1.7](https://github.com/PyThaiNLP/
```

### Comparing `pythainlp-5.0.2/README_TH.md` & `pythainlp-5.0.3/README_TH.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ## ข่าวสาร
 
 > คุณสามารถพูดคุยหรือแชทกับทีม PyThaiNLP หรือผู้สนับสนุนคนอื่น ๆ ได้ที่ <a href="https://matrix.to/#/#thainlp:matrix.org" rel="noopener" target="_blank"><img src="https://matrix.to/img/matrix-badge.svg" alt="Chat on Matrix"></a>
 
 | รุ่น | คำอธิบาย | สถานะ |
 |:------:|:--:|:------:|
-| [5.0.2](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [5.0.3](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
 | [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 5.1  | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/900) |
 
 ติดตามพวกเราบน [PyThaiNLP Facebook page](https://www.facebook.com/pythainlp/) เพื่อรับข่าวสารเพิ่มเติม
 
 ## เริ่มต้นกับ PyThaiNLP
 
 พวกเราได้จัดทำ [PyThaiNLP Get Started Tutorial](https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html) สำหรับสำรวจความสามารถของ PyThaiNLP; พวกเรามีเอกสารสอนใช้งาน สามารถศึกษาได้ที่ [หน้า tutorial](https://pythainlp.github.io/tutorials).
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
                  _B_a_d_g_e_]_[_F_O_S_S_A_ _S_t_a_t_u_s_]_[_G_o_o_g_l_e_ _C_o_l_a_b_ _B_a_d_g_e_]_[_D_O_I_]
 PyThaiNLP
 à¹à¸à¹à¸à¹à¸¥à¸à¸²à¸£à¸µà¸ à¸²à¸©à¸²à¹à¸à¸à¸­à¸à¸ªà¸³à¸«à¸£à¸±à¸à¸à¸£à¸°à¸¡à¸§à¸¥à¸à¸¥à¸ à¸²à¸©à¸²à¸à¸£à¸£à¸¡à¸à¸²à¸à¸´
 à¹à¸à¸¢à¹à¸à¹à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢ ## à¸à¹à¸²à¸§à¸ªà¸²à¸£ >
 à¸à¸¸à¸à¸ªà¸²à¸¡à¸²à¸£à¸à¸à¸¹à¸à¸à¸¸à¸¢à¸«à¸£à¸·à¸­à¹à¸à¸à¸à¸±à¸à¸à¸µà¸¡
 PyThaiNLP à¸«à¸£à¸·à¸­à¸à¸¹à¹à¸ªà¸à¸±à¸à¸ªà¸à¸¸à¸à¸à¸à¸­à¸·à¹à¸ à¹
 à¹à¸à¹à¸à¸µà¹ _[_C_h_a_t_ _o_n_ _M_a_t_r_i_x_]| à¸£à¸¸à¹à¸ | à¸à¸³à¸­à¸à¸´à¸à¸²à¸¢ |
-à¸ªà¸à¸²à¸à¸° | |:------:|:--:|:------:| | [5.0.2](https://github.com/
+à¸ªà¸à¸²à¸à¸° | |:------:|:--:|:------:| | [5.0.3](https://github.com/
 PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/
 PyThaiNLP/pythainlp/issues/788) | | [`dev`](https://github.com/PyThaiNLP/
 pythainlp/tree/dev) | Release Candidate for 5.1 | [Change Log](https://
 github.com/PyThaiNLP/pythainlp/issues/900) |
 à¸à¸´à¸à¸à¸²à¸¡à¸à¸§à¸à¹à¸£à¸²à¸à¸ [PyThaiNLP Facebook page](https://
 www.facebook.com/pythainlp/
 ) à¹à¸à¸·à¹à¸­à¸£à¸±à¸à¸à¹à¸²à¸§à¸ªà¸²à¸£à¹à¸à¸´à¹à¸¡à¹à¸à¸´à¸¡ ##
```

### Comparing `pythainlp-5.0.2/pythainlp/__init__.py` & `pythainlp-5.0.3/pythainlp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # SPDX-FileCopyrightText: 2016-2024 PyThaiNLP Project
 # SPDX-License-Identifier: Apache-2.0
-__version__ = "5.0.2"
+__version__ = "5.0.3"
 
 thai_consonants = "กขฃคฅฆงจฉชซฌญฎฏฐฑฒณดตถทธนบปผฝพฟภมยรลวศษสหฬอฮ"  # 44 chars
 
 thai_vowels = (
     "\u0e24\u0e26\u0e30\u0e31\u0e32\u0e33\u0e34\u0e35\u0e36\u0e37"
     + "\u0e38\u0e39\u0e40\u0e41\u0e42\u0e43\u0e44\u0e45\u0e4d\u0e47"
 )  # 20
```

### Comparing `pythainlp-5.0.2/pythainlp/__main__.py` & `pythainlp-5.0.3/pythainlp/__main__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/ancient/aksonhan.py` & `pythainlp-5.0.3/pythainlp/ancient/aksonhan.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/lm/fasttext.py` & `pythainlp-5.0.3/pythainlp/augment/lm/fasttext.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/lm/phayathaibert.py` & `pythainlp-5.0.3/pythainlp/augment/lm/phayathaibert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/lm/wangchanberta.py` & `pythainlp-5.0.3/pythainlp/augment/lm/wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/word2vec/bpemb_wv.py` & `pythainlp-5.0.3/pythainlp/augment/word2vec/bpemb_wv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/word2vec/core.py` & `pythainlp-5.0.3/pythainlp/augment/word2vec/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/word2vec/ltw2v.py` & `pythainlp-5.0.3/pythainlp/augment/word2vec/ltw2v.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/word2vec/thai2fit.py` & `pythainlp-5.0.3/pythainlp/augment/word2vec/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/augment/wordnet.py` & `pythainlp-5.0.3/pythainlp/augment/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/benchmarks/word_tokenization.py` & `pythainlp-5.0.3/pythainlp/benchmarks/word_tokenization.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/chat/core.py` & `pythainlp-5.0.3/pythainlp/chat/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/classify/param_free.py` & `pythainlp-5.0.3/pythainlp/classify/param_free.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/cli/__init__.py` & `pythainlp-5.0.3/pythainlp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/cli/benchmark.py` & `pythainlp-5.0.3/pythainlp/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/cli/data.py` & `pythainlp-5.0.3/pythainlp/cli/data.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/cli/soundex.py` & `pythainlp-5.0.3/pythainlp/cli/soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/cli/tag.py` & `pythainlp-5.0.3/pythainlp/cli/tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/cli/tokenize.py` & `pythainlp-5.0.3/pythainlp/cli/tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/coref/_fastcoref.py` & `pythainlp-5.0.3/pythainlp/coref/_fastcoref.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/coref/core.py` & `pythainlp-5.0.3/pythainlp/coref/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/__init__.py` & `pythainlp-5.0.3/pythainlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/common.py` & `pythainlp-5.0.3/pythainlp/corpus/common.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/conceptnet.py` & `pythainlp-5.0.3/pythainlp/corpus/conceptnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/core.py` & `pythainlp-5.0.3/pythainlp/corpus/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/icu.py` & `pythainlp-5.0.3/pythainlp/corpus/icu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/oscar.py` & `pythainlp-5.0.3/pythainlp/corpus/oscar.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/th_en_translit.py` & `pythainlp-5.0.3/pythainlp/corpus/th_en_translit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/tnc.py` & `pythainlp-5.0.3/pythainlp/corpus/tnc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/ttc.py` & `pythainlp-5.0.3/pythainlp/corpus/ttc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/util.py` & `pythainlp-5.0.3/pythainlp/corpus/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,35 +86,35 @@
     :param Iterable[Iterable[str]] training_data: tokenized text, to be used\
         as a training set
     :return: words that are considered to make `tokenize` perform badly
     :rtype: Set[str]
 
     :Example::
     ::
+    
+        from pythainlp.corpus import thai_words
+        from pythainlp.corpus.util import revise_wordset
+        from pythainlp.tokenize.longest import segment
+
+        base_words = thai_words()
+        more_words = {
+            "ถวิล อุดล", "ทองอินทร์ ภูริพัฒน์", "เตียง ศิริขันธ์", "จำลอง ดาวเรือง"
+        }
+        base_words = base_words.union(more_words)
+        dict_trie = Trie(wordlist)
+
+        tokenize = lambda text: segment(text, dict_trie)
+
+        training_data = [
+            [str, str, str. ...],
+            [str, str, str, str, ...],
+            ...
+        ]
 
-    from pythainlp.corpus import thai_words
-    from pythainlp.corpus.util import revise_wordset
-    from pythainlp.tokenize.longest import segment
-
-    base_words = thai_words()
-    more_words = {
-        "ถวิล อุดล", "ทองอินทร์ ภูริพัฒน์", "เตียง ศิริขันธ์", "จำลอง ดาวเรือง"
-    }
-    base_words = base_words.union(more_words)
-    dict_trie = Trie(wordlist)
-
-    tokenize = lambda text: segment(text, dict_trie)
-
-    training_data = [
-        [str, str, str. ...],
-        [str, str, str, str, ...],
-        ...
-    ]
-
-    revised_words = revise_wordset(tokenize, wordlist, training_data)
+        revised_words = revise_wordset(tokenize, wordlist, training_data)
     """
     bad_words = find_badwords(tokenize, training_data)
     return set(orig_words) - bad_words
 
 
 def revise_newmm_default_wordset(
     training_data: Iterable[Iterable[str]],
```

### Comparing `pythainlp-5.0.2/pythainlp/corpus/volubilis.py` & `pythainlp-5.0.3/pythainlp/corpus/volubilis.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/wikipedia.py` & `pythainlp-5.0.3/pythainlp/corpus/wikipedia.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/corpus/wordnet.py` & `pythainlp-5.0.3/pythainlp/corpus/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/el/_multiel.py` & `pythainlp-5.0.3/pythainlp/el/_multiel.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/el/core.py` & `pythainlp-5.0.3/pythainlp/el/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/generate/core.py` & `pythainlp-5.0.3/pythainlp/generate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/generate/thai2fit.py` & `pythainlp-5.0.3/pythainlp/generate/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/generate/wangchanglm.py` & `pythainlp-5.0.3/pythainlp/generate/wangchanglm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/khavee/core.py` & `pythainlp-5.0.3/pythainlp/khavee/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/khavee/example.py` & `pythainlp-5.0.3/pythainlp/khavee/example.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/morpheme/thaiwordcheck.py` & `pythainlp-5.0.3/pythainlp/morpheme/thaiwordcheck.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/morpheme/word_formation.py` & `pythainlp-5.0.3/pythainlp/morpheme/word_formation.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/parse/core.py` & `pythainlp-5.0.3/pythainlp/parse/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/parse/esupar_engine.py` & `pythainlp-5.0.3/pythainlp/parse/esupar_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/parse/spacy_thai_engine.py` & `pythainlp-5.0.3/pythainlp/parse/spacy_thai_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/parse/transformers_ud.py` & `pythainlp-5.0.3/pythainlp/parse/transformers_ud.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/parse/ud_goeswith.py` & `pythainlp-5.0.3/pythainlp/parse/ud_goeswith.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/phayathaibert/core.py` & `pythainlp-5.0.3/pythainlp/phayathaibert/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/soundex/__init__.py` & `pythainlp-5.0.3/pythainlp/soundex/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/soundex/core.py` & `pythainlp-5.0.3/pythainlp/soundex/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/soundex/lk82.py` & `pythainlp-5.0.3/pythainlp/soundex/lk82.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/soundex/metasound.py` & `pythainlp-5.0.3/pythainlp/soundex/metasound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/soundex/prayut_and_somchaip.py` & `pythainlp-5.0.3/pythainlp/soundex/prayut_and_somchaip.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/soundex/sound.py` & `pythainlp-5.0.3/pythainlp/soundex/sound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/soundex/udom83.py` & `pythainlp-5.0.3/pythainlp/soundex/udom83.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/spell/core.py` & `pythainlp-5.0.3/pythainlp/spell/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/spell/pn.py` & `pythainlp-5.0.3/pythainlp/spell/pn.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/spell/symspellpy.py` & `pythainlp-5.0.3/pythainlp/spell/symspellpy.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/spell/wanchanberta_thai_grammarly.py` & `pythainlp-5.0.3/pythainlp/spell/wanchanberta_thai_grammarly.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/summarize/core.py` & `pythainlp-5.0.3/pythainlp/summarize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/summarize/freq.py` & `pythainlp-5.0.3/pythainlp/summarize/freq.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/summarize/keybert.py` & `pythainlp-5.0.3/pythainlp/summarize/keybert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/summarize/mt5.py` & `pythainlp-5.0.3/pythainlp/summarize/mt5.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/__init__.py` & `pythainlp-5.0.3/pythainlp/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/_tag_perceptron.py` & `pythainlp-5.0.3/pythainlp/tag/_tag_perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/blackboard.py` & `pythainlp-5.0.3/pythainlp/tag/blackboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/chunk.py` & `pythainlp-5.0.3/pythainlp/tag/chunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/crfchunk.py` & `pythainlp-5.0.3/pythainlp/tag/crfchunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/locations.py` & `pythainlp-5.0.3/pythainlp/tag/locations.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/named_entity.py` & `pythainlp-5.0.3/pythainlp/tag/named_entity.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/orchid.py` & `pythainlp-5.0.3/pythainlp/tag/orchid.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/perceptron.py` & `pythainlp-5.0.3/pythainlp/tag/perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/pos_tag.py` & `pythainlp-5.0.3/pythainlp/tag/pos_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/thainer.py` & `pythainlp-5.0.3/pythainlp/tag/thainer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/tltk.py` & `pythainlp-5.0.3/pythainlp/tag/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/unigram.py` & `pythainlp-5.0.3/pythainlp/tag/unigram.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tag/wangchanberta_onnx.py` & `pythainlp-5.0.3/pythainlp/tag/wangchanberta_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/__init__.py` & `pythainlp-5.0.3/pythainlp/tokenize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/_utils.py` & `pythainlp-5.0.3/pythainlp/tokenize/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         token = segments[segment_idx]
         if is_span_beginning:
             connected_token = ""
             while pos < match.end() and segment_idx < len(segments):
                 connected_token += segments[segment_idx]
                 pos += len(segments[segment_idx])
                 segment_idx += 1
-
-            tokens_joined.append(connected_token)
+            if connected_token:
+                tokens_joined.append(connected_token)
             match = next(matching_results, None)
         else:
             tokens_joined.append(token)
             segment_idx += 1
             pos += len(token)
     tokens_joined += segments[segment_idx:]
     return tokens_joined
```

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/attacut.py` & `pythainlp-5.0.3/pythainlp/tokenize/attacut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/core.py` & `pythainlp-5.0.3/pythainlp/tokenize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/crfcls.py` & `pythainlp-5.0.3/pythainlp/tokenize/crfcls.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/crfcut.py` & `pythainlp-5.0.3/pythainlp/tokenize/crfcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/deepcut.py` & `pythainlp-5.0.3/pythainlp/tokenize/deepcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/etcc.py` & `pythainlp-5.0.3/pythainlp/tokenize/etcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/han_solo.py` & `pythainlp-5.0.3/pythainlp/tokenize/han_solo.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/longest.py` & `pythainlp-5.0.3/pythainlp/tokenize/longest.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/multi_cut.py` & `pythainlp-5.0.3/pythainlp/tokenize/multi_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/nercut.py` & `pythainlp-5.0.3/pythainlp/tokenize/nercut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/newmm.py` & `pythainlp-5.0.3/pythainlp/tokenize/newmm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/nlpo3.py` & `pythainlp-5.0.3/pythainlp/tokenize/nlpo3.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/oskut.py` & `pythainlp-5.0.3/pythainlp/tokenize/oskut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/pyicu.py` & `pythainlp-5.0.3/pythainlp/tokenize/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/sefr_cut.py` & `pythainlp-5.0.3/pythainlp/tokenize/sefr_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/tcc.py` & `pythainlp-5.0.3/pythainlp/tokenize/tcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/tcc_p.py` & `pythainlp-5.0.3/pythainlp/tokenize/tcc_p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/thaisumcut.py` & `pythainlp-5.0.3/pythainlp/tokenize/thaisumcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/tltk.py` & `pythainlp-5.0.3/pythainlp/tokenize/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tokenize/wtsplit.py` & `pythainlp-5.0.3/pythainlp/tokenize/wtsplit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tools/misspell.py` & `pythainlp-5.0.3/pythainlp/tools/misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/tools/path.py` & `pythainlp-5.0.3/pythainlp/tools/path.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/translate/core.py` & `pythainlp-5.0.3/pythainlp/translate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/translate/en_th.py` & `pythainlp-5.0.3/pythainlp/translate/en_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/translate/small100.py` & `pythainlp-5.0.3/pythainlp/translate/small100.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/translate/th_fr.py` & `pythainlp-5.0.3/pythainlp/translate/th_fr.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/translate/tokenization_small100.py` & `pythainlp-5.0.3/pythainlp/translate/tokenization_small100.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/translate/zh_th.py` & `pythainlp-5.0.3/pythainlp/translate/zh_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/core.py` & `pythainlp-5.0.3/pythainlp/transliterate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/ipa.py` & `pythainlp-5.0.3/pythainlp/transliterate/ipa.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/iso_11940.py` & `pythainlp-5.0.3/pythainlp/transliterate/iso_11940.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/lookup.py` & `pythainlp-5.0.3/pythainlp/transliterate/lookup.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/pyicu.py` & `pythainlp-5.0.3/pythainlp/transliterate/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/royin.py` & `pythainlp-5.0.3/pythainlp/transliterate/royin.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/spoonerism.py` & `pythainlp-5.0.3/pythainlp/transliterate/spoonerism.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/thai2rom.py` & `pythainlp-5.0.3/pythainlp/transliterate/thai2rom.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/thai2rom_onnx.py` & `pythainlp-5.0.3/pythainlp/transliterate/thai2rom_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/thaig2p.py` & `pythainlp-5.0.3/pythainlp/transliterate/thaig2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/tltk.py` & `pythainlp-5.0.3/pythainlp/transliterate/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/w2p.py` & `pythainlp-5.0.3/pythainlp/transliterate/w2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/transliterate/wunsen.py` & `pythainlp-5.0.3/pythainlp/transliterate/wunsen.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/ulmfit/__init__.py` & `pythainlp-5.0.3/pythainlp/ulmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/ulmfit/core.py` & `pythainlp-5.0.3/pythainlp/ulmfit/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/ulmfit/preprocess.py` & `pythainlp-5.0.3/pythainlp/ulmfit/preprocess.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/ulmfit/tokenizer.py` & `pythainlp-5.0.3/pythainlp/ulmfit/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/__init__.py` & `pythainlp-5.0.3/pythainlp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/abbreviation.py` & `pythainlp-5.0.3/pythainlp/util/abbreviation.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/collate.py` & `pythainlp-5.0.3/pythainlp/util/collate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/date.py` & `pythainlp-5.0.3/pythainlp/util/date.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 ):
     """
     Thai strptime
 
     :param str text: text
     :param str fmt: string containing date and time directives
     :param str year: year of the text \
-        (ad isAnno Domini and be is Buddhist calendar)
+        (ad is Anno Domini and be is Buddhist Era)
     :param int add_year: add to year when converting to ad
     :param object tzinfo: tzinfo (default is Asia/Bangkok)
     :return: The year that is converted to datetime.datetime
     :rtype: datetime.datetime
 
     The fmt chars that are supported:
         * *%d* - Day (1 - 31)
```

### Comparing `pythainlp-5.0.2/pythainlp/util/digitconv.py` & `pythainlp-5.0.3/pythainlp/util/digitconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/emojiconv.py` & `pythainlp-5.0.3/pythainlp/util/emojiconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/encoding.py` & `pythainlp-5.0.3/pythainlp/util/encoding.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/keyboard.py` & `pythainlp-5.0.3/pythainlp/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/keywords.py` & `pythainlp-5.0.3/pythainlp/util/keywords.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/morse.py` & `pythainlp-5.0.3/pythainlp/util/morse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/normalize.py` & `pythainlp-5.0.3/pythainlp/util/normalize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/numtoword.py` & `pythainlp-5.0.3/pythainlp/util/numtoword.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/phoneme.py` & `pythainlp-5.0.3/pythainlp/util/phoneme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/pronounce.py` & `pythainlp-5.0.3/pythainlp/util/pronounce.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/remove_trailing_repeat_consonants.py` & `pythainlp-5.0.3/pythainlp/util/remove_trailing_repeat_consonants.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/spell_words.py` & `pythainlp-5.0.3/pythainlp/util/spell_words.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/strftime.py` & `pythainlp-5.0.3/pythainlp/util/strftime.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/syllable.py` & `pythainlp-5.0.3/pythainlp/util/syllable.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/thai.py` & `pythainlp-5.0.3/pythainlp/util/thai.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/time.py` & `pythainlp-5.0.3/pythainlp/util/time.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/trie.py` & `pythainlp-5.0.3/pythainlp/util/trie.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/util/wordtonum.py` & `pythainlp-5.0.3/pythainlp/util/wordtonum.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/wangchanberta/core.py` & `pythainlp-5.0.3/pythainlp/wangchanberta/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/word_vector/core.py` & `pythainlp-5.0.3/pythainlp/word_vector/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp/wsd/core.py` & `pythainlp-5.0.3/pythainlp/wsd/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp.egg-info/PKG-INFO` & `pythainlp-5.0.3/pythainlp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 5.0.2
+Version: 5.0.3
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pythainlp.github.io/docs/5.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
```

### Comparing `pythainlp-5.0.2/pythainlp.egg-info/SOURCES.txt` & `pythainlp-5.0.3/pythainlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/pythainlp.egg-info/requires.txt` & `pythainlp-5.0.3/pythainlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/setup.cfg` & `pythainlp-5.0.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 5.0.2
+current_version = 5.0.3
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `pythainlp-5.0.2/setup.py` & `pythainlp-5.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         "sentence-transformers>=2.2.2",
         "khamyo>=0.2.0",
     ],
 }
 
 setup(
     name="pythainlp",
-    version="5.0.2",
+    version="5.0.3",
     description="Thai Natural Language Processing library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="PyThaiNLP",
     author_email="email@wannaphong.com",
     url="https://github.com/PyThaiNLP/pythainlp",
     packages=find_packages(exclude=["tests", "tests.*"]),
```

### Comparing `pythainlp-5.0.2/tests/data/eval-details-input.json` & `pythainlp-5.0.3/tests/data/eval-details-input.json`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/data/sentences.yml` & `pythainlp-5.0.3/tests/data/sentences.yml`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_ancient.py` & `pythainlp-5.0.3/tests/test_ancient.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_augment.py` & `pythainlp-5.0.3/tests/test_augment.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_benchmarks.py` & `pythainlp-5.0.3/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_classify.py` & `pythainlp-5.0.3/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_cli.py` & `pythainlp-5.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_coref.py` & `pythainlp-5.0.3/tests/test_coref.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_corpus.py` & `pythainlp-5.0.3/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_generate.py` & `pythainlp-5.0.3/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_khavee.py` & `pythainlp-5.0.3/tests/test_khavee.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_misspell.py` & `pythainlp-5.0.3/tests/test_misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_morpheme.py` & `pythainlp-5.0.3/tests/test_morpheme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_parse.py` & `pythainlp-5.0.3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_soundex.py` & `pythainlp-5.0.3/tests/test_soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_spell.py` & `pythainlp-5.0.3/tests/test_spell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_summarize.py` & `pythainlp-5.0.3/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_tag.py` & `pythainlp-5.0.3/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_tokenize.py` & `pythainlp-5.0.3/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_tools.py` & `pythainlp-5.0.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_translate.py` & `pythainlp-5.0.3/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_transliterate.py` & `pythainlp-5.0.3/tests/test_transliterate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_ulmfit.py` & `pythainlp-5.0.3/tests/test_ulmfit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_util.py` & `pythainlp-5.0.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_wangchanberta.py` & `pythainlp-5.0.3/tests/test_wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_word_vector.py` & `pythainlp-5.0.3/tests/test_word_vector.py`

 * *Files identical despite different names*

### Comparing `pythainlp-5.0.2/tests/test_wsd.py` & `pythainlp-5.0.3/tests/test_wsd.py`

 * *Files identical despite different names*

